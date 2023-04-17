# Comparing `tmp/nml-0.7.2.tar.gz` & `tmp/nml-r1512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nml-0.7.2.tar", last modified: Mon Apr 17 19:55:21 2023, max compression
+gzip compressed data, was "nml-r1512.tar", last modified: Fri Jul  8 21:18:54 2011, max compression, from Unix
```

## Comparing `nml-0.7.2.tar` & `nml-r1512.tar`

### file list

```diff
@@ -1,355 +1,227 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.340185 nml-0.7.2/
--rw-r--r--   0 runner     (501) staff       (20)    17988 2023-04-17 19:54:52.000000 nml-0.7.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      756 2023-04-17 19:54:52.000000 nml-0.7.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      520 2023-04-17 19:54:52.000000 nml-0.7.2/Makefile
--rw-r--r--   0 runner     (501) staff       (20)      995 2023-04-17 19:55:21.339739 nml-0.7.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6369 2023-04-17 19:54:52.000000 nml-0.7.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.167341 nml-0.7.2/docs/
--rw-r--r--   0 runner     (501) staff       (20)    33048 2023-04-17 19:54:52.000000 nml-0.7.2/docs/changelog.txt
--rw-r--r--   0 runner     (501) staff       (20)      668 2023-04-17 19:54:52.000000 nml-0.7.2/docs/index.html
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-17 19:54:52.000000 nml-0.7.2/docs/nml.spec
--rw-r--r--   0 runner     (501) staff       (20)     2802 2023-04-17 19:54:52.000000 nml-0.7.2/docs/nmlc.1
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.158588 nml-0.7.2/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.167934 nml-0.7.2/examples/industry/
--rw-r--r--   0 runner     (501) staff       (20)     4485 2023-04-17 19:54:52.000000 nml-0.7.2/examples/industry/example_industry.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.168444 nml-0.7.2/examples/industry/lang/
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-17 19:54:52.000000 nml-0.7.2/examples/industry/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.169311 nml-0.7.2/examples/object/
--rw-r--r--   0 runner     (501) staff       (20)     5619 2023-04-17 19:54:52.000000 nml-0.7.2/examples/object/cc_grid.png
--rw-r--r--   0 runner     (501) staff       (20)     6213 2023-04-17 19:54:52.000000 nml-0.7.2/examples/object/example_object.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.169741 nml-0.7.2/examples/object/lang/
--rw-r--r--   0 runner     (501) staff       (20)      716 2023-04-17 19:54:52.000000 nml-0.7.2/examples/object/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.170146 nml-0.7.2/examples/railtype/
--rw-r--r--   0 runner     (501) staff       (20)    11842 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/example_railtype.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.175777 nml-0.7.2/examples/railtype/gfx/
--rw-r--r--   0 runner     (501) staff       (20)     3384 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/depot_electric.png
--rw-r--r--   0 runner     (501) staff       (20)     3264 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/depot_normal.png
--rw-r--r--   0 runner     (501) staff       (20)     1891 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/fences.png
--rw-r--r--   0 runner     (501) staff       (20)     3983 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/gui_erail.png
--rw-r--r--   0 runner     (501) staff       (20)     3507 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/gui_rail.png
--rw-r--r--   0 runner     (501) staff       (20)     3834 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/lc_left.png
--rw-r--r--   0 runner     (501) staff       (20)     4024 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/lc_right.png
--rw-r--r--   0 runner     (501) staff       (20)     7668 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/rails_overlays.png
--rw-r--r--   0 runner     (501) staff       (20)     1640 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/gfx/tunnel_track.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.176201 nml-0.7.2/examples/railtype/lang/
--rw-r--r--   0 runner     (501) staff       (20)      476 2023-04-17 19:54:52.000000 nml-0.7.2/examples/railtype/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.176612 nml-0.7.2/examples/road_vehicle/
--rw-r--r--   0 runner     (501) staff       (20)    14820 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/example_road_vehicle.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.179530 nml-0.7.2/examples/road_vehicle/gfx/
--rw-r--r--   0 runner     (501) staff       (20)     2098 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/gfx/flatbed_truck_1_copper.png
--rw-r--r--   0 runner     (501) staff       (20)     2066 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/gfx/flatbed_truck_1_goods.png
--rw-r--r--   0 runner     (501) staff       (20)     2111 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/gfx/flatbed_truck_1_paper.png
--rw-r--r--   0 runner     (501) staff       (20)     2109 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/gfx/flatbed_truck_1_steel.png
--rw-r--r--   0 runner     (501) staff       (20)     2261 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/gfx/flatbed_truck_1_wood.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.180051 nml-0.7.2/examples/road_vehicle/lang/
--rw-r--r--   0 runner     (501) staff       (20)     1000 2023-04-17 19:54:52.000000 nml-0.7.2/examples/road_vehicle/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.180602 nml-0.7.2/examples/roadtype_and_tramtype/
--rw-r--r--   0 runner     (501) staff       (20)    10042 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/example_roadtype_and_tramtype.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.187855 nml-0.7.2/examples/roadtype_and_tramtype/gfx/
--rw-r--r--   0 runner     (501) staff       (20)     3384 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/depot_electric.png
--rw-r--r--   0 runner     (501) staff       (20)     3264 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/depot_normal.png
--rw-r--r--   0 runner     (501) staff       (20)     1891 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/fences.png
--rw-r--r--   0 runner     (501) staff       (20)     3983 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/gui_erail.png
--rw-r--r--   0 runner     (501) staff       (20)     3507 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/gui_rail.png
--rw-r--r--   0 runner     (501) staff       (20)     3834 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/lc_left.png
--rw-r--r--   0 runner     (501) staff       (20)     4024 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/lc_right.png
--rw-r--r--   0 runner     (501) staff       (20)     7668 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/rails_overlays.png
--rw-r--r--   0 runner     (501) staff       (20)    11142 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/roads_blue.png
--rw-r--r--   0 runner     (501) staff       (20)    11137 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/roads_red.png
--rw-r--r--   0 runner     (501) staff       (20)    10029 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/roads_underlay.png
--rw-r--r--   0 runner     (501) staff       (20)    11143 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/roads_yellow.png
--rw-r--r--   0 runner     (501) staff       (20)     9850 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/tram_green.png
--rw-r--r--   0 runner     (501) staff       (20)     1640 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/gfx/tunnel_track.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.188682 nml-0.7.2/examples/roadtype_and_tramtype/lang/
--rw-r--r--   0 runner     (501) staff       (20)     2799 2023-04-17 19:54:52.000000 nml-0.7.2/examples/roadtype_and_tramtype/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.189512 nml-0.7.2/examples/station/
--rw-r--r--   0 runner     (501) staff       (20)     2087 2023-04-17 19:54:52.000000 nml-0.7.2/examples/station/cows_cargo.png
--rw-r--r--   0 runner     (501) staff       (20)     3661 2023-04-17 19:54:52.000000 nml-0.7.2/examples/station/example_station.nml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.189920 nml-0.7.2/examples/station/lang/
--rw-r--r--   0 runner     (501) staff       (20)      589 2023-04-17 19:54:52.000000 nml-0.7.2/examples/station/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.193615 nml-0.7.2/examples/train/
--rw-r--r--   0 runner     (501) staff       (20)    17048 2023-04-17 19:54:52.000000 nml-0.7.2/examples/train/cargo_wagons.png
--rw-r--r--   0 runner     (501) staff       (20)    14420 2023-04-17 19:54:52.000000 nml-0.7.2/examples/train/example_train.nml
--rw-r--r--   0 runner     (501) staff       (20)     4074 2023-04-17 19:54:52.000000 nml-0.7.2/examples/train/icm.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.194479 nml-0.7.2/examples/train/lang/
--rw-r--r--   0 runner     (501) staff       (20)     1645 2023-04-17 19:54:52.000000 nml-0.7.2/examples/train/lang/dutch.lng
--rw-r--r--   0 runner     (501) staff       (20)     1664 2023-04-17 19:54:52.000000 nml-0.7.2/examples/train/lang/english.lng
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.210389 nml-0.7.2/nml/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-17 19:54:52.000000 nml-0.7.2/nml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       59 2023-04-17 19:55:20.000000 nml-0.7.2/nml/__version__.py
--rw-r--r--   0 runner     (501) staff       (20)     5871 2023-04-17 19:54:52.000000 nml-0.7.2/nml/_lz77.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.230021 nml-0.7.2/nml/actions/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    42172 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action0.py
--rw-r--r--   0 runner     (501) staff       (20)    60420 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action0properties.py
--rw-r--r--   0 runner     (501) staff       (20)     9352 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action1.py
--rw-r--r--   0 runner     (501) staff       (20)     1084 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action10.py
--rw-r--r--   0 runner     (501) staff       (20)     4152 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action11.py
--rw-r--r--   0 runner     (501) staff       (20)     3168 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action12.py
--rw-r--r--   0 runner     (501) staff       (20)    10145 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action14.py
--rw-r--r--   0 runner     (501) staff       (20)    21198 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2.py
--rw-r--r--   0 runner     (501) staff       (20)    32565 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2layout.py
--rw-r--r--   0 runner     (501) staff       (20)     8200 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2production.py
--rw-r--r--   0 runner     (501) staff       (20)    15547 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2random.py
--rw-r--r--   0 runner     (501) staff       (20)     6280 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2real.py
--rw-r--r--   0 runner     (501) staff       (20)    50007 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2var.py
--rw-r--r--   0 runner     (501) staff       (20)    54896 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action2var_variables.py
--rw-r--r--   0 runner     (501) staff       (20)    26496 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action3.py
--rw-r--r--   0 runner     (501) staff       (20)    18863 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action3_callbacks.py
--rw-r--r--   0 runner     (501) staff       (20)     8487 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action4.py
--rw-r--r--   0 runner     (501) staff       (20)     5685 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action5.py
--rw-r--r--   0 runner     (501) staff       (20)     2018 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action6.py
--rw-r--r--   0 runner     (501) staff       (20)    13129 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action7.py
--rw-r--r--   0 runner     (501) staff       (20)     1465 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/action8.py
--rw-r--r--   0 runner     (501) staff       (20)     2791 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/actionA.py
--rw-r--r--   0 runner     (501) staff       (20)     4264 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/actionB.py
--rw-r--r--   0 runner     (501) staff       (20)    19969 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/actionD.py
--rw-r--r--   0 runner     (501) staff       (20)     1233 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/actionE.py
--rw-r--r--   0 runner     (501) staff       (20)     8576 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/actionF.py
--rw-r--r--   0 runner     (501) staff       (20)     1955 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/base_action.py
--rw-r--r--   0 runner     (501) staff       (20)    26175 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/real_sprite.py
--rw-r--r--   0 runner     (501) staff       (20)      976 2023-04-17 19:54:52.000000 nml-0.7.2/nml/actions/sprite_count.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.245424 nml-0.7.2/nml/ast/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6177 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/alt_sprites.py
--rw-r--r--   0 runner     (501) staff       (20)     3068 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/assignment.py
--rw-r--r--   0 runner     (501) staff       (20)     3742 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/base_graphics.py
--rw-r--r--   0 runner     (501) staff       (20)     6229 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/base_statement.py
--rw-r--r--   0 runner     (501) staff       (20)     7001 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/basecost.py
--rw-r--r--   0 runner     (501) staff       (20)     2328 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/cargotable.py
--rw-r--r--   0 runner     (501) staff       (20)     2944 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/conditional.py
--rw-r--r--   0 runner     (501) staff       (20)     1563 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/deactivate.py
--rw-r--r--   0 runner     (501) staff       (20)     2896 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/disable_item.py
--rw-r--r--   0 runner     (501) staff       (20)     4052 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/error.py
--rw-r--r--   0 runner     (501) staff       (20)     3367 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/font.py
--rw-r--r--   0 runner     (501) staff       (20)     2834 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/general.py
--rw-r--r--   0 runner     (501) staff       (20)    13763 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/grf.py
--rw-r--r--   0 runner     (501) staff       (20)    12030 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/item.py
--rw-r--r--   0 runner     (501) staff       (20)     1949 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/loop.py
--rw-r--r--   0 runner     (501) staff       (20)     2428 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/override.py
--rw-r--r--   0 runner     (501) staff       (20)     6583 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/produce.py
--rw-r--r--   0 runner     (501) staff       (20)     6741 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/replace.py
--rw-r--r--   0 runner     (501) staff       (20)     1204 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/skipall.py
--rw-r--r--   0 runner     (501) staff       (20)     6666 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/snowline.py
--rw-r--r--   0 runner     (501) staff       (20)     2384 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/sort_vehicles.py
--rw-r--r--   0 runner     (501) staff       (20)     3792 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/sprite_container.py
--rw-r--r--   0 runner     (501) staff       (20)    11570 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/spriteblock.py
--rw-r--r--   0 runner     (501) staff       (20)    20513 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/switch.py
--rw-r--r--   0 runner     (501) staff       (20)     5666 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/tilelayout.py
--rw-r--r--   0 runner     (501) staff       (20)    16922 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/townnames.py
--rw-r--r--   0 runner     (501) staff       (20)     4710 2023-04-17 19:54:52.000000 nml-0.7.2/nml/ast/tracktypetable.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.247801 nml-0.7.2/nml/editors/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-17 19:54:52.000000 nml-0.7.2/nml/editors/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5904 2023-04-17 19:54:52.000000 nml-0.7.2/nml/editors/extract_tables.py
--rw-r--r--   0 runner     (501) staff       (20)     7635 2023-04-17 19:54:52.000000 nml-0.7.2/nml/editors/kate.py
--rw-r--r--   0 runner     (501) staff       (20)     4028 2023-04-17 19:54:52.000000 nml-0.7.2/nml/editors/notepadpp.py
--rw-r--r--   0 runner     (501) staff       (20)     5654 2023-04-17 19:54:52.000000 nml-0.7.2/nml/editors/visualstudiocode.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.258037 nml-0.7.2/nml/expression/
--rw-r--r--   0 runner     (501) staff       (20)     1932 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2051 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/abs_op.py
--rw-r--r--   0 runner     (501) staff       (20)     1545 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/array.py
--rw-r--r--   0 runner     (501) staff       (20)     6093 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/base_expression.py
--rw-r--r--   0 runner     (501) staff       (20)     4249 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/bin_not.py
--rw-r--r--   0 runner     (501) staff       (20)    11927 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/binop.py
--rw-r--r--   0 runner     (501) staff       (20)     2170 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/bitmask.py
--rw-r--r--   0 runner     (501) staff       (20)     2103 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/boolean.py
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/cargo.py
--rw-r--r--   0 runner     (501) staff       (20)    27019 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/functioncall.py
--rw-r--r--   0 runner     (501) staff       (20)     2319 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/functionptr.py
--rw-r--r--   0 runner     (501) staff       (20)     3061 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/identifier.py
--rw-r--r--   0 runner     (501) staff       (20)     4583 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/parameter.py
--rw-r--r--   0 runner     (501) staff       (20)     1570 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/patch_variable.py
--rw-r--r--   0 runner     (501) staff       (20)     3251 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/special_parameter.py
--rw-r--r--   0 runner     (501) staff       (20)     3850 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/spritegroup_ref.py
--rw-r--r--   0 runner     (501) staff       (20)     5646 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/storage_op.py
--rw-r--r--   0 runner     (501) staff       (20)     2141 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/string.py
--rw-r--r--   0 runner     (501) staff       (20)     1474 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/string_literal.py
--rw-r--r--   0 runner     (501) staff       (20)     3774 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/ternaryop.py
--rw-r--r--   0 runner     (501) staff       (20)     4072 2023-04-17 19:54:52.000000 nml-0.7.2/nml/expression/variable.py
--rw-r--r--   0 runner     (501) staff       (20)     4732 2023-04-17 19:54:52.000000 nml-0.7.2/nml/free_number_list.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.258483 nml-0.7.2/nml/generated/
--rw-r--r--   0 runner     (501) staff       (20)      315 2023-04-17 19:54:52.000000 nml-0.7.2/nml/generated/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16890 2023-04-17 19:54:52.000000 nml-0.7.2/nml/generic.py
--rw-r--r--   0 runner     (501) staff       (20)    63907 2023-04-17 19:54:52.000000 nml-0.7.2/nml/global_constants.py
--rw-r--r--   0 runner     (501) staff       (20)    49152 2023-04-17 19:54:52.000000 nml-0.7.2/nml/grfstrings.py
--rw-r--r--   0 runner     (501) staff       (20)     2695 2023-04-17 19:54:52.000000 nml-0.7.2/nml/lz77.py
--rw-r--r--   0 runner     (501) staff       (20)    22325 2023-04-17 19:54:52.000000 nml-0.7.2/nml/main.py
--rw-r--r--   0 runner     (501) staff       (20)    12383 2023-04-17 19:54:52.000000 nml-0.7.2/nml/nmlop.py
--rw-r--r--   0 runner     (501) staff       (20)    10014 2023-04-17 19:54:52.000000 nml-0.7.2/nml/output_base.py
--rw-r--r--   0 runner     (501) staff       (20)     1233 2023-04-17 19:54:52.000000 nml-0.7.2/nml/output_dep.py
--rw-r--r--   0 runner     (501) staff       (20)     7587 2023-04-17 19:54:52.000000 nml-0.7.2/nml/output_grf.py
--rw-r--r--   0 runner     (501) staff       (20)     6279 2023-04-17 19:54:52.000000 nml-0.7.2/nml/output_nfo.py
--rw-r--r--   0 runner     (501) staff       (20)     1087 2023-04-17 19:54:52.000000 nml-0.7.2/nml/output_nml.py
--rw-r--r--   0 runner     (501) staff       (20)    21178 2023-04-17 19:54:52.000000 nml-0.7.2/nml/palette.py
--rw-r--r--   0 runner     (501) staff       (20)    29327 2023-04-17 19:54:52.000000 nml-0.7.2/nml/parser.py
--rw-r--r--   0 runner     (501) staff       (20)    12972 2023-04-17 19:54:52.000000 nml-0.7.2/nml/spritecache.py
--rw-r--r--   0 runner     (501) staff       (20)    22099 2023-04-17 19:54:52.000000 nml-0.7.2/nml/spriteencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     9650 2023-04-17 19:54:52.000000 nml-0.7.2/nml/tokens.py
--rw-r--r--   0 runner     (501) staff       (20)     3927 2023-04-17 19:54:52.000000 nml-0.7.2/nml/unit.py
--rw-r--r--   0 runner     (501) staff       (20)     2382 2023-04-17 19:54:52.000000 nml-0.7.2/nml/version_info.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.213338 nml-0.7.2/nml.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      995 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    10219 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       16 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-04-17 19:55:21.000000 nml-0.7.2/nml.egg-info/top_level.txt
--rwxr-xr-x   0 runner     (501) staff       (20)       89 2023-04-17 19:54:52.000000 nml-0.7.2/nmlc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.289345 nml-0.7.2/regression/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-04-17 19:54:52.000000 nml-0.7.2/regression/001_action8.nml
--rw-r--r--   0 runner     (501) staff       (20)      243 2023-04-17 19:54:52.000000 nml-0.7.2/regression/002_sounds.nml
--rw-r--r--   0 runner     (501) staff       (20)      328 2023-04-17 19:54:52.000000 nml-0.7.2/regression/003_assignment.nml
--rw-r--r--   0 runner     (501) staff       (20)      164 2023-04-17 19:54:52.000000 nml-0.7.2/regression/004_deactivate.nml
--rw-r--r--   0 runner     (501) staff       (20)      203 2023-04-17 19:54:52.000000 nml-0.7.2/regression/005_error.nml
--rw-r--r--   0 runner     (501) staff       (20)     3024 2023-04-17 19:54:52.000000 nml-0.7.2/regression/006_vehicle.nml
--rw-r--r--   0 runner     (501) staff       (20)     1202 2023-04-17 19:54:52.000000 nml-0.7.2/regression/007_townnames.nml
--rw-r--r--   0 runner     (501) staff       (20)      158 2023-04-17 19:54:52.000000 nml-0.7.2/regression/008_railtypes.nml
--rw-r--r--   0 runner     (501) staff       (20)      749 2023-04-17 19:54:52.000000 nml-0.7.2/regression/009_replace.nml
--rw-r--r--   0 runner     (501) staff       (20)     2511 2023-04-17 19:54:52.000000 nml-0.7.2/regression/010_liveryoverride.nml
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-17 19:54:52.000000 nml-0.7.2/regression/011_snowline.nml
--rw-r--r--   0 runner     (501) staff       (20)      319 2023-04-17 19:54:52.000000 nml-0.7.2/regression/012_basecost.nml
--rw-r--r--   0 runner     (501) staff       (20)     5079 2023-04-17 19:54:52.000000 nml-0.7.2/regression/013_train_callback.nml
--rw-r--r--   0 runner     (501) staff       (20)     1125 2023-04-17 19:54:52.000000 nml-0.7.2/regression/014_read_special_param.nml
--rw-r--r--   0 runner     (501) staff       (20)     1087 2023-04-17 19:54:52.000000 nml-0.7.2/regression/015_basic_object.nml
--rw-r--r--   0 runner     (501) staff       (20)      551 2023-04-17 19:54:52.000000 nml-0.7.2/regression/016_basic_airporttiles.nml
--rw-r--r--   0 runner     (501) staff       (20)     2416 2023-04-17 19:54:52.000000 nml-0.7.2/regression/017_articulated_tram.nml
--rw-r--r--   0 runner     (501) staff       (20)      544 2023-04-17 19:54:52.000000 nml-0.7.2/regression/018_airport_tile.nml
--rw-r--r--   0 runner     (501) staff       (20)     1007 2023-04-17 19:54:52.000000 nml-0.7.2/regression/019_switch.nml
--rw-r--r--   0 runner     (501) staff       (20)     1236 2023-04-17 19:54:52.000000 nml-0.7.2/regression/020_recolour.nml
--rw-r--r--   0 runner     (501) staff       (20)     1300 2023-04-17 19:54:52.000000 nml-0.7.2/regression/021_grf_parameter.nml
--rw-r--r--   0 runner     (501) staff       (20)      334 2023-04-17 19:54:52.000000 nml-0.7.2/regression/022_disable_item.nml
--rw-r--r--   0 runner     (501) staff       (20)      354 2023-04-17 19:54:52.000000 nml-0.7.2/regression/023_engine_override.nml
--rw-r--r--   0 runner     (501) staff       (20)       96 2023-04-17 19:54:52.000000 nml-0.7.2/regression/024_conditional.nml
--rw-r--r--   0 runner     (501) staff       (20)       40 2023-04-17 19:54:52.000000 nml-0.7.2/regression/025_loop.nml
--rw-r--r--   0 runner     (501) staff       (20)      830 2023-04-17 19:54:52.000000 nml-0.7.2/regression/026_asl.nml
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-04-17 19:54:52.000000 nml-0.7.2/regression/027_airport_layout.nml
--rw-r--r--   0 runner     (501) staff       (20)      916 2023-04-17 19:54:52.000000 nml-0.7.2/regression/028_font.nml
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-17 19:54:52.000000 nml-0.7.2/regression/029_base_graphics.nml
--rw-r--r--   0 runner     (501) staff       (20)     6842 2023-04-17 19:54:52.000000 nml-0.7.2/regression/030_house.nml
--rw-r--r--   0 runner     (501) staff       (20)      664 2023-04-17 19:54:52.000000 nml-0.7.2/regression/031_aircraft.nml
--rw-r--r--   0 runner     (501) staff       (20)      866 2023-04-17 19:54:52.000000 nml-0.7.2/regression/032_simple_house.nml
--rw-r--r--   0 runner     (501) staff       (20)     1031 2023-04-17 19:54:52.000000 nml-0.7.2/regression/033_procedure.nml
--rw-r--r--   0 runner     (501) staff       (20)      120 2023-04-17 19:54:52.000000 nml-0.7.2/regression/034_roadtypes.nml
--rw-r--r--   0 runner     (501) staff       (20)      918 2023-04-17 19:54:52.000000 nml-0.7.2/regression/035_switch_scope.nml
--rw-r--r--   0 runner     (501) staff       (20)     1384 2023-04-17 19:54:52.000000 nml-0.7.2/regression/036_procedure_scope.nml
--rw-r--r--   0 runner     (501) staff       (20)      476 2023-04-17 19:54:52.000000 nml-0.7.2/regression/037_optimised_trigger.nml
--rw-r--r--   0 runner     (501) staff       (20)     1486 2023-04-17 19:54:52.000000 nml-0.7.2/regression/038_optimised_scope.nml
--rw-r--r--   0 runner     (501) staff       (20)      633 2023-04-17 19:54:52.000000 nml-0.7.2/regression/039_storage.nml
--rw-r--r--   0 runner     (501) staff       (20)     3324 2023-04-17 19:54:52.000000 nml-0.7.2/regression/040_station.nml
--rw-r--r--   0 runner     (501) staff       (20)     1998 2023-04-17 19:54:52.000000 nml-0.7.2/regression/Makefile
--rw-r--r--   0 runner     (501) staff       (20)    24598 2023-04-17 19:54:52.000000 nml-0.7.2/regression/arctic_railwagons.pcx
--rw-r--r--   0 runner     (501) staff       (20)        4 2023-04-17 19:54:52.000000 nml-0.7.2/regression/beef.wav
--rw-r--r--   0 runner     (501) staff       (20)     7397 2023-04-17 19:54:52.000000 nml-0.7.2/regression/brewery.png
--rw-r--r--   0 runner     (501) staff       (20)     7424 2023-04-17 19:54:52.000000 nml-0.7.2/regression/brewery_snow.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.337540 nml-0.7.2/regression/expected/
--rw-r--r--   0 runner     (501) staff       (20)      148 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/001_action8.grf
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/001_action8.nfo
--rw-r--r--   0 runner     (501) staff       (20)      236 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/002_sounds.grf
--rw-r--r--   0 runner     (501) staff       (20)      923 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/002_sounds.nfo
--rw-r--r--   0 runner     (501) staff       (20)      218 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/003_assignment.grf
--rw-r--r--   0 runner     (501) staff       (20)     1241 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/003_assignment.nfo
--rw-r--r--   0 runner     (501) staff       (20)       49 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/004_deactivate.grf
--rw-r--r--   0 runner     (501) staff       (20)      490 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/004_deactivate.nfo
--rw-r--r--   0 runner     (501) staff       (20)      207 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/005_error.grf
--rw-r--r--   0 runner     (501) staff       (20)      835 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/005_error.nfo
--rw-r--r--   0 runner     (501) staff       (20)     6709 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/006_vehicle.grf
--rw-r--r--   0 runner     (501) staff       (20)     4257 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/006_vehicle.nfo
--rw-r--r--   0 runner     (501) staff       (20)      408 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/007_townnames.grf
--rw-r--r--   0 runner     (501) staff       (20)     1292 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/007_townnames.nfo
--rw-r--r--   0 runner     (501) staff       (20)       49 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/008_railtypes.grf
--rw-r--r--   0 runner     (501) staff       (20)      492 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/008_railtypes.nfo
--rw-r--r--   0 runner     (501) staff       (20)      939 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/009_replace.grf
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/009_replace.nfo
--rw-r--r--   0 runner     (501) staff       (20)     5461 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/010_liveryoverride.grf
--rw-r--r--   0 runner     (501) staff       (20)     2669 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/010_liveryoverride.nfo
--rw-r--r--   0 runner     (501) staff       (20)      545 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/011_snowline.grf
--rw-r--r--   0 runner     (501) staff       (20)     1839 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/011_snowline.nfo
--rw-r--r--   0 runner     (501) staff       (20)      416 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/012_basecost.grf
--rw-r--r--   0 runner     (501) staff       (20)     1576 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/012_basecost.nfo
--rw-r--r--   0 runner     (501) staff       (20)     7776 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/013_train_callback.grf
--rw-r--r--   0 runner     (501) staff       (20)     7674 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/013_train_callback.nfo
--rw-r--r--   0 runner     (501) staff       (20)      560 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/014_read_special_param.grf
--rw-r--r--   0 runner     (501) staff       (20)     1946 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/014_read_special_param.nfo
--rw-r--r--   0 runner     (501) staff       (20)      267 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/015_basic_object.grf
--rw-r--r--   0 runner     (501) staff       (20)     1012 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/015_basic_object.nfo
--rw-r--r--   0 runner     (501) staff       (20)      261 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/016_basic_airporttiles.grf
--rw-r--r--   0 runner     (501) staff       (20)      746 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/016_basic_airporttiles.nfo
--rw-r--r--   0 runner     (501) staff       (20)     2032 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/017_articulated_tram.grf
--rw-r--r--   0 runner     (501) staff       (20)     1931 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/017_articulated_tram.nfo
--rw-r--r--   0 runner     (501) staff       (20)      223 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/018_airport_tile.grf
--rw-r--r--   0 runner     (501) staff       (20)      981 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/018_airport_tile.nfo
--rw-r--r--   0 runner     (501) staff       (20)      493 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/019_switch.grf
--rw-r--r--   0 runner     (501) staff       (20)     2294 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/019_switch.nfo
--rw-r--r--   0 runner     (501) staff       (20)     2685 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/020_recolour.grf
--rw-r--r--   0 runner     (501) staff       (20)     3763 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/020_recolour.nfo
--rw-r--r--   0 runner     (501) staff       (20)      921 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/021_grf_parameter.grf
--rw-r--r--   0 runner     (501) staff       (20)     1751 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/021_grf_parameter.nfo
--rw-r--r--   0 runner     (501) staff       (20)      320 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/022_disable_item.grf
--rw-r--r--   0 runner     (501) staff       (20)     1155 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/022_disable_item.nfo
--rw-r--r--   0 runner     (501) staff       (20)      190 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/023_engine_override.grf
--rw-r--r--   0 runner     (501) staff       (20)      769 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/023_engine_override.nfo
--rw-r--r--   0 runner     (501) staff       (20)       75 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/024_conditional.grf
--rw-r--r--   0 runner     (501) staff       (20)      610 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/024_conditional.nfo
--rw-r--r--   0 runner     (501) staff       (20)      111 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/025_loop.grf
--rw-r--r--   0 runner     (501) staff       (20)      761 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/025_loop.nfo
--rw-r--r--   0 runner     (501) staff       (20)     2019 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/026_asl.grf
--rw-r--r--   0 runner     (501) staff       (20)     5657 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/026_asl.nfo
--rw-r--r--   0 runner     (501) staff       (20)      144 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/027_airport_layout.grf
--rw-r--r--   0 runner     (501) staff       (20)      851 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/027_airport_layout.nfo
--rw-r--r--   0 runner     (501) staff       (20)      718 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/028_font.grf
--rw-r--r--   0 runner     (501) staff       (20)     1119 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/028_font.nfo
--rw-r--r--   0 runner     (501) staff       (20)     1086 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/029_base_graphics.grf
--rw-r--r--   0 runner     (501) staff       (20)     2366 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/029_base_graphics.nfo
--rw-r--r--   0 runner     (501) staff       (20)    14397 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/030_house.grf
--rw-r--r--   0 runner     (501) staff       (20)     9228 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/030_house.nfo
--rw-r--r--   0 runner     (501) staff       (20)      207 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/031_aircraft.grf
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/031_aircraft.nfo
--rw-r--r--   0 runner     (501) staff       (20)      752 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/032_simple_house.grf
--rw-r--r--   0 runner     (501) staff       (20)     1387 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/032_simple_house.nfo
--rw-r--r--   0 runner     (501) staff       (20)      833 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/033_procedure.grf
--rw-r--r--   0 runner     (501) staff       (20)     3558 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/033_procedure.nfo
--rw-r--r--   0 runner     (501) staff       (20)       43 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/034_roadtypes.grf
--rw-r--r--   0 runner     (501) staff       (20)      478 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/034_roadtypes.nfo
--rw-r--r--   0 runner     (501) staff       (20)      706 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/035_switch_scope.grf
--rw-r--r--   0 runner     (501) staff       (20)     3406 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/035_switch_scope.nfo
--rw-r--r--   0 runner     (501) staff       (20)     1070 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/036_procedure_scope.grf
--rw-r--r--   0 runner     (501) staff       (20)     4765 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/036_procedure_scope.nfo
--rw-r--r--   0 runner     (501) staff       (20)      232 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/037_optimised_trigger.grf
--rw-r--r--   0 runner     (501) staff       (20)     1021 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/037_optimised_trigger.nfo
--rw-r--r--   0 runner     (501) staff       (20)      731 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/038_optimised_scope.grf
--rw-r--r--   0 runner     (501) staff       (20)     3541 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/038_optimised_scope.nfo
--rw-r--r--   0 runner     (501) staff       (20)      410 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/039_storage.grf
--rw-r--r--   0 runner     (501) staff       (20)     1821 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/039_storage.nfo
--rw-r--r--   0 runner     (501) staff       (20)     1265 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/040_station.grf
--rw-r--r--   0 runner     (501) staff       (20)     5275 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/040_station.nfo
--rw-r--r--   0 runner     (501) staff       (20)      918 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_industry.grf
--rw-r--r--   0 runner     (501) staff       (20)     3258 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_industry.nfo
--rw-r--r--   0 runner     (501) staff       (20)     7075 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_object.grf
--rw-r--r--   0 runner     (501) staff       (20)     5247 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_object.nfo
--rw-r--r--   0 runner     (501) staff       (20)    39472 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_railtype.grf
--rw-r--r--   0 runner     (501) staff       (20)    10983 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_railtype.nfo
--rw-r--r--   0 runner     (501) staff       (20)    17814 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_road_vehicle.grf
--rw-r--r--   0 runner     (501) staff       (20)    16641 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_road_vehicle.nfo
--rw-r--r--   0 runner     (501) staff       (20)    68061 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_roadtype_and_tramtype.grf
--rw-r--r--   0 runner     (501) staff       (20)    13101 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_roadtype_and_tramtype.nfo
--rw-r--r--   0 runner     (501) staff       (20)     3927 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_station.grf
--rw-r--r--   0 runner     (501) staff       (20)     3405 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_station.nfo
--rw-r--r--   0 runner     (501) staff       (20)    12437 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_train.grf
--rw-r--r--   0 runner     (501) staff       (20)    14239 2023-04-17 19:54:52.000000 nml-0.7.2/regression/expected/example_train.nfo
--rw-r--r--   0 runner     (501) staff       (20)     1169 2023-04-17 19:54:52.000000 nml-0.7.2/regression/font_addl.png
--rw-r--r--   0 runner     (501) staff       (20)     1190 2023-04-17 19:54:52.000000 nml-0.7.2/regression/fonts.png
--rw-r--r--   0 runner     (501) staff       (20)     3039 2023-04-17 19:54:52.000000 nml-0.7.2/regression/groundtiles.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:55:21.339135 nml-0.7.2/regression/lang/
--rw-r--r--   0 runner     (501) staff       (20)      279 2023-04-17 19:54:52.000000 nml-0.7.2/regression/lang/dutch.lng
--rw-r--r--   0 runner     (501) staff       (20)     2096 2023-04-17 19:54:52.000000 nml-0.7.2/regression/lang/english.lng
--rw-r--r--   0 runner     (501) staff       (20)       43 2023-04-17 19:54:52.000000 nml-0.7.2/regression/lang/us.lng
--rw-r--r--   0 runner     (501) staff       (20)     1509 2023-04-17 19:54:52.000000 nml-0.7.2/regression/nlhs.png
--rw-r--r--   0 runner     (501) staff       (20)     2655 2023-04-17 19:54:52.000000 nml-0.7.2/regression/oneway.png
--rw-r--r--   0 runner     (501) staff       (20)    14463 2023-04-17 19:54:52.000000 nml-0.7.2/regression/opengfx_generic_trams1.pcx
--rw-r--r--   0 runner     (501) staff       (20)    10007 2023-04-17 19:54:52.000000 nml-0.7.2/regression/opengfx_generic_trams1.png
--rw-r--r--   0 runner     (501) staff       (20)    16633 2023-04-17 19:54:52.000000 nml-0.7.2/regression/opengfx_trains_start.pcx
--rw-r--r--   0 runner     (501) staff       (20)     5280 2023-04-17 19:54:52.000000 nml-0.7.2/regression/station.png
--rw-r--r--   0 runner     (501) staff       (20)     7772 2023-04-17 19:54:52.000000 nml-0.7.2/regression/temperate_railwagons.png
--rw-r--r--   0 runner     (501) staff       (20)     2445 2023-04-17 19:54:52.000000 nml-0.7.2/regression/tram_foster_express.png
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-17 19:55:21.340396 nml-0.7.2/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     2160 2023-04-17 19:54:52.000000 nml-0.7.2/setup.py
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/regression/
+-rw-r--r--   0 hg        (1002) hg        (1003)      319 2011-07-08 20:55:33.000000 nml-r1512/regression/012_basecost.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     2509 2011-07-08 20:55:33.000000 nml-r1512/regression/010_liveryoverride.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      328 2011-07-08 20:55:33.000000 nml-r1512/regression/003_assignment.nml
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     1087 2011-07-08 20:55:33.000000 nml-r1512/regression/015_basic_object.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      445 2011-07-08 20:55:33.000000 nml-r1512/regression/026_asl.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)       70 2011-07-08 20:55:33.000000 nml-r1512/regression/002_sounds.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     7772 2011-07-08 20:55:33.000000 nml-r1512/regression/temperate_railwagons.png
+-rw-r--r--   0 hg        (1002) hg        (1003)      277 2011-07-08 20:55:33.000000 nml-r1512/regression/011_snowline.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      640 2011-07-08 20:55:33.000000 nml-r1512/regression/Makefile
+-rw-r--r--   0 hg        (1002) hg        (1003)     1298 2011-07-08 20:55:33.000000 nml-r1512/regression/021_grf_parameter.nml
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/regression/lang/
+-rw-r--r--   0 hg        (1002) hg        (1003)       43 2011-07-08 20:55:33.000000 nml-r1512/regression/lang/us.lng
+-rw-r--r--   0 hg        (1002) hg        (1003)     1775 2011-07-08 20:55:33.000000 nml-r1512/regression/lang/english.lng
+-rw-r--r--   0 hg        (1002) hg        (1003)      279 2011-07-08 20:55:33.000000 nml-r1512/regression/lang/dutch.lng
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      511 2011-07-08 20:55:33.000000 nml-r1512/regression/018_airport_tile.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      281 2011-07-08 20:55:33.000000 nml-r1512/regression/004_deactivate.nml
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/regression/expected/
+-rw-r--r--   0 hg        (1002) hg        (1003)     1959 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/014_read_special_param.nfo
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      692 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/016_basic_airporttiles.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      169 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/003_assignment.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      753 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/025_loop.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      117 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/001_action8.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)       88 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/004_deactivate.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      754 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/007_townnames.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      758 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/009_replaceTTDsprite.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     6892 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/013_train_callback.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      810 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/004_deactivate.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1763 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/021_grf_parameter.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      223 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/026_asl.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      888 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/021_grf_parameter.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)       65 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/002_sounds.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      830 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/005_error.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      493 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/014_read_special_param.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      148 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/018_airport_tile.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      584 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/002_sounds.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      151 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/023_engine_override.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     1496 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/012_basecost.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     5370 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/013_train_callback.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1252 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/003_assignment.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      363 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/009_replaceTTDsprite.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      810 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/027_airport_layout.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1865 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/011_snowline.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      510 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/011_snowline.grf
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      226 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/015_basic_object.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     1738 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/006_vehicle.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      737 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/023_engine_override.nfo
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      219 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/016_basic_airporttiles.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      113 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/027_airport_layout.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      323 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/012_basecost.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      279 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/022_disable_item.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     2516 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/020_recolour.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)       80 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/025_loop.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     1885 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/017_articulated_tram.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     5012 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/010_liveryoverride.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      631 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/001_action8.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      160 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/007_townnames.grf
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      970 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/015_basic_object.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      320 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/019_switch.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      766 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/018_airport_tile.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      176 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/005_error.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)      605 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/024_conditional.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1889 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/006_vehicle.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)       50 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/024_conditional.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     3702 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/020_recolour.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1126 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/022_disable_item.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     2337 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/010_liveryoverride.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)      480 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/008_railtypes.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     1604 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/019_switch.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)       28 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/008_railtypes.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     1870 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/017_articulated_tram.grf
+-rw-r--r--   0 hg        (1002) hg        (1003)     1249 2011-07-08 20:55:33.000000 nml-r1512/regression/expected/026_asl.nfo
+-rw-r--r--   0 hg        (1002) hg        (1003)     2445 2011-07-08 20:55:33.000000 nml-r1512/regression/tram_foster_express.png
+-rw-r--r--   0 hg        (1002) hg        (1003)      203 2011-07-08 20:55:33.000000 nml-r1512/regression/005_error.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     1234 2011-07-08 20:55:33.000000 nml-r1512/regression/020_recolour.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)    14313 2011-07-08 20:55:33.000000 nml-r1512/regression/opengfx_generic_trams1.pcx
+-rw-r--r--   0 hg        (1002) hg        (1003)      332 2011-07-08 20:55:33.000000 nml-r1512/regression/022_disable_item.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     5036 2011-07-08 20:55:33.000000 nml-r1512/regression/013_train_callback.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      158 2011-07-08 20:55:33.000000 nml-r1512/regression/008_railtypes.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)        4 2011-07-08 20:55:33.000000 nml-r1512/regression/beef.wav
+-rw-r--r--   0 hg        (1002) hg        (1003)      427 2011-07-08 20:55:33.000000 nml-r1512/regression/009_replaceTTDsprite.nml
+-rwxr-xr-x   0 hg        (1002) hg        (1003)      348 2011-07-08 20:55:33.000000 nml-r1512/regression/023_engine_override.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     2242 2011-07-08 20:55:33.000000 nml-r1512/regression/006_vehicle.nml
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     1193 2011-07-08 20:55:33.000000 nml-r1512/regression/019_switch.nml
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     2614 2011-07-08 20:55:33.000000 nml-r1512/regression/017_articulated_tram.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)     1125 2011-07-08 20:55:33.000000 nml-r1512/regression/014_read_special_param.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)    24598 2011-07-08 20:55:33.000000 nml-r1512/regression/arctic_railwagons.pcx
+-rw-r--r--   0 hg        (1002) hg        (1003)    16423 2011-07-08 20:55:33.000000 nml-r1512/regression/opengfx_trains_start.pcx
+-rw-r--r--   0 hg        (1002) hg        (1003)      609 2011-07-08 20:55:33.000000 nml-r1512/regression/016_basic_airporttiles.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      462 2011-07-08 20:55:33.000000 nml-r1512/regression/007_townnames.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)       86 2011-07-08 20:55:33.000000 nml-r1512/regression/024_conditional.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      152 2011-07-08 20:55:33.000000 nml-r1512/regression/001_action8.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)       40 2011-07-08 20:55:33.000000 nml-r1512/regression/025_loop.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      914 2011-07-08 20:55:33.000000 nml-r1512/regression/027_airport_layout.nml
+-rw-r--r--   0 hg        (1002) hg        (1003)      717 2011-07-08 21:18:54.000000 nml-r1512/PKG-INFO
+-rw-r--r--   0 hg        (1002) hg        (1003)      227 2011-07-08 20:55:32.000000 nml-r1512/MANIFEST.in
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/nml/
+-rw-r--r--   0 hg        (1002) hg        (1003)     4018 2011-07-08 20:55:33.000000 nml-r1512/nml/output_nfo.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2628 2011-07-08 20:55:33.000000 nml-r1512/nml/free_number_list.py
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/nml/ast/
+-rw-r--r--   0 hg        (1002) hg        (1003)     6843 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/basecost.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      495 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/skipall.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    25332 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/switch.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    10465 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/item.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2139 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/disable_item.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     3278 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/error.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1227 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/loop.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1195 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/cargotable.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      756 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/deactivate.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     5166 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/produce.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    15370 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/townnames.py
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     5825 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/alt_sprites.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    10516 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/spriteblock.py
+-rw-r--r--   0 hg        (1002) hg        (1003)        0 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/__init__.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2161 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/conditional.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     5378 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/replace.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2625 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/base_sprites.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1452 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/font.py
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     4791 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/tilelayout.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     9960 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/grf.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1485 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/general.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1773 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/override.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1570 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/assignment.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1780 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/switch_range.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     5400 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/base_statement.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2021 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/railtypetable.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     4572 2011-07-08 20:55:32.000000 nml-r1512/nml/ast/snowline.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    19390 2011-07-08 20:55:33.000000 nml-r1512/nml/palette.py
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/nml/actions/
+-rw-r--r--   0 hg        (1002) hg        (1003)     4520 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action5.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1163 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/base_action.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    10049 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action3_callbacks.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      757 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action8.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    30527 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2var.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     6697 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action1.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2530 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action11.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     8557 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action14.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1871 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/actionE.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     3977 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/actionB.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2693 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2production.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1758 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/actionA.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    19891 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action0.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    17618 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    16091 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/real_sprite.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    34142 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action0properties.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      278 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/sprite_count.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2733 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2real.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     6392 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/actionF.py
+-rw-r--r--   0 hg        (1002) hg        (1003)        0 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/__init__.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    20308 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2var_variables.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2473 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action12.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    16799 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/actionD.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    10533 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action7.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    12031 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action3.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      408 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action10.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     6737 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action4.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      864 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action6.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    20266 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2layout.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     3515 2011-07-08 20:55:32.000000 nml-r1512/nml/actions/action2random.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    11620 2011-07-08 20:55:33.000000 nml-r1512/nml/main.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2752 2011-07-08 20:55:33.000000 nml-r1512/nml/version_info.py
+-rw-r--r--   0 hg        (1002) hg        (1003)        0 2011-07-08 20:55:32.000000 nml-r1512/nml/__init__.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    38098 2011-07-08 20:55:33.000000 nml-r1512/nml/global_constants.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     9513 2011-07-08 20:55:33.000000 nml-r1512/nml/nmlop.py
+-rw-r--r--   0 hg        (1002) hg        (1003)       74 2011-07-08 21:18:54.000000 nml-r1512/nml/__version__.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     5283 2011-07-08 20:55:33.000000 nml-r1512/nml/output_base.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      415 2011-07-08 20:55:33.000000 nml-r1512/nml/output_nml.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    25395 2011-07-08 20:55:33.000000 nml-r1512/nml/grfstrings.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    26563 2011-07-08 20:55:33.000000 nml-r1512/nml/parser.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    10221 2011-07-08 20:55:33.000000 nml-r1512/nml/output_grf.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      462 2011-07-08 20:55:33.000000 nml-r1512/nml/unit.py
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/nml/expression/
+-rw-r--r--   0 hg        (1002) hg        (1003)     2545 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/special_parameter.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1590 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/identifier.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     3535 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/parameter.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     4822 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/base_expression.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2897 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/bin_not.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1067 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/string.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      593 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/array.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1949 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/spritegroup_ref.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     2237 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/ternaryop.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1003 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/boolean.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     3247 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/variable.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      899 2011-07-08 20:55:32.000000 nml-r1512/nml/expression/__init__.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1554 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/functionptr.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      887 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/patch_variable.py
+-rw-r--r--   0 hg        (1002) hg        (1003)      641 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/string_literal.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1189 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/bitmask.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     9278 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/binop.py
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     3895 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/storage_op.py
+-rw-r--r--   0 hg        (1002) hg        (1003)    17886 2011-07-08 20:55:33.000000 nml-r1512/nml/expression/functioncall.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     1727 2011-07-08 20:55:33.000000 nml-r1512/nml/lz77.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     5781 2011-07-08 20:55:33.000000 nml-r1512/nml/tokens.py
+-rw-r--r--   0 hg        (1002) hg        (1003)     4074 2011-07-08 20:55:33.000000 nml-r1512/nml/generic.py
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/
+-rw-r--r--   0 hg        (1002) hg        (1003)      717 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/PKG-INFO
+-rw-r--r--   0 hg        (1002) hg        (1003)        1 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/dependency_links.txt
+-rw-r--r--   0 hg        (1002) hg        (1003)       57 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/entry_points.txt
+-rw-r--r--   0 hg        (1002) hg        (1003)        4 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/top_level.txt
+-rw-r--r--   0 hg        (1002) hg        (1003)     6036 2011-07-08 21:18:54.000000 nml-r1512/nml.egg-info/SOURCES.txt
+drwxr-xr-x   0 hg        (1002) hg        (1003)        0 2011-07-08 21:18:54.000000 nml-r1512/docs/
+-rw-r--r--   0 hg        (1002) hg        (1003)    36027 2011-07-08 20:55:32.000000 nml-r1512/docs/compileprocess.png
+-rw-r--r--   0 hg        (1002) hg        (1003)      480 2011-07-08 20:55:32.000000 nml-r1512/docs/bridges.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     4552 2011-07-08 20:55:32.000000 nml-r1512/docs/houses.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    11349 2011-07-08 20:55:32.000000 nml-r1512/docs/objects.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     5570 2011-07-08 20:55:32.000000 nml-r1512/docs/ttd-newgrf-win.gpl
+-rw-r--r--   0 hg        (1002) hg        (1003)     1950 2011-07-08 20:55:32.000000 nml-r1512/docs/nml.css
+-rw-r--r--   0 hg        (1002) hg        (1003)     7469 2011-07-08 20:55:32.000000 nml-r1512/docs/general.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    24558 2011-07-08 20:55:32.000000 nml-r1512/docs/tileh.png
+-rw-r--r--   0 hg        (1002) hg        (1003)     3707 2011-07-08 20:55:32.000000 nml-r1512/docs/language-files.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     7412 2011-07-08 20:55:32.000000 nml-r1512/docs/index.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     5570 2011-07-08 20:55:32.000000 nml-r1512/docs/ttd-newgrf-dos.gpl
+-rw-r--r--   0 hg        (1002) hg        (1003)      470 2011-07-08 20:55:32.000000 nml-r1512/docs/canals.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     6387 2011-07-08 20:55:32.000000 nml-r1512/docs/cargos.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     4135 2011-07-08 20:55:32.000000 nml-r1512/docs/airports.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    47585 2011-07-08 20:55:32.000000 nml-r1512/docs/refs.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     1170 2011-07-08 20:55:32.000000 nml-r1512/docs/warnings.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    11317 2011-07-08 20:55:32.000000 nml-r1512/docs/liveryoverride.png
+-rw-r--r--   0 hg        (1002) hg        (1003)    72737 2011-07-08 20:55:32.000000 nml-r1512/docs/nml-language.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     2666 2011-07-08 20:55:32.000000 nml-r1512/docs/compatible.html
+-rw-r--r--   0 hg        (1002) hg        (1003)     8711 2011-07-08 20:55:32.000000 nml-r1512/docs/railtypes.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    25788 2011-07-08 20:55:32.000000 nml-r1512/docs/industries.html
+-rw-r--r--   0 hg        (1002) hg        (1003)    27014 2011-07-08 20:55:32.000000 nml-r1512/docs/vehicles.html
+-rw-r--r--   0 hg        (1002) hg        (1003)      486 2011-07-08 20:55:32.000000 nml-r1512/docs/stations.html
+-rwxr-xr-x   0 hg        (1002) hg        (1003)     1522 2011-07-08 20:55:33.000000 nml-r1512/setup.py
+-rw-r--r--   0 hg        (1002) hg        (1003)       59 2011-07-08 21:18:54.000000 nml-r1512/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nml-0.7.2/nml/actions/action12.py` & `nml-r1512/nml/actions/action12.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,60 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic
+from nml import generic, expression
 from nml.actions import base_action, real_sprite
 
-
 class Action12(base_action.BaseAction):
-    # sets: list of (font_size, num_char, base_char) tuples
+
+    #sets: list of (font_size, num_char, base_char) tuples
     def __init__(self, sets):
         self.sets = sets
 
     def write(self, file):
-        # <sprite-number> * <length> 12 <num-def> (<font> <num-char> <base-char>){n}
+        #<sprite-number> * <length> 12 <num-def> (<font> <num-char> <base-char>){n}
         size = 2 + 4 * len(self.sets)
         file.start_sprite(size)
         file.print_bytex(0x12)
         file.print_byte(len(self.sets))
         file.newline()
         for font_size, num_char, base_char in self.sets:
             font_size.write(file, 1)
             file.print_byte(num_char)
             file.print_word(base_char)
             file.newline()
         file.end_sprite()
 
-
 font_sizes = {
-    "NORMAL": 0,
-    "SMALL": 1,
-    "LARGE": 2,
-    "MONO": 3,
+    'NORMAL' : 0,
+    'SMALL'  : 1,
+    'LARGE'  : 2,
 }
 
-
 def parse_action12(font_glyphs):
     try:
         font_size = font_glyphs.font_size.reduce_constant([font_sizes])
         if isinstance(font_glyphs.base_char, expression.StringLiteral) and len(font_glyphs.base_char.value) == 1:
             base_char = ord(font_glyphs.base_char.value)
         else:
             base_char = font_glyphs.base_char.reduce_constant()
     except generic.ConstError:
-        raise generic.ScriptError("Parameters of font_glyph have to be compile-time constants", font_glyphs.pos)
+        raise generic.ScriptError("Parameters of font_glpyh have to be compile-time constants", font_glyphs.pos)
     if font_size.value not in font_sizes.values():
-        raise generic.ScriptError(
-            "Invalid value for parameter 'font_size' in font_glyph, valid values are 0, 1, 2", font_size.pos
-        )
+        raise generic.ScriptError("Invalid value for parameter 'font_size' in font_glpyh, valid values are 0, 1, 2", font_size.pos)
     if not (0 <= base_char.value <= 0xFFFF):
-        raise generic.ScriptError(
-            "Invalid value for parameter 'base_char' in font_glyph, valid values are 0-0xFFFF", base_char.pos
-        )
+        raise generic.ScriptError("Invalid value for parameter 'base_char' in font_glyph, valid values are 0-0xFFFF", base_char.pos)
 
-    real_sprite_list = real_sprite.parse_sprite_data(font_glyphs)
+    real_sprite_list = real_sprite.parse_sprite_list(font_glyphs.sprite_list, font_glyphs.pcx, block_name = font_glyphs.name)
     char = base_char.value
     last_char = char + len(real_sprite_list)
     if last_char > 0xFFFF:
-        raise generic.ScriptError(
-            "Character numbers in font_glyph block exceed the allowed range (0-0xFFFF)", font_glyphs.pos
-        )
+        raise generic.ScriptError("Character numbers in font_glyph block exceed the allowed range (0-0xFFFF)", font_glyphs.pos)
 
     sets = []
     while char < last_char:
-        # each set of characters must fit in a single 128-char block, according to specs / TTDP
-        if (char // 128) * 128 != (last_char // 128) * 128:
+        #each set of characters must fit in a single 128-char block, according to specs / TTDP
+        if (char // 128) * 128 != (last_char // 128)  * 128:
             num_in_set = (char // 128 + 1) * 128 - char
         else:
             num_in_set = last_char - char
         sets.append((font_size, num_in_set, char))
         char += num_in_set
 
     return [Action12(sets)] + real_sprite_list
```

### Comparing `nml-0.7.2/nml/actions/action14.py` & `nml-r1512/nml/actions/action14.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,30 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic, grfstrings
+from nml import grfstrings
 from nml.actions import base_action
 
 
 class Action14(base_action.BaseAction):
     def __init__(self, nodes):
         self.nodes = nodes
 
     def skip_action7(self):
         return False
 
     def write(self, file):
-        size = 2  # final 0-byte
-        for node in self.nodes:
-            size += node.get_size()
+        size = 2 # final 0-byte
+        for node in self.nodes: size += node.get_size()
 
         file.start_sprite(size)
         file.print_bytex(0x14)
         for node in self.nodes:
             node.write(file)
         file.print_bytex(0)
 
         file.end_sprite()
 
-
 def split_action14(node, max_size):
     if node.get_size() <= max_size:
         return [node, None]
     if not isinstance(node, BranchNode):
         return [None, node]
     new_node = BranchNode(node.id)
     rest = BranchNode(node.id)
@@ -59,58 +42,55 @@
             copy_to_rest = True
 
     assert len(rest.subnodes) > 0
     if len(new_node.subnodes) == 0:
         return [None, rest]
     return [new_node, rest]
 
-
 def get_actions(root):
     action_list = []
     while True:
         node, root = split_action14(root, 65535)
         assert node is not None
         action_list.append(Action14([node]))
         if root is None:
             break
 
     return action_list
 
-
-class Action14Node:
+class Action14Node(object):
     def __init__(self, type_string, id):
         self.type_string = type_string
         self.id = id
 
     def get_size(self):
         """
         How many bytes will be written to the output file by L{write}?
 
         @return: The size (in bytes) of this node.
         """
-        raise NotImplementedError("get_size must be implemented in Action14Node-subclass {!r}".format(type(self)))
+        raise NotImplementedError('get_size must be implemented in Action14Node-subclass %r' % type(self))
 
     def write(self, file):
         """
         Write this node to the output file.
 
         @param file: The file to write the output to.
         """
-        raise NotImplementedError("write must be implemented in Action14Node-subclass {!r}".format(type(self)))
+        raise NotImplementedError('write must be implemented in Action14Node-subclass %r' % type(self))
 
     def write_type_id(self, file):
         file.print_string(self.type_string, False, True)
-        if isinstance(self.id, str):
+        if isinstance(self.id, basestring):
             file.print_string(self.id, False, True)
         else:
             file.print_dword(self.id)
 
-
 class TextNode(Action14Node):
-    def __init__(self, id, string, skip_default_langid=False):
+    def __init__(self, id, string, skip_default_langid = False):
         Action14Node.__init__(self, "T", id)
         self.string = string
         grfstrings.validate_string(self.string)
         self.skip_default_langid = skip_default_langid
 
     def get_size(self):
         if self.skip_default_langid:
@@ -130,75 +110,59 @@
             file.newline()
         for lang_id in grfstrings.get_translations(self.string):
             self.write_type_id(file)
             file.print_bytex(lang_id)
             file.print_string(grfstrings.get_translation(self.string, lang_id))
             file.newline()
 
-
 class BranchNode(Action14Node):
     def __init__(self, id):
         Action14Node.__init__(self, "C", id)
         self.subnodes = []
 
     def get_size(self):
-        size = 6  # "C", id, final 0-byte
+        size = 6 # "C", id, final 0-byte
         for node in self.subnodes:
             size += node.get_size()
         return size
 
     def write(self, file):
         self.write_type_id(file)
         file.newline()
         for node in self.subnodes:
             node.write(file)
         file.print_bytex(0)
         file.newline()
 
-
 class BinaryNode(Action14Node):
-    def __init__(self, id, size, val=None):
+    def __init__(self, id, size, val = None):
         Action14Node.__init__(self, "B", id)
         self.size = size
         self.val = val
 
     def get_size(self):
-        return 7 + self.size  # "B" (1), id (4), size (2), data (self.size)
+        return 7 + self.size # "B" (1), id (4), size (2), data (self.size)
 
     def write(self, file):
         self.write_type_id(file)
         file.print_word(self.size)
         file.print_varx(self.val, self.size)
         file.newline()
 
-
 class UsedPaletteNode(BinaryNode):
     def __init__(self, pal):
         BinaryNode.__init__(self, "PALS", 1)
         self.pal = pal
 
     def write(self, file):
         self.write_type_id(file)
         file.print_word(self.size)
         file.print_string(self.pal, False, True)
         file.newline()
 
-
-class BlitterNode(BinaryNode):
-    def __init__(self, blitter):
-        BinaryNode.__init__(self, "BLTR", 1)
-        self.blitter = blitter
-
-    def write(self, file):
-        self.write_type_id(file)
-        file.print_word(self.size)
-        file.print_string(self.blitter, False, True)
-        file.newline()
-
-
 class SettingMaskNode(BinaryNode):
     def __init__(self, param_num, first_bit, num_bits):
         BinaryNode.__init__(self, "MASK", 3)
         self.param_num = param_num
         self.first_bit = first_bit
         self.num_bits = num_bits
 
@@ -206,45 +170,39 @@
         self.write_type_id(file)
         file.print_word(self.size)
         file.print_byte(self.param_num)
         file.print_byte(self.first_bit)
         file.print_byte(self.num_bits)
         file.newline()
 
-
 class LimitNode(BinaryNode):
     def __init__(self, min_val, max_val):
         BinaryNode.__init__(self, "LIMI", 8)
         self.min_val = min_val
         self.max_val = max_val
 
     def write(self, file):
         self.write_type_id(file)
         file.print_word(self.size)
         file.print_dword(self.min_val)
         file.print_dword(self.max_val)
         file.newline()
 
-
-def grf_name_desc_actions(root, name, desc, url, version, min_compatible_version):
+def grf_name_desc_actions(root, name, desc, version, min_compatible_version):
     if len(grfstrings.get_translations(name)) > 0:
         name_node = TextNode("NAME", name, True)
         root.subnodes.append(name_node)
     if len(grfstrings.get_translations(desc)) > 0:
         desc_node = TextNode("DESC", desc, True)
         root.subnodes.append(desc_node)
-    if url is not None:
-        desc_node = TextNode("URL_", url)
-        root.subnodes.append(desc_node)
     version_node = BinaryNode("VRSN", 4, version.value)
     root.subnodes.append(version_node)
     min_compatible_version_node = BinaryNode("MINV", 4, min_compatible_version.value)
     root.subnodes.append(min_compatible_version_node)
 
-
 def param_desc_actions(root, params):
     num_params = 0
     for param_desc in params:
         num_params += len(param_desc.setting_list)
     root.subnodes.append(BinaryNode("NPAR", 1, num_params))
     param_root = BranchNode("PARA")
     param_num = 0
@@ -254,44 +212,35 @@
             param_num = param_desc.num.value
         for setting in param_desc.setting_list:
             setting_node = BranchNode(setting_num)
             if setting.name_string is not None:
                 setting_node.subnodes.append(TextNode("NAME", setting.name_string))
             if setting.desc_string is not None:
                 setting_node.subnodes.append(TextNode("DESC", setting.desc_string))
-            if setting.type == "int":
+            if setting.type == 'int':
                 setting_node.subnodes.append(BinaryNode("MASK", 1, param_num))
-                min_val = setting.min_val.uvalue if setting.min_val is not None else 0
-                max_val = setting.max_val.uvalue if setting.max_val is not None else 0xFFFFFFFF
-                def_val = setting.def_val.uvalue if setting.def_val is not None else 0
-                if min_val > max_val or def_val < min_val or def_val > max_val:
-                    generic.print_warning(
-                        generic.Warning.GENERIC,
-                        "Limits for GRF parameter {} are incoherent, ignoring.".format(param_num),
-                    )
-                    min_val = 0
-                    max_val = 0xFFFFFFFF
+                min_val = setting.min_val.value if setting.min_val is not None else 0
+                max_val = setting.max_val.value if setting.max_val is not None else 0xFFFFFFFF
                 setting_node.subnodes.append(LimitNode(min_val, max_val))
                 if len(setting.val_names) > 0:
                     value_names_node = BranchNode("VALU")
                     for set_val_pair in setting.val_names:
                         value_names_node.subnodes.append(TextNode(set_val_pair[0], set_val_pair[1]))
                     setting_node.subnodes.append(value_names_node)
             else:
-                assert setting.type == "bool"
+                assert setting.type == 'bool'
                 setting_node.subnodes.append(BinaryNode("TYPE", 1, 1))
                 bit = setting.bit_num.value if setting.bit_num is not None else 0
                 setting_node.subnodes.append(SettingMaskNode(param_num, bit, 1))
             if setting.def_val is not None:
                 setting_node.subnodes.append(BinaryNode("DFLT", 4, setting.def_val.value))
             param_root.subnodes.append(setting_node)
             setting_num += 1
         param_num += 1
     if len(param_root.subnodes) > 0:
         root.subnodes.append(param_root)
 
-
 def PaletteAction(pal):
     root = BranchNode("INFO")
     pal_node = UsedPaletteNode(pal)
     root.subnodes.append(pal_node)
     return [Action14([root])]
```

### Comparing `nml-0.7.2/nml/actions/action2.py` & `nml-r1512/nml/actions/action2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,59 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic, global_constants
+from nml import generic
 from nml.actions import base_action
-from nml.ast import base_statement, general
-
-total_action2_ids = 0x100
-free_action2_ids = list(range(0, total_action2_ids))
-
-"""
-Statistics about spritegroups.
-The 1st field of type C{int} contains the largest number of concurrently active spritegroup ids.
-The 2nd field of type L{Position} contains a positional reference
-  to the last spritegroup of the concurrently active ones.
-"""
-spritegroup_stats = (0, None)
-
-total_tmp_locations = 0x7F
-
-"""
-Statistics about temporary Action2 registers.
-The 1st field of type C{int} contains the largest number of concurrently active register ids.
-The 2nd field of type L{Position} contains a positional reference to the spritegroup.
-"""
-a2register_stats = (0, None)
-
-
-def print_stats():
-    """
-    Print statistics about used ids.
-    """
-    if spritegroup_stats[0] > 0:
-        generic.print_info(
-            "Concurrent spritegroups: {}/{} ({})".format(
-                spritegroup_stats[0], total_action2_ids, str(spritegroup_stats[1])
-            )
-        )
-    if a2register_stats[0] > 0:
-        generic.print_info(
-            "Concurrent Action2 registers: {}/{} ({})".format(
-                a2register_stats[0], total_tmp_locations, str(a2register_stats[1])
-            )
-        )
+from nml.ast import base_statement
+import nml
 
+free_action2_ids = list(range(1, 255))
 
 class Action2(base_action.BaseAction):
     """
     Abstract Action2 base class.
 
-    @ivar name: Name of the action2.
+    @ivar name; Name of the action2.
     @type name: C{str}
 
     @ivar feature: Action2 feature byte.
     @type feature: C{int}
 
-    @ivar pos: Position reference to source.
-    @type pos: L{Position}
-
     @ivar num_refs: Number of references to this action2.
     @type num_refs: C{int}
 
     @ivar id: Number of this action2.
     @type id: C{int}, or C{None} if no number is allocated yet.
 
     @ivar references: All Action2s that are referenced by this Action2.
     @type references: C{list} of L{Action2Reference}
 
     @ivar tmp_locations: List of address in the temporary storage that are free
                          to be used in this varaction2.
     @type tmp_locations: C{list} of C{int}
     """
-
-    def __init__(self, feature, name, pos):
+    def __init__(self, feature, name):
         self.feature = feature
         self.name = name
-        self.pos = pos
         self.num_refs = 0
         self.id = None
         self.references = []
-        # 0x00 - 0x7F: available to user
-        # 0x80 - 0xFE: used by NML
-        # 0xFF: Used for some house variables
-        # 0x100 - 0x10F: Special meaning (used for some CB results)
-        self.tmp_locations = list(range(0x80, 0x80 + total_tmp_locations))
+        #0x00 - 0x7F: available to user
+        #0x80 - 0x85: used for production CB
+        #0x86 - 0x100: available as temp. registers
+        self.tmp_locations = list(range(0x86, 0x100))
 
-    def prepare_output(self, sprite_num):
+    def prepare_output(self):
         free_references(self)
 
-        global spritegroup_stats
-
-        try:
-            if self.num_refs == 0:
-                self.id = free_action2_ids[0]
-            else:
-                self.id = free_action2_ids.pop()
-                num_used = total_action2_ids - len(free_action2_ids)
-                if num_used > spritegroup_stats[0]:
-                    spritegroup_stats = (num_used, self.pos)
-        except IndexError:
-            raise generic.ScriptError(
-                "Unable to allocate ID for [random]switch, sprite set/layout/group or produce-block."
-                " Try reducing the number of such blocks.",
-                self.pos,
-            )
+        if self.num_refs == 0:
+            self.id = free_action2_ids[0]
+        else:
+            self.id = free_action2_ids.pop()
 
-    def write_sprite_start(self, file, size, extra_comment=None):
-        assert self.num_refs == 0, "Action2 reference counting has {:d} dangling references.".format(self.num_refs)
+    def write_sprite_start(self, file, size):
+        assert self.num_refs == 0, "Action2 reference counting has %d dangling references." % self.num_refs
         file.comment("Name: " + self.name)
-        if extra_comment:
-            for c in extra_comment:
-                file.comment(c)
         file.start_sprite(size + 3)
         file.print_bytex(2)
         file.print_bytex(self.feature)
         file.print_bytex(self.id)
 
     def skip_action7(self):
         return False
@@ -147,44 +75,35 @@
         @param location: Number of the storage register to remove.
         @type location: C{int}
 
         @param force_recursive: Force removing this location recursively,
                                 also for 'chained' action2s.
         @type force_recursive: C{bool}
         """
-        global a2register_stats
-
-        if location in self.tmp_locations:
-            self.tmp_locations.remove(location)
-            num_used = total_tmp_locations - len(self.tmp_locations)
-            if num_used > a2register_stats[0]:
-                a2register_stats = (num_used, self.pos)
-
+        if location not in self.tmp_locations: return
+        self.tmp_locations.remove(location)
         for act2_ref in self.references:
             if force_recursive or act2_ref.is_proc:
                 act2_ref.action2.remove_tmp_location(location, True)
 
-
 class Action2Reference:
     """
     Container class to store information about an action2 reference
 
     @ivar action2: The target action2
     @type action2: L{Action2}
 
     @ivar is_proc: Whether this reference is made because of a procedure call
     @type is_proc: C{bool}
     """
-
     def __init__(self, action2, is_proc):
         self.action2 = action2
         self.is_proc = is_proc
 
-
-def add_ref(ref, source_action, reference_as_proc=False):
+def add_ref(ref, source_action, reference_as_proc = False):
     """
     Add a reference to a certain action2.
     This is needed so we can correctly reserve / free action2 IDs later on.
     To be called when creating the actions from the AST.
 
     @param ref: Reference to the sprite group that corresponds to the action2.
     @type ref: L{SpriteGroupRef}
@@ -194,69 +113,79 @@
 
     @param reference_as_proc: True iff the reference source is a procedure call,
                               which needs special precautions for temp registers.
     @type reference_as_proc: C{bool}
     """
 
     # Add reference to list of references of the source action
-    act2 = ref.act2 if ref.act2 is not None else resolve_spritegroup(ref.name).get_action2(source_action.feature)
+    if ref.name.value == 'CB_FAILED': return
+    act2 = ref.act2 if ref.act2 is not None else resolve_spritegroup(ref.name).get_action2()
     source_action.references.append(Action2Reference(act2, reference_as_proc))
     act2.num_refs += 1
 
-
 def free_references(source_action):
     """
     Free all references to other action2s from a certain action 2/3
 
     @param source_action: Action that contains the reference
     @type  source_action: L{Action2} or L{Action3}
     """
     for act2_ref in source_action.references:
         act2 = act2_ref.action2
         act2.num_refs -= 1
-        if act2.num_refs == 0:
-            free_action2_ids.append(act2.id)
+        if act2.num_refs == 0: free_action2_ids.append(act2.id)
 
-
-# Features using sprite groups directly: vehicles, stations, canals, cargos, railtypes, airports, roadtypes, tramtypes
-features_sprite_group = [0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x0B, 0x0D, 0x10, 0x12, 0x13]
-# Features using sprite layouts: houses, industry tiles, objects, airport tiles, and road stops
-features_sprite_layout = [0x07, 0x09, 0x0F, 0x11, 0x14]
+# Features using sprite groups directly: vehicles, canals, cargos, railtypes, airports
+features_sprite_group = [0x00, 0x01, 0x02, 0x03, 0x05, 0x0B, 0x0D, 0x10]
+# Features using sprite layouts: stations, houses, industry tiles, objects and airport tiles
+features_sprite_layout = [0x04, 0x07, 0x09, 0x0F, 0x11]
 # All features that need sprite sets
 features_sprite_set = features_sprite_group + features_sprite_layout
 
+class SpriteGroupRefType:
+    """
+    'Enum'-class that stores the various types of references that are possible
+    """
+    NONE = 0 # No possible references
+    SPRITESET = 1 # References to sprite sets
+    SPRITEGROUP = 2 # References to sprite groups
+    ALL = 3 # References to both sprite sets and groups
 
-def make_sprite_group_class(cls_is_spriteset, cls_is_referenced, cls_has_explicit_feature, cls_is_relocatable=False):
+def make_sprite_group_class(cls_own_type, cls_referring_to_type, cls_referred_by_type, cls_has_explicit_feature, cls_allow_parameters = False, cls_is_relocatable = False):
     """
     Metaclass factory which makes base classes for all nodes 'Action 2 graph'
     This graph is made up of all blocks that are eventually compiled to Action2,
-    which use the same name space. Spritesets do inherit from this class to make
-    referencing them possible, but they are not part of the refernce graph that
-    is built.
+    which use the same name space.
 
-    @param cls_is_spriteset: Whether this class represents a spriteset
-    @type cls_is_spriteset: C{bool}
+    @param cls_own_type: Type of instances of this class
+    @type cls_own_type: C{int} (values from L{SpriteGroupRefType})
 
-    @param cls_is_referenced: True iff this node can be referenced by other nodes
-    @type cls_is_referenced: C{bool}
+    @param cls_referring_to_type: Types of items that instances of this class may refer to
+    @type cls_referring_to_type: C{int} (values from L{SpriteGroupRefType})
+
+    @param cls_referred_by_type: Types of items that may refer to an instance of this class
+    @type cls_referred_by_type: C{int} (values from L{SpriteGroupRefType})
 
     @param cls_has_explicit_feature: Whether the feature of an instance is explicitly set,
                                     or derived from nodes that link to it.
     @type cls_has_explicit_feature: C{bool}
 
+    @param cls_allow_parameters: Whether parameters can be passed when referencing to an instance of this class.
+                                    If true, the derived class is expected to have a C{param_list} variable
+    @type cls_allow_parameters: C{bool}
+
     @param cls_is_relocatable: Whether instances of this class can be freely moved around or whether they need
                                to to be converted to nfo code at the same location as they are in the nml code.
     @type cls_is_relocatable: C{bool}
 
     @return: The constructed class
     @rtype: C{type}
     """
-
-    # without either references or an explicit feature, we have nothing to base our feature on
-    assert cls_is_referenced or cls_has_explicit_feature
+    #without either references or an explicit feature, we have nothing to base our feature on
+    assert cls_referred_by_type != SpriteGroupRefType.NONE or cls_has_explicit_feature
 
     class ASTSpriteGroup(base_statement.BaseStatement):
         """
         Abstract base class for all AST nodes that represent a sprite group
         This handles all the relations between the various nodes
 
         Child classes should do the following:
@@ -271,131 +200,111 @@
 
         @ivar _referenced_nodes: Set of nodes that this node refers to
         @type _referenced_nodes: C{set}
 
         @ivar _prepared: True iff prepare_output has already been executed
         @type _prepared: C{bool}
 
-        @ivar _action2: Mapping of features to action2s
-        @type _action2: C{dict} that maps C{int} to L{Action2}
+        @ivar _action2: Reference to the action2 that corresponds to this node, if applicable
+        @type _action2: L{Action2}, or C{None} if N/A
 
-        @ivar feature_set: Set of features that use this node
-        @type feature_set: C{set} of C{int}
+        @ivar feature: Feature of this node
+        @type feature: L{ConstantNumeric}
 
         @ivar name: Name of this node, as declared by the user
         @type name: L{Identifier}
-
-        @ivar num_params: Number of parameters that can be (and have to be) passed
-        @type num_params: C{int}
-
-        @ivar used_sprite_sets: List of sprite sets used by this node
-        @type used_sprite_sets: C{list} of L{SpriteSet}
         """
-
         def __init__(self):
             """
             Subclasses should implement their own __init__ method.
             This method should not be called, because calling a method on a meta class can be troublesome.
             Instead, call initialize(..).
             """
-            raise NotImplementedError(
-                (
-                    "__init__ must be implemented in ASTSpriteGroup-subclass {!r},"
-                    " initialize(..) should be called instead"
-                ).format(type(self))
-            )
+            raise NotImplementedError('__init__ must be implemented in ASTSpriteGroup-subclass %r, initialize(..) should be called instead' % type(self))
 
-        def initialize(self, name=None, feature=None, num_params=0):
+        def initialize(self, name = None, feature = None):
             """
             Initialize this instance.
             This function is generally, but not necessarily, called from the child class' constructor.
             Calling it later (during pre-processing) is also possible, as long as it's called
             before any other actions are done.
 
-            @param name: Name of this node, as set by the user (if applicable)
-                            Should be be set (not None) iff cls_is_referenced is True
-            @type name: L{Identifier} or C{None} if N/A
+            @param name: Name of this node, as set by the user
+                            Should be be set (not None) iff cls_referred_by_type != SpriteGroupRefType.NONE
+            @type name: L{Identifier}
 
             @param feature: Feature of this node, if set by the user.
                                 Should be set (not None) iff cls_has_explicit_feature is True
-            @type feature: C{int} or C{None}
+            @type feature: L{ConstantNumeric}
             """
             assert not (self._has_explicit_feature() and feature is None)
-            assert not (cls_is_referenced and name is None)
+            assert self._referred_by_type() == SpriteGroupRefType.NONE or name is not None
             self._referencing_nodes = set()
             self._referenced_nodes = set()
             self._prepared = False
-            self._action2 = {}
-            self.feature_set = {feature} if feature is not None else set()
+            self._action2 = None
+            self.feature = feature
             self.name = name
-            self.num_params = num_params
-            self.used_sprite_sets = []
-            self.optimised = None
 
         def register_names(self):
-            if cls_is_relocatable and cls_is_referenced:
+            if cls_is_relocatable and self._referred_by_type() != SpriteGroupRefType.NONE:
                 register_spritegroup(self)
 
         def pre_process(self):
             """
             Pre-process this node.
             During this stage, the reference graph is built.
             """
-            refs = self.collect_references()
-            for ref in refs:
-                self._add_reference(ref)
-            if (not cls_is_relocatable) and cls_is_referenced:
+            if self._referring_to_type() != SpriteGroupRefType.NONE:
+                refs = self.collect_references()
+                for ref in refs:
+                    self._add_reference(ref)
+            if not cls_is_relocatable and self._referred_by_type() != SpriteGroupRefType.NONE:
                 register_spritegroup(self)
 
-        def prepare_act2_output(self):
+        def prepare_output(self):
             """
             Prepare this node for outputting.
             This sets the feature and makes sure it is correct.
 
             @return: True iff parsing of this node is needed
             @rtype: C{bool}
             """
-            if not cls_is_referenced:
-                return True
+            if self._referred_by_type() == SpriteGroupRefType.NONE: return True
             if not self._prepared:
                 self._prepared = True
                 # copy, since we're going to modify
                 ref_nodes = self._referencing_nodes.copy()
                 for node in ref_nodes:
-                    used = node.prepare_act2_output()
+                    used = node.prepare_output()
                     if not used:
                         node._remove_reference(self)
 
                 # now determine the feature
                 if self._has_explicit_feature():
                     # by this time, feature should be set
-                    assert len(self.feature_set) == 1
-                    for n in self._referencing_nodes:
-                        if n.feature_set != self.feature_set:
-                            msg = "Cannot refer to block '{}' with feature '{}', expected feature is '{}'"
-                            msg = msg.format(
-                                self.name.value,
-                                general.feature_name(next(iter(self.feature_set))),
-                                general.feature_name(n.feature_set.difference(self.feature_set).pop()),
-                            )
-                            raise generic.ScriptError(msg, n.pos)
-
+                    assert self.feature is not None
                 elif len(self._referencing_nodes) != 0:
                     for n in self._referencing_nodes:
-                        # Add the features from all calling blocks to the set
-                        self.feature_set.update(n.feature_set)
+                        # get the feature of the first item in the set
+                        self.feature = n.feature
+                        break
+
+                for node in self._referencing_nodes:
+                    if node.feature.value != self.feature.value:
+                        if self._has_explicit_feature():
+                            msg = "Cannot refer to block '%s' with feature '%02X', expected feature is '%02X'"
+                        else:
+                            msg = "Block '%s' cannot be used for feature '%02X' (already used for feature '%02X')"
+                        raise generic.ScriptError(msg % (self.name.value, self.feature.value, node.feature.value), node.pos)
 
-                if len(self._referencing_nodes) == 0 and (not self.optimised or self.optimised is self):
+                if len(self._referencing_nodes) == 0:
                     # if we can be 'not used', there ought to be a way to refer to this block
                     assert self.name is not None
-                    generic.print_warning(
-                        generic.Warning.OPTIMISATION,
-                        "Block '{}' is not referenced, ignoring.".format(self.name.value),
-                        self.pos,
-                    )
+                    generic.print_warning("Block '%s' is not referenced, ignoring." % self.name.value, self.pos)
 
             return len(self._referencing_nodes) != 0
 
         def referenced_nodes(self):
             """
             Get the nodes that this node refers to.
             @note: Make sure to sort this in a deterministic way when the order of items affects the output.
@@ -412,152 +321,117 @@
 
             @return: A set of nodes
             @rtype: C{set} of L{ASTSpriteGroup}
             """
 
             return self._referencing_nodes
 
-        def optimise(self):
-            """
-            Optimise this sprite group.
-
-            @return: True iff this sprite group has been optimised
-            @rtype: C{bool}
-            """
-            return False
-
         def collect_references(self):
             """
             This function should collect all references to other nodes from this instance.
+            It must be implemented and called iff the C{cls_referring_to_type} metaclass parameter is not 0
 
             @return: A collection containing all links to other nodes.
             @rtype: C{iterable} of L{SpriteGroupRef}
             """
-            raise NotImplementedError(
-                "collect_references must be implemented in ASTSpriteGroup-subclass {!r}".format(type(self))
-            )
+            assert self._referring_to_type() != SpriteGroupRefType.NONE
+            raise NotImplementedError('collect_references must be implemented in ASTSpriteGroup-subclass %r' % type(self))
 
-        def set_action2(self, action2, feature):
+        def set_action2(self, action2):
             """
             Set this node's resulting action2
 
-            @param feature: Feature of the Action2
-            @type feature: C{int}
-
             @param action2: Action2 to set
             @type action2: L{Action2}
             """
-            assert feature not in self._action2
-            self._action2[feature] = action2
+            assert self._own_type() == SpriteGroupRefType.SPRITEGROUP
+            assert self._action2 is None
+            self._action2 = action2
 
-        def get_action2(self, feature):
+        def get_action2(self):
             """
             Get this node's resulting action2
 
-            @param feature: Feature of the Action2
-            @type feature: C{int}
-
             @return: Action2 to get
             @rtype: L{Action2}
             """
-            assert feature in self._action2
-            return self._action2[feature]
-
-        def has_action2(self, feature):
-            """
-            Check, if this node already has an action2 for a given feature
-
-            @param feature: Feature to check
-            @type feature: C{int}
-
-            @return: True iff there is an action2 for this feature
-            @rtype: C{bool}
-            """
-            return feature in self._action2
+            assert self._own_type() == SpriteGroupRefType.SPRITEGROUP
+            assert self._action2 is not None
+            return self._action2
 
         def _add_reference(self, target_ref):
             """
             Add a reference from C{self} to a target with a given name.
 
             @param target_ref: Name of the reference target
             @type target_ref: L{SpriteGroupRef}
             """
 
-            if target_ref.name.value == "CB_FAILED":
-                return
-
             target = resolve_spritegroup(target_ref.name)
-            if target.is_spriteset():
-                assert target.num_params == 0
-                # Referencing a spriteset directly from graphics/[random]switch
-                # Passing parameters is not possible here
-                if len(target_ref.param_list) != 0:
-                    raise generic.ScriptError(
-                        "Passing parameters to '{}' is only possible from a spritelayout.".format(
-                            target_ref.name.value
-                        ),
-                        target_ref.pos,
-                    )
-
-                self.used_sprite_sets.append(target)
-            else:
-                if len(target_ref.param_list) != target.num_params:
-                    msg = "'{}' expects {:d} parameters, encountered {:d}."
-                    msg = msg.format(target_ref.name.value, target.num_params, len(target_ref.param_list))
-                    raise generic.ScriptError(msg, target_ref.pos)
-
-                self._referenced_nodes.add(target)
-                target._referencing_nodes.add(self)
+            if (target._own_type() & self._referring_to_type() == 0) or \
+                    (self._own_type() & target._referred_by_type() == 0):
+                raise generic.ScriptError("Encountered an incorrect type of reference: '%s'" % target_ref.name.value, target_ref.pos)
+            if len(target_ref.param_list) != 0 and not target._allow_parameters():
+                raise generic.ScriptError("Passing parameters to '%s' is not possible." % target_ref.name.value, target_ref.pos)
+            self._referenced_nodes.add(target)
+            target._referencing_nodes.add(self)
 
         def _remove_reference(self, target):
             """
             Add a reference from C{self} to a target
 
             @param target: Existing reference target to be removed
             @type target: L{ASTSpriteGroup}
             """
             assert target in self._referenced_nodes
             assert self in target._referencing_nodes
             self._referenced_nodes.remove(target)
             target._referencing_nodes.remove(self)
 
-        # Make metaclass arguments available outside of the class
-        def is_spriteset(self):
-            return cls_is_spriteset
+        #Make metaclass arguments available
+        def _own_type(self):
+            return cls_own_type
+
+        def _referring_to_type(self):
+            return cls_referring_to_type
+
+        def _referred_by_type(self):
+            return cls_referred_by_type
 
         def _has_explicit_feature(self):
             return cls_has_explicit_feature
 
-    return ASTSpriteGroup
+        def _allow_parameters(self):
+            return cls_allow_parameters
 
+    return ASTSpriteGroup
 
-# list of all registered sprite sets and sprite groups
+#list of all registered sprite sets and sprite groups
 spritegroup_list = {}
 
-
 def register_spritegroup(spritegroup):
     """
     Register a sprite group, so it can be resolved by name later
 
     @param spritegroup: Sprite group to register
     @type spritegroup: L{ASTSpriteGroup}
     """
     name = spritegroup.name.value
     if name in spritegroup_list:
-        raise generic.ScriptError("Block with name '{}' has already been defined".format(name), spritegroup.pos)
+        raise generic.ScriptError("Block with name '%s' has already been defined" % name, spritegroup.pos)
     spritegroup_list[name] = spritegroup
-    global_constants.spritegroups[name] = name
-
+    nml.global_constants.spritegroups[name] = name
 
 def resolve_spritegroup(name):
     """
     Resolve a sprite group with a given name
 
     @param name: Name of the sprite group.
     @type name: L{Identifier}
 
     @return: The sprite group that the name refers to.
     @rtype: L{ASTSpriteGroup}
     """
     if name.value not in spritegroup_list:
-        raise generic.ScriptError("Unknown identifier encountered: '{}'".format(name.value), name.pos)
+        raise generic.ScriptError("Unknown identifier encountered: '%s'" % name.value, name.pos)
     return spritegroup_list[name.value]
+
```

### Comparing `nml-0.7.2/nml/actions/action2layout.py` & `nml-r1512/nml/actions/action2layout.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,144 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic, nmlop
-from nml.actions import action0, action1, action2, action2real, action2var, action6, actionD, real_sprite
-from nml.ast import general, spriteblock
-
+from nml import generic, global_constants, expression, nmlop
+from nml.actions import action2, action6, actionD, action1, action2var, real_sprite
+from nml.ast import switch_range
 
 class Action2Layout(action2.Action2):
-    def __init__(self, feature, name, pos, layout, param_registers):
-        action2.Action2.__init__(self, feature, name, pos)
-        self.layout = layout
-        self.param_registers = param_registers
-
-    def resolve_tmp_storage(self):
-        for reg in self.param_registers:
-            if not self.tmp_locations:
-                raise generic.ScriptError(
-                    "There are not enough registers available "
-                    + "to perform all required computations in switch blocks. "
-                    + "Please reduce the complexity of your code.",
-                    self.pos,
-                )
-            location = self.tmp_locations[0]
-            self.remove_tmp_location(location, False)
-            reg.set_register(location)
+    def __init__(self, feature, name, ground_sprite, sprite_list):
+        action2.Action2.__init__(self, feature, name)
+        assert ground_sprite.type == Action2LayoutSpriteType.GROUND
+        self.ground_sprite = ground_sprite
+        self.sprite_list = sprite_list
 
     def write(self, file):
-        size = self.layout.get_size()
-        regs = ["{} : register {:X}".format(reg.name, reg.register) for reg in self.param_registers]
-        action2.Action2.write_sprite_start(self, file, size, regs)
-        self.layout.write(file)
+        advanced = any(x.is_advanced_sprite() for x in self.sprite_list + [self.ground_sprite])
+        size = 5
+        if advanced: size += self.ground_sprite.get_registers_size()
+        for sprite in self.sprite_list:
+            if sprite.type == Action2LayoutSpriteType.CHILD:
+                size += 7
+            else:
+                size += 10
+            if advanced: size += sprite.get_registers_size()
+        if len(self.sprite_list) == 0:
+            size += 9
+
+        action2.Action2.write_sprite_start(self, file, size)
+        if advanced:
+            file.print_byte(0x40 | len(self.sprite_list))
+        else:
+            file.print_byte(len(self.sprite_list))
+        self.ground_sprite.write_sprite_number(file)
+        if advanced:
+            self.ground_sprite.write_flags(file)
+            self.ground_sprite.write_registers(file)
+        file.newline()
+        if len(self.sprite_list) == 0:
+            file.print_dwordx(0) #sprite number 0 == no sprite
+            for i in range(0, 5):
+                file.print_byte(0) #empty bounding box. Note that number of zeros is 5, not 6
+        else:
+            for sprite in self.sprite_list:
+                sprite.write_sprite_number(file)
+                if advanced: sprite.write_flags(file)
+                file.print_byte(sprite.get_param('xoffset').value)
+                file.print_byte(sprite.get_param('yoffset').value)
+                if sprite.type == Action2LayoutSpriteType.CHILD:
+                    file.print_bytex(0x80)
+                else:
+                    #normal building sprite
+                    file.print_byte(sprite.get_param('zoffset').value)
+                    file.print_byte(sprite.get_param('xextent').value)
+                    file.print_byte(sprite.get_param('yextent').value)
+                    file.print_byte(sprite.get_param('zextent').value)
+                if advanced: sprite.write_registers(file)
+                file.newline()
         file.end_sprite()
 
 
-class Action2LayoutSpriteType:
-    GROUND = 0
+class Action2LayoutSpriteType(object):
+    GROUND   = 0
     BUILDING = 1
-    CHILD = 2
-
+    CHILD    = 2
 
-# these keywords are used to identify a ground/building/childsprite
+#these keywords are used to identify a ground/building/childsprite
 layout_sprite_types = {
-    "ground": Action2LayoutSpriteType.GROUND,
-    "building": Action2LayoutSpriteType.BUILDING,
-    "childsprite": Action2LayoutSpriteType.CHILD,
+    'ground'      : Action2LayoutSpriteType.GROUND,
+    'building'    : Action2LayoutSpriteType.BUILDING,
+    'childsprite' : Action2LayoutSpriteType.CHILD,
 }
 
-
-class Action2LayoutSprite:
-    def __init__(self, feature, type, pos=None, extra_dicts=None):
-        self.feature = feature
+class Action2LayoutSprite(object):
+    def __init__(self, type, pos = None):
         self.type = type
         self.pos = pos
-        self.extra_dicts = extra_dicts or []
         self.params = {
-            "sprite": {"value": None, "validator": self._validate_sprite},
-            "recolour_mode": {"value": 0, "validator": self._validate_recolour_mode},
-            "palette": {"value": expression.ConstantNumeric(0), "validator": self._validate_palette},
-            "always_draw": {"value": 0, "validator": self._validate_always_draw},
-            "xoffset": {"value": expression.ConstantNumeric(0), "validator": self._validate_bounding_box},
-            "yoffset": {"value": expression.ConstantNumeric(0), "validator": self._validate_bounding_box},
-            "zoffset": {"value": expression.ConstantNumeric(0), "validator": self._validate_bounding_box},
-            "xextent": {"value": expression.ConstantNumeric(16), "validator": self._validate_bounding_box},
-            "yextent": {"value": expression.ConstantNumeric(16), "validator": self._validate_bounding_box},
-            "zextent": {"value": expression.ConstantNumeric(16), "validator": self._validate_bounding_box},
-            "hide_sprite": {"value": None, "validator": self._validate_hide_sprite},  # Value not used
+            'sprite'        : {'value': None, 'validator': self._validate_sprite},
+            'recolour_mode' : {'value': 0,  'validator': self._validate_recolour_mode},
+            'palette'       : {'value': expression.ConstantNumeric(0), 'validator': self._validate_palette},
+            'always_draw'   : {'value': 0,  'validator': self._validate_always_draw},
+            'xoffset'       : {'value': expression.ConstantNumeric(0),  'validator': self._validate_bounding_box},
+            'yoffset'       : {'value': expression.ConstantNumeric(0),  'validator': self._validate_bounding_box},
+            'zoffset'       : {'value': expression.ConstantNumeric(0),  'validator': self._validate_bounding_box},
+            'xextent'       : {'value': expression.ConstantNumeric(16), 'validator': self._validate_bounding_box},
+            'yextent'       : {'value': expression.ConstantNumeric(16), 'validator': self._validate_bounding_box},
+            'zextent'       : {'value': expression.ConstantNumeric(16), 'validator': self._validate_bounding_box},
+            'hide_sprite'   : {'value': None, 'validator': self._validate_hide_sprite}, # Value not used
         }
         for i in self.params:
-            self.params[i]["is_set"] = False
-            self.params[i]["register"] = None
+            self.params[i]['is_set'] = False
+            self.params[i]['register'] = None
         self.sprite_from_action1 = False
         self.palette_from_action1 = False
-        self.var10_for_sprite = None
-        self.var10_for_palette = None
 
     def is_advanced_sprite(self):
-        if self.feature == 0x04:
-            return True
-        if self.palette_from_action1:
-            return True
+        if self.palette_from_action1: return True
         return len(self.get_all_registers()) != 0
 
     def get_registers_size(self):
         # Number of registers to write
         size = len(self.get_all_registers())
-        # Add station specific registers
-        if self.feature == 0x04:
-            if self.var10_for_sprite:
-                size += 1
-            if self.var10_for_palette:
-                size += 1
         # Add 2 for the flags
         size += 2
         return size
 
     def write_flags(self, file):
         flags = 0
-        if self.get_register("hide_sprite") is not None:
+        if self.get_register('hide_sprite') is not None:
             flags |= 1 << 0
-        if self.get_register("sprite") is not None:
+        if self.get_register('sprite') is not None:
             flags |= 1 << 1
-        if self.get_register("palette") is not None:
+        if self.get_register('palette') is not None:
             flags |= 1 << 2
         if self.palette_from_action1:
             flags |= 1 << 3
-        # for building sprites: bit 4 => xoffset+yoffset, bit 5 => zoffset (x and y always set totgether)
-        # for child sprites: bit 4 => xoffset, bit 5 => yoffset
-        if self.type == Action2LayoutSpriteType.BUILDING:
-            assert (self.get_register("xoffset") is not None) == (self.get_register("yoffset") is not None)
-        if self.get_register("xoffset") is not None:
+        assert (self.get_register('xoffset') is not None) == (self.get_register('yoffset') is not None)
+        if self.get_register('xoffset') is not None:
             flags |= 1 << 4
-        nextreg = "zoffset" if self.type == Action2LayoutSpriteType.BUILDING else "yoffset"
-        if self.get_register(nextreg) is not None:
+        if self.get_register('zoffset') is not None:
             flags |= 1 << 5
-        if self.feature == 0x04:
-            if self.var10_for_sprite is not None:
-                flags |= 1 << 6
-            if self.var10_for_palette is not None:
-                flags |= 1 << 7
         file.print_wordx(flags)
 
     def write_register(self, file, name):
         register = self.get_register(name)[0]
         file.print_bytex(register.parameter)
 
     def write_registers(self, file):
-        if self.is_set("hide_sprite"):
-            self.write_register(file, "hide_sprite")
-        if self.get_register("sprite") is not None:
-            self.write_register(file, "sprite")
-        if self.get_register("palette") is not None:
-            self.write_register(file, "palette")
-        if self.get_register("xoffset") is not None:
-            self.write_register(file, "xoffset")
-        if self.get_register("yoffset") is not None:
-            self.write_register(file, "yoffset")
-        if self.get_register("zoffset") is not None:
-            self.write_register(file, "zoffset")
-        if self.feature == 0x04:
-            if self.var10_for_sprite is not None:
-                file.print_bytex(self.var10_for_sprite)
-            if self.var10_for_palette is not None:
-                file.print_bytex(self.var10_for_palette)
+        if self.is_set('hide_sprite'):
+            self.write_register(file, 'hide_sprite')
+        if self.get_register('sprite') is not None:
+            self.write_register(file, 'sprite')
+        if self.get_register('palette') is not None:
+            self.write_register(file, 'palette')
+        assert (self.get_register('xoffset') is not None) == (self.get_register('yoffset') is not None)
+        if self.get_register('xoffset') is not None:
+            self.write_register(file, 'xoffset')
+            self.write_register(file, 'yoffset')
+        if self.get_register('zoffset') is not None:
+            self.write_register(file, 'zoffset')
 
     def write_sprite_number(self, file):
         num = self.get_sprite_number()
         if isinstance(num, expression.ConstantNumeric):
             num.write(file, 4)
         else:
             file.print_dwordx(0)
@@ -165,585 +146,296 @@
     def get_sprite_number(self):
         # Layout of sprite number
         # bit  0 - 13: Sprite number
         # bit 14 - 15: Recolour mode (normal/transparent/remap)
         # bit 16 - 29: Palette sprite number
         # bit 30: Always draw sprite, even in transparent mode
         # bit 31: This is a custom sprite (from action1), not a TTD sprite
-        if not self.is_set("sprite"):
+        if not self.is_set('sprite'):
             raise generic.ScriptError("'sprite' must be set for this layout sprite", self.pos)
 
         # Make sure that recolouring is set correctly
-        if self.get_param("recolour_mode") == 0 and self.is_set("palette"):
+        if self.get_param('recolour_mode') == 0 and self.is_set('palette'):
             raise generic.ScriptError("'palette' may not be set when 'recolour_mode' is RECOLOUR_NONE.")
-        elif self.get_param("recolour_mode") != 0 and not self.is_set("palette"):
+        elif self.get_param('recolour_mode') != 0 and not self.is_set('palette'):
             raise generic.ScriptError("'palette' must be set when 'recolour_mode' is not set to RECOLOUR_NONE.")
 
-        # Add the constant terms first
-        sprite_num = self.get_param("recolour_mode") << 14
-        if self.get_param("always_draw"):
+        # add the constant terms first
+        sprite_num = self.get_param('recolour_mode') << 14
+        if self.get_param('always_draw'):
             sprite_num |= 1 << 30
         if self.sprite_from_action1:
             sprite_num |= 1 << 31
 
-        # Add the sprite
-        expr = nmlop.ADD(self.get_param("sprite"), sprite_num, self.pos)
-        # Add the palette
-        expr = nmlop.ADD(nmlop.SHIFT_LEFT(self.get_param("palette"), 16, self.pos), expr)
+        add_sprite = False
+        sprite = self.get_param('sprite')
+        if isinstance(sprite, expression.ConstantNumeric):
+            sprite_num |= sprite.value
+        else:
+            add_sprite = True
+
+        add_palette = False
+        palette = self.get_param('palette')
+        if isinstance(palette, expression.ConstantNumeric):
+            sprite_num |= palette.value << 16
+        else:
+            add_palette = True
+
+        expr = expression.ConstantNumeric(sprite_num, sprite.pos)
+        if add_sprite:
+            expr = expression.BinOp(nmlop.ADD, sprite, expr, sprite.pos)
+        if add_palette:
+            expr = expression.BinOp(nmlop.ADD, palette, expr, sprite.pos)
         return expr.reduce()
 
     def get_param(self, name):
         assert name in self.params
-        return self.params[name]["value"]
+        return self.params[name]['value']
 
     def is_set(self, name):
         assert name in self.params
-        return self.params[name]["is_set"]
+        return self.params[name]['is_set']
 
     def get_register(self, name):
         assert name in self.params
-        return self.params[name]["register"]
+        return self.params[name]['register']
 
     def get_all_registers(self):
-        return [self.get_register(name) for name in sorted(self.params) if self.get_register(name) is not None]
+        return [self.get_register(name) for name in self.params if self.get_register(name) is not None]
 
     def create_register(self, name, value):
-        if (
-            # Always copy values from "prepare_layout" into new registers, to prevent "default" from modifying them.
-            self.feature != 0x04
-            and isinstance(value, expression.StorageOp)
-            and value.name == "LOAD_TEMP"
-            and isinstance(value.register, expression.ConstantNumeric)
-        ):
+        if isinstance(value, expression.StorageOp) and value.name == "LOAD_TEMP" and isinstance(value.register, expression.ConstantNumeric):
             store_tmp = None
-            load_tmp = action2var.VarAction2Var(0x7D, 0, 0xFFFFFFFF, value.register.value)
+            load_tmp = action2var.VarAction2Var(0x7F, 0, 0xFFFFFFFF, value.register.value)
         else:
             store_tmp = action2var.VarAction2StoreTempVar()
             load_tmp = action2var.VarAction2LoadTempVar(store_tmp)
-        self.params[name]["register"] = (load_tmp, store_tmp, value)
+        self.params[name]['register'] = (load_tmp, store_tmp, value)
 
     def set_param(self, name, value):
         assert isinstance(name, expression.Identifier)
-        assert isinstance(value, expression.Expression)
+        assert isinstance(value, expression.Expression) or isinstance(value, expression.SpriteGroupRef)
         name = name.value
+        if name == 'ttdsprite':
+            name = 'sprite'
+            generic.print_warning("Using 'ttdsprite' in sprite layouts is deprecated, use 'sprite' instead", value.pos)
 
-        if name not in self.params:
-            raise generic.ScriptError("Unknown sprite parameter '{}'".format(name), value.pos)
+        if not name in self.params:
+            raise generic.ScriptError("Unknown sprite parameter '%s'" % name, value.pos)
         if self.is_set(name):
-            raise generic.ScriptError("Sprite parameter '{}' can be set only once per sprite.".format(name), value.pos)
+            raise generic.ScriptError("Sprite parameter '%s' can be set only once per sprite." % name, value.pos)
 
-        self.params[name]["value"] = self.params[name]["validator"](name, value)
-        self.params[name]["is_set"] = True
-
-    def _validate_offset(self, offset, spriteset, pos):
-        if len(offset) == 0:
-            offset = None
-        elif len(offset) == 1:
-            id_dicts = [
-                (spriteset.labels if spriteset else {}, lambda name, val, pos: expression.ConstantNumeric(val, pos))
-            ]
-            offset = action2var.reduce_varaction2_expr(
-                offset[0], action2var.get_scope(self.feature), self.extra_dicts + id_dicts
-            )
-            if spriteset and isinstance(offset, expression.ConstantNumeric):
-                generic.check_range(
-                    offset.value,
-                    0,
-                    len(real_sprite.parse_sprite_data(spriteset)) - 1,
-                    "offset within spriteset",
-                    pos,
-                )
-        else:
-            raise generic.ScriptError("Expected 0 or 1 parameter, got " + str(len(offset)), pos)
-        return offset
+        self.params[name]['value'] = self.params[name]['validator'](name, value)
+        self.params[name]['is_set'] = True
 
     def resolve_spritegroup_ref(self, sg_ref):
         """
         Resolve a reference to a (sprite/palette) sprite group
 
         @param sg_ref: Reference to a sprite group
         @type sg_ref: L{SpriteGroupRef}
 
         @return: Sprite number (index of action1 set) to use
         @rtype: L{Expression}
         """
         spriteset = action2.resolve_spritegroup(sg_ref.name)
-        offset = self._validate_offset(sg_ref.param_list, spriteset, sg_ref.pos)
+
+        if len(sg_ref.param_list) == 0:
+            offset = None
+        elif len(sg_ref.param_list) == 1:
+            id_dicts = [(spriteset.labels, lambda val, pos: expression.ConstantNumeric(val, pos))]
+            expression.identifier.ignore_all_invalid_ids = True
+            offset = sg_ref.param_list[0].reduce(global_constants.const_list + id_dicts)
+            expression.identifier.ignore_all_invalid_ids = False
+            if isinstance(offset, expression.ConstantNumeric):
+                generic.check_range(offset.value, 0, len(real_sprite.parse_sprite_list(spriteset.sprite_list, spriteset.pcx)) - 1, "offset within spriteset", sg_ref.pos)
+        else:
+            raise generic.ScriptError("Expected 0 or 1 parameter, got " + str(len(sg_ref.param_list)), sg_ref.pos)
+
         num = action1.get_action1_index(spriteset)
         generic.check_range(num, 0, (1 << 14) - 1, "sprite", sg_ref.pos)
         return expression.ConstantNumeric(num), offset
 
     def _validate_sprite(self, name, value):
         if isinstance(value, expression.SpriteGroupRef):
-            assert self.feature != 0x04
             self.sprite_from_action1 = True
             val, offset = self.resolve_spritegroup_ref(value)
             if offset is not None:
                 self.create_register(name, offset)
             return val
-        elif isinstance(value, StationSpriteset):
-            assert self.feature == 0x04
-            self.sprite_from_action1 = True
-            if value.offset is not None:
-                offset = self._validate_offset(value.offset, value.spriteset, value.pos)
-                if offset is not None:
-                    self.create_register(name, offset)
-            self.var10_for_sprite = value.var10
-            return expression.ConstantNumeric(0x42D)
         else:
             self.sprite_from_action1 = False
             if isinstance(value, expression.ConstantNumeric):
                 generic.check_range(value.value, 0, (1 << 14) - 1, "sprite", value.pos)
                 return value
-            if value.supported_by_actionD(raise_error=False):
-                return value
             self.create_register(name, value)
             return expression.ConstantNumeric(0)
 
     def _validate_recolour_mode(self, name, value):
         if not isinstance(value, expression.ConstantNumeric):
             raise generic.ScriptError("Expected a compile-time constant.", value.pos)
 
-        if value.value not in (0, 1, 2):
-            raise generic.ScriptError(
-                "Value of 'recolour_mode' must be RECOLOUR_NONE, RECOLOUR_TRANSPARENT or RECOLOUR_REMAP."
-            )
+        if not value.value in (0, 1, 2):
+            raise generic.ScriptError("Value of 'recolour_mode' must be RECOLOUR_NONE, RECOLOUR_TRANSPARENT or RECOLOUR_REMAP.")
         return value.value
 
     def _validate_palette(self, name, value):
         if isinstance(value, expression.SpriteGroupRef):
-            assert self.feature != 0x04
             self.palette_from_action1 = True
             val, offset = self.resolve_spritegroup_ref(value)
             if offset is not None:
                 self.create_register(name, offset)
             return val
-        elif isinstance(value, StationSpriteset):
-            assert self.feature == 0x04
-            self.palette_from_action1 = True
-            if value.offset is not None:
-                offset = self._validate_offset(value.offset, value.spriteset, value.pos)
-                if offset is not None:
-                    self.create_register(name, offset)
-            self.var10_for_palette = value.var10
-            return expression.ConstantNumeric(0x42D)
         else:
-            self.palette_from_action1 = False
             if isinstance(value, expression.ConstantNumeric):
                 generic.check_range(value.value, 0, (1 << 14) - 1, "palette", value.pos)
-                return value
-            if value.supported_by_actionD(raise_error=False):
-                return value
-            self.create_register(name, value)
-            return expression.ConstantNumeric(0)
+            self.palette_from_action1 = False
+            return value
 
     def _validate_always_draw(self, name, value):
         if not isinstance(value, expression.ConstantNumeric):
             raise generic.ScriptError("Expected a compile-time constant number.", value.pos)
         # Not valid for ground sprites, raise error
         if self.type == Action2LayoutSpriteType.GROUND:
-            raise generic.ScriptError(
-                "'always_draw' may not be set for groundsprites, these are always drawn anyways.", value.pos
-            )
+            raise generic.ScriptError("'always_draw' may not be set for groundsprites, these are always drawn anyways.", value.pos)
 
         if value.value not in (0, 1):
             raise generic.ScriptError("Value of 'always_draw' should be 0 or 1", value.pos)
         return value.value
 
     def _validate_bounding_box(self, name, value):
         if self.type == Action2LayoutSpriteType.GROUND:
             raise generic.ScriptError(name + " can not be set for ground sprites", value.pos)
         elif self.type == Action2LayoutSpriteType.CHILD:
-            if name not in ("xoffset", "yoffset"):
+            if name not in ('xoffset', 'yoffset'):
                 raise generic.ScriptError(name + " can not be set for child sprites", value.pos)
             if isinstance(value, expression.ConstantNumeric):
                 generic.check_range(value.value, 0, 255, name, value.pos)
                 return value
         else:
             assert self.type == Action2LayoutSpriteType.BUILDING
-            if name in ("xoffset", "yoffset", "zoffset"):
+            if name in ('xoffset', 'yoffset', 'zoffset'):
                 if isinstance(value, expression.ConstantNumeric):
                     generic.check_range(value.value, -128, 127, name, value.pos)
                     return value
             else:
-                assert name in ("xextent", "yextent", "zextent")
+                assert name in ('xextent', 'yextent', 'zextent')
                 if not isinstance(value, expression.ConstantNumeric):
-                    raise generic.ScriptError(
-                        "Value of '{}' must be a compile-time constant number.".format(name), value.pos
-                    )
+                    raise generic.ScriptError("Value of '%s' must be a compile-time constant number." % name, value.pos)
                 generic.check_range(value.value, 0, 255, name, value.pos)
                 return value
         # Value must be written to a register
         self.create_register(name, value)
-        if self.type == Action2LayoutSpriteType.BUILDING:
-            # For building sprites, x and y registers are always written together
-            if name == "xoffset" and self.get_register("yoffset") is None:
-                self.create_register("yoffset", expression.ConstantNumeric(0))
-            if name == "yoffset" and self.get_register("xoffset") is None:
-                self.create_register("xoffset", expression.ConstantNumeric(0))
+        if name == 'xoffset' and self.get_register('yoffset') is None:
+            self.create_register('yoffset', expression.ConstantNumeric(0))
+        if name == 'yoffset' and self.get_register('xoffset') is None:
+            self.create_register('xoffset', expression.ConstantNumeric(0))
         return expression.ConstantNumeric(0)
 
     def _validate_hide_sprite(self, name, value):
-        self.create_register(name, expression.Not(value).reduce())
-
-
-class ParsedSpriteLayout:
-    def __init__(self, registers=None):
-        self.ground_sprite = None
-        self.building_sprites = []
-        self.registers = registers or []
-        self.advanced = False
+        self.create_register(name, expression.Not(value))
+        return None
 
-    def get_size(self):
-        size = 5
-        if self.advanced:
-            size += self.ground_sprite.get_registers_size()
-        for sprite in self.building_sprites:
-            if sprite.type == Action2LayoutSpriteType.CHILD:
-                size += 7
-            else:
-                size += 10
-            if self.advanced:
-                size += sprite.get_registers_size()
-        if len(self.building_sprites) == 0 and not self.advanced:
-            size += 9
-        return size
-
-    def write(self, file):
-        if self.advanced:
-            file.print_byte(0x40 | len(self.building_sprites))
-        else:
-            file.print_byte(len(self.building_sprites))
-        self.ground_sprite.write_sprite_number(file)
-        if self.advanced:
-            self.ground_sprite.write_flags(file)
-            self.ground_sprite.write_registers(file)
-        file.newline()
-        if len(self.building_sprites) == 0 and not self.advanced:
-            file.print_dwordx(0)  # sprite number 0 == no sprite
-            for _ in range(0, 5):
-                file.print_byte(0)  # empty bounding box. Note that number of zeros is 5, not 6
-        else:
-            for sprite in self.building_sprites:
-                sprite.write_sprite_number(file)
-                if self.advanced:
-                    sprite.write_flags(file)
-                file.print_byte(sprite.get_param("xoffset").value)
-                file.print_byte(sprite.get_param("yoffset").value)
-                if sprite.type == Action2LayoutSpriteType.CHILD:
-                    file.print_bytex(0x80)
-                else:
-                    # normal building sprite
-                    file.print_byte(sprite.get_param("zoffset").value)
-                    file.print_byte(sprite.get_param("xextent").value)
-                    file.print_byte(sprite.get_param("yextent").value)
-                    file.print_byte(sprite.get_param("zextent").value)
-                if self.advanced:
-                    sprite.write_registers(file)
-                file.newline()
-
-    def process(self, spritelayout, feature, param_map, actions, var10map=None):
-        if not isinstance(param_map, list):
-            param_map = [param_map]
-
-        # Reduce all expressions, can't do that earlier as feature is not known
-        all_sprite_sets = []
-        layout_sprite_list = []  # Create a new structure
-        for layout_sprite in spritelayout.layout_sprite_list:
-            param_list = []
-            layout_sprite_list.append((layout_sprite.type, layout_sprite.pos, param_list))
-            for param in layout_sprite.param_list:
-                param_val = action2var.reduce_varaction2_expr(param.value, action2var.get_scope(feature), param_map)
-                if isinstance(param_val, expression.SpriteGroupRef):
-                    spriteset = action2.resolve_spritegroup(param_val.name)
-                    if not spriteset.is_spriteset():
-                        raise generic.ScriptError("Expected a reference to a spriteset.", param_val.pos)
-                    if feature == 0x04:
-                        assert var10map is not None
-                        param_val = var10map.translate(spriteset, param_val.param_list, param_val.pos)
-                    else:
-                        all_sprite_sets.append(spriteset)
-                param_list.append((param.name, param_val))
-
-        actions.extend(action1.add_to_action1(all_sprite_sets, feature, spritelayout.pos))
-
-        for type, pos, param_list in layout_sprite_list:
-            if type.value not in layout_sprite_types:
-                raise generic.ScriptError(
-                    "Invalid sprite type '{}' encountered. Expected 'ground', 'building', or 'childsprite'.".format(
-                        type.value
-                    ),
-                    type.pos,
-                )
-            sprite = Action2LayoutSprite(feature, layout_sprite_types[type.value], pos, param_map)
-            for name, value in param_list:
-                sprite.set_param(name, value)
-            self.registers.extend(sprite.get_all_registers())
-            if sprite.type == Action2LayoutSpriteType.GROUND:
-                if self.ground_sprite is not None:
-                    raise generic.ScriptError("Sprite layout can have no more than one ground sprite", spritelayout.pos)
-                self.ground_sprite = sprite
-            else:
-                self.building_sprites.append(sprite)
-
-        if self.ground_sprite is None:
-            if len(self.building_sprites) == 0:
-                # no sprites defined at all, that's not very much.
-                raise generic.ScriptError("Sprite layout requires at least one sprite", spritelayout.pos)
-            # set to 0 for no ground sprite
-            self.ground_sprite = Action2LayoutSprite(feature, Action2LayoutSpriteType.GROUND)
-            self.ground_sprite.set_param(expression.Identifier("sprite"), expression.ConstantNumeric(0))
-
-        self.advanced = any(x.is_advanced_sprite() for x in self.building_sprites + [self.ground_sprite])
-
-    def write_action_value(self, actions, act6, offset):
-        sprite_num = self.ground_sprite.get_sprite_number()
-        sprite_num, offset = actionD.write_action_value(sprite_num, actions, act6, offset, 4)
-        if self.advanced:
-            offset += self.ground_sprite.get_registers_size()
-
-        for sprite in self.building_sprites:
-            sprite_num = sprite.get_sprite_number()
-            sprite_num, offset = actionD.write_action_value(sprite_num, actions, act6, offset, 4)
-            if self.advanced:
-                offset += sprite.get_registers_size()
-            offset += 3 if sprite.type == Action2LayoutSpriteType.CHILD else 6
-
-        return offset
-
-    def parse_registers(self, varact2parser):
-        if self.registers:
-            for register_info in self.registers:
-                reg, expr = register_info[1], register_info[2]
-                if reg is None:
-                    continue
-                varact2parser.parse_expr(expr)
-                varact2parser.var_list.append(nmlop.STO_TMP)
-                varact2parser.var_list.append(reg)
-                varact2parser.var_list.append(nmlop.VAL2)
-                varact2parser.var_list_size += reg.get_size() + 2
-
-
-def get_layout_action2s(spritelayout, feature):
+def get_layout_action2s(spritegroup):
+    ground_sprite = None
+    building_sprites = []
     actions = []
 
+    feature = spritegroup.feature.value
     if feature not in action2.features_sprite_layout:
-        raise generic.ScriptError(
-            "Sprite layouts are not supported for feature '{}'.".format(general.feature_name(feature))
-        )
-
-    # Allocate registers
-    param_map = {}
-    param_registers = []
-    for param in spritelayout.param_list:
-        reg = action2var.VarAction2CallParam(param.value)
-        param_registers.append(reg)
-        param_map[param.value] = reg
-    param_map = (param_map, lambda name, value, pos: action2var.VarAction2LoadCallParam(value, name))
-    spritelayout.register_map[feature] = param_registers
+        raise generic.ScriptError("Sprite layouts are not supported for feature '%02X'." % feature)
 
-    layout = ParsedSpriteLayout()
-    layout.process(spritelayout, feature, param_map, actions)
+    all_spritesets = []
+    for layout_sprite in spritegroup.layout_sprite_list:
+        for param in layout_sprite.param_list:
+            if param.name.value in ('sprite', 'palette') and isinstance(param.value, expression.SpriteGroupRef):
+                all_spritesets.append(action2.resolve_spritegroup(param.value.name))
+    actions.extend(action1.add_to_action1(all_spritesets, feature, spritegroup.pos))
+
+    temp_registers = []
+    for layout_sprite in spritegroup.layout_sprite_list:
+        if layout_sprite.type.value not in layout_sprite_types:
+            raise generic.ScriptError("Invalid sprite type '%s' encountered. Expected 'ground', 'building', or 'childsprite'." % layout_sprite.type.value, layout_sprite.type.pos)
+        sprite = Action2LayoutSprite(layout_sprite_types[layout_sprite.type.value], layout_sprite.pos)
+        for param in layout_sprite.param_list:
+            sprite.set_param(param.name, param.value)
+        temp_registers.extend(sprite.get_all_registers())
+        if sprite.type == Action2LayoutSpriteType.GROUND:
+            if ground_sprite is not None:
+                raise generic.ScriptError("Sprite layout can have no more than one ground sprite", spritegroup.pos)
+            ground_sprite = sprite
+        else:
+            building_sprites.append(sprite)
+
+    if ground_sprite is None:
+        if len(building_sprites) == 0:
+            #no sprites defined at all, that's not very much.
+            raise generic.ScriptError("Sprite layout requires at least one sprite", spritegroup.pos)
+        #set to 0 for no ground sprite
+        ground_sprite = Action2LayoutSprite(Action2LayoutSpriteType.GROUND)
+        ground_sprite.set_param(expression.Identifier('sprite'), expression.ConstantNumeric(0))
 
     action6.free_parameters.save()
     act6 = action6.Action6()
 
-    layout.write_action_value(actions, act6, 4)
+    offset = 4
+    sprite_num = ground_sprite.get_sprite_number()
+    if not isinstance(sprite_num, expression.ConstantNumeric):
+        param, extra_actions = actionD.get_tmp_parameter(sprite_num)
+        actions.extend(extra_actions)
+        act6.modify_bytes(param, 4, offset)
+    offset += 4
+    offset += ground_sprite.get_registers_size()
+
+    for sprite in building_sprites:
+        sprite_num = sprite.get_sprite_number()
+        if not isinstance(sprite_num, expression.ConstantNumeric):
+            param, extra_actions = actionD.get_tmp_parameter(sprite_num)
+            actions.extend(extra_actions)
+            act6.modify_bytes(param, 4, offset)
+        offset += sprite.get_registers_size()
+        offset += 7 if sprite.type == Action2LayoutSpriteType.CHILD else 10
 
     if len(act6.modifications) > 0:
         actions.append(act6)
 
-    layout_action = Action2Layout(
-        feature,
-        spritelayout.name.value + " - feature {:02X}".format(feature),
-        spritelayout.pos,
-        layout,
-        param_registers,
-    )
+    layout_action = Action2Layout(feature, spritegroup.name.value, ground_sprite, building_sprites)
     actions.append(layout_action)
 
-    varact2parser = action2var.Varaction2Parser(feature)
-    layout.parse_registers(varact2parser)
+    if temp_registers:
+        varact2parser = action2var.Varaction2Parser(feature)
+        for register_info in temp_registers:
+            reg, expr = register_info[1], register_info[2]
+            if reg is None: continue
+            varact2parser.parse_expr(action2var.reduce_varaction2_expr(expr, feature))
+            varact2parser.var_list.append(nmlop.STO_TMP)
+            varact2parser.var_list.append(reg)
+            varact2parser.var_list.append(nmlop.VAL2)
+            varact2parser.var_list_size += reg.get_size() + 2
 
     # Only continue if we actually needed any new registers
-    if varact2parser.var_list:
-        # Remove the last VAL2 operator
+    if temp_registers and varact2parser.var_list:
+        #Remove the last VAL2 operator
         varact2parser.var_list.pop()
         varact2parser.var_list_size -= 1
 
         actions.extend(varact2parser.extra_actions)
         extra_act6 = action6.Action6()
         for mod in varact2parser.mods:
             extra_act6.modify_bytes(mod.param, mod.size, mod.offset + 4)
-        if len(extra_act6.modifications) > 0:
-            actions.append(extra_act6)
+        if len(extra_act6.modifications) > 0: actions.append(extra_act6)
 
-        varaction2 = action2var.Action2Var(
-            feature, "{}@registers - feature {:02X}".format(spritelayout.name.value, feature), spritelayout.pos, 0x89
-        )
+        varaction2 = action2var.Action2Var(feature, '%s@registers' % spritegroup.name.value, 0x89)
         varaction2.var_list = varact2parser.var_list
-        ref = expression.SpriteGroupRef(spritelayout.name, [], None, layout_action)
-        varaction2.ranges.append(
-            action2var.VarAction2Range(expression.ConstantNumeric(0), expression.ConstantNumeric(0), ref, "")
-        )
+        ref = expression.SpriteGroupRef(spritegroup.name, [], None, layout_action)
+        varaction2.ranges.append(switch_range.SwitchRange(expression.ConstantNumeric(0), expression.ConstantNumeric(0), ref, comment=''))
         varaction2.default_result = ref
-        varaction2.default_comment = ""
+        varaction2.default_comment = ''
 
-        # Add two references (default + range)
-        # Make sure that registers allocated here are not used by the spritelayout
-        action2.add_ref(ref, varaction2, True)
-        action2.add_ref(ref, varaction2, True)
-        spritelayout.set_action2(varaction2, feature)
+        action2.add_ref(ref, varaction2)
+        spritegroup.set_action2(varaction2)
         actions.append(varaction2)
     else:
-        spritelayout.set_action2(layout_action, feature)
+        spritegroup.set_action2(layout_action)
 
     action6.free_parameters.restore()
     return actions
-
-
-def make_empty_layout_action2(feature, pos):
-    """
-    Make an empty layout action2
-    For use with failed callbacks
-
-    @param feature: Feature of the sprite layout to create
-    @type feature: C{int}
-
-    @param pos: Positional context.
-    @type  pos: L{Position}
-
-    @return: The created sprite layout action2
-    @rtype: L{Action2Layout}
-    """
-    layout = ParsedSpriteLayout()
-    layout.ground_sprite = Action2LayoutSprite(feature, Action2LayoutSpriteType.GROUND)
-    layout.ground_sprite.set_param(expression.Identifier("sprite"), expression.ConstantNumeric(0))
-    return Action2Layout(feature, "@CB_FAILED_LAYOUT{:02X}".format(feature), pos, layout, [])
-
-
-class StationSpriteset(expression.Expression):
-    def __init__(self, spriteset, args, var10, pos=None):
-        expression.Expression.__init__(self, pos)
-        self.spriteset = spriteset
-        self.offset = args
-        self.var10 = var10
-
-
-class StationSpritesetVar10Map:
-    def __init__(self):
-        self.spritesets = {}
-        self.var10 = 1  # Reserving 0 for SPRITESET() (basic action2)
-
-    def translate(self, spriteset, args, pos):
-        if spriteset not in self.spritesets:
-            if self.var10 == 8:
-                raise generic.ScriptError("A station can't use more than 6 different sprite sets", pos)
-            self.spritesets[spriteset] = self.var10
-            self.var10 += 1 if self.var10 != 1 else 2  # Reserving 2 for custom foundations
-        return StationSpriteset(
-            None if isinstance(spriteset, int) else spriteset, args, self.spritesets[spriteset], pos
-        )
-
-    def append_mapping(self, mapping, feature, actions, default, custom_spritesets):
-        for spriteset, var10 in self.spritesets.items():
-            if not isinstance(spriteset, int):
-                if not spriteset.has_action2(feature):
-                    actions.extend(action1.add_to_action1([spriteset], feature, None))
-                    real_action2 = action2real.make_simple_real_action2(
-                        feature,
-                        spriteset.name.value + " - feature {:02X}".format(feature),
-                        None,
-                        action1.get_action1_index(spriteset),
-                    )
-                    actions.append(real_action2)
-                    spriteset.set_action2(real_action2, feature)
-                ref = expression.SpriteGroupRef(spriteset.name, [], None, spriteset.get_action2(feature))
-            else:
-                if spriteset > len(custom_spritesets):
-                    raise generic.ScriptError("Index out of range")
-                ref = custom_spritesets[spriteset]
-            # Skip default result
-            if ref == default:
-                continue
-            mapping[var10] = (ref, None)
-        return mapping
-
-
-def parse_station_layouts(feature, id, layouts):
-    var10map = StationSpritesetVar10Map()
-
-    # Add DEFAULT([offset]) to reference active spriteset, selected by basic action2
-    # and CUSTOM(index, [offset]) to reference a spriteset from the custom list
-    def parse_spriteset(name, args, pos, info):
-        if info:
-            if len(args) < 1:
-                raise generic.ScriptError("'{}' expects 1 or 2 parameters".format(name), pos)
-            if not isinstance(args[0], expression.ConstantNumeric):
-                raise generic.ScriptError("First parameter for '{}' must be a constant".format(name), pos)
-            return var10map.translate(args[0].value, args[1:], pos)
-        return StationSpriteset(None, args, info, pos)
-
-    default_param = [
-        (
-            {"DEFAULT": None, "CUSTOM": True},
-            lambda name, value, pos: expression.FunctionPtr(expression.Identifier(name, pos), parse_spriteset, value),
-        )
-    ]
-
-    actions = []
-    param_registers = []
-    parsed_layouts = []
-    varact2parser = action2var.Varaction2Parser(feature)
-
-    for layout in layouts:
-        spritelayout = (
-            action2.resolve_spritegroup(layout.name) if isinstance(layout, expression.SpriteGroupRef) else None
-        )
-        if not spritelayout or not isinstance(spritelayout, spriteblock.SpriteLayout):
-            raise generic.ScriptError("Expected a SpriteLayout", layout.pos)
-
-        # Allocate registers
-        registers = []
-        param_map = {}
-        for i, param in enumerate(spritelayout.param_list):
-            reg = action2var.VarAction2CallParam(param.value)
-            param_registers.append(reg)
-            param_map[param.value] = reg
-            store_tmp = action2var.VarAction2StoreCallParam(reg)
-            registers.append((reg, store_tmp, layout.param_list[i]))
-        param_map = [(param_map, lambda name, value, pos: action2var.VarAction2LoadCallParam(value, name))]
-        param_map.extend(default_param)
-
-        layout = ParsedSpriteLayout(registers)
-        layout.process(spritelayout, feature, param_map, actions, var10map)
-        layout.parse_registers(varact2parser)
-        parsed_layouts.append(layout)
-
-    actions.extend(action0.get_layout_action0(feature, id, parsed_layouts))
-
-    registers_ref = None
-
-    # Create a procedure only if needed
-    if varact2parser.var_list:
-        # Remove the last VAL2 operator
-        varact2parser.var_list.pop()
-        varact2parser.var_list_size -= 1
-
-        actions.extend(varact2parser.extra_actions)
-        extra_act6 = action6.Action6()
-        for mod in varact2parser.mods:
-            extra_act6.modify_bytes(mod.param, mod.size, mod.offset + 4)
-        if len(extra_act6.modifications) > 0:
-            actions.append(extra_act6)
-
-        varaction2 = action2var.Action2Var(
-            feature, "Station Layout@registers - Id {:02X}".format(id.value), None, 0x89, param_registers
-        )
-        varaction2.var_list = varact2parser.var_list
-        varaction2.default_result = expression.ConstantNumeric(0)
-        varaction2.default_comment = "Return computed value"
-
-        actions.append(varaction2)
-        registers_ref = expression.SpriteGroupRef(expression.Identifier(varaction2.name), [], None, varaction2)
-
-    return (actions, var10map, registers_ref)
```

### Comparing `nml-0.7.2/nml/actions/action4.py` & `nml-r1512/nml/actions/action4.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic, grfstrings
-from nml.actions import action6, actionD, base_action
-
+from nml import expression, grfstrings
+from nml.actions import base_action, action6, actionD
 
 class Action4(base_action.BaseAction):
     """
     Class representing a single action 4.
     Format: 04 <feature> <language-id> <num-ent> <offset> <text>
 
     @ivar feature: Feature of this action 4
@@ -31,28 +15,26 @@
     @ivar size: Size of the id, may be 1 (byte), 2 (word) or 3 (ext. byte)
     @type size: C{int}
 
     @ivar id: ID of the first string to write
     @type id: C{int}
 
     @ivar texts: List of strings to write
-    @type texts: C{list} of C{str}
+    @type texts: C{list} of C{unicode}
     """
-
     def __init__(self, feature, lang, size, id, texts):
         self.feature = feature
         self.lang = lang
         self.size = size
         self.id = id
         self.texts = texts
 
-    def prepare_output(self, sprite_num):
-        # To indicate a word value, bit 7 of the lang ID must be set
-        if self.size == 2:
-            self.lang = self.lang | 0x80
+    def prepare_output(self):
+        #To indicate a word value, bit 7 of the lang ID must be set
+        if self.size == 2: self.lang = self.lang | 0x80
 
     def write(self, file):
         size = 4 + self.size
         for text in self.texts:
             size += grfstrings.get_string_size(text)
         file.start_sprite(size)
         file.print_bytex(4)
@@ -64,102 +46,80 @@
             file.print_string(text)
         file.newline()
         file.end_sprite()
 
     def skip_action9(self):
         return False
 
-
 # List of various string ranges that may be used
 # Attributes:
-#  - random_id: If true, string IDs may be allocated randomly, else the ID has a special meaning and must be assigned
-#               (e.g. for vehicles, string ID = vehicle ID)
+#  - random_id: If true, string IDs may be allocated randomly, else the ID has a special meaning and must be assigned (e.g. for vehicles, string ID = vehicle ID)
 #  - ids: List of free IDs, only needed if random_id is true. Whenever an ID is used, it's removed from the list
 string_ranges = {
-    0xC4: {"random_id": False},  # Station class names
-    0xC5: {"random_id": False},  # Station names
-    0xC9: {"random_id": False},  # House name
-    # Misc. text ids, used for callbacks and such
-    0xD0: {"random_id": True, "total": 0x400, "ids": list(range(0xD3FF, 0xCFFF, -1))},
-    # Misc. persistent text ids, used to set properties.
-    # Use Ids DC00..DCFF first to keep compatibility with older versions of OTTD.
-    0xDC: {"random_id": True, "total": 0x800, "ids": list(range(0xDBFF, 0xD7FF, -1)) + list(range(0xDFFF, 0xDBFF, -1))},
+    0xC4: {'random_id': False}, # Station class names
+    0xC5: {'random_id': False}, # Station names
+    0xC9: {'random_id': False}, # House name
+    0xD0: {'random_id': True, 'ids': list(range(0x3FF, -1, -1))}, # Misc. text ids, used for callbacks and such
+    0xDC: {'random_id': True, 'ids': list(range(0xFF, -1, -1))}, # Misc. persistent text ids, used to set properties
 }
 
 # Mapping of string identifiers to D0xx/DCxx text ids
 # This allows outputting strings only once, instead of everywhere they are used
 used_strings = {
     0xD0: {},
     0xDC: {},
 }
 
-
-def print_stats():
-    """
-    Print statistics about used ids.
-    """
-    for t, l in string_ranges.items():
-        if l["random_id"]:
-            num_used = l["total"] - len(l["ids"])
-            if num_used > 0:
-                generic.print_info("{:02X}xx strings: {}/{}".format(t, num_used, l["total"]))
-
-
 def get_global_string_actions():
     """
     Get a list of global string actions
     i.e. print all D0xx / DCxx texts at once
 
     @return: A list of all D0xx / DCxx action4s
     @rtype: C{list} of L{BaseAction}
     """
     texts = []
     actions = []
-    for strings in used_strings.values():
-        for feature_name, id in strings.items():
-            feature, string_name = feature_name
-            texts.append((0x7F, id, grfstrings.get_translation(string_name), feature))
+    for string_range, strings in used_strings.iteritems():
+        for string_name, id in strings.iteritems():
+            texts.append( (0x7F, (string_range << 8) | id, grfstrings.get_translation(string_name)) )
             for lang_id in grfstrings.get_translations(string_name):
-                texts.append((lang_id, id, grfstrings.get_translation(string_name, lang_id), feature))
+                texts.append( (lang_id, (string_range << 8) | id, grfstrings.get_translation(string_name, lang_id)) )
 
     last_lang = -1
     last_id = -1
-    last_feature = -1
     # Sort to have a deterministic ordering and to have as much consecutive IDs as possible
     texts.sort(key=lambda text: (-1 if text[0] == 0x7F else text[0], text[1]))
 
     for text in texts:
-        str_lang, str_id, str_text, feature = text
+        str_lang, str_id, str_text = text
         # If possible, append strings to the last action 4 instead of creating a new one
-        if str_lang != last_lang or str_id - 1 != last_id or feature != last_feature or len(actions[-1].texts) == 0xFF:
-            actions.append(Action4(feature, str_lang, 2, str_id, [str_text]))
+        if str_lang != last_lang or str_id - 1 != last_id:
+            actions.append(Action4(0x08, str_lang, 2, str_id, [str_text]))
         else:
             actions[-1].texts.append(str_text)
         last_lang = str_lang
         last_id = str_id
-        last_feature = feature
     return actions
 
-
-def get_string_action4s(feature, string_range, string, id=None):
+def get_string_action4s(feature, string_range, string, id = None):
     """
     Let a string from the lang files be used in the rest of NML.
     This may involve adding actions directly, but otherwise an ID is allocated and the string will be written later
 
     @param feature: Feature that uses the string
     @type feature: C{int}
 
     @param string_range: String range to use, either a value from L{string_ranges} or C{None} if N/A (item names)
     @type string_range: C{int} or C{None}
 
     @param string: String to parse
     @type string: L{expression.String}
 
-    @param id: ID to use for this string, or C{None} if it will be allocated dynamically
-               (random_id is true for the string range)
+    @param id: ID to use for this string, or C{None} if it will be allocated dynamically (random_id is true for the string range)
     @type id: L{Expression} or C{None}
 
     @return: A tuple of two values:
                 - ID of the string (useful if allocated dynamically)
                 - Resulting action list to be appended
     @rtype: C{tuple} of (C{int}, C{list} of L{BaseAction})
     """
@@ -167,52 +127,43 @@
     write_action4s = True
     action6.free_parameters.save()
     actions = []
 
     mod = None
     if string_range is not None:
         size = 2
-        if string_ranges[string_range]["random_id"]:
+        if string_ranges[string_range]['random_id']:
             # ID is allocated randomly, we will output the actions later
             write_action4s = False
-            if (feature, string) in used_strings[string_range]:
-                id_val = used_strings[string_range][(feature, string)]
+            if string in used_strings[string_range]:
+                id_val = used_strings[string_range][string]
             else:
-                try:
-                    id_val = string_ranges[string_range]["ids"].pop()
-                    used_strings[string_range][(feature, string)] = id_val
-                except IndexError:
-                    raise generic.ScriptError(
-                        "Unable to allocate ID for string, no more free IDs available (maximum is {:d})".format(
-                            string_ranges[string_range]["total"]
-                        ),
-                        string.pos,
-                    )
+                id_val = string_ranges[string_range]['ids'].pop()
+                used_strings[string_range][string] = id_val
         else:
             # ID must be supplied
             assert id is not None
             assert isinstance(id, expression.ConstantNumeric)
-            id_val = id.value | (string_range << 8)
+            id_val = id.value
+        id_val = id_val | (string_range << 8)
     else:
-        # Not a string range, so we must have an id
+        # Not a string range, so we must have an idea
         assert id is not None
         size = 3 if feature <= 3 else 1
         if isinstance(id, expression.ConstantNumeric):
             id_val = id.value
         else:
             id_val = 0
             tmp_param, tmp_param_actions = actionD.get_tmp_parameter(id)
             actions.extend(tmp_param_actions)
             # Apply ID via action4 later
             mod = (tmp_param, 2 if feature <= 3 else 1, 5 if feature <= 3 else 4)
 
     if write_action4s:
-        strings = [
-            (lang_id, grfstrings.get_translation(string, lang_id)) for lang_id in grfstrings.get_translations(string)
-        ]
+        strings = [(lang_id, grfstrings.get_translation(string, lang_id)) for lang_id in grfstrings.get_translations(string)]
         # Sort the strings for deterministic ordering and prepend the default language
         strings = [(0x7F, grfstrings.get_translation(string))] + sorted(strings, key=lambda lang_text: lang_text[0])
 
         for lang_id, text in strings:
             if mod is not None:
                 act6 = action6.Action6()
                 act6.modify_bytes(*mod)
```

### Comparing `nml-0.7.2/nml/actions/action7.py` & `nml-r1512/nml/actions/action7.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,116 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, free_number_list, generic, nmlop
-from nml.actions import action6, action10, actionD, base_action
-
-free_labels = free_number_list.FreeNumberList(
-    list(range(0xFF, 0x0F, -1)),
-    "No label available to use for large if-blocks and loops.",
-    "No unique label available to use for large if-blocks and loops.",
-)
-
-
-def print_stats():
-    """
-    Print statistics about used ids.
-    """
-    if free_labels.stats[0] > 0:
-        generic.print_info(
-            "Concurrent Action10 labels: {}/{} ({})".format(
-                free_labels.stats[0], free_labels.total_amount, str(free_labels.stats[1])
-            )
-        )
+from nml import expression, nmlop, free_number_list
+from nml.actions import base_action, action6, actionD, action10
 
+free_labels = free_number_list.FreeNumberList(list(range(0xFF, 0x0F, -1)))
 
 class SkipAction(base_action.BaseAction):
     def __init__(self, action_type, var, varsize, condtype, value, label):
         self.action_type = action_type
         self.label = label
         self.var = var
         self.varsize = varsize
         self.condtype = condtype
         self.value = value
         self.label = label
-        if self.condtype[0] == 0 or self.condtype[0] == 1:
-            assert self.varsize == 1
 
     def write(self, file):
         size = 5 + self.varsize
         file.start_sprite(size)
         file.print_bytex(self.action_type)
         file.print_bytex(self.var)
         file.print_bytex(self.varsize)
         file.print_bytex(self.condtype[0], self.condtype[1])
         if self.varsize == 8:
-            # grfid + mask
+            #grfid + mask
             file.print_dwordx(self.value & 0xFFFFFFFF)
             file.print_dwordx(self.value >> 32)
         else:
             file.print_varx(self.value, self.varsize)
         file.print_bytex(self.label)
         file.newline()
         file.end_sprite()
 
     def skip_action7(self):
         return self.action_type == 7
 
     def skip_action9(self):
         return self.action_type == 9 or self.label == 0
 
-
 class UnconditionalSkipAction(SkipAction):
     def __init__(self, action_type, label):
-        SkipAction.__init__(self, action_type, 0x9A, 1, (0, r"\71"), 0, label)
-
+        SkipAction.__init__(self, action_type, 0x9A, 1, (0, r'\71'), 0, label)
 
 def op_to_cond_op(op):
-    # The operators are reversed as we want to skip if the expression is true
-    # while the nml-syntax wants to execute the block if the expression is true
-    if op == nmlop.CMP_NEQ:
-        return (2, r"\7=")
-    if op == nmlop.CMP_EQ:
-        return (3, r"\7!")
-    if op == nmlop.CMP_GE:
-        return (4, r"\7<")
-    if op == nmlop.CMP_LE:
-        return (5, r"\7>")
-    # Not reached
-    raise ValueError("Unexpected operator '{}'".format(op.token))
-
+    #The operators are reversed as we want to skip if the expression is true
+    #while the nml-syntax wants to execute the block if the expression is true
+    if op == nmlop.CMP_NEQ: return (2, r'\7=')
+    if op == nmlop.CMP_EQ: return (3, r'\7!')
+    if op == nmlop.CMP_GE: return (4, r'\7<')
+    if op == nmlop.CMP_LE: return (5, r'\7>')
 
 def parse_conditional(expr):
-    """
+    '''
     Parse an expression and return enough information to use
     that expression as a conditional statement.
     Return value is a tuple with the following elements:
     - Parameter number (as integer) to use in comparison or None for unconditional skip
     - List of actions needed to set the given parameter to the correct value
     - The type of comparison to be done
     - The value to compare against (as integer)
     - The size of the value (as integer)
-    """
+    '''
     if expr is None:
-        return (None, [], (2, r"\7="), 0, 4)
+        return (None, [], (2, r'\7='), 0, 4)
     if isinstance(expr, expression.BinOp):
         if expr.op == nmlop.HASBIT or expr.op == nmlop.NOTHASBIT:
             if isinstance(expr.expr1, expression.Parameter) and isinstance(expr.expr1.num, expression.ConstantNumeric):
                 param = expr.expr1.num.value
                 actions = []
             else:
                 param, actions = actionD.get_tmp_parameter(expr.expr1)
             if isinstance(expr.expr2, expression.ConstantNumeric):
                 bit_num = expr.expr2.value
             else:
-                if isinstance(expr.expr2, expression.Parameter) and isinstance(
-                    expr.expr2.num, expression.ConstantNumeric
-                ):
+                if isinstance(expr.expr2, expression.Parameter) and isinstance(expr.expr2.num, expression.ConstantNumeric):
                     param = expr.expr2.num.value
                 else:
                     param, tmp_action_list = actionD.get_tmp_parameter(expr.expr2)
                     actions.extend(tmp_action_list)
                 act6 = action6.Action6()
                 act6.modify_bytes(param, 1, 4)
                 actions.append(act6)
                 bit_num = 0
-            comp_type = (1, r"\70") if expr.op == nmlop.HASBIT else (0, r"\71")
-            return (param, actions, comp_type, bit_num, 1)
-        elif expr.op in (nmlop.CMP_EQ, nmlop.CMP_NEQ, nmlop.CMP_LE, nmlop.CMP_GE) and isinstance(
-            expr.expr2, expression.ConstantNumeric
-        ):
+            comp_type = (1, r'\70') if expr.op == nmlop.HASBIT else (0, r'\71')
+            return (param, actions, comp_type, bit_num , 1)
+        elif expr.op in (nmlop.CMP_EQ, nmlop.CMP_NEQ, nmlop.CMP_LE, nmlop.CMP_GE) \
+                and isinstance(expr.expr2, expression.ConstantNumeric):
             if isinstance(expr.expr1, expression.Parameter) and isinstance(expr.expr1.num, expression.ConstantNumeric):
                 param = expr.expr1.num.value
                 actions = []
             else:
                 param, actions = actionD.get_tmp_parameter(expr.expr1)
             op = op_to_cond_op(expr.op)
             return (param, actions, op, expr.expr2.value, 4)
-
-    if isinstance(expr, expression.Boolean):
-        expr = expr.expr
-
     if isinstance(expr, expression.Not):
         param, actions = actionD.get_tmp_parameter(expr.expr)
-        return (param, actions, (3, r"\7!"), 0, 4)
+        return (param, actions, (3, r'\7!'), 0, 4)
 
     param, actions = actionD.get_tmp_parameter(expr)
-    return (param, actions, (2, r"\7="), 0, 4)
-
+    return (param, actions, (2, r'\7='), 0, 4)
 
-def cond_skip_actions(action_list, param, condtype, value, value_size, pos):
-    if len(action_list) == 0:
-        return []
+def cond_skip_actions(action_list, param, condtype, value, value_size):
+    if len(action_list) == 0: return []
+    if len(free_labels.states) == 0:
+        # We only save a single state (at toplevel nml-blocks) because
+        # we don't know at the start of the block how many labels we need.
+        # Getting the same label for a block that was already used in a
+        # sub-block would be very bad, since the action7/9 would skip
+        # to the action10 of the sub-block.
+        free_labels.save()
     actions = []
     start, length = 0, 0
     # Whether to allow not-skipping, using action7 or using action9
     skip_opts = (True, True, True)
     # Add a sentinel value to the list to avoid code duplication
     for action in action_list + [None]:
         assert any(skip_opts)
@@ -175,166 +130,107 @@
             length += 1
             skip_opts = new_opts
             continue
 
         # We need to create a new block
         if skip_opts[0]:
             # We can just choose to not skip the preceeding actions without harm
-            actions.extend(action_list[start : start + length])
+            actions.extend(action_list[start:start+length])
         else:
             action_type = 7 if skip_opts[1] else 9
             if length < 0x10:
                 # Lengths under 0x10 are handled without labels, to avoid excessive label usage
                 target = length
                 label = None
             else:
-                target = free_labels.pop(pos)
+                target = free_labels.pop()
                 label = action10.Action10(target)
             actions.append(SkipAction(action_type, param, value_size, condtype, value, target))
-            actions.extend(action_list[start : start + length])
-            if label is not None:
-                actions.append(label)
+            actions.extend(action_list[start:start+length])
+            if label is not None: actions.append(label)
 
         start = start + length
         length = 1
         skip_opts = act_opts
     assert start == len(action_list)
 
+    if len(free_labels.states) == 1:
+        free_labels.restore()
     return actions
 
-
-recursive_cond_blocks = 0
-
-
 def parse_conditional_block(cond_list):
-    global recursive_cond_blocks
-    recursive_cond_blocks += 1
-    if recursive_cond_blocks == 1:
-        # We only save a single state (at toplevel nml-blocks) because
-        # we don't know at the start of the block how many labels we need.
-        # Getting the same label for a block that was already used in a
-        # sub-block would be very bad, since the action7/9 would skip
-        # to the action10 of the sub-block.
-        free_labels.save()
-
     blocks = []
     for cond in cond_list.statements:
         if isinstance(cond.expr, expression.ConstantNumeric):
             if cond.expr.value == 0:
                 continue
             else:
-                blocks.append({"expr": None, "statements": cond.statements})
+                blocks.append({'expr': None, 'statements': cond.statements})
                 break
-        blocks.append({"expr": cond.expr, "statements": cond.statements})
+        blocks.append({'expr': cond.expr, 'statements': cond.statements})
     if blocks:
-        blocks[-1]["last_block"] = True
+        blocks[-1]['last_block'] = True
 
-    if len(blocks) == 1 and blocks[0]["expr"] is None:
+    if len(blocks) == 1 and blocks[0]['expr'] is None:
         action_list = []
-        for stmt in blocks[0]["statements"]:
+        for stmt in blocks[0]['statements']:
             action_list.extend(stmt.get_action_list())
         return action_list
 
     action6.free_parameters.save()
-
+    
     if len(blocks) > 1:
         # the skip all parameter is used to skip all blocks after one
         # of the conditionals was true. We can't always skip directly
         # to the end of the blocks since action7/action9 can't always
         # be mixed
         param_skip_all, action_list = actionD.get_tmp_parameter(expression.ConstantNumeric(0xFFFFFFFF))
     else:
         action_list = []
 
     # use parse_conditional here, we also need to know if all generated
     # actions (like action6) can be skipped safely
     for block in blocks:
-        (
-            block["param_dst"],
-            block["cond_actions"],
-            block["cond_type"],
-            block["cond_value"],
-            block["cond_value_size"],
-        ) = parse_conditional(block["expr"])
-        if "last_block" not in block:
-            block["action_list"] = [
-                actionD.ActionD(
-                    # If this isn't the last block, len(blocks) > 1 so param_skip_all is initialized.
-                    expression.ConstantNumeric(param_skip_all),  # lgtm [py/uninitialized-local-variable]
-                    expression.ConstantNumeric(0xFF),
-                    nmlop.ASSIGN,
-                    expression.ConstantNumeric(0),
-                    expression.ConstantNumeric(0),
-                )
-            ]
+        block['param_dst'], block['cond_actions'], block['cond_type'], block['cond_value'], block['cond_value_size'] = parse_conditional(block['expr'])
+        if not 'last_block' in block:
+            block['action_list'] = [actionD.ActionD(expression.ConstantNumeric(param_skip_all), expression.ConstantNumeric(0xFF), nmlop.ASSIGN, expression.ConstantNumeric(0), expression.ConstantNumeric(0))]
         else:
-            block["action_list"] = []
-        for stmt in block["statements"]:
-            block["action_list"].extend(stmt.get_action_list())
+            block['action_list'] = []
+        for stmt in block['statements']:
+            block['action_list'].extend(stmt.get_action_list())
 
     # Main problem: action10 can't be skipped by action9, so we're
     # nearly forced to use action7, but action7 can't safely skip action6
     # Solution: use temporary parameter, set to 0 for not skip, !=0 for skip.
     # then skip every block of actions (as large as possible) with either
     # action7 or action9, depending on which of the two works.
 
     for i, block in enumerate(blocks):
-        param = block["param_dst"]
-        if i == 0:
-            action_list.extend(block["cond_actions"])
+        param = block['param_dst']
+        if i == 0: action_list.extend(block['cond_actions'])
         else:
-            action_list.extend(
-                cond_skip_actions(block["cond_actions"], param_skip_all, (2, r"\7="), 0, 4, cond_list.pos)
-            )
+            action_list.extend(cond_skip_actions(block['cond_actions'], param_skip_all, (2, r'\7='), 0, 4))
             if param is None:
                 param = param_skip_all
             else:
-                action_list.append(
-                    actionD.ActionD(
-                        expression.ConstantNumeric(block["param_dst"]),
-                        expression.ConstantNumeric(block["param_dst"]),
-                        nmlop.AND,
-                        expression.ConstantNumeric(param_skip_all),
-                    )
-                )
-        action_list.extend(
-            cond_skip_actions(
-                block["action_list"],
-                param,
-                block["cond_type"],
-                block["cond_value"],
-                block["cond_value_size"],
-                cond_list.pos,
-            )
-        )
+                action_list.append(actionD.ActionD(expression.ConstantNumeric(block['param_dst']), expression.ConstantNumeric(block['param_dst']), nmlop.AND, expression.ConstantNumeric(param_skip_all)))
+        action_list.extend(cond_skip_actions(block['action_list'], param, block['cond_type'], block['cond_value'], block['cond_value_size']))
 
-    if recursive_cond_blocks == 1:
-        free_labels.restore()
-    recursive_cond_blocks -= 1
     action6.free_parameters.restore()
     return action_list
 
-
 def parse_loop_block(loop):
-    global recursive_cond_blocks
-    recursive_cond_blocks += 1
-    if recursive_cond_blocks == 1:
-        free_labels.save()
-
     action6.free_parameters.save()
-    begin_label = free_labels.pop_unique(loop.pos)
+    begin_label = free_labels.pop_unique()
     action_list = [action10.Action10(begin_label)]
 
     cond_param, cond_actions, cond_type, cond_value, cond_value_size = parse_conditional(loop.expr)
     block_actions = []
     for stmt in loop.statements:
         block_actions.extend(stmt.get_action_list())
 
     action_list.extend(cond_actions)
     block_actions.append(UnconditionalSkipAction(9, begin_label))
-    action_list.extend(cond_skip_actions(block_actions, cond_param, cond_type, cond_value, cond_value_size, loop.pos))
+    action_list.extend(cond_skip_actions(block_actions, cond_param, cond_type, cond_value, cond_value_size))
 
-    if recursive_cond_blocks == 1:
-        free_labels.restore()
-    recursive_cond_blocks -= 1
     action6.free_parameters.restore()
     return action_list
```

### Comparing `nml-0.7.2/nml/actions/actionA.py` & `nml-r1512/nml/actions/action2production.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,74 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
+from nml.actions import action2, action6, actionD
+from nml import expression
 
-from nml import nmlop
-from nml.actions import action6, actionD, base_action, real_sprite
+class Action2Production(action2.Action2):
+    """
+    Class corresponding to Action2Industries (=production CB)
 
+    @ivar version: Production CB version. Version 0 uses constants, version 1 uses registers.
+    @type version: C{int}
 
-class ActionA(base_action.BaseAction):
-    """
-    Action class for Action A (sprite replacement)
+    @ivar sub_in: Amounts (v0) or registers (v1) to subtract from incoming cargos.
+    @type sub_in: C{list} of C{int}
 
-    @ivar sets: List of sprite collections to be replaced.
-    @type sets: C{list} of (C{int}, C{int})-tuples
+    @ivar add_out: Amounts (v0) or registers (v1) to add to the output cargos.
+    @type add_out: C{list} of C{int}
+
+    @ivar again: Number (v0) or register (v1), production CB will be run again if nonzero.
+    @type again C{int}
     """
+    def __init__(self, name, version, sub_in, add_out, again):
+        action2.Action2.__init__(self, 0x0A, name)
+        self.version = version
+        assert version == 0 or version == 1
+        self.sub_in = sub_in
+        assert len(self.sub_in) == 3
+        self.add_out = add_out
+        assert len(self.add_out) == 2
+        self.again = again
 
-    def __init__(self, sets):
-        self.sets = sets
+    def prepare_output(self):
+        action2.Action2.prepare_output(self)
 
     def write(self, file):
-        # <Sprite-number> * <Length> 0A <num-sets> [<num-sprites> <first-sprite>]+
-        size = 2 + 3 * len(self.sets)
-        file.start_sprite(size)
-        file.print_bytex(0x0A)
-        file.print_byte(len(self.sets))
-        for num, first in self.sets:
-            file.print_byte(num)
-            file.print_word(first)
+        cargo_size = 2 if self.version == 0 else 1
+        size = 2 + 5 * cargo_size
+        action2.Action2.write_sprite_start(self, file, size)
+        file.print_bytex(self.version)
+        for c in self.sub_in + self.add_out:
+            file.print_varx(c, cargo_size)
+        file.print_bytex(self.again)
         file.newline()
         file.end_sprite()
 
-
-def parse_actionA(replaces):
+def get_production_actions(produce):
     """
-    Parse replace-block to ActionA.
+    Get the action list that implements the given produce-block in nfo.
 
-    @param replaces: Replace-block to parse.
-    @type  replaces: L{ReplaceSprite}
+    @param produce: Produce-block to parse.
+    @type produce: L{Produce}
     """
     action_list = []
-    action6.free_parameters.save()
     act6 = action6.Action6()
+    action6.free_parameters.save()
 
-    real_sprite_list = real_sprite.parse_sprite_data(replaces)
-    block_list = []
-    total_sprites = len(real_sprite_list)
-    offset = 2  # Skip 0A and <num-sets>
-    sprite_offset = 0  # Number of sprites already covered by previous [<num-sprites> <first-sprite>]-pairs
-
-    while total_sprites > 0:
-        this_block = min(total_sprites, 255)  # number of sprites in this block
-        total_sprites -= this_block
-        offset += 1  # Skip <num-sprites>
-
-        first_sprite = replaces.start_id  # number of first sprite
-        if sprite_offset != 0:
-            first_sprite = nmlop.ADD(first_sprite, sprite_offset).reduce()
-        first_sprite, offset = actionD.write_action_value(first_sprite, action_list, act6, offset, 2)
-        block_list.append((this_block, first_sprite.value))
-
-        sprite_offset += this_block  # increase first-sprite for next block
+    result_list = []
+    for i, param in enumerate(produce.param_list):
+        if isinstance(param, expression.ConstantNumeric):
+            result_list.append(param.value)
+        else:
+            if isinstance(param, expression.Parameter) and isinstance(param.num, expression.ConstantNumeric):
+                param_num = param.num.value
+            else:
+                param_num, tmp_param_actions = actionD.get_tmp_parameter(param)
+                action_list.extend(tmp_param_actions)
+            act6.modify_bytes(param_num, 2 if i < 5 else 1, 1 + 2 * i)
+            result_list.append(0)
 
-    if len(act6.modifications) > 0:
-        action_list.append(act6)
+    if len(act6.modifications) > 0: action_list.append(act6)
     action6.free_parameters.restore()
-
-    action_list.append(ActionA(block_list))
-    action_list.extend(real_sprite_list)
+    prod_action = Action2Production(produce.name.value, produce.version, result_list[0:3], result_list[3:5], result_list[5])
+    action_list.append(prod_action)
+    produce.set_action2(prod_action)
 
     return action_list
```

### Comparing `nml-0.7.2/nml/actions/actionB.py` & `nml-r1512/nml/actions/actionB.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import expression, generic, grfstrings
-from nml.actions import action6, actionD, base_action
-
+from nml.actions import base_action, action6, actionD
 
 class ActionB(base_action.BaseAction):
     def __init__(self, severity, lang, msg, data, extra_params):
         self.severity = severity
         self.lang = lang
         self.msg = msg
         self.data = data
         self.extra_params = extra_params
 
     def write(self, file):
         size = 4
-        if not isinstance(self.msg, int):
-            size += grfstrings.get_string_size(self.msg)
+        if not isinstance(self.msg, int): size += grfstrings.get_string_size(self.msg)
         if self.data is not None:
             size += grfstrings.get_string_size(self.data) + len(self.extra_params)
 
         file.start_sprite(size)
         file.print_bytex(0x0B)
         self.severity.write(file, 1)
         file.print_bytex(self.lang)
@@ -47,63 +30,66 @@
                 param.write(file, 1)
         file.newline()
         file.end_sprite()
 
     def skip_action7(self):
         return False
 
-
 default_error_msg = {
-    "REQUIRES_TTDPATCH": 0,
-    "REQUIRES_DOS_WINDOWS": 1,
-    "USED_WITH": 2,
-    "INVALID_PARAMETER": 3,
-    "MUST_LOAD_BEFORE": 4,
-    "MUST_LOAD_AFTER": 5,
-    "REQUIRES_OPENTTD": 6,
+    'REQUIRES_TTDPATCH' : 0,
+    'REQUIRES_DOS_WINDOWS' : 1,
+    'USED_WITH' : 2,
+    'INVALID_PARAMETER' : 3,
+    'MUST_LOAD_BEFORE' : 4,
+    'MUST_LOAD_AFTER' : 5,
+    'REQUIRES_OPENTTD' : 6,
 }
 
 error_severity = {
-    "NOTICE": 0,
-    "WARNING": 1,
-    "ERROR": 2,
-    "FATAL": 3,
+    'NOTICE'  : 0,
+    'WARNING' : 1,
+    'ERROR'   : 2,
+    'FATAL'   : 3,
 }
 
-
 def parse_error_block(error):
     action6.free_parameters.save()
     action_list = []
     act6 = action6.Action6()
 
-    severity = actionD.write_action_value(error.severity, action_list, act6, 1, 1)[0]
+    if isinstance(error.severity, expression.ConstantNumeric):
+        severity = error.severity
+    elif isinstance(error.severity, expression.Parameter) and isinstance(error.severity.num, expression.ConstantNumeric):
+        act6.modify_bytes(error.severity.num.value, 1, 1)
+        severity = expression.ConstantNumeric(0)
+    else:
+        tmp_param, tmp_param_actions = actionD.get_tmp_parameter(error.severity)
+        action_list.extend(tmp_param_actions)
+        act6.modify_bytes(tmp_param, 1, 1)
+        severity = expression.ConstantNumeric(0)
 
     langs = [0x7F]
     if isinstance(error.msg, expression.String):
         custom_msg = True
         msg_string = error.msg
         grfstrings.validate_string(msg_string)
         langs.extend(grfstrings.get_translations(msg_string))
-        for lang in langs:
-            assert lang is not None
+        for l in langs: assert l is not None
     else:
         custom_msg = False
         msg = error.msg.reduce_constant().value
 
     if error.data is not None:
         error.data = error.data.reduce()
         if isinstance(error.data, expression.String):
             grfstrings.validate_string(error.data)
             langs.extend(grfstrings.get_translations(error.data))
-            for lang in langs:
-                assert lang is not None
+            for l in langs: assert l is not None
         elif not isinstance(error.data, expression.StringLiteral):
-            raise generic.ScriptError(
-                "Error parameter 3 'data' should be the identifier of a custom sting", error.data.pos
-            )
+            raise generic.ScriptError("Error parameter 3 'data' should be the identifier of a custom sting", error.data.pos)
 
     params = []
     for expr in error.params:
         if isinstance(expr, expression.Parameter) and isinstance(expr.num, expression.ConstantNumeric):
             params.append(expr.num)
         else:
             tmp_param, tmp_param_actions = actionD.get_tmp_parameter(expr)
@@ -117,13 +103,12 @@
             msg = grfstrings.get_translation(msg_string, lang)
         if error.data is None:
             data = None
         elif isinstance(error.data, expression.StringLiteral):
             data = error.data.value
         else:
             data = grfstrings.get_translation(error.data, lang)
-        if len(act6.modifications) > 0:
-            action_list.append(act6)
+        if len(act6.modifications) > 0: action_list.append(act6)
         action_list.append(ActionB(severity, lang, msg, data, params))
 
     action6.free_parameters.restore()
     return action_list
```

### Comparing `nml-0.7.2/nml/actions/actionD.py` & `nml-r1512/nml/actions/actionD.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic, global_constants, nmlop
-from nml.actions import action6, action7, base_action
-from nml.ast import base_statement, conditional
-
+from nml import generic, global_constants, expression, nmlop
+from nml.actions import base_action, action6
+from nml.ast import base_statement
+import nml
 
 class ActionD(base_action.BaseAction):
     """
     ActionD class
     General procedure: target = param1 op param2
     If one of the params is 0xFF, the value of 'data' is read instead.
 
@@ -36,196 +21,123 @@
     @ivar param2: Paramter number of the second operand
     @type param2: L{ConstantNumeric}
 
     @ivar data: Numerical data that will be used instead of parameter value,
                     if the parameter number is 0xFF. None if n/a.
     @type data: L{ConstantNumeric} or C{None}
     """
-
-    def __init__(self, target, param1, op, param2, data=None):
+    def __init__(self, target, param1, op, param2, data = None):
         self.target = target
         self.param1 = param1
         self.op = op
         self.param2 = param2
         self.data = data
 
     def write(self, file):
         size = 5
-        if self.data is not None:
-            size += 4
+        if self.data is not None: size += 4
 
-        # print the statement for easier debugging
-        str1 = "param[{}]".format(self.param1) if self.param1.value != 0xFF else str(self.data)
-        str2 = "param[{}]".format(self.param2) if self.param2.value != 0xFF else str(self.data)
+        #print the statement for easier debugging
+        str1 = "param[%s]" % self.param1 if self.param1.value != 0xFF else str(self.data)
+        str2 = "param[%s]" % self.param2 if self.param2.value != 0xFF else str(self.data)
         str_total = self.op.to_string(str1, str2) if self.op != nmlop.ASSIGN else str1
-        file.comment("param[{}] = {}".format(self.target, str_total))
+        file.comment("param[%s] = %s" % (self.target, str_total))
 
         file.start_sprite(size)
         file.print_bytex(0x0D)
         self.target.write(file, 1)
         file.print_bytex(self.op.actd_num, self.op.actd_str)
         self.param1.write(file, 1)
         self.param2.write(file, 1)
-        if self.data is not None:
-            self.data.write(file, 4)
+        if self.data is not None: self.data.write(file, 4)
         file.newline()
         file.end_sprite()
 
     def skip_action7(self):
         return False
 
-
 class ParameterAssignment(base_statement.BaseStatement):
     """
     AST-node for a parameter assignment.
     NML equivalent: param[$num] = $expr;
 
     @ivar param: Target expression to assign (must evaluate to a parameter)
     @type param: L{Expression}
 
     @ivar value: Value to assign to this parameter
     @type value: L{Expression}
     """
-
     def __init__(self, param, value):
         base_statement.BaseStatement.__init__(self, "parameter assignment", param.pos)
         self.param = param
         self.value = value
 
     def pre_process(self):
         self.value = self.value.reduce(global_constants.const_list)
 
-        self.param = self.param.reduce(global_constants.const_list, unknown_id_fatal=False)
+        self.param = self.param.reduce(global_constants.const_list, unknown_id_fatal = False)
         if isinstance(self.param, expression.SpecialParameter):
             if not self.param.can_assign():
-                raise generic.ScriptError(
-                    "Trying to assign a value to the read-only variable '{}'".format(self.param.name), self.param.pos
-                )
+                raise generic.ScriptError("Trying to assign a value to the read-only variable '%s'" % self.param.name, self.param.pos)
         elif isinstance(self.param, expression.Identifier):
-            if global_constants.identifier_refcount[self.param.value] == 0:
-                generic.print_warning(
-                    generic.Warning.OPTIMISATION,
-                    "Named parameter '{}' is not referenced, ignoring.".format(self.param.value),
-                    self.param.pos,
-                )
-                return
-            num = action6.free_parameters.pop_unique(self.pos)
+            num = action6.free_parameters.pop_unique()
             global_constants.named_parameters[self.param.value] = num
         elif not isinstance(self.param, expression.Parameter):
             raise generic.ScriptError("Left side of an assignment must be a parameter.", self.param.pos)
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Parameter assignment")
+        print indentation*' ' + 'Parameter assignment'
         self.param.debug_print(indentation + 2)
         self.value.debug_print(indentation + 2)
 
     def get_action_list(self):
         return parse_actionD(self)
 
     def __str__(self):
-        return "{} = {};\n".format(self.param, self.value)
-
+        return '%s = %s;\n' % (str(self.param), str(self.value))
 
-# prevent evaluating common sub-expressions multiple times
+#prevent evaluating common sub-expressions multiple times
 def parse_subexpression(expr, action_list):
-    if isinstance(expr, expression.ConstantNumeric) or (
-        isinstance(expr, expression.Parameter) and isinstance(expr.num, expression.ConstantNumeric)
-    ):
+    if isinstance(expr, expression.ConstantNumeric) or \
+            (isinstance(expr, expression.Parameter) and isinstance(expr.num, expression.ConstantNumeric)):
         return expr
     else:
         tmp_param, tmp_param_actions = get_tmp_parameter(expr)
         action_list.extend(tmp_param_actions)
         return expression.Parameter(expression.ConstantNumeric(tmp_param))
 
-
-# returns a (param_num, action_list) tuple.
+#returns a (param_num, action_list) tuple.
 def get_tmp_parameter(expr):
-    param = action6.free_parameters.pop(expr.pos)
+    param = action6.free_parameters.pop()
     actions = parse_actionD(ParameterAssignment(expression.Parameter(expression.ConstantNumeric(param)), expr))
     return (param, actions)
 
-
-def write_action_value(expr, action_list, act6, offset, size):
-    """
-    Write a single numeric value that is part of an action
-    Possibly use action6 and/or actionD if needed
-
-    @param expr: Expression to write
-    @type expr: L{Expression}
-
-    @param action_list: Action list to append any extra actions to
-    @type action_list: C{list} of L{BaseAction}
-
-    @param act6: Action6 to append any modifications to
-    @type act6: L{Action6}
-
-    @param offset: Offset to use for the action 6 (if applicable)
-    @type offset: C{int}
-
-    @param size: Size to use for the action 6 (if applicable)
-    @type size: C{int}
-
-    @return: 2-tuple containing -
-        - the value to be used when writing the action (0 if overwritten by action 6)
-        - the offset just past this numeric value (=offset + size)
-    @rtype: C{tuple} of (L{ConstantNumeric}, C{int})
-    """
-    if isinstance(expr, expression.ConstantNumeric):
-        result = expr
-    elif isinstance(expr, expression.Parameter) and isinstance(expr.num, expression.ConstantNumeric):
-        act6.modify_bytes(expr.num.value, size, offset)
-        result = expression.ConstantNumeric(0)
-    else:
-        tmp_param, tmp_param_actions = get_tmp_parameter(expr)
-        action_list.extend(tmp_param_actions)
-        act6.modify_bytes(tmp_param, size, offset)
-        result = expression.ConstantNumeric(0)
-    return result, offset + size
-
-
 def parse_ternary_op(assignment):
     assert isinstance(assignment.value, expression.TernaryOp)
     actions = parse_actionD(ParameterAssignment(assignment.param, assignment.value.expr2))
-    cond_block = conditional.Conditional(
-        assignment.value.guard, [ParameterAssignment(assignment.param, assignment.value.expr1)], None
-    )
-    actions.extend(conditional.ConditionalList([cond_block]).get_action_list())
-    return actions
-
-
-def parse_abs_op(assignment):
-    assert isinstance(assignment.value, expression.AbsOp)
-    actions = parse_actionD(ParameterAssignment(assignment.param, assignment.value.expr))
-    cond_block = conditional.Conditional(
-        nmlop.CMP_LT(assignment.value.expr, 0),
-        [ParameterAssignment(assignment.param, nmlop.SUB(0, assignment.value.expr))],
-        None,
-    )
-    actions.extend(conditional.ConditionalList([cond_block]).get_action_list())
+    cond_block = nml.ast.conditional.Conditional(assignment.value.guard, [ParameterAssignment(assignment.param, assignment.value.expr1)], None)
+    actions.extend(nml.ast.conditional.ConditionalList([cond_block]).get_action_list())
     return actions
 
-
 def parse_special_check(assignment):
     check = assignment.value
     assert isinstance(check, expression.SpecialCheck)
     actions = parse_actionD(ParameterAssignment(assignment.param, expression.ConstantNumeric(check.results[0])))
 
     value = check.value
+    size = 4
     if check.mask is not None:
         value &= check.mask
         value += check.mask << 32
-        assert check.varsize == 8
-    else:
-        assert check.varsize <= 4
-    actions.append(action7.SkipAction(9, check.varnum, check.varsize, check.op, value, 1))
+        size = 8
+    actions.append(nml.actions.action7.SkipAction(9, check.varnum, size, check.op, value, 1))
 
     actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.ConstantNumeric(check.results[1]))))
     return actions
 
-
 def parse_grm(assignment):
     assert isinstance(assignment.value, expression.GRMOp)
 
     action6.free_parameters.save()
     action_list = []
     act6 = action6.Action6()
     assert isinstance(assignment.param, expression.Parameter)
@@ -240,153 +152,129 @@
         action_list.extend(tmp_param_actions)
 
     op = nmlop.ASSIGN
     param1 = assignment.value.op
     param2 = expression.ConstantNumeric(0xFE)
     data = expression.ConstantNumeric(0xFF | (assignment.value.feature << 8) | (assignment.value.count << 16))
 
-    if len(act6.modifications) > 0:
-        action_list.append(act6)
+    if len(act6.modifications) > 0: action_list.append(act6)
 
     action_list.append(ActionD(target, param1, op, param2, data))
     action6.free_parameters.restore()
     return action_list
 
-
 def parse_hasbit(assignment):
-    assert isinstance(assignment.value, expression.BinOp) and (
-        assignment.value.op == nmlop.HASBIT or assignment.value.op == nmlop.NOTHASBIT
-    )
+    assert isinstance(assignment.value, expression.BinOp) and (assignment.value.op == nmlop.HASBIT or assignment.value.op == nmlop.NOTHASBIT)
     actions = parse_actionD(ParameterAssignment(assignment.param, expression.ConstantNumeric(0)))
-    cond_block = conditional.Conditional(
-        assignment.value, [ParameterAssignment(assignment.param, expression.ConstantNumeric(1))], None
-    )
-    actions.extend(conditional.ConditionalList([cond_block]).get_action_list())
+    cond_block = nml.ast.conditional.Conditional(assignment.value, [ParameterAssignment(assignment.param, expression.ConstantNumeric(1))], None)
+    actions.extend(nml.ast.conditional.ConditionalList([cond_block]).get_action_list())
     return actions
 
-
 def parse_min_max(assignment):
     assert isinstance(assignment.value, expression.BinOp) and assignment.value.op in (nmlop.MIN, nmlop.MAX)
-    # min(a, b) ==> a < b ? a : b.
-    # max(a, b) ==> a > b ? a : b.
+    #min(a, b) ==> a < b ? a : b.
+    #max(a, b) ==> a > b ? a : b.
     action6.free_parameters.save()
     action_list = []
     expr1 = parse_subexpression(assignment.value.expr1, action_list)
     expr2 = parse_subexpression(assignment.value.expr2, action_list)
     guard = expression.BinOp(nmlop.CMP_LT if assignment.value.op == nmlop.MIN else nmlop.CMP_GT, expr1, expr2)
-    action_list.extend(
-        parse_actionD(ParameterAssignment(assignment.param, expression.TernaryOp(guard, expr1, expr2, None)))
-    )
+    action_list.extend(parse_actionD(ParameterAssignment(assignment.param, expression.TernaryOp(guard, expr1, expr2, None))))
     action6.free_parameters.restore()
     return action_list
 
-
 def parse_boolean(assignment):
     assert isinstance(assignment.value, expression.Boolean)
     actions = parse_actionD(ParameterAssignment(assignment.param, expression.ConstantNumeric(0)))
-    expr = nmlop.CMP_NEQ(assignment.value.expr, 0)
-    cond_block = conditional.Conditional(
-        expr, [ParameterAssignment(assignment.param, expression.ConstantNumeric(1))], None
-    )
-    actions.extend(conditional.ConditionalList([cond_block]).get_action_list())
+    expr = expression.BinOp(nmlop.CMP_NEQ, assignment.value.expr, expression.ConstantNumeric(0))
+    cond_block = nml.ast.conditional.Conditional(expr, [ParameterAssignment(assignment.param, expression.ConstantNumeric(1))], None)
+    actions.extend(nml.ast.conditional.ConditionalList([cond_block]).get_action_list())
     return actions
 
-
 def transform_bin_op(assignment):
     op = assignment.value.op
     expr1 = assignment.value.expr1
     expr2 = assignment.value.expr2
     extra_actions = []
 
     if op == nmlop.CMP_GE:
         expr1, expr2 = expr2, expr1
         op = nmlop.CMP_LE
 
     if op == nmlop.CMP_LE:
-        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, nmlop.SUB(expr1, expr2))))
+        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.BinOp(nmlop.SUB, expr1, expr2))))
         op = nmlop.CMP_LT
         expr1 = assignment.param
         expr2 = expression.ConstantNumeric(1)
 
     if op == nmlop.CMP_GT:
         expr1, expr2 = expr2, expr1
         op = nmlop.CMP_LT
 
     if op == nmlop.CMP_LT:
-        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, nmlop.SUB(expr1, expr2))))
-        op = nmlop.SHIFTU_LEFT  # shift left by negative number = shift right
+        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.BinOp(nmlop.SUB, expr1, expr2))))
+        op = nmlop.SHIFTU_LEFT #shift left by negative number = shift right
         expr1 = assignment.param
         expr2 = expression.ConstantNumeric(-31)
 
     elif op == nmlop.CMP_NEQ:
-        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, nmlop.SUB(expr1, expr2))))
+        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.BinOp(nmlop.SUB, expr1, expr2))))
         op = nmlop.DIV
         # We rely here on the (ondocumented) behavior of both OpenTTD and TTDPatch
         # that expr/0==expr. What we do is compute A/A, which will result in 1 if
         # A != 0 and in 0 if A == 0
         expr1 = assignment.param
         expr2 = assignment.param
 
     elif op == nmlop.CMP_EQ:
         # We compute A==B by doing not(A - B) which will result in a value != 0
         # if A is equal to B
-        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, nmlop.SUB(expr1, expr2))))
+        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.BinOp(nmlop.SUB, expr1, expr2))))
         # Clamp the value to 0/1, see above for details
-        extra_actions.extend(
-            parse_actionD(ParameterAssignment(assignment.param, nmlop.DIV(assignment.param, assignment.param)))
-        )
+        extra_actions.extend(parse_actionD(ParameterAssignment(assignment.param, expression.BinOp(nmlop.DIV, assignment.param, assignment.param))))
         op = nmlop.SUB
         expr1 = expression.ConstantNumeric(1)
         expr2 = assignment.param
 
     if op == nmlop.SHIFT_RIGHT or op == nmlop.SHIFTU_RIGHT:
         if isinstance(expr2, expression.ConstantNumeric):
             expr2.value *= -1
         else:
-            expr2 = nmlop.SUB(0, expr2)
+            expr2 = expression.BinOp(nmlop.SUB, expression.ConstantNumeric(0), expr2)
         op = nmlop.SHIFT_LEFT if op == nmlop.SHIFT_RIGHT else nmlop.SHIFTU_LEFT
 
     elif op == nmlop.XOR:
-        # a ^ b ==> (a | b) - (a & b)
+        #a ^ b ==> (a | b) - (a & b)
         expr1 = parse_subexpression(expr1, extra_actions)
         expr2 = parse_subexpression(expr2, extra_actions)
-        tmp_param1, tmp_action_list1 = get_tmp_parameter(nmlop.OR(expr1, expr2))
-        tmp_param2, tmp_action_list2 = get_tmp_parameter(nmlop.AND(expr1, expr2))
+        tmp_param1, tmp_action_list1 = get_tmp_parameter(expression.BinOp(nmlop.OR, expr1, expr2))
+        tmp_param2, tmp_action_list2 = get_tmp_parameter(expression.BinOp(nmlop.AND, expr1, expr2))
         extra_actions.extend(tmp_action_list1)
         extra_actions.extend(tmp_action_list2)
         expr1 = expression.Parameter(expression.ConstantNumeric(tmp_param1))
         expr2 = expression.Parameter(expression.ConstantNumeric(tmp_param2))
         op = nmlop.SUB
 
     return op, expr1, expr2, extra_actions
 
-
 def parse_actionD(assignment):
     assignment.value.supported_by_actionD(True)
 
     if isinstance(assignment.param, expression.SpecialParameter):
         assignment.param, assignment.value = assignment.param.to_assignment(assignment.value)
     elif isinstance(assignment.param, expression.Identifier):
-        if global_constants.identifier_refcount[assignment.param.value] == 0:
-            # Named parameter is not referenced, ignoring
-            return []
-        assignment.param = expression.Parameter(
-            expression.ConstantNumeric(global_constants.named_parameters[assignment.param.value]), assignment.param.pos
-        )
+        assignment.param = expression.Parameter(expression.ConstantNumeric(global_constants.named_parameters[assignment.param.value]), assignment.param.pos)
     assert isinstance(assignment.param, expression.Parameter)
 
     if isinstance(assignment.value, expression.SpecialParameter):
         assignment.value = assignment.value.to_reading()
 
     if isinstance(assignment.value, expression.TernaryOp):
         return parse_ternary_op(assignment)
 
-    if isinstance(assignment.value, expression.AbsOp):
-        return parse_abs_op(assignment)
-
     if isinstance(assignment.value, expression.SpecialCheck):
         return parse_special_check(assignment)
 
     if isinstance(assignment.value, expression.GRMOp):
         return parse_grm(assignment)
 
     if isinstance(assignment.value, expression.BinOp):
@@ -396,19 +284,19 @@
         elif op == nmlop.MIN or op == nmlop.MAX:
             return parse_min_max(assignment)
 
     if isinstance(assignment.value, expression.Boolean):
         return parse_boolean(assignment)
 
     if isinstance(assignment.value, expression.Not):
-        expr = nmlop.SUB(1, assignment.value.expr)
+        expr = expression.BinOp(nmlop.SUB, expression.ConstantNumeric(1), assignment.value.expr)
         assignment = ParameterAssignment(assignment.param, expr)
 
     if isinstance(assignment.value, expression.BinNot):
-        expr = nmlop.SUB(0xFFFFFFFF, assignment.value.expr)
+        expr = expression.BinOp(nmlop.SUB, expression.ConstantNumeric(0xFFFFFFFF), assignment.value.expr)
         assignment = ParameterAssignment(assignment.param, expr)
 
     action6.free_parameters.save()
     action_list = []
     act6 = action6.Action6()
     assert isinstance(assignment.param, expression.Parameter)
     target = assignment.param.num
@@ -418,15 +306,15 @@
     elif not isinstance(target, expression.ConstantNumeric):
         tmp_param, tmp_param_actions = get_tmp_parameter(target)
         act6.modify_bytes(tmp_param, 1, 1)
         target = expression.ConstantNumeric(0)
         action_list.extend(tmp_param_actions)
 
     data = None
-    # print assignment.value
+    #print assignment.value
     if isinstance(assignment.value, expression.ConstantNumeric):
         op = nmlop.ASSIGN
         param1 = expression.ConstantNumeric(0xFF)
         param2 = expression.ConstantNumeric(0)
         data = assignment.value
     elif isinstance(assignment.value, expression.Parameter):
         if isinstance(assignment.value.num, expression.ConstantNumeric):
@@ -445,15 +333,15 @@
             param1 = assignment.value.num
         else:
             tmp_param, tmp_param_actions = get_tmp_parameter(assignment.value.num)
             act6.modify_bytes(tmp_param, 1, 3)
             action_list.extend(tmp_param_actions)
             param1 = expression.ConstantNumeric(0)
         param2 = expression.ConstantNumeric(0xFE)
-        data = expression.ConstantNumeric(expression.parse_string_to_dword(assignment.value.grfid))
+        data = assignment.value.grfid
     elif isinstance(assignment.value, expression.PatchVariable):
         op = nmlop.ASSIGN
         param1 = expression.ConstantNumeric(assignment.value.num)
         param2 = expression.ConstantNumeric(0xFE)
         data = expression.ConstantNumeric(0xFFFF)
     elif isinstance(assignment.value, expression.BinOp):
         op, expr1, expr2, extra_actions = transform_bin_op(assignment)
@@ -477,16 +365,14 @@
         elif isinstance(expr2, expression.Parameter) and isinstance(expr2.num, expression.ConstantNumeric):
             param2 = expr2.num
         else:
             tmp_param, tmp_param_actions = get_tmp_parameter(expr2)
             action_list.extend(tmp_param_actions)
             param2 = expression.ConstantNumeric(tmp_param)
 
-    else:
-        raise generic.ScriptError("Invalid expression in argument assignment", assignment.value.pos)
+    else: raise generic.ScriptError("Invalid expression in argument assignment", assignment.value.pos)
 
-    if len(act6.modifications) > 0:
-        action_list.append(act6)
+    if len(act6.modifications) > 0: action_list.append(act6)
 
     action_list.append(ActionD(target, param1, op, param2, data))
     action6.free_parameters.restore()
     return action_list
```

### Comparing `nml-0.7.2/nml/ast/base_statement.py` & `nml-r1512/nml/ast/base_statement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic
 
-
-class BaseStatement:
+class BaseStatement(object):
     """
     Base class for a statement (AST node) in NML.
     Note: All instance variables (except 'pos') are prefixed with "bs_" to avoid naming conflicts
 
     @ivar bs_name: Name of the statement type
     @type bs_name: C{str}
 
@@ -31,22 +15,21 @@
     @type bs_skipable: C{bool}
 
     @ivar bs_loopable: Whether the statement may be executed multiple times using a while-block (default: True)
     @type bs_loopable: C{bool}
 
     @pre: bs_skipable or not bs_loopable
 
-    @ivar bs_in_item: Whether the statement may be part of an item block (default: False)
+    @ivar bs_in_item: Whether the statement may be part of an item block (default: False_
     @type bs_in_item: C{bool}
 
     @ivar bs_out_item: Whether the statement may appear outside of item blocks (default: True)
     @type bs_out_item: C{bool}
     """
-
-    def __init__(self, name, pos, skipable=True, loopable=True, in_item=False, out_item=True):
+    def __init__(self, name, pos, skipable = True, loopable = True, in_item = False, out_item = True):
         assert skipable or not loopable
         self.bs_name = name
         self.pos = pos
         self.bs_skipable = skipable
         self.bs_loopable = loopable
         self.bs_in_item = in_item
         self.bs_out_item = out_item
@@ -57,27 +40,22 @@
 
         @param scope_list: List of nested blocks containing this statement
         @type scope_list: C{list} of L{BaseStatementList}
         """
         seen_item = False
         for scope in scope_list:
             if scope.list_type == BaseStatementList.LIST_TYPE_SKIP:
-                if not self.bs_skipable:
-                    raise generic.ScriptError(
-                        "{} may not appear inside a conditional block.".format(self.bs_name), self.pos
-                    )
+                if not self.bs_skipable: raise generic.ScriptError("%s may not appear inside a conditional block." % self.bs_name, self.pos)
             if scope.list_type == BaseStatementList.LIST_TYPE_LOOP:
-                if not self.bs_loopable:
-                    raise generic.ScriptError("{} may not appear inside a loop.".format(self.bs_name), self.pos)
+                if not self.bs_loopable: raise generic.ScriptError("%s may not appear inside a loop." % self.bs_name, self.pos)
             if scope.list_type == BaseStatementList.LIST_TYPE_ITEM:
                 seen_item = True
-                if not self.bs_in_item:
-                    raise generic.ScriptError("{} may not appear inside an item block.".format(self.bs_name), self.pos)
+                if not self.bs_in_item: raise generic.ScriptError("%s may not appear inside an item block." % self.bs_name, self.pos)
         if not (seen_item or self.bs_out_item):
-            raise generic.ScriptError("{} must appear inside an item block.".format(self.bs_name), self.pos)
+            raise generic.ScriptError("%s must appear inside an item block." % self.bs_name, self.pos)
 
     def register_names(self):
         """
         Called to register identifiers, that must be available before their definition.
         """
         pass
 
@@ -91,55 +69,52 @@
     def debug_print(self, indentation):
         """
         Print all AST information to the standard output
 
         @param indentation: Print all lines with at least C{indentation} spaces
         @type indentation: C{int}
         """
-        raise NotImplementedError("debug_print must be implemented in BaseStatement-subclass {!r}".format(type(self)))
+        raise NotImplementedError('debug_print must be implemented in BaseStatement-subclass %r' % type(self))
 
     def get_action_list(self):
         """
         Generate a list of NFO actions associated with this statement
 
         @return: A list of action
         @rtype: C{list} of L{BaseAction}
         """
-        raise NotImplementedError(
-            "get_action_list must be implemented in BaseStatement-subclass {!r}".format(type(self))
-        )
+        raise NotImplementedError('get_action_list must be implemented in BaseStatement-subclass %r' % type(self))
 
     def __str__(self):
         """
         Generate a string representing this statement in valid NML-code.
 
         @return: An NML string representing this action
         @rtype: C{str}
         """
-        raise NotImplementedError("__str__ must be implemented in BaseStatement-subclass {!r}".format(type(self)))
+        raise NotImplementedError('__str__ must be implemented in BaseStatement-subclass %r' % type(self))
 
 
 class BaseStatementList(BaseStatement):
     """
     Base class for anything that contains a list of statements
 
     @ivar list_type: Type of this list, used for validation logic
     @type list_type: C{int}, see constants below
     @pre list_type in (LIST_TYPE_NONE, LIST_TYPE_SKIP, LIST_TYPE_LOOP, LIST_TYPE_ITEM)
 
     @ivar statements: List of sub-statements in this block
     @type statements: C{list} of L{BaseStatement}
     """
-
     LIST_TYPE_NONE = 0
     LIST_TYPE_SKIP = 1
     LIST_TYPE_LOOP = 2
     LIST_TYPE_ITEM = 3
 
-    def __init__(self, name, pos, list_type, statements, skipable=True, loopable=True, in_item=False, out_item=True):
+    def __init__(self, name, pos, list_type, statements, skipable = True, loopable = True, in_item = False, out_item = True):
         BaseStatement.__init__(self, name, pos, skipable, loopable, in_item, out_item)
         assert list_type in (self.LIST_TYPE_NONE, self.LIST_TYPE_SKIP, self.LIST_TYPE_LOOP, self.LIST_TYPE_ITEM)
         self.list_type = list_type
         self.statements = statements
 
     def validate(self, scope_list):
         new_list = scope_list + [self]
@@ -161,11 +136,11 @@
     def get_action_list(self):
         action_list = []
         for stmt in self.statements:
             action_list.extend(stmt.get_action_list())
         return action_list
 
     def __str__(self):
-        res = ""
+        res = "" 
         for stmt in self.statements:
-            res += "\t" + str(stmt).replace("\n", "\n\t")[0:-1]
+            res += '\t' + str(stmt).replace('\n', '\n\t')[0:-1]
         return res
```

### Comparing `nml-0.7.2/nml/ast/basecost.py` & `nml-r1512/nml/ast/basecost.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,130 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import expression, generic, global_constants, nmlop
-from nml.actions import action0
 from nml.ast import assignment, base_statement
-
+from nml.actions import action0
 
 class BaseCost(base_statement.BaseStatement):
     """
     AST Node for a base costs table.
 
     @ivar costs: List of base cost values to set.
     @type costs: C{list} of L{Assignment}
     """
-
     def __init__(self, costs, pos):
         base_statement.BaseStatement.__init__(self, "basecost-block", pos)
         self.costs = costs
 
     def pre_process(self):
         new_costs = []
 
         for cost in self.costs:
             cost.value = cost.value.reduce(global_constants.const_list)
             if isinstance(cost.value, expression.ConstantNumeric):
-                generic.check_range(cost.value.value, -8, 16, "Base cost value", cost.value.pos)
-            cost.value = nmlop.ADD(cost.value, 8).reduce()
+                generic.check_range(cost.value.value, -8, 16, 'Base cost value', cost.value.pos)
+            cost.value = expression.BinOp(nmlop.ADD, cost.value, expression.ConstantNumeric(8), cost.value.pos).reduce()
 
             if isinstance(cost.name, expression.Identifier):
                 if cost.name.value in base_cost_table:
                     cost.name = expression.ConstantNumeric(base_cost_table[cost.name.value][0])
                     new_costs.append(cost)
                 elif cost.name.value in generic_base_costs:
-                    # create temporary list, so it can be sorted for efficiency
+                    #create temporary list, so it can be sorted for efficiency
                     tmp_list = []
                     for num, type in base_cost_table.values():
                         if type == cost.name.value:
-                            tmp_list.append(
-                                assignment.Assignment(expression.ConstantNumeric(num), cost.value, cost.name.pos)
-                            )
-                    tmp_list.sort(key=lambda x: x.name.value)
+                            tmp_list.append(assignment.Assignment(expression.ConstantNumeric(num), cost.value, cost.name.pos))
+                    tmp_list.sort(lambda x, y: cmp(x.name.value, y.name.value))
                     new_costs.extend(tmp_list)
                 else:
-                    raise generic.ScriptError(
-                        "Unrecognized base cost identifier '{}' encountered".format(cost.name.value), cost.name.pos
-                    )
+                    raise generic.ScriptError("Unrecognized base cost identifier '%s' encountered" % cost.name.value, cost.name.pos)
             else:
                 cost.name = cost.name.reduce()
                 if isinstance(cost.name, expression.ConstantNumeric):
-                    generic.check_range(cost.name.value, 0, len(base_cost_table), "Base cost number", cost.name.pos)
+                    generic.check_range(cost.name.value, 0, len(base_cost_table), 'Base cost number', cost.name.pos)
                 new_costs.append(cost)
         self.costs = new_costs
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Base costs")
+        print indentation*' ' + 'Base costs'
         for cost in self.costs:
             cost.debug_print(indentation + 2)
 
     def get_action_list(self):
         return action0.get_basecost_action(self)
 
     def __str__(self):
         ret = "basecost {\n"
         for cost in self.costs:
-            ret += "\t{}: {};\n".format(cost.name, cost.value)
+            ret += "\t%s: %s;\n" % (str(cost.name), str(cost.value))
         ret += "}\n"
         return ret
 
-
 base_cost_table = {
-    "PR_STATION_VALUE": (0, ""),
-    "PR_BUILD_RAIL": (1, "PR_CONSTRUCTION"),
-    "PR_BUILD_ROAD": (2, "PR_CONSTRUCTION"),
-    "PR_BUILD_SIGNALS": (3, "PR_CONSTRUCTION"),
-    "PR_BUILD_BRIDGE": (4, "PR_CONSTRUCTION"),
-    "PR_BUILD_DEPOT_TRAIN": (5, "PR_CONSTRUCTION"),
-    "PR_BUILD_DEPOT_ROAD": (6, "PR_CONSTRUCTION"),
-    "PR_BUILD_DEPOT_SHIP": (7, "PR_CONSTRUCTION"),
-    "PR_BUILD_TUNNEL": (8, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_RAIL": (9, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_RAIL_LENGTH": (10, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_AIRPORT": (11, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_BUS": (12, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_TRUCK": (13, "PR_CONSTRUCTION"),
-    "PR_BUILD_STATION_DOCK": (14, "PR_CONSTRUCTION"),
-    "PR_BUILD_VEHICLE_TRAIN": (15, "PR_BUILD_VEHICLE"),
-    "PR_BUILD_VEHICLE_WAGON": (16, "PR_BUILD_VEHICLE"),
-    "PR_BUILD_VEHICLE_AIRCRAFT": (17, "PR_BUILD_VEHICLE"),
-    "PR_BUILD_VEHICLE_ROAD": (18, "PR_BUILD_VEHICLE"),
-    "PR_BUILD_VEHICLE_SHIP": (19, "PR_BUILD_VEHICLE"),
-    "PR_BUILD_TREES": (20, "PR_CONSTRUCTION"),
-    "PR_TERRAFORM": (21, "PR_CONSTRUCTION"),
-    "PR_CLEAR_GRASS": (22, "PR_CONSTRUCTION"),
-    "PR_CLEAR_ROUGH": (23, "PR_CONSTRUCTION"),
-    "PR_CLEAR_ROCKS": (24, "PR_CONSTRUCTION"),
-    "PR_CLEAR_FIELDS": (25, "PR_CONSTRUCTION"),
-    "PR_CLEAR_TREES": (26, "PR_CONSTRUCTION"),
-    "PR_CLEAR_RAIL": (27, "PR_CONSTRUCTION"),
-    "PR_CLEAR_SIGNALS": (28, "PR_CONSTRUCTION"),
-    "PR_CLEAR_BRIDGE": (29, "PR_CONSTRUCTION"),
-    "PR_CLEAR_DEPOT_TRAIN": (30, "PR_CONSTRUCTION"),
-    "PR_CLEAR_DEPOT_ROAD": (31, "PR_CONSTRUCTION"),
-    "PR_CLEAR_DEPOT_SHIP": (32, "PR_CONSTRUCTION"),
-    "PR_CLEAR_TUNNEL": (33, "PR_CONSTRUCTION"),
-    "PR_CLEAR_WATER": (34, "PR_CONSTRUCTION"),
-    "PR_CLEAR_STATION_RAIL": (35, "PR_CONSTRUCTION"),
-    "PR_CLEAR_STATION_AIRPORT": (36, "PR_CONSTRUCTION"),
-    "PR_CLEAR_STATION_BUS": (37, "PR_CONSTRUCTION"),
-    "PR_CLEAR_STATION_TRUCK": (38, "PR_CONSTRUCTION"),
-    "PR_CLEAR_STATION_DOCK": (39, "PR_CONSTRUCTION"),
-    "PR_CLEAR_HOUSE": (40, "PR_CONSTRUCTION"),
-    "PR_CLEAR_ROAD": (41, "PR_CONSTRUCTION"),
-    "PR_RUNNING_TRAIN_STEAM": (42, "PR_RUNNING"),
-    "PR_RUNNING_TRAIN_DIESEL": (43, "PR_RUNNING"),
-    "PR_RUNNING_TRAIN_ELECTRIC": (44, "PR_RUNNING"),
-    "PR_RUNNING_AIRCRAFT": (45, "PR_RUNNING"),
-    "PR_RUNNING_ROADVEH": (46, "PR_RUNNING"),
-    "PR_RUNNING_SHIP": (47, "PR_RUNNING"),
-    "PR_BUILD_INDUSTRY": (48, "PR_CONSTRUCTION"),
-    "PR_CLEAR_INDUSTRY": (49, "PR_CONSTRUCTION"),
-    "PR_BUILD_UNMOVABLE": (50, "PR_CONSTRUCTION"),
-    "PR_CLEAR_UNMOVABLE": (51, "PR_CONSTRUCTION"),
-    "PR_BUILD_WAYPOINT_RAIL": (52, "PR_CONSTRUCTION"),
-    "PR_CLEAR_WAYPOINT_RAIL": (53, "PR_CONSTRUCTION"),
-    "PR_BUILD_WAYPOINT_BUOY": (54, "PR_CONSTRUCTION"),
-    "PR_CLEAR_WAYPOINT_BUOY": (55, "PR_CONSTRUCTION"),
-    "PR_TOWN_ACTION": (56, "PR_CONSTRUCTION"),
-    "PR_BUILD_FOUNDATION": (57, "PR_CONSTRUCTION"),
-    "PR_BUILD_INDUSTRY_RAW": (58, "PR_CONSTRUCTION"),
-    "PR_BUILD_TOWN": (59, "PR_CONSTRUCTION"),
-    "PR_BUILD_CANAL": (60, "PR_CONSTRUCTION"),
-    "PR_CLEAR_CANAL": (61, "PR_CONSTRUCTION"),
-    "PR_BUILD_AQUEDUCT": (62, "PR_CONSTRUCTION"),
-    "PR_CLEAR_AQUEDUCT": (63, "PR_CONSTRUCTION"),
-    "PR_BUILD_LOCK": (64, "PR_CONSTRUCTION"),
-    "PR_CLEAR_LOCK": (65, "PR_CONSTRUCTION"),
-    "PR_MAINTENANCE_RAIL": (66, "PR_RUNNING"),
-    "PR_MAINTENANCE_ROAD": (67, "PR_RUNNING"),
-    "PR_MAINTENANCE_CANAL": (68, "PR_RUNNING"),
-    "PR_MAINTENANCE_STATION": (69, "PR_RUNNING"),
-    "PR_MAINTENANCE_AIRPORT": (70, "PR_RUNNING"),
+    'PR_STATION_VALUE'              : (0,  ''),
+    'PR_BUILD_RAIL'                 : (1,  'PR_CONSTRUCTION'),
+    'PR_BUILD_ROAD'                 : (2,  'PR_CONSTRUCTION'),
+    'PR_BUILD_SIGNALS'              : (3,  'PR_CONSTRUCTION'),
+    'PR_BUILD_BRIDGE'               : (4,  'PR_CONSTRUCTION'),
+    'PR_BUILD_DEPOT_TRAIN'          : (5,  'PR_CONSTRUCTION'),
+    'PR_BUILD_DEPOT_ROAD'           : (6,  'PR_CONSTRUCTION'),
+    'PR_BUILD_DEPOT_SHIP'           : (7,  'PR_CONSTRUCTION'),
+    'PR_BUILD_TUNNEL'               : (8,  'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_RAIL'         : (9,  'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_RAIL_LENGTH'  : (10, 'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_AIRPORT'      : (11, 'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_BUS'          : (12, 'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_TRUCK'        : (13, 'PR_CONSTRUCTION'),
+    'PR_BUILD_STATION_DOCK'         : (14, 'PR_CONSTRUCTION'),
+    'PR_BUILD_VEHICLE_TRAIN'        : (15, 'PR_BUILD_VEHICLE'),
+    'PR_BUILD_VEHICLE_WAGON'        : (16, 'PR_BUILD_VEHICLE'),
+    'PR_BUILD_VEHICLE_AIRCRAFT'     : (17, 'PR_BUILD_VEHICLE'),
+    'PR_BUILD_VEHICLE_ROAD'         : (18, 'PR_BUILD_VEHICLE'),
+    'PR_BUILD_VEHICLE_SHIP'         : (19, 'PR_BUILD_VEHICLE'),
+    'PR_BUILD_TREES'                : (20, 'PR_CONSTRUCTION'),
+    'PR_TERRAFORM'                  : (21, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_GRASS'                : (22, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_ROUGH'                : (23, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_ROCKS'                : (24, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_FIELDS'               : (25, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_TREES'                : (26, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_RAIL'                 : (27, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_SIGNALS'              : (28, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_BRIDGE'               : (29, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_DEPOT_TRAIN'          : (30, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_DEPOT_ROAD'           : (31, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_DEPOT_SHIP'           : (32, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_TUNNEL'               : (33, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_WATER'                : (34, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_STATION_RAIL'         : (35, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_STATION_AIRPORT'      : (36, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_STATION_BUS'          : (37, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_STATION_TRUCK'        : (38, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_STATION_DOCK'         : (39, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_HOUSE'                : (40, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_ROAD'                 : (41, 'PR_CONSTRUCTION'),
+    'PR_RUNNING_TRAIN_STEAM'        : (42, 'PR_RUNNING'),
+    'PR_RUNNING_TRAIN_DIESEL'       : (43, 'PR_RUNNING'),
+    'PR_RUNNING_TRAIN_ELECTRIC'     : (44, 'PR_RUNNING'),
+    'PR_RUNNING_AIRCRAFT'           : (45, 'PR_RUNNING'),
+    'PR_RUNNING_ROADVEH'            : (46, 'PR_RUNNING'),
+    'PR_RUNNING_SHIP'               : (47, 'PR_RUNNING'),
+    'PR_BUILD_INDUSTRY'             : (48, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_INDUSTRY'             : (49, 'PR_CONSTRUCTION'),
+    'PR_BUILD_UNMOVABLE'            : (50, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_UNMOVABLE'            : (51, 'PR_CONSTRUCTION'),
+    'PR_BUILD_WAYPOINT_RAIL'        : (52, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_WAYPOINT_RAIL'        : (53, 'PR_CONSTRUCTION'),
+    'PR_BUILD_WAYPOINT_BUOY'        : (54, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_WAYPOINT_BUOY'        : (55, 'PR_CONSTRUCTION'),
+    'PR_TOWN_ACTION'                : (56, 'PR_CONSTRUCTION'),
+    'PR_BUILD_FOUNDATION'           : (57, 'PR_CONSTRUCTION'),
+    'PR_BUILD_INDUSTRY_RAW'         : (58, 'PR_CONSTRUCTION'),
+    'PR_BUILD_TOWN'                 : (59, 'PR_CONSTRUCTION'),
+    'PR_BUILD_CANAL'                : (60, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_CANAL'                : (61, 'PR_CONSTRUCTION'),
+    'PR_BUILD_AQUEDUCT'             : (62, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_AQUEDUCT'             : (63, 'PR_CONSTRUCTION'),
+    'PR_BUILD_LOCK'                 : (64, 'PR_CONSTRUCTION'),
+    'PR_CLEAR_LOCK'                 : (65, 'PR_CONSTRUCTION'),
 }
 
-generic_base_costs = ["PR_CONSTRUCTION", "PR_RUNNING", "PR_BUILD_VEHICLE"]
+generic_base_costs = ['PR_CONSTRUCTION', 'PR_RUNNING', 'PR_BUILD_VEHICLE']
```

### Comparing `nml-0.7.2/nml/ast/cargotable.py` & `nml-r1512/nml/ast/cargotable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,28 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic, global_constants
+from nml import generic, global_constants, expression
 from nml.actions import action0
 from nml.ast import base_statement
 
-
 class CargoTable(base_statement.BaseStatement):
     def __init__(self, cargo_list, pos):
         base_statement.BaseStatement.__init__(self, "cargo table", pos, False, False)
         self.cargo_list = cargo_list
-
-    def register_names(self):
         generic.OnlyOnce.enforce(self, "cargo table")
-        for i, cargo in enumerate(self.cargo_list):
+        for i, cargo in enumerate(cargo_list):
             if isinstance(cargo, expression.Identifier):
-                self.cargo_list[i] = expression.StringLiteral(cargo.value, cargo.pos)
-            expression.parse_string_to_dword(
-                self.cargo_list[i]
-            )  # we don't care about the result, only validate the input
-            if self.cargo_list[i].value in global_constants.cargo_numbers:
-                generic.print_warning(
-                    generic.Warning.GENERIC,
-                    "Duplicate entry in cargo table: {}".format(self.cargo_list[i].value),
-                    cargo.pos,
-                )
-            else:
-                global_constants.cargo_numbers[self.cargo_list[i].value] = i
+                 self.cargo_list[i] = expression.StringLiteral(cargo.value, cargo.pos)
+            expression.parse_string_to_dword(self.cargo_list[i])
+            global_constants.cargo_numbers[self.cargo_list[i].value] = i
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Cargo table")
+        print indentation*' ' + 'Cargo table'
         for cargo in self.cargo_list:
-            generic.print_dbg(indentation, "Cargo:", cargo.value)
+            print (indentation+2)*' ' + 'Cargo:', cargo.value
 
     def get_action_list(self):
         return action0.get_cargolist_action(self.cargo_list)
 
     def __str__(self):
-        ret = "cargotable {\n"
-        ret += ", ".join([expression.identifier_to_print(cargo.value) for cargo in self.cargo_list])
-        ret += "\n}\n"
+        ret = 'cargotable {\n'
+        ret += ', '.join([expression.identifier_to_print(cargo.value) for cargo in self.cargo_list])
+        ret += '\n}\n'
         return ret
```

### Comparing `nml-0.7.2/nml/ast/conditional.py` & `nml-r1512/nml/ast/conditional.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,59 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic, global_constants
+from nml import global_constants
 from nml.actions import action7
 from nml.ast import base_statement
 
-
 class ConditionalList(base_statement.BaseStatementList):
     """
     Wrapper for a complete if/else if/else if/else block.
     """
-
     def __init__(self, conditionals):
         assert len(conditionals) > 0
-        base_statement.BaseStatementList.__init__(
-            self,
-            "if/else-block",
-            conditionals[0].pos,
-            base_statement.BaseStatementList.LIST_TYPE_SKIP,
-            conditionals,
-            in_item=True,
-        )
+        base_statement.BaseStatementList.__init__(self, "if/else-block", conditionals[0].pos,
+                base_statement.BaseStatementList.LIST_TYPE_SKIP, conditionals, in_item = True)
 
     def get_action_list(self):
         return action7.parse_conditional_block(self)
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Conditional")
+        print indentation*' ' + 'Conditional'
         base_statement.BaseStatementList.debug_print(self, indentation + 2)
 
     def __str__(self):
-        ret = ""
-        ret += " else ".join([str(stmt) for stmt in self.statements])
-        ret += "\n"
+        ret = ''
+        ret += ' else '.join([str(stmt) for stmt in self.statements])
+        ret += '\n'
         return ret
 
-
 class Conditional(base_statement.BaseStatementList):
     """
     Condition along with the code that has to be executed if the condition
     evaluates to some value not equal to 0.
 
     @ivar expr: The expression where the execution of code in this block depends on.
     @type expr: L{Expression}
     """
-
     def __init__(self, expr, block, pos):
-        base_statement.BaseStatementList.__init__(
-            self, "if/else-block", pos, base_statement.BaseStatementList.LIST_TYPE_SKIP, block, in_item=True
-        )
+        base_statement.BaseStatementList.__init__(self, "if/else-block", pos,
+                base_statement.BaseStatementList.LIST_TYPE_SKIP, block, in_item = True)
         self.expr = expr
 
     def pre_process(self):
         if self.expr is not None:
             self.expr = self.expr.reduce(global_constants.const_list)
         base_statement.BaseStatementList.pre_process(self)
 
     def debug_print(self, indentation):
         if self.expr is not None:
-            generic.print_dbg(indentation, "Expression:")
+            print indentation*' ' + 'Expression:'
             self.expr.debug_print(indentation + 2)
-
-        generic.print_dbg(indentation, "Block:")
+        print indentation*' ' + 'Block:'
         base_statement.BaseStatementList.debug_print(self, indentation + 2)
 
     def __str__(self):
-        ret = ""
+        ret = ''
         if self.expr is not None:
-            ret += "if ({})".format(self.expr)
-        ret += " {\n"
+            ret += 'if (%s)' % str(self.expr)
+        ret += ' {\n'
         ret += base_statement.BaseStatementList.__str__(self)
-        ret += "}\n"
+        ret += '}\n'
         return ret
```

### Comparing `nml-0.7.2/nml/ast/disable_item.py` & `nml-r1512/nml/ast/disable_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,28 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic, global_constants
+from nml import expression, generic, global_constants
 from nml.actions import action0
 from nml.ast import base_statement, general
 
-
 class DisableItem(base_statement.BaseStatement):
     """
     Class representing a 'disable_item' statement in the AST.
 
     @ivar feature: Feature of the items to disable
     @type feature: L{ConstantNumeric}
 
     @ivar first_id: First item ID to disable
     @type first_id: L{ConstantNumeric}, or C{None} if not set
 
     @ivar last_id: Last item ID to disable
     @type last_id: L{ConstantNumeric}, or C{None} if not set
     """
-
     def __init__(self, param_list, pos):
         base_statement.BaseStatement.__init__(self, "disable_item()", pos)
         if not (1 <= len(param_list) <= 3):
-            raise generic.ScriptError(
-                "disable_item() requires between 1 and 3 parameters, encountered {:d}.".format(len(param_list)), pos
-            )
+            raise generic.ScriptError("disable_item() requires between 1 and 3 parameters, encountered %d." % len(param_list), pos)
         self.feature = general.parse_feature(param_list[0])
 
         if len(param_list) > 1:
             self.first_id = param_list[1].reduce_constant(global_constants.const_list)
         else:
             self.first_id = None
 
@@ -49,25 +30,23 @@
             self.last_id = param_list[2].reduce_constant(global_constants.const_list)
             if self.last_id.value < self.first_id.value:
                 raise generic.ScriptError("Last id to disable may not be lower than the first id.", pos)
         else:
             self.last_id = None
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Disable items, feature=" + str(self.feature.value))
+        print indentation*' ' + 'Disable items, feature=' + str(self.feature.value)
         if self.first_id is not None:
-            generic.print_dbg(indentation + 2, "First ID:")
+            print (indentation+2)*' ' + 'First ID:'
             self.first_id.debug_print(indentation + 4)
         if self.last_id is not None:
-            generic.print_dbg(indentation + 2, "Last ID:")
+            print (indentation+2)*' ' + 'Last ID:'
             self.last_id.debug_print(indentation + 4)
 
     def __str__(self):
         ret = str(self.feature)
-        if self.first_id is not None:
-            ret += ", " + str(self.first_id)
-        if self.last_id is not None:
-            ret += ", " + str(self.last_id)
-        return "disable_item({});\n".format(ret)
+        if self.first_id is not None: ret += ', ' + str(self.first_id)
+        if self.last_id is not None: ret += ', ' + str(self.last_id)
+        return 'disable_item(%s);\n' % ret
 
     def get_action_list(self):
         return action0.get_disable_actions(self)
```

### Comparing `nml-0.7.2/nml/ast/error.py` & `nml-r1512/nml/ast/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic
+from nml import generic, expression
 from nml.actions import actionB
 from nml.ast import base_statement
 
-
 class Error(base_statement.BaseStatement):
     """
     An error has occured while parsing the GRF. This can be anything ranging from
     an imcompatible GRF file that was found or a game setting that is set to the
     wrong value to a wrong combination of parameters. The action taken by the host
     depends on the severity level of the error.
     NML equivalent: error(level, message[, extra_text[, parameter1[, parameter2]]]).
@@ -37,64 +21,57 @@
                language file.
     @type msg: L{Expression}
 
     @ivar data: Optional extra message that is inserted in place of the second
                 {STRING}-code of msg.
     @type data: C{None} or L{String} or L{StringLiteral}
     """
-
     def __init__(self, param_list, pos):
         base_statement.BaseStatement.__init__(self, "error()", pos)
         if not 2 <= len(param_list) <= 5:
-            raise generic.ScriptError(
-                "'error' expects between 2 and 5 parameters, got " + str(len(param_list)), self.pos
-            )
+            raise generic.ScriptError("'error' expects between 2 and 5 parameters, got " + str(len(param_list)), self.pos)
         self.severity = param_list[0]
-        self.msg = param_list[1]
-        self.data = param_list[2] if len(param_list) >= 3 else None
+        self.msg      = param_list[1]
+        self.data     = param_list[2] if len(param_list) >= 3 else None
         self.params = param_list[3:]
 
     def pre_process(self):
         self.severity = self.severity.reduce([actionB.error_severity])
-        self.msg = self.msg.reduce([actionB.default_error_msg])
+        self.msg      = self.msg.reduce([actionB.default_error_msg])
         if self.data:
             self.data = self.data.reduce()
         self.params = [x.reduce() for x in self.params]
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Error message")
-        generic.print_dbg(indentation + 2, "Message:")
+        print indentation*' ' + 'Error message'
+        print (indentation+2)*' ' + 'Message:'
         self.msg.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation + 2, "Severity:")
+        print (indentation+2)*' ' + 'Severity:'
         self.severity.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation, "Data: ")
-        if self.data is not None:
-            self.data.debug_print(indentation + 4)
-
+        print (indentation+2)*' ' + 'Data: '
+        if self.data is not None: self.data.debug_print(indentation + 4)
         if len(self.params) > 0:
-            generic.print_dbg(indentation + 2, "Param1: ")
+            print (indentation+2)*' ' + 'Param1: '
             self.params[0].debug_print(indentation + 4)
         if len(self.params) > 1:
-            generic.print_dbg(indentation + 2, "Param2: ")
+            print (indentation+2)*' ' + 'Param2: '
             self.params[1].debug_print(indentation + 4)
 
     def get_action_list(self):
         return actionB.parse_error_block(self)
 
     def __str__(self):
         sev = str(self.severity)
         if isinstance(self.severity, expression.ConstantNumeric):
             for s in actionB.error_severity:
                 if self.severity.value == actionB.error_severity[s]:
                     sev = s
                     break
-        res = "error({}, {}".format(sev, self.msg)
+        res = 'error(%s, %s' % (sev, self.msg)
         if self.data is not None:
-            res += ", {}".format(self.data)
+            res += ', %s' % self.data
         if len(self.params) > 0:
-            res += ", {}".format(self.params[0])
+            res += ', %s' % self.params[0]
         if len(self.params) > 1:
-            res += ", {}".format(self.params[1])
-        res += ");\n"
+            res += ', %s' % self.params[1]
+        res += ');\n'
         return res
```

### Comparing `nml-0.7.2/nml/ast/grf.py` & `nml-r1512/nml/ast/grf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,23 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import expression, generic, global_constants, grfstrings
+from nml import expression, generic, grfstrings, global_constants
 from nml.actions import action8, action14
 from nml.ast import base_statement
 
 palette_node = None
-blitter_node = None
-
-"""
-Statistics about registers used for parameters.
-The 1st field is the largest parameter register used.
-The 2nd field is the maximum amount of parameter registers available. This is where L{action6.free_parameters} begins.
-"""
-param_stats = [0, 0x40]
-
-
-def print_stats():
-    """
-    Print statistics about used ids.
-    """
-    if param_stats[0] > 0:
-        generic.print_info("GRF parameter registers: {}/{}".format(param_stats[0], param_stats[1]))
-
 
 def set_palette_used(pal):
     """
     Set the used palette in the action 14 node, if applicable
 
     @param pal: Palette to use
     @type pal: C{str} of length 1
     """
     if palette_node:
         palette_node.pal = pal
 
-
-def set_preferred_blitter(blitter):
-    """
-    Set the preferred blitter in the action14 node, if applicable
-
-    @param blitter: The blitter to set
-    @type blitter: C{str} of length 1
-    """
-    if blitter_node:
-        blitter_node.blitter = blitter
-
-
 class GRF(base_statement.BaseStatement):
     """
     AST Node for a grf block, that supplies (static) information about the GRF
     This is equivalent to actions 8 and 14
 
     @ivar name: Name of the GRF (short)
     @type name: L{Expression}, should be L{String} else user error
@@ -77,270 +33,194 @@
 
     @ivar min_compatible_version: Minimum (older) version of the same GRF that it is compatible with
     @type min_compatible_version: L{Expression}
 
     @ivar params: List of user-configurable GRF parameters
     @type params: C{list} of L{ParameterDescription}
     """
-
     def __init__(self, alist, pos):
         base_statement.BaseStatement.__init__(self, "grf-block", pos, False, False)
         self.name = None
         self.desc = None
-        self.url = None
         self.grfid = None
         self.version = None
         self.min_compatible_version = None
         self.params = []
+        generic.OnlyOnce.enforce(self, "GRF-block")
         for assignment in alist:
             if isinstance(assignment, ParameterDescription):
                 self.params.append(assignment)
-            elif assignment.name.value == "name":
-                self.name = assignment.value
-            elif assignment.name.value == "desc":
-                self.desc = assignment.value
-            elif assignment.name.value == "url":
-                self.url = assignment.value
-            elif assignment.name.value == "grfid":
-                self.grfid = assignment.value
-            elif assignment.name.value == "version":
-                self.version = assignment.value
-            elif assignment.name.value == "min_compatible_version":
-                self.min_compatible_version = assignment.value
-            else:
-                raise generic.ScriptError("Unknown item in GRF-block: " + str(assignment.name), assignment.name.pos)
-
-    def register_names(self):
-        generic.OnlyOnce.enforce(self, "GRF-block")
+            elif assignment.name.value == "name": self.name = assignment.value
+            elif assignment.name.value == "desc": self.desc = assignment.value
+            elif assignment.name.value == "grfid": self.grfid = assignment.value
+            elif assignment.name.value == "version": self.version = assignment.value
+            elif assignment.name.value == "min_compatible_version": self.min_compatible_version = assignment.value
+            else: raise generic.ScriptError("Unknown item in GRF-block: " + str(assignment.name), assignment.name.pos)
 
     def pre_process(self):
         if None in (self.name, self.desc, self.grfid, self.version, self.min_compatible_version):
-            raise generic.ScriptError(
-                "A GRF-block requires the"
-                " 'name', 'desc', 'grfid', 'version' and 'min_compatible_version' properties to be set.",
-                self.pos,
-            )
+            raise generic.ScriptError("A GRF-block requires the 'name', 'desc', 'grfid', 'version' and 'min_compatible_version' properties to be set.", self.pos)
 
         self.grfid = self.grfid.reduce()
-        global_constants.constant_numbers["GRFID"] = expression.parse_string_to_dword(self.grfid)
+        global_constants.constant_numbers['GRFID'] = expression.parse_string_to_dword(self.grfid)
         self.name = self.name.reduce()
         if not isinstance(self.name, expression.String):
             raise generic.ScriptError("GRF-name must be a string", self.name.pos)
         grfstrings.validate_string(self.name)
         self.desc = self.desc.reduce()
         if not isinstance(self.desc, expression.String):
             raise generic.ScriptError("GRF-description must be a string", self.desc.pos)
         grfstrings.validate_string(self.desc)
-        if self.url is not None:
-            self.url = self.url.reduce()
-            if not isinstance(self.url, expression.String):
-                raise generic.ScriptError("URL must be a string", self.url.pos)
-            grfstrings.validate_string(self.url)
         self.version = self.version.reduce_constant()
         self.min_compatible_version = self.min_compatible_version.reduce_constant()
-
-        global param_stats
-
         param_num = 0
         for param in self.params:
             param.pre_process(expression.ConstantNumeric(param_num))
             param_num = param.num.value + 1
-            if param_num > param_stats[1]:
-                raise generic.ScriptError(
-                    "No free parameters available."
-                    " Consider assigning <num> manually and combine multiple bool parameters into"
-                    " a single bitmask parameter using <bit>.",
-                    self.pos,
-                )
-            if param_num > param_stats[0]:
-                param_stats[0] = param_num
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "GRF")
-        generic.print_dbg(indentation + 2, "grfid:")
+        print indentation*' ' + 'GRF'
+        print (2+indentation)*' ' + 'grfid:'
         self.grfid.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation + 2, "Name:")
+        print (2+indentation)*' ' + 'Name:'
         self.name.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation + 2, "Description:")
+        print (2+indentation)*' ' + 'Description:'
         self.desc.debug_print(indentation + 4)
-
-        if self.url is not None:
-            generic.print_dbg(indentation + 2, "URL:")
-            self.url.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation + 2, "Version:")
+        print (2+indentation)*' ' + 'Version:'
         self.version.debug_print(indentation + 4)
-
-        generic.print_dbg(indentation + 2, "Minimal compatible version:")
+        print (2+indentation)*' ' + 'Minimal compatible version:'
         self.min_compatible_version.debug_print(indentation + 4)
 
-        if len(self.params) > 0:
-            generic.print_dbg(indentation + 2, "Params:")
-            for param in self.params:
-                param.debug_print(indentation + 4)
-
     def get_action_list(self):
-        global palette_node, blitter_node
+        global palette_node
         palette_node = action14.UsedPaletteNode("A")
-        blitter_node = action14.BlitterNode("8")
         action14_root = action14.BranchNode("INFO")
-        action14.grf_name_desc_actions(
-            action14_root, self.name, self.desc, self.url, self.version, self.min_compatible_version
-        )
+        action14.grf_name_desc_actions(action14_root, self.name, self.desc, self.version, self.min_compatible_version)
         action14.param_desc_actions(action14_root, self.params)
         action14_root.subnodes.append(palette_node)
-        action14_root.subnodes.append(blitter_node)
         return action14.get_actions(action14_root) + [action8.Action8(self.grfid, self.name, self.desc)]
 
     def __str__(self):
-        ret = "grf {\n"
-        ret += "\tgrfid: {};\n".format(str(self.grfid))
-        ret += "\tname: {};\n".format(str(self.name))
-        ret += "\tdesc: {};\n".format(str(self.desc))
-        if self.url is not None:
-            ret += "\turl: {};\n".format(self.url)
-        ret += "\tversion: {};\n".format(self.version)
-        ret += "\tmin_compatible_version: {};\n".format(self.min_compatible_version)
+        ret = 'grf {\n'
+        ret += '\tgrfid: %s;\n' % str(self.grfid)
+        ret += '\tname: %s;\n' % str(self.name)
+        ret += '\tdesc: %s;\n' % str(self.desc)
+        ret += '\tversion: %s;\n' % str(self.version)
+        ret += '\tmin_compatible_version: %s;\n' % str(self.min_compatible_version)
         for param in self.params:
             ret += str(param)
-        ret += "}\n"
+        ret += '}\n'
         return ret
 
-
-class ParameterSetting:
+class ParameterSetting(object):
     def __init__(self, name, value_list):
         self.name = name
         self.value_list = value_list
-        self.type = "int"
+        self.type = 'int'
         self.name_string = None
         self.desc_string = None
         self.min_val = None
         self.max_val = None
         self.def_val = None
         self.bit_num = None
         self.val_names = []
         self.properties_set = set()
 
     def pre_process(self):
         for set_val in self.value_list:
             self.set_property(set_val.name.value, set_val.value)
 
     def __str__(self):
-        ret = "\t\t{} {{\n".format(self.name)
+        ret = "\t\t%s {\n" % str(self.name)
         for val in self.value_list:
-            if val.name.value == "names":
+            if val.name.value == 'names':
                 ret += "\t\t\tnames: {\n"
                 for name in val.value.values:
-                    ret += "\t\t\t\t{}: {};\n".format(name.name, name.value)
+                    ret += "\t\t\t\t%s: %s;\n" % (name.name, name.value)
                 ret += "\t\t\t};\n"
             else:
-                ret += "\t\t\t{}: {};\n".format(val.name, val.value)
+                ret += "\t\t\t%s: %s;\n" % (val.name, val.value)
         ret += "\t\t}\n"
         return ret
 
-    def debug_print(self, indentation):
-        self.name.debug_print(indentation)
-        for val in self.value_list:
-            val.name.debug_print(indentation + 2)
-            if val.name.value == "names":
-                for name in val.value.values:
-                    name.name.debug_print(indentation + 4)
-                    name.value.debug_print(indentation + 4)
-            else:
-                val.value.debug_print(indentation + 4)
-
     def set_property(self, name, value):
         """
         Set a single parameter property
 
         @param name: Name of the property to be set
-        @type name: C{str}
+        @type name: C{basestring}
 
         @param value: Value of the property (note: may be an array)
         @type value: L{Expression}
         """
         if name in self.properties_set:
-            raise generic.ScriptError(
-                "You cannot set the same property twice in a parameter description block", value.pos
-            )
+            raise generic.ScriptError("You cannot set the same property twice in a parameter description block", value.pos)
         self.properties_set.add(name)
-        if name == "names":
+        if name == 'names':
             for name_value in value.values:
                 num = name_value.name.reduce_constant().value
                 desc = name_value.value
                 if not isinstance(desc, expression.String):
                     raise generic.ScriptError("setting name description must be a string", desc.pos)
                 self.val_names.append((num, desc))
             return
-        value = value.reduce(unknown_id_fatal=False)
-        if name == "type":
-            if not isinstance(value, expression.Identifier) or (value.value != "int" and value.value != "bool"):
+        value = value.reduce(unknown_id_fatal = False)
+        if name == 'type':
+            if not isinstance(value, expression.Identifier) or (value.value != 'int' and value.value != 'bool'):
                 raise generic.ScriptError("setting-type must be either 'int' or 'bool'", value.pos)
             self.type = value.value
-        elif name == "name":
+        elif name == 'name':
             if not isinstance(value, expression.String):
                 raise generic.ScriptError("setting-name must be a string", value.pos)
             self.name_string = value
-        elif name == "desc":
+        elif name == 'desc':
             if not isinstance(value, expression.String):
                 raise generic.ScriptError("setting-description must be a string", value.pos)
             self.desc_string = value
-        elif name == "bit":
-            if self.type != "bool":
+        elif name == 'bit':
+            if self.type != 'bool':
                 raise generic.ScriptError("setting-bit is only valid for 'bool' settings", value.pos)
             self.bit_num = value.reduce_constant()
-        elif name == "min_value":
-            if self.type != "int":
+        elif name == 'min_value':
+            if self.type != 'int':
                 raise generic.ScriptError("setting-min_value is only valid for 'int' settings", value.pos)
             self.min_val = value.reduce_constant()
-        elif name == "max_value":
-            if self.type != "int":
+        elif name == 'max_value':
+            if self.type != 'int':
                 raise generic.ScriptError("setting-max_value is only valid for 'int' settings", value.pos)
             self.max_val = value.reduce_constant()
-        elif name == "def_value":
+        elif name == 'def_value':
             self.def_val = value.reduce_constant()
-            if self.type == "bool" and self.def_val.value != 0 and self.def_val.value != 1:
+            if self.type == 'bool' and self.def_val.value != 0 and self.def_val.value != 1:
                 raise generic.ScriptError("setting-def_value must be either 0 or 1 for 'bool' settings", value.pos)
         else:
             raise generic.ScriptError("Unknown setting-property " + name, value.pos)
 
-
-class ParameterDescription:
-    def __init__(self, setting_list, num=None, pos=None):
+class ParameterDescription(object):
+    def __init__(self, setting_list, num = None, pos = None):
         self.setting_list = setting_list
         self.num = num
         self.pos = pos
 
     def __str__(self):
         ret = "\tparam"
         if self.num:
             ret += " " + str(self.num)
         ret += " {\n"
         for setting in self.setting_list:
             ret += str(setting)
         ret += "\t}\n"
         return ret
 
-    def debug_print(self, indentation):
-        if self.num is not None:
-            self.num.debug_print(indentation)
-        for setting in self.setting_list:
-            setting.debug_print(indentation + 2)
-
     def pre_process(self, num):
-        if self.num is None:
-            self.num = num
+        if self.num is None: self.num = num
         self.num = self.num.reduce_constant()
         for setting in self.setting_list:
             setting.pre_process()
         for setting in self.setting_list:
-            if setting.type == "int":
+            if setting.type == 'int':
                 if len(self.setting_list) > 1:
-                    raise generic.ScriptError(
-                        "When packing multiple settings in one parameter only bool settings are allowed", self.pos
-                    )
-                global_constants.settings[setting.name.value] = {"num": self.num.value, "size": 4}
+                    raise generic.ScriptError("When packing multiple settings in one parameter only bool settings are allowed", self.pos)
+                global_constants.settings[setting.name.value] = {'num': self.num.value, 'size': 4}
             else:
                 bit = 0 if setting.bit_num is None else setting.bit_num.value
-                global_constants.misc_grf_bits[setting.name.value] = {"param": self.num.value, "bit": bit}
+                global_constants.misc_grf_bits[setting.name.value] = {'param': self.num.value, 'bit': bit}
```

### Comparing `nml-0.7.2/nml/ast/spriteblock.py` & `nml-r1512/nml/ast/spriteblock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,280 +1,243 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import expression, generic, global_constants
-from nml.actions import action2, action2layout, action2real, real_sprite
-from nml.ast import base_statement, sprite_container
-
+from nml.actions import action1, action2, action2layout, action2real, real_sprite
+from nml.ast import base_statement
 
 class TemplateDeclaration(base_statement.BaseStatement):
     def __init__(self, name, param_list, sprite_list, pos):
         base_statement.BaseStatement.__init__(self, "template declaration", pos, False, False)
         self.name = name
         self.param_list = param_list
         self.sprite_list = sprite_list
-
+    
     def pre_process(self):
-        # check that all templates that are referred to exist at this point
-        # This prevents circular dependencies
+        #check that all templates that are referred to exist at this point
+        #This prevents circular dependencies
         for sprite in self.sprite_list:
             if isinstance(sprite, real_sprite.TemplateUsage):
                 if sprite.name.value == self.name.value:
-                    raise generic.ScriptError(
-                        "Sprite template '{}' includes itself.".format(sprite.name.value), self.pos
-                    )
+                    raise generic.ScriptError("Sprite template '%s' includes itself." % sprite.name.value, self.pos)
                 elif sprite.name.value not in real_sprite.sprite_template_map:
-                    raise generic.ScriptError(
-                        "Encountered unknown template identifier: " + sprite.name.value, sprite.pos
-                    )
-        # Register template
+                    raise generic.ScriptError("Encountered unknown template identifier: " + sprite.name.value, sprite.pos)
+        #Register template
         if self.name.value not in real_sprite.sprite_template_map:
             real_sprite.sprite_template_map[self.name.value] = self
         else:
-            raise generic.ScriptError(
-                "Template named '{}' is already defined, first definition at {}".format(
-                    self.name.value, real_sprite.sprite_template_map[self.name.value].pos
-                ),
-                self.pos,
-            )
+            raise generic.ScriptError("Template named '%s' is already defined, first definition at %s" % (self.name.value, real_sprite.sprite_template_map[self.name.value].pos), self.pos)
 
     def get_labels(self):
         labels = {}
         offset = 0
         for sprite in self.sprite_list:
             sprite_labels, num_sprites = sprite.get_labels()
-            for lbl, lbl_offset in sprite_labels.items():
+            for lbl, lbl_offset in sprite_labels.iteritems():
                 if lbl in labels:
-                    raise generic.ScriptError("Duplicate label encountered; '{}' already exists.".format(lbl), self.pos)
+                    raise generic.ScriptError("Duplicate label encountered; '%s' already exists." % lbl, self.pos)
                 labels[lbl] = lbl_offset + offset
             offset += num_sprites
         return labels, offset
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Template declaration:", self.name.value)
-        generic.print_dbg(indentation + 2, "Parameters:")
+        print indentation*' ' + 'Template declaration:', self.name.value
+        print (indentation+2)*' ' + 'Parameters:'
         for param in self.param_list:
             param.debug_print(indentation + 4)
-        generic.print_dbg(indentation + 2, "Sprites:")
+        print (indentation+2)*' ' + 'Sprites:'
         for sprite in self.sprite_list:
             sprite.debug_print(indentation + 4)
 
     def get_action_list(self):
         return []
 
     def __str__(self):
-        ret = "template {}({}) {{\n".format(str(self.name), ", ".join([str(param) for param in self.param_list]))
+        ret = "template %s(%s) {\n" % (str(self.name), ", ".join([str(param) for param in self.param_list]))
         for sprite in self.sprite_list:
-            ret += "\t{}\n".format(sprite)
+            ret += "\t%s\n" % str(sprite)
         ret += "}\n"
         return ret
 
+spriteset_base_class = action2.make_sprite_group_class(action2.SpriteGroupRefType.SPRITESET, action2.SpriteGroupRefType.NONE, action2.SpriteGroupRefType.SPRITEGROUP, False, True, cls_is_relocatable = True)
 
-spriteset_base_class = action2.make_sprite_group_class(True, True, False, cls_is_relocatable=True)
-
-
-class SpriteSet(spriteset_base_class, sprite_container.SpriteContainer):
+class SpriteSet(spriteset_base_class):
     def __init__(self, param_list, sprite_list, pos):
         base_statement.BaseStatement.__init__(self, "spriteset", pos, False, False)
         if not (1 <= len(param_list) <= 2):
             raise generic.ScriptError("Spriteset requires 1 or 2 parameters, encountered " + str(len(param_list)), pos)
         name = param_list[0]
         if not isinstance(name, expression.Identifier):
             raise generic.ScriptError("Spriteset parameter 1 'name' should be an identifier", name.pos)
-        sprite_container.SpriteContainer.__init__(self, "spriteset", name)
         self.initialize(name)
-
         if len(param_list) >= 2:
-            self.image_file = param_list[1].reduce()
-            if not isinstance(self.image_file, expression.StringLiteral):
-                raise generic.ScriptError(
-                    "Spriteset-block parameter 2 'file' must be a string literal", self.image_file.pos
-                )
+            self.pcx = param_list[1].reduce()
+            if not isinstance(self.pcx, expression.StringLiteral):
+                raise generic.ScriptError("Spriteset-block parameter 2 'file' must be a string literal", self.pcx.pos)
         else:
-            self.image_file = None
+            self.pcx = None
         self.sprite_list = sprite_list
-        self.action1_num = None  # set number in action1
-        self.labels = {}  # mapping of real sprite labels to offsets
-        self.add_sprite_data(self.sprite_list, self.image_file, pos)
+        self.action1_num = None #set number in action1
+        self.labels = {} #mapping of real sprite labels to offsets
 
     def pre_process(self):
         spriteset_base_class.pre_process(self)
         offset = 0
         for sprite in self.sprite_list:
             sprite_labels, num_sprites = sprite.get_labels()
-            for lbl, lbl_offset in sprite_labels.items():
+            for lbl, lbl_offset in sprite_labels.iteritems():
                 if lbl in self.labels:
-                    raise generic.ScriptError("Duplicate label encountered; '{}' already exists.".format(lbl), self.pos)
+                    raise generic.ScriptError("Duplicate label encountered; '%s' already exists." % lbl, self.pos)
                 self.labels[lbl] = lbl_offset + offset
             offset += num_sprites
 
     def collect_references(self):
         return []
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Sprite set:", self.name.value)
-        generic.print_dbg(
-            indentation + 2, "Source:  ", self.image_file.value if self.image_file is not None else "None"
-        )
-
-        generic.print_dbg(indentation + 2, "Sprites:")
+        print indentation*' ' + 'Sprite set:', self.name.value
+        print (indentation+2)*' ' + 'Source:  ', self.pcx.value if self.pcx is not None else 'None'
+        print (indentation+2)*' ' + 'Sprites:'
         for sprite in self.sprite_list:
             sprite.debug_print(indentation + 4)
 
     def get_action_list(self):
-        # Actions are created when parsing the action2s, not here
         return []
 
     def __str__(self):
-        filename = (", " + str(self.image_file)) if self.image_file is not None else ""
-        ret = "spriteset({}{}) {{\n".format(self.name, filename)
+        filename = (", " + str(self.pcx)) if self.pcx is not None else ""
+        ret = "spriteset(%s%s) {\n" % (self.name, filename)
         for sprite in self.sprite_list:
-            ret += "\t{}\n".format(str(sprite))
+            ret += "\t%s\n" % str(sprite)
         ret += "}\n"
         return ret
 
-
-spritegroup_base_class = action2.make_sprite_group_class(False, True, False)
-
+spritegroup_base_class = action2.make_sprite_group_class(action2.SpriteGroupRefType.SPRITEGROUP, action2.SpriteGroupRefType.SPRITESET, action2.SpriteGroupRefType.SPRITEGROUP, False)
 
 class SpriteGroup(spritegroup_base_class):
-    def __init__(self, name, spriteview_list, pos=None):
+    def __init__(self, name, spriteview_list, pos = None):
         base_statement.BaseStatement.__init__(self, "spritegroup", pos, False, False)
         self.initialize(name)
         self.spriteview_list = spriteview_list
+        self.parsed = False
 
+    # pre_process is defined by the base class
     def pre_process(self):
         for spriteview in self.spriteview_list:
             spriteview.pre_process()
         spritegroup_base_class.pre_process(self)
 
     def collect_references(self):
-        return []
+        all_sets = []
+        for spriteview in self.spriteview_list:
+            all_sets.extend(spriteview.spriteset_list)
+        return all_sets
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Sprite group:", self.name.value)
+        print indentation*' ' + 'Sprite group:', self.name.value
         for spriteview in self.spriteview_list:
             spriteview.debug_print(indentation + 2)
 
     def get_action_list(self):
-        action_list = []
-        if self.prepare_act2_output():
-            for feature in sorted(self.feature_set):
-                action_list.extend(action2real.get_real_action2s(self, feature))
-        return action_list
+        if not self.parsed:
+            if not self.prepare_output():
+                return []
+            self.parsed = True
+            return action2real.get_real_action2s(self)
+        return []
 
     def __str__(self):
-        ret = "spritegroup {} {{\n".format(self.name)
+        ret = "spritegroup %s {\n" % (self.name)
         for spriteview in self.spriteview_list:
-            ret += "\t{}\n".format(spriteview)
+            ret += "\t%s\n" % str(spriteview)
         ret += "}\n"
         return ret
 
-
-class SpriteView:
+class SpriteView(object):
     def __init__(self, name, spriteset_list, pos):
         self.name = name
         self.spriteset_list = spriteset_list
         self.pos = pos
 
     def pre_process(self):
         self.spriteset_list = [x.reduce(global_constants.const_list) for x in self.spriteset_list]
-        for sg_ref in self.spriteset_list:
-            if not (
-                isinstance(sg_ref, expression.SpriteGroupRef)
-                and action2.resolve_spritegroup(sg_ref.name).is_spriteset()
-            ):
-                raise generic.ScriptError("Expected a sprite set reference", sg_ref.pos)
-            if len(sg_ref.param_list) != 0:
-                raise generic.ScriptError(
-                    "Spritesets referenced from a spritegroup may not have parameters.", sg_ref.pos
-                )
+        if any(map(lambda x: not isinstance(x, expression.SpriteGroupRef), self.spriteset_list)):
+            raise generic.ScriptError("All items in a spritegroup must be spritegroup references", self.pos)
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Sprite view:", self.name.value)
-        generic.print_dbg(indentation + 2, "Sprite sets:")
+        print indentation*' ' + 'Sprite view:', self.name.value
+        print (indentation+2)*' ' + 'Sprite sets:'
         for spriteset in self.spriteset_list:
             spriteset.debug_print(indentation + 4)
 
     def __str__(self):
-        return "{}: [{}];".format(self.name, ", ".join([str(spriteset) for spriteset in self.spriteset_list]))
-
-
-spritelayout_base_class = action2.make_sprite_group_class(False, True, False)
+        return "%s: [%s];" % (str(self.name), ", ".join([str(spriteset) for spriteset in self.spriteset_list]))
 
+spritelayout_base_class = action2.make_sprite_group_class(action2.SpriteGroupRefType.SPRITEGROUP, action2.SpriteGroupRefType.SPRITESET, action2.SpriteGroupRefType.SPRITEGROUP, False, True)
 
 class SpriteLayout(spritelayout_base_class):
-    def __init__(self, name, param_list, layout_sprite_list, pos=None):
+    def __init__(self, name, param_list, layout_sprite_list, pos = None):
         base_statement.BaseStatement.__init__(self, "spritelayout", pos, False, False)
-        self.initialize(name, None, len(param_list))
+        self.initialize(name)
         self.param_list = param_list
-        self.register_map = {}  # Set during action generation for easier referencing
+        if len(param_list) != 0:
+            generic.print_warning("spritelayout parameters are not (yet) supported, ignoring.", pos)
         self.layout_sprite_list = layout_sprite_list
+        self.parsed = False
 
-    # Do not reduce expressions here as they may contain variables
-    # And the feature is not known yet
     def pre_process(self):
-        # Check parameter names
-        seen_names = set()
-        for param in self.param_list:
-            if not isinstance(param, expression.Identifier):
-                raise generic.ScriptError("spritelayout parameter names must be identifiers.", param.pos)
-            if param.value in seen_names:
-                raise generic.ScriptError("Duplicate parameter name '{}' encountered.".format(param.value), param.pos)
-            seen_names.add(param.value)
+        for layout_sprite in self.layout_sprite_list:
+            for param in layout_sprite.param_list:
+                try:
+                    param.value = param.value.reduce(global_constants.const_list)
+                except generic.ScriptError:
+                    pass
         spritelayout_base_class.pre_process(self)
 
     def collect_references(self):
-        return []
+        all_sets = []
+        for layout_sprite in self.layout_sprite_list:
+            all_sets.extend(layout_sprite.collect_spritesets())
+        return all_sets
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Sprite layout:", self.name.value)
-        generic.print_dbg(indentation + 2, "Parameters:")
+        print indentation*' ' + 'Sprite layout:', self.name.value
+        print (indentation+2)*' ' + 'Parameters:'
         for param in self.param_list:
             param.debug_print(indentation + 4)
-        generic.print_dbg(indentation + 2, "Sprites:")
+        print (indentation+2)*' ' + 'Sprites:'
         for layout_sprite in self.layout_sprite_list:
             layout_sprite.debug_print(indentation + 4)
 
     def __str__(self):
-        params = "" if not self.param_list else "({})".format(", ".join(str(x) for x in self.param_list))
-        return "spritelayout {}{} {{\n{}\n}}\n".format(
-            str(self.name), params, "\n".join(str(x) for x in self.layout_sprite_list)
-        )
+        return 'spritelayout %s {\n%s\n}\n' % (str(self.name), '\n'.join([str(x) for x in self.layout_sprite_list]))
 
     def get_action_list(self):
-        action_list = []
-        if self.prepare_act2_output():
-            for feature in sorted(self.feature_set):
-                if feature == 0x04:
-                    continue
-                action_list.extend(action2layout.get_layout_action2s(self, feature))
-        return action_list
-
+        if not self.parsed:
+            if not self.prepare_output():
+                return []
+            self.parsed = True
+            return action2layout.get_layout_action2s(self)
+        return []
 
-class LayoutSprite:
+class LayoutSprite(object):
     def __init__(self, ls_type, param_list, pos):
         self.type = ls_type
         self.param_list = param_list
         self.pos = pos
 
+    # called by SpriteLayout
+    def collect_spritesets(self):
+        used_sets = []
+        for layout_param in self.param_list:
+            try:
+                layout_param.value = layout_param.value.reduce(global_constants.const_list)
+            except generic.ScriptError:
+                pass
+            if isinstance(layout_param.value, expression.SpriteGroupRef):
+                used_sets.append(layout_param.value)
+        return used_sets
+
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Tile layout sprite of type:", self.type)
+        print indentation*' ' + 'Tile layout sprite of type:', self.type
         for layout_param in self.param_list:
             layout_param.debug_print(indentation + 2)
 
     def __str__(self):
-        return "\t{} {{\n\t\t{}\n\t}}".format(
-            self.type, "\n\t\t".join(str(layout_param) for layout_param in self.param_list)
-        )
+        return '\t%s {\n\t\t%s\n\t}' % (self.type, '\n\t\t'.join([str(layout_param) for layout_param in self.param_list]))
```

### Comparing `nml-0.7.2/nml/ast/townnames.py` & `nml-r1512/nml/ast/townnames.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 import heapq
-
 from nml import expression, generic, grfstrings
 from nml.actions import actionF
 from nml.ast import base_statement
 
 townname_serial = 1
 
-
 class TownNames(base_statement.BaseStatement):
     """
     'town_names' ast node.
 
     @ivar name: Name ID of the town_name.
     @type name: C{None}, L{Identifier}, or L{ConstantNumeric}
 
@@ -40,43 +23,50 @@
 
     @ivar parts: Parts of the names.
     @type parts: C{list} of L{TownNamesPart}
 
     @ivar param_list: Stored parameter list.
     @type param_list: C{list} of (L{TownNamesPart} or L{TownNamesParam})
     """
-
     def __init__(self, name, param_list, pos):
         base_statement.BaseStatement.__init__(self, "town_names-block", pos, False, False)
         self.name = name
         self.param_list = param_list
 
         self.id_number = None
         self.style_name = None
         self.actFs = []
         self.parts = []
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Town name")
-        if self.name is not None:
-            generic.print_dbg(indentation + 2, "Name:")
-            self.name.debug_print(indentation + 4)
-        for param in self.param_list:
-            param.debug_print(indentation + 2)
+        if isinstance(self.name, basestring):
+            name_text = "name = " + repr(self.name)
+            if self.id_number is not None: name_text += " (allocated number is 0x%x)" % self.id_number
+        elif self.id_number is not None:
+            name_text = "number = 0x%x" % self.id_number
+        else:
+            name_text = "(unnamed)"
+
+        print indentation*' ' + 'Town name ' + name_text
+        if self.style_name is not None:
+            print indentation*' ' + "  style name string:", self.style_name
+        for part in self.parts:
+            print indentation*' ' + "-name part:"
+            part.debug_print(indentation + 2)
 
     def pre_process(self):
         self.actFs = []
         self.parts = []
         for param in self.param_list:
             if isinstance(param, TownNamesPart):
                 actFs, part = param.make_actions()
                 self.actFs.extend(actFs)
                 self.parts.append(part)
             else:
-                if param.key.value != "styles":
+                if param.key.value != 'styles':
                     raise generic.ScriptError("Expected 'styles' keyword.", param.pos)
                 if len(param.value.params) > 0:
                     raise generic.ScriptError("Parameters of the 'styles' were not expected.", param.pos)
                 if self.style_name is not None:
                     raise generic.ScriptError("'styles' is already defined.", self.pos)
                 self.style_name = param.value
 
@@ -87,33 +77,33 @@
         # Allocate it now, before the self.prepare_output() call (to prevent names to grab it).
         if self.name is not None and not isinstance(self.name, expression.Identifier):
             value = self.name.reduce_constant()
             if not isinstance(value, expression.ConstantNumeric):
                 raise generic.ScriptError("ID should be an integer number.", self.pos)
 
             self.id_number = value.value
-            if self.id_number < 0 or self.id_number > 0x7F:
+            if self.id_number < 0 or self.id_number > 0x7f:
                 raise generic.ScriptError("ID must be a number between 0 and 0x7f (inclusive)", self.pos)
 
             if self.id_number not in actionF.free_numbers:
-                raise generic.ScriptError("town names ID 0x{:x} is already used.".format(self.id_number), self.pos)
+                raise generic.ScriptError("town names ID 0x%x is already used." % self.id_number, self.pos)
             actionF.free_numbers.remove(self.id_number)
 
     def __str__(self):
-        ret = "town_names"
+        ret = 'town_names'
         if self.name is not None:
-            ret += "({})".format(self.name)
-        ret += "{{\n{}}}\n".format("".join(str(x) for x in self.param_list))
+            ret += '(%s)' % str(self.name)
+        ret += '{\n%s}\n' % ''.join(str(x) for x in self.param_list)
         return ret
 
     def get_action_list(self):
         return self.actFs + [actionF.ActionF(self.name, self.id_number, self.style_name, self.parts, self.pos)]
 
 
-class TownNamesPart:
+class TownNamesPart(object):
     """
     A class containing a town name part.
 
     @ivar pieces: Pieces of the town name part.
     @type pieces: C{list} of (L{TownNamesEntryDefinition} or L{TownNamesEntryText})
 
     @ivar pos: Position information of the parts block.
@@ -121,15 +111,14 @@
 
     @ivar startbit: First bit to use for this part, if defined.
     @type startbit: C{int} or C{None}
 
     @ivar num_bits: Number of bits to use, if defined.
     @type num_bits: C{int} or C{None}
     """
-
     def __init__(self, pieces, pos):
         self.pos = pos
         self.pieces = pieces
 
         self.startbit = None
         self.num_bits = None
 
@@ -140,29 +129,25 @@
         @return: Action F that should be defined before, and the processed part.
         @rtype: C{list} of L{ActionF}, L{TownNamesPart}
         """
         new_pieces = []
         for piece in self.pieces:
             piece.pre_process()
             if piece.probability.value == 0:
-                generic.print_warning(
-                    generic.Warning.OPTIMISATION, "Dropping town name piece with 0 probability.", piece.pos
-                )
+                generic.print_warning("Dropping town name piece with 0 probability.", piece.pos)
             else:
                 new_pieces.append(piece)
 
         self.pieces = new_pieces
 
         actFs = self.move_pieces()
         if len(self.pieces) == 0:
             raise generic.ScriptError("Expected names and/or town_name references in the part.", self.pos)
         if len(self.pieces) > 255:
-            raise generic.ScriptError(
-                "Too many values in a part, found {:d}, maximum is 255".format(len(self.pieces)), self.pos
-            )
+            raise generic.ScriptError("Too many values in a part, found %d, maximum is 255" % len(self.pieces), self.pos)
 
         return actFs, self
 
     def move_pieces(self):
         """
         Move pieces to new action F instances to make it fit, if needed.
 
@@ -170,59 +155,48 @@
         @rtype:  C{list} of L{ActionF}
 
         @note: Function may change L{pieces}.
         """
         global townname_serial
 
         if len(self.pieces) <= 255:
-            return []  # Trivially correct.
+            return [] # Trivially correct.
 
         # There are too many pieces.
-        number_action_f = (len(self.pieces) + 254) // 255
+        nactf = (len(self.pieces) + 254) // 255
         pow2 = 1
-        while pow2 < number_action_f:
-            pow2 = pow2 * 2
-        if pow2 < 255:
-            number_action_f = pow2
+        while pow2 < nactf: pow2 = pow2 * 2
+        if pow2 < 255: nactf = pow2
 
-        heap = []  # Heap of (summed probability, subset-of-pieces)
+        heap = [] # Heap of (summed probability, subset-of-pieces)
         i = 0
-        while i < number_action_f:
+        while i < nactf:
             # Index 'i' is added to have a unique sorting when lists have equal total probabilities.
             heapq.heappush(heap, (0, i, []))
             i = i + 1
 
-        finished_actions = []
         # Index 'idx' is added to have a unique sorting when pieces have equal probabilities.
-        rev_pieces = sorted(((p.probability.value, idx, p) for idx, p in enumerate(self.pieces)), reverse=True)
+        rev_pieces = sorted(((p.probability.value, idx, p) for idx, p in enumerate(self.pieces)), reverse = True)
         for prob, _idx, piece in rev_pieces:
-            while True:
-                sub = heapq.heappop(heap)
-                if len(sub[2]) < 255:
-                    break
-                # If a subset already has the max number of parts, consider it finished.
-                finished_actions.append(sub)
-
+            sub = heapq.heappop(heap)
             sub[2].append(piece)
             sub = (sub[0] + prob, sub[1], sub[2])
             heapq.heappush(heap, sub)
 
-        finished_actions.extend(heap)
-
         # To ensure the chances do not get messed up due to one part needing less bits for its
         # selection, all parts are forced to use the same number of bits.
-        max_prob = max(sub[0] for sub in finished_actions)
+        max_prob = max(sub[0] for sub in heap)
         num_bits = 1
         while (1 << num_bits) < max_prob:
             num_bits = num_bits + 1
 
         # Assign to action F
         actFs = []
-        for _prob, _idx, sub in finished_actions:
-            actF_name = expression.Identifier("**townname #{:d}**".format(townname_serial), None)
+        for _prob, _idx, sub in heap:
+            actF_name = expression.Identifier("**townname #%d**" % townname_serial, None)
             townname_serial = townname_serial + 1
             town_part = TownNamesPart(sub, self.pos)
             town_part.set_numbits(num_bits)
             actF = actionF.ActionF(actF_name, None, None, [town_part], self.pos)
             actFs.append(actF)
 
             # Remove pieces of 'sub' from self.pieces
@@ -232,104 +206,95 @@
             assert len(self.pieces) == counts[0] - counts[1]
 
             self.pieces.append(TownNamesEntryDefinition(actF_name, expression.ConstantNumeric(1), self.pos))
 
         # update self.parts
         return actFs
 
+
+
     def assign_bits(self, startbit):
         """
         Assign bits for this piece.
 
         @param startbit: First bit free for use.
         @type  startbit: C{int}
 
         @return: Number of bits needed for this piece.
         @rtype:  C{int}
         """
         assert len(self.pieces) <= 255
         total = sum(piece.probability.value for piece in self.pieces)
 
-        if self.startbit is None or self.startbit < startbit:
-            self.startbit = startbit
+        self.startbit = startbit
         if self.num_bits is None:
             n = 1
-            while total > (1 << n):
-                n = n + 1
+            while total > (1 << n): n = n + 1
             self.num_bits = n
         assert (1 << self.num_bits) >= total
         return self.num_bits
 
     def set_numbits(self, numbits):
         """
         Set the number of bits that this part should use.
         """
         assert self.num_bits is None
         self.num_bits = numbits
 
     def debug_print(self, indentation):
         total = sum(piece.probability.value for piece in self.pieces)
-        generic.print_dbg(indentation, "Town names part (total {:d})".format(total))
+        print indentation*' ' + 'Town names part (total %d)' % total
         for piece in self.pieces:
             piece.debug_print(indentation + 2, total)
 
     def __str__(self):
-        return "{{\n\t{}\n}}\n".format("\n\t".join(str(piece) for piece in self.pieces))
+        return '{\n\t%s\n}\n' % '\n\t'.join([str(piece) for piece in self.pieces])
 
     def get_length(self):
-        size = 3  # textcount, firstbit, bitcount bytes.
+        size = 3 # textcount, firstbit, bitcount bytes.
         size += sum(piece.get_length() for piece in self.pieces)
         return size
 
     def resolve_townname_id(self):
-        """
+        '''
         Resolve the reference numbers to previous C{town_names} blocks.
 
         @return: Set of referenced C{town_names} block numbers.
-        """
+        '''
         blocks = set()
         for piece in self.pieces:
             block = piece.resolve_townname_id()
-            if block is not None:
-                blocks.add(block)
+            if block is not None: blocks.add(block)
         return blocks
 
     def write(self, file):
         file.print_bytex(len(self.pieces))
         file.print_bytex(self.startbit)
         file.print_bytex(self.num_bits)
         for piece in self.pieces:
             piece.write(file)
             file.newline()
 
 
-class TownNamesParam:
+class TownNamesParam(object):
     """
     Class containing a parameter of a town name.
     Currently known key/values:
      - 'styles'  / string expression
     """
-
     def __init__(self, key, value, pos):
         self.key = key
         self.value = value
         self.pos = pos
 
-    def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Town names param")
-        generic.print_dbg(indentation + 2, "Key:")
-        self.key.debug_print(indentation + 4)
-        generic.print_dbg(indentation + 2, "Value:")
-        self.value.debug_print(indentation + 4)
-
     def __str__(self):
-        return "{}: {};\n".format(self.key, self.value)
+        return '%s: %s;\n' % (self.key, self.value)
 
 
-class TownNamesEntryDefinition:
+class TownNamesEntryDefinition(object):
     """
     An entry in a part referring to a non-final town name, with a given probability.
 
     @ivar def_number: Name or number referring to a previous town_names node.
     @type def_number: L{Identifier} or L{ConstantNumeric}
 
     @ivar number: Actual ID to use.
@@ -337,126 +302,105 @@
 
     @ivar probability: Probability of picking this reference.
     @type probability: C{ConstantNumeric}
 
     @ivar pos: Position information of the parts block.
     @type pos: L{Position}
     """
-
     def __init__(self, def_number, probability, pos):
         self.def_number = def_number
         self.number = None
         self.probability = probability
         self.pos = pos
 
     def pre_process(self):
         self.number = None
         if not isinstance(self.def_number, expression.Identifier):
             self.def_number = self.def_number.reduce_constant()
             if not isinstance(self.def_number, expression.ConstantNumeric):
                 raise generic.ScriptError("Reference to other town name ID should be an integer number.", self.pos)
-            if self.def_number.value < 0 or self.def_number.value > 0x7F:
-                raise generic.ScriptError(
-                    "Reference number out of range (must be between 0 and 0x7f inclusive).", self.pos
-                )
+            if self.def_number.value < 0 or self.def_number.value > 0x7f:
+                raise generic.ScriptError("Reference number out of range (must be between 0 and 0x7f inclusive).", self.pos)
 
         self.probability = self.probability.reduce_constant()
         if not isinstance(self.probability, expression.ConstantNumeric):
             raise generic.ScriptError("Probability should be an integer number.", self.pos)
-        if self.probability.value < 0 or self.probability.value > 0x7F:
+        if self.probability.value < 0 or self.probability.value > 0x7f:
             raise generic.ScriptError("Probability out of range (must be between 0 and 0x7f inclusive).", self.pos)
 
     def debug_print(self, indentation, total):
-        if isinstance(self.def_number, expression.Identifier):
-            name_text = "name '" + self.def_number.value + "'"
-        else:
-            name_text = "number 0x{:x}".format(self.def_number.value)
-
-        generic.print_dbg(
-            indentation,
-            "Insert town_name ID {} with probability {:d}/{:d}".format(name_text, self.probability.value, total),
-        )
+        if isinstance(self.def_number, expression.Identifier): name_text = "name '" + self.def_number.value + "'"
+        else: name_text = "number 0x%x" % self.def_number.value
+        print indentation*' ' + ('Insert town_name ID %s with probability %d/%d' % (name_text, self.probability.value, total))
 
     def __str__(self):
-        return "town_names({}, {:d}),".format(str(self.def_number), self.probability.value)
+        return 'town_names(%s, %d),' % (str(self.def_number), self.probability.value)
 
     def get_length(self):
         return 2
 
     def resolve_townname_id(self):
-        """
+        '''
         Resolve the reference number to a previous C{town_names} block.
 
         @return: Number of the referenced C{town_names} block.
-        """
+        '''
         if isinstance(self.def_number, expression.Identifier):
             self.number = actionF.named_numbers.get(self.def_number.value)
             if self.number is None:
-                raise generic.ScriptError(
-                    'Town names name "{}" is not defined or points to a next town_names node'.format(
-                        self.def_number.value
-                    ),
-                    self.pos,
-                )
+                raise generic.ScriptError('Town names name "%s" is not defined or points to a next town_names node' % self.def_number.value, self.pos)
         else:
             self.number = self.def_number.value
             if self.number not in actionF.numbered_numbers:
-                raise generic.ScriptError(
-                    'Town names number "{}" is not defined or points to a next town_names node'.format(self.number),
-                    self.pos,
-                )
+                raise generic.ScriptError('Town names number "%s" is not defined or points to a next town_names node' % self.number, self.pos)
         return self.number
 
     def write(self, file):
         file.print_bytex(self.probability.value | 0x80)
         file.print_bytex(self.number)
 
-
-class TownNamesEntryText:
+class TownNamesEntryText(object):
     """
     An entry in a part, a text-string with a given probability.
 
     @ivar pos: Position information of the parts block.
     @type pos: L{Position}
     """
-
     def __init__(self, id, text, probability, pos):
         self.id = id
         self.text = text
         self.probability = probability
         self.pos = pos
 
     def pre_process(self):
-        if self.id.value != "text":
+        if self.id.value != 'text':
             raise generic.ScriptError("Expected 'text' prefix.", self.pos)
 
         if not isinstance(self.text, expression.StringLiteral):
             raise generic.ScriptError("Expected string literal for the name.", self.pos)
 
         self.probability = self.probability.reduce_constant()
         if not isinstance(self.probability, expression.ConstantNumeric):
             raise generic.ScriptError("Probability should be an integer number.", self.pos)
-        if self.probability.value < 0 or self.probability.value > 0x7F:
+        if self.probability.value < 0 or self.probability.value > 0x7f:
             raise generic.ScriptError("Probability out of range (must be between 0 and 0x7f inclusive).", self.pos)
 
     def debug_print(self, indentation, total):
-        generic.print_dbg(
-            indentation, "Text {} with probability {:d}/{:d}".format(self.text.value, self.probability.value, total)
-        )
+        print indentation*' ' + ('Text %s with probability %d/%d' % (self.text.value, self.probability.value, total))
 
     def __str__(self):
-        return "text({}, {:d}),".format(self.text, self.probability.value)
+        return 'text(%s, %d),' % (str(self.text), self.probability.value)
 
     def get_length(self):
-        return 1 + grfstrings.get_string_size(self.text.value)  # probability, text
+        return 1 + grfstrings.get_string_size(self.text.value) # probability, text
 
     def resolve_townname_id(self):
-        """
+        '''
         Resolve the reference number to a previous C{town_names} block.
 
         @return: C{None}, as being the block number of a referenced previous C{town_names} block.
-        """
+        '''
         return None
 
     def write(self, file):
         file.print_bytex(self.probability.value)
-        file.print_string(self.text.value, final_zero=True)
+        file.print_string(self.text.value, final_zero = True)
```

### Comparing `nml-0.7.2/nml/expression/abs_op.py` & `nml-r1512/nml/ast/switch_range.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
+from nml import expression, global_constants, generic
+from nml.actions import action2
 
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic
-
-from .base_expression import ConstantNumeric, Expression, Type
-
-
-class AbsOp(Expression):
-    def __init__(self, expr, pos):
-        Expression.__init__(self, pos)
-        self.expr = expr
+class SwitchRange(object):
+    def __init__(self, min, max, result, unit = None, comment = None):
+        self.min = min
+        self.max = max
+        self.result = result
+        self.unit = unit
+        self.comment = comment
+
+    def pre_process(self):
+        self.min = self.min.reduce(global_constants.const_list)
+        self.max = self.max.reduce(global_constants.const_list)
+        # Result may be None here, not pre-processed yet
+        if self.result is not None:
+            try:
+                self.result = self.result.reduce(global_constants.const_list)
+            except generic.ScriptError:
+                # We want to reduce the result here as much as possible however there
+                # are valid expressions that will still fail here. Ignore the error for
+                # now, if it was a real error it'll be raised again later.
+                pass
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "abs():")
-        self.expr.debug_print(indentation + 2)
-
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
-        expr = self.expr.reduce(id_dicts)
-        if expr.type() != Type.INTEGER:
-            if expr.type() == Type.SPRITEGROUP_REF:
-                raise generic.ProcCallSyntaxError(expr.name, expr.pos)
-            raise generic.ScriptError("abs() requires an integer argument.", expr.pos)
-        if isinstance(expr, ConstantNumeric):
-            if expr.value < 0:
-                return ConstantNumeric(-expr.value)
-            else:
-                return ConstantNumeric(expr.value)
-        return AbsOp(expr, self.pos)
-
-    def supported_by_action2(self, raise_error):
-        return self.expr.supported_by_action2(raise_error)
-
-    def supported_by_actionD(self, raise_error):
-        return self.expr.supported_by_actionD(raise_error)
-
-    def collect_references(self):
-        return self.expr.collect_references()
-
-    def is_read_only(self):
-        return self.expr.is_read_only()
+        print indentation*' ' + 'Min:'
+        self.min.debug_print(indentation + 2)
+        print indentation*' ' + 'Max:'
+        self.max.debug_print(indentation + 2)
+        print indentation*' ' + 'Result:'
+        self.result.debug_print(indentation + 2)
 
     def __str__(self):
-        return "abs(" + str(self.expr) + ")"
+        ret = str(self.min)
+        if not isinstance(self.min, expression.ConstantNumeric) or not isinstance(self.max, expression.ConstantNumeric) or self.max.value != self.min.value:
+            ret += '..' + str(self.max)
+        if self.result is None:
+            ret += ': return;'
+        elif isinstance(self.result, expression.SpriteGroupRef):
+            ret += ': %s;' % str(self.result)
+        else:
+            ret += ': return %s;' % str(self.result)
+        return ret
```

### Comparing `nml-0.7.2/nml/expression/base_expression.py` & `nml-r1512/nml/expression/base_expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,60 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic
 
-
-class Type:
+class Type(object):
     """
     Enum-type class of the various value types possible in NML
     """
-
     INTEGER = 0
     FLOAT = 1
     STRING_LITERAL = 2
     FUNCTION_PTR = 3
     SPRITEGROUP_REF = 4
 
-
-class Expression:
+class Expression(object):
     """
     Superclass for all expression classes.
 
     @ivar pos: Position of the data in the original file.
     @type pos: :L{Position}
     """
-
     def __init__(self, pos):
         self.pos = pos
 
     def debug_print(self, indentation):
         """
         Print all data with explanation of what it is to standard output.
 
         @param indentation: Indent all printed lines with at least
             C{indentation} spaces.
         """
-        raise NotImplementedError("debug_print must be implemented in expression-subclass {!r}".format(type(self)))
+        raise NotImplementedError('debug_print must be implemented in expression-subclass %r' % type(self))
 
     def __str__(self):
         """
         Convert this expression to a string representing this expression in valid NML-code.
 
         @return: A string representation of this expression.
         """
-        raise NotImplementedError("__str__ must be implemented in expression-subclass {!r}".format(type(self)))
+        raise NotImplementedError('__str__ must be implemented in expression-subclass %r' % type(self))
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         """
         Reduce this expression to the simplest representation possible.
 
         @param id_dicts: A list with dicts that are used to map identifiers
             to another (often numeric) representation.
         @param unknown_id_fatal: Is encountering an unknown identifier somewhere
             in this expression a fatal error?
 
         @return: A deep copy of this expression simplified as much as possible.
         """
-        raise NotImplementedError("reduce must be implemented in expression-subclass {!r}".format(type(self)))
+        raise NotImplementedError('reduce must be implemented in expression-subclass %r' % type(self))
 
-    def reduce_constant(self, id_dicts=None):
+    def reduce_constant(self, id_dicts = []):
         """
         Reduce this expression and make sure the result is a constant number.
 
         @param id_dicts: A list with dicts that are used to map identifiers
             to another (often numeric) representation.
 
         @return: A constant number that is the result of this expression.
@@ -87,82 +68,59 @@
         """
         Check if this expression can be used inside a switch-block.
 
         @param raise_error: If true raise a scripterror instead of returning false.
 
         @return: True if this expression can be calculated by advanced varaction2.
         """
-        if raise_error:
-            raise generic.ScriptError("This expression is not supported in a switch-block", self.pos)
+        if raise_error: raise generic.ScriptError("This expression is not supported in a switch-block", self.pos)
         return False
 
     def supported_by_actionD(self, raise_error):
         """
         Check if this expression can be used inside a parameter-assignment.
 
         @param raise_error: If true raise a scripterror instead of returning false.
 
         @return: True if this expression can be calculated by actionD.
         """
-        if raise_error:
-            raise generic.ScriptError("This expression can not be assigned to a parameter", self.pos)
+        if raise_error: raise generic.ScriptError("This expression can not be assigned to a parameter", self.pos)
         return False
 
-    def collect_references(self):
-        """
-        This function should collect all references to other nodes from this instance.
-
-        @return: A collection containing all links to other nodes.
-        @rtype: C{iterable} of L{SpriteGroupRef}
-        """
-        return []
-
-    def is_read_only(self):
-        """
-        Check if this expression store values.
-
-        @return: True if the expression doesn't store values.
-        """
-        return True
-
     def is_boolean(self):
         """
         Check if this expression is limited to 0 or 1 as value.
 
         @return: True if the value of this expression is either 0 or 1.
         """
         return False
-
+    
     def type(self):
         """
         Determine the datatype of this expression.
 
         @return: A constant from the L{Type} class, representing the data type.
         """
         return Type.INTEGER
 
-
 class ConstantNumeric(Expression):
-    def __init__(self, value, pos=None):
+    def __init__(self, value, pos = None):
         Expression.__init__(self, pos)
         self.value = generic.truncate_int32(value)
-        self.uvalue = self.value
-        if self.uvalue < 0:
-            self.uvalue += 2**32
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Int:", self.value)
+        print indentation*' ' + 'Int:', self.value
 
     def write(self, file, size):
         file.print_varx(self.value, size)
 
     def __str__(self):
         return str(self.value)
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         return self
 
     def supported_by_action2(self, raise_error):
         return True
 
     def supported_by_actionD(self, raise_error):
         return True
@@ -172,24 +130,23 @@
 
     def __eq__(self, other):
         return other is not None and isinstance(other, ConstantNumeric) and other.value == self.value
 
     def __hash__(self):
         return self.value
 
-
 class ConstantFloat(Expression):
     def __init__(self, value, pos):
         Expression.__init__(self, pos)
         self.value = float(value)
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Float:", self.value)
+        print indentation*' ' + 'Float:', self.value
 
     def __str__(self):
         return str(self.value)
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         return self
-
+    
     def type(self):
         return Type.FLOAT
```

### Comparing `nml-0.7.2/nml/expression/binop.py` & `nml-r1512/nml/expression/binop.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,27 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic, nmlop
-
-from .base_expression import ConstantFloat, ConstantNumeric, Expression
-from .boolean import Boolean
+from .base_expression import Expression, ConstantNumeric, ConstantFloat
 from .string_literal import StringLiteral
 from .variable import Variable
 
-
 class BinOp(Expression):
-    def __init__(self, op, expr1, expr2, pos=None):
-        self.op = op
-        self.expr1 = expr1 if isinstance(expr1, Expression) else ConstantNumeric(expr1)
-        self.expr2 = expr2 if isinstance(expr2, Expression) else ConstantNumeric(expr2)
-        pos = pos or self.expr1.pos or self.expr2.pos
-        self.expr1.pos = self.expr1.pos or pos
-        self.expr2.pos = self.expr2.pos or pos
+    def __init__(self, op, expr1, expr2, pos = None):
         Expression.__init__(self, pos)
+        self.op = op
+        self.expr1 = expr1
+        self.expr2 = expr2
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Binary operator, op =", self.op.token)
+        print indentation*' ' + 'Binary operator, op = ', self.op.token
         self.expr1.debug_print(indentation + 2)
         self.expr2.debug_print(indentation + 2)
 
     def __str__(self):
         if self.op == nmlop.SUB and isinstance(self.expr1, ConstantNumeric) and self.expr1.value == 0:
-            return "-" + str(self.expr2)
+            return '-' + str(self.expr2)
         return self.op.to_string(self.expr1, self.expr2)
 
     def get_priority(self, expr):
         """
         Get the priority of an expression. For optimalization reason we prefer complexer
         expressions (= low priority) on the left hand side of this expression. The following
         priorities are used:
@@ -53,23 +32,20 @@
 
         @param expr: The expression to get the priority of.
         @type  expr: L{Expression}
 
         @return: The priority for the given expression.
         @rtype: C{int}
         """
-        if isinstance(expr, Variable):
-            return 0
-        if isinstance(expr, ConstantNumeric):
-            return 2
-        if expr.supported_by_actionD(False):
-            return 1
+        if isinstance(expr, Variable): return 0
+        if isinstance(expr, ConstantNumeric): return 2
+        if expr.supported_by_actionD(False): return 1
         return -1
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         # Reducing a BinOp expression is done in several phases:
         # - Reduce both subexpressions.
         # - If both subexpressions are constant, compute the result and return it.
         # - If the operator allows it and the second expression is more complex than
         #   the first one swap them.
         # - If the operation is a no-op, delete it.
         # - Variables (as used in action2var) can have some computations attached to
@@ -81,36 +57,28 @@
         expr2 = self.expr2.reduce(id_dicts)
 
         # Make sure the combination of operands / operator is valid
         if self.op.validate_func is not None:
             self.op.validate_func(expr1, expr2, self.pos)
 
         # - If both subexpressions are constant, compute the result and return it.
-        if (
-            isinstance(expr1, ConstantNumeric)
-            and isinstance(expr2, ConstantNumeric)
-            and self.op.compiletime_func is not None
-        ):
+        if isinstance(expr1, ConstantNumeric) and isinstance(expr2, ConstantNumeric) and self.op.compiletime_func is not None:
             return ConstantNumeric(self.op.compiletime_func(expr1.value, expr2.value), self.pos)
 
         if isinstance(expr1, StringLiteral) and isinstance(expr2, StringLiteral):
             assert self.op == nmlop.ADD
             return StringLiteral(expr1.value + expr2.value, expr1.pos)
 
-        if (
-            isinstance(expr1, (ConstantNumeric, ConstantFloat))
-            and isinstance(expr2, (ConstantNumeric, ConstantFloat))
-            and self.op.compiletime_func is not None
-        ):
+        if isinstance(expr1, (ConstantNumeric, ConstantFloat)) and isinstance(expr2, (ConstantNumeric, ConstantFloat)) and self.op.compiletime_func is not None:
             return ConstantFloat(self.op.compiletime_func(expr1.value, expr2.value), self.pos)
 
         # - If the operator allows it and the second expression is more complex than
         #   the first one swap them.
         op = self.op
-        if op.commutative or op in (nmlop.CMP_LT, nmlop.CMP_GT):
+        if op in commutative_operators or self.op in (nmlop.CMP_LT, nmlop.CMP_GT):
             prio1 = self.get_priority(expr1)
             prio2 = self.get_priority(expr2)
             if prio2 < prio1:
                 expr1, expr2 = expr2, expr1
                 if op == nmlop.CMP_LT:
                     op = nmlop.CMP_GT
                 elif op == nmlop.CMP_GT:
@@ -119,154 +87,99 @@
         # - If the operation is a no-op, delete it.
         if op == nmlop.AND and isinstance(expr2, ConstantNumeric) and (expr2.value == -1 or expr2.value == 0xFFFFFFFF):
             return expr1
 
         if op in (nmlop.DIV, nmlop.DIVU, nmlop.MUL) and isinstance(expr2, ConstantNumeric) and expr2.value == 1:
             return expr1
 
-        if (
-            op
-            in (
-                nmlop.ADD,
-                nmlop.SUB,
-                nmlop.SHIFTU_LEFT,
-                nmlop.SHIFT_LEFT,
-                nmlop.SHIFTU_RIGHT,
-                nmlop.SHIFT_RIGHT,
-                nmlop.OR,
-                nmlop.XOR,
-                nmlop.ROT_RIGHT,
-            )
-            and isinstance(expr2, ConstantNumeric)
-            and expr2.value == 0
-        ):
+        if op in (nmlop.ADD, nmlop.SUB) and isinstance(expr2, ConstantNumeric) and expr2.value == 0:
             return expr1
 
         # - Variables (as used in action2var) can have some computations attached to
         #   them, do that if possible.
         if isinstance(expr1, Variable) and expr2.supported_by_actionD(False):
             # An action2 Variable has some special fields (mask, add, div and mod) that can be used
             # to perform some operations on the value. These operations are faster than a normal
             # advanced varaction2 operator so we try to use them whenever we can.
             if op == nmlop.AND and expr1.add is None:
-                expr1.mask = nmlop.AND(expr1.mask, expr2, self.pos).reduce(id_dicts)
+                expr1.mask = BinOp(nmlop.AND, expr1.mask, expr2, self.pos).reduce(id_dicts)
                 return expr1
             if op == nmlop.ADD and expr1.div is None and expr1.mod is None:
-                if expr1.add is None:
-                    expr1.add = expr2
-                else:
-                    expr1.add = nmlop.ADD(expr1.add, expr2, self.pos).reduce(id_dicts)
+                if expr1.add is None: expr1.add = expr2
+                else: expr1.add = BinOp(nmlop.ADD, expr1.add, expr2, self.pos).reduce(id_dicts)
                 return expr1
             if op == nmlop.SUB and expr1.div is None and expr1.mod is None:
-                if expr1.add is None:
-                    expr1.add = ConstantNumeric(0)
-                expr1.add = nmlop.SUB(expr1.add, expr2, self.pos).reduce(id_dicts)
+                if expr1.add is None: expr1.add = ConstantNumeric(0)
+                expr1.add = BinOp(nmlop.SUB, expr1.add, expr2, self.pos).reduce(id_dicts)
                 return expr1
             # The div and mod fields cannot be used at the same time. Also whenever either of those
             # two are used the add field has to be set, so we change it to zero when it's not yet set.
             if op == nmlop.DIV and expr1.div is None and expr1.mod is None:
-                if expr1.add is None:
-                    expr1.add = ConstantNumeric(0)
+                if expr1.add is None: expr1.add = ConstantNumeric(0)
                 expr1.div = expr2
                 return expr1
             if op == nmlop.MOD and expr1.div is None and expr1.mod is None:
-                if expr1.add is None:
-                    expr1.add = ConstantNumeric(0)
+                if expr1.add is None: expr1.add = ConstantNumeric(0)
                 expr1.mod = expr2
                 return expr1
             # Since we have a lot of nml-variables that are in fact only the high bits of an nfo
             # variable it can happen that we want to shift back the variable to the left.
             # Don't use any extra opcodes but just reduce the shift-right in that case.
-            if (
-                op == nmlop.SHIFT_LEFT
-                and isinstance(expr2, ConstantNumeric)
-                and expr1.add is None
-                and expr2.value < expr1.shift.value
-            ):
+            if op == nmlop.SHIFT_LEFT and isinstance(expr2, ConstantNumeric) and expr1.add is None and expr2.value < expr1.shift.value:
                 expr1.shift.value -= expr2.value
-                expr1.mask = nmlop.SHIFT_LEFT(expr1.mask, expr2).reduce()
-                return expr1
-
-            if (
-                (
-                    op == nmlop.SHIFTU_RIGHT
-                    or (
-                        op == nmlop.SHIFT_RIGHT
-                        and isinstance(expr1.mask, ConstantNumeric)
-                        and expr1.mask.uvalue < 0x80000000
-                    )
-                )
-                and isinstance(expr2, ConstantNumeric)
-                and expr2.value >= 0
-                and expr1.shift.value >= 0
-                and (expr1.shift.value + expr2.value) < 32
-            ):
-                expr1.shift.value += expr2.value
-                expr1.mask = nmlop.SHIFTU_RIGHT(expr1.mask, expr2).reduce()
+                expr1.mask = BinOp(nmlop.SHIFT_LEFT, expr1.mask, expr2).reduce()
                 return expr1
 
         # - Try to merge multiple additions/subtractions with constant numbers
-        if (
-            op in (nmlop.ADD, nmlop.SUB)
-            and isinstance(expr2, ConstantNumeric)
-            and isinstance(expr1, BinOp)
-            and expr1.op in (nmlop.ADD, nmlop.SUB)
-            and isinstance(expr1.expr2, ConstantNumeric)
-        ):
+        if op in (nmlop.ADD, nmlop.SUB) and isinstance(expr2, ConstantNumeric) and \
+                isinstance(expr1, BinOp) and expr1.op in (nmlop.ADD, nmlop.SUB) and isinstance(expr1.expr2, ConstantNumeric):
             val = expr2.value if op == nmlop.ADD else -expr2.value
             if expr1.op == nmlop.ADD:
-                return nmlop.ADD(expr1.expr1, (expr1.expr2.value + val), self.pos).reduce()
+                return BinOp(nmlop.ADD, expr1.expr1, ConstantNumeric(expr1.expr2.value + val), self.pos).reduce()
             if expr1.op == nmlop.SUB:
-                return nmlop.SUB(expr1.expr1, (expr1.expr2.value - val), self.pos).reduce()
-
-        if op == nmlop.OR and isinstance(expr1, Boolean) and isinstance(expr2, Boolean):
-            return Boolean(nmlop.OR(expr1.expr, expr2.expr, self.pos)).reduce(id_dicts)
+                return BinOp(nmlop.SUB, expr1.expr1, ConstantNumeric(expr1.expr2.value - val), self.pos).reduce()
 
         return BinOp(op, expr1, expr2, self.pos)
 
     def supported_by_action2(self, raise_error):
         if not self.op.act2_supports:
-            token = " '{}'".format(self.op.token) if self.op.token else ""
-            if raise_error:
-                raise generic.ScriptError("Operator{} not supported in a switch-block".format(token), self.pos)
+            token = " '%s'" % self.op.token if self.op.token else ""
+            if raise_error: raise generic.ScriptError("Operator%s not supported in a switch-block" % token, self.pos)
             return False
         return self.expr1.supported_by_action2(raise_error) and self.expr2.supported_by_action2(raise_error)
 
     def supported_by_actionD(self, raise_error):
         if not self.op.actd_supports:
+            token = " '%s'" % self.op.token if self.op.token else ""
             if raise_error:
-                if self.op == nmlop.STO_PERM:
-                    raise generic.ScriptError("STORE_PERM is only available in switch-blocks.", self.pos)
-                elif self.op == nmlop.STO_TMP:
-                    raise generic.ScriptError("STORE_TEMP is only available in switch-blocks.", self.pos)
-
-                # default case
-                token = " '{}'".format(self.op.token) if self.op.token else ""
-                raise generic.ScriptError("Operator{} not supported in parameter assignment".format(token), self.pos)
+                if self.op == nmlop.STO_PERM: raise generic.ScriptError("STORE_PERM is only available in switch-blocks.", self.pos)
+                elif self.op == nmlop.STO_TMP: raise generic.ScriptError("STORE_TEMP is only available in switch-blocks.", self.pos)
+                #default case
+                raise generic.ScriptError("Operator%s not supported in parameter assignment" % token, self.pos)
             return False
         return self.expr1.supported_by_actionD(raise_error) and self.expr2.supported_by_actionD(raise_error)
 
-    def collect_references(self):
-        return self.expr1.collect_references() + self.expr2.collect_references()
-
-    def is_read_only(self):
-        return self.expr1.is_read_only() and self.expr2.is_read_only()
-
     def is_boolean(self):
         if self.op in (nmlop.AND, nmlop.OR, nmlop.XOR):
             return self.expr1.is_boolean() and self.expr2.is_boolean()
         return self.op.returns_boolean
 
     def __eq__(self, other):
-        return (
-            other is not None
-            and isinstance(other, BinOp)
-            and self.op == other.op
-            and self.expr1 == other.expr1
-            and self.expr2 == other.expr2
-        )
+        return other is not None and isinstance(other, BinOp) and self.op == other.op and self.expr1 == other.expr1 and self.expr2 == other.expr2
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash((self.op, self.expr1, self.expr2))
+
+commutative_operators = set([
+    nmlop.ADD,
+    nmlop.MUL,
+    nmlop.AND,
+    nmlop.OR,
+    nmlop.XOR,
+    nmlop.CMP_EQ,
+    nmlop.CMP_NEQ,
+    nmlop.MIN,
+    nmlop.MAX,
+])
```

### Comparing `nml-0.7.2/nml/expression/functioncall.py` & `nml-r1512/nml/expression/functioncall.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,771 +1,451 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-import calendar
-import datetime
-import math
-from functools import reduce
-
-from nml import generic, global_constants, nmlop
-
-from . import identifier
-from .base_expression import ConstantFloat, ConstantNumeric, Expression, Type
+import datetime, calendar, math
+from nml.actions import action11
+from nml import generic, nmlop
+from .base_expression import Type, Expression, ConstantNumeric, ConstantFloat
+from .binop import BinOp
 from .bitmask import BitMask
-from .cargo import AcceptCargo, ProduceCargo
 from .parameter import parse_string_to_dword
 from .storage_op import StorageOp
 from .string_literal import StringLiteral
-from .abs_op import AbsOp
-
+from .ternaryop import TernaryOp
+import identifier
 
 class FunctionCall(Expression):
     def __init__(self, name, params, pos):
         Expression.__init__(self, pos)
         self.name = name
         self.params = params
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Call function: " + self.name.value)
+        print indentation*' ' + 'Call function: ' + self.name.value
         for param in self.params:
-            generic.print_dbg(indentation + 2, "Parameter:")
+            print (indentation+2)*' ' + 'Parameter:'
             param.debug_print(indentation + 4)
 
     def __str__(self):
-        ret = "{}({})".format(self.name, ", ".join(str(param) for param in self.params))
+        ret = ''
+        for param in self.params:
+            if ret == '': ret = str(param)
+            else: ret = '%s, %s' % (ret, str(param))
+        ret = '%s(%s)' % (self.name, ret)
         return ret
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
-        # At this point we don't care about invalid arguments, they'll be handled later.
-        identifier.ignore_all_invalid_ids = True
-        params = [param.reduce(id_dicts, unknown_id_fatal=False) for param in self.params]
-        identifier.ignore_all_invalid_ids = False
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         if self.name.value in function_table:
             func = function_table[self.name.value]
-            val = func(self.name.value, params, self.pos)
+            val = func(self.name.value, self.params, self.pos)
             return val.reduce(id_dicts)
         else:
-            # try user-defined functions
-            func_ptr = self.name.reduce(id_dicts, unknown_id_fatal=False, search_func_ptr=True)
-            if func_ptr != self.name:  # we found something!
+            #try user-defined functions
+            func_ptr = self.name.reduce(id_dicts, unknown_id_fatal = False, search_func_ptr = True)
+            if func_ptr != self.name: # we found something!
                 if func_ptr.type() == Type.SPRITEGROUP_REF:
-                    func_ptr.param_list = params
-                    func_ptr.is_procedure = True
+                    func_ptr.param_list = self.params
                     return func_ptr
                 if func_ptr.type() != Type.FUNCTION_PTR:
-                    raise generic.ScriptError(
-                        "'{}' is defined, but it is not a function.".format(self.name.value), self.pos
-                    )
-                return func_ptr.call(params)
+                    raise generic.ScriptError("'%s' is defined, but it is not a function." % self.name.value, self.pos)
+                return func_ptr.call(self.params)
             if unknown_id_fatal:
-                raise generic.ScriptError("'{}' is not defined as a function.".format(self.name.value), self.pos)
-            return FunctionCall(self.name, params, self.pos)
+                raise generic.ScriptError("'%s' is not defined as a function." % self.name.value, self.pos)
+            return FunctionCall(self.name, self.params, self.pos)
 
 
 class SpecialCheck(Expression):
     """
     Action7/9 special check (e.g. to see whether a cargo is defined)
 
     @ivar op: Action7/9 operator to use
-    @type op: (C{int}, C{str})-tuple
+    @type op: (C{int}, C{basestring})-tuple
 
     @ivar varnum: Variable number to read
     @type varnum: C{int}
 
     @ivar results: Result of the check when skipping (0) or not skipping (1)
     @type results: (C{int}, C{int})-tuple
 
     @ivar value: Value to test
     @type value: C{int}
 
-    @ivar varsize: Varsize for the action7/9 check
-    @type varsize: C{int}
-
     @ivar mask: Mask to to test only certain bits of the value
     @type mask: C{int}
 
     @ivar pos: Position information
     @type pos: L{Position}
     """
-
-    def __init__(self, op, varnum, results, value, to_string, varsize=4, mask=None, pos=None):
+    def __init__(self, op, varnum, results, value, to_string, mask = None, pos = None):
         Expression.__init__(self, pos)
         self.op = op
         self.varnum = varnum
         self.results = results
         self.value = value
         self.to_string = to_string
-        self.varsize = varsize
         self.mask = mask
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         return self
 
     def __str__(self):
         return self.to_string
 
     def supported_by_actionD(self, raise_error):
         return True
 
-
 class GRMOp(Expression):
-    def __init__(self, op, feature, count, to_string, pos=None):
+    def __init__(self, op, feature, count, to_string, pos = None):
         Expression.__init__(self, pos)
         self.op = op
         self.feature = feature
         self.count = count
         self.to_string = to_string
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         return self
 
     def __str__(self):
         return self.to_string(self)
 
     def supported_by_actionD(self, raise_error):
         return True
 
 
-function_table = {}
-
-
-def builtin(func):
-    """
-    Decorator that adds a function named `builtin_func` to the function table as `func`.
-    """
-    assert func.__name__.startswith("builtin_")
-    name = func.__name__[8:]  # Strip the "builtin_". str.removeprefix() is only added in py3.9.
-    function_table[name] = func
-    return func
-
-
-def builtins(*names):
-    """
-    Decorator that adds a function to the function table with one or more custom names.
-    """
-
-    def dec(func):
-        for name in names:
-            function_table[name] = func
-        return func
-
-    return dec
-
-
-# { Builtin functions
-
+#{ Builtin functions
 
-@builtin
 def builtin_min(name, args, pos):
     """
     min(...) builtin function.
 
     @return Lowest value of the given arguments.
     """
     if len(args) < 2:
         raise generic.ScriptError("min() requires at least 2 arguments", pos)
-    return reduce(lambda x, y: nmlop.MIN(x, y, pos), args)
+    return reduce(lambda x, y: BinOp(nmlop.MIN, x, y, pos), args)
 
-
-@builtin
 def builtin_max(name, args, pos):
     """
     max(...) builtin function.
 
     @return Heighest value of the given arguments.
     """
     if len(args) < 2:
         raise generic.ScriptError("max() requires at least 2 arguments", pos)
-    return reduce(lambda x, y: nmlop.MAX(x, y, pos), args)
-
+    return reduce(lambda x, y: BinOp(nmlop.MAX, x, y, pos), args)
 
-@builtin
 def builtin_date(name, args, pos):
     """
     date(year, month, day) builtin function.
 
     @return Days since 1 jan 1 of the given date.
     """
-    days_in_month = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
     if len(args) != 3:
         raise generic.ScriptError("date() requires exactly 3 arguments", pos)
+    from nml import global_constants
     identifier.ignore_all_invalid_ids = True
     year = args[0].reduce(global_constants.const_list)
     identifier.ignore_all_invalid_ids = False
     try:
         month = args[1].reduce_constant().value
         day = args[2].reduce_constant().value
     except generic.ConstError:
         raise generic.ScriptError("Month and day parameters of date() should be compile-time constants", pos)
-    generic.check_range(month, 1, 12, "month", args[1].pos)
-    generic.check_range(day, 1, days_in_month[month - 1], "day", args[2].pos)
-
     if not isinstance(year, ConstantNumeric):
         if month != 1 or day != 1:
-            raise generic.ScriptError(
-                "when the year parameter of date() is not a compile time constant month and day should be 1", pos
-            )
-        # num_days = year*365 + year/4 - year/100 + year/400
-        part1 = nmlop.MUL(year, 365)
-        part2 = nmlop.DIV(year, 4)
-        part3 = nmlop.DIV(year, 100)
-        part4 = nmlop.DIV(year, 400)
-        res = nmlop.ADD(part1, part2)
-        res = nmlop.SUB(res, part3)
-        res = nmlop.ADD(res, part4)
+            raise generic.ScriptError("when the year parameter of date() is not a compile time constant month and day should be 1", pos)
+        #num_days = year*365 + year/4 - year/100 + year/400
+        part1 = BinOp(nmlop.MUL, year, ConstantNumeric(365))
+        part2 = BinOp(nmlop.DIV, year, ConstantNumeric(4))
+        part3 = BinOp(nmlop.DIV, year, ConstantNumeric(100))
+        part4 = BinOp(nmlop.DIV, year, ConstantNumeric(400))
+        res = BinOp(nmlop.ADD, part1, part2)
+        res = BinOp(nmlop.SUB, res, part3)
+        res = BinOp(nmlop.ADD, res, part4)
         return res
-
-    generic.check_range(year.value, 0, 5000000, "year", year.pos)
+    days_in_month = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
     day_in_year = 0
     for i in range(month - 1):
         day_in_year += days_in_month[i]
     day_in_year += day
     if month >= 3 and (year.value % 4 == 0) and ((not year.value % 100 == 0) or (year.value % 400 == 0)):
         day_in_year += 1
     return ConstantNumeric(year.value * 365 + calendar.leapdays(0, year.value) + day_in_year - 1, pos)
 
-
-@builtin
 def builtin_day_of_year(name, args, pos):
     """
     day_of_year(month, day) builtin function.
 
     @return Day of the year, assuming February has 28 days.
     """
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have a month and a day parameter", pos)
 
     month = args[0].reduce()
     if not isinstance(month, ConstantNumeric):
-        raise generic.ScriptError("Month should be a compile-time constant.", month.pos)
+        raise generic.ScriptError('Month should be a compile-time constant.', month.pos)
     if month.value < 1 or month.value > 12:
-        raise generic.ScriptError("Month should be a value between 1 and 12.", month.pos)
+        raise generic.ScriptError('Month should be a value between 1 and 12.', month.pos)
 
     day = args[1].reduce()
     if not isinstance(day, ConstantNumeric):
-        raise generic.ScriptError("Day should be a compile-time constant.", day.pos)
+        raise generic.ScriptError('Day should be a compile-time constant.', day.pos)
 
     # Mapping of month to number of days in that month.
     number_days = {1: 31, 2: 28, 3: 31, 4: 30, 5: 31, 6: 30, 7: 31, 8: 31, 9: 30, 10: 31, 11: 30, 12: 31}
     if day.value < 1 or day.value > number_days[month.value]:
-        raise generic.ScriptError("Day should be value between 1 and {:d}.".format(number_days[month.value]), day.pos)
+        raise generic.ScriptError('Day should be value between 1 and %d.' % number_days[month.value], day.pos)
 
     return ConstantNumeric(datetime.date(1, month.value, day.value).toordinal(), pos)
 
-
-@builtins("STORE_TEMP", "STORE_PERM", "LOAD_TEMP", "LOAD_PERM")
 def builtin_storage(name, args, pos):
     """
     Accesses to temporary / persistent storage
     """
     return StorageOp(name, args, pos)
 
-
-@builtin
-def builtin_UCMP(name, args, pos):
+def builtin_ucmp(name, args, pos):
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have exactly two parameters", pos)
-    return nmlop.VACT2_UCMP(args[0], args[1], pos)
-
+    return BinOp(nmlop.VACT2_UCMP, args[0], args[1], pos)
 
-@builtin
-def builtin_CMP(name, args, pos):
+def builtin_cmp(name, args, pos):
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have exactly two parameters", pos)
-    return nmlop.VACT2_CMP(args[0], args[1], pos)
+    return BinOp(nmlop.VACT2_CMP, args[0], args[1], pos)
 
-
-@builtin
 def builtin_rotate(name, args, pos):
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have exactly two parameters", pos)
-    return nmlop.ROT_RIGHT(args[0], args[1], pos)
-
-
-@builtin
-def builtin_bitmask(name, args, pos):
-    return BitMask(args, pos)
+    return BinOp(nmlop.ROT_RIGHT, args[0], args[1], pos)
 
-
-@builtin
 def builtin_hasbit(name, args, pos):
     """
     hasbit(value, bit_num) builtin function.
 
     @return C{1} if and only if C{value} has bit C{bit_num} set, C{0} otherwise.
     """
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have exactly two parameters", pos)
-    return nmlop.HASBIT(args[0], args[1], pos)
-
-
-@builtin
-def builtin_getbits(name, args, pos):
-    """
-    getbits(value, first, amount) builtin function.
-
-    @return Extract C{amount} bits starting at C{first} from C{value},
-            that is (C{value} >> C{first}) & (1 << C{amount} - 1)
-    """
-    if len(args) != 3:
-        raise generic.ScriptError(name + "() must have exactly three parameters", pos)
+    return BinOp(nmlop.HASBIT, args[0], args[1], pos)
 
-    # getbits(value, first, amount) = (value >> first) & ((0xFFFFFFFF << amount) ^ 0xFFFFFFFF)
-    part1 = nmlop.SHIFTU_RIGHT(args[0], args[1], pos)
-    part2 = nmlop.SHIFT_LEFT(0xFFFFFFFF, args[2], pos)
-    part3 = nmlop.XOR(part2, 0xFFFFFFFF, pos)
-
-    return nmlop.AND(part1, part3, pos)
-
-
-@builtin
 def builtin_version_openttd(name, args, pos):
     """
     version_openttd(major, minor, revision[, build]) builtin function.
 
     @return The version information encoded in a double-word.
     """
     if len(args) > 4 or len(args) < 3:
         raise generic.ScriptError(name + "() must have 3 or 4 parameters", pos)
     major = args[0].reduce_constant().value
     minor = args[1].reduce_constant().value
     revision = args[2].reduce_constant().value
     build = args[3].reduce_constant().value if len(args) == 4 else 0x80000
     return ConstantNumeric((major << 28) | (minor << 24) | (revision << 20) | build)
 
+def builtin_cargotype_available(name, args, pos):
+    """
+    cargotype_available(cargo_label) builtin function.
 
-@builtins("cargotype_available", "railtype_available", "roadtype_available", "tramtype_available")
-def builtin_typelabel_available(name, args, pos):
+    @return 1 if the cargo label is available, 0 otherwise.
     """
-    {cargo|rail|road|tram}type_available(label) builtin functions.
+    if len(args) != 1:
+        raise generic.ScriptError(name + "() must have exactly 1 parameter", pos)
+    label = args[0].reduce()
+    return SpecialCheck((0x0B, r'\7c'), 0, (0, 1), parse_string_to_dword(label), "%s(%s)" % (name, str(label)), pos = args[0].pos)
 
-    @return 1 if the label is available, 0 otherwise.
+def builtin_railtype_available(name, args, pos):
     """
-    op = {
-        "cargotype_available": (0x0B, r"\7c"),
-        "railtype_available": (0x0D, None),
-        "roadtype_available": (0x0F, None),
-        "tramtype_available": (0x11, None),
-    }[name]
+    railtype_available(cargo_label) builtin function.
 
+    @return 1 if the railtype label is available, 0 otherwise.
+    """
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have exactly 1 parameter", pos)
     label = args[0].reduce()
-    return SpecialCheck(op, 0, (0, 1), parse_string_to_dword(label), "{}({})".format(name, label), pos=args[0].pos)
+    return SpecialCheck((0x0D, None), 0, (0, 1), parse_string_to_dword(label), "%s(%s)" % (name, str(label)), pos = args[0].pos)
 
-
-@builtins("grf_current_status", "grf_future_status", "grf_order_behind")
 def builtin_grf_status(name, args, pos):
     """
-    grf_{current_status|future_status|order_behind}(grfid[, mask]) builtin functions.
+    grf_(current_status|future_status|order_behind)(grfid[, mask]) builtin function.
 
     @return 1 if the grf is, or will be, active, 0 otherwise.
     """
-    op, results = {
-        # can't use \7g (0, 1), because that's false when the queried grf isn't present at all.
-        "grf_current_status": ((0x06, r"\7G"), (1, 0)),
-        "grf_future_status": ((0x0A, r"\7gg"), (0, 1)),
-        "grf_order_behind": ((0x08, r"\7gG"), (0, 1)),
-    }[name]
-
-    if len(args) == 1:
-        grfid = args[0].reduce()
-        mask = None
-        string = "{}({})".format(name, grfid)
-        varsize = 4
-    elif len(args) == 2:
-        grfid = args[0].reduce()
-        mask = parse_string_to_dword(args[1].reduce())
-        string = "{}({}, {})".format(name, grfid, mask)
-        varsize = 8
-    else:
+    if len(args) not in (1, 2):
         raise generic.ScriptError(name + "() must have 1 or 2 parameters", pos)
+    labels = [label.reduce() for label in args]
+    mask = parse_string_to_dword(labels[1]) if len(labels) > 1 else None
+    if name == 'grf_current_status':
+        op = (0x06, r'\7G')
+        results = (1, 0)
+    elif name == 'grf_future_status':
+        op = (0x0A, r'\7gg')
+        results = (0, 1)
+    elif name == 'grf_order_behind':
+        op = (0x08, r'\7gG')
+        results = (0, 1)
+    else:
+        assert False, "Unknown grf status function"
+    if mask is None:
+        string = "%s(%s)" % (name, str(label))
+    else:
+        string = "%s(%s, %s)" % (name, str(label), str(mask))
+    return SpecialCheck(op, 0x88, results, parse_string_to_dword(labels[0]), string, mask, args[0].pos)
 
-    return SpecialCheck(op, 0x88, results, parse_string_to_dword(grfid), string, varsize, mask, args[0].pos)
-
-
-@builtins("visual_effect", "visual_effect_and_powered")
 def builtin_visual_effect_and_powered(name, args, pos):
     """
     Builtin function, used in two forms:
     visual_effect_and_powered(effect, offset, powered)
     visual_effect(effect, offset)
     Use this to set the vehicle property visual_effect[_and_powered]
     and for the callback VEH_CB_VISUAL_EFFECT[_AND_POWERED]
-
+    
     """
-    arg_len = 2 if name == "visual_effect" else 3
+    arg_len = 2 if name == 'visual_effect' else 3
     if len(args) != arg_len:
-        raise generic.ScriptError(name + "() must have {:d} parameters".format(arg_len), pos)
+        raise generic.ScriptError(name + "() must have %d parameters" % arg_len, pos)
+    from nml import global_constants
     effect = args[0].reduce_constant(global_constants.const_list).value
-    offset = nmlop.ADD(args[1], 8).reduce_constant().value
+    offset = BinOp(nmlop.ADD, args[1], ConstantNumeric(8), args[1].pos).reduce_constant().value
     generic.check_range(offset, 0, 0x0F, "offset in function " + name, pos)
     if arg_len == 3:
         powered = args[2].reduce_constant(global_constants.const_list).value
         if powered != 0 and powered != 0x80:
-            raise generic.ScriptError(
-                "3rd argument to visual_effect_and_powered (powered) must be"
-                " either ENABLE_WAGON_POWER or DISABLE_WAGON_POWER",
-                pos,
-            )
+            raise generic.ScriptError("3rd argument to visual_effect_and_powered (powered) must be either ENABLE_WAGON_POWER or DISABLE_WAGON_POWER", pos)
     else:
         powered = 0
     return ConstantNumeric(effect | offset | powered)
 
-
-@builtin
-def builtin_create_effect(name, args, pos):
-    """
-    Builtin function:
-    create_effect(effect_sprite, l_x_offset, t_y_offset, z_offset)
-    Use this to set the values for temporary storages 100+x
-    in the callback create_effect
-
-    """
-    if len(args) != 4:
-        raise generic.ScriptError(name + "() must have 4 parameters", pos)
-
-    sprite = args[0].reduce_constant(global_constants.const_list).value
-    offset1 = args[1].reduce_constant().value
-    offset2 = args[2].reduce_constant().value
-    offset3 = args[3].reduce_constant().value
-
-    generic.check_range(sprite, 0, 255, "effect_sprite in function " + name, args[0].pos)
-    generic.check_range(offset1, -128, 127, "l_x_offset in function " + name, args[1].pos)
-    generic.check_range(offset2, -128, 127, "t_y_offset in function " + name, args[2].pos)
-    generic.check_range(offset3, -128, 127, "z_offset in function " + name, args[3].pos)
-
-    return ConstantNumeric(sprite | (offset1 & 0xFF) << 8 | (offset2 & 0xFF) << 16 | (offset3 & 0xFF) << 24)
-
-
-@builtin
 def builtin_str2number(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
     return ConstantNumeric(parse_string_to_dword(args[0]))
 
-
-@builtins("cargotype", "railtype", "roadtype", "tramtype")
-def builtin_resolve_typelabel(name, args, pos, table_name=None):
-    """
-    {cargo,rail,road,tram}type(label) builtin functions.
-
-    Also used from some Action2Var variables to resolve cargo labels.
-    """
-    tracktype_funcs = {
-        "cargotype": global_constants.cargo_numbers,
-        "railtype": global_constants.railtype_table,
-        "roadtype": global_constants.roadtype_table,
-        "tramtype": global_constants.tramtype_table,
-    }
-
-    if not table_name:
-        table_name = name
-    table = tracktype_funcs[table_name]
-    if table_name == "cargotype":
-        table_name = "cargo"  # NML syntax uses "cargotable" and "railtypetable"
-
+def builtin_cargotype(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
-    if not isinstance(args[0], StringLiteral) or args[0].value not in table:
-        raise generic.ScriptError(
-            "Parameter for {}() must be a string literal that is also in your {} table".format(name, table_name), pos
-        )
-    return ConstantNumeric(table[args[0].value])
+    from nml import global_constants
+    if not isinstance(args[0], StringLiteral) or args[0].value not in global_constants.cargo_numbers:
+        raise generic.ScriptError("Parameter for " + name + "() must be a string literal that is also in your cargo table", pos)
+    return ConstantNumeric(global_constants.cargo_numbers[args[0].value])
 
+def builtin_railtype(name, args, pos):
+    if len(args) != 1:
+        raise generic.ScriptError(name + "() must have 1 parameter", pos)
+    from nml import global_constants
+    if not isinstance(args[0], StringLiteral) or args[0].value not in global_constants.railtype_table:
+        raise generic.ScriptError("Parameter for " + name + "() must be a string literal that is also in your railtype table", pos)
+    return ConstantNumeric(global_constants.railtype_table[args[0].value])
 
-@builtin
 def builtin_reserve_sprites(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
     count = args[0].reduce_constant()
-    return GRMOp(nmlop.GRM_RESERVE, 0x08, count.value, lambda x: "{}({:d})".format(name, count.value), pos)
+    func = lambda x: '%s(%d)' % (name, count.value)
+    return GRMOp(nmlop.GRM_RESERVE, 0x08, count.value, func, pos)
 
-
-@builtin
 def builtin_industry_type(name, args, pos):
     """
     industry_type(IND_TYPE_OLD | IND_TYPE_NEW, id) builtin function
 
     @return The industry type in the format used by grfs (industry prop 0x16 and var 0x64)
     """
     if len(args) != 2:
         raise generic.ScriptError(name + "() must have 2 parameters", pos)
 
+    from nml import global_constants
     type = args[0].reduce_constant(global_constants.const_list).value
     if type not in (0, 1):
         raise generic.ScriptError("First argument of industry_type() must be IND_TYPE_OLD or IND_TYPE_NEW", pos)
 
-    # Industry ID uses 7 bits (0 .. 6), bit 7 is for old/new
+    # Industry ID uses 6 bits (0 .. 5), so bit 6 is never used
     id = args[1].reduce_constant(global_constants.const_list).value
-    if not 0 <= id <= 127:
-        raise generic.ScriptError("Second argument 'id' of industry_type() must be in range 0..127", pos)
+    if not 0 <= id <= 63:
+        raise generic.ScriptError("Second argument 'id' of industry_type() must be in range 0..63", pos)
 
     return ConstantNumeric(type << 7 | id)
 
-
-@builtins("accept_cargo", "produce_cargo")
-def builtin_cargoexpr(name, args, pos):
-    if len(args) < 1:
-        raise generic.ScriptError(name + "() must have 1 or more parameters", pos)
-
-    if not isinstance(args[0], StringLiteral) or args[0].value not in global_constants.cargo_numbers:
-        raise generic.ScriptError(
-            "First argument of " + name + "() must be a string literal that is also in your cargo table", pos
-        )
-    cargotype = global_constants.cargo_numbers[args[0].value]
-
-    if name == "produce_cargo":
-        return ProduceCargo(cargotype, args[1:], pos)
-    elif name == "accept_cargo":
-        return AcceptCargo(cargotype, args[1:], pos)
-    else:
-        raise AssertionError()
-
-
-@builtins("acos", "asin", "atan", "cos", "sin", "sqrt", "tan")
-def builtin_math(name, args, pos):
+def builtin_trigonometric(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
     val = args[0].reduce()
     if not isinstance(val, (ConstantNumeric, ConstantFloat)):
         raise generic.ScriptError("Parameter for " + name + "() must be a constant", pos)
-    math_func_table = {
-        "acos": math.acos,
-        "asin": math.asin,
-        "atan": math.atan,
-        "cos": math.cos,
-        "sin": math.sin,
-        "sqrt": math.sqrt,
-        "tan": math.tan,
-    }
-    return ConstantFloat(math_func_table[name](val.value), val.pos)
-
-
-@builtin
-def builtin_round(name, args, pos):
-    if len(args) != 1:
-        raise generic.ScriptError(name + "() must have 1 parameter", pos)
-    val = args[0].reduce()
-    if not isinstance(val, (ConstantNumeric, ConstantFloat)):
         raise generic.ScriptError("Parameter for " + name + "() must be a constant", pos)
-    return ConstantNumeric(round(val.value), pos)
-
+    trigonometric_func_table = {
+        'acos': math.acos,
+        'asin': math.asin,
+        'atan': math.atan,
+        'cos': math.cos,
+        'sin': math.sin,
+        'tan': math.tan,
+    }
+    return ConstantFloat(trigonometric_func_table[name](val.value), val.pos)
 
-@builtin
 def builtin_int(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
     val = args[0].reduce()
     if not isinstance(val, (ConstantNumeric, ConstantFloat)):
         raise generic.ScriptError("Parameter for " + name + "() must be a constant", pos)
     return ConstantNumeric(int(val.value), val.pos)
 
-
-@builtin
 def builtin_abs(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
-    return AbsOp(args[0], args[0].pos).reduce()
-
-
-@builtin
-def builtin_sound(name, args, pos):
-    if len(args) not in (1, 2):
-        raise generic.ScriptError(name + "() must have 1 or 2 parameters", pos)
-    if not isinstance(args[0], StringLiteral):
-        raise generic.ScriptError("Parameter for " + name + "() must be a string literal", pos)
-    volume = args[1].reduce_constant().value if len(args) >= 2 else 100
-    generic.check_range(volume, 0, 100, "sound volume", pos)
-    from nml.actions import action11
-
-    return ConstantNumeric(action11.add_sound((args[0].value, volume), pos), pos)
-
-
-@builtin
-def builtin_import_sound(name, args, pos):
-    if len(args) not in (2, 3):
-        raise generic.ScriptError(name + "() must have 2 or 3 parameters", pos)
-    grfid = parse_string_to_dword(args[0].reduce())
-    sound_num = args[1].reduce_constant().value
-    volume = args[2].reduce_constant().value if len(args) >= 3 else 100
-    generic.check_range(volume, 0, 100, "sound volume", pos)
-    from nml.actions import action11
-
-    return ConstantNumeric(action11.add_sound((grfid, sound_num, volume), pos), pos)
-
-
-@builtin
-def builtin_relative_coord(name, args, pos):
-    """
-    relative_coord(x, y) builtin function.
-
-    @return Coordinates in 0xYYXX format.
-    """
-    if len(args) != 2:
-        raise generic.ScriptError(name + "() must have x and y coordinates as parameters", pos)
-
-    if isinstance(args[0], ConstantNumeric):
-        generic.check_range(args[0].value, 0, 255, "Argument of '{}'".format(name), args[0].pos)
-    if isinstance(args[1], ConstantNumeric):
-        generic.check_range(args[1].value, 0, 255, "Argument of '{}'".format(name), args[1].pos)
-
-    x_coord = nmlop.AND(args[0], 0xFF)
-    y_coord = nmlop.AND(args[1], 0xFF)
-    # Shift Y to its position.
-    y_coord = nmlop.SHIFT_LEFT(y_coord, 8)
-
-    return nmlop.OR(x_coord, y_coord, pos)
-
-
-@builtin
-def builtin_num_corners_raised(name, args, pos):
-    """
-    num_corners_raised(slope) builtin function.
-    slope is a 5-bit value
-
-    @return Number of raised corners in a slope (4 for steep slopes)
-    """
-    if len(args) != 1:
-        raise generic.ScriptError(name + "() must have 1 parameter", pos)
+    guard = BinOp(nmlop.CMP_LT, args[0], ConstantNumeric(0), args[0].pos)
+    return TernaryOp(guard, BinOp(nmlop.SUB, ConstantNumeric(0), args[0], args[0].pos), args[0], args[0].pos).reduce()
 
-    slope = args[0]
-    # The returned value is ((slope x 0x8421) & 0x11111) % 0xF
-    # Explanation in steps: (numbers in binary)
-    # - Masking constrains the slope to 5 bits, just to be sure (a|bcde)
-    # - Multiplication creates 4 copies of those bits (abcd|eabc|deab|cdea|bcde)
-    # - And-masking leaves only the lowest bit in each nibble (000d|000c|000b|000a|000e)
-    # - The modulus operation adds one to the output for each set bit
-    # - We now have the count of bits in the slope, which is wat we want. yay!
-    slope = nmlop.AND(slope, 0x1F, pos)
-    slope = nmlop.MUL(slope, 0x8421)
-    slope = nmlop.AND(slope, 0x11111)
-    return nmlop.MOD(slope, 0xF)
-
-
-@builtin
-def builtin_slope_to_sprite_offset(name, args, pos):
-    """
-    builtin function slope_to_sprite_offset(slope)
-
-    @return sprite offset to use
-    """
-    if len(args) != 1:
-        raise generic.ScriptError(name + "() must have 1 parameter", pos)
-
-    if isinstance(args[0], ConstantNumeric):
-        generic.check_range(args[0].value, 0, 15, "Argument of '{}'".format(name), args[0].pos)
-
-    # step 1: ((slope >= 0) & (slope <= 14)) * slope
-    # This handles all non-steep slopes
-    expr = nmlop.AND(nmlop.CMP_LE(args[0], 14, pos), nmlop.CMP_GE(args[0], 0, pos))
-    expr = nmlop.MUL(expr, args[0])
-    # Now handle the steep slopes separately
-    # So add (slope == SLOPE_XX) * offset_of_SLOPE_XX for each steep slope
-    steep_slopes = [(23, 16), (27, 17), (29, 15), (30, 18)]
-    for slope, offset in steep_slopes:
-        to_add = nmlop.MUL(nmlop.CMP_EQ(args[0], slope, pos), offset)
-        expr = nmlop.ADD(expr, to_add)
-    return expr
-
-
-@builtin
-def builtin_palette_1cc(name, args, pos):
-    """
-    palette_1cc(colour) builtin function.
-
-    @return Recolour sprite to use
-    """
+def builtin_sound_file(name, args, pos):
     if len(args) != 1:
         raise generic.ScriptError(name + "() must have 1 parameter", pos)
+    if not isinstance(args[0], StringLiteral):
+        raise generic.ScriptError("Parameter for " + name + "() must be a string literal", pos)
+    return ConstantNumeric(action11.add_sound(args[0].value), pos)
 
-    if isinstance(args[0], ConstantNumeric):
-        generic.check_range(args[0].value, 0, 15, "Argument of '{}'".format(name), args[0].pos)
-
-    return nmlop.ADD(args[0], 775, pos)
-
-
-@builtin
-def builtin_palette_2cc(name, args, pos):
-    """
-    palette_2cc(colour1, colour2) builtin function.
-
-    @return Recolour sprite to use
-    """
-    if len(args) != 2:
-        raise generic.ScriptError(name + "() must have 2 parameters", pos)
-
-    for i in range(0, 2):
-        if isinstance(args[i], ConstantNumeric):
-            generic.check_range(args[i].value, 0, 15, "Argument of '{}'".format(name), args[i].pos)
-
-    col2 = nmlop.MUL(args[1], 16, pos)
-    col12 = nmlop.ADD(col2, args[0])
-    # Base sprite is not a constant
-    base = global_constants.patch_variable("base_sprite_2cc", global_constants.patch_variables["base_sprite_2cc"], pos)
-
-    return nmlop.ADD(col12, base)
-
-
-@builtin
-def builtin_vehicle_curv_info(name, args, pos):
-    """
-    vehicle_curv_info(prev_cur, cur_next) builtin function
-
-    @return Value to use with vehicle var curv_info
-    """
+def builtin_sound_import(name, args, pos):
     if len(args) != 2:
-        raise generic.ScriptError(name + "() must have 2 parameters", pos)
-
-    for arg in args:
-        if isinstance(arg, ConstantNumeric):
-            generic.check_range(arg.value, -2, 2, "Argument of '{}'".format(name), arg.pos)
-
-    args = [nmlop.AND(arg, 0xF, pos) for arg in args]
-    cur_next = nmlop.SHIFT_LEFT(args[1], 8)
-    return nmlop.OR(args[0], cur_next)
-
-
-@builtin
-def builtin_format_string(name, args, pos):
-    """
-    format_string(format, ... args ..) builtin function
-
-    @return Formatted string
-    """
-    if len(args) < 1:
-        raise generic.ScriptError(name + "() must have at least one parameter", pos)
-
-    format = args[0].reduce()
-    if not isinstance(format, StringLiteral):
-        raise generic.ScriptError(name + "() parameter 1 'format' must be a literal string", format.pos)
-
-    # Validate other args
-    format_args = []
-    for i, arg in enumerate(args[1:]):
-        arg = arg.reduce()
-        if not isinstance(arg, (StringLiteral, ConstantFloat, ConstantNumeric)):
-            raise generic.ScriptError(
-                name + "() parameter {:d} is not a constant number of literal string".format(i + 1), arg.pos
-            )
-        format_args.append(arg.value)
-
-    try:
-        result = format.value % tuple(format_args)
-        return StringLiteral(result, pos)
-    except Exception as ex:
-        raise generic.ScriptError("Invalid combination of format / arguments for {}: {}".format(name, str(ex)), pos)
-
+        raise generic.ScriptError(name + "() must have 2 parameter", pos)
+    grfid = args[0].reduce()
+    if isinstance(grfid, ConstantNumeric):
+        grfid = grfid.value
+    else:
+        grfid = parse_string_to_dword(grfid)
+    sound_num = args[1].reduce_constant().value
+    return ConstantNumeric(action11.add_sound((grfid, sound_num)), pos)
+#}
 
-# }
+function_table = {
+    'min' : builtin_min,
+    'max' : builtin_max,
+    'date' : builtin_date,
+    'day_of_year' : builtin_day_of_year,
+    'bitmask' : lambda name, args, pos: BitMask(args, pos),
+    'STORE_TEMP' : builtin_storage,
+    'STORE_PERM' : builtin_storage,
+    'LOAD_TEMP' : builtin_storage,
+    'LOAD_PERM' : builtin_storage,
+    'hasbit' : builtin_hasbit,
+    'version_openttd' : builtin_version_openttd,
+    'cargotype_available' : builtin_cargotype_available,
+    'railtype_available' : builtin_railtype_available,
+    'grf_current_status' : builtin_grf_status,
+    'grf_future_status' : builtin_grf_status,
+    'grf_order_behind' : builtin_grf_status,
+    'visual_effect' : builtin_visual_effect_and_powered,
+    'visual_effect_and_powered' : builtin_visual_effect_and_powered,
+    'str2number' : builtin_str2number,
+    'cargotype' : builtin_cargotype,
+    'railtype' : builtin_railtype,
+    'reserve_sprites' : builtin_reserve_sprites,
+    'industry_type' : builtin_industry_type,
+    'int' : builtin_int,
+    'abs' : builtin_abs,
+    'acos' : builtin_trigonometric,
+    'asin' : builtin_trigonometric,
+    'atan' : builtin_trigonometric,
+    'cos' : builtin_trigonometric,
+    'sin' : builtin_trigonometric,
+    'tan' : builtin_trigonometric,
+    'UCMP' : builtin_ucmp,
+    'CMP' : builtin_cmp,
+    'rotate' : builtin_rotate,
+    'sound' : builtin_sound_file,
+    'import_sound': builtin_sound_import,
+}
```

### Comparing `nml-0.7.2/nml/expression/parameter.py` & `nml-r1512/nml/expression/parameter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,92 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic, grfstrings
-
-from .base_expression import ConstantNumeric, Expression, Type
+from .base_expression import Type, Expression, ConstantNumeric
 from .string_literal import StringLiteral
 
-
 class Parameter(Expression):
-    def __init__(self, num, pos=None, by_user=False):
+    def __init__(self, num, pos = None, by_user = False):
         Expression.__init__(self, pos)
         self.num = num
         if by_user and isinstance(num, ConstantNumeric) and not (0 <= num.value <= 63):
-            generic.print_warning(
-                generic.Warning.GENERIC,
-                "Accessing parameters out of the range 0..63 is not supported and may lead to unexpected behaviour.",
-                pos,
-            )
+            generic.print_warning("Accessing parameters out of the range 0..63 is not supported and may lead to unexpected behaviour.", pos)
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Parameter:")
+        print indentation*' ' + 'Parameter:'
         self.num.debug_print(indentation + 2)
 
     def __str__(self):
-        return "param[{}]".format(self.num)
+        return 'param[%s]' % str(self.num)
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         num = self.num.reduce(id_dicts)
         if num.type() != Type.INTEGER:
             raise generic.ScriptError("Parameter number must be an integer.", num.pos)
         return Parameter(num, self.pos)
 
     def supported_by_action2(self, raise_error):
         supported = isinstance(self.num, ConstantNumeric)
         if not supported and raise_error:
-            raise generic.ScriptError(
-                "Parameter acessess with non-constant numbers are not supported in a switch-block.", self.pos
-            )
+            raise generic.ScriptError("Parameter acessess with non-constant numbers are not supported in a switch-block.", self.pos)
         return supported
 
     def supported_by_actionD(self, raise_error):
         return True
 
     def __eq__(self, other):
         return other is not None and isinstance(other, Parameter) and self.num == other.num
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash((self.num,))
 
-
 class OtherGRFParameter(Expression):
-    def __init__(self, grfid, num, pos=None):
+    def __init__(self, grfid, num, pos = None):
         Expression.__init__(self, pos)
         self.grfid = grfid
         self.num = num
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "OtherGRFParameter:")
+        print indentation*' ' + 'OtherGRFParameter:'
         self.grfid.debug_print(indentation + 2)
         self.num.debug_print(indentation + 2)
 
     def __str__(self):
-        return "param[{}, {}]".format(self.grfid, self.num)
+        return 'param[%s, %s]' % (str(self.grfid), str(self.num))
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
-        grfid = self.grfid.reduce(id_dicts)
-        # Test validity
-        parse_string_to_dword(grfid)
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
+        grfid = self.grfid.reduce()
+        if isinstance(grfid, StringLiteral):
+            grfid = ConstantNumeric(parse_string_to_dword(grfid))
+        grfid.reduce_constant()
         num = self.num.reduce(id_dicts)
         if num.type() != Type.INTEGER:
             raise generic.ScriptError("Parameter number must be an integer.", num.pos)
         return OtherGRFParameter(grfid, num, self.pos)
 
     def supported_by_action2(self, raise_error):
         if raise_error:
-            raise generic.ScriptError(
-                "Reading parameters from another GRF is not supported in a switch-block.", self.pos
-            )
+            raise generic.ScriptError("Reading parameters from another GRF is not supported in a switch-block.", self.pos)
         return False
 
     def supported_by_actionD(self, raise_error):
         return True
 
-
 def parse_string_to_dword(string):
-    """
-    Convert string literal expression of length 4 to it's equivalent 32 bit number.
-
-    @param string: Expression to convert.
-    @type  string: L{Expression}
-
-    @return: Value of the converted expression (a 32 bit integer number, little endian).
-    @rtype:  C{int}
-    """
     if not isinstance(string, StringLiteral) or grfstrings.get_string_size(string.value, False, True) != 4:
         raise generic.ScriptError("Expected a string literal of length 4", string.pos)
-
     pos = string.pos
     string = string.value
     bytes = []
     i = 0
     try:
         while len(bytes) < 4:
-            if string[i] == "\\":
-                bytes.append(int(string[i + 1 : i + 3], 16))
+            if string[i] == '\\':
+                bytes.append(int(string[i+1:i+3], 16))
                 i += 3
             else:
                 bytes.append(ord(string[i]))
                 i += 1
     except ValueError:
         raise generic.ScriptError("Cannot convert string to integer id", pos)
-
     return bytes[0] | (bytes[1] << 8) | (bytes[2] << 16) | (bytes[3] << 24)
```

### Comparing `nml-0.7.2/nml/expression/special_parameter.py` & `nml-r1512/nml/expression/special_parameter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,18 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic
-
 from .base_expression import Expression
 
-
 class SpecialParameter(Expression):
     """
     Class for handling special grf parameters.
     These can be assigned special, custom methods for reading / writing to them.
 
-    @ivar name: Name of the parameter, for debugging purposes.
-    @type name: C{str}
+    @ivar name: Name of the parameter, for debugging purposes
+    @type name: C{basestring}
 
-    @ivar info: Information about the parameter.
+    @ivar info: Information about the parameter
     @type info: C{dict}
 
     @ivar write_func: Function that will be called when the parameter is the target of an assignment
                         Arguments:
                             Dictionary with parameter information (self.info)
                             Target expression to assign
                             Position information
@@ -47,29 +29,29 @@
                             Expression that should be evaluated to get the parameter value
     @type read_func: C{function}
 
     @ivar is_bool: Does read_func return a boolean value?
     @type is_bool: C{bool}
     """
 
-    def __init__(self, name, info, write_func, read_func, is_bool, pos=None):
+    def __init__(self, name, info, write_func, read_func, is_bool, pos = None):
         Expression.__init__(self, pos)
         self.name = name
         self.info = info
         self.write_func = write_func
         self.read_func = read_func
         self.is_bool = is_bool
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Special parameter '{}'".format(self.name))
+        print indentation*' ' + "Special parameter '%s'" % self.name
 
     def __str__(self):
         return self.name
 
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
         return self
 
     def is_boolean(self):
         return self.is_bool
 
     def can_assign(self):
         return self.write_func is not None
```

### Comparing `nml-0.7.2/nml/expression/storage_op.py` & `nml-r1512/nml/ast/produce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,107 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
-from nml import generic
-
-from .base_expression import ConstantNumeric, Expression, Type
-from .parameter import parse_string_to_dword
-
-storage_op_info = {
-    "STORE_PERM": {"store": True, "perm": True, "grfid": False, "max": 0xFF, "reserved": ()},
-    "STORE_TEMP": {"store": True, "perm": False, "grfid": False, "max": 0x10F, "reserved": range(0x80, 0xFF + 1)},
-    "LOAD_PERM": {"store": False, "perm": True, "grfid": True, "max": 0xFF, "reserved": ()},
-    "LOAD_TEMP": {"store": False, "perm": False, "grfid": False, "max": 0xFF, "reserved": range(0x80, 0xFF + 1)},
-}
+from nml import expression, generic, global_constants, nmlop
+from nml.actions import action2, action2production
+from nml.ast import base_statement, switch
 
+produce_base_class = action2.make_sprite_group_class(action2.SpriteGroupRefType.SPRITEGROUP, action2.SpriteGroupRefType.NONE, action2.SpriteGroupRefType.SPRITEGROUP, True)
 
-class StorageOp(Expression):
+class Produce(produce_base_class):
     """
-    Class for reading/writing to (temporary or permanent) storage
+    AST node for a 'produce'-block, which is basically equivalent to the production callback.
+    Syntax: produce(name, sub1, sub2, sub3, add1, add2[, again])
 
-    @ivar name: Name of the called storage function
-    @type name: C{str}
+    @ivar param_list: List of parameters supplied to the produce-block.
+                      After pre-processing, their order is:
+                       - 0..2: Amounts of cargo to subtract from input
+                       - 3..4: Amounts of cargo to add to output
+                       - 5:    Run the production CB again if nonzero
+    @type param_list: C{list} of L{Expression}
 
-    @ivar info: Dictionary containting information about the operation to perform
-    @type info: C{dict}
+    @ivar pos: Position of produce-block.
+    @type pos: L{Position}
 
-    @ivar value: Value to store, or C{None} for loading operations
-    @type value: L{Expression}
-
-    @ivar register: Register to access
-    @type register: L{Expression}
-
-    @ivar grfid: GRFID of the register to access
-    @type grfid: L{Expression}
+    @ivar switch: Switch block that precedes this produce block to put *stuff* in registers
+    @type switch: L{Switch} or C{None} if N/A
 
+    @ivar version: Version of the production CB (0 or 1) to be used
+    @type version: C{int}
     """
+    def __init__(self, param_list, pos):
+        base_statement.BaseStatement.__init__(self, "produce-block", pos, False, False)
+        self.param_list = param_list
+        self.switch = None
+
+    def pre_process(self):
+        if not (6 <= len(self.param_list) <= 7):
+            raise generic.ScriptError("produce-block requires 6 or 7 parameters, encountered " + str(len(self.param_list)), self.pos)
+
+        name = self.param_list[0]
+        if not isinstance(name, expression.Identifier):
+            raise generic.ScriptError("produce parameter 1 'name' should be an identifier.", name.pos)
+
+        self.param_list = self.param_list[1:]
+        for i, param in enumerate(self.param_list):
+            self.param_list[i] = param.reduce(global_constants.const_list)
+
+        if len(self.param_list) < 6:
+            self.param_list.append(expression.ConstantNumeric(0))
+
+        self.version = 0 if all(map(lambda x: x.supported_by_actionD(False), self.param_list)) else 1
+        if self.version == 1:
+            va2_expr = None
+            for i, param in enumerate(self.param_list[:]):
+                if isinstance(param, expression.Variable) and isinstance(param.num, expression.ConstantNumeric) and \
+                        param.num.value == 0x7D and isinstance(param.param, expression.ConstantNumeric):
+                    # We can load a register directly
+                    self.param_list[i] = param.param
+                else:
+                    expr = expression.BinOp(nmlop.STO_TMP, param, expression.ConstantNumeric(0x80 + i))
+                    if va2_expr is None:
+                        va2_expr = expr
+                    else:
+                        va2_expr = expression.BinOp(nmlop.VAL2, va2_expr, expr)
+                    self.param_list[i] = expression.ConstantNumeric(0x80 + i)
+
+            if va2_expr is not None:
+                # We need a preceding switch/varaction2 to store *stuff* in registers
+                va2_feature = expression.ConstantNumeric(0x0A)
+                va2_range = expression.Identifier('SELF', self.pos)
+                va2_name = expression.Identifier(name.value, self.pos)
+
+                # Rename ourself
+                name.value += '@prod'
+
+                va2_body = switch.SwitchBody([], expression.SpriteGroupRef(expression.Identifier(name.value, self.pos), [], self.pos))
+                self.switch = switch.Switch(va2_feature, va2_range, va2_name, va2_expr, va2_body, self.pos)
+
+        # initialize base class and pre_process it as well (in that order), do the same for switch if applicable
+        self.initialize(name, expression.ConstantNumeric(0x0A))
+        produce_base_class.pre_process(self)
+        if self.switch is not None: self.switch.pre_process()
 
-    def __init__(self, name, args, pos=None):
-        Expression.__init__(self, pos)
-        self.name = name
-        assert name in storage_op_info
-        self.info = storage_op_info[name]
-
-        arg_len = (2,) if self.info["store"] else (1,)
-        if self.info["grfid"]:
-            arg_len += (arg_len[0] + 1,)
-        if len(args) not in arg_len:
-            argstr = "{:d}".format(arg_len[0]) if len(arg_len) == 1 else "{}..{}".format(arg_len[0], arg_len[1])
-            raise generic.ScriptError(
-                "{} requires {} argument(s), encountered {:d}".format(name, argstr, len(args)), pos
-            )
-
-        i = 0
-        if self.info["store"]:
-            self.value = args[i]
-            i += 1
-        else:
-            self.value = None
-
-        self.register = args[i]
-        i += 1
-
-        if i < len(args):
-            self.grfid = args[i]
-            assert self.info["grfid"]
-        else:
-            self.grfid = None
-
-    def debug_print(self, indentation):
-        generic.print_dbg(indentation, self.name)
-        generic.print_dbg(indentation + 2, "Register:")
-        self.register.debug_print(indentation + 4)
-        if self.value is not None:
-            generic.print_dbg(indentation + 2, "Value:")
-            self.value.debug_print(indentation + 4)
-        if self.grfid is not None:
-            generic.print_dbg(indentation + 2, "GRFID:")
-            self.grfid.debug_print(indentation + 4)
+    def collect_references(self):
+        return []
 
     def __str__(self):
-        args = []
-        if self.value is not None:
-            args.append(str(self.value))
-        args.append(str(self.register))
-        if self.grfid is not None:
-            args.append(str(self.grfid))
-        return "{}({})".format(self.name, ", ".join(args))
-
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
-        args = []
-        if self.value is not None:
-            value = self.value.reduce(id_dicts)
-            if value.type() != Type.INTEGER:
-                if value.type() == Type.SPRITEGROUP_REF:
-                    raise generic.ProcCallSyntaxError(value.name, value.pos)
-                raise generic.ScriptError("Value to store must be an integer.", value.pos)
-            args.append(value)
-
-        register = self.register.reduce(id_dicts)
-        if register.type() != Type.INTEGER:
-            if register.type() == Type.SPRITEGROUP_REF:
-                raise generic.ProcCallSyntaxError(register.name, register.pos)
-            raise generic.ScriptError("Register to access must be an integer.", register.pos)
-        if isinstance(register, ConstantNumeric) and register.value > self.info["max"]:
-            raise generic.ScriptError("Maximum register for {} is {:d}".format(self.name, self.info["max"]), self.pos)
-        if isinstance(register, ConstantNumeric) and register.value in self.info["reserved"]:
-            raise generic.ScriptError(
-                "Temporary registers from 128 to 255 are reserved for NML's internal calculations.", self.pos
-            )
-        args.append(register)
-
-        if self.grfid is not None:
-            grfid = self.grfid.reduce(id_dicts)
-            # Test validity
-            parse_string_to_dword(grfid)
-            args.append(grfid)
-
-        return StorageOp(self.name, args, self.pos)
-
-    def supported_by_action2(self, raise_error):
-        return True
-
-    def supported_by_actionD(self, raise_error):
-        if raise_error:
-            raise generic.ScriptError("{}() may only be used inside switch-blocks".format(self.name), self.pos)
-        return False
-
-    def collect_references(self):
-        return self.register.collect_references() + (self.value.collect_references() if self.value is not None else [])
+        return 'produce(%s);\n' % ', '.join(str(x) for x in self.param_list)
 
-    def is_read_only(self):
-        assert self.info["store"] == (self.value is not None)
-        return (not self.info["store"]) and self.register.is_read_only()
+    def debug_print(self, indentation):
+        print indentation*' ' + 'Produce, name =', str(self.name)
+        print (indentation+2)*' ' + ('Using numeric values' if self.version == 0 else 'Using temp. registers')
+        print (indentation+2)*' ' + 'Subtract from input:'
+        for expr in self.param_list[0:3]:
+            expr.debug_print(indentation + 4)
+        print (indentation+2)*' ' + 'Add to output:'
+        for expr in self.param_list[3:5]:
+            expr.debug_print(indentation + 4)
+        print (indentation+2)*' ' + 'Again:'
+        self.param_list[5].debug_print(indentation + 4)
+        if self.switch is not None:
+            print (indentation+2)*' ' + 'Preceding switch block:'
+            self.switch.debug_print(indentation + 4)
+
+    def get_action_list(self):
+        action_list = []
+        if self.prepare_output():
+            action_list += action2production.get_production_actions(self)
+            if self.switch is not None: action_list += self.switch.get_action_list()
+        return action_list
```

### Comparing `nml-0.7.2/nml/expression/ternaryop.py` & `nml-r1512/nml/expression/variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,67 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic
+from .base_expression import Type, Expression, ConstantNumeric
 
-from .base_expression import ConstantNumeric, Expression, Type
-
-
-class TernaryOp(Expression):
-    def __init__(self, guard, expr1, expr2, pos):
+class Variable(Expression):
+    def __init__(self, num, shift = None, mask = None, param = None, pos = None):
         Expression.__init__(self, pos)
-        self.guard = guard
-        self.expr1 = expr1
-        self.expr2 = expr2
+        self.num = num
+        self.shift = shift if shift is not None else ConstantNumeric(0)
+        self.mask = mask if mask is not None else ConstantNumeric(0xFFFFFFFF)
+        self.param = param
+        self.add = None
+        self.div = None
+        self.mod = None
+        self.extra_params = []
 
     def debug_print(self, indentation):
-        generic.print_dbg(indentation, "Ternary operator")
-        generic.print_dbg(indentation, "Guard:")
-        self.guard.debug_print(indentation + 2)
-        generic.print_dbg(indentation, "Expression 1:")
-        self.expr1.debug_print(indentation + 2)
-        generic.print_dbg(indentation, "Expression 2:")
-        self.expr2.debug_print(indentation + 2)
-
-    def reduce(self, id_dicts=None, unknown_id_fatal=True):
-        guard = self.guard.reduce(id_dicts)
-        expr1 = self.expr1.reduce(id_dicts)
-        expr2 = self.expr2.reduce(id_dicts)
-        if isinstance(guard, ConstantNumeric):
-            if guard.value != 0:
-                return expr1
+        print indentation*' ' + 'Action2 variable'
+        self.num.debug_print(indentation + 2)
+        if self.param is not None:
+            print (indentation+2)*' ' + 'Parameter:'
+            if isinstance(self.param, basestring):
+                print (indentation+4)*' ' + 'Procedure call:', self.param
             else:
-                return expr2
-        if guard.type() != Type.INTEGER or expr1.type() != Type.INTEGER or expr2.type() != Type.INTEGER:
-            if guard.type() == Type.SPRITEGROUP_REF:
-                raise generic.ProcCallSyntaxError(guard.name, guard.pos)
-            if expr1.type() == Type.SPRITEGROUP_REF:
-                raise generic.ProcCallSyntaxError(expr1.name, expr1.pos)
-            if expr2.type() == Type.SPRITEGROUP_REF:
-                raise generic.ProcCallSyntaxError(expr2.name, expr2.pos)
-            raise generic.ScriptError("All parts of the ternary operator (?:) must be integers.", self.pos)
-        return TernaryOp(guard, expr1, expr2, self.pos)
+                self.param.debug_print(indentation + 4)
+            if len(self.extra_params) > 0: print (indentation+2)*' ' + 'Extra parameters:'
+            for extra_param in self.extra_params:
+                extra_param.debug_print(indentation + 4)
+
+    def __str__(self):
+        num = "0x%02X" % self.num.value if isinstance(self.num, ConstantNumeric) else str(self.num)
+        ret = 'var[%s, %s, %s' % (num, str(self.shift), str(self.mask))
+        if self.param is not None:
+            ret += ', %s' % str(self.param)
+        ret += ']'
+        if self.add is not None:
+            ret = '(%s + %s)' % (ret, self.add)
+        if self.div is not None:
+            ret = '(%s / %s)' % (ret, self.div)
+        if self.mod is not None:
+            ret = '(%s %% %s)' % (ret, self.mod)
+        return ret
+
+    def reduce(self, id_dicts = [], unknown_id_fatal = True):
+        num = self.num.reduce(id_dicts)
+        shift = self.shift.reduce(id_dicts)
+        mask = self.mask.reduce(id_dicts)
+        param = self.param.reduce(id_dicts) if self.param is not None else None
+        if not all(map(lambda x: x.type() == Type.INTEGER, (num, shift, mask))) or \
+                (param is not None and param.type() != Type.INTEGER):
+            raise generic.ScriptError("All parts of a variable access must be integers.", self.pos)
+        var = Variable(num, shift, mask, param, self.pos)
+        var.add = None if self.add is None else self.add.reduce(id_dicts)
+        var.div = None if self.div is None else self.div.reduce(id_dicts)
+        var.mod = None if self.mod is None else self.mod.reduce(id_dicts)
+        var.extra_params = [(extra_param[0], extra_param[1].reduce(id_dicts)) for extra_param in self.extra_params]
+        return var
 
     def supported_by_action2(self, raise_error):
-        return (
-            self.guard.supported_by_action2(raise_error)
-            and self.expr1.supported_by_action2(raise_error)
-            and self.expr2.supported_by_action2(raise_error)
-        )
+        return True
 
     def supported_by_actionD(self, raise_error):
-        return (
-            self.guard.supported_by_actionD(raise_error)
-            and self.expr1.supported_by_actionD(raise_error)
-            and self.expr2.supported_by_actionD(raise_error)
-        )
-
-    def collect_references(self):
-        return self.guard.collect_references() + self.expr1.collect_references() + self.expr2.collect_references()
-
-    def is_read_only(self):
-        return self.guard.is_read_only() and self.expr1.is_read_only() and self.expr2.is_read_only()
-
-    def is_boolean(self):
-        return self.expr1.is_boolean() and self.expr2.is_boolean()
-
-    def __eq__(self, other):
-        return (
-            other is not None
-            and isinstance(other, TernaryOp)
-            and self.guard == other.guard
-            and self.expr1 == other.expr1
-            and self.expr2 == other.expr2
-        )
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
-        return hash((self.guard, self.expr1, self.expr2))
-
-    def __str__(self):
-        return "({} ? {} : {})".format(str(self.guard), str(self.expr1), str(self.expr2))
+        if raise_error:
+            if isinstance(self.num, ConstantNumeric):
+                if self.num.value == 0x7C: raise generic.ScriptError("LOAD_PERM is only available in switch-blocks.", self.pos)
+                if self.num.value == 0x7D: raise generic.ScriptError("LOAD_TEMP is only available in switch-blocks.", self.pos)
+            raise generic.ScriptError("Variable accesses are not supported outside of switch-blocks.", self.pos)
+        return False
```

### Comparing `nml-0.7.2/nml/palette.py` & `nml-r1512/nml/palette.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,308 +1,289 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
 from nml import generic
 
-# fmt: off
 raw_palette_data = [
-    # DOS palette
-    [
-         0,   0, 255,     16,  16,  16,     32,  32,  32,     48,  48,  48,
-        64,  64,  64,     80,  80,  80,    100, 100, 100,    116, 116, 116,
-       132, 132, 132,    148, 148, 148,    168, 168, 168,    184, 184, 184,
-       200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
-        52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
-       132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
-        48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
-       120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
-        72,  44,   4,     88,  60,  20,    104,  80,  44,    124, 104,  72,
-       152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
-        64,   0,   4,     88,   4,  16,    112,  16,  32,    136,  32,  52,
-       160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
-       236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
-       252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
-       136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
-        68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
-       184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
-       252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
-        84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
-       168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
-         8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
-        64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
-        28,  52,  24,     44,  68,  32,     60,  88,  48,     80, 104,  60,
-       104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
-        16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
-        96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
-        32,  24,   0,     56,  28,   0,     72,  40,   4,     88,  52,  12,
-       104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
-        76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
-       164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
-       224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
-       120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
-        36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
-       100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
-        40,  20, 112,     64,  44, 144,     88,  64, 172,    104,  76, 196,
-       120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
-         0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
-         0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
-       128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
-        40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
-       156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
-       252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
-       252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
-       112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
-       208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
-       128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
-       252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
-       252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
-       204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
-       252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
-        20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
-        72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
-       124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
-       180, 220, 236,    132, 188, 216,     88, 152, 172,    244,   0, 244,
-       245,   0, 245,    246,   0, 246,    247,   0, 247,    248,   0, 248,
-       249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
-       253,   0, 253,    254,   0, 254,    255,   0, 255,     76,  24,   8,
-       108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
-       252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
-       252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
-       255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
-       255, 255,   0,     32,  68, 112,     36,  72, 116,     40,  76, 120,
-        44,  80, 124,     48,  84, 128,     72, 100, 144,    100, 132, 168,
-       216, 244, 252,     96, 128, 164,     68,  96, 140,    255, 255, 255
-    ],  # end of DOS palette
-
-    # Windows palette
-    [
-         0,   0, 255,    238,   0, 238,    239,   0, 239,    240,   0, 240,
-       241,   0, 241,    242,   0, 242,    243,   0, 243,    244,   0, 244,
-       245,   0, 245,    246,   0, 246,    168, 168, 168,    184, 184, 184,
-       200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
-        52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
-       132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
-        48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
-       120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
-       100, 100, 100,    116, 116, 116,    104,  80,  44,    124, 104,  72,
-       152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
-       132, 132, 132,     88,   4,  16,    112,  16,  32,    136,  32,  52,
-       160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
-       236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
-       252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
-       136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
-        68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
-       184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
-       252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
-        84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
-       168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
-         8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
-        64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
-        64,  64,  64,     44,  68,  32,     60,  88,  48,     80, 104,  60,
-       104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
-        16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
-        96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
-        32,  24,   0,     56,  28,   0,     80,  80,  80,     88,  52,  12,
-       104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
-        76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
-       164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
-       224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
-       120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
-        36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
-       100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
-        48,  48,  48,     64,  44, 144,     88,  64, 172,    104,  76, 196,
-       120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
-         0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
-         0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
-       128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
-        40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
-       156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
-       252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
-       252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
-       112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
-       208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
-       128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
-       252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
-       252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
-       204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
-       252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
-        20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
-        72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
-       124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
-       180, 220, 236,    132, 188, 216,     88, 152, 172,     16,  16,  16,
-        32,  32,  32,     32,  68, 112,     36,  72, 116,     40,  76, 120,
-        44,  80, 124,     48,  84, 128,     72, 100, 144,    100, 132, 168,
-       216, 244, 252,     96, 128, 164,     68,  96, 140,     76,  24,   8,
-       108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
-       252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
-       252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
-       255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
-       255, 255,   0,    148, 148, 148,    247,   0, 247,    248,   0, 248,
-       249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
-       253,   0, 253,    254,   0, 254,    255,   0, 255,    255, 255, 255
-    ],  # end of Windows palette
-
-    # DOS Toyland palette
-    [
-          0,   0, 255,     16,  16,  16,     32,  32,  32,     48,  48,  48,
-         64,  64,  64,     80,  80,  80,    100, 100, 100,    116, 116, 116,
-        132, 132, 132,    148, 148, 148,    168, 168, 168,    184, 184, 184,
-        200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
-         52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
-        132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
-         48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
-        120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
-         72,  44,   4,     88,  60,  20,    104,  80,  44,    124, 104,  72,
-        152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
-         64,   0,   4,     88,   4,  16,    112,  16,  32,    136,  32,  52,
-        160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
-        236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
-        252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
-        136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
-         68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
-        184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
-        252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
-         84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
-        168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
-          8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
-         64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
-         28,  52,  24,     44,  68,  32,     60,  88,  48,     80, 104,  60,
-        104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
-         16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
-         96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
-         32,  24,   0,     56,  28,   0,     72,  40,   4,     88,  52,  12,
-        104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
-         76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
-        164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
-        224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
-        120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
-         36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
-        100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
-         40,  20, 112,     64,  44, 144,     88,  64, 172,    104,  76, 196,
-        120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
-          0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
-          0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
-        128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
-         40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
-        156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
-        252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
-        252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
-        112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
-        208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
-        128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
-        252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
-        252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
-        204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
-        252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
-         20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
-         72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
-        124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
-        180, 220, 236,    132, 188, 216,     88, 152, 172,    244,   0, 244,
-        245,   0, 245,    246,   0, 246,    247,   0, 247,    248,   0, 248,
-        249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
-        253,   0, 253,    254,   0, 254,    255,   0, 255,     76,  24,   8,
-        108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
-        252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
-        252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
-        255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
-        255, 255,   0,     28, 108, 124,     32, 112, 128,     36, 116, 132,
-         40, 120, 136,     44, 124, 140,     92, 164, 184,    116, 180, 196,
-        216, 244, 252,    112, 176, 192,     88, 160, 180,    255, 255, 255
-    ],  # end of DOS Toyland palette
-
-    # Windows Toyland palette
-    [
-          0, 255, 255,    238,   0, 238,    239,   0, 239,    240,   0, 240,
-        241,   0, 241,    242,   0, 242,    243,   0, 243,    244,   0, 244,
-        245,   0, 245,    246,   0, 246,    168, 168, 168,    184, 184, 184,
-        200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
-         52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
-        132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
-         48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
-        120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
-        100, 100, 100,    116, 116, 116,    104,  80,  44,    124, 104,  72,
-        152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
-        132, 132, 132,     88,   4,  16,    112,  16,  32,    136,  32,  52,
-        160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
-        236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
-        252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
-        136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
-         68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
-        184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
-        252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
-         84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
-        168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
-          8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
-         64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
-         64,  64,  64,     44,  68,  32,     60,  88,  48,     80, 104,  60,
-        104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
-         16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
-         96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
-         32,  24,   0,     56,  28,   0,     80,  80,  80,     88,  52,  12,
-        104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
-         76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
-        164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
-        224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
-        120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
-         36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
-        100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
-         48,  48,  48,     64,  44, 144,     88,  64, 172,    104,  76, 196,
-        120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
-          0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
-          0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
-        128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
-         40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
-        156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
-        252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
-        252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
-        112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
-        208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
-        128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
-        252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
-        252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
-        204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
-        252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
-         20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
-         72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
-        124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
-        180, 220, 236,    132, 188, 216,     88, 152, 172,     16,  16,  16,
-         32,  32,  32,     28, 108, 124,     32, 112, 128,     36, 116, 132,
-         40, 120, 136,     44, 124, 140,     92, 164, 184,    116, 180, 196,
-        216, 244, 252,    112, 176, 192,     88, 160, 180,     76,  24,   8,
-        108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
-        252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
-        252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
-        255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
-        255, 255,   0,    148, 148, 148,    247,   0, 247,    248,   0, 248,
-        249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
-        253,   0, 253,    254,   0, 254,    255,   0, 255,    255, 255, 255
-    ],  # end of Windows Toyland palette
+#DOS palette
+[
+     0,   0, 255,     16,  16,  16,     32,  32,  32,     48,  48,  48,
+    64,  64,  64,     80,  80,  80,    100, 100, 100,    116, 116, 116,
+   132, 132, 132,    148, 148, 148,    168, 168, 168,    184, 184, 184,
+   200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
+    52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
+   132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
+    48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
+   120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
+    72,  44,   4,     88,  60,  20,    104,  80,  44,    124, 104,  72,
+   152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
+    64,   0,   4,     88,   4,  16,    112,  16,  32,    136,  32,  52,
+   160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
+   236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
+   252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
+   136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
+    68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
+   184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
+   252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
+    84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
+   168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
+     8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
+    64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
+    28,  52,  24,     44,  68,  32,     60,  88,  48,     80, 104,  60,
+   104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
+    16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
+    96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
+    32,  24,   0,     56,  28,   0,     72,  40,   4,     88,  52,  12,
+   104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
+    76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
+   164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
+   224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
+   120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
+    36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
+   100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
+    40,  20, 112,     64,  44, 144,     88,  64, 172,    104,  76, 196,
+   120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
+     0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
+     0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
+   128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
+    40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
+   156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
+   252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
+   252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
+   112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
+   208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
+   128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
+   252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
+   252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
+   204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
+   252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
+    20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
+    72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
+   124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
+   180, 220, 236,    132, 188, 216,     88, 152, 172,    244,   0, 244,
+   245,   0, 245,    246,   0, 246,    247,   0, 247,    248,   0, 248,
+   249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
+   253,   0, 253,    254,   0, 254,    255,   0, 255,     76,  24,   8,
+   108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
+   252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
+   252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
+   255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
+   255, 255,   0,     32,  68, 112,     36,  72, 116,     40,  76, 120,
+    44,  80, 124,     48,  84, 128,     72, 100, 144,    100, 132, 168,
+   216, 244, 252,     96, 128, 164,     68,  96, 140,    255, 255, 255
+], #end of DOS palette
+
+#Windows palette
+[
+     0,   0, 255,    238,   0, 238,    239,   0, 239,    240,   0, 240,
+   241,   0, 241,    242,   0, 242,    243,   0, 243,    244,   0, 244,
+   245,   0, 245,    246,   0, 246,    168, 168, 168,    184, 184, 184,
+   200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
+    52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
+   132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
+    48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
+   120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
+   100, 100, 100,    116, 116, 116,    104,  80,  44,    124, 104,  72,
+   152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
+   132, 132, 132,     88,   4,  16,    112,  16,  32,    136,  32,  52,
+   160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
+   236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
+   252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
+   136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
+    68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
+   184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
+   252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
+    84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
+   168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
+     8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
+    64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
+    64,  64,  64,     44,  68,  32,     60,  88,  48,     80, 104,  60,
+   104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
+    16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
+    96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
+    32,  24,   0,     56,  28,   0,     80,  80,  80,     88,  52,  12,
+   104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
+    76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
+   164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
+   224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
+   120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
+    36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
+   100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
+    48,  48,  48,     64,  44, 144,     88,  64, 172,    104,  76, 196,
+   120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
+     0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
+     0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
+   128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
+    40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
+   156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
+   252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
+   252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
+   112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
+   208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
+   128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
+   252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
+   252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
+   204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
+   252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
+    20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
+    72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
+   124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
+   180, 220, 236,    132, 188, 216,     88, 152, 172,     16,  16,  16,
+    32,  32,  32,     32,  68, 112,     36,  72, 116,     40,  76, 120,
+    44,  80, 124,     48,  84, 128,     72, 100, 144,    100, 132, 168,
+   216, 244, 252,     96, 128, 164,     68,  96, 140,     76,  24,   8,
+   108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
+   252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
+   252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
+   255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
+   255, 255,   0,    148, 148, 148,    247,   0, 247,    248,   0, 248,
+   249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
+   253,   0, 253,    254,   0, 254,    255,   0, 255,    255, 255, 255
+], #end of Windows palette
+
+# DOS Toyland palette
+[
+      0,   0, 255,     16,  16,  16,     32,  32,  32,     48,  48,  48,
+     64,  64,  64,     80,  80,  80,    100, 100, 100,    116, 116, 116,
+    132, 132, 132,    148, 148, 148,    168, 168, 168,    184, 184, 184,
+    200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
+     52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
+    132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
+     48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
+    120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
+     72,  44,   4,     88,  60,  20,    104,  80,  44,    124, 104,  72,
+    152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
+     64,   0,   4,     88,   4,  16,    112,  16,  32,    136,  32,  52,
+    160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
+    236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
+    252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
+    136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
+     68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
+    184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
+    252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
+     84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
+    168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
+      8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
+     64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
+     28,  52,  24,     44,  68,  32,     60,  88,  48,     80, 104,  60,
+    104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
+     16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
+     96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
+     32,  24,   0,     56,  28,   0,     72,  40,   4,     88,  52,  12,
+    104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
+     76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
+    164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
+    224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
+    120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
+     36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
+    100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
+     40,  20, 112,     64,  44, 144,     88,  64, 172,    104,  76, 196,
+    120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
+      0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
+      0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
+    128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
+     40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
+    156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
+    252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
+    252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
+    112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
+    208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
+    128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
+    252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
+    252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
+    204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
+    252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
+     20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
+     72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
+    124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
+    180, 220, 236,    132, 188, 216,     88, 152, 172,    244,   0, 244,
+    245,   0, 245,    246,   0, 246,    247,   0, 247,    248,   0, 248,
+    249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
+    253,   0, 253,    254,   0, 254,    255,   0, 255,     76,  24,   8,
+    108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
+    252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
+    252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
+    255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
+    255, 255,   0,     28, 108, 124,     32, 112, 128,     36, 116, 132,
+     40, 120, 136,     44, 124, 140,     92, 164, 184,    116, 180, 196,
+    216, 244, 252,    112, 176, 192,     88, 160, 180,    255, 255, 255
+], #end of DOS Toyland palette
+
+#Windows Toyland palette
+[
+      0, 255, 255,    238,   0, 238,    239,   0, 239,    240,   0, 240,
+    241,   0, 241,    242,   0, 242,    243,   0, 243,    244,   0, 244,
+    245,   0, 245,    246,   0, 246,    168, 168, 168,    184, 184, 184,
+    200, 200, 200,    216, 216, 216,    232, 232, 232,    252, 252, 252,
+     52,  60,  72,     68,  76,  92,     88,  96, 112,    108, 116, 132,
+    132, 140, 152,    156, 160, 172,    176, 184, 196,    204, 208, 220,
+     48,  44,   4,     64,  60,  12,     80,  76,  20,     96,  92,  28,
+    120, 120,  64,    148, 148, 100,    176, 176, 132,    204, 204, 168,
+    100, 100, 100,    116, 116, 116,    104,  80,  44,    124, 104,  72,
+    152, 132,  92,    184, 160, 120,    212, 188, 148,    244, 220, 176,
+    132, 132, 132,     88,   4,  16,    112,  16,  32,    136,  32,  52,
+    160,  56,  76,    188,  84, 108,    204, 104, 124,    220, 132, 144,
+    236, 156, 164,    252, 188, 192,    252, 208,   0,    252, 232,  60,
+    252, 252, 128,     76,  40,   0,     96,  60,   8,    116,  88,  28,
+    136, 116,  56,    156, 136,  80,    176, 156, 108,    196, 180, 136,
+     68,  24,   0,     96,  44,   4,    128,  68,   8,    156,  96,  16,
+    184, 120,  24,    212, 156,  32,    232, 184,  16,    252, 212,   0,
+    252, 248, 128,    252, 252, 192,     32,   4,   0,     64,  20,   8,
+     84,  28,  16,    108,  44,  28,    128,  56,  40,    148,  72,  56,
+    168,  92,  76,    184, 108,  88,    196, 128, 108,    212, 148, 128,
+      8,  52,   0,     16,  64,   0,     32,  80,   4,     48,  96,   4,
+     64, 112,  12,     84, 132,  20,    104, 148,  28,    128, 168,  44,
+     64,  64,  64,     44,  68,  32,     60,  88,  48,     80, 104,  60,
+    104, 124,  76,    128, 148,  92,    152, 176, 108,    180, 204, 124,
+     16,  52,  24,     32,  72,  44,     56,  96,  72,     76, 116,  88,
+     96, 136, 108,    120, 164, 136,    152, 192, 168,    184, 220, 200,
+     32,  24,   0,     56,  28,   0,     80,  80,  80,     88,  52,  12,
+    104,  64,  24,    124,  84,  44,    140, 108,  64,    160, 128,  88,
+     76,  40,  16,     96,  52,  24,    116,  68,  40,    136,  84,  56,
+    164,  96,  64,    184, 112,  80,    204, 128,  96,    212, 148, 112,
+    224, 168, 128,    236, 188, 148,     80,  28,   4,    100,  40,  20,
+    120,  56,  40,    140,  76,  64,    160, 100,  96,    184, 136, 136,
+     36,  40,  68,     48,  52,  84,     64,  64, 100,     80,  80, 116,
+    100, 100, 136,    132, 132, 164,    172, 172, 192,    212, 212, 224,
+     48,  48,  48,     64,  44, 144,     88,  64, 172,    104,  76, 196,
+    120,  88, 224,    140, 104, 252,    160, 136, 252,    188, 168, 252,
+      0,  24, 108,      0,  36, 132,      0,  52, 160,      0,  72, 184,
+      0,  96, 212,     24, 120, 220,     56, 144, 232,     88, 168, 240,
+    128, 196, 252,    188, 224, 252,     16,  64,  96,     24,  80, 108,
+     40,  96, 120,     52, 112, 132,     80, 140, 160,    116, 172, 192,
+    156, 204, 220,    204, 240, 252,    172,  52,  52,    212,  52,  52,
+    252,  52,  52,    252, 100,  88,    252, 144, 124,    252, 184, 160,
+    252, 216, 200,    252, 244, 236,     72,  20, 112,     92,  44, 140,
+    112,  68, 168,    140, 100, 196,    168, 136, 224,    200, 176, 248,
+    208, 184, 255,    232, 208, 252,     60,   0,   0,     92,   0,   0,
+    128,   0,   0,    160,   0,   0,    196,   0,   0,    224,   0,   0,
+    252,   0,   0,    252,  80,   0,    252, 108,   0,    252, 136,   0,
+    252, 164,   0,    252, 192,   0,    252, 220,   0,    252, 252,   0,
+    204, 136,   8,    228, 144,   4,    252, 156,   0,    252, 176,  48,
+    252, 196, 100,    252, 216, 152,      8,  24,  88,     12,  36, 104,
+     20,  52, 124,     28,  68, 140,     40,  92, 164,     56, 120, 188,
+     72, 152, 216,    100, 172, 224,     92, 156,  52,    108, 176,  64,
+    124, 200,  76,    144, 224,  92,    224, 244, 252,    200, 236, 248,
+    180, 220, 236,    132, 188, 216,     88, 152, 172,     16,  16,  16,
+     32,  32,  32,     28, 108, 124,     32, 112, 128,     36, 116, 132,
+     40, 120, 136,     44, 124, 140,     92, 164, 184,    116, 180, 196,
+    216, 244, 252,    112, 176, 192,     88, 160, 180,     76,  24,   8,
+    108,  44,  24,    144,  72,  52,    176, 108,  84,    210, 146, 126,
+    252,  60,   0,    252,  84,   0,    252, 104,   0,    252, 124,   0,
+    252, 148,   0,    252, 172,   0,    252, 196,   0,     64,   0,   0,
+    255,   0,   0,     48,  48,   0,     64,  64,   0,     80,  80,   0,
+    255, 255,   0,    148, 148, 148,    247,   0, 247,    248,   0, 248,
+    249,   0, 249,    250,   0, 250,    251,   0, 251,    252,   0, 252,
+    253,   0, 253,    254,   0, 254,    255,   0, 255,    255, 255, 255
+] #end of Windows Toyland palette
 ]
-# fmt: on
-
-# Convert palettes to strings for fast comparison.
-palette_data = [bytes(pal) for pal in raw_palette_data]
 
-palette_name = ["DEFAULT", "LEGACY", "DEFAULT_TOYLAND", "LEGACY_TOYLAND"]
+#Convert palettes to strings for fast comparision
+palette_data = [''.join([chr(c) for c in pal]) for pal in raw_palette_data]
 
+palette_name = ["DOS", "WIN", "DOS_TOYLAND", "WIN_TOYLAND"]
 
 def validate_palette(image, filename):
     palette = image.palette.palette
     if len(palette) != 768:
         raise generic.ImageError("Invalid palette; does not contain 256 entries.", filename)
     for i, pal in enumerate(palette_data):
-        if pal != palette:
-            continue
+        if pal != palette: continue
         return palette_name[i]
     raise generic.ImageError("Palette is not recognized as a valid palette.", filename)
```

### Comparing `nml-0.7.2/nml/parser.py` & `nml-r1512/nml/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,841 +1,658 @@
-__license__ = """
-NML is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2 of the License, or
-(at your option) any later version.
-
-NML is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along
-with NML; if not, write to the Free Software Foundation, Inc.,
-51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA."""
-
+from nml import generic, expression, tokens, nmlop
+from nml.ast import assignment, basecost, cargotable, conditional, deactivate, disable_item, error, font, general, grf, item, loop, produce, railtypetable, replace, spriteblock, switch, switch_range, townnames, snowline, skipall, tilelayout, alt_sprites, base_sprites, override
+from nml.actions import action2, action2random, actionD, real_sprite
 import ply.yacc as yacc
 
-from nml import expression, generic, nmlop, tokens, unit
-from nml.actions import actionD, real_sprite
-from nml.ast import (
-    alt_sprites,
-    assignment,
-    base_graphics,
-    basecost,
-    cargotable,
-    conditional,
-    deactivate,
-    disable_item,
-    error,
-    font,
-    general,
-    grf,
-    item,
-    loop,
-    override,
-    produce,
-    replace,
-    skipall,
-    snowline,
-    sort_vehicles,
-    spriteblock,
-    switch,
-    tilelayout,
-    townnames,
-    tracktypetable,
-)
-
-
-class NMLParser:
-    """
-    @ivar lexer: Scanner providing tokens.
-    @type lexer: L{NMLLexer}
-
-    @ivar tokens: Tokens of the scanner (used by PLY).
-    @type tokens: C{List} of C{str}
-
-    @ivar parser: PLY parser.
-    @type parser: L{ply.yacc}
-    """
-
-    def __init__(self, rebuild=False, debug=False):
-        if debug:
-            try:
-                import os
-
-                os.remove(os.path.normpath(os.path.join(os.path.dirname(__file__), "generated", "parsetab.py")))
-            except FileNotFoundError:
-                # Tried to remove a non existing file
-                pass
+class NMLParser(object):
+    def __init__(self):
         self.lexer = tokens.NMLLexer()
-        self.lexer.build(rebuild or debug)
+        self.lexer.build()
         self.tokens = self.lexer.tokens
-        self.parser = yacc.yacc(
-            module=self,
-            debug=debug,
-            optimize=not (rebuild or debug),
-            write_tables=not debug,
-            tabmodule="nml.generated.parsetab",
-        )
-
-    def parse(self, text, input_filename):
-        self.lexer.setup(text, input_filename)
-        return self.parser.parse(None, lexer=self.lexer.lexer)
+        self.parser = yacc.yacc(debug = False, module = self)
+
+    def parse(self, text):
+        return self.parser.parse(text, lexer = self.lexer.lexer)
+
 
-    # operator precedence (lower in the list = higher priority)
+    #operator precedence (lower in the list = higher priority)
     precedence = (
-        ("left", "COMMA"),
-        ("right", "TERNARY_OPEN", "COLON"),
-        ("left", "LOGICAL_OR"),
-        ("left", "LOGICAL_AND"),
-        ("left", "OR"),
-        ("left", "XOR"),
-        ("left", "AND"),
-        ("left", "COMP_EQ", "COMP_NEQ", "COMP_LE", "COMP_GE", "COMP_LT", "COMP_GT"),
-        ("left", "SHIFT_LEFT", "SHIFT_RIGHT", "SHIFTU_RIGHT"),
-        ("left", "PLUS", "MINUS"),
-        ("left", "TIMES", "DIVIDE", "MODULO"),
-        ("left", "LOGICAL_NOT", "BINARY_NOT"),
+        ('left','COMMA'),
+        ('right','TERNARY_OPEN','COLON'),
+        ('left','LOGICAL_OR'),
+        ('left','LOGICAL_AND'),
+        ('left','OR'),
+        ('left','XOR'),
+        ('left','AND'),
+        ('left','COMP_EQ','COMP_NEQ','COMP_LE','COMP_GE','COMP_LT','COMP_GT'),
+        ('left','SHIFT_LEFT','SHIFT_RIGHT','SHIFTU_RIGHT'),
+        ('left','PLUS','MINUS'),
+        ('left','TIMES','DIVIDE','MODULO'),
+        ('left','LOGICAL_NOT','BINARY_NOT'),
     )
 
     def p_error(self, t):
         if t is None:
-            raise generic.ScriptError("Syntax error, unexpected end-of-file")
+            raise generic.ScriptError('Syntax error, unexpected end-of-file')
         else:
-            raise generic.ScriptError('Syntax error, unexpected token "{}"'.format(t.value), t.lineno)
+            raise generic.ScriptError('Syntax error, unexpected token "%s"' % t.value, t.lineno)
+
 
     #
     # Main script blocks
     #
     def p_main_script(self, t):
-        "main_script : script"
+        'main_script : script'
         t[0] = general.MainScript(t[1])
 
     def p_script(self, t):
-        """script :
-        | script main_block"""
-        if len(t) == 1:
-            t[0] = []
-        else:
-            t[0] = t[1] + [t[2]]
+        '''script :
+                  | script main_block'''
+        if len(t) == 1: t[0] = []
+        else: t[0] = t[1] + [t[2]]
 
     def p_main_block(self, t):
-        """main_block : switch
-        | random_switch
-        | produce
-        | spriteset
-        | spritegroup
-        | spritelayout
-        | template_declaration
-        | tilelayout
-        | town_names
-        | cargotable
-        | railtype
-        | roadtype
-        | tramtype
-        | grf_block
-        | param_assignment
-        | skip_all
-        | conditional
-        | loop
-        | item
-        | property_block
-        | graphics_block
-        | liveryoverride_block
-        | error_block
-        | disable_item
-        | deactivate
-        | replace
-        | replace_new
-        | base_graphics
-        | font_glyph
-        | alt_sprites
-        | snowline
-        | engine_override
-        | sort_vehicles
-        | basecost"""
+        '''main_block : switch
+                      | random_switch
+                      | produce
+                      | spriteset
+                      | spritegroup
+                      | spritelayout
+                      | template_declaration
+                      | tilelayout
+                      | town_names
+                      | cargotable
+                      | railtype
+                      | grf_block
+                      | param_assignment
+                      | skip_all
+                      | conditional
+                      | loop
+                      | item
+                      | property_block
+                      | graphics_block
+                      | liveryoverride_block
+                      | error_block
+                      | disable_item
+                      | deactivate
+                      | replace
+                      | replace_new
+                      | base_sprites
+                      | font_glyph
+                      | alt_sprites
+                      | snowline
+                      | engine_override
+                      | basecost'''
         t[0] = t[1]
 
     #
     # Expressions
     #
     def p_expression(self, t):
-        """expression : NUMBER
-        | FLOAT
-        | param
-        | variable
-        | ID
-        | STRING_LITERAL
-        | string"""
+        '''expression : NUMBER
+                      | FLOAT
+                      | param
+                      | variable
+                      | ID
+                      | STRING_LITERAL
+                      | string'''
         t[0] = t[1]
 
     def p_parenthesed_expression(self, t):
-        "expression : LPAREN expression RPAREN"
+        'expression : LPAREN expression RPAREN'
         t[0] = t[2]
 
     def p_parameter(self, t):
-        "param : PARAMETER LBRACKET expression RBRACKET"
+        'param : PARAMETER LBRACKET expression RBRACKET'
         t[0] = expression.Parameter(t[3], t.lineno(1), True)
 
     def p_parameter_other_grf(self, t):
-        "param : PARAMETER LBRACKET expression COMMA expression RBRACKET"
+        'param : PARAMETER LBRACKET expression COMMA expression RBRACKET'
         t[0] = expression.OtherGRFParameter(t[3], t[5], t.lineno(1))
 
     code_to_op = {
-        "+": nmlop.ADD,
-        "-": nmlop.SUB,
-        "*": nmlop.MUL,
-        "/": nmlop.DIV,
-        "%": nmlop.MOD,
-        "&": nmlop.AND,
-        "|": nmlop.OR,
-        "^": nmlop.XOR,
-        "&&": nmlop.AND,
-        "||": nmlop.OR,
-        "==": nmlop.CMP_EQ,
-        "!=": nmlop.CMP_NEQ,
-        "<=": nmlop.CMP_LE,
-        ">=": nmlop.CMP_GE,
-        "<": nmlop.CMP_LT,
-        ">": nmlop.CMP_GT,
-        "<<": nmlop.SHIFT_LEFT,
-        ">>": nmlop.SHIFT_RIGHT,
-        ">>>": nmlop.SHIFTU_RIGHT,
+        '+'  : nmlop.ADD,
+        '-'  : nmlop.SUB,
+        '*'  : nmlop.MUL,
+        '/'  : nmlop.DIV,
+        '%'  : nmlop.MOD,
+        '&'  : nmlop.AND,
+        '|'  : nmlop.OR,
+        '^'  : nmlop.XOR,
+        '&&' : nmlop.AND,
+        '||' : nmlop.OR,
+        '==' : nmlop.CMP_EQ,
+        '!=' : nmlop.CMP_NEQ,
+        '<=' : nmlop.CMP_LE,
+        '>=' : nmlop.CMP_GE,
+        '<'  : nmlop.CMP_LT,
+        '>'  : nmlop.CMP_GT,
+        '<<' : nmlop.SHIFT_LEFT,
+        '>>' : nmlop.SHIFT_RIGHT,
+        '>>>': nmlop.SHIFTU_RIGHT,
     }
 
     def p_binop(self, t):
-        """expression : expression PLUS expression
-        | expression MINUS expression
-        | expression TIMES expression
-        | expression DIVIDE expression
-        | expression MODULO expression
-        | expression AND expression
-        | expression OR expression
-        | expression XOR expression
-        | expression SHIFT_LEFT expression
-        | expression SHIFT_RIGHT expression
-        | expression SHIFTU_RIGHT expression
-        | expression COMP_EQ expression
-        | expression COMP_NEQ expression
-        | expression COMP_LE expression
-        | expression COMP_GE expression
-        | expression COMP_LT expression
-        | expression COMP_GT expression"""
+        '''expression : expression PLUS expression
+                      | expression MINUS expression
+                      | expression TIMES expression
+                      | expression DIVIDE expression
+                      | expression MODULO expression
+                      | expression AND expression
+                      | expression OR expression
+                      | expression XOR expression
+                      | expression SHIFT_LEFT expression
+                      | expression SHIFT_RIGHT expression
+                      | expression SHIFTU_RIGHT expression
+                      | expression COMP_EQ expression
+                      | expression COMP_NEQ expression
+                      | expression COMP_LE expression
+                      | expression COMP_GE expression
+                      | expression COMP_LT expression
+                      | expression COMP_GT expression'''
         t[0] = expression.BinOp(self.code_to_op[t[2]], t[1], t[3], t[1].pos)
 
     def p_binop_logical(self, t):
-        """expression : expression LOGICAL_AND expression
-        | expression LOGICAL_OR expression"""
+        '''expression : expression LOGICAL_AND expression
+                      | expression LOGICAL_OR expression'''
         t[0] = expression.BinOp(self.code_to_op[t[2]], expression.Boolean(t[1]), expression.Boolean(t[3]), t[1].pos)
 
     def p_logical_not(self, t):
-        "expression : LOGICAL_NOT expression"
+        'expression : LOGICAL_NOT expression'
         t[0] = expression.Not(expression.Boolean(t[2]), t.lineno(1))
 
     def p_binary_not(self, t):
-        "expression : BINARY_NOT expression"
+        'expression : BINARY_NOT expression'
         t[0] = expression.BinNot(t[2], t.lineno(1))
 
     def p_ternary_op(self, t):
-        "expression : expression TERNARY_OPEN expression COLON expression"
+        'expression : expression TERNARY_OPEN expression COLON expression'
         t[0] = expression.TernaryOp(t[1], t[3], t[5], t[1].pos)
 
     def p_unary_minus(self, t):
-        "expression : MINUS expression"
-        t[0] = nmlop.SUB(0, t[2], t.lineno(1))
+        'expression : MINUS expression'
+        t[0] = expression.BinOp(self.code_to_op[t[1]], expression.ConstantNumeric(0), t[2], t.lineno(1))
 
     def p_variable(self, t):
-        "variable : VARIABLE LBRACKET expression_list RBRACKET"
+        'variable : VARIABLE LBRACKET expression_list RBRACKET'
         t[0] = expression.Variable(*t[3])
         t[0].pos = t.lineno(1)
 
     def p_function(self, t):
-        "expression : ID LPAREN expression_list RPAREN"
+        'expression : ID LPAREN expression_list RPAREN'
         t[0] = expression.FunctionCall(t[1], t[3], t[1].pos)
 
     def p_array(self, t):
-        "expression : LBRACKET expression_list RBRACKET"
+        'expression : LBRACKET expression_list RBRACKET'
         t[0] = expression.Array(t[2], t.lineno(1))
 
+
     #
     # Commonly used non-terminals that are not expressions
     #
     def p_assignment_list(self, t):
-        """assignment_list : assignment
-        | param_desc
-        | assignment_list assignment
-        | assignment_list param_desc"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''assignment_list : assignment
+                           | param_desc
+                           | assignment_list assignment
+                           | assignment_list param_desc'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_assignment(self, t):
-        "assignment : ID COLON expression SEMICOLON"
+        'assignment : ID COLON expression SEMICOLON'
         t[0] = assignment.Assignment(t[1], t[3], t[1].pos)
 
     def p_param_desc(self, t):
-        """param_desc : PARAMETER expression LBRACE setting_list RBRACE
-        | PARAMETER LBRACE setting_list RBRACE"""
-        if len(t) == 5:
-            t[0] = grf.ParameterDescription(t[3])
-        else:
-            t[0] = grf.ParameterDescription(t[4], t[2])
+        '''param_desc : PARAMETER expression LBRACE setting_list RBRACE
+                      | PARAMETER LBRACE setting_list RBRACE'''
+        if len(t) == 5: t[0] = grf.ParameterDescription(t[3])
+        else: t[0] = grf.ParameterDescription(t[4], t[2])
 
     def p_setting_list(self, t):
-        """setting_list : setting
-        | setting_list setting"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''setting_list : setting
+                        | setting_list setting'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_setting(self, t):
-        "setting : ID LBRACE setting_value_list RBRACE"
+        'setting : ID LBRACE setting_value_list RBRACE'
         t[0] = grf.ParameterSetting(t[1], t[3])
 
     def p_setting_value_list(self, t):
-        """setting_value_list : setting_value
-        | setting_value_list setting_value"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''setting_value_list : setting_value
+                              | setting_value_list setting_value'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_setting_value(self, t):
-        "setting_value : assignment"
-        t[0] = t[1]
+        'setting_value : assignment'
+        t[0] =  t[1]
 
     def p_names_setting_value(self, t):
-        "setting_value : ID COLON LBRACE name_string_list RBRACE SEMICOLON"
-        t[0] = assignment.Assignment(t[1], t[4], t[1].pos)
+        'setting_value : ID COLON LBRACE name_string_list RBRACE SEMICOLON'
+        t[0] =  assignment.Assignment(t[1], t[4], t[1].pos)
 
     def p_name_string_list(self, t):
-        """name_string_list : name_string_item
-        | name_string_list name_string_item"""
-        if len(t) == 2:
-            t[0] = expression.Array([t[1]], t[1].pos)
-        else:
-            t[0] = expression.Array(t[1].values + [t[2]], t[1].pos)
+        '''name_string_list : name_string_item
+                            | name_string_list name_string_item'''
+        if len(t) == 2: t[0] = expression.Array([t[1]], t[1].pos)
+        else: t[0] = expression.Array(t[1].values + [t[2]], t[1].pos)
 
     def p_name_string_item(self, t):
-        "name_string_item : expression COLON string SEMICOLON"
+        'name_string_item : expression COLON string SEMICOLON'
         t[0] = assignment.Assignment(t[1], t[3], t[1].pos)
 
     def p_string(self, t):
-        "string : STRING LPAREN expression_list RPAREN"
-        t[0] = expression.String(t[3], t.lineno(1))
+        'string : STRING LPAREN expression_list RPAREN'
+        t[0] = expression.String(t[3][0], t[3][1:], t.lineno(1))
 
     def p_non_empty_expression_list(self, t):
-        """non_empty_expression_list : expression
-        | non_empty_expression_list COMMA expression"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[3]]
+        '''non_empty_expression_list : expression
+                                     | non_empty_expression_list COMMA expression'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[3]]
 
     def p_expression_list(self, t):
-        """expression_list :
-        | non_empty_expression_list
-        | non_empty_expression_list COMMA"""
+        '''expression_list :
+                           | non_empty_expression_list
+                           | non_empty_expression_list COMMA'''
         t[0] = [] if len(t) == 1 else t[1]
 
     def p_non_empty_id_list(self, t):
-        """non_empty_id_list : ID
-        | non_empty_id_list COMMA ID"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[3]]
+        '''non_empty_id_list : ID
+                             | non_empty_id_list COMMA ID'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[3]]
 
     def p_id_list(self, t):
-        """id_list :
-        | non_empty_id_list
-        | non_empty_id_list COMMA"""
+        '''id_list :
+                   | non_empty_id_list
+                   | non_empty_id_list COMMA'''
         t[0] = [] if len(t) == 1 else t[1]
 
     def p_generic_assignment(self, t):
-        "generic_assignment : expression COLON expression SEMICOLON"
+        'generic_assignment : expression COLON expression SEMICOLON'
         t[0] = assignment.Assignment(t[1], t[3], t.lineno(1))
 
     def p_generic_assignment_list(self, t):
-        """generic_assignment_list :
-        | generic_assignment_list generic_assignment"""
-        t[0] = [] if len(t) == 1 else t[1] + [t[2]]
-
-    def p_snowline_assignment(self, t):
-        """snowline_assignment : expression COLON expression SEMICOLON
-        | expression COLON expression UNIT SEMICOLON"""
-        unit_value = None if len(t) == 5 else unit.get_unit(t[4])
-        t[0] = assignment.UnitAssignment(t[1], t[3], unit_value, t.lineno(1))
-
-    def p_snowline_assignment_list(self, t):
-        """snowline_assignment_list :
-        | snowline_assignment_list snowline_assignment"""
+        '''generic_assignment_list : 
+                                   | generic_assignment_list generic_assignment'''
         t[0] = [] if len(t) == 1 else t[1] + [t[2]]
 
     #
     # Item blocks
     #
     def p_item(self, t):
-        "item : ITEM LPAREN expression_list RPAREN LBRACE script RBRACE"
+        'item : ITEM LPAREN expression_list RPAREN LBRACE script RBRACE'
         t[0] = item.Item(t[3], t[6], t.lineno(1))
 
     def p_property_block(self, t):
-        "property_block : PROPERTY LBRACE property_list RBRACE"
+        'property_block : PROPERTY LBRACE property_list RBRACE'
         t[0] = item.PropertyBlock(t[3], t.lineno(1))
 
     def p_property_list(self, t):
-        """property_list : property_assignment
-        | property_list property_assignment"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''property_list : property_assignment
+                         | property_list property_assignment'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_property_assignment(self, t):
-        """property_assignment : ID COLON expression SEMICOLON
-        | ID COLON expression UNIT SEMICOLON
-        | NUMBER COLON expression SEMICOLON
-        | NUMBER COLON expression UNIT SEMICOLON"""
+        '''property_assignment : ID COLON expression SEMICOLON
+                               | ID COLON expression UNIT SEMICOLON
+                               | NUMBER COLON expression SEMICOLON
+                               | NUMBER COLON expression UNIT SEMICOLON'''
         name = t[1]
-        unit_value = None if len(t) == 5 else unit.get_unit(t[4])
-        t[0] = item.Property(name, t[3], unit_value, t.lineno(1))
+        unit = None if len(t) == 5 else item.Unit(t[4])
+        t[0] = item.Property(name, t[3], unit, t.lineno(1))
 
     def p_graphics_block(self, t):
-        "graphics_block : GRAPHICS LBRACE graphics_list RBRACE"
+        'graphics_block : GRAPHICS LBRACE graphics_list RBRACE'
         t[0] = item.GraphicsBlock(t[3][0], t[3][1], t.lineno(1))
 
     def p_liveryoverride_block(self, t):
-        "liveryoverride_block : LIVERYOVERRIDE LPAREN expression RPAREN LBRACE graphics_list RBRACE"
+        'liveryoverride_block : LIVERYOVERRIDE LPAREN expression RPAREN LBRACE graphics_list RBRACE'
         t[0] = item.LiveryOverride(t[3], item.GraphicsBlock(t[6][0], t[6][1], t.lineno(1)), t.lineno(1))
 
     def p_graphics_list(self, t):
-        """graphics_list : graphics_assignment_list
-        | graphics_assignment_list switch_value
-        | switch_value"""
+        '''graphics_list : graphics_assignment_list
+                         | graphics_assignment_list expression SEMICOLON
+                         | expression SEMICOLON'''
         # Save graphics block as a tuple, we need to add position info later
         if len(t) == 2:
-            if isinstance(t[1], list):
-                t[0] = (t[1], None)
-            else:
-                t[0] = ([], t[1])
-        else:
+            t[0] = (t[1], None)
+        elif len(t) == 4:
             t[0] = (t[1], t[2])
+        else:
+            t[0] = ([], t[1])
 
     def p_graphics_assignment(self, t):
-        "graphics_assignment : expression COLON switch_value"
+        'graphics_assignment : expression COLON expression SEMICOLON'
         t[0] = item.GraphicsDefinition(t[1], t[3])
 
     def p_graphics_assignment_list(self, t):
-        """graphics_assignment_list : graphics_assignment
-        | graphics_assignment_list graphics_assignment"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''graphics_assignment_list : graphics_assignment
+                                    | graphics_assignment_list graphics_assignment'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     #
     # Program flow control (if/else/while)
     #
     def p_conditional(self, t):
-        """conditional : if_else_parts
-        | if_else_parts else_block"""
+        '''conditional : if_else_parts
+                       | if_else_parts else_block'''
         parts = t[1]
         if len(t) > 2:
             parts.append(t[2])
         t[0] = conditional.ConditionalList(parts)
 
     def p_else_block(self, t):
-        "else_block : ELSE LBRACE script RBRACE"
+        'else_block : ELSE LBRACE script RBRACE'
         t[0] = conditional.Conditional(None, t[3], t.lineno(1))
 
     def p_if_else_parts(self, t):
-        """if_else_parts : IF LPAREN expression RPAREN LBRACE script RBRACE
-        | if_else_parts ELSE IF LPAREN expression RPAREN LBRACE script RBRACE"""
-        if len(t) == 8:
-            t[0] = [conditional.Conditional(t[3], t[6], t.lineno(1))]
-        else:
-            t[0] = t[1] + [conditional.Conditional(t[5], t[8], t.lineno(2))]
+        '''if_else_parts : IF LPAREN expression RPAREN LBRACE script RBRACE
+                         | if_else_parts ELSE IF LPAREN expression RPAREN LBRACE script RBRACE'''
+        if len(t) == 8: t[0] = [conditional.Conditional(t[3], t[6], t.lineno(1))]
+        else: t[0] = t[1] + [conditional.Conditional(t[5], t[8], t.lineno(2))]
 
     def p_loop(self, t):
-        "loop : WHILE LPAREN expression RPAREN LBRACE script RBRACE"
+        'loop : WHILE LPAREN expression RPAREN LBRACE script RBRACE'
         t[0] = loop.Loop(t[3], t[6], t.lineno(1))
 
     #
     # (Random) Switch block
     #
     def p_switch(self, t):
-        "switch : SWITCH LPAREN expression_list RPAREN LBRACE switch_body RBRACE"
-        t[0] = switch.Switch(t[3], t[6], t.lineno(1))
+        'switch : SWITCH LPAREN expression COMMA ID COMMA ID COMMA expression RPAREN LBRACE switch_body RBRACE'
+        t[0] = switch.Switch(t[3], t[5], t[7], t[9], t[12], t.lineno(1))
 
     def p_switch_body(self, t):
-        """switch_body : switch_ranges switch_value
-        | switch_ranges"""
-        t[0] = switch.SwitchBody(t[1], t[2] if len(t) == 3 else None)
+        'switch_body : switch_ranges switch_value'
+        t[0] = switch.SwitchBody(t[1], t[2])
 
     def p_switch_ranges(self, t):
-        """switch_ranges :
-        | switch_ranges expression COLON switch_value
-        | switch_ranges expression UNIT COLON switch_value
-        | switch_ranges expression RANGE expression COLON switch_value
-        | switch_ranges expression RANGE expression UNIT COLON switch_value"""
-        if len(t) == 1:
-            t[0] = []
-        elif len(t) == 5:
-            t[0] = t[1] + [switch.SwitchRange(t[2], t[2], t[4])]
-        elif len(t) == 6:
-            t[0] = t[1] + [switch.SwitchRange(t[2], t[2], t[5], t[3])]
-        elif len(t) == 7:
-            t[0] = t[1] + [switch.SwitchRange(t[2], t[4], t[6])]
-        else:
-            t[0] = t[1] + [switch.SwitchRange(t[2], t[4], t[7], t[5])]
+        '''switch_ranges :
+                         | switch_ranges expression COLON switch_value
+                         | switch_ranges expression UNIT COLON switch_value
+                         | switch_ranges expression RANGE expression COLON switch_value
+                         | switch_ranges expression RANGE expression UNIT COLON switch_value'''
+        if len(t) == 1: t[0] = []
+        elif len(t) == 5: t[0] = t[1] + [switch_range.SwitchRange(t[2], t[2], t[4])]
+        elif len(t) == 6: t[0] = t[1] + [switch_range.SwitchRange(t[2], t[2], t[5], t[3])]
+        elif len(t) == 7: t[0] = t[1] + [switch_range.SwitchRange(t[2], t[4], t[6])]
+        else: t[0] = t[1] + [switch_range.SwitchRange(t[2], t[4], t[7], t[5])]
 
     def p_switch_value(self, t):
-        """switch_value : RETURN expression SEMICOLON
-        | RETURN SEMICOLON
-        | expression SEMICOLON"""
-        if len(t) == 4:
-            t[0] = switch.SwitchValue(t[2], True, t[2].pos)
-        elif t[1] == "return":
-            t[0] = switch.SwitchValue(None, True, t.lineno(1))
-        else:
-            t[0] = switch.SwitchValue(t[1], False, t[1].pos)
+        '''switch_value : RETURN expression SEMICOLON
+                        | RETURN SEMICOLON
+                        | expression SEMICOLON'''
+        if len(t) == 4: t[0] = t[2]
+        elif t[1] == 'return': t[0] = None
+        else: t[0] = t[1]
 
     def p_random_switch(self, t):
-        "random_switch : RANDOMSWITCH LPAREN expression_list RPAREN LBRACE random_body RBRACE"
+        'random_switch : RANDOMSWITCH LPAREN expression_list RPAREN LBRACE random_body RBRACE'
         t[0] = switch.RandomSwitch(t[3], t[6], t.lineno(1))
 
     def p_random_body(self, t):
-        """random_body :
-        | random_body expression COLON switch_value"""
-        if len(t) == 1:
-            t[0] = []
-        else:
-            t[0] = t[1] + [switch.RandomChoice(t[2], t[4])]
-
-    def p_produce_cargo_list(self, t):
-        """produce_cargo_list : LBRACKET RBRACKET
-        | LBRACKET setting_value_list RBRACKET"""
-        if len(t) == 3:
-            t[0] = []
-        else:
-            t[0] = t[2]
+        '''random_body :
+                       | random_body expression COLON switch_value'''
+        if len(t) == 1: t[0] = []
+        else: t[0] = t[1] + [action2random.RandomChoice(t[2], t[4])]
 
     def p_produce(self, t):
-        """produce : PRODUCE LPAREN ID COMMA expression_list RPAREN SEMICOLON
-        | PRODUCE LPAREN ID COMMA produce_cargo_list COMMA produce_cargo_list COMMA expression RPAREN
-        | PRODUCE LPAREN ID COMMA produce_cargo_list COMMA produce_cargo_list RPAREN"""
-        if len(t) == 8:
-            t[0] = produce.ProduceOld([t[3]] + t[5], t.lineno(1))
-        elif len(t) == 11:
-            t[0] = produce.Produce(t[3], t[5], t[7], t[9], t.lineno(1))
-        else:
-            t[0] = produce.Produce(t[3], t[5], t[7], expression.ConstantNumeric(0), t.lineno(1))
+        'produce : PRODUCE LPAREN expression_list RPAREN SEMICOLON'
+        t[0] = produce.Produce(t[3], t.lineno(1))
 
     #
     # Real sprites and related stuff
     #
     def p_real_sprite(self, t):
-        """real_sprite : LBRACKET expression_list RBRACKET
-        | ID COLON LBRACKET expression_list RBRACKET"""
+        '''real_sprite : LBRACKET expression_list RBRACKET
+                       | ID COLON LBRACKET expression_list RBRACKET'''
         if len(t) == 4:
-            t[0] = real_sprite.RealSprite(param_list=t[2], poslist=[t.lineno(1)])
+            t[0] = real_sprite.RealSprite(t[2])
         else:
-            t[0] = real_sprite.RealSprite(param_list=t[4], label=t[1], poslist=[t.lineno(1)])
+            t[0] = real_sprite.RealSprite(t[4], t[1])
 
     def p_recolour_assignment_list(self, t):
-        """recolour_assignment_list :
-        | recolour_assignment_list recolour_assignment"""
+        '''recolour_assignment_list :
+                                    | recolour_assignment_list recolour_assignment'''
         t[0] = [] if len(t) == 1 else t[1] + [t[2]]
 
     def p_recolour_assignment_1(self, t):
-        "recolour_assignment : expression COLON expression SEMICOLON"
+        'recolour_assignment : expression COLON expression SEMICOLON'
         t[0] = assignment.Assignment(assignment.Range(t[1], None), assignment.Range(t[3], None), t[1].pos)
 
     def p_recolour_assignment_2(self, t):
-        "recolour_assignment : expression RANGE expression COLON expression RANGE expression SEMICOLON"
+        'recolour_assignment : expression RANGE expression COLON expression RANGE expression SEMICOLON'
         t[0] = assignment.Assignment(assignment.Range(t[1], t[3]), assignment.Range(t[5], t[7]), t[1].pos)
 
     def p_recolour_assignment_3(self, t):
-        "recolour_assignment : expression RANGE expression COLON expression SEMICOLON"
+        'recolour_assignment : expression RANGE expression COLON expression SEMICOLON'
         t[0] = assignment.Assignment(assignment.Range(t[1], t[3]), assignment.Range(t[5], None), t[1].pos)
 
     def p_recolour_sprite(self, t):
-        """real_sprite : RECOLOUR_SPRITE LBRACE recolour_assignment_list RBRACE
-        | ID COLON RECOLOUR_SPRITE LBRACE recolour_assignment_list RBRACE"""
-        if len(t) == 5:
-            t[0] = real_sprite.RecolourSprite(mapping=t[3], poslist=[t.lineno(1)])
-        else:
-            t[0] = real_sprite.RecolourSprite(mapping=t[5], label=t[1], poslist=[t.lineno(1)])
+        'real_sprite : RECOLOUR_SPRITE LBRACE recolour_assignment_list RBRACE'
+        t[0] = real_sprite.RecolourSprite(t[3])
 
     def p_template_declaration(self, t):
-        "template_declaration : TEMPLATE ID LPAREN id_list RPAREN LBRACE spriteset_contents RBRACE"
+        'template_declaration : TEMPLATE ID LPAREN id_list RPAREN LBRACE spriteset_contents RBRACE'
         t[0] = spriteblock.TemplateDeclaration(t[2], t[4], t[7], t.lineno(1))
 
     def p_template_usage(self, t):
-        """template_usage : ID LPAREN expression_list RPAREN
-        | ID COLON ID LPAREN expression_list RPAREN"""
+        '''template_usage : ID LPAREN expression_list RPAREN
+                          | ID COLON ID LPAREN expression_list RPAREN'''
         if len(t) == 5:
             t[0] = real_sprite.TemplateUsage(t[1], t[3], None, t.lineno(1))
         else:
             t[0] = real_sprite.TemplateUsage(t[3], t[5], t[1], t.lineno(1))
 
     def p_spriteset_contents(self, t):
-        """spriteset_contents : real_sprite
-        | template_usage
-        | spriteset_contents real_sprite
-        | spriteset_contents template_usage"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''spriteset_contents : real_sprite
+                              | template_usage
+                              | spriteset_contents real_sprite
+                              | spriteset_contents template_usage'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_replace(self, t):
-        """replace : REPLACESPRITE LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
-        | REPLACESPRITE ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"""
-        if len(t) == 9:
-            t[0] = replace.ReplaceSprite(t[4], t[7], t[2], t.lineno(1))
-        else:
-            t[0] = replace.ReplaceSprite(t[3], t[6], None, t.lineno(1))
+        '''replace : REPLACESPRITE LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
+                   | REPLACESPRITE ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'''
+        if len(t) == 9: t[0] = replace.ReplaceSprite(t[4], t[7], t[2], t.lineno(1))
+        else: t[0] = replace.ReplaceSprite(t[3], t[6], None, t.lineno(1))
 
     def p_replace_new(self, t):
-        """replace_new : REPLACENEWSPRITE LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
-        | REPLACENEWSPRITE ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"""
-        if len(t) == 9:
-            t[0] = replace.ReplaceNewSprite(t[4], t[7], t[2], t.lineno(1))
-        else:
-            t[0] = replace.ReplaceNewSprite(t[3], t[6], None, t.lineno(1))
-
-    def p_base_graphics(self, t):
-        """base_graphics : BASE_GRAPHICS LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
-        | BASE_GRAPHICS ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"""
-        if len(t) == 9:
-            t[0] = base_graphics.BaseGraphics(t[4], t[7], t[2], t.lineno(1))
-        else:
-            t[0] = base_graphics.BaseGraphics(t[3], t[6], None, t.lineno(1))
+        '''replace_new : REPLACENEWSPRITE LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
+                       | REPLACENEWSPRITE ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'''
+        if len(t) == 9: t[0] = replace.ReplaceNewSprite(t[4], t[7], t[2], t.lineno(1))
+        else: t[0] = replace.ReplaceNewSprite(t[3], t[6], None, t.lineno(1))
+
+    def p_base_sprites(self, t):
+        '''base_sprites : BASE_SPRITES LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
+                        | BASE_SPRITES ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'''
+        if len(t) == 9: t[0] = base_sprites.BaseSprite(t[4], t[7], t[2], t.lineno(1))
+        else: t[0] = base_sprites.BaseSprite(t[3], t[6], None, t.lineno(1))
 
     def p_font_glyph(self, t):
-        """font_glyph : FONTGLYPH LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
-        | FONTGLYPH ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"""
-        if len(t) == 9:
-            t[0] = font.FontGlyphBlock(t[4], t[7], t[2], t.lineno(1))
-        else:
-            t[0] = font.FontGlyphBlock(t[3], t[6], None, t.lineno(1))
+        '''font_glyph : FONTGLYPH LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE
+                      | FONTGLYPH ID LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'''
+        if len(t) == 9: t[0] = font.FontGlyphBlock(t[4], t[7], t[2], t.lineno(1))
+        else: t[0] = font.FontGlyphBlock(t[3], t[6], None, t.lineno(1))
 
     def p_alt_sprites(self, t):
-        "alt_sprites : ALT_SPRITES LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"
+        'alt_sprites : ALT_SPRITES LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'
         t[0] = alt_sprites.AltSpritesBlock(t[3], t[6], t.lineno(1))
 
     #
     # Sprite sets/groups and such
     #
 
     def p_spriteset(self, t):
-        "spriteset : SPRITESET LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE"
+        'spriteset : SPRITESET LPAREN expression_list RPAREN LBRACE spriteset_contents RBRACE'
         t[0] = spriteblock.SpriteSet(t[3], t[6], t.lineno(1))
 
     def p_spritegroup_normal(self, t):
-        "spritegroup : SPRITEGROUP ID LBRACE spriteview_list RBRACE"
+        'spritegroup : SPRITEGROUP ID LBRACE spriteview_list RBRACE'
         t[0] = spriteblock.SpriteGroup(t[2], t[4], t.lineno(1))
 
     def p_spritelayout(self, t):
-        """spritelayout : SPRITELAYOUT ID LBRACE layout_sprite_list RBRACE
-        | SPRITELAYOUT ID LPAREN id_list RPAREN LBRACE layout_sprite_list RBRACE"""
+        '''spritelayout : SPRITELAYOUT ID LBRACE layout_sprite_list RBRACE
+                        | SPRITELAYOUT ID LPAREN id_list RPAREN LBRACE layout_sprite_list RBRACE'''
         if len(t) == 6:
             t[0] = spriteblock.SpriteLayout(t[2], [], t[4], t.lineno(1))
         else:
             t[0] = spriteblock.SpriteLayout(t[2], t[4], t[7], t.lineno(1))
 
     def p_spriteview_list(self, t):
-        """spriteview_list :
-        | spriteview_list spriteview"""
-        if len(t) == 1:
-            t[0] = []
-        else:
-            t[0] = t[1] + [t[2]]
+        '''spriteview_list :
+                           | spriteview_list spriteview'''
+        if len(t) == 1: t[0] = []
+        else: t[0] = t[1] + [t[2]]
 
     def p_spriteview(self, t):
-        """spriteview : ID COLON LBRACKET expression_list RBRACKET SEMICOLON
-        | ID COLON expression SEMICOLON"""
-        if len(t) == 7:
-            t[0] = spriteblock.SpriteView(t[1], t[4], t.lineno(1))
-        else:
-            t[0] = spriteblock.SpriteView(t[1], [t[3]], t.lineno(1))
+        '''spriteview : ID COLON LBRACKET expression_list RBRACKET SEMICOLON
+                      | ID COLON expression SEMICOLON'''
+        if len(t) == 7: t[0] = spriteblock.SpriteView(t[1], t[4], t.lineno(1))
+        else: t[0] = spriteblock.SpriteView(t[1], [t[3]], t.lineno(1))
 
     def p_layout_sprite_list(self, t):
-        """layout_sprite_list :
-        | layout_sprite_list layout_sprite"""
-        if len(t) == 1:
-            t[0] = []
-        else:
-            t[0] = t[1] + [t[2]]
+        '''layout_sprite_list :
+                              | layout_sprite_list layout_sprite'''
+        if len(t) == 1: t[0] = []
+        else: t[0] = t[1] + [t[2]]
 
     def p_layout_sprite(self, t):
-        "layout_sprite : ID LBRACE layout_param_list RBRACE"
+        'layout_sprite : ID LBRACE layout_param_list RBRACE'
         t[0] = spriteblock.LayoutSprite(t[1], t[3], t.lineno(1))
 
     def p_layout_param_list(self, t):
-        """layout_param_list : assignment
-        | layout_param_list assignment"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''layout_param_list : assignment
+                             | layout_param_list assignment'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     #
     # Town names
     #
     def p_town_names(self, t):
-        """town_names : TOWN_NAMES LPAREN expression RPAREN LBRACE town_names_param_list RBRACE
-        | TOWN_NAMES LBRACE town_names_param_list RBRACE"""
-        if len(t) == 8:
-            t[0] = townnames.TownNames(t[3], t[6], t.lineno(1))
-        else:
-            t[0] = townnames.TownNames(None, t[3], t.lineno(1))
+        '''town_names : TOWN_NAMES LPAREN expression RPAREN LBRACE town_names_param_list RBRACE
+                      | TOWN_NAMES LBRACE town_names_param_list RBRACE'''
+        if len(t) == 8: t[0] = townnames.TownNames(t[3], t[6], t.lineno(1))
+        else: t[0] = townnames.TownNames(None, t[3], t.lineno(1))
 
     def p_town_names_param_list(self, t):
-        """town_names_param_list : town_names_param
-        | town_names_param_list town_names_param"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''town_names_param_list : town_names_param
+                                 | town_names_param_list town_names_param'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_town_names_param(self, t):
-        """town_names_param : ID COLON string SEMICOLON
-        | LBRACE town_names_part_list RBRACE
-        | LBRACE town_names_part_list COMMA RBRACE"""
-        if t[1] != "{":
-            t[0] = townnames.TownNamesParam(t[1], t[3], t.lineno(1))
-        else:
-            t[0] = townnames.TownNamesPart(t[2], t.lineno(1))
+        '''town_names_param : ID COLON string SEMICOLON
+                            | LBRACE town_names_part_list RBRACE
+                            | LBRACE town_names_part_list COMMA RBRACE'''
+        if t[1] != '{': t[0] = townnames.TownNamesParam(t[1], t[3], t.lineno(1))
+        else: t[0] = townnames.TownNamesPart(t[2], t.lineno(1))
 
     def p_town_names_part_list(self, t):
-        """town_names_part_list : town_names_part
-        | town_names_part_list COMMA town_names_part"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[3]]
+        '''town_names_part_list : town_names_part
+                                | town_names_part_list COMMA town_names_part'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[3]]
 
     def p_town_names_part(self, t):
-        """town_names_part : TOWN_NAMES LPAREN expression COMMA expression RPAREN
-        | ID LPAREN STRING_LITERAL COMMA expression RPAREN"""
-        if t[1] == "town_names":
-            t[0] = townnames.TownNamesEntryDefinition(t[3], t[5], t.lineno(1))
-        else:
-            t[0] = townnames.TownNamesEntryText(t[1], t[3], t[5], t.lineno(1))
+        '''town_names_part : TOWN_NAMES LPAREN expression COMMA expression RPAREN
+                           | ID LPAREN STRING_LITERAL COMMA expression RPAREN'''
+        if t[1] == 'town_names': t[0] = townnames.TownNamesEntryDefinition(t[3], t[5], t.lineno(1))
+        else: t[0] = townnames.TownNamesEntryText(t[1], t[3], t[5], t.lineno(1))
 
     #
     # Snow line
     #
     def p_snowline(self, t):
-        "snowline : SNOWLINE LPAREN ID RPAREN LBRACE snowline_assignment_list RBRACE"
+        'snowline : SNOWLINE LPAREN ID RPAREN LBRACE generic_assignment_list RBRACE'
         t[0] = snowline.Snowline(t[3], t[6], t.lineno(1))
 
     #
     # Various misc. main script blocks that don't belong anywhere else
     #
     def p_param_assignment(self, t):
-        "param_assignment : expression EQ expression SEMICOLON"
+        'param_assignment : expression EQ expression SEMICOLON'
         t[0] = actionD.ParameterAssignment(t[1], t[3])
 
     def p_error_block(self, t):
-        "error_block : ERROR LPAREN expression_list RPAREN SEMICOLON"
+        'error_block : ERROR LPAREN expression_list RPAREN SEMICOLON'
         t[0] = error.Error(t[3], t.lineno(1))
 
     def p_disable_item(self, t):
-        "disable_item : DISABLE_ITEM LPAREN expression_list RPAREN SEMICOLON"
+        'disable_item : DISABLE_ITEM LPAREN expression_list RPAREN SEMICOLON'
         t[0] = disable_item.DisableItem(t[3], t.lineno(1))
 
     def p_cargotable(self, t):
-        """cargotable : CARGOTABLE LBRACE cargotable_list RBRACE
-        | CARGOTABLE LBRACE cargotable_list COMMA RBRACE"""
+        '''cargotable : CARGOTABLE LBRACE cargotable_list RBRACE
+                      | CARGOTABLE LBRACE cargotable_list COMMA RBRACE'''
         t[0] = cargotable.CargoTable(t[3], t.lineno(1))
 
     def p_cargotable_list(self, t):
-        """cargotable_list : ID
-        | STRING_LITERAL
-        | cargotable_list COMMA ID
-        | cargotable_list COMMA STRING_LITERAL"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[3]]
+        '''cargotable_list : ID
+                           | STRING_LITERAL
+                           | cargotable_list COMMA ID
+                           | cargotable_list COMMA STRING_LITERAL'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[3]]
 
     def p_railtypetable(self, t):
-        """railtype : RAILTYPETABLE LBRACE tracktypetable_list RBRACE
-        | RAILTYPETABLE LBRACE tracktypetable_list COMMA RBRACE"""
-        t[0] = tracktypetable.RailtypeTable(t[3], t.lineno(1))
-
-    def p_roadtypetable(self, t):
-        """roadtype : ROADTYPETABLE LBRACE tracktypetable_list RBRACE
-        | ROADTYPETABLE LBRACE tracktypetable_list COMMA RBRACE"""
-        t[0] = tracktypetable.RoadtypeTable(t[3], t.lineno(1))
-
-    def p_tramtypetable(self, t):
-        """tramtype : TRAMTYPETABLE LBRACE tracktypetable_list RBRACE
-        | TRAMTYPETABLE LBRACE tracktypetable_list COMMA RBRACE"""
-        t[0] = tracktypetable.TramtypeTable(t[3], t.lineno(1))
-
-    def p_tracktypetable_list(self, t):
-        """tracktypetable_list : tracktypetable_item
-        | tracktypetable_list COMMA tracktypetable_item"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[3]]
-
-    def p_tracktypetable_item(self, t):
-        """tracktypetable_item : ID
-        | STRING_LITERAL
-        | ID COLON LBRACKET expression_list RBRACKET"""
-        if len(t) == 2:
-            t[0] = t[1]
-        else:
-            t[0] = assignment.Assignment(t[1], t[4], t[1].pos)
+        '''railtype : RAILTYPETABLE LBRACE railtypetable_list RBRACE
+                    | RAILTYPETABLE LBRACE railtypetable_list COMMA RBRACE'''
+        t[0] = railtypetable.RailtypeTable(t[3], t.lineno(1))
+
+    def p_railtypetable_list(self, t):
+        '''railtypetable_list : railtypetable_item
+                              | railtypetable_list COMMA railtypetable_item'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[3]]
+
+    def p_railtypetable_item(self, t):
+        '''railtypetable_item : ID
+                              | STRING_LITERAL
+                              | ID COLON LBRACKET expression_list RBRACKET'''
+        if len(t) == 2: t[0] = t[1]
+        else: t[0] = assignment.Assignment(t[1], t[4], t[1].pos)
 
     def p_basecost(self, t):
-        "basecost : BASECOST LBRACE generic_assignment_list RBRACE"
+        'basecost : BASECOST LBRACE generic_assignment_list RBRACE'
         t[0] = basecost.BaseCost(t[3], t.lineno(1))
 
     def p_deactivate(self, t):
-        "deactivate : DEACTIVATE LPAREN expression_list RPAREN SEMICOLON"
+        'deactivate : DEACTIVATE LPAREN expression_list RPAREN SEMICOLON'
         t[0] = deactivate.DeactivateBlock(t[3], t.lineno(1))
 
     def p_grf_block(self, t):
-        "grf_block : GRF LBRACE assignment_list RBRACE"
+        'grf_block : GRF LBRACE assignment_list RBRACE'
         t[0] = grf.GRF(t[3], t.lineno(1))
 
     def p_skip_all(self, t):
-        "skip_all : SKIP_ALL SEMICOLON"
+        'skip_all : SKIP_ALL SEMICOLON'
         t[0] = skipall.SkipAll(t.lineno(1))
 
     def p_engine_override(self, t):
-        "engine_override : ENGINE_OVERRIDE LPAREN expression_list RPAREN SEMICOLON"
+        'engine_override : ENGINE_OVERRIDE LPAREN expression_list RPAREN SEMICOLON'
         t[0] = override.EngineOverride(t[3], t.lineno(1))
 
-    def p_sort_vehicles(self, t):
-        "sort_vehicles : SORT_VEHICLES LPAREN expression_list RPAREN SEMICOLON"
-        t[0] = sort_vehicles.SortVehicles(t[3], t.lineno(1))
-
     def p_tilelayout(self, t):
-        "tilelayout : TILELAYOUT ID LBRACE tilelayout_list RBRACE"
+        'tilelayout : TILELAYOUT ID LBRACE tilelayout_list RBRACE'
         t[0] = tilelayout.TileLayout(t[2], t[4], t.lineno(1))
 
     def p_tilelayout_list(self, t):
-        """tilelayout_list : tilelayout_item
-        | tilelayout_list tilelayout_item"""
-        if len(t) == 2:
-            t[0] = [t[1]]
-        else:
-            t[0] = t[1] + [t[2]]
+        '''tilelayout_list : tilelayout_item
+                           | tilelayout_list tilelayout_item'''
+        if len(t) == 2: t[0] = [t[1]]
+        else: t[0] = t[1] + [t[2]]
 
     def p_tilelayout_item_tile(self, t):
-        "tilelayout_item : expression COMMA expression COLON expression SEMICOLON"
+        'tilelayout_item : expression COMMA expression COLON expression SEMICOLON'
         t[0] = tilelayout.LayoutTile(t[1], t[3], t[5])
 
     def p_tilelayout_item_prop(self, t):
-        "tilelayout_item : assignment"
+        'tilelayout_item : assignment'
         t[0] = t[1]
```

### Comparing `nml-0.7.2/regression/010_liveryoverride.nml` & `nml-r1512/regression/010_liveryoverride.nml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 grf {
-    grfid: "NML\10";
+    grfid: "test";
     name: string(STR_REGRESSION_NAME);
     desc: string(STR_REGRESSION_DESC);
     version: 0;
     min_compatible_version: 0;
 }
 
 /*
@@ -61,23 +61,23 @@
     property {
         sprite_id:                    SPRITE_ID_NEW_TRAIN;    // We have our own sprites
         misc_flags:                   bitmask(TRAIN_FLAG_MU); // We use special sprites for passenger and mail wagons
     }
     graphics {
         turbotrain_engine_group;
     }
-    livery_override(passenger_wagon) {
+    livery_override(passenger_wagon) { 
         turbotrain_passenger_group;
     }
 }
 
 item(FEAT_TRAINS, passenger_wagon, 27) {
     property {
         sprite_id:                    SPRITE_ID_NEW_TRAIN;    // We have our own sprites
         misc_flags:                   bitmask(TRAIN_FLAG_MU); // We use special sprites for passenger and mail wagons
         refittable_cargo_classes:     bitmask(CC_PASSENGERS); // Allow passengers (and tourists)
         non_refittable_cargo_classes: NO_CARGO_CLASS;         // Disallow other cargos
     }
     graphics {
         normal_passenger_group;
     }
-}
+}
```

### Comparing `nml-0.7.2/regression/013_train_callback.nml` & `nml-r1512/regression/013_train_callback.nml`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     grfid: "NML\13";
     name: string(STR_REGRESSION_NAME);
     desc: string(STR_REGRESSION_DESC);
     version: 0;
     min_compatible_version: 0;
 }
 
-/*
+/* 
  * ********************************************
  * Define cargo and railtype translation tables
  * ********************************************
  */
 
 cargotable { // cargos needed for special refit orders
     WDPR, SCRP, CMNT, WOOD, // bulk, bulk+piece+flat, tank, piece
@@ -88,62 +88,61 @@
     FICR: return 25;
     FRUT: return 20;
     FRVG: return 20;
     GRAI: return 25;
     MAIZ: return 25;
     RSGR: return 20;
     WHEA: return 25;
-    // no default: instead fail CB and use capacity set in properties (30)
+    CB_FAILED; // return capacity set in properties (30)
 }
 
-switch (FEAT_TRAINS, SELF, bulk_wagon_cb_weight_switch, cargo_type_in_veh) {
+switch (FEAT_TRAINS, SELF, bulk_wagon_cb_property_weight_switch, cargo_type_in_veh) {
     COAL: return 18;
     FRUT: return 18;
     FRVG: return 18;
     RSGR: return 18;
-    // no default: instead fail CB and use weight set in properties (25t)
+    CB_FAILED; // return weight set in properties (25t)
+}
+
+switch (FEAT_TRAINS, SELF, bulk_wagon_cb_property_switch, extra_callback_info1) {
+    0x16: bulk_wagon_cb_property_weight_switch;
+    CB_FAILED;
+}
+
+switch (FEAT_TRAINS, SELF, bulk_wagon_cb_switch, current_callback) {
+    VEH_CB_REFITTED_CAPACITY: bulk_wagon_cb_capacity_switch;
+    VEH_CB_VEHICLE_PROPERTIES: bulk_wagon_cb_property_switch;
+    bulk_wagon_graphics_switch;
 }
 
 
 item(FEAT_TRAINS, bulk_wagon) {
     property {
-        // Some bogus property assignments to test handling of units
-        speed: 10 m/s;
-        speed: param[1] m/s;
-        speed: param[2] km/h;
-        speed: param[3] mph;
-        power: param[4] kW;
-    }
-    property {
         // We try to simulate the stats of the temperate grain wagon
         name: string(STR_NAME_BULK_WAGON);
         climates_available: ALL_CLIMATES;
         refittable_cargo_classes: bitmask(CC_BULK);
         non_refittable_cargo_classes: bitmask(CC_PASSENGERS, CC_MAIL, CC_ARMOURED, CC_LIQUID, CC_REFRIGERATED, CC_HAZARDOUS);
-        cargo_allow_refit: [WDPR, SCRP, FRUT, FRVG];
-        default_cargo_type: COAL;
+        refittable_cargo_types: bitmask(WDPR, SCRP, FRUT, FRVG);
         sprite_id: SPRITE_ID_NEW_TRAIN;
         introduction_date: date(1880,1,1);
         model_life: VEHICLE_NEVER_EXPIRES;
         retire_early: 0;
         vehicle_life: 30;
         reliability_decay: 0;
         loading_speed: 10;
         cost_factor: 182;
         running_cost_factor: 5;
         speed: 0;
         refit_cost: 40;
+        callback_flags: bitmask(VEH_CBF_REFITTED_CAPACITY);
         track_type: RAIL;
         power: 0;
         running_cost_base: RUNNING_COST_STEAM;
         cargo_capacity: 30;
-        weight: param[1] ton;
+        weight: 25 ton;
         bitmask_vehicle_info: 0;
     }
     graphics {
-        weight: bulk_wagon_cb_weight_switch;
-        purchase_weight: return 25;
-        cargo_capacity: bulk_wagon_cb_capacity_switch;
-        purchase_cargo_capacity: return 30;
-        default: bulk_wagon_graphics_switch;
+        bulk_wagon_cb_switch;
     }
 }
```

### Comparing `nml-0.7.2/regression/014_read_special_param.nml` & `nml-r1512/regression/014_read_special_param.nml`

 * *Files identical despite different names*

### Comparing `nml-0.7.2/regression/015_basic_object.nml` & `nml-r1512/regression/015_basic_object.nml`

 * *Files identical despite different names*

### Comparing `nml-0.7.2/regression/016_basic_airporttiles.nml` & `nml-r1512/regression/016_basic_airporttiles.nml`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 
 item(FEAT_AIRPORTTILES, small_airport_tiles) {
     property {
         substitute: 0;
         animation_info: [ANIMATION_LOOPING, 4]; // loop, 4 frames
         animation_speed: 1;
         animation_triggers: 1;
+        callback_flags: bitmask(APT_CBF_ANIM_NEXT_FRAME);
     }
     graphics {
         small_airport_tiles_graphics;
     }
 }
```

### Comparing `nml-0.7.2/regression/017_articulated_tram.nml` & `nml-r1512/regression/017_articulated_tram.nml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
 A simple articulated tram, graphics from OpenGFX+rv
 Code is modified in some places for testing reasons.
 */
 
 grf {
-    grfid: "NML\17";
+    grfid: "test";
     name: string(STR_REGRESSION_NAME);
     desc: string(STR_REGRESSION_DESC);
     version: 0;
     min_compatible_version: 0;
 }
 
 template tmpl_tram(x, y) {
@@ -20,44 +20,50 @@
     [144 + x, y, 20, 18,  -14,  -9]
     [176 + x, y, 28, 15,  -14,  -8]
     [224 + x, y, 20, 18,   -6,  -7]
 }
 spriteset(foster_express_set, "tram_foster_express.png") {
     tmpl_tram(48,1)
 }
-
+spritegroup foster_express_group {
+    loading: foster_express_set;
+    loaded: foster_express_set;
+}
 switch(FEAT_ROADVEHS, SELF, foster_express_articulated_parts, extra_callback_info1) {
-    1..3: return foster_express_tram;
-    return 0xFF;
+    1..3: return 88;
+    CB_FAILED;
 }
 
+switch(FEAT_ROADVEHS, SELF, foster_express_callbacks, current_callback) {
+    VEH_CB_ARTICULATED_PARTS: foster_express_articulated_parts;
+    foster_express_group;
+}
 
 item(FEAT_ROADVEHS, foster_express_tram, 88) {
     property {
-        name:                         string(STR_NAME_FOSTER_TURBO_TRAM);
+        name:                         string(STR_NAME_FOSTER_EXPRESS_TRAM);
         climates_available:           ALL_CLIMATES;
         model_life:                   40;                         // years
         vehicle_life:                 30;                         // years
         introduction_date:            date(1965,1,1);
-        reliability_decay:            1;
+        reliability_decay:            1; 
         running_cost_base:            RUNNING_COST_ROADVEH;       // Default road vehicle running cost base
         running_cost_factor:          135;
         cost_factor:                  143;
-        speed:                        317 mph;
+        speed:                        75 km/h;
         power:                        220 hp;
         weight:                       22 ton;
         sprite_id:                    SPRITE_ID_NEW_ROADVEH;      // We have our own sprites
         loading_speed:                16;                         // loading speed
         tractive_effort_coefficient:  0.3;
         air_drag_coefficient:         0.5;
         cargo_capacity:               45;                         // passengers
         refittable_cargo_classes:     bitmask(CC_PASSENGERS); // Allow passengers (and tourists)
         non_refittable_cargo_classes: NO_CARGO_CLASS;         // Disallow other cargos
-        cargo_allow_refit:            [];
-        default_cargo_type:           DEFAULT_CARGO_FIRST_REFITTABLE;
+        refittable_cargo_types:       0;
         misc_flags:                   bitmask(ROADVEH_FLAG_TRAM); // This is a tram
+        callback_flags:               bitmask(VEH_CBF_ARTICULATED_PARTS);
     }
     graphics {
-        articulated_part: foster_express_articulated_parts;
-        foster_express_set;
+        foster_express_callbacks;
     }
 }
```

### Comparing `nml-0.7.2/regression/020_recolour.nml` & `nml-r1512/regression/020_recolour.nml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 grf {
-    grfid: "NML\20";
+    grfid: "test";
     name: string(STR_REGRESSION_NAME);
     desc: string(STR_REGRESSION_DESC);
     version: 0;
     min_compatible_version: 0;
 }
 
 template company_recolour(offset) {
```

### Comparing `nml-0.7.2/regression/021_grf_parameter.nml` & `nml-r1512/regression/021_grf_parameter.nml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // define the newgrf
 grf {
-    grfid: "NML\21";
+    grfid: "test";
     name: string(STR_REGRESSION_NAME);
     desc: string(STR_REGRESSION_DESC);
     version: 1;
     min_compatible_version: 0;
     param (0) {
         param_NoGrid {
             type:    bool;
```

### Comparing `nml-0.7.2/regression/arctic_railwagons.pcx` & `nml-r1512/regression/arctic_railwagons.pcx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 0a05 0108 0000 0000 ef00 8902 4800 4800  ............H.H.
+00000000: 0a05 0108 0000 0000 ef00 8902 2c01 2c01  ............,.,.
 00000010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 0001 f000 0100 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `nml-0.7.2/regression/expected/001_action8.nfo` & `nml-r1512/regression/expected/001_action8.nfo`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d2
+0 * 4 \d2 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\1" "NML regression test" 00 "A test newgrf testing NML" 00
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00
```

### Comparing `nml-0.7.2/regression/expected/003_assignment.nfo` & `nml-r1512/regression/expected/003_assignment.nfo`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
 // param[0] = 3
-0 * 9 0D 00 \D= FF 00 \dx00000003
+0 * 9 0D 00 \D= FF 00 \dx00000003 
 
 // param[1] = 4
-1 * 9 0D 01 \D= FF 00 \dx00000004
+1 * 9 0D 01 \D= FF 00 \dx00000004 
 
 // param[2] = (param[0] + param[1])
-2 * 5 0D 02 \D+ 00 01
+2 * 5 0D 02 \D+ 00 01 
 
 // param[3] = (param[0] * 3)
-3 * 9 0D 03 \D* 00 FF \dx00000003
+3 * 9 0D 03 \D* 00 FF \dx00000003 
 
 // param[4] = 11
-4 * 9 0D 04 \D= FF 00 \dx0000000B
+4 * 9 0D 04 \D= FF 00 \dx0000000B 
 
 // param[5] = (param[4] & 3)
-5 * 9 0D 05 \D& 04 FF \dx00000003
+5 * 9 0D 05 \D& 04 FF \dx00000003 
 
-// param[127] = (param[1] + param[2])
-6 * 5 0D 7F \D+ 01 02
+// param[64] = (param[1] + param[2])
+6 * 5 0D 40 \D+ 01 02 
 
-// param[6] = (param[127] + param[3])
-7 * 5 0D 06 \D+ 7F 03
+// param[6] = (param[64] + param[3])
+7 * 5 0D 06 \D+ 40 03 
 
-// param[127] = param[3]
-8 * 5 0D 7F \D= 03 00
+// param[64] = param[3]
+8 * 5 0D 40 \D= 03 00 
 
-9 * 7 06
-7F 01 FF \wx0003
-FF
+9 * 7 06 
+40 01 FF \wx0003 
+FF 
 
 // param[7] = param[0]
-10 * 5 0D 07 \D= 00 00
+10 * 5 0D 07 \D= 00 00 
 
-11 * 7 06
-00 01 FF \wx0001
-FF
+11 * 7 06 
+00 01 FF \wx0001 
+FF 
 
 // param[0] = 5
-12 * 9 0D 00 \D= FF 00 \dx00000005
+12 * 9 0D 00 \D= FF 00 \dx00000005 
 
-// param[127] = param[3]
-13 * 5 0D 7F \D= 03 00
+// param[64] = param[3]
+13 * 5 0D 40 \D= 03 00 
 
-14 * 12 06
-00 01 FF \wx0001
-7F 01 FF \wx0003
-FF
+14 * 12 06 
+00 01 FF \wx0001 
+40 01 FF \wx0003 
+FF 
 
 // param[0] = param[0]
-15 * 5 0D 00 \D= 00 00
+15 * 5 0D 00 \D= 00 00
```

### Comparing `nml-0.7.2/regression/expected/005_error.nfo` & `nml-r1512/regression/expected/005_error.nfo`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 9 0B 00 1F 02 "zorg" 00
+0 * 9 0B 00 1F 02 "zorg" 00 
 
-1 * 9 0B 00 7F 02 "care" 00
+1 * 9 0B 00 7F 02 "care" 00 
 
-// param[127] = 14
-2 * 9 0D 7F \D= FF 00 \dx0000000E
+// param[64] = 14
+2 * 9 0D 40 \D= FF 00 \dx0000000E 
 
-// param[125] = (param[2] * 12)
-3 * 9 0D 7D \D* 02 FF \dx0000000C
+// param[66] = (param[2] * 12)
+3 * 9 0D 42 \D* 02 FF \dx0000000C 
 
-// param[126] = (param[1] + param[125])
-4 * 5 0D 7E \D+ 01 7D
+// param[65] = (param[1] + param[66])
+4 * 5 0D 41 \D+ 01 42 
 
-5 * 66 0B 03 1F FF "De wissels zijn bevroren, onze excuses voor het ongemak." 00 "42" 00 7F 7E
+5 * 66 0B 03 1F FF "De wissels zijn bevroren, onze excuses voor het ongemak." 00 "42" 00 40 41 
 
-6 * 42 0B 03 7F FF "Something bad (tm) has happened." 00 "42" 00 7F 7E
+6 * 42 0B 03 7F FF "Something bad (tm) has happened." 00 "42" 00 40 41
```

### Comparing `nml-0.7.2/regression/expected/010_liveryoverride.grf` & `nml-r1512/regression/expected/010_liveryoverride.grf`

 * *Files 18% similar despite different names*

```diff
@@ -1,342 +1,314 @@
-00000000: 0000 4752 4682 0d0a 1a0a e901 0000 0004  ..GRF...........
-00000010: 0000 00ff 2300 0000 3600 0000 ff14 4349  ....#...6.....CI
-00000020: 4e46 4f42 5652 534e 0400 0000 0000 424d  NFOBVRSN......BM
-00000030: 494e 5604 0000 0000 0042 4e50 4152 0100  INV......BNPAR..
-00000040: 0042 5041 4c53 0100 5742 424c 5452 0100  .BPALS..WBBLTR..
-00000050: 3800 0034 0000 00ff 0808 4e4d 4c10 4e4d  8..4......NML.NM
-00000060: 4c20 7265 6772 6573 7369 6f6e 2074 6573  L regression tes
-00000070: 7400 4120 7465 7374 206e 6577 6772 6620  t.A test newgrf 
-00000080: 7465 7374 696e 6720 4e4d 4c00 0600 0000  testing NML.....
-00000090: ff01 0003 ff08 0004 0000 00fd 0500 0000  ................
-000000a0: 0400 0000 fd06 0000 0004 0000 00fd 0700  ................
-000000b0: 0000 0400 0000 fd08 0000 0004 0000 00fd  ................
-000000c0: 0900 0000 0400 0000 fd0a 0000 0004 0000  ................
-000000d0: 00fd 0b00 0000 0400 0000 fd0c 0000 0004  ................
-000000e0: 0000 00fd 0d00 0000 0400 0000 fd0e 0000  ................
-000000f0: 0004 0000 00fd 0f00 0000 0400 0000 fd10  ................
-00000100: 0000 0004 0000 00fd 1100 0000 0400 0000  ................
-00000110: fd12 0000 0004 0000 00fd 1300 0000 0400  ................
-00000120: 0000 fd14 0000 0004 0000 00fd 1500 0000  ................
-00000130: 0400 0000 fd16 0000 0004 0000 00fd 1700  ................
-00000140: 0000 0400 0000 fd18 0000 0004 0000 00fd  ................
-00000150: 1900 0000 0400 0000 fd1a 0000 0004 0000  ................
-00000160: 00fd 1b00 0000 0400 0000 fd1c 0000 0009  ................
-00000170: 0000 00ff 0200 ff01 0100 0000 0009 0000  ................
-00000180: 00ff 0200 fe01 0101 0001 0009 0000 00ff  ................
-00000190: 0200 fd01 0102 0002 000b 0000 00ff 0000  ................
-000001a0: 0201 ff14 0012 fd27 0409 0000 00ff 0300  .......'........
-000001b0: 01ff 1400 00ff 0009 0000 00ff 0300 81ff  ................
-000001c0: 1b00 00fd 001b 0000 00ff 0000 0601 ff1b  ................
-000001d0: 0012 fd27 0428 0100 1d00 0000 0029 0000  ...'.(.......)..
-000001e0: 1d00 0000 0009 0000 00ff 0300 01ff 1b00  ................
-000001f0: 00fe 0000 0000 0005 0000 009d 0000 0004  ................
-00000200: 0016 0008 00fd fff6 ff07 00c6 c8c8 c8c8  ................
-00000210: c7e8 0707 caca caca c9c8 c6e0 0705 cbca  ................
-00000220: c9c7 cbe8 07e8 0411 c810 11cb cc10 11ca  ................
-00000230: c911 cacb cccb 12c9 c9e8 16e8 180b cc14  ................
-00000240: 14ca 1413 ca12 14cb 13e8 3905 c913 ccc6  ..........9.....
-00000250: c7d8 2f02 cac6 e821 01cc e840 c808 e010  ../....!...@....
-00000260: 02cc cce8 59e0 60e0 5002 c7c8 e030 03c9  ....Y.`.P....0..
-00000270: cac8 e84a e068 e850 02d7 d7e8 7107 cac9  ...J.h.P....q...
-00000280: d7d8 d7d7 12e8 1be0 0804 10c8 c7c7 e010  ................
-00000290: 05d8 c6d7 d7d7 e803 d006 e00c 0600 0000  ................
-000002a0: e800 0000 0400 0f00 1500 f2ff f9ff 0300  ................
-000002b0: 0000 e803 d006 0500 c7c9 c9c8 9811 e013  ................
-000002c0: 06ca cacb cbca c9a0 2602 8812 e813 e815  ........&.......
-000002d0: 02ca ccb8 390d 1312 caca 8812 cccb cacc  ....9...........
-000002e0: 13cc 20c0 4e04 12ca 1112 e829 05cc 13cd  .. .N......)....
-000002f0: cd16 d015 02c6 c9e8 6201 cae8 3fe8 1304  ........b...?...
-00000300: 170d 0d58 d813 d061 0ac9 13cc cc17 0d0e  ...X...a........
-00000310: 0c0c d8c8 1303 cccc cde8 3c0b 1614 0e0d  ..........<.....
-00000320: 0c0a c900 c7c7 c8e8 8903 cccd cce8 640e  ..............d.
-00000330: 130c 150c 0b28 d7c7 0010 10d8 c8c8 e861  .....(.........a
-00000340: 0acb ca16 0d0c 0bf5 0a28 d7e8 cf06 10d7  .........(......
-00000350: d7d8 c9c9 e826 0616 0d0d 0cf5 21d0 8e08  .....&......!...
-00000360: d8d7 d7d7 10c7 150f e828 020a 28c0 a1e8  .........(..(...
-00000370: 1408 d7d8 1017 0d0b 0af5 c0b4 c817 03c6  ................
-00000380: 0c0a c839 a017 0188 e05f b131 0700 0000  ...9....._.1....
-00000390: 3a01 0000 0400 0c00 1f00 f0ff f8ff 0300  :...............
-000003a0: 0000 e803 d006 0900 c7c7 2820 c7c9 c7c9  ..........( ....
-000003b0: e004 01c7 981a e027 0f10 c9c9 c9c9 caca  .......'........
-000003c0: cbcb cbcb cbca c912 e03a 06c6 c6c6 c7c7  .........:......
-000003d0: c7e8 0308 c8c8 c710 c9cb 2058 d81d 09cc  .......... X....
-000003e0: cccb ca13 cbcb 0000 c82c e82e 03c9 c810  .........,......
-000003f0: e83b e83c 03cc cbcc e041 0514 cccc be00  .;.<.....A......
-00000400: e829 03cd cdcd e810 e820 1311 ca12 cb12  .)....... ......
-00000410: cc13 cc13 cd14 cd14 1414 cdcd f510 e06a  ...............j
-00000420: e83c 01cb e038 e844 02cc cad8 1d09 16cd  .<...8.D........
-00000430: 1616 cc16 16be 6ae8 3ae8 3fe0 42e0 06d8  ......j.:.?.B...
-00000440: 4bc8 0c09 cd0c 0c28 580c 0e15 13e8 0302  K......(X.......
-00000450: 0f14 e803 0812 0e13 110e 0d0d 0de8 03e8  ................
-00000460: 0609 0e17 17f5 880c 0e16 15e8 0309 0e16  ................
-00000470: 140d 1514 0d13 12b8 1e02 0d0e e83e 05d8  .............>..
-00000480: 0a0b 0b0b e803 d006 030b 2821 b80f 0a0c  ..........(!....
-00000490: 0b0a 0a58 d728 1515 15e8 03d0 061b 0a28  ...X.(.........(
-000004a0: 210a 0a0a 0af5 f528 2828 f528 1313 c600  !......(((.(....
-000004b0: 5820 2020 2020 2121 21e8 0304 2121 6a6a  X     !!!...!!jj
-000004c0: e00a 0b88 58d7 d7d7 8888 d7c8 c600 0800  ....X...........
-000004d0: 0000 fa00 0000 0400 1000 1500 faff f9ff  ................
-000004e0: 0500 0000 00c9 e005 e009 c008 0600 00ca  ................
-000004f0: caca ca88 1706 00ca cbcb cbcb 8817 03c9  ................
-00000500: c9ca e017 e82d 04c8 c9c9 c8c8 4802 11c9  .....-......H...
-00000510: e017 e013 04ca ca10 12c8 1703 12f5 10e8  ................
-00000520: 1703 c9c6 c8e8 13d0 31e8 7b0a 2828 1128  ........1.{.((.(
-00000530: 10c9 c611 11c8 e85d 01cc e05e e844 0a58  .......]...^.D.X
-00000540: 2121 2811 1211 cac9 10e8 86e8 1710 14cc  !!(.............
-00000550: 1300 00d7 5820 2021 2812 2820 c9ca e017  ....X  !(.( ....
-00000560: 0516 15cb cc28 e8bc 0258 6ae8 1604 28f5  .....(...Xj...(.
-00000570: f514 e057 06cc cccc 16bf 6ae0 d211 586a  ...W......j...Xj
-00000580: 2121 20f5 15f5 14ca cacc 0cbf 6a28 21d0  !! .........j(!.
-00000590: e203 586a 6ae8 2d08 150a 0a0c 6a20 5820  ..Xjj.-.....j X 
-000005a0: d82a d82e e85a 09f5 0a0b 0a58 586a 58d8  .*...Z.....XXjX.
-000005b0: b10c 03d8 8858 e85a 05d8 d888 d8d7 a121  .....X.Z.......!
-000005c0: 07d7 c6c8 88d7 d7d7 9814 e146 01c6 d946  ...........F...F
-000005d0: 0900 0000 ae00 0000 0400 1800 0800 fdff  ................
-000005e0: f6ff 1000 c8c8 c9c9 c9c9 00c7 c9ca cacb  ................
-000005f0: caca c9e8 0802 cbcc e809 c808 02c9 c8c8  ................
-00000600: 10e8 0802 cccc d020 e826 03ca cac6 d837  ....... .&.....7
-00000610: 0bc9 c9c6 1011 cacb 1011 c9c7 e807 03cc  ................
-00000620: cb12 e028 d838 e04f 01cb e051 e82f e85a  ...(.8.O...Q./.Z
-00000630: 0ac9 ca11 cb13 14cc 0ccb 11e8 0807 15cc  ................
-00000640: 0c16 c8c9 cbc8 6002 cbcc e859 23cb c828  ......`....Y#..(
-00000650: 0a0b 0b0c 0ecb 206a bf58 21bf 130c 2088  ...... j.X!... .
-00000660: 886a 2013 6a0b 6ad8 8858 6a6a 8815 88d7  .j .j.j..Xjj....
-00000670: e809 1388 d86a c7d7 d8d8 88d8 d7c7 0000  .....j..........
-00000680: d7d7 d7d7 0000 0a00 0000 f600 0000 0400  ................
-00000690: 1000 1500 f1ff faff 0300 0000 e803 d006  ................
-000006a0: e00c 01c6 8811 e013 04c9 caca c988 26e8  ..............&.
-000006b0: 1304 cbcb caca c03e 04c8 c8c9 c8e0 1205  .......>........
-000006c0: cbcc cccc cbd0 1605 c8c9 1011 cbe0 2704  ..............'.
-000006d0: cccc cdcc e82c d849 e037 0211 13e8 07e8  .....,.I.7......
-000006e0: 2904 cbca 1515 d828 e04b e836 08cc cdcb  )......(.K.6....
-000006f0: cb15 1315 17e8 1505 10c9 14ca cae8 4904  ..............I.
-00000700: cb13 cdcc e812 0a16 0d0c 2800 12cb cb12  ..........(.....
-00000710: 14e8 7313 13cd cd12 0d15 170d 0b0a 21d7  ..s...........!.
-00000720: 88bf 2814 cbcc 13e8 1304 0e0f 130d e013  ..(.............
-00000730: 136a 0000 88d8 58bf f516 cccd 0e0e 0f0e  .j....X.........
-00000740: f50b 0a28 e813 0f00 00d8 886a 6a6a 0d0e  ...(.......jjj..
-00000750: 0f0f 0e0d 0b28 d013 0900 00d7 d888 8888  .....(..........
-00000760: 0c0e e813 c826 d815 0ad7 d8d8 d8f5 0b0c  .....&..........
-00000770: 2058 d8a9 1c08 d7d7 d7d7 10c9 c8d7 892f   X............./
-00000780: e8fa 8941 0b00 0000 3501 0000 0400 0c00  ...A....5.......
-00000790: 2000 f0ff f8ff 0800 0000 0000 c7c7 c7e8   ...............
-000007a0: 03e8 0604 2028 c7c7 d812 d817 c00a 0fd8  .... (..........
-000007b0: c7c8 c9ca caca cbcb cbc9 c9cb cb12 8821  ...............!
-000007c0: 04c9 c910 c8e0 1c0f cbcc cccc 2028 cccd  ............ (..
-000007d0: 13c8 c8c6 c6c6 c6d0 5408 0000 beca ca11  ........T.......
-000007e0: c9c9 e840 e023 e843 03ca 15c8 e046 d80b  ...@.#.C.....F..
-000007f0: 16cb ca88 5821 caca 1212 11ca 12cb 12cc  ....X!..........
-00000800: 13cc 13cd 14cd 17e8 2de8 4b0f cdcd cdcc  ........-.K.....
-00000810: cdcc 886a be13 13c9 1211 cbe0 2001 14e8  ...j........ ...
-00000820: 14e8 1701 cbb8 4c07 cbca d8d8 21f5 f5d0  ......L.....!...
-00000830: 7ce8 7f07 cccd caca ccca cbe8 03d0 06e8  |...............
-00000840: 9107 d728 1515 0b0b 0be8 03e0 0608 0e11  ...(............
-00000850: 130e 1214 0f13 e803 0215 0ee8 0305 0c6a  ...............j
-00000860: d720 f5a8 200b 0d12 130d 1415 0d14 160e  . .. ...........
-00000870: 15e8 0306 160e 0c58 d7d7 e861 030a 0a0a  .......X...a....
-00000880: e803 e006 0220 21b0 0ce0 1611 d800 c611  ..... !.........
-00000890: 2120 2821 2121 2828 f5f5 f5f5 20e8 8fe0  ! (!!!((.... ...
-000008a0: 08d0 0602 f528 e820 06c8 d788 88d7 d7e8  .....(. ........
-000008b0: 0506 2020 2020 6a6a e006 e00a d808 0258  ..    jj.......X
-000008c0: 6a0c 0000 00e4 0000 0004 000f 0015 00fa  j...............
-000008d0: fff9 ff08 0000 0000 c6c7 c8c8 e008 e00c  ................
-000008e0: c808 07c7 c9ca caca cac9 9817 0a10 c6c8  ................
-000008f0: cacb cbcb ca12 88b0 2e09 8888 10c8 c8cb  ................
-00000900: cb13 88e8 0401 12c0 4506 d812 11c8 10ca  ........E.......
-00000910: e82c 0516 14cb 14ca c015 0f21 2112 c9ca  .,.........!!...
-00000920: 10cb cb15 cbca c9c9 cac9 d02a 0620 2021  ...........*.  !
-00000930: 2113 c8e8 1702 cac9 e85c e872 e090 01c8  !........\.r....
-00000940: e016 0111 e859 01c9 e829 e017 01c9 e82e  .....Y...)......
-00000950: 09c6 d758 2020 6a11 1010 d016 e01a e05b  ...X  j........[
-00000960: 0ad7 586a 6a20 2011 2110 c9e8 2e03 cad8  ..Xjj  .!.......
-00000970: d8d8 1505 0000 5858 6ae0 4402 2810 e86b  ......XXj.D.(..k
-00000980: 0310 d8d8 c0df e816 0b20 2128 1228 cac9  ......... !(.(..
-00000990: d8d8 d7d8 b8f4 d017 e829 03d7 d7d7 a909  .........)......
-000009a0: e044 01c8 e814 891c 0258 88d0 260d 0000  .D.......X..&...
-000009b0: 0083 0000 0004 0017 0008 00fd fff5 ff07  ................
-000009c0: 00d7 d7d7 d788 d7e0 0704 88d7 8858 c807  .............X..
-000009d0: 026a 88d8 0f01 88e0 08e8 0702 586a e819  .j..........Xj..
-000009e0: d818 e008 e81f d810 e826 0120 d008 016a  .........&. ...j
-000009f0: c808 8810 9020 e845 d008 e807 e838 07c7  ..... .E.....8..
-00000a00: c8d7 d7cb cb6a e807 e875 09cb cbc8 c9d7  .....j...u......
-00000a10: 8381 d7ca e008 0284 83e8 0802 c7c9 e08e  ................
-00000a20: e808 01c8 e887 e010 02c7 58e8 9d05 cacb  ..........X.....
-00000a30: 8888 88e8 0302 8888 0e00 0000 cb00 0000  ................
-00000a40: 0400 1100 1600 f2ff f7ff 0300 0000 e803  ................
-00000a50: d006 e80c 03d7 d788 8812 d814 0488 5858  ..............XX
-00000a60: 5888 2807 8858 6a58 6a20 20a8 17e0 28d0  X.(..XjXj  ...(.
-00000a70: 14e8 1ba8 28e8 0fe8 28e8 4402 810c 9814  ....(...(.D.....
-00000a80: 046a 5888 d7e8 1401 83e0 16e8 78e0 52b0  .jX.........x.R.
-00000a90: 1402 cacb d014 0188 a828 04cb c9ca cbe8  .........(......
-00000aa0: 8c01 d7a0 140b c9c9 caca 5858 c8c8 d7d7  ..........XX....
-00000ab0: 6ab0 1401 cae0 1408 6a21 c8d7 58d7 d758  j.......j!..X..X
-00000ac0: e078 d028 0cc9 c96a 2100 00c8 d783 81d7  .x.(...j!.......
-00000ad0: c7d8 64d8 14d0 f106 c7d7 8483 d7c7 e878  ..d............x
-00000ae0: e815 c014 e016 0488 58d7 c8e8 3901 c9b0  ........X...9...
-00000af0: 14d1 1106 d7c8 c9c9 5858 912d 04d7 d7d7  ........XX.-....
-00000b00: c8e0 7889 54e9 5588 1401 000f 0000 00ed  ..x.T.U.........
-00000b10: 0000 0004 000c 0020 00f0 fff8 ff05 0000  ....... ........
-00000b20: d7d7 d7e8 03d0 06a0 0cd8 18d8 1f03 88d7  ................
-00000b30: 88e0 05d8 09e0 0ae0 0703 8888 58e8 03e8  ............X...
-00000b40: 05d0 1ce0 1402 5858 e810 e004 e808 0388  ......XX........
-00000b50: 586a e80f 036a 6a6a e03a e819 e81c e80f  Xj...jjj.:......
-00000b60: e013 d808 016a e004 016a e808 0120 e85c  .....j...j... .\
-00000b70: e826 e829 d006 b00c 0320 2020 e803 0120  .&.).....   ... 
-00000b80: e06f c86d c047 b809 e062 07d7 c90a 8483  .o.m.G...b......
-00000b90: 810c e004 c008 a010 01cb e820 0385 8483  ........... ....
-00000ba0: e004 c008 c010 010c e004 07cb d7c8 c8c9  ................
-00000bb0: c9c9 e803 03ca caca e803 d006 b80c 03cb  ................
-00000bc0: cbd7 c808 01cb e803 d806 01cc e004 02cc  ................
-00000bd0: cce8 03e8 0603 cdcd 00e8 f8e1 0c02 d7d7  ................
-00000be0: d047 d04d 01c9 e0f6 d817 0300 0021 e90a  .G.M.........!..
-00000bf0: 0721 6a00 0000 0000 e112 e116 e00d c817  .!j.............
-00000c00: 1000 0000 bd00 0000 0400 1100 1600 faff  ................
-00000c10: f7ff 0700 0000 0058 6a6a e007 e00b c008  .......Xjj......
-00000c20: 0500 88d7 8858 8818 d815 01d7 e018 0120  .....X......... 
-00000c30: a030 03d7 d7d7 e815 02d7 8890 1802 f581  .0..............
-00000c40: b018 016a b830 0328 830a b818 e85f c848  ...j.0.(....._.H
-00000c50: 03c7 c9f5 b818 0558 886a 5820 d860 03c8  .......X.jX .`..
-00000c60: c8c9 a018 0158 d018 02d7 d7e8 1701 c9b0  .....X..........
-00000c70: 48e8 bc05 6ac9 6a6a 58d8 1801 c8b8 60e8  H...j.jjX.....`.
-00000c80: 1006 c9cb 0000 6a58 e046 c018 01ca e018  ......jX.F......
-00000c90: e816 e0b5 d818 d878 04ca d781 83c8 16a8  .......x........
-00000ca0: 1804 cad7 8384 b816 b830 04ca d758 88a8  .........0...X..
-00000cb0: 16d8 fde0 1601 88e9 18a1 43e0 90e8 6e98  ..........C...n.
-00000cc0: 14c0 18e1 7211 0000 0083 0000 0004 0017  ....r...........
-00000cd0: 0008 00fd fff5 ff07 00d7 d7d7 d788 d7e0  ................
-00000ce0: 0704 88d7 8858 c807 026a 88d8 0f01 88e0  .....X...j......
-00000cf0: 08e8 0702 586a e819 d818 e008 e81f d810  ....Xj..........
-00000d00: e826 0120 d008 016a c808 8810 9020 e845  .&. ...j..... .E
-00000d10: d008 e807 e838 07c7 c8d7 d7cb cb6a e807  .....8.......j..
-00000d20: e875 09cb cbc8 c9d7 8381 d7ca e008 0284  .u..............
-00000d30: 83e8 0802 c7c9 e08e e808 01c8 e887 e010  ................
-00000d40: 02c7 58e8 9d05 cacb 8888 88e8 0302 8888  ..X.............
-00000d50: 1200 0000 cb00 0000 0400 1100 1600 f2ff  ................
-00000d60: f7ff 0300 0000 e803 d006 e80c 03d7 d788  ................
-00000d70: 8812 d814 0488 5858 5888 2807 8858 6a58  ......XXX.(..XjX
-00000d80: 6a20 20a8 17e0 28d0 14e8 1ba8 28e8 0fe8  j  ...(.....(...
-00000d90: 28e8 4402 810c 9814 046a 5888 d7e8 1401  (.D......jX.....
-00000da0: 83e0 16e8 78e0 52b0 1402 cacb d014 0188  ....x.R.........
-00000db0: a828 04cb c9ca cbe8 8c01 d7a0 140b c9c9  .(..............
-00000dc0: caca 5858 c8c8 d7d7 6ab0 1401 cae0 1408  ..XX....j.......
-00000dd0: 6a21 c8d7 58d7 d758 e078 d028 0cc9 c96a  j!..X..X.x.(...j
-00000de0: 2100 00c8 d783 81d7 c7d8 64d8 14d0 f106  !.........d.....
-00000df0: c7d7 8483 d7c7 e878 e815 c014 e016 0488  .......x........
-00000e00: 58d7 c8e8 3901 c9b0 14d1 1106 d7c8 c9c9  X...9...........
-00000e10: 5858 912d 04d7 d7d7 c8e0 7889 54e9 5588  XX.-......x.T.U.
-00000e20: 1401 0013 0000 00ed 0000 0004 000c 0020  ............... 
-00000e30: 00f0 fff8 ff05 0000 d7d7 d7e8 03d0 06a0  ................
-00000e40: 0cd8 18d8 1f03 88d7 88e0 05d8 09e0 0ae0  ................
-00000e50: 0703 8888 58e8 03e8 05d0 1ce0 1402 5858  ....X.........XX
-00000e60: e810 e004 e808 0388 586a e80f 036a 6a6a  ........Xj...jjj
-00000e70: e03a e819 e81c e80f e013 d808 016a e004  .:...........j..
-00000e80: 016a e808 0120 e85c e826 e829 d006 b00c  .j... .\.&.)....
-00000e90: 0320 2020 e803 0120 e06f c86d c047 b809  .   ... .o.m.G..
-00000ea0: e062 07d7 c90a 8483 810c e004 c008 a010  .b..............
-00000eb0: 01cb e820 0385 8483 e004 c008 c010 010c  ... ............
-00000ec0: e004 07cb d7c8 c8c9 c9c9 e803 03ca caca  ................
-00000ed0: e803 d006 b80c 03cb cbd7 c808 01cb e803  ................
-00000ee0: d806 01cc e004 02cc cce8 03e8 0603 cdcd  ................
-00000ef0: 00e8 f8e1 0c02 d7d7 d047 d04d 01c9 e0f6  .........G.M....
-00000f00: d817 0300 0021 e90a 0721 6a00 0000 0000  .....!...!j.....
-00000f10: e112 e116 e00d c817 1400 0000 bd00 0000  ................
-00000f20: 0400 1100 1600 faff f7ff 0700 0000 0058  ...............X
-00000f30: 6a6a e007 e00b c008 0500 88d7 8858 8818  jj...........X..
-00000f40: d815 01d7 e018 0120 a030 03d7 d7d7 e815  ....... .0......
-00000f50: 02d7 8890 1802 f581 b018 016a b830 0328  ...........j.0.(
-00000f60: 830a b818 e85f c848 03c7 c9f5 b818 0558  ....._.H.......X
-00000f70: 886a 5820 d860 03c8 c8c9 a018 0158 d018  .jX .`.......X..
-00000f80: 02d7 d7e8 1701 c9b0 48e8 bc05 6ac9 6a6a  ........H...j.jj
-00000f90: 58d8 1801 c8b8 60e8 1006 c9cb 0000 6a58  X.....`.......jX
-00000fa0: e046 c018 01ca e018 e816 e0b5 d818 d878  .F.............x
-00000fb0: 04ca d781 83c8 16a8 1804 cad7 8384 b816  ................
-00000fc0: b830 04ca d758 88a8 16d8 fde0 1601 88e9  .0...X..........
-00000fd0: 18a1 43e0 90e8 6e98 14c0 18e1 7215 0000  ..C...n.....r...
-00000fe0: 0066 0000 0004 0015 0008 00fd fff6 ff10  .f..............
-00000ff0: 00c8 c8c9 c9c9 c900 c7c9 caca cbca cac9  ................
-00001000: e808 02cb cce8 0901 c6d0 0801 c9c8 0888  ................
-00001010: 1088 2088 3088 40d8 5003 c7c8 c8e8 5e02  .. .0.@.P.....^.
-00001020: c9ca e86e e069 e80a 03cb d7d7 d872 05d7  ...n.i.......r..
-00001030: d8d7 d712 e81b e008 0410 c8c7 c7e0 1005  ................
-00001040: d8c6 d7d7 d7e8 03d0 06e0 0c16 0000 00b7  ................
-00001050: 0000 0004 000f 0014 00f3 fff9 ff03 0000  ................
-00001060: 00e8 03d0 06e8 0c01 c688 10e8 1204 c9ca  ................
-00001070: cac9 8812 06ca cacb cbca cab0 3b01 c7d8  ............;...
-00001080: 1204 cccc cccb c015 c012 02cd cce8 2aa8  ..............*.
-00001090: 36e0 12e8 2602 1515 8812 05ca 1315 1715  6...&...........
-000010a0: 8812 080d 160d 0c28 c7c7 c8e8 6ec0 360b  .......(....n.6.
-000010b0: 160d 0b0a 21d7 1010 d8c8 c8e8 7006 cbca  ....!.......p...
-000010c0: 0d14 160a e812 096a 0000 10d7 d7d8 c9c9  .......j........
-000010d0: e848 0516 0d0d 0af5 e012 0a00 00d8 d7d7  .H..............
-000010e0: d710 c715 0fe0 3601 20d8 1202 0000 e813  ......6. .......
-000010f0: 04d7 d810 17e0 48c8 12c8 1605 c60c 0a21  ......H........!
-00001100: 2091 0e04 d7d7 88d7 a120 1700 0000 c500   ........ ......
-00001110: 0000 0400 0a00 1c00 f4ff faff 05c6 c6c7  ................
-00001120: c7c7 e803 d806 c80d c813 0600 caca cbcb  ................
-00001130: cbe8 03d0 06b0 0c0c cacb cad8 cacb cccd  ................
-00001140: cdcd cccc d006 01cc e80a e80d d812 01cb  ................
-00001150: e81c e024 883c d03a 0188 e034 04cd cdcb  ...$.<.:...4....
-00001160: cce8 40e8 47d8 06d0 0c12 cccc 200f 1413  ..@.G....... ...
-00001170: 0e14 120d 1311 0c12 100c 1010 e006 1112  ................
-00001180: 110d 1312 0f13 0f21 0f16 140d 1513 0c14  .......!........
-00001190: e803 0413 0c13 12c8 090d 1514 0e14 0e20  ............... 
-000011a0: 0b0b 0b0b 0a0a 0ae8 03e8 0602 2821 b80b  ............(!..
-000011b0: e818 0688 2821 f5f5 f5e8 03d8 0602 2120  ....(!........! 
-000011c0: a80c 0928 88d8 d758 5820 2020 e803 d006  ...(...XX   ....
-000011d0: c00c 0458 d7d8 6a18 0000 00b8 0000 0004  ...X..j.........
-000011e0: 0010 0014 00fa fff9 ff05 0000 0000 c9e0  ................
-000011f0: 05e0 09c0 0805 00ca caca ca88 1605 cacb  ................
-00001200: cbcb cb90 1603 c9c9 ca88 1604 0000 11c9  ................
-00001210: 8816 e861 0312 f510 8816 0600 0028 2811  ...a.........((.
-00001220: 2888 1604 0058 2121 e816 0211 c8e0 58e0  (....X!!......X.
-00001230: 6f0c cac9 c900 d758 2020 2128 2111 e042  o......X  !(!..B
-00001240: e86f d81b e82a 056a 2020 206a e042 e02d  .o...*.j   j.B.-
-00001250: 02d8 d8e0 14e0 1602 6a6a e042 0113 e899  ........jj.B....
-00001260: 0410 d8d8 c8d0 d701 58d8 4208 2828 cac9  ........X.B.((..
-00001270: d8d8 d7d8 c0eb e042 0228 14e8 2703 d7d7  .......B.(..'...
-00001280: d7b0 ffe8 5803 2110 c698 13e9 2101 d7e8  ....X.!.....!...
-00001290: 3990 12d8 16d9 3619 0000 0066 0000 0004  9.....6....f....
-000012a0: 0015 0008 00fd fff6 ff10 00c8 c8c9 c9c9  ................
-000012b0: c900 c7c9 caca cbca cac9 e808 02cb cce8  ................
-000012c0: 0901 c6d0 0801 c9c8 0888 1088 2088 3088  ............ .0.
-000012d0: 40d8 5003 c7c8 c8e8 5e02 c9ca e86e e069  @.P.....^....n.i
-000012e0: e80a 03cb d7d7 d872 05d7 d8d7 d712 e81b  .......r........
-000012f0: e008 0410 c8c7 c7e0 1005 d8c6 d7d7 d7e8  ................
-00001300: 03d0 06e0 0c1a 0000 00b7 0000 0004 000f  ................
-00001310: 0014 00f1 fffa ff03 0000 00e8 03d0 06e8  ................
-00001320: 0c01 c688 10e8 1204 c9ca cac9 8812 06ca  ................
-00001330: cacb cbca cab0 3b01 c7d8 1204 cccc cccb  ......;.........
-00001340: c015 c012 02cd cce8 2aa8 36e0 12e8 2602  ........*.6...&.
-00001350: 1515 8812 05ca 1315 1715 8812 080d 160d  ................
-00001360: 0c28 c7c7 c8e8 6ec0 360b 160d 0b0a 21d7  .(....n.6.....!.
-00001370: 1010 d8c8 c8e8 7006 cbca 0d14 160a e812  ......p.........
-00001380: 096a 0000 10d7 d7d8 c9c9 e848 0516 0d0d  .j.........H....
-00001390: 0af5 e012 0a00 00d8 d7d7 d710 c715 0fe0  ................
-000013a0: 3601 20d8 1202 0000 e813 04d7 d810 17e0  6. .............
-000013b0: 48c8 12c8 1605 c60c 0a21 2091 0e04 d7d7  H........! .....
-000013c0: 88d7 a120 1b00 0000 c500 0000 0400 0a00  ... ............
-000013d0: 1c00 f0ff faff 05c6 c6c7 c7c7 e803 d806  ................
-000013e0: c80d c813 0600 caca cbcb cbe8 03d0 06b0  ................
-000013f0: 0c0c cacb cad8 cacb cccd cdcd cccc d006  ................
-00001400: 01cc e80a e80d d812 01cb e81c e024 883c  .............$.<
-00001410: d03a 0188 e034 04cd cdcb cce8 40e8 47d8  .:...4......@.G.
-00001420: 06d0 0c12 cccc 200f 1413 0e14 120d 1311  ...... .........
-00001430: 0c12 100c 1010 e006 1112 110d 1312 0f13  ................
-00001440: 0f21 0f16 140d 1513 0c14 e803 0413 0c13  .!..............
-00001450: 12c8 090d 1514 0e14 0e20 0b0b 0b0b 0a0a  ......... ......
-00001460: 0ae8 03e8 0602 2821 b80b e818 0688 2821  ......(!......(!
-00001470: f5f5 f5e8 03d8 0602 2120 a80c 0928 88d8  ........! ...(..
-00001480: d758 5820 2020 e803 d006 c00c 0458 d7d8  .XX   .......X..
-00001490: 6a1c 0000 00b8 0000 0004 0010 0014 00fa  j...............
-000014a0: fff9 ff05 0000 0000 c9e0 05e0 09c0 0805  ................
-000014b0: 00ca caca ca88 1605 cacb cbcb cb90 1603  ................
-000014c0: c9c9 ca88 1604 0000 11c9 8816 e861 0312  .............a..
-000014d0: f510 8816 0600 0028 2811 2888 1604 0058  .......((.(....X
-000014e0: 2121 e816 0211 c8e0 58e0 6f0c cac9 c900  !!......X.o.....
-000014f0: d758 2020 2128 2111 e042 e86f d81b e82a  .X  !(!..B.o...*
-00001500: 056a 2020 206a e042 e02d 02d8 d8e0 14e0  .j   j.B.-......
-00001510: 1602 6a6a e042 0113 e899 0410 d8d8 c8d0  ..jj.B..........
-00001520: d701 58d8 4208 2828 cac9 d8d8 d7d8 c0eb  ..X.B.((........
-00001530: e042 0228 14e8 2703 d7d7 d7b0 ffe8 5803  .B.(..'.......X.
-00001540: 2110 c698 13e9 2101 d7e8 3990 12d8 16d9  !.....!...9.....
-00001550: 3600 0000 00                             6....
+00000000: 0400 ff23 0000 002e 00ff 1443 494e 464f  ...#.......CINFO
+00000010: 4256 5253 4e04 0000 0000 0042 4d49 4e56  BVRSN......BMINV
+00000020: 0400 0000 0000 424e 5041 5201 0000 4250  ......BNPAR...BP
+00000030: 414c 5301 0057 0000 3400 ff08 0774 6573  ALS..W..4....tes
+00000040: 744e 4d4c 2072 6567 7265 7373 696f 6e20  tNML regression 
+00000050: 7465 7374 0041 2074 6573 7420 6e65 7767  test.A test newg
+00000060: 7266 2074 6573 7469 6e67 204e 4d4c 0006  rf testing NML..
+00000070: 00ff 0100 03ff 0800 b800 0116 0800 fdff  ................
+00000080: f6ff 0700 c6c8 c8c8 c8c7 e807 07ca caca  ................
+00000090: cac9 c8c6 e007 05cb cac9 c7cb e807 e804  ................
+000000a0: 11c8 1011 cbcc 1011 cac9 11ca cbcc cb12  ................
+000000b0: c9c9 e816 e818 0bcc 1414 ca14 13ca 1214  ................
+000000c0: cb13 e839 05c9 13cc c6c7 d82f 02ca c6e8  ...9......./....
+000000d0: 2101 cce8 40c8 08e0 1002 cccc e859 e060  !...@........Y.`
+000000e0: e050 02c7 c8e0 3003 c9ca c8e8 4ae0 68e8  .P....0.....J.h.
+000000f0: 5002 d7d7 e871 07ca c9d7 d8d7 d712 e81b  P....q..........
+00000100: e008 0410 c8c7 c7e0 1005 d8c6 d7d7 d7e8  ................
+00000110: 03d0 06e0 0c43 0101 0f15 00f2 fff9 ff03  .....C..........
+00000120: 0000 00e8 03d0 0605 00c7 c9c9 c898 11e0  ................
+00000130: 1306 caca cbcb cac9 a026 0288 12e8 13e8  .........&......
+00000140: 1502 cacc b839 0d13 12ca ca88 12cc cbca  .....9..........
+00000150: cc13 cc20 c04e 0412 ca11 12e8 2905 cc13  ... .N......)...
+00000160: cdcd 16d0 1502 c6c9 e862 01ca e83f e813  .........b...?..
+00000170: 0417 0d0d 58d8 13d0 610a c913 cccc 170d  ....X...a.......
+00000180: 0e0c 0cd8 c813 03cc cccd e83c 0b16 140e  ...........<....
+00000190: 0d0c 0ac9 00c7 c7c8 e889 03cc cdcc e864  ...............d
+000001a0: 0e13 0c15 0c0b 28d7 c700 1010 d8c8 c8e8  ......(.........
+000001b0: 610a cbca 160d 0c0b f50a 28d7 e8cf 0610  a.........(.....
+000001c0: d7d7 d8c9 c9e8 2606 160d 0d0c f521 d08e  ......&......!..
+000001d0: 08d8 d7d7 d710 c715 0fe8 2802 0a28 c0a1  ..........(..(..
+000001e0: e814 08d7 d810 170d 0b0a f5c0 b4c8 1703  ................
+000001f0: c60c 0ac8 39a0 1701 88e0 5fb1 317c 0101  ....9....._.1|..
+00000200: 0c1f 00f0 fff8 ff03 0000 00e8 03d0 0609  ................
+00000210: 00c7 c728 20c7 c9c7 c9e0 0401 c798 1ae0  ...( ...........
+00000220: 270f 10c9 c9c9 c9ca cacb cbcb cbcb cac9  '...............
+00000230: 12e0 3a06 c6c6 c6c7 c7c7 e803 08c8 c8c7  ..:.............
+00000240: 10c9 cb20 58d8 1d09 cccc cbca 13cb cb00  ... X...........
+00000250: 00c8 2ce8 2e03 c9c8 10e8 3be8 3c03 cccb  ..,.......;.<...
+00000260: cce0 4105 14cc ccbe 00e8 2903 cdcd cde8  ..A.......).....
+00000270: 10e8 2013 11ca 12cb 12cc 13cc 13cd 14cd  .. .............
+00000280: 1414 14cd cdf5 10e0 6ae8 3c01 cbe0 38e8  ........j.<...8.
+00000290: 4402 ccca d81d 0916 cd16 16cc 1616 be6a  D..............j
+000002a0: e83a e83f e042 e006 d84b c80c 09cd 0c0c  .:.?.B...K......
+000002b0: 2858 0c0e 1513 e803 020f 14e8 0308 120e  (X..............
+000002c0: 1311 0e0d 0d0d e803 e806 090e 1717 f588  ................
+000002d0: 0c0e 1615 e803 090e 1614 0d15 140d 1312  ................
+000002e0: b81e 020d 0ee8 3e05 d80a 0b0b 0be8 03d0  ......>.........
+000002f0: 0603 0b28 21b8 0f0a 0c0b 0a0a 58d7 2815  ...(!.......X.(.
+00000300: 1515 e803 d006 1b0a 2821 0a0a 0a0a f5f5  ........(!......
+00000310: 2828 28f5 2813 13c6 0058 2020 2020 2021  (((.(....X     !
+00000320: 2121 e803 0421 216a 6ae0 0a0b 8858 d7d7  !!...!!jj....X..
+00000330: d788 88d7 c8c6 0058 0101 1015 00fa fff9  .......X........
+00000340: ff05 0000 0000 c9e0 05e0 09c0 0806 0000  ................
+00000350: caca caca 8817 0600 cacb cbcb cb88 1703  ................
+00000360: c9c9 cae0 17e8 2d04 c8c9 c9c8 c848 0211  ......-......H..
+00000370: c9e0 17e0 1304 caca 1012 c817 0312 f510  ................
+00000380: e817 03c9 c6c8 e813 d031 e87b 0a28 2811  .........1.{.((.
+00000390: 2810 c9c6 1111 c8e8 5d01 cce0 5ee8 440a  (.......]...^.D.
+000003a0: 5821 2128 1112 11ca c910 e886 e817 1014  X!!(............
+000003b0: cc13 0000 d758 2020 2128 1228 20c9 cae0  .....X  !(.( ...
+000003c0: 1705 1615 cbcc 28e8 bc02 586a e816 0428  ......(...Xj...(
+000003d0: f5f5 14e0 5706 cccc cc16 bf6a e0d2 1158  ....W......j...X
+000003e0: 6a21 2120 f515 f514 caca cc0c bf6a 2821  j!! .........j(!
+000003f0: d0e2 0358 6a6a e82d 0815 0a0a 0c6a 2058  ...Xjj.-.....j X
+00000400: 20d8 2ad8 2ee8 5a09 f50a 0b0a 5858 6a58   .*...Z.....XXjX
+00000410: d8b1 0c03 d888 58e8 5a05 d8d8 88d8 d7a1  ......X.Z.......
+00000420: 2107 d7c6 c888 d7d7 d798 14e1 4601 c6d9  !...........F...
+00000430: 46c8 0001 1808 00fd fff6 ff10 00c8 c8c9  F...............
+00000440: c9c9 c900 c7c9 caca cbca cac9 e808 02cb  ................
+00000450: cce8 09c8 0802 c9c8 c810 e808 02cc ccd0  ................
+00000460: 20e8 2603 caca c6d8 370b c9c9 c610 11ca   .&.....7.......
+00000470: cb10 11c9 c7e8 0703 cccb 12e0 28d8 38e0  ............(.8.
+00000480: 4f01 cbe0 51e8 2fe8 5a0a c9ca 11cb 1314  O...Q./.Z.......
+00000490: cc0c cb11 e808 0715 cc0c 16c8 c9cb c860  ...............`
+000004a0: 02cb cce8 5923 cbc8 280a 0b0b 0c0e cb20  ....Y#..(...... 
+000004b0: 6abf 5821 bf13 0c20 8888 6a20 136a 0b6a  j.X!... ..j .j.j
+000004c0: d888 586a 6a88 1588 d7e8 0913 88d8 6ac7  ..Xjj.........j.
+000004d0: d7d8 d888 d8d7 c700 00d7 d7d7 d700 0058  ...............X
+000004e0: 0101 1015 00f1 fffa ff03 0000 00e8 03d0  ................
+000004f0: 06e0 0c01 c688 11e0 1304 c9ca cac9 8826  ...............&
+00000500: e813 04cb cbca cac0 3e04 c8c8 c9c8 e012  ........>.......
+00000510: 05cb cccc cccb d016 05c8 c910 11cb e027  ...............'
+00000520: 04cc cccd cce8 2cd8 49e0 3702 1113 e807  ......,.I.7.....
+00000530: e829 04cb ca15 15d8 28e0 4be8 3608 cccd  .)......(.K.6...
+00000540: cbcb 1513 1517 e815 0510 c914 caca e849  ...............I
+00000550: 04cb 13cd cce8 120a 160d 0c28 0012 cbcb  ...........(....
+00000560: 1214 e873 1313 cdcd 120d 1517 0d0b 0a21  ...s...........!
+00000570: d788 bf28 14cb cc13 e813 040e 0f13 0de0  ...(............
+00000580: 1313 6a00 0088 d858 bff5 16cc cd0e 0e0f  ..j....X........
+00000590: 0ef5 0b0a 28e8 130f 0000 d888 6a6a 6a0d  ....(.......jjj.
+000005a0: 0e0f 0f0e 0d0b 28d0 1309 0000 d7d8 8888  ......(.........
+000005b0: 880c 0ee8 13c8 26d8 150a d7d8 d8d8 f50b  ......&.........
+000005c0: 0c20 58d8 a91c 08d7 d7d7 d710 c9c8 d789  . X.............
+000005d0: 2fe8 fa89 4188 0101 0c20 00f0 fff8 ff08  /...A.... ......
+000005e0: 0000 0000 00c7 c7c7 e803 e806 0420 28c7  ............. (.
+000005f0: c7d8 12d8 17c0 0a0f d8c7 c8c9 caca cacb  ................
+00000600: cbcb c9c9 cbcb 1288 2104 c9c9 10c8 e01c  ........!.......
+00000610: 0fcb cccc cc20 28cc cd13 c8c8 c6c6 c6c6  ..... (.........
+00000620: d054 0800 00be caca 11c9 c9e8 40e0 23e8  .T..........@.#.
+00000630: 4303 ca15 c8e0 46d8 0b16 cbca 8858 21ca  C.....F......X!.
+00000640: ca12 1211 ca12 cb12 cc13 cc13 cd14 cd17  ................
+00000650: e82d e84b 0fcd cdcd cccd cc88 6abe 1313  .-.K........j...
+00000660: c912 11cb e020 0114 e814 e817 01cb b84c  ..... .........L
+00000670: 07cb cad8 d821 f5f5 d07c e87f 07cc cdca  .....!...|......
+00000680: cacc cacb e803 d006 e891 07d7 2815 150b  ............(...
+00000690: 0b0b e803 e006 080e 1113 0e12 140f 13e8  ................
+000006a0: 0302 150e e803 050c 6ad7 20f5 a820 0b0d  ........j. .. ..
+000006b0: 1213 0d14 150d 1416 0e15 e803 0616 0e0c  ................
+000006c0: 58d7 d7e8 6103 0a0a 0ae8 03e0 0602 2021  X...a......... !
+000006d0: b00c e016 11d8 00c6 1121 2028 2121 2128  .........! (!!!(
+000006e0: 28f5 f5f5 f520 e88f e008 d006 02f5 28e8  (.... ........(.
+000006f0: 2006 c8d7 8888 d7d7 e805 0620 2020 206a   ..........    j
+00000700: 6ae0 06e0 0ad8 0802 586a 4301 010f 1500  j.......XjC.....
+00000710: faff f9ff 0800 0000 00c6 c7c8 c8e0 08e0  ................
+00000720: 0cc8 0807 c7c9 caca caca c998 170a 10c6  ................
+00000730: c8ca cbcb cbca 1288 b02e 0988 8810 c8c8  ................
+00000740: cbcb 1388 e804 0112 c045 06d8 1211 c810  .........E......
+00000750: cae8 2c05 1614 cb14 cac0 150f 2121 12c9  ..,.........!!..
+00000760: ca10 cbcb 15cb cac9 c9ca c9d0 2a06 2020  ............*.  
+00000770: 2121 13c8 e817 02ca c9e8 5ce8 72e0 9001  !!........\.r...
+00000780: c8e0 1601 11e8 5901 c9e8 29e0 1701 c9e8  ......Y...).....
+00000790: 2e09 c6d7 5820 206a 1110 10d0 16e0 1ae0  ....X  j........
+000007a0: 5b0a d758 6a6a 2020 1121 10c9 e82e 03ca  [..Xjj  .!......
+000007b0: d8d8 d815 0500 0058 586a e044 0228 10e8  .......XXj.D.(..
+000007c0: 6b03 10d8 d8c0 dfe8 160b 2021 2812 28ca  k......... !(.(.
+000007d0: c9d8 d8d7 d8b8 f4d0 17e8 2903 d7d7 d7a9  ..........).....
+000007e0: 09e0 4401 c8e8 1489 1c02 5888 d026 c800  ..D.......X..&..
+000007f0: 0118 0800 fdff f4ff 0300 0000 e803 e806  ................
+00000800: 06d7 d7d7 d788 d7e0 0704 88d7 8858 c807  .............X..
+00000810: 026a 88d8 0f01 88e0 08e8 0702 586a e819  .j..........Xj..
+00000820: d818 e008 e81f d810 e826 0120 d008 016a  .........&. ...j
+00000830: c808 8810 9020 e845 d008 e807 e838 07c7  ..... .E.....8..
+00000840: c8d7 d7cb cb6a e807 e875 09cb cbc8 c9d7  .....j...u......
+00000850: 8381 d7ca e008 0284 83e8 0802 c7c9 e08e  ................
+00000860: e808 01c8 e887 e010 02c7 58e8 9d05 cacb  ..........X.....
+00000870: 8888 88e8 0302 8888 7e01 0111 1600 f2ff  ........~.......
+00000880: f7ff 0300 0000 e803 d006 e80c 03d7 d788  ................
+00000890: 8812 d814 0488 5858 5888 2807 8858 6a58  ......XXX.(..XjX
+000008a0: 6a20 20a8 17e0 28d0 14e8 1ba8 28e8 0fe8  j  ...(.....(...
+000008b0: 28e8 4402 810c 9814 046a 5888 d7e8 1401  (.D......jX.....
+000008c0: 83e0 16e8 78e0 52b0 1402 cacb d014 0188  ....x.R.........
+000008d0: a828 04cb c9ca cbe8 8c01 d7a0 140b c9c9  .(..............
+000008e0: caca 5858 c8c8 d7d7 6ab0 1401 cae0 1408  ..XX....j.......
+000008f0: 6a21 c8d7 58d7 d758 e078 d028 0cc9 c96a  j!..X..X.x.(...j
+00000900: 2100 00c8 d783 81d7 c7d8 64d8 14d0 f106  !.........d.....
+00000910: c7d7 8483 d7c7 e878 e815 c014 e016 0488  .......x........
+00000920: 58d7 c8e8 3901 c9b0 14d1 1106 d7c8 c9c9  X...9...........
+00000930: 5858 912d 04d7 d7d7 c8e0 7889 54e9 5588  XX.-......x.T.U.
+00000940: 1401 0088 0101 0c20 00f0 fff8 ff05 0000  ....... ........
+00000950: d7d7 d7e8 03d0 06a0 0cd8 18d8 1f03 88d7  ................
+00000960: 88e0 05d8 09e0 0ae0 0703 8888 58e8 03e8  ............X...
+00000970: 05d0 1ce0 1402 5858 e810 e004 e808 0388  ......XX........
+00000980: 586a e80f 036a 6a6a e03a e819 e81c e80f  Xj...jjj.:......
+00000990: e013 d808 016a e004 016a e808 0120 e85c  .....j...j... .\
+000009a0: e826 e829 d006 b00c 0320 2020 e803 0120  .&.).....   ... 
+000009b0: e06f c86d c047 b809 e062 07d7 c90a 8483  .o.m.G...b......
+000009c0: 810c e004 c008 a010 01cb e820 0385 8483  ........... ....
+000009d0: e004 c008 c010 010c e004 07cb d7c8 c8c9  ................
+000009e0: c9c9 e803 03ca caca e803 d006 b80c 03cb  ................
+000009f0: cbd7 c808 01cb e803 d806 01cc e004 02cc  ................
+00000a00: cce8 03e8 0603 cdcd 00e8 f8e1 0c02 d7d7  ................
+00000a10: d047 d04d 01c9 e0f6 d817 0300 0021 e90a  .G.M.........!..
+00000a20: 0721 6a00 0000 0000 e112 e116 e00d c817  .!j.............
+00000a30: 7e01 0111 1600 faff f7ff 0700 0000 0058  ~..............X
+00000a40: 6a6a e007 e00b c008 0500 88d7 8858 8818  jj...........X..
+00000a50: d815 01d7 e018 0120 a030 03d7 d7d7 e815  ....... .0......
+00000a60: 02d7 8890 1802 f581 b018 016a b830 0328  ...........j.0.(
+00000a70: 830a b818 e85f c848 03c7 c9f5 b818 0558  ....._.H.......X
+00000a80: 886a 5820 d860 03c8 c8c9 a018 0158 d018  .jX .`.......X..
+00000a90: 02d7 d7e8 1701 c9b0 48e8 bc05 6ac9 6a6a  ........H...j.jj
+00000aa0: 58d8 1801 c8b8 60e8 1006 c9cb 0000 6a58  X.....`.......jX
+00000ab0: e046 c018 01ca e018 e816 e0b5 d818 d878  .F.............x
+00000ac0: 04ca d781 83c8 16a8 1804 cad7 8384 b816  ................
+00000ad0: b830 04ca d758 88a8 16d8 fde0 1601 88e9  .0...X..........
+00000ae0: 18a1 43e0 90e8 6e98 14c0 18e1 72c8 0001  ..C...n.....r...
+00000af0: 1808 00fd fff4 ff03 0000 00e8 03e8 0606  ................
+00000b00: d7d7 d7d7 88d7 e007 0488 d788 58c8 0702  ............X...
+00000b10: 6a88 d80f 0188 e008 e807 0258 6ae8 19d8  j..........Xj...
+00000b20: 18e0 08e8 1fd8 10e8 2601 20d0 0801 6ac8  ........&. ...j.
+00000b30: 0888 1090 20e8 45d0 08e8 07e8 3807 c7c8  .... .E.....8...
+00000b40: d7d7 cbcb 6ae8 07e8 7509 cbcb c8c9 d783  ....j...u.......
+00000b50: 81d7 cae0 0802 8483 e808 02c7 c9e0 8ee8  ................
+00000b60: 0801 c8e8 87e0 1002 c758 e89d 05ca cb88  .........X......
+00000b70: 8888 e803 0288 887e 0101 1116 00f2 fff7  .......~........
+00000b80: ff03 0000 00e8 03d0 06e8 0c03 d7d7 8888  ................
+00000b90: 12d8 1404 8858 5858 8828 0788 586a 586a  .....XXX.(..XjXj
+00000ba0: 2020 a817 e028 d014 e81b a828 e80f e828    ...(.....(...(
+00000bb0: e844 0281 0c98 1404 6a58 88d7 e814 0183  .D......jX......
+00000bc0: e016 e878 e052 b014 02ca cbd0 1401 88a8  ...x.R..........
+00000bd0: 2804 cbc9 cacb e88c 01d7 a014 0bc9 c9ca  (...............
+00000be0: ca58 58c8 c8d7 d76a b014 01ca e014 086a  .XX....j.......j
+00000bf0: 21c8 d758 d7d7 58e0 78d0 280c c9c9 6a21  !..X..X.x.(...j!
+00000c00: 0000 c8d7 8381 d7c7 d864 d814 d0f1 06c7  .........d......
+00000c10: d784 83d7 c7e8 78e8 15c0 14e0 1604 8858  ......x........X
+00000c20: d7c8 e839 01c9 b014 d111 06d7 c8c9 c958  ...9...........X
+00000c30: 5891 2d04 d7d7 d7c8 e078 8954 e955 8814  X.-......x.T.U..
+00000c40: 0100 8801 010c 2000 f0ff f8ff 0500 00d7  ...... .........
+00000c50: d7d7 e803 d006 a00c d818 d81f 0388 d788  ................
+00000c60: e005 d809 e00a e007 0388 8858 e803 e805  ...........X....
+00000c70: d01c e014 0258 58e8 10e0 04e8 0803 8858  .....XX........X
+00000c80: 6ae8 0f03 6a6a 6ae0 3ae8 19e8 1ce8 0fe0  j...jjj.:.......
+00000c90: 13d8 0801 6ae0 0401 6ae8 0801 20e8 5ce8  ....j...j... .\.
+00000ca0: 26e8 29d0 06b0 0c03 2020 20e8 0301 20e0  &.).....   ... .
+00000cb0: 6fc8 6dc0 47b8 09e0 6207 d7c9 0a84 8381  o.m.G...b.......
+00000cc0: 0ce0 04c0 08a0 1001 cbe8 2003 8584 83e0  .......... .....
+00000cd0: 04c0 08c0 1001 0ce0 0407 cbd7 c8c8 c9c9  ................
+00000ce0: c9e8 0303 caca cae8 03d0 06b8 0c03 cbcb  ................
+00000cf0: d7c8 0801 cbe8 03d8 0601 cce0 0402 cccc  ................
+00000d00: e803 e806 03cd cd00 e8f8 e10c 02d7 d7d0  ................
+00000d10: 47d0 4d01 c9e0 f6d8 1703 0000 21e9 0a07  G.M.........!...
+00000d20: 216a 0000 0000 00e1 12e1 16e0 0dc8 177e  !j.............~
+00000d30: 0101 1116 00fa fff7 ff07 0000 0000 586a  ..............Xj
+00000d40: 6ae0 07e0 0bc0 0805 0088 d788 5888 18d8  j...........X...
+00000d50: 1501 d7e0 1801 20a0 3003 d7d7 d7e8 1502  ...... .0.......
+00000d60: d788 9018 02f5 81b0 1801 6ab8 3003 2883  ..........j.0.(.
+00000d70: 0ab8 18e8 5fc8 4803 c7c9 f5b8 1805 5888  ...._.H.......X.
+00000d80: 6a58 20d8 6003 c8c8 c9a0 1801 58d0 1802  jX .`.......X...
+00000d90: d7d7 e817 01c9 b048 e8bc 056a c96a 6a58  .......H...j.jjX
+00000da0: d818 01c8 b860 e810 06c9 cb00 006a 58e0  .....`.......jX.
+00000db0: 46c0 1801 cae0 18e8 16e0 b5d8 18d8 7804  F.............x.
+00000dc0: cad7 8183 c816 a818 04ca d783 84b8 16b8  ................
+00000dd0: 3004 cad7 5888 a816 d8fd e016 0188 e918  0...X...........
+00000de0: a143 e090 e86e 9814 c018 e172 b000 0115  .C...n.....r....
+00000df0: 0800 fdff f6ff 1000 c8c8 c9c9 c9c9 00c7  ................
+00000e00: c9ca cacb caca c9e8 0802 cbcc e809 01c6  ................
+00000e10: d008 01c9 c808 8810 8820 8830 8840 d850  ......... .0.@.P
+00000e20: 03c7 c8c8 e85e 02c9 cae8 6ee0 69e8 0a03  .....^....n.i...
+00000e30: cbd7 d7d8 7205 d7d8 d7d7 12e8 1be0 0804  ....r...........
+00000e40: 10c8 c7c7 e010 05d8 c6d7 d7d7 e803 d006  ................
+00000e50: e00c 3401 010f 1400 f3ff f9ff 0300 0000  ..4.............
+00000e60: e803 d006 e80c 01c6 8810 e812 04c9 caca  ................
+00000e70: c988 1206 caca cbcb caca b03b 01c7 d812  ...........;....
+00000e80: 04cc cccc cbc0 15c0 1202 cdcc e82a a836  .............*.6
+00000e90: e012 e826 0215 1588 1205 ca13 1517 1588  ...&............
+00000ea0: 1208 0d16 0d0c 28c7 c7c8 e86e c036 0b16  ......(....n.6..
+00000eb0: 0d0b 0a21 d710 10d8 c8c8 e870 06cb ca0d  ...!.......p....
+00000ec0: 1416 0ae8 1209 6a00 0010 d7d7 d8c9 c9e8  ......j.........
+00000ed0: 4805 160d 0d0a f5e0 120a 0000 d8d7 d7d7  H...............
+00000ee0: 10c7 150f e036 0120 d812 0200 00e8 1304  .....6. ........
+00000ef0: d7d8 1017 e048 c812 c816 05c6 0c0a 2120  .....H........! 
+00000f00: 910e 04d7 d788 d7a1 2020 0101 0a1c 00f4  ........  ......
+00000f10: fffa ff05 c6c6 c7c7 c7e8 03d8 06c8 0dc8  ................
+00000f20: 1306 00ca cacb cbcb e803 d006 b00c 0cca  ................
+00000f30: cbca d8ca cbcc cdcd cdcc ccd0 0601 cce8  ................
+00000f40: 0ae8 0dd8 1201 cbe8 1ce0 2488 3cd0 3a01  ..........$.<.:.
+00000f50: 88e0 3404 cdcd cbcc e840 e847 d806 d00c  ..4......@.G....
+00000f60: 12cc cc20 0f14 130e 1412 0d13 110c 1210  ... ............
+00000f70: 0c10 10e0 0611 1211 0d13 120f 130f 210f  ..............!.
+00000f80: 1614 0d15 130c 14e8 0304 130c 1312 c809  ................
+00000f90: 0d15 140e 140e 200b 0b0b 0b0a 0a0a e803  ...... .........
+00000fa0: e806 0228 21b8 0be8 1806 8828 21f5 f5f5  ...(!......(!...
+00000fb0: e803 d806 0221 20a8 0c09 2888 d8d7 5858  .....! ...(...XX
+00000fc0: 2020 20e8 03d0 06c0 0c04 58d7 d86a 4801     .......X..jH.
+00000fd0: 0110 1400 faff f9ff 0500 0000 00c9 e005  ................
+00000fe0: e009 c008 0500 caca caca 8816 05ca cbcb  ................
+00000ff0: cbcb 9016 03c9 c9ca 8816 0400 0011 c988  ................
+00001000: 16e8 6103 12f5 1088 1606 0000 2828 1128  ..a.........((.(
+00001010: 8816 0400 5821 21e8 1602 11c8 e058 e06f  ....X!!......X.o
+00001020: 0cca c9c9 00d7 5820 2021 2821 11e0 42e8  ......X  !(!..B.
+00001030: 6fd8 1be8 2a05 6a20 2020 6ae0 42e0 2d02  o...*.j   j.B.-.
+00001040: d8d8 e014 e016 026a 6ae0 4201 13e8 9904  .......jj.B.....
+00001050: 10d8 d8c8 d0d7 0158 d842 0828 28ca c9d8  .......X.B.((...
+00001060: d8d7 d8c0 ebe0 4202 2814 e827 03d7 d7d7  ......B.(..'....
+00001070: b0ff e858 0321 10c6 9813 e921 01d7 e839  ...X.!.....!...9
+00001080: 9012 d816 d936 b000 0115 0800 fdff f6ff  .....6..........
+00001090: 1000 c8c8 c9c9 c9c9 00c7 c9ca cacb caca  ................
+000010a0: c9e8 0802 cbcc e809 01c6 d008 01c9 c808  ................
+000010b0: 8810 8820 8830 8840 d850 03c7 c8c8 e85e  ... .0.@.P.....^
+000010c0: 02c9 cae8 6ee0 69e8 0a03 cbd7 d7d8 7205  ....n.i.......r.
+000010d0: d7d8 d7d7 12e8 1be0 0804 10c8 c7c7 e010  ................
+000010e0: 05d8 c6d7 d7d7 e803 d006 e00c 3401 010f  ............4...
+000010f0: 1400 f1ff faff 0300 0000 e803 d006 e80c  ................
+00001100: 01c6 8810 e812 04c9 caca c988 1206 caca  ................
+00001110: cbcb caca b03b 01c7 d812 04cc cccc cbc0  .....;..........
+00001120: 15c0 1202 cdcc e82a a836 e012 e826 0215  .......*.6...&..
+00001130: 1588 1205 ca13 1517 1588 1208 0d16 0d0c  ................
+00001140: 28c7 c7c8 e86e c036 0b16 0d0b 0a21 d710  (....n.6.....!..
+00001150: 10d8 c8c8 e870 06cb ca0d 1416 0ae8 1209  .....p..........
+00001160: 6a00 0010 d7d7 d8c9 c9e8 4805 160d 0d0a  j.........H.....
+00001170: f5e0 120a 0000 d8d7 d7d7 10c7 150f e036  ...............6
+00001180: 0120 d812 0200 00e8 1304 d7d8 1017 e048  . .............H
+00001190: c812 c816 05c6 0c0a 2120 910e 04d7 d788  ........! ......
+000011a0: d7a1 2020 0101 0a1c 00f0 fffa ff05 c6c6  ..  ............
+000011b0: c7c7 c7e8 03d8 06c8 0dc8 1306 00ca cacb  ................
+000011c0: cbcb e803 d006 b00c 0cca cbca d8ca cbcc  ................
+000011d0: cdcd cdcc ccd0 0601 cce8 0ae8 0dd8 1201  ................
+000011e0: cbe8 1ce0 2488 3cd0 3a01 88e0 3404 cdcd  ....$.<.:...4...
+000011f0: cbcc e840 e847 d806 d00c 12cc cc20 0f14  ...@.G....... ..
+00001200: 130e 1412 0d13 110c 1210 0c10 10e0 0611  ................
+00001210: 1211 0d13 120f 130f 210f 1614 0d15 130c  ........!.......
+00001220: 14e8 0304 130c 1312 c809 0d15 140e 140e  ................
+00001230: 200b 0b0b 0b0a 0a0a e803 e806 0228 21b8   ............(!.
+00001240: 0be8 1806 8828 21f5 f5f5 e803 d806 0221  .....(!........!
+00001250: 20a8 0c09 2888 d8d7 5858 2020 20e8 03d0   ...(...XX   ...
+00001260: 06c0 0c04 58d7 d86a 4801 0110 1400 faff  ....X..jH.......
+00001270: f9ff 0500 0000 00c9 e005 e009 c008 0500  ................
+00001280: caca caca 8816 05ca cbcb cbcb 9016 03c9  ................
+00001290: c9ca 8816 0400 0011 c988 16e8 6103 12f5  ............a...
+000012a0: 1088 1606 0000 2828 1128 8816 0400 5821  ......((.(....X!
+000012b0: 21e8 1602 11c8 e058 e06f 0cca c9c9 00d7  !......X.o......
+000012c0: 5820 2021 2821 11e0 42e8 6fd8 1be8 2a05  X  !(!..B.o...*.
+000012d0: 6a20 2020 6ae0 42e0 2d02 d8d8 e014 e016  j   j.B.-.......
+000012e0: 026a 6ae0 4201 13e8 9904 10d8 d8c8 d0d7  .jj.B...........
+000012f0: 0158 d842 0828 28ca c9d8 d8d7 d8c0 ebe0  .X.B.((.........
+00001300: 4202 2814 e827 03d7 d7d7 b0ff e858 0321  B.(..'.......X.!
+00001310: 10c6 9813 e921 01d7 e839 9012 d816 d936  .....!...9.....6
+00001320: 0900 ff02 00fe 0101 0000 0000 0900 ff02  ................
+00001330: 00fd 0101 0100 0100 0900 ff02 00fc 0101  ................
+00001340: 0200 0200 0b00 ff00 0002 01ff 1400 12fd  ................
+00001350: 2704 0900 ff03 0001 ff14 0000 fe00 0900  '...............
+00001360: ff03 0081 ff1b 0000 fc00 1500 ff00 0006  ................
+00001370: 01ff 1b00 12fd 2704 2801 0015 ff29 0000  ......'.(....)..
+00001380: 15ff 0900 ff03 0001 ff1b 0000 fd00 0000  ................
+00001390: 0000 0000                                ....
```

### Comparing `nml-0.7.2/regression/expected/012_basecost.nfo` & `nml-r1512/regression/expected/012_basecost.nfo`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d20
+0 * 4 \d19 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\12" "NML regression test" 00 "A test newgrf testing NML" 00
-// param[127] = (param[2] + 8)
-3 * 9 0D 7F \D+ 02 FF \dx00000008
-
-4 * 7 06
-7F 01 FF \wx0008
-FF
-
-5 * 9 00 08 \b1 01 FF \wx0001
-08 00
-
-6 * 14 00 08 \b1 06 FF \wx002A
-08 06 06 06 06 06 06
-
-7 * 13 00 08 \b1 05 FF \wx0042
-08 06 06 06 06 06
-
-// param[126] = (param[1] + 9)
-8 * 9 0D 7E \D+ 01 FF \dx00000009
-
-9 * 27 06
-7E 01 FF \wx0008
-7E 01 FF \wx0009
-7E 01 FF \wx000A
-7E 01 FF \wx000B
-7E 01 FF \wx000C
-FF
-
-10 * 13 00 08 \b1 05 FF \wx000F
-08 00 00 00 00 00
-
-11 * 9 00 08 \b1 01 FF \wx0034
-08 15
-
-// param[124] = param[11]
-12 * 5 0D 7C \D= 0B 00
-
-13 * 7 06
-7C 01 FF \wx0003
-FF
-
-// param[125] = param[0]
-14 * 5 0D 7D \D= 00 00
-
-// param[122] = (param[11] + 1)
-15 * 9 0D 7A \D+ 0B FF \dx00000001
-
-16 * 7 06
-7A 01 FF \wx0003
-FF
-
-// param[123] = param[0]
-17 * 5 0D 7B \D= 00 00
-
-// param[124] = (param[123] + 8)
-18 * 9 0D 7C \D+ 7B FF \dx00000008
-
-19 * 12 06
-7D 02 FF \wx0005
-7C 01 FF \wx0008
-FF
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "NML\12" "NML regression test" 00 "A test newgrf testing NML" 00 
+// param[64] = (param[2] + 8)
+3 * 9 0D 40 \D+ 02 FF \dx00000008 
+
+4 * 7 06 
+40 01 FF \wx0006 
+FF 
+
+5 * 7 00 08 \b1 01 01 
+08 00 
+
+6 * 12 00 08 \b1 06 2A 
+08 06 06 06 06 06 06 
+
+// param[65] = (param[1] + 9)
+7 * 9 0D 41 \D+ 01 FF \dx00000009 
+
+8 * 27 06 
+41 01 FF \wx0006 
+41 01 FF \wx0007 
+41 01 FF \wx0008 
+41 01 FF \wx0009 
+41 01 FF \wx000A 
+FF 
+
+9 * 11 00 08 \b1 05 0F 
+08 00 00 00 00 00 
+
+10 * 7 00 08 \b1 01 34 
+08 15 
+
+// param[67] = param[11]
+11 * 5 0D 43 \D= 0B 00 
+
+12 * 7 06 
+43 01 FF \wx0003 
+FF 
+
+// param[66] = param[0]
+13 * 5 0D 42 \D= 00 00 
+
+// param[69] = (param[11] + 1)
+14 * 9 0D 45 \D+ 0B FF \dx00000001 
+
+15 * 7 06 
+45 01 FF \wx0003 
+FF 
+
+// param[68] = param[0]
+16 * 5 0D 44 \D= 00 00 
+
+// param[67] = (param[68] + 8)
+17 * 9 0D 43 \D+ 44 FF \dx00000008 
+
+18 * 12 06 
+42 01 FF \wx0004 
+43 01 FF \wx0006 
+FF 
 
-20 * 9 00 08 \b1 01 FF \wx0000
-08 00
+19 * 7 00 08 \b1 01 00 
+08 00
```

### Comparing `nml-0.7.2/regression/expected/013_train_callback.grf` & `nml-r1512/regression/expected/013_train_callback.grf`

 * *Files 21% similar despite different names*

```diff
@@ -1,486 +1,431 @@
-00000000: 0000 4752 4682 0d0a 1a0a 3c06 0000 0004  ..GRF.....<.....
-00000010: 0000 00ff 4b00 0000 3600 0000 ff14 4349  ....K...6.....CI
-00000020: 4e46 4f42 5652 534e 0400 0000 0000 424d  NFOBVRSN......BM
-00000030: 494e 5604 0000 0000 0042 4e50 4152 0100  INV......BNPAR..
-00000040: 0042 5041 4c53 0100 5742 424c 5452 0100  .BPALS..WBBLTR..
-00000050: 3800 0034 0000 00ff 0808 4e4d 4c13 4e4d  8..4......NML.NM
-00000060: 4c20 7265 6772 6573 7369 6f6e 2074 6573  L regression tes
-00000070: 7400 4120 7465 7374 206e 6577 6772 6620  t.A test newgrf 
-00000080: 7465 7374 696e 6720 4e4d 4c00 d000 0000  testing NML.....
-00000090: ff00 0801 32ff 0000 0957 4450 5253 4352  ....2....WDPRSCR
-000000a0: 5043 4d4e 5457 4f4f 444c 5653 5453 5445  PCMNTWOODLVSTSTE
-000000b0: 4c56 4548 4942 5243 4b57 4f4f 4c42 5542  LVEHIBRCKWOOLBUB
-000000c0: 4c54 4f59 5346 5a44 5246 5255 5446 5256  LTOYSFZDRFRUTFRV
-000000d0: 4746 4f4f 444f 494c 5f47 4f4f 4457 4154  GFOODOIL_GOODWAT
-000000e0: 524d 494c 4b43 4f41 4c49 4f52 4541 4f52  RMILKCOALIOREAOR
-000000f0: 4543 4c41 5947 5256 4c53 414e 4447 5241  ECLAYGRVLSANDGRA
-00000100: 4952 5347 524d 4149 5a43 4f52 4546 4552  IRSGRMAIZCOREFER
-00000110: 5443 5443 4453 554c 5057 4845 4152 4650  TCTCDSULPWHEARFP
-00000120: 5243 4f4c 4150 4554 5250 4150 5254 4f46  RCOLAPETRPAPRTOF
-00000130: 4653 5547 5250 4153 534d 4149 4c42 4154  FSUGRPASSMAILBAT
-00000140: 5453 5745 5452 5542 5246 4d53 5045 4e53  TSWETRUBRFMSPENS
-00000150: 504d 4e53 5046 4943 5250 4c41 5350 4c53  PMNSPFICRPLASPLS
-00000160: 541c 0000 00ff 0008 0105 ff00 0012 5241  T.............RA
-00000170: 494c 454c 524c 4d4f 4e4f 4d47 4c56 5452  ILELRLMONOMGLVTR
-00000180: 5044 0600 0000 ff01 0008 ff04 0004 0000  PD..............
-00000190: 00fd 0700 0000 0400 0000 fd08 0000 0004  ................
-000001a0: 0000 00fd 0900 0000 0400 0000 fd0a 0000  ................
-000001b0: 0004 0000 00fd 0b00 0000 0400 0000 fd0c  ................
-000001c0: 0000 0004 0000 00fd 0d00 0000 0400 0000  ................
-000001d0: fd0e 0000 0004 0000 00fd 0f00 0000 0400  ................
-000001e0: 0000 fd10 0000 0004 0000 00fd 1100 0000  ................
-000001f0: 0400 0000 fd12 0000 0004 0000 00fd 1300  ................
-00000200: 0000 0400 0000 fd14 0000 0004 0000 00fd  ................
-00000210: 1500 0000 0400 0000 fd16 0000 0004 0000  ................
-00000220: 00fd 1700 0000 0400 0000 fd18 0000 0004  ................
-00000230: 0000 00fd 1900 0000 0400 0000 fd1a 0000  ................
-00000240: 0004 0000 00fd 1b00 0000 0400 0000 fd1c  ................
-00000250: 0000 0004 0000 00fd 1d00 0000 0400 0000  ................
-00000260: fd1e 0000 0004 0000 00fd 1f00 0000 0400  ................
-00000270: 0000 fd20 0000 0004 0000 00fd 2100 0000  ... ........!...
-00000280: 0400 0000 fd22 0000 0004 0000 00fd 2300  ....."........#.
-00000290: 0000 0400 0000 fd24 0000 0004 0000 00fd  .......$........
-000002a0: 2500 0000 0400 0000 fd26 0000 000d 0000  %........&......
-000002b0: 00ff 0200 ff02 0200 0001 0000 0001 000d  ................
-000002c0: 0000 00ff 0200 fe02 0202 0003 0002 0003  ................
-000002d0: 000d 0000 00ff 0200 fd02 0204 0005 0004  ................
-000002e0: 0005 000d 0000 00ff 0200 fc02 0206 0007  ................
-000002f0: 0006 0007 000f 0000 00ff 0200 fd80 0200  ................
-00000300: 04ff 00ff 00ff 00fd 0009 0000 00ff 0d7f  ................
-00000310: 0783 ffff 0000 0007 0000 00ff 067f 04ff  ................
-00000320: 0600 ff17 0000 00ff 0200 fd89 1a00 0000  ................
-00000330: 0000 01fe 0001 0000 0001 0000 00fd 0017  ................
-00000340: 0000 00ff 0200 fc89 4700 ff00 0000 01fd  ........G.......
-00000350: 0013 0000 0013 0000 00fc 0009 0000 00ff  ................
-00000360: 0200 fd01 0100 0000 0017 0000 00ff 0200  ................
-00000370: fd89 0c00 ffff 0000 0100 8000 0000 0000  ................
-00000380: 0000 00fd 0053 0000 00ff 0200 fe89 4700  .....S........G.
-00000390: ff00 0000 0719 802f 0000 002f 0000 0014  ......./.../....
-000003a0: 800c 0000 000c 0000 0014 800d 0000 000d  ................
-000003b0: 0000 0019 8019 0000 0019 0000 0019 801b  ................
-000003c0: 0000 001b 0000 0014 801a 0000 001a 0000  ................
-000003d0: 0019 8020 0000 0020 0000 00fd 0035 0000  ... ... .....5..
-000003e0: 00ff 0200 fd89 4700 ff00 0000 0412 8013  ......G.........
-000003f0: 0000 0013 0000 0012 800c 0000 000c 0000  ................
-00000400: 0012 800d 0000 000d 0000 0012 801a 0000  ................
-00000410: 001a 0000 00fd 0009 0000 00ff 0d7d 0401  .............}..
-00000420: ff88 1300 0009 0000 00ff 0d7e 017d ffba  ...........~.}..
-00000430: 0200 0009 0000 00ff 0d7f 0a7e ff75 0500  ...........~.u..
-00000440: 0009 0000 00ff 0d7c 0402 ffd4 3000 0009  .......|....0...
-00000450: 0000 00ff 0d7d 017c ff8e 1800 0009 0000  .....}.|........
-00000460: 00ff 0d7e 0a7d ff1d 3100 0009 0000 00ff  ...~.}..1.......
-00000470: 0d7b 0403 ff08 0000 0009 0000 00ff 0d7c  .{.............|
-00000480: 017b ff02 0000 0009 0000 00ff 0d7d 0a7c  .{...........}.|
-00000490: ff05 0000 0009 0000 00ff 0d7a 0404 ff95  ...........z....
-000004a0: 0b00 0009 0000 00ff 0d7b 017a ff51 0400  .........{.z.Q..
-000004b0: 0009 0000 00ff 0d7c 0a7b ffa3 0800 0016  .......|.{......
-000004c0: 0000 00ff 067f 02ff 0b00 7e02 ff0e 007d  ..........~....}
-000004d0: 02ff 1100 7c02 ff14 00ff 1600 0000 ff00  ....|...........
-000004e0: 0005 01ff 7400 0924 0009 0000 0900 0009  ....t..$........
-000004f0: 0000 0b00 0009 0000 00ff 0d7f 0701 ffff  ................
-00000500: 0000 0009 0000 00ff 0d7e 0601 fff8 ffff  .........~......
-00000510: ff0c 0000 00ff 067f 01ff 4d00 7e01 ff4f  ..........M.~..O
-00000520: 00ff 5200 0000 ff00 001a 01ff 7400 060f  ..R.........t...
-00000530: 2810 001d 0000 0000 29cb 011d 0000 0000  (.......).......
-00000540: 2c04 0001 0c0d 1d00 0000 0015 1312 fd2a  ,..............*
-00000550: 407a 0a00 04ff 2600 031e 0200 070a 17b6  @z....&.........
-00000560: 0d05 0900 001c 2805 000b 0000 0e30 4c00  ......(......0L.
-00000570: 0014 1e16 0024 0025 001b 0000 00ff 0400  .....$.%........
-00000580: 7f01 ff74 004e 4d4c 2054 6573 7420 6275  ...t.NML Test bu
-00000590: 6c6b 2077 6167 6f6e 0009 0000 00ff 0000  lk wagon........
-000005a0: 0101 ff74 001e 0821 0000 00ff 0200 fd89  ...t...!........
-000005b0: 1000 ff00 0000 02fe 0014 0000 0014 0000  ................
-000005c0: 00fd 0016 0000 0016 0000 00fc 0021 0000  .............!..
-000005d0: 00ff 0200 ff89 1000 ff00 0000 021e 8014  ................
-000005e0: 0000 0014 0000 0019 8016 0000 0016 0000  ................
-000005f0: 00fc 0021 0000 00ff 0200 fd89 0c00 ffff  ...!............
-00000600: 0000 02fe 0015 0000 0015 0000 00fd 0036  ...............6
-00000610: 0000 0036 0000 00fc 0017 0000 00ff 0200  ...6............
-00000620: fc89 0c00 ffff 0000 01ff 0036 0000 0036  ...........6...6
-00000630: 0000 00fc 000c 0000 00ff 0300 01ff 7400  ..............t.
-00000640: 01ff fc00 fd00 0000 0000 0700 0000 7300  ..............s.
-00000650: 0000 0400 1500 0800 fdff f7ff 0615 1515  ................
-00000660: 1514 14e8 0606 1313 1313 1312 c008 0114  ................
-00000670: d810 0712 1214 1410 1010 e803 0b14 1411  ................
-00000680: 1110 10d7 d714 1412 d809 0315 1412 d809  ................
-00000690: e008 e012 0116 8810 8810 8820 e830 d876  ........... .0.v
-000006a0: 0616 1616 1112 12e8 7a04 1415 1011 e008  ........z.......
-000006b0: 0213 14c0 0802 106a e011 066a 1400 8888  .......j...j....
-000006c0: 88e8 0301 0008 0000 00c5 0000 0004 000f  ................
-000006d0: 0016 00f2 fff9 ff03 0000 00e8 03d0 0606  ................
-000006e0: 0000 1415 1516 9012 e814 0514 1212 1111  ................
-000006f0: 9018 e014 e815 0310 10d7 b030 d814 0112  ...........0....
-00000700: d014 0215 15c0 50d8 1401 11e0 2802 cb10  ......P.....(...
-00000710: d05c d014 e029 0514 15ca cbcb e806 b814  .\...)..........
-00000720: e83e 0a14 1514 14c9 cacb 1113 14c0 1402  .>..............
-00000730: 1211 e814 0210 13e8 1605 ca11 6a21 11e8  ............j!..
-00000740: 0ee0 680f 1415 cb10 1310 1313 c8c9 6a21  ..h...........j!
-00000750: 0000 10e0 12e8 32e0 5005 1311 1313 d7d8  ......2.P.......
-00000760: d702 1011 d067 d850 0111 d014 0300 006a  .....g.P.......j
-00000770: e816 e069 e050 c014 0400 00d7 d7d8 2de8  ...i.P........-.
-00000780: 50b0 14d0 1804 6a12 1113 e064 912a e818  P.....j....d.*..
-00000790: 8814 0900 0000 dc00 0000 0400 0b00 2000  .............. .
-000007a0: f0ff f9ff 0600 1515 1414 14e8 03d0 06a8  ................
-000007b0: 0c0b 1515 1516 1600 0015 1212 12e8 03d0  ................
-000007c0: 06b8 0c03 1111 11e8 0301 10a0 20d0 13d0  ............ ...
-000007d0: 19d8 1d02 1010 c820 a812 d816 e01a e01e  ....... ........
-000007e0: 02d7 d7e0 60e8 6888 82c8 7ed0 800d 1111  ....`.h...~.....
-000007f0: 1214 c9ca cbcb cb10 1313 13e8 03e8 06c8  ................
-00000800: 10e0 a306 00d8 1011 1113 d820 0111 e8a9  ........... ....
-00000810: 0113 e004 0113 c810 0113 e8c4 02d8 00e8  ................
-00000820: 7406 13c8 c9ca caca e0b3 e0b8 e821 d010  t............!..
-00000830: e849 0114 e840 0910 1012 c8c8 c9c9 c912  .I...@..........
-00000840: c89f e8f0 d010 e06a 0cd8 00d7 5858 8888  .......j....XX..
-00000850: 5858 d7d7 d7e8 03d8 0603 8888 88e0 12e0  XX..............
-00000860: 160a 5800 0000 6a21 d7d7 6a21 e809 e80c  ..X...j!..j!....
-00000870: d006 e00c c016 0a00 0000 be00 0000 0400  ................
-00000880: 0f00 1600 faff f9ff 0800 0000 0014 1414  ................
-00000890: 15e0 08e0 0cc0 0806 1415 1211 1111 9018  ................
-000008a0: e814 0112 e016 9018 0111 e83e d815 9830  ...........>...0
-000008b0: 0611 14ca cb14 1488 1807 0010 13c9 cacb  ................
-000008c0: 10b0 1802 1516 b016 0112 e887 e873 0210  .............s..
-000008d0: 10e8 03e0 1809 6a58 c8c9 cb11 1214 cae8  ......jX........
-000008e0: 9f03 1010 10e8 0302 d7d7 d018 05ca 1112  ................
-000008f0: 13c9 d860 e813 e814 0214 14d8 be04 d711  ...`............
-00000900: 13c9 d060 0115 e814 0113 c816 e818 01c8  ...`............
-00000910: d060 0313 1313 e803 c016 e018 e060 d017  .`...........`..
-00000920: 016a a900 01d7 e860 d82d 0288 88a1 1602  .j.....`.-......
-00000930: 6a58 e82c 016a 9014 d018 d028 0b00 0000  jX.,.j.....(....
-00000940: 7000 0000 0400 1500 0800 fdff f7ff 0615  p...............
-00000950: 1515 1514 14e8 060f 13d7 8858 d712 1515  ...........X....
-00000960: d7d7 d788 88d7 14e0 0805 d758 8814 14d8  ...........X....
-00000970: 10d0 0801 58c8 08e8 1001 15c8 10d8 08c0  ....X...........
-00000980: 10c8 18e8 4802 8816 8828 a010 d820 d876  ....H....(... .v
-00000990: 0d16 1616 1112 1213 1313 1415 1011 e008  ................
-000009a0: 0213 14c0 0802 106a e011 036a 1400 e87d  .......j...j...}
-000009b0: e880 0100 0c00 0000 cf00 0000 0400 0f00  ................
-000009c0: 1600 f2ff f9ff 0300 0000 e803 d006 0600  ................
-000009d0: 0014 1515 1690 12e8 1405 1412 1211 1190  ................
-000009e0: 18e0 1406 d788 58d7 10d7 b030 0214 15d8  ......X....0....
-000009f0: 1407 88d7 5815 1615 1590 1401 88e8 2802  ....X.........(.
-00000a00: cb10 d05c b814 0888 1415 cacb cb10 14e8  ...\............
-00000a10: 2cb8 3ce8 1408 1414 c9ca cb11 1314 d850  ,.<............P
-00000a20: e065 01d7 e814 0210 13e8 1609 ca11 6a21  .e............j!
-00000a30: 1111 1415 d7e8 1713 1415 cb10 1310 1313  ................
-00000a40: c8c9 6a21 0000 1012 1212 14e8 32e0 5005  ..j!........2.P.
-00000a50: 1311 1313 d7d8 d702 1011 e8ba 0210 10d0  ................
-00000a60: 5001 11d0 1403 0000 6ae8 16e8 17d8 50c0  P.......j.....P.
-00000a70: 1404 0000 d7d7 d82d e850 b014 d018 046a  .......-.P.....j
-00000a80: 1211 13e0 6491 2ae8 1888 140d 0000 00ee  ....d.*.........
-00000a90: 0000 0004 000b 0020 00f0 fff9 ff06 0015  ....... ........
-00000aa0: 1514 1414 e803 d006 a80c 1415 1515 1616  ................
-00000ab0: 0000 1512 12d7 d7d7 d7d7 8858 8888 88e8  ...........X....
-00000ac0: 03e0 08e8 0b06 5858 5858 1110 e020 02d7  ......XXXX... ..
-00000ad0: 88e8 1de8 04e0 24e0 28e8 10e8 2c01 58d8  ......$.(...,.X.
-00000ae0: 22d8 2001 10d8 1fd0 22c8 25d8 2603 5888  ". .....".%.&.X.
-00000af0: d7e0 60e8 6888 82c0 7fe8 810f 0000 1111  ..`.h...........
-00000b00: 1214 c9ca cbcb cb10 1313 13e8 03e8 06c8  ................
-00000b10: 10e0 a306 00d8 1011 1113 d820 0511 1212  ........... ....
-00000b20: 1213 e004 0113 c810 0113 e8c4 0dd8 0010  ................
-00000b30: 1011 13c8 c9ca caca 1111 e84b e004 0113  ...........K....
-00000b40: c810 e849 0114 e840 0910 1012 c8c8 c9c9  ...I...@........
-00000b50: c912 e80a 0111 e00e 0112 c810 e06a 04d8  .............j..
-00000b60: 00d7 58d8 eec0 bee1 0ad9 06d1 0409 0000  ..X.............
-00000b70: 006a 21d7 d76a 21e8 09e8 0cd0 06e0 0cc0  .j!..j!.........
-00000b80: 160e 0000 00c3 0000 0004 000f 0016 00fa  ................
-00000b90: fff9 ff08 0000 0000 1414 1415 e008 e00c  ................
-00000ba0: c008 0614 1512 1111 1190 18e8 1405 12d7  ................
-00000bb0: d788 8890 1801 11e8 3e04 d7d7 d758 9018  ........>....X..
-00000bc0: 0711 14ca cb14 1488 8818 0610 13c9 cacb  ................
-00000bd0: 10b0 1802 1516 b016 0112 e887 0888 88d7  ................
-00000be0: 5858 8810 10e0 1809 6a58 c8c9 cb11 1214  XX......jX......
-00000bf0: cad8 1801 88e8 1802 d7d7 d018 05ca 1112  ................
-00000c00: 13c9 d060 e818 0415 1614 14d8 be04 d711  ...`............
-00000c10: 13c9 d060 0115 e814 0113 c816 e818 01c8  ...`............
-00000c20: d060 0313 1313 e803 c016 e018 e060 d017  .`...........`..
-00000c30: 016a a900 01d7 e860 d82d 0288 88a1 1602  .j.....`.-......
-00000c40: 6a58 e82c 016a 9014 d018 d028 0f00 0000  jX.,.j.....(....
-00000c50: 8f00 0000 0400 1500 0800 fdff f7ff 0f6e  ...............n
-00000c60: 6e6e 6e6d 6e6f 6f6e 6c6c 6c6c 6c6b d808  nnnmnoonlllllk..
-00000c70: 046b 6c6b 6ee8 10e8 0706 6b6d 6d6b 6b6b  .klkn.....kmmkkk
-00000c80: e803 086d 6d35 3535 3569 69e8 1002 356b  ...mm5555ii...5k
-00000c90: e809 016e e818 e809 d808 e80a 0335 6f6e  ...n.........5on
-00000ca0: d810 0235 6fc0 1088 1801 6fe8 66e0 670c  ...5o.....o.f.g.
-00000cb0: 6f69 356b 6b6c 6c6d 6e69 6935 e00a 036d  oi5kkllmnii5...m
-00000cc0: c869 d80a 0bcb c8c9 c9ca caca cacb c8c8  .i..............
-00000cd0: d00a 03d7 d7d7 e803 06d7 d700 8888 88e8  ................
-00000ce0: 0301 0010 0000 00c5 0000 0004 0010 0016  ................
-00000cf0: 00f2 fff8 ff03 0000 00e8 03d0 0606 0000  ................
-00000d00: 6d6e 6e6f 9012 e014 046c 6c6b 3590 1802  mnno.....llk5...
-00000d10: 6d6d e814 056b 3535 6969 b030 d014 016c  mm...k55ii.0...l
-00000d20: e815 046e 6f35 6eb0 3c01 6ce0 14e8 4003  ...no5n.<.l...@.
-00000d30: 356d 35a0 14e8 2904 6d6e 356c d016 d828  5m5...).mn5l...(
-00000d40: e02b 016b d814 e816 02c9 cbc8 1402 6b6c  .+.k..........kl
-00000d50: b014 04ca cac9 69e8 36e0 2cc8 2801 6ce0  ......i.6.,.(.l.
-00000d60: 1408 6a21 0069 356b 6d6d c014 01ca d014  ..j!.i5kmm......
-00000d70: 0600 0069 6935 35e8 40d0 1403 c9c9 c7d8  ...ii55.@.......
-00000d80: ed03 88d7 d7d0 1703 6cc9 c9c0 1404 0000  ........l.......
-00000d90: 5888 e818 e82e e013 c014 0400 00d7 d7e0  X...............
-00000da0: 1890 14c0 1802 c9c7 d864 8818 8814 0100  .........d......
-00000db0: 1100 0000 e400 0000 0400 0b00 2000 f0ff  ............ ...
-00000dc0: f9ff 0600 6e6e 6d6d 6de8 03d0 06a8 0c0e  ....nnmmm.......
-00000dd0: 6e6e 6e6f 6f00 006e 6c6c 6d6c 6c6c e803  nnnoo..nllmlll..
-00000de0: d806 016b e803 e007 066b 6b6b 6b35 35e0  ...k.....kkkk55.
-00000df0: 20a8 1e01 6be8 18d8 1b01 35e8 1c04 3535   ...k.....5...55
-00000e00: 3569 d040 b81c d836 e038 d81d 0269 69d8  5i.@...6.8...ii.
-00000e10: 20e8 6888 82c8 7ed0 8005 6935 6b6b 69e8   .h...~...i5kki.
-00000e20: 5704 696c 6c35 e004 c008 0269 6de0 1004  W.ill5.....im...
-00000e30: 0000 d769 e868 e06c e890 0269 6ce8 0401  ...i.h.l...il...
-00000e40: 6bc0 2008 6d35 69d7 0088 d7d7 e069 0169  k. .m5i......i.i
-00000e50: b024 e8a5 c024 07d7 d788 88c8 c8c8 e803  .$...$..........
-00000e60: d006 03c9 c9c9 e803 d006 10c9 c9ca caca  ................
-00000e70: cb88 00d7 5858 8888 5858 d790 1ce8 12e0  ....XX..XX......
-00000e80: 160a 5800 0000 6a21 d7d7 6a21 e889 0258  ..X...j!..j!...X
-00000e90: 88e8 0ee8 1104 0088 58d7 b816 1200 0000  ........X.......
-00000ea0: c800 0000 0400 1000 1600 faff f8ff 0800  ................
-00000eb0: 0000 006d 6d6d 6ee0 08e0 0cc0 0806 6d6e  ...mmmn.......mn
-00000ec0: 6c6b 6b6b 9018 e814 016c e016 9018 0469  lkkk.....l.....i
-00000ed0: 356d 6ed8 1590 3005 3535 696d 6d88 18e0  5mn...0.55imm...
-00000ee0: 2d02 696b d818 0135 d848 026e 6fe0 8003  -.ik...5.H.no...
-00000ef0: c8c8 35e8 18d0 30e8 1803 356b 35e0 1807  ..5...0...5k5...
-00000f00: c7c8 c8c8 6b69 6bc8 48e8 15e8 5204 6e6f  ....kik.H...R.no
-00000f10: 6a58 c018 d848 d814 046d 6d00 00d8 1801  jX...H...mm.....
-00000f20: c9e8 3005 696c 696d 6ee8 1402 6c6c d0d3  ..0.ilimn...ll..
-00000f30: 01c7 c818 016c e81a e8bf c816 d818 01c9  .....l..........
-00000f40: e830 016c e016 03d7 d788 b900 e017 02c9  .0.l............
-00000f50: 6bd8 1402 8858 a916 d818 e014 02d7 d7a1  k....X..........
-00000f60: 2c04 6a58 c8c9 8814 c818 d028 1300 0000  ,.jX.......(....
-00000f70: 7c00 0000 0400 1500 0800 fdff f7ff 0f6e  |..............n
-00000f80: 6ed7 8858 d76f 6f6e d7d7 d788 88d7 d808  n..X.oon........
-00000f90: 03d7 5888 e817 e010 0388 6d6d d80f d008  ..X.......mm....
-00000fa0: a810 016e c810 e008 e840 0188 c840 0288  ...n.....@...@..
-00000fb0: 6fc8 30d8 08e0 10e8 58d0 2012 6e6d 6d6e  o.0.....X. .nmmn
-00000fc0: 6f6f 6f69 356b 6b6c 6c6d 6e69 6935 e00a  oooi5kkllmnii5..
-00000fd0: 036d c869 d80a 0bcb c8c9 c9ca caca cacb  .m.i............
-00000fe0: c8c8 d00a e087 e08b 0100 e885 e888 0100  ................
-00000ff0: 1400 0000 c500 0000 0400 1000 1600 f2ff  ................
-00001000: f8ff 0300 0000 e803 d006 0600 006d 6e6e  .............mnn
-00001010: 6f90 12e0 1404 6cd7 8888 9018 0a6d 6d6c  o.....l......mml
-00001020: 88d7 8858 d710 d7b0 30c8 1407 88d7 586e  ...X....0.....Xn
-00001030: 6f35 6eb8 3cd8 1401 88e8 2803 356d 3590  o5n.<.....(.5m5.
-00001040: 1405 886d 6e35 6cd0 16c0 2801 d7d0 14e8  ...mn5l...(.....
-00001050: 1602 c9cb d83c e065 01d7 b814 08ca cbc9  .....<.e........
-00001060: 6935 6d6e d7e8 17c8 2801 6ce0 1408 6a21  i5mn....(.l...j!
-00001070: 0069 356b 6d6d c014 03ca caca e014 0900  .i5kmm..........
-00001080: 0069 6935 356b 6c6b d014 03c9 c9c7 d8ed  .ii55klk........
-00001090: e855 d017 036c c9c9 c014 0200 00e0 a401  .U...l..........
-000010a0: d7e8 2ee0 13c0 1404 0000 d7d7 e0bc 9014  ................
-000010b0: c018 02c9 c7d8 6488 1888 1401 0015 0000  ......d.........
-000010c0: 00ee 0000 0004 000b 0020 00f0 fff9 ff06  ......... ......
-000010d0: 006e 6e6d 6d6d e803 d006 a80c 146e 6e6e  .nnmmm.......nnn
-000010e0: 6f6f 0000 6e6c 6cd7 d7d7 d7d7 8858 8888  oo..nll......X..
-000010f0: 88e8 03e0 08e8 0b06 5858 5858 3535 e020  ........XXXX55. 
-00001100: 02d7 88e8 1de8 04e0 24e0 28e8 10e8 2c01  ........$.(...,.
-00001110: 58d8 22d8 2001 10d8 1fd0 22c8 25d8 2603  X.". .....".%.&.
-00001120: 5888 d7e0 60e8 6888 82c8 7ed0 800c 6935  X...`.h...~...i5
-00001130: 6b6b 696b 6b6c 696c 6c35 e004 c008 0269  kkikklill5.....i
-00001140: 6de0 1006 0000 d769 3535 e803 0135 e824  m......i55...5.$
-00001150: e820 e804 016b c020 056d 3569 d700 e89d  . ...k. .m5i....
-00001160: 0569 6969 6969 b024 026b 6ce8 50d0 4ce0  .iiiii.$.kl.P.L.
-00001170: b903 c8c8 c8e8 03d0 0603 c9c9 c9e8 0302  ................
-00001180: c9ca e803 0acb caca caca cbcb 8800 58d8  ..............X.
-00001190: edb8 1cd8 1fe0 1ed0 180e 0000 6a21 d7d7  ............j!..
-000011a0: 6a21 0000 00d8 5888 e806 e809 0400 8858  j!....X........X
-000011b0: d8b8 1816 0000 00cf 0000 0004 0010 0016  ................
-000011c0: 00fa fff8 ff08 0000 0000 6d6d 6d6e e008  ..........mmmn..
-000011d0: e00c c008 066d 6ed7 d7d7 6b90 1806 6d6e  .....mn...k...mn
-000011e0: 8888 d7d7 e804 9818 0269 35d8 2c01 5888  .........i5.,.X.
-000011f0: 1805 3535 696d 6de8 2f90 1804 6935 696b  ..55imm./...i5ik
-00001200: a818 026e 6fe0 8003 c8c8 35e8 18d8 3007  ...no.....5...0.
-00001210: 88d7 5858 88d7 35e0 1807 c7c8 c8c8 6b69  ..XX..5.......ki
-00001220: 6bd0 480b 8888 5858 d7d7 696e 6f6a 58c0  k.H...XX..inojX.
-00001230: 18d8 48e8 1806 6e6f 6d6d 0000 d818 01c9  ..H...nomm......
-00001240: e830 0569 6c69 6d6e e814 026c 6cd0 d301  .0.ilimn...ll...
-00001250: c7c8 1801 6ce8 1a02 6c6c c016 d818 01c9  ....l...ll......
-00001260: e830 016c e016 e8d5 b900 e017 02c9 6bd8  .0.l..........k.
-00001270: 1402 8858 a916 d818 e014 02d7 d7a1 2c04  ...X..........,.
-00001280: 6a58 c8c9 8814 c818 d028 1700 0000 6600  jX.......(....f.
-00001290: 0000 0400 1700 0800 fdff f5ff 0fc9 c9ca  ................
-000012a0: cacb cbcc ccc9 5858 5858 5888 c008 d010  ......XXXXX.....
-000012b0: 0188 e810 0388 8888 e803 08cc c9d8 d8d8  ................
-000012c0: d8d7 d7d8 10e8 09d0 18c0 0802 d8d8 c008  ................
-000012d0: 9810 8828 9028 d077 03cc c7c8 e881 e882  ...(.(.w........
-000012e0: d807 e88b c008 c010 d020 e808 016a e029  ......... ...j.)
-000012f0: 036a cb00 d088 0100 1800 0000 b800 0000  .j..............
-00001300: 0400 1000 1600 f2ff f8ff 0300 0000 e803  ................
-00001310: d006 0600 00ca cbcc cc90 12e0 1404 8888  ................
-00001320: d8d8 9018 e014 e815 03d8 d7d7 b030 d814  .............0..
-00001330: e82b e014 02c9 c9d0 5802 c9ca d014 03d8  .+......X.......
-00001340: d8cb e814 02ca c7b0 14e8 3dc8 1402 cbc8  ..........=.....
-00001350: e028 0558 5858 d858 e868 c014 02cb c8e8  .(.XXX.X.h......
-00001360: 1401 88d0 15b0 1404 ccc8 c8c7 e054 04d8  .............T..
-00001370: 88cb cbb0 1405 6a21 c8c8 c8e8 3001 ca98  ......j!....0...
-00001380: 1402 0000 e814 03c8 c7c7 b03c d87f 0400  ...........<....
-00001390: c7c8 c9e8 1790 1403 0000 6ae8 4101 c9e8  ..........j.A...
-000013a0: 76a0 1404 0000 d7d7 e044 9014 d018 016a  v........D.....j
-000013b0: c864 9140 e818 8814 1900 0000 dc00 0000  .d.@............
-000013c0: 0400 0c00 2000 f0ff f8ff 0400 caca cae8  .... ...........
-000013d0: 03d0 06a0 0cd0 1809 0000 ca88 8888 8888  ................
-000013e0: 58d8 06d8 0bb0 0a03 d7d8 cbd0 2002 5858  X........... .XX
-000013f0: e803 8825 e01f 02d7 cce8 40e0 1d88 4308  ...%......@...C.
-00001400: d8d8 d8d8 d8d7 d7d7 d820 04cb cccc cce8  ......... ......
-00001410: 03d0 06a0 0ce0 1806 0000 c8c9 cbc9 e803  ................
-00001420: 03c9 cbca e803 d006 03c9 cbcb e803 e818  ................
-00001430: 01cb e020 03c7 cbca e803 d006 a00c 03c7  ... ............
-00001440: cbc7 e820 01d7 e820 01c9 8823 b820 08ca  ... ... ...#. ..
-00001450: ccd7 00c8 c8cc c9e8 0303 c8cc cae8 03d0  ................
-00001460: 06c0 0c02 c8ca e840 01c7 e808 c023 8829  .......@.....#.)
-00001470: e89b 0bd7 00c7 c7c7 c7c7 c8c8 c9c9 e803  ................
-00001480: 01c9 e803 d006 c80c e920 0700 6a21 d7d7  ......... ..j!..
-00001490: 6a21 e809 e80c d006 e00c c016 1a00 0000  j!..............
-000014a0: 9c00 0000 0400 1000 1600 faff f8ff 0800  ................
-000014b0: 0000 00c9 caca cbe0 08e0 0cc0 0807 c9ca  ................
-000014c0: 88d8 d8d8 cb98 18e8 1401 88e0 16e8 1801  ................
-000014d0: ccb0 3004 cac9 c9ca d815 9818 02ca c788  ..0.............
-000014e0: 18c0 1698 1801 ccd8 4801 c9e0 16a0 3001  ........H.....0.
-000014f0: d7e0 1802 c9c8 9018 03d7 d7d7 e818 026a  ...............j
-00001500: 58b0 1802 cacb e015 03cc ccc9 e8be 9018  X...............
-00001510: e014 c8bc 01c7 a848 02cb cbb0 eab0 1802  .......H........
-00001520: caca a100 c030 e017 016a a916 d048 e82d  .....0...j...H.-
-00001530: 0288 88a1 2ce0 9002 ca6a 9014 d018 d028  ....,....j.....(
-00001540: 1b00 0000 7400 0000 0400 1700 0800 fdff  ....t...........
-00001550: f5ff 27c9 c9ca cacb cbcc ccc9 d888 5858  ..'...........XX
-00001560: 88d8 ccc9 8846 494a 4888 ccc9 4647 4749  .....FIJH...FGGI
-00001570: 4948 ccc9 4746 4848 4a49 c810 d008 0148  IH..GFHHJI.....H
-00001580: c808 e829 8828 9028 014a e030 0447 4649  ...).(.(.J.0.GFI
-00001590: 49a0 40d8 37e8 50d0 7703 ccc7 c8e8 81e8  I.@.7.P.w.......
-000015a0: 82d8 07e8 8bc0 08c0 10d0 20e8 0801 6ae0  .......... ...j.
-000015b0: 290a 6acb 00d8 d8d8 d8d7 d700 1c00 0000  ).j.............
-000015c0: b400 0000 0400 1000 1600 f2ff f8ff 0300  ................
-000015d0: 0000 e803 d006 0600 00ca cbcc cc90 12e0  ................
-000015e0: 1404 5888 d8d8 9018 e014 0648 494a 48d7  ..X........HIJH.
-000015f0: d7b0 3002 c9ca d814 0749 484a cccc c9c9  ..0......IHJ....
-00001600: 9014 0349 48cb e814 02ca c798 2801 49d0  ...IH.......(.I.
-00001610: 1402 cbc8 8814 d814 07cb c8c9 ca88 8846  ...............F
-00001620: e065 c83c e014 08cc c8c8 c7c9 ca47 47e8  .e.<.........GG.
-00001630: 3c01 cbb0 1405 6a21 c8c8 c8e8 3001 ca98  <.....j!....0...
-00001640: 1402 0000 e814 03c8 c7c7 b03c d87f 0400  ...........<....
-00001650: c7c8 c9e8 1790 1403 0000 6ae8 4101 c9e8  ..........j.A...
-00001660: 76a0 1404 0000 d7d7 e044 9014 d018 016a  v........D.....j
-00001670: c864 9140 e818 8814 1d00 0000 ee00 0000  .d.@............
-00001680: 0400 0c00 2000 f0ff f8ff 0400 caca cae8  .... ...........
-00001690: 03d0 06a0 0cd0 180f 0000 ca88 8846 4747  .............FGG
-000016a0: 4848 494a 4949 49e0 05e8 08e0 0606 4a4a  HHIJIII.......JJ
-000016b0: 4a88 d8cb e820 0146 e01f e821 e024 e827  J.... .F...!.$.'
-000016c0: e006 e82c 014a d822 01cc e020 e03e e042  ...,.J."... .>.B
-000016d0: b822 d82a 0549 484a 4948 e020 04cb cccc  .".*.IHJIH. ....
-000016e0: cce8 03d0 06a0 0ce0 1806 0000 c8c9 cbc9  ................
-000016f0: e803 03c9 cbca e803 d006 03c9 cbcb e803  ................
-00001700: e818 01cb e020 03c7 cbca e803 d006 a00c  ..... ..........
-00001710: 03c7 cbc7 e820 01d7 e820 01c9 8823 b820  ..... ... ...#. 
-00001720: 08ca ccd7 00c8 c8cc c9e8 0303 c8cc cae8  ................
-00001730: 03d0 06c0 0c02 c8ca e840 01c7 e808 c023  .........@.....#
-00001740: 8829 e89b 0bd7 00c7 c7c7 c7c7 c8c8 c9c9  .)..............
-00001750: e803 01c9 e803 d006 c80c e920 0700 6a21  ........... ..j!
-00001760: d7d7 6a21 e809 e80c d006 e00c c016 1e00  ..j!............
-00001770: 0000 b000 0000 0400 1000 1600 faff f8ff  ................
-00001780: 0800 0000 00c9 caca cbe0 08e0 0cc0 0807  ................
-00001790: c9ca 88d8 d8d8 cb98 18e8 1405 8846 4749  .............FGI
-000017a0: 4990 1808 cac9 c9ca 4748 484a d818 01cc  I.......GHHJ....
-000017b0: b816 01c7 e018 0149 8818 e816 d018 0149  .......I.......I
-000017c0: d030 01cc d830 01c9 e016 b818 044a 49d8  .0...0.......JI.
-000017d0: d7e0 1802 c9c8 c018 01ca e830 0149 e818  ...........0.I..
-000017e0: 01d7 e818 026a 58a8 1801 cbe0 1803 cccc  .....jX.........
-000017f0: c9e8 be90 18e0 14c8 bc01 c7b0 48e8 14b0  ............H...
-00001800: eab0 1802 caca a100 c030 e017 016a b116  .........0...j..
-00001810: 016a d048 e82d 0288 88a1 2ce0 9002 ca6a  .j.H.-....,....j
-00001820: 9014 d018 d028 1f00 0000 8000 0000 0400  .....(..........
-00001830: 1600 0800 fdff f6ff 0f15 1515 1514 1516  ................
-00001840: 1615 1313 1313 1312 c008 0115 d810 0312  ................
-00001850: 1214 c008 0414 1212 12e8 0308 1414 1111  ................
-00001860: 1110 1010 e010 e009 0115 e018 e812 c008  ................
-00001870: 0216 15e0 28e8 0888 2088 20e8 2802 1514  ....(... . .(...
-00001880: e077 0416 1112 12e8 7a03 1415 10e8 58e8  .w......z.....X.
-00001890: 0a01 14e8 5ce8 0b05 1212 8888 88e8 0304  ....\...........
-000018a0: 8888 106a e012 036a 1100 d011 0100 2000  ...j...j...... .
-000018b0: 0000 c800 0000 0400 1000 1600 f2ff f8ff  ................
-000018c0: 0300 0000 e803 d006 0600 0014 1515 1690  ................
-000018d0: 12e8 1405 1412 1212 1190 180a 1414 1313  ................
-000018e0: 1211 1110 1010 b030 e014 e815 d814 0215  .......0........
-000018f0: 15c0 50e0 14e0 15e0 14d0 15d8 14e0 3e03  ..P...........>.
-00001900: 1114 15e0 3301 cbb8 14e0 53d0 1404 caca  ....3.....S.....
-00001910: 1514 c814 e83f e046 0415 14ca cae8 4e02  .....?.F......N.
-00001920: 1210 e836 c014 0114 c814 076a 2100 1011  ...6.......j!...
-00001930: 1214 d832 e014 e857 e014 0300 0010 e817  ...2...W........
-00001940: 0112 e83c e050 e887 0188 d8ed e82b d817  ...<.P.......+..
-00001950: d814 0110 d014 0500 006a 1012 e0d2 01c9  .........j......
-00001960: e8d8 b814 0400 00d7 d7e8 43e0 d7a8 14d0  ..........C.....
-00001970: 1804 6a10 1110 d864 8818 8814 0100 2100  ..j....d......!.
-00001980: 0000 cb00 0000 0400 0c00 2000 f0ff f8ff  .......... .....
-00001990: 0600 1515 1414 14e8 03d0 06a8 0c0b 1515  ................
-000019a0: 1516 1600 0015 1313 13e8 03d0 0602 1212  ................
-000019b0: e803 0112 e803 0311 1111 e803 0111 b820  ............... 
-000019c0: 9816 d81d 0510 1010 1010 e040 a031 0210  ...........@.1..
-000019d0: 10d0 18d8 1dc8 20e8 6888 82c8 7ed0 8003  ...... .h...~...
-000019e0: 1011 11e0 73a0 86e0 92c8 a203 0000 88e0  ....s...........
-000019f0: 69e8 8f88 25d0 2208 8800 8888 10c9 c9c9  i...%.".........
-00001a00: e803 03ca caca e803 d006 c80c 03cb 1088  ................
-00001a10: e021 885e d85b d114 e01f c8b0 d8f1 d0fc  .!.^.[..........
-00001a20: d102 d893 e861 0ad7 5858 8888 5858 d7d7  .....a..XX..XX..
-00001a30: d7e8 03d8 0603 8888 88e0 12e0 160c 5800  ..............X.
-00001a40: 0000 6a21 d7d7 6a21 0000 a822 02d7 d7b8  ..j!..j!..."....
-00001a50: 1622 0000 00cb 0000 0004 0010 0016 00fa  ."..............
-00001a60: fff8 ff08 0000 0000 1414 1415 e008 e00c  ................
-00001a70: c008 0614 1513 1212 1290 18e8 1401 13e0  ................
-00001a80: 1690 1804 1111 1415 d815 9030 0511 1112  ...........0....
-00001a90: 1414 8818 0500 00c8 1211 e856 0114 e805  ...........V....
-00001aa0: 0712 1111 1111 1516 e080 0410 11c8 c9e0  ................
-00001ab0: 12e8 18e0 15c8 1805 1010 1112 c9a8 180b  ................
-00001ac0: 1010 1010 1516 6a58 1010 12b8 18d0 1404  ......jX........
-00001ad0: 1414 0000 d818 0113 c830 0115 e814 0213  .........0......
-00001ae0: 13d0 d304 8810 1013 e818 e8cd e8bd 0313  ................
-00001af0: 1111 c0e9 0288 11c8 18e8 14a1 0002 8811  ................
-00001b00: e829 02c9 13e8 1403 1413 6aa9 16e0 18e0  .)........j.....
-00001b10: 1403 1288 88a1 2c02 6a58 e830 016a 9014  ......,.jX.0.j..
-00001b20: d018 d028 2300 0000 8900 0000 0400 1600  ...(#...........
-00001b30: 0800 fdff f6ff 0f15 1515 1514 1516 1615  ................
-00001b40: 1313 1313 1312 e808 1540 4344 4212 1515  .........@CDB...
-00001b50: 4041 4143 4342 1414 4140 4242 4443 c008  @AACCB..A@BBDC..
-00001b60: 0214 14d8 18d0 0804 4443 4315 e820 0343  ........DCC.. .C
-00001b70: 4344 d808 8820 8820 d038 0216 15e8 5702  CD... . .8....W.
-00001b80: 4442 e808 0215 14e0 7704 1611 1212 e87a  DB......w......z
-00001b90: 0614 1510 1111 11e8 0a04 1410 1010 e80b  ................
-00001ba0: 0512 1288 8888 e803 0288 88e0 10e0 1201  ................
-00001bb0: 00d0 1101 0024 0000 00d6 0000 0004 0010  .....$..........
-00001bc0: 0016 00f2 fff8 ff03 0000 00e8 03d0 0606  ................
-00001bd0: 0000 1415 1516 9012 e814 0514 1212 1211  ................
-00001be0: 9018 e814 0713 4243 4442 1010 b030 0314  ......BCDB...0..
-00001bf0: 1413 e014 0743 4244 1516 1515 c050 d014  .....CBD.....P..
-00001c00: 0243 42e0 14d0 15b8 1403 4314 15e8 3302  .CB.......C...3.
-00001c10: 13cb a828 0142 c814 04ca ca15 14e0 3c01  ...(.B........<.
-00001c20: 40e0 6501 42e0 4604 1514 caca e84e 0712  @.e.B.F......N..
-00001c30: 1011 1415 4141 e028 0313 1314 c814 076a  ....AA.(.......j
-00001c40: 2100 1011 1214 d832 e014 e857 e014 0300  !......2...W....
-00001c50: 0010 e817 0112 e83c e050 0413 1212 c7d8  .......<.P......
-00001c60: ede8 2bd8 17d8 1401 10d0 140b 0000 6a10  ..+...........j.
-00001c70: 1213 1211 11c9 13a8 1404 0000 d7d7 e843  ...............C
-00001c80: e8a4 a014 d018 046a 1011 10d8 6488 1888  .......j....d...
-00001c90: 1401 0025 0000 00e9 0000 0004 000c 0020  ...%........... 
-00001ca0: 00f0 fff8 ff06 0015 1514 1414 e803 d006  ................
-00001cb0: a80c 1415 1515 1616 0000 1513 1340 4141  .............@AA
-00001cc0: 4242 4344 4343 43e8 0301 43e8 09e8 0b06  BBCDCCC...C.....
-00001cd0: 4444 4444 1111 e020 0140 e01f e821 e824  DDDD... .@...!.$
-00001ce0: e826 0242 43e0 06e0 23e0 22d8 20e0 3ee0  .&.BC...#.". .>.
-00001cf0: 42d0 22e8 4ae0 4ee8 2a03 4443 42e0 60e8  B.".J.N.*.DCB.`.
-00001d00: 6888 82c8 7ed0 800a 1011 1112 1212 1213  h...~...........
-00001d10: 1313 e803 d006 e00c c8a2 0600 0088 1010  ................
-00001d20: 10e8 2488 25c8 2208 8800 8888 10c9 c9c9  ..$.%.".........
-00001d30: e803 03ca caca e803 d006 c80c 03cb 1088  ................
-00001d40: e021 885e d85b d114 e01f e05f d062 d089  .!.^.[....._.b..
-00001d50: e08d d008 e086 0c88 00d7 5858 8888 5858  ..........XX..XX
-00001d60: d7d7 d7e8 03d8 0603 8888 88e0 12e0 160a  ................
-00001d70: 5800 0000 6a21 d7d7 6a21 e809 e80c d006  X...j!..j!......
-00001d80: e00c c016 2600 0000 d000 0000 0400 1000  ....&...........
-00001d90: 1600 faff f8ff 0800 0000 0014 1414 15e0  ................
-00001da0: 08e0 0cc0 0806 1415 1312 1212 9018 e814  ................
-00001db0: 0513 4041 4343 9018 0811 1114 1541 4242  ..@ACC.......ABB
-00001dc0: 4488 1806 1111 1214 1443 8818 0400 c812  D........C......
-00001dd0: 11e8 56c8 1804 1111 1516 e080 0410 11c8  ..V.............
-00001de0: c9e8 17e0 3004 4342 4444 c818 0510 1011  ....0.CBDD......
-00001df0: 12c9 b818 0143 e818 0910 1015 166a 5810  .....C.......jX.
-00001e00: 1012 9818 0615 1614 1400 00d8 1801 13c8  ................
-00001e10: 3001 15e8 1402 1313 d0d3 04c7 1010 13e8  0...............
-00001e20: 18e8 cd06 1313 1313 1111 c0e9 02c7 11c8  ................
-00001e30: 18e8 14a1 0002 c711 e829 02c9 13e8 1403  .........)......
-00001e40: 1413 6aa9 16e0 18e0 1403 1288 88a1 2c02  ..j...........,.
-00001e50: 6a58 e830 016a 9014 d018 d028 0000 0000  jX.0.j.....(....
+00000000: 0400 ff33 0000 002e 00ff 1443 494e 464f  ...3.......CINFO
+00000010: 4256 5253 4e04 0000 0000 0042 4d49 4e56  BVRSN......BMINV
+00000020: 0400 0000 0000 424e 5041 5201 0000 4250  ......BNPAR...BP
+00000030: 414c 5301 0057 0000 3400 ff08 074e 4d4c  ALS..W..4....NML
+00000040: 134e 4d4c 2072 6567 7265 7373 696f 6e20  .NML regression 
+00000050: 7465 7374 0041 2074 6573 7420 6e65 7767  test.A test newg
+00000060: 7266 2074 6573 7469 6e67 204e 4d4c 00ce  rf testing NML..
+00000070: 00ff 0008 0132 0009 5744 5052 5343 5250  .....2..WDPRSCRP
+00000080: 434d 4e54 574f 4f44 4c56 5354 5354 454c  CMNTWOODLVSTSTEL
+00000090: 5645 4849 4252 434b 574f 4f4c 4255 424c  VEHIBRCKWOOLBUBL
+000000a0: 544f 5953 465a 4452 4652 5554 4652 5647  TOYSFZDRFRUTFRVG
+000000b0: 464f 4f44 4f49 4c5f 474f 4f44 5741 5452  FOODOIL_GOODWATR
+000000c0: 4d49 4c4b 434f 414c 494f 5245 414f 5245  MILKCOALIOREAORE
+000000d0: 434c 4159 4752 564c 5341 4e44 4752 4149  CLAYGRVLSANDGRAI
+000000e0: 5253 4752 4d41 495a 434f 5245 4645 5254  RSGRMAIZCOREFERT
+000000f0: 4354 4344 5355 4c50 5748 4541 5246 5052  CTCDSULPWHEARFPR
+00000100: 434f 4c41 5045 5452 5041 5052 544f 4646  COLAPETRPAPRTOFF
+00000110: 5355 4752 5041 5353 4d41 494c 4241 5454  SUGRPASSMAILBATT
+00000120: 5357 4554 5255 4252 464d 5350 454e 5350  SWETRUBRFMSPENSP
+00000130: 4d4e 5350 4649 4352 504c 4153 504c 5354  MNSPFICRPLASPLST
+00000140: 1a00 ff00 0801 0500 1252 4149 4c45 4c52  .........RAILELR
+00000150: 4c4d 4f4e 4f4d 474c 5654 5250 4406 00ff  LMONOMGLVTRPD...
+00000160: 0100 08ff 0400 c800 0118 0800 fdff f4ff  ................
+00000170: 0300 0000 e803 d006 a00c 0615 1515 1514  ................
+00000180: 14e8 0606 1313 1313 1312 c008 0114 d810  ................
+00000190: 0712 1214 1410 1010 e803 0b14 1411 1110  ................
+000001a0: 10d7 d714 1412 d809 0315 1412 d809 e008  ................
+000001b0: e012 0116 8810 8810 8820 e830 d876 0616  ......... .0.v..
+000001c0: 1616 1112 12e8 7a04 1415 1011 e008 0213  ......z.........
+000001d0: 14c0 0802 106a e011 066a 1400 8888 88e8  .....j...j......
+000001e0: 0301 007e 0101 1116 00f2 fff7 ff03 0000  ...~............
+000001f0: 00e8 03d0 06a0 0c88 1888 27e0 3604 1415  ..........'.6...
+00000200: 1516 883e 0700 1414 1212 1111 9018 e014  ...>............
+00000210: e815 0310 10d7 b030 d814 0112 d014 0215  .......0........
+00000220: 15c0 50d8 1401 11e0 2802 cb10 d05c d014  ..P.....(....\..
+00000230: e029 0514 15ca cbcb e806 b814 e83e 0a14  .)...........>..
+00000240: 1514 14c9 cacb 1113 14c0 1402 1211 e814  ................
+00000250: 0210 13e8 1605 ca11 6a21 11e8 0ee0 680f  ........j!....h.
+00000260: 1415 cb10 1310 1313 c8c9 6a21 0000 10e0  ..........j!....
+00000270: 12e8 32e0 5005 1311 1313 d7d9 0302 1011  ..2.P...........
+00000280: d067 d850 0111 d014 0300 006a e816 e069  .g.P.......j...i
+00000290: e050 c014 0400 00d7 d7d8 2de8 50b0 14d0  .P........-.P...
+000002a0: 1804 6a12 1113 e064 9156 e818 8814 8801  ..j....d.V......
+000002b0: 010c 2000 f0ff f8ff 0300 0000 e803 d006  .. .............
+000002c0: a00c b818 0515 1514 1414 e803 d006 a80c  ................
+000002d0: 0515 1515 1616 e820 0312 1212 e803 d006  ....... ........
+000002e0: b80c 0311 1111 e803 0110 a020 d013 d019  ........... ....
+000002f0: d81d 0210 10c8 20a8 12d8 16e0 1ae0 1e02  ...... .........
+00000300: d7d7 e060 e868 8882 c87e d080 0d11 1112  ...`.h...~......
+00000310: 14c9 cacb cbcb 1013 1313 e803 e806 c810  ................
+00000320: e0a3 0600 d810 1111 13d8 2001 11e8 a901  .......... .....
+00000330: 13e0 0401 13c8 1001 13e8 c402 d800 e874  ...............t
+00000340: 0613 c8c9 caca cae0 b3e0 b8e8 21d0 10e8  ............!...
+00000350: 4901 14e8 4009 1010 12c8 c8c9 c9c9 12c8  I...@...........
+00000360: 9fe8 f0d0 10e0 6a0c d800 d758 5888 8858  ......j....XX..X
+00000370: 58d7 d7d7 e803 d806 0388 8888 e012 e016  X...............
+00000380: 0158 e95f 066a 21d7 d76a 2189 68b8 167e  .X._.j!..j!.h..~
+00000390: 0101 1116 00fa fff7 ff03 0000 00e8 03d0  ................
+000003a0: 06a0 0c88 18b8 2704 1414 1415 8834 0700  ......'......4..
+000003b0: 1415 1211 1111 9018 e814 0112 e016 9018  ................
+000003c0: 0111 e83e d815 9830 0611 14ca cb14 1488  ...>...0........
+000003d0: 1807 0010 13c9 cacb 10b0 1802 1516 b016  ................
+000003e0: 0112 e887 e873 0210 10e8 03e0 1809 6a58  .....s........jX
+000003f0: c8c9 cb11 1214 cae8 9f03 1010 10e8 0302  ................
+00000400: d7d7 d018 05ca 1112 13c9 d860 e813 e814  ...........`....
+00000410: 0214 14d8 f204 d711 13c9 d060 0115 e814  ...........`....
+00000420: 0113 c816 e818 01c8 d060 0313 1313 e803  .........`......
+00000430: c016 e018 e060 d017 016a a934 01d7 e860  .....`...j.4...`
+00000440: d82d 0288 88a1 4a02 6a58 e82c 016a 9014  .-....J.jX.,.j..
+00000450: d018 d028 c800 0118 0800 fdff f4ff 0300  ...(............
+00000460: 0000 e803 d006 a00c 0615 1515 1514 14e8  ................
+00000470: 060f 13d7 8858 d712 1515 d7d7 d788 88d7  .....X..........
+00000480: 14e0 0805 d758 8814 14d8 10d0 0801 58c8  .....X........X.
+00000490: 08e8 1001 15c8 10d8 08c0 10c8 18e8 4802  ..............H.
+000004a0: 8816 8828 a010 d820 d876 0d16 1616 1112  ...(... .v......
+000004b0: 1213 1313 1415 1011 e008 0213 14c0 0802  ................
+000004c0: 106a e011 036a 1400 e87d e880 0100 7e01  .j...j...}....~.
+000004d0: 0111 1600 f2ff f7ff 0300 0000 e803 d006  ................
+000004e0: a00c 8818 8827 e036 0414 1515 1688 3e07  .....'.6......>.
+000004f0: 0014 1412 1211 1190 18e0 1406 d788 58d7  ..............X.
+00000500: 10d7 b030 0214 15d8 1407 88d7 5815 1615  ...0........X...
+00000510: 1590 1401 88e8 2802 cb10 d05c b814 0888  ......(....\....
+00000520: 1415 cacb cb10 14e8 2cb8 3ce8 1408 1414  ........,.<.....
+00000530: c9ca cb11 1314 d850 e065 01d7 e814 0210  .......P.e......
+00000540: 13e8 1609 ca11 6a21 1111 1415 d7e8 1713  ......j!........
+00000550: 1415 cb10 1310 1313 c8c9 6a21 0000 1012  ..........j!....
+00000560: 1212 14e8 32e0 5005 1311 1313 d7d9 0302  ....2.P.........
+00000570: 1011 e8ba 0210 10d0 5001 11d0 1403 0000  ........P.......
+00000580: 6ae8 16e8 17d8 50c0 1404 0000 d7d7 d82d  j.....P........-
+00000590: e850 b014 d018 046a 1211 13e0 6491 56e8  .P.....j....d.V.
+000005a0: 1888 1488 0101 0c20 00f0 fff8 ff03 0000  ....... ........
+000005b0: 00e8 03d0 06a0 0cb8 1805 1515 1414 14e8  ................
+000005c0: 03d0 06a8 0c05 1515 1516 16e8 200c 1212  ............ ...
+000005d0: d7d7 d7d7 d788 5888 8888 e803 e008 e80b  ......X.........
+000005e0: 0658 5858 5811 10e0 2002 d788 e81d e804  .XXXX... .......
+000005f0: e024 e028 e810 e82c 0158 d822 d820 0110  .$.(...,.X.". ..
+00000600: d81f d022 c825 d826 0358 88d7 e060 e868  ...".%.&.X...`.h
+00000610: 8882 c07f e881 0f00 0011 1112 14c9 cacb  ................
+00000620: cbcb 1013 1313 e803 e806 c810 e0a3 0600  ................
+00000630: d810 1111 13d8 2005 1112 1212 13e0 0401  ...... .........
+00000640: 13c8 1001 13e8 c40d d800 1010 1113 c8c9  ................
+00000650: caca ca11 11e8 4be0 0401 13c8 10e8 4901  ......K.......I.
+00000660: 14e8 4009 1010 12c8 c8c9 c9c9 12e8 0a01  ..@.............
+00000670: 11e0 0e01 12c8 10e0 6a04 d800 d758 d8ee  ........j....X..
+00000680: c0be e10a d906 d104 e95f 066a 21d7 d76a  ........._.j!..j
+00000690: 2189 68b8 167e 0101 1116 00fa fff7 ff03  !.h..~..........
+000006a0: 0000 00e8 03d0 06a0 0c88 18b8 2704 1414  ............'...
+000006b0: 1415 8834 0700 1415 1211 1111 9018 e814  ...4............
+000006c0: 0512 d7d7 8888 9018 0111 e83e 04d7 d7d7  ...........>....
+000006d0: 5890 1807 1114 cacb 1414 8888 1806 1013  X...............
+000006e0: c9ca cb10 b018 0215 16b0 1601 12e8 8708  ................
+000006f0: 8888 d758 5888 1010 e018 096a 58c8 c9cb  ...XX......jX...
+00000700: 1112 14ca d818 0188 e818 02d7 d7d0 1805  ................
+00000710: ca11 1213 c9d0 60e8 1804 1516 1414 d8f2  ......`.........
+00000720: 04d7 1113 c9d0 6001 15e8 1401 13c8 16e8  ......`.........
+00000730: 1801 c8d0 6003 1313 13e8 03c0 16e0 18e0  ....`...........
+00000740: 60d0 1701 6aa9 3401 d7e8 60d8 2d02 8888  `...j.4...`.-...
+00000750: a14a 026a 58e8 2c01 6a90 14d0 18d0 28c8  .J.jX.,.j.....(.
+00000760: 0001 1808 00fd fff4 ff03 0000 00e8 03d0  ................
+00000770: 06a0 0c0f 6e6e 6e6e 6d6e 6f6f 6e6c 6c6c  ....nnnnmnoonlll
+00000780: 6c6c 6bd8 0804 6b6c 6b6e e810 e807 066b  llk...klkn.....k
+00000790: 6d6d 6b6b 6be8 0308 6d6d 3535 3535 6969  mmkkk...mm5555ii
+000007a0: e810 0235 6be8 0901 6ee8 18e8 09d8 08e8  ...5k...n.......
+000007b0: 0a03 356f 6ed8 1002 356f c010 8818 016f  ..5on...5o.....o
+000007c0: e866 e067 0c6f 6935 6b6b 6c6c 6d6e 6969  .f.g.oi5kkllmnii
+000007d0: 35e0 0a03 6dc8 69d8 0a0b cbc8 c9c9 caca  5...m.i.........
+000007e0: caca cbc8 c8d0 0a03 d7d7 d7e8 0306 d7d7  ................
+000007f0: 0088 8888 e803 0100 7e01 0111 1600 f2ff  ........~.......
+00000800: f7ff 0300 0000 e803 d006 a00c a018 046d  ...............m
+00000810: 6e6e 6f88 28e8 1404 6c6c 6b35 9018 026d  nno.(...llk5...m
+00000820: 6de8 1405 6b35 3569 69b0 30d0 1401 6ce8  m...k55ii.0...l.
+00000830: 1504 6e6f 356e b03c 016c e014 e840 0335  ..no5n.<.l...@.5
+00000840: 6d35 a014 e829 046d 6e35 6cd0 16d8 28e0  m5...).mn5l...(.
+00000850: 2b01 6bd8 14e8 1602 c9cb c814 026b 6cb0  +.k..........kl.
+00000860: 1404 caca c969 e836 e02c c828 016c e014  .....i.6.,.(.l..
+00000870: 086a 2100 6935 6b6d 6dc0 1401 cad0 1406  .j!.i5kmm.......
+00000880: 0000 6969 3535 e840 d014 03c9 c9c7 d903  ..ii55.@........
+00000890: 0388 d7d7 d017 036c c9c9 c014 0400 0058  .......l.......X
+000008a0: 88e8 18e8 2ee0 13c0 1404 0000 d7d7 e018  ................
+000008b0: 9014 c018 02c9 c7d8 6488 1888 1401 0088  ........d.......
+000008c0: 0101 0c20 00f0 fff8 ff03 0000 00e8 03d0  ... ............
+000008d0: 06a0 0cb8 1805 6e6e 6d6d 6de8 03d0 06a8  ......nnmmm.....
+000008e0: 0c05 6e6e 6e6f 6fe8 2006 6c6c 6d6c 6c6c  ..nnnoo. .llmlll
+000008f0: e803 d806 016b e803 e007 066b 6b6b 6b35  .....k.....kkkk5
+00000900: 35e0 20a8 1e01 6be8 18d8 1b01 35e8 1c04  5. ...k.....5...
+00000910: 3535 3569 d040 b81c d836 e038 d81d 0269  555i.@...6.8...i
+00000920: 69d8 20e8 6888 82c8 7ed0 8005 6935 6b6b  i. .h...~...i5kk
+00000930: 69e8 5704 696c 6c35 e004 c008 0269 6de0  i.W.ill5.....im.
+00000940: 1004 0000 d769 e868 e06c e890 0269 6ce8  .....i.h.l...il.
+00000950: 0401 6bc0 2008 6d35 69d7 0088 d7d7 e069  ..k. .m5i......i
+00000960: 0169 b024 e8a5 c024 07d7 d788 88c8 c8c8  .i.$...$........
+00000970: e803 d006 03c9 c9c9 e803 d006 10c9 c9ca  ................
+00000980: caca cb88 00d7 5858 8888 5858 d790 1ce8  ......XX..XX....
+00000990: 12e0 1601 58e9 5f06 6a21 d7d7 6a21 e889  ....X._.j!..j!..
+000009a0: 0258 88c9 6d03 8858 d7b8 167e 0101 1116  .X..m..X...~....
+000009b0: 00fa fff7 ff03 0000 00e8 03d0 06a0 0c06  ................
+000009c0: 0000 6d6d 6d6e 881e 0700 6d6e 6c6b 6b6b  ..mmmn....mnlkkk
+000009d0: 9018 e814 016c e016 9018 0469 356d 6ed8  .....l.....i5mn.
+000009e0: 1590 3005 3535 696d 6d88 18e0 2d02 696b  ..0.55imm...-.ik
+000009f0: d818 0135 d848 026e 6fe0 9603 c8c8 35e8  ...5.H.no.....5.
+00000a00: 18d0 30e8 1803 356b 35e0 1807 c7c8 c8c8  ..0...5k5.......
+00000a10: 6b69 6bc8 48e8 15e8 5204 6e6f 6a58 c018  kik.H...R.nojX..
+00000a20: d848 d814 046d 6d00 00d8 1801 c9e8 3005  .H...mm.......0.
+00000a30: 696c 696d 6ee8 1402 6c6c d0f1 01c7 c818  ilimn...ll......
+00000a40: 016c e81a e8bf c816 d818 01c9 e830 016c  .l...........0.l
+00000a50: e016 03d7 d788 b91e e017 02c9 6bd8 1402  ............k...
+00000a60: 8858 a934 d818 e014 02d7 d7a1 4a04 6a58  .X.4........J.jX
+00000a70: c8c9 8814 c818 d028 c800 0118 0800 fdff  .......(........
+00000a80: f4ff 0300 0000 e803 d006 a00c 0f6e 6ed7  .............nn.
+00000a90: 8858 d76f 6f6e d7d7 d788 88d7 d808 03d7  .X.oon..........
+00000aa0: 5888 e817 e010 0388 6d6d d80f d008 a810  X.......mm......
+00000ab0: 016e c810 e008 e840 0188 c840 0288 6fc8  .n.....@...@..o.
+00000ac0: 30d8 08e0 10e8 58d0 2012 6e6d 6d6e 6f6f  0.....X. .nmmnoo
+00000ad0: 6f69 356b 6b6c 6c6d 6e69 6935 e00a 036d  oi5kkllmnii5...m
+00000ae0: c869 d80a 0bcb c8c9 c9ca caca cacb c8c8  .i..............
+00000af0: d00a e087 e08b 0100 e885 e888 0100 7e01  ..............~.
+00000b00: 0111 1600 f2ff f7ff 0300 0000 e803 d006  ................
+00000b10: a00c a018 046d 6e6e 6f88 28e8 1404 6cd7  .....mnno.(...l.
+00000b20: 8888 9018 0a6d 6d6c 88d7 8858 d710 d7b0  .....mml...X....
+00000b30: 30c8 1407 88d7 586e 6f35 6eb8 3cd8 1401  0.....Xno5n.<...
+00000b40: 88e8 2803 356d 3590 1405 886d 6e35 6cd0  ..(.5m5....mn5l.
+00000b50: 16c0 2801 d7d0 14e8 1602 c9cb d83c e065  ..(..........<.e
+00000b60: 01d7 b814 08ca cbc9 6935 6d6e d7e8 17c8  ........i5mn....
+00000b70: 2801 6ce0 1408 6a21 0069 356b 6d6d c014  (.l...j!.i5kmm..
+00000b80: 03ca caca e014 0900 0069 6935 356b 6c6b  .........ii55klk
+00000b90: d014 03c9 c9c7 d903 e855 d017 036c c9c9  .........U...l..
+00000ba0: c014 0200 00e0 a401 d7e8 2ee0 13c0 1404  ................
+00000bb0: 0000 d7d7 e0bc 9014 c018 02c9 c7d8 6488  ..............d.
+00000bc0: 1888 1401 0088 0101 0c20 00f0 fff8 ff03  ......... ......
+00000bd0: 0000 00e8 03d0 06a0 0cb8 1805 6e6e 6d6d  ............nnmm
+00000be0: 6de8 03d0 06a8 0c05 6e6e 6e6f 6fe8 200c  m.......nnnoo. .
+00000bf0: 6c6c d7d7 d7d7 d788 5888 8888 e803 e008  ll......X.......
+00000c00: e80b 0658 5858 5835 35e0 2002 d788 e81d  ...XXXX55. .....
+00000c10: e804 e024 e028 e810 e82c 0158 d822 d820  ...$.(...,.X.". 
+00000c20: 0110 d81f d022 c825 d826 0358 88d7 e060  .....".%.&.X...`
+00000c30: e868 8882 c87e d080 0c69 356b 6b69 6b6b  .h...~...i5kkikk
+00000c40: 6c69 6c6c 35e0 04c0 0802 696d e010 0600  lill5.....im....
+00000c50: 00d7 6935 35e8 0301 35e8 24e8 20e8 0401  ..i55...5.$. ...
+00000c60: 6bc0 2005 6d35 69d7 00e8 9d05 6969 6969  k. .m5i.....iiii
+00000c70: 69b0 2402 6b6c e850 d04c e0b9 03c8 c8c8  i.$.kl.P.L......
+00000c80: e803 d006 03c9 c9c9 e803 02c9 cae8 030a  ................
+00000c90: cbca caca cacb cb88 0058 d8ed b81c d81f  .........X......
+00000ca0: e01e d018 0800 006a 21d7 d76a 21e9 6703  .......j!..j!.g.
+00000cb0: d858 88c9 6d03 8858 d8b8 187e 0101 1116  .X..m..X...~....
+00000cc0: 00fa fff7 ff03 0000 00e8 03d0 06a0 0c06  ................
+00000cd0: 0000 6d6d 6d6e 881e 0700 6d6e d7d7 d76b  ..mmmn....mn...k
+00000ce0: 9018 066d 6e88 88d7 d7e8 0498 1802 6935  ...mn.........i5
+00000cf0: d82c 0158 8818 0535 3569 6d6d e82f 9018  .,.X...55imm./..
+00000d00: 0469 3569 6ba8 1802 6e6f e096 03c8 c835  .i5ik...no.....5
+00000d10: e818 d830 0788 d758 5888 d735 e018 07c7  ...0...XX..5....
+00000d20: c8c8 c86b 696b d048 0b88 8858 58d7 d769  ...kik.H...XX..i
+00000d30: 6e6f 6a58 c018 d848 e818 066e 6f6d 6d00  nojX...H...nomm.
+00000d40: 00d8 1801 c9e8 3005 696c 696d 6ee8 1402  ......0.ilimn...
+00000d50: 6c6c d0f1 01c7 c818 016c e81a 026c 6cc0  ll.......l...ll.
+00000d60: 16d8 1801 c9e8 3001 6ce0 16e8 d5b9 1ee0  ......0.l.......
+00000d70: 1702 c96b d814 0288 58a9 34d8 18e0 1402  ...k....X.4.....
+00000d80: d7d7 a14a 046a 58c8 c988 14c8 18d0 28c8  ...J.jX.......(.
+00000d90: 0001 1808 00fd fff4 ff03 0000 00e8 0311  ................
+00000da0: 0000 c9c9 caca cbcb cccc c958 5858 5858  ...........XXXXX
+00000db0: 88c0 08d0 1001 88e8 1003 8888 88e8 0308  ................
+00000dc0: ccc9 d8d8 d8d8 d7d7 d810 e809 d018 c008  ................
+00000dd0: 02d8 d8c0 0898 1088 2890 28d0 7703 ccc7  ........(.(.w...
+00000de0: c8e8 81e8 82d8 07e8 8bc0 08c0 10d0 20e8  .............. .
+00000df0: 0801 6ae0 2903 6acb 00d0 8801 007e 0101  ..j.).j......~..
+00000e00: 1116 00f2 fff7 ff03 0000 00e8 03d0 06a0  ................
+00000e10: 0ca0 1804 cacb cccc 8828 e814 0488 88d8  .........(......
+00000e20: d890 18e0 14e8 1503 d8d7 d7b0 30d8 14e8  ............0...
+00000e30: 2be0 1402 c9c9 d06e 02c9 cad0 1403 d8d8  +......n........
+00000e40: cbe8 1402 cac7 b014 e83d c814 02cb c8e0  .........=......
+00000e50: 2805 5858 58d8 58e8 68c0 1402 cbc8 e814  (.XXX.X.h.......
+00000e60: 0188 d015 b014 04cc c8c8 c7e0 5404 d888  ............T...
+00000e70: cbcb b014 056a 21c8 c8c8 e830 01ca 9814  .....j!....0....
+00000e80: 0200 00e8 1403 c8c7 c7b0 3cd8 7f04 00c7  ..........<.....
+00000e90: c8c9 e817 9014 0300 006a e841 01c9 e876  .........j.A...v
+00000ea0: a014 0400 00d7 d7e0 4490 14d0 1801 6ac8  ........D.....j.
+00000eb0: 6491 56e8 1888 1488 0101 0c20 00f0 fff8  d.V........ ....
+00000ec0: ff04 00ca caca e803 d006 a00c d018 0900  ................
+00000ed0: 00ca 8888 8888 8858 d806 d80b b00a 03d7  .......X........
+00000ee0: d8cb d020 0258 58e8 0388 25e0 1f02 d7cc  ... .XX...%.....
+00000ef0: e840 e01d 8843 08d8 d8d8 d8d8 d7d7 d7d8  .@...C..........
+00000f00: 2004 cbcc cccc e803 d006 a00c e018 0600   ...............
+00000f10: 00c8 c9cb c9e8 0303 c9cb cae8 03d0 0603  ................
+00000f20: c9cb cbe8 03e8 1801 cbe0 2003 c7cb cae8  .......... .....
+00000f30: 03d0 06a0 0c03 c7cb c7e8 2001 d7e8 2001  .......... ... .
+00000f40: c988 23b8 2008 cacc d700 c8c8 ccc9 e803  ..#. ...........
+00000f50: 03c8 ccca e803 d006 c00c 02c8 cae8 4001  ..............@.
+00000f60: c7e8 08c0 2388 29e8 9b0b d700 c7c7 c7c7  ....#.).........
+00000f70: c7c8 c8c9 c9e8 0301 c9e8 03d0 06c8 0ce9  ................
+00000f80: 2007 006a 21d7 d76a 21e8 09e8 0cd0 06e0   ..j!..j!.......
+00000f90: 0cc0 167e 0101 1116 00fa fff7 ff03 0000  ...~............
+00000fa0: 00e8 03d0 06a0 0c06 0000 c9ca cacb 881e  ................
+00000fb0: e814 0588 d8d8 d8cb 9818 e814 0188 e016  ................
+00000fc0: e818 01cc b04e 04ca c9c9 cad8 1598 1802  .....N..........
+00000fd0: cac7 8818 c016 9818 01cc d848 01c9 e016  ...........H....
+00000fe0: a030 01d7 e018 02c9 c890 1803 d7d7 d7e8  .0..............
+00000ff0: 1802 6a58 b018 02ca cbe0 1503 cccc c9e8  ..jX............
+00001000: be90 18e0 14c8 bc01 c7a8 4802 cbcb b0ea  ..........H.....
+00001010: b018 02ca caa1 00c0 30e0 1701 6aa9 34d0  ........0...j.4.
+00001020: 48e8 2d02 8888 a14a e090 02ca 6a90 14d0  H.-....J....j...
+00001030: 18d0 28c8 0001 1808 00fd fff4 ff03 0000  ..(.............
+00001040: 00e8 0329 0000 c9c9 caca cbcb cccc c9d8  ...)............
+00001050: 8858 5888 d8cc c988 4649 4a48 88cc c946  .XX.....FIJH...F
+00001060: 4747 4949 48cc c947 4648 484a 49c8 10d0  GGIIH..GFHHJI...
+00001070: 0801 48c8 08e8 2988 2890 2801 4ae0 3004  ..H...).(.(.J.0.
+00001080: 4746 4949 a040 d837 e850 d077 03cc c7c8  GFII.@.7.P.w....
+00001090: e881 e882 d807 e88b c008 c010 d020 e808  ............. ..
+000010a0: 016a e029 0a6a cb00 d8d8 d8d8 d7d7 007e  .j.).j.........~
+000010b0: 0101 1116 00f2 fff7 ff03 0000 00e8 03d0  ................
+000010c0: 06a0 0ca0 1804 cacb cccc 8828 e814 0458  ...........(...X
+000010d0: 88d8 d890 18e0 1406 4849 4a48 d7d7 b030  ........HIJH...0
+000010e0: 02c9 cad8 1407 4948 4acc ccc9 c990 1403  ......IHJ.......
+000010f0: 4948 cbe8 1402 cac7 9828 0149 d014 02cb  IH.......(.I....
+00001100: c888 14d8 1407 cbc8 c9ca 8888 46e0 65c8  ............F.e.
+00001110: 3ce0 1408 ccc8 c8c7 c9ca 4747 e83c 01cb  <.........GG.<..
+00001120: b014 056a 21c8 c8c8 e830 01ca 9814 0200  ...j!....0......
+00001130: 00e8 1403 c8c7 c7b0 3cd8 7f04 00c7 c8c9  ........<.......
+00001140: e817 9014 0300 006a e841 01c9 e876 a014  .......j.A...v..
+00001150: 0400 00d7 d7e0 4490 14d0 1801 6ac8 6491  ......D.....j.d.
+00001160: 56e8 1888 1488 0101 0c20 00f0 fff8 ff04  V........ ......
+00001170: 00ca caca e803 d006 a00c d018 0f00 00ca  ................
+00001180: 8888 4647 4748 4849 4a49 4949 e005 e808  ..FGGHHIJIII....
+00001190: e006 064a 4a4a 88d8 cbe8 2001 46e0 1fe8  ...JJJ.... .F...
+000011a0: 21e0 24e8 27e0 06e8 2c01 4ad8 2201 cce0  !.$.'...,.J."...
+000011b0: 20e0 3ee0 42b8 22d8 2a05 4948 4a49 48e0   .>.B.".*.IHJIH.
+000011c0: 2004 cbcc cccc e803 d006 a00c e018 0600   ...............
+000011d0: 00c8 c9cb c9e8 0303 c9cb cae8 03d0 0603  ................
+000011e0: c9cb cbe8 03e8 1801 cbe0 2003 c7cb cae8  .......... .....
+000011f0: 03d0 06a0 0c03 c7cb c7e8 2001 d7e8 2001  .......... ... .
+00001200: c988 23b8 2008 cacc d700 c8c8 ccc9 e803  ..#. ...........
+00001210: 03c8 ccca e803 d006 c00c 02c8 cae8 4001  ..............@.
+00001220: c7e8 08c0 2388 29e8 9b0b d700 c7c7 c7c7  ....#.).........
+00001230: c7c8 c8c9 c9e8 0301 c9e8 03d0 06c8 0ce9  ................
+00001240: 2007 006a 21d7 d76a 21e8 09e8 0cd0 06e0   ..j!..j!.......
+00001250: 0cc0 167e 0101 1116 00fa fff7 ff03 0000  ...~............
+00001260: 00e8 03d0 06a0 0c06 0000 c9ca cacb 881e  ................
+00001270: e814 0588 d8d8 d8cb 9818 e814 0588 4647  ..............FG
+00001280: 4949 9018 08ca c9c9 ca47 4848 4ad8 1801  II.......GHHJ...
+00001290: ccb8 1601 c7e0 1801 4988 18e8 16d0 1801  ........I.......
+000012a0: 49d0 3001 ccd8 3001 c9e0 16b8 1804 4a49  I.0...0.......JI
+000012b0: d8d7 e018 02c9 c8c0 1801 cae8 3001 49e8  ............0.I.
+000012c0: 1801 d7e8 1802 6a58 a818 01cb e018 03cc  ......jX........
+000012d0: ccc9 e8be 9018 e014 c8bc 01c7 b048 e814  .............H..
+000012e0: b0ea b018 02ca caa1 00c0 30e0 1701 6ab1  ..........0...j.
+000012f0: 3401 6ad0 48e8 2d02 8888 a14a e090 02ca  4.j.H.-....J....
+00001300: 6a90 14d0 18d0 28c8 0001 1808 00fd fff4  j.....(.........
+00001310: ff03 0000 00e8 03d0 06e0 0c0f 1515 1515  ................
+00001320: 1415 1616 1513 1313 1313 12c0 0801 15d8  ................
+00001330: 1003 1212 14c0 0804 1412 1212 e803 0814  ................
+00001340: 1411 1111 1010 10e0 10e0 0901 15e0 18e8  ................
+00001350: 12c0 0802 1615 e028 e808 8820 8820 e828  .......(... . .(
+00001360: 0215 14e0 7704 1611 1212 e87a 0314 1510  ....w......z....
+00001370: e858 e80a 0114 e85c e80b 0512 1288 8888  .X.....\........
+00001380: e803 0488 8810 6ae0 1203 6a11 00d0 1101  ......j...j.....
+00001390: 007e 0101 1116 00f2 fff7 ff03 0000 00e8  .~..............
+000013a0: 03d0 06a0 0ca0 1804 1415 1516 8828 0700  .............(..
+000013b0: 1414 1212 1211 9018 0a14 1413 1312 1111  ................
+000013c0: 1010 10b0 30e0 14e8 15d8 1402 1515 c050  ....0..........P
+000013d0: e014 e015 e014 d015 d814 e03e 0311 1415  ...........>....
+000013e0: e033 01cb b814 e053 d014 04ca ca15 14c8  .3.....S........
+000013f0: 14e8 3fe0 4604 1514 caca e84e 0212 10e8  ..?.F......N....
+00001400: 36c0 1401 14c8 1407 6a21 0010 1112 14d8  6.......j!......
+00001410: 32e0 14e8 57e0 1403 0000 10e8 1701 12e8  2...W...........
+00001420: 3ce0 50e8 8701 88d9 03e8 2bd8 17d8 1401  <.P.......+.....
+00001430: 10d0 1405 0000 6a10 12e0 d201 c9e8 d8b8  ......j.........
+00001440: 1404 0000 d7d7 e843 e0d7 a814 d018 046a  .......C.......j
+00001450: 1011 10d8 6488 1888 1401 0088 0101 0c20  ....d.......... 
+00001460: 00f0 fff8 ff06 0015 1514 1414 e803 d006  ................
+00001470: a80c 0b15 1515 1616 0000 1513 1313 e803  ................
+00001480: d006 0212 12e8 0301 12e8 0303 1111 11e8  ................
+00001490: 0301 11b8 2098 16d8 1d05 1010 1010 10e0  .... ...........
+000014a0: 40a0 3102 1010 d018 d81d c820 e868 8882  @.1........ .h..
+000014b0: c87e d080 0310 1111 e073 a086 e092 c8a2  .~.......s......
+000014c0: 0300 0088 e069 e88f 8825 d022 0888 0088  .....i...%."....
+000014d0: 8810 c9c9 c9e8 0303 caca cae8 03d0 06c8  ................
+000014e0: 0c03 cb10 88e0 2188 5ed8 5bd1 14e0 1fc8  ......!.^.[.....
+000014f0: b0d8 f1d0 fcd1 02d8 93e8 610a d758 5888  ..........a..XX.
+00001500: 8858 58d7 d7d7 e803 d806 0388 8888 e012  .XX.............
+00001510: e016 0c58 0000 006a 21d7 d76a 2100 00a8  ...X...j!..j!...
+00001520: 2202 d7d7 b816 7e01 0111 1600 faff f7ff  ".....~.........
+00001530: 0300 0000 e803 d006 a00c 0600 0014 1414  ................
+00001540: 1588 1e07 0014 1513 1212 1290 18e8 1401  ................
+00001550: 13e0 1690 1804 1111 1415 d815 9030 0511  .............0..
+00001560: 1112 1414 8818 0500 00c8 1211 e856 0114  .............V..
+00001570: e805 0712 1111 1111 1516 e096 0410 11c8  ................
+00001580: c9e0 12e8 18e0 15c8 1805 1010 1112 c9a8  ................
+00001590: 180b 1010 1010 1516 6a58 1010 12b8 18d0  ........jX......
+000015a0: 1404 1414 0000 d818 0113 c830 0115 e814  ...........0....
+000015b0: 0213 13d0 f104 8810 1013 e818 e8cd e8bd  ................
+000015c0: 0313 1111 c107 0288 11c8 18e8 14a1 0002  ................
+000015d0: 8811 e829 02c9 13e8 1403 1413 6aa9 34e0  ...)........j.4.
+000015e0: 18e0 1403 1288 88a1 4a02 6a58 e830 016a  ........J.jX.0.j
+000015f0: 9014 d018 d028 c800 0118 0800 fdff f4ff  .....(..........
+00001600: 0300 0000 e803 d006 e00c 0f15 1515 1514  ................
+00001610: 1516 1615 1313 1313 1312 e808 1540 4344  .............@CD
+00001620: 4212 1515 4041 4143 4342 1414 4140 4242  B...@AACCB..A@BB
+00001630: 4443 c008 0214 14d8 18d0 0804 4443 4315  DC..........DCC.
+00001640: e820 0343 4344 d808 8820 8820 d038 0216  . .CCD... . .8..
+00001650: 15e8 5702 4442 e808 0215 14e0 7704 1611  ..W.DB......w...
+00001660: 1212 e87a 0614 1510 1111 11e8 0a04 1410  ...z............
+00001670: 1010 e80b 0512 1288 8888 e803 0288 88e0  ................
+00001680: 10e0 1201 00d0 1101 007e 0101 1116 00f2  .........~......
+00001690: fff7 ff03 0000 00e8 03d0 06a0 0ca0 1804  ................
+000016a0: 1415 1516 8828 0700 1414 1212 1211 9018  .....(..........
+000016b0: e814 0713 4243 4442 1010 b030 0314 1413  ....BCDB...0....
+000016c0: e014 0743 4244 1516 1515 c050 d014 0243  ...CBD.....P...C
+000016d0: 42e0 14d0 15b8 1403 4314 15e8 3302 13cb  B.......C...3...
+000016e0: a828 0142 c814 04ca ca15 14e0 3c01 40e0  .(.B........<.@.
+000016f0: 6501 42e0 4604 1514 caca e84e 0712 1011  e.B.F......N....
+00001700: 1415 4141 e028 0313 1314 c814 076a 2100  ..AA.(.......j!.
+00001710: 1011 1214 d832 e014 e857 e014 0300 0010  .....2...W......
+00001720: e817 0112 e83c e050 0413 1212 c7d9 03e8  .....<.P........
+00001730: 2bd8 17d8 1401 10d0 140b 0000 6a10 1213  +...........j...
+00001740: 1211 11c9 13a8 1404 0000 d7d7 e843 e8a4  .............C..
+00001750: a014 d018 046a 1011 10d8 6488 1888 1401  .....j....d.....
+00001760: 0088 0101 0c20 00f0 fff8 ff06 0015 1514  ..... ..........
+00001770: 1414 e803 d006 a80c 1415 1515 1616 0000  ................
+00001780: 1513 1340 4141 4242 4344 4343 43e8 0301  ...@AABBCDCCC...
+00001790: 43e8 09e8 0b06 4444 4444 1111 e020 0140  C.....DDDD... .@
+000017a0: e01f e821 e824 e826 0242 43e0 06e0 23e0  ...!.$.&.BC...#.
+000017b0: 22d8 20e0 3ee0 42d0 22e8 4ae0 4ee8 2a03  ". .>.B.".J.N.*.
+000017c0: 4443 42e0 60e8 6888 82c8 7ed0 800a 1011  DCB.`.h...~.....
+000017d0: 1112 1212 1213 1313 e803 d006 e00c c8a2  ................
+000017e0: 0600 0088 1010 10e8 2488 25c8 2208 8800  ........$.%."...
+000017f0: 8888 10c9 c9c9 e803 03ca caca e803 d006  ................
+00001800: c80c 03cb 1088 e021 885e d85b d114 e01f  .......!.^.[....
+00001810: e05f d062 d089 e08d d008 e086 0c88 00d7  ._.b............
+00001820: 5858 8888 5858 d7d7 d7e8 03d8 0603 8888  XX..XX..........
+00001830: 88e0 12e0 160a 5800 0000 6a21 d7d7 6a21  ......X...j!..j!
+00001840: e809 e80c d006 e00c c016 7e01 0111 1600  ..........~.....
+00001850: faff f7ff 0300 0000 e803 d006 a00c 0600  ................
+00001860: 0014 1414 1588 1e07 0014 1513 1212 1290  ................
+00001870: 18e8 1405 1340 4143 4390 1808 1111 1415  .....@ACC.......
+00001880: 4142 4244 8818 0611 1112 1414 4388 1804  ABBD........C...
+00001890: 00c8 1211 e856 c818 0411 1115 16e0 9604  .....V..........
+000018a0: 1011 c8c9 e817 e030 0443 4244 44c8 1805  .......0.CBDD...
+000018b0: 1010 1112 c9b8 1801 43e8 1809 1010 1516  ........C.......
+000018c0: 6a58 1010 1298 1806 1516 1414 0000 d818  jX..............
+000018d0: 0113 c830 0115 e814 0213 13d0 f104 c710  ...0............
+000018e0: 1013 e818 e8cd 0613 1313 1311 11c1 0702  ................
+000018f0: c711 c818 e814 a100 02c7 11e8 2902 c913  ............)...
+00001900: e814 0314 136a a934 e018 e014 0312 8888  .....j.4........
+00001910: a14a 026a 58e8 3001 6a90 14d0 18d0 280d  .J.jX.0.j.....(.
+00001920: 00ff 0200 fe02 0200 0001 0000 0001 000d  ................
+00001930: 00ff 0200 fd02 0202 0003 0002 0003 000d  ................
+00001940: 00ff 0200 fc02 0204 0005 0004 0005 000d  ................
+00001950: 00ff 0200 fb02 0206 0007 0006 0007 000f  ................
+00001960: 00ff 0200 fc80 0200 04fe 00fe 00fe 00fc  ................
+00001970: 0017 00ff 0200 fc89 0300 0300 0000 01fd  ................
+00001980: 0001 0000 0001 0000 00fc 0017 00ff 0200  ................
+00001990: fb89 4700 ff00 0000 01fc 0013 0000 0013  ..G.............
+000019a0: 0000 00fb 0053 00ff 0200 fc89 4700 ff00  .....S......G...
+000019b0: 0000 0719 802f 0000 002f 0000 0014 800c  ...../.../......
+000019c0: 0000 000c 0000 0014 800d 0000 000d 0000  ................
+000019d0: 0019 8019 0000 0019 0000 0019 801b 0000  ................
+000019e0: 001b 0000 0014 801a 0000 001a 0000 0019  ................
+000019f0: 8020 0000 0020 0000 0000 0035 00ff 0200  . ... .....5....
+00001a00: fd89 4700 ff00 0000 0412 8013 0000 0013  ..G.............
+00001a10: 0000 0012 800c 0000 000c 0000 0012 800d  ................
+00001a20: 0000 000d 0000 0012 801a 0000 001a 0000  ................
+00001a30: 0000 0017 00ff 0200 fd89 1000 ffff ffff  ................
+00001a40: 01fd 0016 0000 0016 0000 0000 0021 00ff  .............!..
+00001a50: 0200 fb89 0c00 ffff 0000 02fc 0015 0000  ................
+00001a60: 0015 0000 00fd 0036 0000 0036 0000 00fb  .......6...6....
+00001a70: 0048 00ff 0000 1a01 ff74 0006 0f28 1000  .H.......t...(..
+00001a80: 15ff 29cb 0115 ff1d 0330 0000 15ff 12fd  ..)......0......
+00001a90: 2a40 7a0a 0004 ff26 0003 1e02 0007 0a17  *@z....&........
+00001aa0: b60d 0509 0000 1c28 1e08 0500 0b00 000e  .......(........
+00001ab0: 304c 0000 141e 1619 2400 2500 1b00 ff04  0L......$.%.....
+00001ac0: 007f 01ff 7400 4e4d 4c20 5465 7374 2062  ....t.NML Test b
+00001ad0: 756c 6b20 7761 676f 6e00 0900 ff03 0001  ulk wagon.......
+00001ae0: ff74 0000 fb00 0000 0000 0000            .t..........
```

### Comparing `nml-0.7.2/regression/expected/014_read_special_param.nfo` & `nml-r1512/regression/expected/014_read_special_param.nfo`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,87 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d20
+0 * 4 \d20 
 
-1 * 231 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 03
-"C" "PARA"
-"C" \d0
-"T" "NAME" 7F "Name of the int setting" 00
-"T" "DESC" 7F "Description of a setting" 00
-"B" "MASK" \w1 00
-"B" "LIMI" \w8 \d0 \d2
-"B" "DFLT" \w4 \dx00000000
-00
-"C" \d1
-"B" "TYPE" \w1 01
-"B" "MASK" \w3 \b1 \b0 \b1
-"B" "DFLT" \w4 \dx00000000
-00
-"C" \d2
-"B" "TYPE" \w1 01
-"B" "MASK" \w3 \b1 \b2 \b1
-"B" "DFLT" \w4 \dx00000001
-00
-00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\14" "NML regression test" 00 "A test newgrf testing NML" 00
+1 * 223 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 03 
+"C" "PARA" 
+"C" \d0 
+"T" "NAME" 7F "Name of the int setting" 00 
+"T" "DESC" 7F "Description of a setting" 00 
+"B" "MASK" \w1 00 
+"B" "LIMI" \w8 \d0 \d2 
+"B" "DFLT" \w4 \dx00000000 
+00 
+"C" \d1 
+"B" "TYPE" \w1 01 
+"B" "MASK" \w3 \b1 \b0 \b1 
+"B" "DFLT" \w4 \dx00000000 
+00 
+"C" \d2 
+"B" "TYPE" \w1 01 
+"B" "MASK" \w3 \b1 \b2 \b1 
+"B" "DFLT" \w4 \dx00000001 
+00 
+00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "NML\14" "NML regression test" 00 "A test newgrf testing NML" 00 
 // param[16] = param[0]
-3 * 5 0D 10 \D= 00 00
+3 * 5 0D 10 \D= 00 00 
 
 // param[17] = 0
-4 * 9 0D 11 \D= FF 00 \dx00000000
+4 * 9 0D 11 \D= FF 00 \dx00000000 
 
-5 * 6 09 01 01 \70 00 01
+5 * 6 09 01 01 \70 00 01 
 
 // param[17] = 1
-6 * 9 0D 11 \D= FF 00 \dx00000001
+6 * 9 0D 11 \D= FF 00 \dx00000001 
 
 // param[18] = 0
-7 * 9 0D 12 \D= FF 00 \dx00000000
+7 * 9 0D 12 \D= FF 00 \dx00000000 
 
-8 * 6 09 01 01 \70 02 01
+8 * 6 09 01 01 \70 02 01 
 
 // param[18] = 1
-9 * 9 0D 12 \D= FF 00 \dx00000001
+9 * 9 0D 12 \D= FF 00 \dx00000001 
 
 // param[19] = param[0]
-10 * 9 0D 13 \D= 00 FE \dx014C4D4E
+10 * 9 0D 13 \D= 00 FE \dx014C4D4E 
 
 // param[158] = (param[158] | 2)
-11 * 9 0D 9E \D| 9E FF \dx00000002
+11 * 9 0D 9E \D| 9E FF \dx00000002 
 
 // param[20] = 0
-12 * 9 0D 14 \D= FF 00 \dx00000000
+12 * 9 0D 14 \D= FF 00 \dx00000000 
 
-13 * 6 09 9E 01 \70 03 01
+13 * 6 09 9E 01 \70 03 01 
 
 // param[20] = 1
-14 * 9 0D 14 \D= FF 00 \dx00000001
+14 * 9 0D 14 \D= FF 00 \dx00000001 
 
 // param[142] = -2
-15 * 9 0D 8E \D= FF 00 \dxFFFFFFFE
+15 * 9 0D 8E \D= FF 00 \dxFFFFFFFE 
 
 // param[21] = param[164]
-16 * 5 0D 15 \D= A4 00
+16 * 5 0D 15 \D= A4 00 
 
-// param[125] = param[19]
-17 * 9 0D 7D \D= 13 FE \dx0000FFFF
+// param[66] = param[19]
+17 * 9 0D 42 \D= 13 FE \dx0000FFFF 
 
-// param[126] = (param[125] & 255)
-18 * 9 0D 7E \D& 7D FF \dx000000FF
+// param[65] = (param[66] & 255)
+18 * 9 0D 41 \D& 42 FF \dx000000FF 
 
-// param[127] = (param[126] + 12)
-19 * 9 0D 7F \D+ 7E FF \dx0000000C
+// param[64] = (param[65] + 12)
+19 * 9 0D 40 \D+ 41 FF \dx0000000C 
 
-// param[22] = (1 << param[127])
-20 * 9 0D 16 \D<< FF 7F \dx00000001
+// param[22] = (1 << param[64])
+20 * 9 0D 16 \D<< FF 40 \dx00000001
```

### Comparing `nml-0.7.2/regression/expected/015_basic_object.nfo` & `nml-r1512/regression/expected/015_basic_object.nfo`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d6
+0 * 4 \d6 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\15" "NML regression test" 00 "A test newgrf testing NML" 00
-3 * 33 04 0F FF 02 \wxD000 "Miscellaneous" 00 "Basic object" 00
-
-// Name: obj_basic_tile - feature 0F
-4 * 18 02 0F FF \b1 \dx0000058C
-\dx03078A48 \b0 \b0 \b0 \b16 \b16 \b30
-
-5 * 41 00 0F \b11 01 FF \wx0000
-08 "MISC"
-09 \wxD000
-0A \wxD001
-0B 07
-0C 11
-0E \dx000A96C9
-0F \dx000AC196
-0D 01
-14 01
-10 \wx0800
-16 04
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "NML\15" "NML regression test" 00 "A test newgrf testing NML" 00 
+// Name: obj_basic_tile
+3 * 18 02 0F FE \b1 \dx0000058C 
+\dx03078A48 \b0 \b0 \b0 \b16 \b16 \b30 
+
+4 * 39 00 0F \b11 01 00 
+08 "MISC" 
+09 \wxD000 
+0A \wxD001 
+0B 07 
+0C 11 
+0E \dx000A96C9 
+0F \dx000AC196 
+0D 01 
+14 01 
+10 \wx0800 
+16 04 
 
-6 * 7 03 0F 01 00 \b0
-\wx00FF 	// obj_basic_tile;
+5 * 7 03 0F 01 00 \b0 
+\wx00FE 
+
+6 * 33 04 08 FF 02 \wxD000 "Miscellaneous" 00 "Basic object" 00
```

### Comparing `nml-0.7.2/regression/expected/016_basic_airporttiles.nfo` & `nml-r1512/regression/expected/016_basic_airporttiles.nfo`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 6 01 11 \b1 FF \wx0001
+0 * 6 01 11 \b1 FF \wx0001 
 
-1 opengfx_trains_start.pcx 8bpp 142 112 8 22 -3 -10 normal
+1 opengfx_trains_start.pcx 142 112 01 22 8 -3 -10 
 
-// Name: small_airport_tiles_graphics - feature 11
-2 * 15 02 11 FF \b1 \dx00000F8D
-\dxC0000000 \b0 \b0 80
+// Name: small_airport_tiles_graphics
+2 * 15 02 11 FE \b1 \dx00000F8D 
+\dxC0000000 \b0 \b0 80 
 
-3 * 16 00 11 \b4 01 FF \wx0000
-08 00
-0F \wx0103
-10 01
-11 01
+3 * 16 00 11 \b5 01 00 
+08 00 
+0F \wx0103 
+10 01 
+11 01 
+0E 01 
 
-4 * 7 03 11 01 00 \b0
-\wx00FF 	// small_airport_tiles_graphics;
+4 * 7 03 11 01 00 \b0 
+\wx00FE
```

### Comparing `nml-0.7.2/regression/expected/017_articulated_tram.grf` & `nml-r1512/regression/expected/017_articulated_tram.grf`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,117 @@
-00000000: 0000 4752 4682 0d0a 1a0a a401 0000 0004  ..GRF...........
-00000010: 0000 00ff 1200 0000 3600 0000 ff14 4349  ........6.....CI
-00000020: 4e46 4f42 5652 534e 0400 0000 0000 424d  NFOBVRSN......BM
-00000030: 494e 5604 0000 0000 0042 4e50 4152 0100  INV......BNPAR..
-00000040: 0042 5041 4c53 0100 5742 424c 5452 0100  .BPALS..WBBLTR..
-00000050: 3800 0034 0000 00ff 0808 4e4d 4c17 4e4d  8..4......NML.NM
-00000060: 4c20 7265 6772 6573 7369 6f6e 2074 6573  L regression tes
-00000070: 7400 4120 7465 7374 206e 6577 6772 6620  t.A test newgrf 
-00000080: 7465 7374 696e 6720 4e4d 4c00 1700 0000  testing NML.....
-00000090: ff02 01ff 8910 00ff ffff ff01 5880 0100  ............X...
-000000a0: 0000 0300 0000 ff80 4a00 0000 ff00 0119  ........J.......
-000000b0: 01ff 5800 060f 0428 031e 1f86 f30a 0002  ..X....(........
-000000c0: 010a 484c 0000 0987 118f 08ff 15fe 1316  ..HL............
-000000d0: 1458 0eff 0710 184d 1980 0f2d 1d01 0016  .X.....M...-....
-000000e0: 0000 0000 1e00 0016 0000 0000 2400 1600  ............$...
-000000f0: 0000 0010 ff1c 0119 0000 00ff 0401 7f01  ................
-00000100: ff58 0046 6f73 7465 7220 5475 7262 6f20  .X.Foster Turbo 
-00000110: 5472 616d 0006 0000 00ff 0101 01ff 0800  Tram............
-00000120: 0400 0000 fd08 0000 0004 0000 00fd 0900  ................
-00000130: 0000 0400 0000 fd0a 0000 0004 0000 00fd  ................
-00000140: 0b00 0000 0400 0000 fd0c 0000 0004 0000  ................
-00000150: 00fd 0d00 0000 0400 0000 fd0e 0000 0004  ................
-00000160: 0000 00fd 0f00 0000 0900 0000 ff02 01fe  ................
-00000170: 0101 0000 0000 0900 0000 ff00 0101 01ff  ................
-00000180: 5800 1710 1700 0000 ff02 01fe 890c 00ff  X...............
-00000190: ff00 0001 ff00 1600 0000 1600 0000 fe00  ................
-000001a0: 0900 0000 ff03 0101 ff58 0000 fe00 0000  .........X......
-000001b0: 0000 0800 0000 7700 0000 0400 1200 0800  ......w.........
-000001c0: fdff f6ff 1200 c9ca cacb cbcc 00c7 c9ca  ................
-000001d0: c9ca cbcc cbc7 c9e8 1101 cce0 08e8 1003  ................
-000001e0: cacc cad8 10d8 18c0 2003 caca d8d0 2003  ........ ..... .
-000001f0: cbd8 cac8 08d8 3002 cbcc c808 d010 04c7  ......0.........
-00000200: c8c9 d8e8 59e8 0702 ca6a e862 0fc8 8381  ....Y....j.b....
-00000210: caca 8381 cbc8 8483 caca 8483 d848 01ca  .............H..
-00000220: e87b 02c7 b5e0 0903 b7cb 00e0 2903 caca  .{..........)...
-00000230: 0009 0000 00c8 0000 0004 0010 0014 00f2  ................
-00000240: fffb ff03 0000 00e8 03d0 0604 c9ca cccb  ................
-00000250: a010 0800 00c7 caca cbcb cba0 1603 c7c9  ................
-00000260: c9e0 1304 cbcc cccc a812 e839 e811 e018  ...........9....
-00000270: 046a d8d8 d8e8 03d8 37e8 1205 cacb ca84  .j......7.......
-00000280: 83d0 36e8 38d8 1201 c9e8 1203 8584 00d8  ..6.8...........
-00000290: 1201 caa8 1204 83ca c7c8 e825 a824 08ca  ...........%.$..
-000002a0: caca cac9 c8c8 c790 1209 c8ca 8381 c9c8  ................
-000002b0: c7cb cab8 240a cb82 58c8 8483 c9c9 c9c7  ....$...X.......
-000002c0: c036 0ccc 8258 826a 00c7 c8c9 8381 c7c8  .6...X.j........
-000002d0: 1202 cbc9 e812 0400 00b5 c8e8 2b01 c8d8  ............+...
-000002e0: 5903 cbc9 c8c8 e605 c8c8 c8c9 c8e8 d8e8  Y...............
-000002f0: 48a8 fc03 c8b5 c8e8 5ad8 36a0 16d0 48c1  H.......Z.6...H.
-00000300: 380a 0000 00df 0000 0004 000f 001c 00f2  8...............
-00000310: fff8 ff05 6ad8 0000 00e8 03d0 06a0 0ce0  ....j...........
-00000320: 1801 d888 1e88 1e88 3ca0 4a07 cac9 d8d8  ........<.J.....
-00000330: c9c9 c9e8 03d0 06d0 0ce0 6c05 c9c9 cbcb  ..........l.....
-00000340: c9d8 1e03 cac9 cae8 0304 caca cacb e803  ................
-00000350: 02ca cae8 3504 cacb cbcc e014 0358 58cb  ....5........XX.
-00000360: e80b e017 01cc e807 05cc cbcc cccc e805  ................
-00000370: d80d e00f d813 d017 e03f e043 e022 e026  .........?.C.".&
-00000380: c008 a010 01cb d865 d866 d841 d006 07cb  .......e.f.A....
-00000390: 8080 cb81 8384 e004 c008 c010 0780 8181  ................
-000003a0: 85cb 8384 e004 c008 b810 0381 80ca e8c1  ................
-000003b0: 03cb cac8 8854 e09b e8cf 01b5 d063 d072  .....T.......c.r
-000003c0: d09d d0c9 e8cf 0900 cbcb 8258 5858 58d7  ...........XXXX.
-000003d0: c887 02cc ccd0 0f03 cccd cde1 8506 826a  ...............j
-000003e0: 8888 826a b98f b00f 0b00 0000 e300 0000  ...j............
-000003f0: 0400 1200 1400 faff f9ff 0400 0000 6ae8  ..............j.
-00000400: 04e8 07d0 06c0 0c01 d888 1588 15b0 3303  ..............3.
-00000410: ccd8 cb90 4007 cac9 cacb cbd8 cca0 1603  ....@...........
-00000420: c9c9 cae8 03e8 15b0 1603 c9c9 c9e0 1604  ................
-00000430: caca cbcc b816 0283 81c0 1601 cbb8 1602  ................
-00000440: 8483 e816 01c7 e02c 0ccb cacc cbcc cbcc  .......,........
-00000450: ca00 00c7 c9a8 1601 cbe0 2c05 ca00 c8c8  ..........,.....
-00000460: c9c0 1601 cae8 55e0 4103 cbca d7e8 15d0  ......U.A.......
-00000470: 2cd8 1507 cccc 81cb c758 d7e0 1601 c8d8  ,........X......
-00000480: 58e8 5409 c780 83cb 0082 6a58 d7e8 a2d0  X.T.......jX....
-00000490: 42e8 1302 8184 e866 e816 03c7 cacb e82b  B......f.......+
-000004a0: e86e 05ca c781 83ca e014 e92f 03c6 c8cb  .n........./....
-000004b0: e858 04c8 c9ca 80e8 bdc8 1403 0000 c8e8  .X..............
-000004c0: 58d8 6601 34c0 28d8 4203 58d7 c8e8 b903  X.f.4.(.B.X.....
-000004d0: cacb 000c 0000 0079 0000 0004 0012 0008  .......y........
-000004e0: 00fd fff6 ff04 0000 006a e804 0a00 00c7  .........j......
-000004f0: c9d8 c9ca c900 c7d8 080a cbc9 c7c9 cad8  ................
-00000500: cacb ccca d808 01ca e008 02c9 cae8 1001  ................
-00000510: cbe8 18e8 1fd8 08e8 1ed8 10d8 18e0 3102  ..............1.
-00000520: cbcc d008 e830 01cb d017 08cc cbca 8181  .....0..........
-00000530: 8180 81e8 49e0 0705 8384 ccc9 80e0 0701  ....I...........
-00000540: 84d8 20e8 3ae8 4d03 ca34 34e0 0801 c9e0  .. .:.M..44.....
-00000550: 6102 caca 0d00 0000 da00 0000 0400 1200  a...............
-00000560: 1400 f2ff f7ff 0300 0000 e803 d006 e00c  ................
-00000570: 016a 8811 e820 01d8 8824 8813 c026 02c9  .j... ...$...&..
-00000580: cb90 4c07 c7c9 d8ca cacb cba8 160a c7c9  ..L.............
-00000590: c9d8 cbcc cbcc cccc c02b e812 02ca cad0  .........+......
-000005a0: 12e8 19c0 12e8 35e0 240b caca ca84 8300  ......5.$.......
-000005b0: 00c9 cacc cae8 14d8 1201 c9e8 1203 8584  ................
-000005c0: 00d8 58e8 47b8 1204 cbcb c9c9 e86b e05b  ..X.G........k.[
-000005d0: b812 06ca cbc9 80c9 c9e0 5a02 cbcb c812  ..........Z.....
-000005e0: 07ca cccc c980 8080 e82b d848 e87c 0bca  .........+.H.|..
-000005f0: cb82 58c9 c880 8081 81c9 b824 0d82 5882  ..X........$..X.
-00000600: 6a00 c8c9 8183 83c9 8584 e885 e8a1 01c8  j...............
-00000610: e812 e88a 03c8 c9c9 e835 0183 e0d7 02c9  .........5......
-00000620: c8d1 3a04 c9c9 43c9 e0c5 e848 c812 d016  ..:...C....H....
-00000630: e8d9 d848 c160 0e00 0000 de00 0000 0400  ...H.`..........
-00000640: 0f00 1c00 f2ff f8ff 0300 0000 e803 d006  ................
-00000650: a00c 0400 00d8 6a88 1cb0 1a01 d888 3688  ......j.......6.
-00000660: 1a05 0000 c9c9 c9e8 03d0 06d0 0c04 d8d8  ................
-00000670: c9ca d86c 03ca cacb e803 05ca caca cac9  ...l............
-00000680: e803 01ca d81a 0bc9 cbcb cbcb 0000 cccc  ................
-00000690: cbcc e80a 01cc e021 06cb cbca cb58 58e0  .......!.....XX.
-000006a0: 24e0 1301 cae8 37e8 0ad8 21c0 25e0 34d8  $.....7...!.%.4.
-000006b0: 06e8 17e8 1ad0 06a0 0cd8 2f01 80d8 28d8  ........../...(.
-000006c0: 2de0 54d0 7a01 cad8 7108 cc81 8180 8483  -.T.z...q.......
-000006d0: 81cb e004 c008 d010 07cb 8383 ca80 8185  ................
-000006e0: e809 e004 c008 b810 e8b9 8854 e0cf 01c8  ...........T....
-000006f0: e0b5 d8ca d0bf d869 b06e e81c 0a00 cdcd  .......i.n......
-00000700: ccd7 5858 5858 82e8 ead0 98d0 0fe0 fde9  ..XXXX..........
-00000710: 8906 6a82 8888 6a82 b992 b80f 0f00 0000  ..j...j.........
-00000720: c800 0000 0400 1000 1400 faff f9ff 0800  ................
-00000730: 0000 00cb cacb cbe0 08e0 0cd0 08e8 1104  ................
-00000740: cbcb cccc a016 01ca d014 a016 03ca c9ca  ................
-00000750: e816 e805 e82b c02c 0783 81c9 c9c9 c9c9  .....+.,........
-00000760: e81b e041 08d8 d8d8 d8d8 6a84 83e8 1601  ...A......j.....
-00000770: c7e0 1602 cbca e041 e058 02c8 83a8 16d8  .......A.X......
-00000780: 5703 cc00 c8e8 3ba8 2ce0 5503 ccc8 d7e0  W.....;.,.U.....
-00000790: 50e0 4201 c8e0 42e0 ab05 cbd7 58d7 c9e8  P.B...B.....X...
-000007a0: 2c01 c8d8 58e0 8409 ca83 8100 826a 58d7  ,...X........jX.
-000007b0: cac0 2ce8 1103 ca84 83e8 dc03 826a c7e8  ..,..........j..
-000007c0: a2d8 58e8 11e8 c4d0 e803 c7c8 cbd8 58e0  ..X...........X.
-000007d0: 3c02 cab5 c0fc d058 d814 01c8 b910 e058  <......X.......X
-000007e0: 03cb cab5 a812 d016 01c9 d024 0000 0000  ...........$....
+00000000: 0400 ff12 0000 002e 00ff 1443 494e 464f  ...........CINFO
+00000010: 4256 5253 4e04 0000 0000 0042 4d49 4e56  BVRSN......BMINV
+00000020: 0400 0000 0000 424e 5041 5201 0000 4250  ......BNPAR...BP
+00000030: 414c 5301 0057 0000 3400 ff08 0774 6573  ALS..W..4....tes
+00000040: 744e 4d4c 2072 6567 7265 7373 696f 6e20  tNML regression 
+00000050: 7465 7374 0041 2074 6573 7420 6e65 7767  test.A test newg
+00000060: 7266 2074 6573 7469 6e67 204e 4d4c 0006  rf testing NML..
+00000070: 00ff 0101 01ff 0800 9800 0112 0800 fdff  ................
+00000080: f6ff 1200 c9ca cacb cbcc 00c7 c9ca c9ca  ................
+00000090: cbcc cbc7 c9e8 1101 cce0 08e8 1003 cacc  ................
+000000a0: cad8 10d8 18c0 2003 caca d8d0 2003 cbd8  ...... ..... ...
+000000b0: cac8 08d8 3002 cbcc c808 d010 04c7 c8c9  ....0...........
+000000c0: d8e8 59e8 0702 ca6a e862 0fc8 8381 caca  ..Y....j.b......
+000000d0: 8381 cbc8 8483 caca 8483 d848 01ca e87b  ...........H...{
+000000e0: 02c7 b5e0 0903 b7cb 00e0 2903 caca 0070  ..........)....p
+000000f0: 0101 1214 00f2 fffb ff03 0000 00e8 03d0  ................
+00000100: 0604 c9ca cccb a010 0800 00c7 caca cbcb  ................
+00000110: cba0 1603 c7c9 c9e0 1304 cbcc cccc a812  ................
+00000120: e839 e811 e018 046a d8d8 d8e8 03d8 37e8  .9.....j......7.
+00000130: 1205 cacb ca84 83d0 36e8 38d8 1201 c9e8  ........6.8.....
+00000140: 1203 8584 00d8 1201 caa8 1204 83ca c7c8  ................
+00000150: e825 a824 08ca caca cac9 c8c8 c790 1209  .%.$............
+00000160: c8ca 8381 c9c8 c7cb cab8 240a cb82 58c8  ..........$...X.
+00000170: 8483 c9c9 c9c7 c036 0ccc 8258 826a 00c7  .......6...X.j..
+00000180: c8c9 8381 c7c8 1202 cbc9 e812 0400 00b5  ................
+00000190: c8e8 2b01 c8d8 5903 cbc9 c8c8 e605 c8c8  ..+...Y.........
+000001a0: c8c9 c8e8 d8e8 48a8 fc03 c8b5 c8e8 5ad8  ......H.......Z.
+000001b0: 36a0 16d0 4891 2888 1188 20e1 64ac 0101  6...H.(... .d...
+000001c0: 0f1c 00f2 fff8 ff05 6ad8 0000 00e8 03d0  ........j.......
+000001d0: 06a0 0ce0 1801 d888 1e88 1e88 3ca0 4a07  ............<.J.
+000001e0: cac9 d8d8 c9c9 c9e8 03d0 06d0 0ce0 6c05  ..............l.
+000001f0: c9c9 cbcb c9d8 1e03 cac9 cae8 0304 caca  ................
+00000200: cacb e803 02ca cae8 3504 cacb cbcc e014  ........5.......
+00000210: 0358 58cb e80b e017 01cc e807 05cc cbcc  .XX.............
+00000220: cccc e805 d80d e00f d813 d017 e03f e043  .............?.C
+00000230: e022 e026 c008 a010 01cb d865 d866 d841  .".&.......e.f.A
+00000240: d006 07cb 8080 cb81 8384 e004 c008 c010  ................
+00000250: 0780 8181 85cb 8384 e004 c008 b810 0381  ................
+00000260: 80ca e8c1 03cb cac8 8854 e09b e8cf 01b5  .........T......
+00000270: d063 d072 d09d d0c9 e8cf 0900 cbcb 8258  .c.r...........X
+00000280: 5858 58d7 c887 02cc ccd0 0f03 cccd cde1  XXX.............
+00000290: 8506 826a 8888 826a b98f b00f 7001 0112  ...j...j....p...
+000002a0: 1400 faff f9ff 0400 0000 6ae8 04e8 07d0  ..........j.....
+000002b0: 06c0 0c01 d888 1588 15b0 3303 ccd8 cb90  ..........3.....
+000002c0: 4007 cac9 cacb cbd8 cca0 1603 c9c9 cae8  @...............
+000002d0: 03e8 15b0 1603 c9c9 c9e0 1604 caca cbcc  ................
+000002e0: b816 0283 81c0 1601 cbb8 1602 8483 e816  ................
+000002f0: 01c7 e02c 0ccb cacc cbcc cbcc ca00 00c7  ...,............
+00000300: c9a8 1601 cbe0 2c05 ca00 c8c8 c9c0 1601  ......,.........
+00000310: cae8 55e0 4103 cbca d7e8 15d0 2cd8 1507  ..U.A.......,...
+00000320: cccc 81cb c758 d7e0 1601 c8d8 58e8 5409  .....X......X.T.
+00000330: c780 83cb 0082 6a58 d7e8 a2d0 42e8 1302  ......jX....B...
+00000340: 8184 e866 e816 03c7 cacb e82b e86e 05ca  ...f.......+.n..
+00000350: c781 83ca e014 e92f 03c6 c8cb e858 04c8  ......./.....X..
+00000360: c9ca 80e8 bdc8 1403 0000 c8e8 58d8 6601  ............X.f.
+00000370: 34c0 28d8 4203 58d7 c8e8 b903 cacb 0098  4.(.B.X.........
+00000380: 0001 1208 00fd fff6 ff04 0000 006a e804  .............j..
+00000390: 0a00 00c7 c9d8 c9ca c900 c7d8 080a cbc9  ................
+000003a0: c7c9 cad8 cacb ccca d808 01ca e008 02c9  ................
+000003b0: cae8 1001 cbe8 18e8 1fd8 08e8 1ed8 10d8  ................
+000003c0: 18e0 3102 cbcc d008 e830 01cb d017 08cc  ..1......0......
+000003d0: cbca 8181 8180 81e8 49e0 0705 8384 ccc9  ........I.......
+000003e0: 80e0 0701 84d8 20e8 3ae8 4d03 ca34 34e0  ...... .:.M..44.
+000003f0: 0801 c9e0 6102 caca 7001 0112 1400 f2ff  ....a...p.......
+00000400: f7ff 0300 0000 e803 d006 e00c 016a 8811  .............j..
+00000410: e820 01d8 8824 8813 c026 02c9 cb90 4c07  . ...$...&....L.
+00000420: c7c9 d8ca cacb cba8 160a c7c9 c9d8 cbcc  ................
+00000430: cbcc cccc c02b e812 02ca cad0 12e8 19c0  .....+..........
+00000440: 12e8 35e0 240b caca ca84 8300 00c9 cacc  ..5.$...........
+00000450: cae8 14d8 1201 c9e8 1203 8584 00d8 58e8  ..............X.
+00000460: 47b8 1204 cbcb c9c9 e86b e05b b812 06ca  G........k.[....
+00000470: cbc9 80c9 c9e0 5a02 cbcb c812 07ca cccc  ......Z.........
+00000480: c980 8080 e82b d848 e87c 0bca cb82 58c9  .....+.H.|....X.
+00000490: c880 8081 81c9 b824 0d82 5882 6a00 c8c9  .......$..X.j...
+000004a0: 8183 83c9 8584 e885 e8a1 01c8 e812 e88a  ................
+000004b0: 03c8 c9c9 e835 0183 e0d7 02c9 c8d1 3a04  .....5........:.
+000004c0: c9c9 43c9 e0c5 e848 c812 d016 e8d9 d848  ..C....H.......H
+000004d0: c160 ac01 010f 1c00 f2ff f8ff 0300 0000  .`..............
+000004e0: e803 d006 a00c 0400 00d8 6a88 1cb0 1a01  ..........j.....
+000004f0: d888 3688 1a05 0000 c9c9 c9e8 03d0 06d0  ..6.............
+00000500: 0c04 d8d8 c9ca d86c 03ca cacb e803 05ca  .......l........
+00000510: caca cac9 e803 01ca d81a 0bc9 cbcb cbcb  ................
+00000520: 0000 cccc cbcc e80a 01cc e021 06cb cbca  ...........!....
+00000530: cb58 58e0 24e0 1301 cae8 37e8 0ad8 21c0  .XX.$.....7...!.
+00000540: 25e0 34d8 06e8 17e8 1ad0 06a0 0cd8 2f01  %.4.........../.
+00000550: 80d8 28d8 2de0 54d0 7a01 cad8 7108 cc81  ..(.-.T.z...q...
+00000560: 8180 8483 81cb e004 c008 d010 07cb 8383  ................
+00000570: ca80 8185 e809 e004 c008 b810 e8b9 8854  ...............T
+00000580: e0cf 01c8 e0b5 d8ca d0bf d869 b06e e81c  ...........i.n..
+00000590: 0a00 cdcd ccd7 5858 5858 82e8 ead0 98d0  ......XXXX......
+000005a0: 0fe0 fde9 8906 6a82 8888 6a82 b992 b80f  ......j...j.....
+000005b0: 7001 0112 1400 faff f9ff 0800 0000 00cb  p...............
+000005c0: cacb cbe0 08e0 0cd0 08e8 1104 cbcb cccc  ................
+000005d0: a016 01ca d014 a016 03ca c9ca e816 e805  ................
+000005e0: e82b c02c 0783 81c9 c9c9 c9c9 e81b e041  .+.,...........A
+000005f0: 08d8 d8d8 d8d8 6a84 83e8 1601 c7e0 1602  ......j.........
+00000600: cbca e041 e058 02c8 83a8 16d8 5703 cc00  ...A.X......W...
+00000610: c8e8 3ba8 2ce0 5503 ccc8 d7e0 50e0 4201  ..;.,.U.....P.B.
+00000620: c8e0 42e0 ab05 cbd7 58d7 c9e8 2c01 c8d8  ..B.....X...,...
+00000630: 58e0 8409 ca83 8100 826a 58d7 cac0 2ce8  X........jX...,.
+00000640: 1103 ca84 83e8 dc03 826a c7e8 a2d8 58e8  .........j....X.
+00000650: 11e8 c4d0 e803 c7c8 cbd8 58e0 3c02 cab5  ..........X.<...
+00000660: c0fc d058 d814 01c8 b910 e058 03cb cab5  ...X.......X....
+00000670: a812 d016 01c9 8812 9141 881b 0200 0009  .........A......
+00000680: 00ff 0201 fe01 0100 0000 0017 00ff 0201  ................
+00000690: fd89 1000 ffff ffff 0158 8001 0000 0003  .........X......
+000006a0: 0000 0000 0017 00ff 0201 fe89 0c00 ffff  ................
+000006b0: 0000 01fd 0016 0000 0016 0000 00fe 0042  ...............B
+000006c0: 00ff 0001 1801 ff58 0006 0f04 2803 1e1f  .......X....(...
+000006d0: 86f3 0a00 0201 0a48 4c00 0009 8711 8f08  .......HL.......
+000006e0: 9513 1614 580e ff07 1018 4d19 800f 2d1d  ....X.....M...-.
+000006f0: 0100 10ff 1e00 0010 ff16 0000 0000 10ff  ................
+00000700: 1c01 1710 1b00 ff04 017f 01ff 5800 466f  ............X.Fo
+00000710: 7374 6572 2045 7870 7265 7373 2054 7261  ster Express Tra
+00000720: 6d00 1700 ff04 011f 01ff 5800 466f 7374  m.........X.Fost
+00000730: 6572 2053 6e65 6c74 7261 6d00 0900 ff03  er Sneltram.....
+00000740: 0101 ff58 0000 fe00 0000 0000 0000       ...X..........
```

### Comparing `nml-0.7.2/regression/expected/019_switch.nfo` & `nml-r1512/regression/expected/019_switch.nfo`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,55 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d13
-
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\19" "NML regression test" 00 "A test newgrf testing NML" 00
-3 * 51 04 00 FF 03 \wxD000 "\98coal" 00 "\98diamonds" 00 "\98Extra info for coal mine: \7B" 00
-
-// Name: return_switch
-4 * 38 02 0A FF 89
-24 60 \dxFFFFFFFF \dxFFFFF862 \dx00000001
-\2psto 1A 00 \dx00000001
-\b1
-\wx8000 \dx00000001 \dx00000000 	// Bogus range to avoid nvar == 0
-\wx8000 // default: return 0;
+0 * 4 \d8 
 
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
 // Name: coal_mine_subtype_switch
-// a : register 80
-5 * 48 02 0A FF 89
-7D 80 20 \dxFFFFFFFF 	// a
-\2psto 1A 20 \dx00000000
-\2r 02 00 \dx000000FF
-\b2
+3 * 37 02 0A FE 89 
+1A 20 \dx00000004 
+\2psto 1A 20 \dx00000000 
+\2r 02 00 \dx000000FF 
+\b1 
 \wx8000 \dx00000000 \dx0000000A 	// 0 .. 10: return string(STR_COALMINE_MONTH_0_10);
-\wx00FF \dx0000000D \dx0000000D 	// 13 .. 13: return_switch;
 \wx8001 // default: return string(STR_COALMINE_MONTH_11);
 
-6 * 11 00 0A \b2 01 FF \wx0000
-08 00
-09 00
-
-7 * 11 00 0A \b2 01 FF \wx0000
-21 40
-22 03
-
-// Name: @return_action_0
-8 * 30 02 0A FF 89
-1A 20 \dx00000004
-\2sto 1A 00 \dx00000080
-\b1
-\wx00FF \dx00000000 \dx00000000 	// coal_mine_subtype_switch
-\wx00FF // coal_mine_subtype_switch
-
-// Name: @return_action_1
-9 * 13 02 0A FE 89
-10 00 \dx00000001
-\b0
-\wx8000 // Return computed value
-
-// Name: @CB_FAILED_PROD
-10 * 15 02 0A FD 00 \wx0000 \wx0000 \wx0000 \wx0000 \wx0000 00
-
-// Name: @CB_FAILED0A
-11 * 23 02 0A FD 89
-0C 00 \dx0000FFFF
-\b1
-\wx8000 \dx00000000 \dx00000000 	// graphics callback -> return 0
-\wx00FD // Non-graphics callback, return graphics result
-
-// Name: @action3_0
-12 * 43 02 0A FD 89
-0C 00 \dx0000FFFF
-\b3
-\wx00FF \dx00000037 \dx00000037 	// @return_action_0;
-\wx8002 \dx0000003A \dx0000003A 	// return string(STR_COALMINE_EXTRA_TEXT);
-\wx00FE \dx0000003B \dx0000003B 	// return var[0x10, 0, 1]
-\wx00FD // @CB_FAILED0A;
+// Name: coal_mine_switch@return
+4 * 13 02 0A FD 89 
+1C 00 \dxFFFFFFFF 
+\b0 
+\wx0000 // Return computed value
+
+// Name: coal_mine_switch
+5 * 64 02 0A FD 89 
+1A 20 \dx00000004 
+\2sto 1A 20 \dx00000100 
+\2& 1A 20 \dx00000000 
+\2| 0C 00 \dx0000FFFF 
+\b3 
+\wx8002 \dx0000003A \dx0000003A 	// 58 .. 58: return string(STR_COALMINE_EXTRA_TEXT);
+\wx00FE \dx00000037 \dx00000037 	// 55 .. 55: coal_mine_subtype_switch;
+\wx00FD \dx0000FFFF \dx0000FFFF 	// 65535 .. 65535: coal_mine_switch@return;
+\wx0000 // default: CB_FAILED;
+
+6 * 13 00 0A \b4 01 00 
+08 00 
+09 00 
+21 00 
+22 01 
+
+7 * 7 03 0A 01 00 \b0 
+\wx00FD 
 
-13 * 7 03 0A 01 00 \b0
-\wx00FD 	// @action3_0;
+8 * 51 04 08 FF 03 \wxD000 "\98coal" 00 "\98diamonds" 00 "\98Extra info for coal mine: \7B" 00
```

### Comparing `nml-0.7.2/regression/expected/020_recolour.grf` & `nml-r1512/regression/expected/020_recolour.grf`

 * *Files 12% similar despite different names*

```diff
@@ -1,168 +1,158 @@
-00000000: 0000 4752 4682 0d0a 1a0a 2704 0000 0004  ..GRF.....'.....
-00000010: 0000 00ff 1300 0000 3600 0000 ff14 4349  ........6.....CI
-00000020: 4e46 4f42 5652 534e 0400 0000 0000 424d  NFOBVRSN......BM
-00000030: 494e 5604 0000 0000 0042 4e50 4152 0100  INV......BNPAR..
-00000040: 0042 5041 4c53 0100 5742 424c 5452 0100  .BPALS..WBBLTR..
-00000050: 3800 0034 0000 00ff 0808 4e4d 4c20 4e4d  8..4......NML NM
-00000060: 4c20 7265 6772 6573 7369 6f6e 2074 6573  L regression tes
-00000070: 7400 4120 7465 7374 206e 6577 6772 6620  t.A test newgrf 
-00000080: 7465 7374 696e 6720 4e4d 4c00 0900 0000  testing NML.....
-00000090: ff0d 0300 00fe ff08 0300 0700 0000 ff06  ................
-000000a0: 0302 ff03 00ff 0500 0000 ff0a 0103 0000  ................
-000000b0: 0101 0000 ff00 0000 0000 0000 0000 0000  ................
-000000c0: 0a0b 0c0d 0e0f 1011 1213 1415 1617 1819  ................
-000000d0: 1a1b 1c1d 1e1f 2021 2223 2425 2627 2829  ...... !"#$%&'()
-000000e0: 2a2b 2c2d 2e2f 3031 3233 3435 3637 3839  *+,-./0123456789
-000000f0: 3a3b 3c3d 3e3f 4041 4243 4445 4647 4849  :;<=>?@ABCDEFGHI
-00000100: 4a4b 4c4d 4e4f 5051 5253 5455 5657 5859  JKLMNOPQRSTUVWXY
-00000110: 5a5b 5c5d 5e5f 6061 6263 6465 6667 6869  Z[\]^_`abcdefghi
-00000120: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-00000130: 7a7b 7c7d 7e7f 8081 8283 8485 8687 8889  z{|}~...........
-00000140: 8a8b 8c8d 8e8f 9091 9293 9495 9697 9899  ................
-00000150: 9a9b 9c9d 9e9f a0a1 a2a3 a4a5 a6a7 a8a9  ................
-00000160: aaab acad aeaf b0b1 b2b3 b4b5 b6b7 b8b9  ................
-00000170: babb bcbd bebf c0c1 c2c3 c4c5 b2d9 0a0b  ................
-00000180: 0c0d 0e0f cecf d0d1 d2d3 d4d5 d6d7 d8d9  ................
-00000190: dadb dcdd dedf e0e1 e2e3 e4e5 e6e7 e8e9  ................
-000001a0: eaeb eced eeef f0f1 f2f3 f4f5 0000 0000  ................
-000001b0: 0000 0000 00ff 0101 0000 ff00 0000 0000  ................
-000001c0: 0000 0000 0000 0a0b 0c0d 0e0f 1011 1213  ................
-000001d0: 1415 1617 1819 1a1b 1c1d 1e1f 2021 2223  ............ !"#
-000001e0: 2425 2627 2829 2a2b 2c2d 2e2f 3031 3233  $%&'()*+,-./0123
-000001f0: 3435 3637 3839 3a3b 3c3d 3e3f 4041 4243  456789:;<=>?@ABC
-00000200: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
-00000210: 5455 5657 5859 5a5b 5c5d 5e5f 6061 6263  TUVWXYZ[\]^_`abc
-00000220: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00000230: 7475 7677 7879 7a7b 7c7d 7e7f 8081 8283  tuvwxyz{|}~.....
-00000240: 8485 8687 8889 8a8b 8c8d 8e8f 9091 9293  ................
-00000250: 9495 9697 9899 9a9b 9c9d 9e9f a0a1 a2a3  ................
-00000260: a4a5 a6a7 a8a9 aaab acad aeaf b0b1 b2b3  ................
-00000270: b4b5 b6b7 b8b9 babb bcbd bebf c0c1 c2c3  ................
-00000280: c4c5 3e3f 4041 4243 4445 cecf d0d1 d2d3  ..>?@ABCDE......
-00000290: d4d5 d6d7 d8d9 dadb dcdd dedf e0e1 e2e3  ................
-000002a0: e4e5 e6e7 e8e9 eaeb eced eeef f0f1 f2f3  ................
-000002b0: f4f5 0000 0000 0000 0000 00ff 0101 0000  ................
-000002c0: ff00 0000 0000 0000 0000 0000 0a0b 0c0d  ................
-000002d0: 0e0f 1011 1213 1415 1617 1819 1a1b 1c1d  ................
-000002e0: 1e1f 2021 2223 2425 2627 2829 2a2b 2c2d  .. !"#$%&'()*+,-
-000002f0: 2e2f 3031 3233 3435 3637 3839 3a3b 3c3d  ./0123456789:;<=
-00000300: 3e3f 4041 4243 4445 4647 4849 4a4b 4c4d  >?@ABCDEFGHIJKLM
-00000310: 4e4f 5051 5253 5455 5657 5859 5a5b 5c5d  NOPQRSTUVWXYZ[\]
-00000320: 5e5f 6061 6263 6465 6667 6869 6a6b 6c6d  ^_`abcdefghijklm
-00000330: 6e6f 7071 7273 7475 7677 7879 7a7b 7c7d  nopqrstuvwxyz{|}
-00000340: 7e7f 8081 8283 8485 8687 8889 8a8b 8c8d  ~...............
-00000350: 8e8f 9091 9293 9495 9697 9899 9a9b 9c9d  ................
-00000360: 9e9f a0a1 a2a3 a4a5 a6a7 a8a9 aaab acad  ................
-00000370: aeaf b0b1 b2b3 b4b5 b6b7 b8b9 babb bcbd  ................
-00000380: bebf c0c1 c2c3 c4c5 9a9b 9c9d 9e9f a0a1  ................
-00000390: cecf d0d1 d2d3 d4d5 d6d7 d8d9 dadb dcdd  ................
-000003a0: dedf e0e1 e2e3 e4e5 e6e7 e8e9 eaeb eced  ................
-000003b0: eeef f0f1 f2f3 f4f5 0000 0000 0000 0000  ................
-000003c0: 00ff 0600 0000 ff01 0101 ff08 0004 0000  ................
-000003d0: 00fd 0b00 0000 0400 0000 fd0c 0000 0004  ................
-000003e0: 0000 00fd 0d00 0000 0400 0000 fd0e 0000  ................
-000003f0: 0004 0000 00fd 0f00 0000 0400 0000 fd10  ................
-00000400: 0000 0004 0000 00fd 1100 0000 0400 0000  ................
-00000410: fd12 0000 0009 0000 00ff 0201 ff01 0100  ................
-00000420: 0000 0009 0000 00ff 0301 01ff 5800 00ff  ............X...
-00000430: 0000 0000 000b 0000 0077 0000 0004 0012  .........w......
-00000440: 0008 00fd fff6 ff12 00c9 caca cbcb cc00  ................
-00000450: c7c9 cac9 cacb cccb c7c9 e811 01cc e008  ................
-00000460: e810 03ca ccca d810 d818 c020 03ca cad8  ........... ....
-00000470: d020 03cb d8ca c808 d830 02cb ccc8 08d0  . .......0......
-00000480: 1004 c7c8 c9d8 e859 e807 02ca 6ae8 620f  .......Y....j.b.
-00000490: c883 81ca ca83 81cb c884 83ca ca84 83d8  ................
-000004a0: 4801 cae8 7b02 c7b5 e009 03b7 cb00 e029  H...{..........)
-000004b0: 03ca ca00 0c00 0000 c800 0000 0400 1000  ................
-000004c0: 1400 f2ff fbff 0300 0000 e803 d006 04c9  ................
-000004d0: cacc cba0 1008 0000 c7ca cacb cbcb a016  ................
-000004e0: 03c7 c9c9 e013 04cb cccc cca8 12e8 39e8  ..............9.
-000004f0: 11e0 1804 6ad8 d8d8 e803 d837 e812 05ca  ....j......7....
-00000500: cbca 8483 d036 e838 d812 01c9 e812 0385  .....6.8........
-00000510: 8400 d812 01ca a812 0483 cac7 c8e8 25a8  ..............%.
-00000520: 2408 caca caca c9c8 c8c7 9012 09c8 ca83  $...............
-00000530: 81c9 c8c7 cbca b824 0acb 8258 c884 83c9  .......$...X....
-00000540: c9c9 c7c0 360c cc82 5882 6a00 c7c8 c983  ....6...X.j.....
-00000550: 81c7 c812 02cb c9e8 1204 0000 b5c8 e82b  ...............+
-00000560: 01c8 d859 03cb c9c8 c8e6 05c8 c8c8 c9c8  ...Y............
-00000570: e8d8 e848 a8fc 03c8 b5c8 e85a d836 a016  ...H.......Z.6..
-00000580: d048 c138 0d00 0000 df00 0000 0400 0f00  .H.8............
-00000590: 1c00 f2ff f8ff 056a d800 0000 e803 d006  .......j........
-000005a0: a00c e018 01d8 881e 881e 883c a04a 07ca  ...........<.J..
-000005b0: c9d8 d8c9 c9c9 e803 d006 d00c e06c 05c9  .............l..
-000005c0: c9cb cbc9 d81e 03ca c9ca e803 04ca caca  ................
-000005d0: cbe8 0302 caca e835 04ca cbcb cce0 1403  .......5........
-000005e0: 5858 cbe8 0be0 1701 cce8 0705 cccb cccc  XX..............
-000005f0: cce8 05d8 0de0 0fd8 13d0 17e0 3fe0 43e0  ............?.C.
-00000600: 22e0 26c0 08a0 1001 cbd8 65d8 66d8 41d0  ".&.......e.f.A.
-00000610: 0607 cb80 80cb 8183 84e0 04c0 08c0 1007  ................
-00000620: 8081 8185 cb83 84e0 04c0 08b8 1003 8180  ................
-00000630: cae8 c103 cbca c888 54e0 9be8 cf01 b5d0  ........T.......
-00000640: 63d0 72d0 9dd0 c9e8 cf09 00cb cb82 5858  c.r...........XX
-00000650: 5858 d7c8 8702 cccc d00f 03cc cdcd e185  XX..............
-00000660: 0682 6a88 8882 6ab9 8fb0 0f0e 0000 00e9  ..j...j.........
-00000670: 0000 0004 0013 0014 00fa fff9 ff04 0000  ................
-00000680: 006a e804 e807 d006 c00c 01d8 8815 8815  .j..............
-00000690: b033 03cc d8cb 9040 07ca c9ca cbcb d8cc  .3.....@........
-000006a0: a016 03c9 c9ca e803 e815 b016 03c9 c9c9  ................
-000006b0: e016 04ca cacb ccb8 1602 8381 c016 01cb  ................
-000006c0: b816 0284 83e8 1601 c7e0 2c0c cbca cccb  ..........,.....
-000006d0: cccb ccca 0000 c7c9 a816 01cb e02c 05ca  .............,..
-000006e0: 00c8 c8c9 c016 01ca e855 e041 03cb cad7  .........U.A....
-000006f0: e815 d02c d815 07cc cc81 cbc7 58d7 e016  ...,........X...
-00000700: 01c8 d858 e854 09c7 8083 cb00 826a 58d7  ...X.T.......jX.
-00000710: e8a2 d042 e813 0281 84e8 66e8 1603 c7ca  ...B......f.....
-00000720: cbe8 2be8 6e05 cac7 8183 cae0 14e9 2f03  ..+.n........./.
-00000730: c6c8 cbe8 5804 c8c9 ca80 e8bd c814 0300  ....X...........
-00000740: 00c8 e858 d866 0134 c028 d842 0358 d7c8  ...X.f.4.(.B.X..
-00000750: e8b9 01ca 9923 0382 6ac8 d012 0f00 0000  .....#..j.......
-00000760: 7900 0000 0400 1200 0800 fdff f6ff 0400  y...............
-00000770: 0000 6ae8 040a 0000 c7c9 d8c9 cac9 00c7  ..j.............
-00000780: d808 0acb c9c7 c9ca d8ca cbcc cad8 0801  ................
-00000790: cae0 0802 c9ca e810 01cb e818 e81f d808  ................
-000007a0: e81e d810 d818 e031 02cb ccd0 08e8 3001  .......1......0.
-000007b0: cbd0 1708 cccb ca81 8181 8081 e849 e007  .............I..
-000007c0: 0583 84cc c980 e007 0184 d820 e83a e84d  ........... .:.M
-000007d0: 03ca 3434 e008 01c9 e061 02ca ca10 0000  ..44.....a......
-000007e0: 00de 0000 0004 0013 0014 00f2 fff7 ff03  ................
-000007f0: 0000 00e8 03d0 06e0 0c01 6a88 11e8 2001  ..........j... .
-00000800: d888 2488 13c0 2602 c9cb 904c 07c7 c9d8  ..$...&....L....
-00000810: caca cbcb a816 0ac7 c9c9 d8cb cccb cccc  ................
-00000820: ccc0 2be8 1202 caca d012 e819 c012 e835  ..+............5
-00000830: e024 0bca caca 8483 0000 c9ca ccca e814  .$..............
-00000840: d812 01c9 e812 0385 8400 d858 e847 b812  ...........X.G..
-00000850: 04cb cbc9 c9e8 6be0 5bb8 1206 cacb c980  ......k.[.......
-00000860: c9c9 e05a 02cb cbc8 1207 cacc ccc9 8080  ...Z............
-00000870: 80e8 2bd8 48e8 7c0b cacb 8258 c9c8 8080  ..+.H.|....X....
-00000880: 8181 c9b8 240d 8258 826a 00c8 c981 8383  ....$..X.j......
-00000890: c985 84e8 85e8 a101 c8e8 12e8 8a03 c8c9  ................
-000008a0: c9e8 3501 83e0 d702 c9c8 d13a 04c9 c943  ..5........:...C
-000008b0: c9e0 c5e8 48c8 12d0 16e8 d9d8 48a1 60e8  ....H.......H.`.
-000008c0: 2998 1211 0000 00de 0000 0004 000f 001c  )...............
-000008d0: 00f2 fff8 ff03 0000 00e8 03d0 06a0 0c04  ................
-000008e0: 0000 d86a 881c b01a 01d8 8836 881a 0500  ...j.......6....
-000008f0: 00c9 c9c9 e803 d006 d00c 04d8 d8c9 cad8  ................
-00000900: 6c03 caca cbe8 0305 caca caca c9e8 0301  l...............
-00000910: cad8 1a0b c9cb cbcb cb00 00cc cccb cce8  ................
-00000920: 0a01 cce0 2106 cbcb cacb 5858 e024 e013  ....!.....XX.$..
-00000930: 01ca e837 e80a d821 c025 e034 d806 e817  ...7...!.%.4....
-00000940: e81a d006 a00c d82f 0180 d828 d82d e054  ......./...(.-.T
-00000950: d07a 01ca d871 08cc 8181 8084 8381 cbe0  .z...q..........
-00000960: 04c0 08d0 1007 cb83 83ca 8081 85e8 09e0  ................
-00000970: 04c0 08b8 10e8 b988 54e0 cf01 c8e0 b5d8  ........T.......
-00000980: cad0 bfd8 69b0 6ee8 1c0a 00cd cdcc d758  ....i.n........X
-00000990: 5858 5882 e8ea d098 d00f e0fd e989 066a  XXX............j
-000009a0: 8288 886a 82b9 92b8 0f12 0000 00c8 0000  ...j............
-000009b0: 0004 0010 0014 00fa fff9 ff08 0000 0000  ................
-000009c0: cbca cbcb e008 e00c d008 e811 04cb cbcc  ................
-000009d0: cca0 1601 cad0 14a0 1603 cac9 cae8 16e8  ................
-000009e0: 05e8 2bc0 2c07 8381 c9c9 c9c9 c9e8 1be0  ..+.,...........
-000009f0: 4108 d8d8 d8d8 d86a 8483 e816 01c7 e016  A......j........
-00000a00: 02cb cae0 41e0 5802 c883 a816 d857 03cc  ....A.X......W..
-00000a10: 00c8 e83b a82c e055 03cc c8d7 e050 e042  ...;.,.U.....P.B
-00000a20: 01c8 e042 e0ab 05cb d758 d7c9 e82c 01c8  ...B.....X...,..
-00000a30: d858 e084 09ca 8381 0082 6a58 d7ca c02c  .X........jX...,
-00000a40: e811 03ca 8483 e8dc 0382 6ac7 e8a2 d858  ..........j....X
-00000a50: e811 e8c4 d0e8 03c7 c8cb d858 e03c 02ca  ...........X.<..
-00000a60: b5c0 fcd0 58d8 1401 c8b9 10e0 5803 cbca  ....X.......X...
-00000a70: b5a8 12d0 1601 c9d0 2400 0000 00         ........$....
+00000000: 0400 ff13 0000 002e 00ff 1443 494e 464f  ...........CINFO
+00000010: 4256 5253 4e04 0000 0000 0042 4d49 4e56  BVRSN......BMINV
+00000020: 0400 0000 0000 424e 5041 5201 0000 4250  ......BNPAR...BP
+00000030: 414c 5301 0057 0000 3400 ff08 0774 6573  ALS..W..4....tes
+00000040: 744e 4d4c 2072 6567 7265 7373 696f 6e20  tNML regression 
+00000050: 7465 7374 0041 2074 6573 7420 6e65 7767  test.A test newg
+00000060: 7266 2074 6573 7469 6e67 204e 4d4c 0009  rf testing NML..
+00000070: 00ff 0d03 0000 feff 0803 0007 00ff 0603  ................
+00000080: 02ff 0300 ff05 00ff 0a01 0300 0001 01ff  ................
+00000090: 0000 0000 0000 0000 0000 000a 0b0c 0d0e  ................
+000000a0: 0f10 1112 1314 1516 1718 191a 1b1c 1d1e  ................
+000000b0: 1f20 2122 2324 2526 2728 292a 2b2c 2d2e  . !"#$%&'()*+,-.
+000000c0: 2f30 3132 3334 3536 3738 393a 3b3c 3d3e  /0123456789:;<=>
+000000d0: 3f40 4142 4344 4546 4748 494a 4b4c 4d4e  ?@ABCDEFGHIJKLMN
+000000e0: 4f50 5152 5354 5556 5758 595a 5b5c 5d5e  OPQRSTUVWXYZ[\]^
+000000f0: 5f60 6162 6364 6566 6768 696a 6b6c 6d6e  _`abcdefghijklmn
+00000100: 6f70 7172 7374 7576 7778 797a 7b7c 7d7e  opqrstuvwxyz{|}~
+00000110: 7f80 8182 8384 8586 8788 898a 8b8c 8d8e  ................
+00000120: 8f90 9192 9394 9596 9798 999a 9b9c 9d9e  ................
+00000130: 9fa0 a1a2 a3a4 a5a6 a7a8 a9aa abac adae  ................
+00000140: afb0 b1b2 b3b4 b5b6 b7b8 b9ba bbbc bdbe  ................
+00000150: bfc0 c1c2 c3c4 c5b2 d90a 0b0c 0d0e 0fce  ................
+00000160: cfd0 d1d2 d3d4 d5d6 d7d8 d9da dbdc ddde  ................
+00000170: dfe0 e1e2 e3e4 e5e6 e7e8 e9ea ebec edee  ................
+00000180: eff0 f1f2 f3f4 f500 0000 0000 0000 0000  ................
+00000190: ff01 01ff 0000 0000 0000 0000 0000 000a  ................
+000001a0: 0b0c 0d0e 0f10 1112 1314 1516 1718 191a  ................
+000001b0: 1b1c 1d1e 1f20 2122 2324 2526 2728 292a  ..... !"#$%&'()*
+000001c0: 2b2c 2d2e 2f30 3132 3334 3536 3738 393a  +,-./0123456789:
+000001d0: 3b3c 3d3e 3f40 4142 4344 4546 4748 494a  ;<=>?@ABCDEFGHIJ
+000001e0: 4b4c 4d4e 4f50 5152 5354 5556 5758 595a  KLMNOPQRSTUVWXYZ
+000001f0: 5b5c 5d5e 5f60 6162 6364 6566 6768 696a  [\]^_`abcdefghij
+00000200: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
+00000210: 7b7c 7d7e 7f80 8182 8384 8586 8788 898a  {|}~............
+00000220: 8b8c 8d8e 8f90 9192 9394 9596 9798 999a  ................
+00000230: 9b9c 9d9e 9fa0 a1a2 a3a4 a5a6 a7a8 a9aa  ................
+00000240: abac adae afb0 b1b2 b3b4 b5b6 b7b8 b9ba  ................
+00000250: bbbc bdbe bfc0 c1c2 c3c4 c53e 3f40 4142  ...........>?@AB
+00000260: 4344 45ce cfd0 d1d2 d3d4 d5d6 d7d8 d9da  CDE.............
+00000270: dbdc ddde dfe0 e1e2 e3e4 e5e6 e7e8 e9ea  ................
+00000280: ebec edee eff0 f1f2 f3f4 f500 0000 0000  ................
+00000290: 0000 0000 ff01 01ff 0000 0000 0000 0000  ................
+000002a0: 0000 000a 0b0c 0d0e 0f10 1112 1314 1516  ................
+000002b0: 1718 191a 1b1c 1d1e 1f20 2122 2324 2526  ......... !"#$%&
+000002c0: 2728 292a 2b2c 2d2e 2f30 3132 3334 3536  '()*+,-./0123456
+000002d0: 3738 393a 3b3c 3d3e 3f40 4142 4344 4546  789:;<=>?@ABCDEF
+000002e0: 4748 494a 4b4c 4d4e 4f50 5152 5354 5556  GHIJKLMNOPQRSTUV
+000002f0: 5758 595a 5b5c 5d5e 5f60 6162 6364 6566  WXYZ[\]^_`abcdef
+00000300: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
+00000310: 7778 797a 7b7c 7d7e 7f80 8182 8384 8586  wxyz{|}~........
+00000320: 8788 898a 8b8c 8d8e 8f90 9192 9394 9596  ................
+00000330: 9798 999a 9b9c 9d9e 9fa0 a1a2 a3a4 a5a6  ................
+00000340: a7a8 a9aa abac adae afb0 b1b2 b3b4 b5b6  ................
+00000350: b7b8 b9ba bbbc bdbe bfc0 c1c2 c3c4 c59a  ................
+00000360: 9b9c 9d9e 9fa0 a1ce cfd0 d1d2 d3d4 d5d6  ................
+00000370: d7d8 d9da dbdc ddde dfe0 e1e2 e3e4 e5e6  ................
+00000380: e7e8 e9ea ebec edee eff0 f1f2 f3f4 f500  ................
+00000390: 0000 0000 0000 0000 ff06 00ff 0101 01ff  ................
+000003a0: 0800 9800 0112 0800 fdff f6ff 1200 c9ca  ................
+000003b0: cacb cbcc 00c7 c9ca c9ca cbcc cbc7 c9e8  ................
+000003c0: 1101 cce0 08e8 1003 cacc cad8 10d8 18c0  ................
+000003d0: 2003 caca d8d0 2003 cbd8 cac8 08d8 3002   ..... .......0.
+000003e0: cbcc c808 d010 04c7 c8c9 d8e8 59e8 0702  ............Y...
+000003f0: ca6a e862 0fc8 8381 caca 8381 cbc8 8483  .j.b............
+00000400: caca 8483 d848 01ca e87b 02c7 b5e0 0903  .....H...{......
+00000410: b7cb 00e0 2903 caca 0084 0101 1314 00f2  ....)...........
+00000420: fffb ff03 0000 00e8 03d0 0604 c9ca cccb  ................
+00000430: a010 0800 00c7 caca cbcb cba0 1603 c7c9  ................
+00000440: c9e0 1304 cbcc cccc a812 e839 e811 e018  ...........9....
+00000450: 046a d8d8 d8e8 03d8 37e8 1205 cacb ca84  .j......7.......
+00000460: 83d0 36e8 38d8 1201 c9e8 1203 8584 00d8  ..6.8...........
+00000470: 1201 caa8 1204 83ca c7c8 e825 a824 08ca  ...........%.$..
+00000480: caca cac9 c8c8 c790 1209 c8ca 8381 c9c8  ................
+00000490: c7cb cab8 240a cb82 58c8 8483 c9c9 c9c7  ....$...X.......
+000004a0: c036 0ccc 8258 826a 00c7 c8c9 8381 c7c8  .6...X.j........
+000004b0: 1202 cbc9 e812 0400 00b5 c8e8 2b01 c8d8  ............+...
+000004c0: 5903 cbc9 c8c8 e605 c8c8 c8c9 c8e8 d8e8  Y...............
+000004d0: 48a8 fc03 c8b5 c8e8 5ad8 36a0 16d0 4891  H.......Z.6...H.
+000004e0: 2888 1188 2088 2fb9 73ac 0101 0f1c 00f2  (... ./.s.......
+000004f0: fff8 ff05 6ad8 0000 00e8 03d0 06a0 0ce0  ....j...........
+00000500: 1801 d888 1e88 1e88 3ca0 4a07 cac9 d8d8  ........<.J.....
+00000510: c9c9 c9e8 03d0 06d0 0ce0 6c05 c9c9 cbcb  ..........l.....
+00000520: c9d8 1e03 cac9 cae8 0304 caca cacb e803  ................
+00000530: 02ca cae8 3504 cacb cbcc e014 0358 58cb  ....5........XX.
+00000540: e80b e017 01cc e807 05cc cbcc cccc e805  ................
+00000550: d80d e00f d813 d017 e03f e043 e022 e026  .........?.C.".&
+00000560: c008 a010 01cb d865 d866 d841 d006 07cb  .......e.f.A....
+00000570: 8080 cb81 8384 e004 c008 c010 0780 8181  ................
+00000580: 85cb 8384 e004 c008 b810 0381 80ca e8c1  ................
+00000590: 03cb cac8 8854 e09b e8cf 01b5 d063 d072  .....T.......c.r
+000005a0: d09d d0c9 e8cf 0900 cbcb 8258 5858 58d7  ...........XXXX.
+000005b0: c887 02cc ccd0 0f03 cccd cde1 8506 826a  ...............j
+000005c0: 8888 826a b98f b00f 8401 0113 1400 faff  ...j............
+000005d0: f9ff 0400 0000 6ae8 04e8 07d0 06c0 0c01  ......j.........
+000005e0: d888 1588 15b0 3303 ccd8 cb90 4007 cac9  ......3.....@...
+000005f0: cacb cbd8 cca0 1603 c9c9 cae8 03e8 15b0  ................
+00000600: 1603 c9c9 c9e0 1604 caca cbcc b816 0283  ................
+00000610: 81c0 1601 cbb8 1602 8483 e816 01c7 e02c  ...............,
+00000620: 0ccb cacc cbcc cbcc ca00 00c7 c9a8 1601  ................
+00000630: cbe0 2c05 ca00 c8c8 c9c0 1601 cae8 55e0  ..,...........U.
+00000640: 4103 cbca d7e8 15d0 2cd8 1507 cccc 81cb  A.......,.......
+00000650: c758 d7e0 1601 c8d8 58e8 5409 c780 83cb  .X......X.T.....
+00000660: 0082 6a58 d7e8 a2d0 42e8 1302 8184 e866  ..jX....B......f
+00000670: e816 03c7 cacb e82b e86e 05ca c781 83ca  .......+.n......
+00000680: e014 e92f 03c6 c8cb e858 04c8 c9ca 80e8  .../.....X......
+00000690: bdc8 1403 0000 c8e8 58d8 6601 34c0 28d8  ........X.f.4.(.
+000006a0: 4203 58d7 c8e8 b901 ca99 2303 826a c8d0  B.X.......#..j..
+000006b0: 1298 0001 1208 00fd fff6 ff04 0000 006a  ...............j
+000006c0: e804 0a00 00c7 c9d8 c9ca c900 c7d8 080a  ................
+000006d0: cbc9 c7c9 cad8 cacb ccca d808 01ca e008  ................
+000006e0: 02c9 cae8 1001 cbe8 18e8 1fd8 08e8 1ed8  ................
+000006f0: 10d8 18e0 3102 cbcc d008 e830 01cb d017  ....1......0....
+00000700: 08cc cbca 8181 8180 81e8 49e0 0705 8384  ..........I.....
+00000710: ccc9 80e0 0701 84d8 20e8 3ae8 4d03 ca34  ........ .:.M..4
+00000720: 34e0 0801 c9e0 6102 caca 8401 0113 1400  4.....a.........
+00000730: f2ff f7ff 0300 0000 e803 d006 e00c 016a  ...............j
+00000740: 8811 e820 01d8 8824 8813 c026 02c9 cb90  ... ...$...&....
+00000750: 4c07 c7c9 d8ca cacb cba8 160a c7c9 c9d8  L...............
+00000760: cbcc cbcc cccc c02b e812 02ca cad0 12e8  .......+........
+00000770: 19c0 12e8 35e0 240b caca ca84 8300 00c9  ....5.$.........
+00000780: cacc cae8 14d8 1201 c9e8 1203 8584 00d8  ................
+00000790: 58e8 47b8 1204 cbcb c9c9 e86b e05b b812  X.G........k.[..
+000007a0: 06ca cbc9 80c9 c9e0 5a02 cbcb c812 07ca  ........Z.......
+000007b0: cccc c980 8080 e82b d848 e87c 0bca cb82  .......+.H.|....
+000007c0: 58c9 c880 8081 81c9 b824 0d82 5882 6a00  X........$..X.j.
+000007d0: c8c9 8183 83c9 8584 e885 e8a1 01c8 e812  ................
+000007e0: e88a 03c8 c9c9 e835 0183 e0d7 02c9 c8d1  .......5........
+000007f0: 3a04 c9c9 43c9 e0c5 e848 c812 d016 e8d9  :...C....H......
+00000800: d848 a160 e829 9812 ac01 010f 1c00 f2ff  .H.`.)..........
+00000810: f8ff 0300 0000 e803 d006 a00c 0400 00d8  ................
+00000820: 6a88 1cb0 1a01 d888 3688 1a05 0000 c9c9  j.......6.......
+00000830: c9e8 03d0 06d0 0c04 d8d8 c9ca d86c 03ca  .............l..
+00000840: cacb e803 05ca caca cac9 e803 01ca d81a  ................
+00000850: 0bc9 cbcb cbcb 0000 cccc cbcc e80a 01cc  ................
+00000860: e021 06cb cbca cb58 58e0 24e0 1301 cae8  .!.....XX.$.....
+00000870: 37e8 0ad8 21c0 25e0 34d8 06e8 17e8 1ad0  7...!.%.4.......
+00000880: 06a0 0cd8 2f01 80d8 28d8 2de0 54d0 7a01  ..../...(.-.T.z.
+00000890: cad8 7108 cc81 8180 8483 81cb e004 c008  ..q.............
+000008a0: d010 07cb 8383 ca80 8185 e809 e004 c008  ................
+000008b0: b810 e8b9 8854 e0cf 01c8 e0b5 d8ca d0bf  .....T..........
+000008c0: d869 b06e e81c 0a00 cdcd ccd7 5858 5858  .i.n........XXXX
+000008d0: 82e8 ead0 98d0 0fe0 fde9 8906 6a82 8888  ............j...
+000008e0: 6a82 b992 b80f 8401 0113 1400 faff f9ff  j...............
+000008f0: 0800 0000 00cb cacb cbe0 08e0 0cd0 08e8  ................
+00000900: 1104 cbcb cccc a016 01ca d014 a016 03ca  ................
+00000910: c9ca e816 e805 e82b c02c 0783 81c9 c9c9  .......+.,......
+00000920: c9c9 e81b e041 08d8 d8d8 d8d8 6a84 83e8  .....A......j...
+00000930: 1601 c7e0 1602 cbca e041 e058 02c8 83a8  .........A.X....
+00000940: 16d8 5703 cc00 c8e8 3ba8 2ce0 5503 ccc8  ..W.....;.,.U...
+00000950: d7e0 50e0 4201 c8e0 42e0 ab05 cbd7 58d7  ..P.B...B.....X.
+00000960: c9e8 2c01 c8d8 58e0 8409 ca83 8100 826a  ..,...X........j
+00000970: 58d7 cac0 2ce8 1103 ca84 83e8 dc03 826a  X...,..........j
+00000980: c7e8 a2d8 58e8 11e8 c4d0 e803 c7c8 cbd8  ....X...........
+00000990: 58e0 3c02 cab5 c0fc d058 d814 01c8 b910  X.<......X......
+000009a0: e058 03cb cab5 a812 d016 01c9 8812 9141  .X.............A
+000009b0: 881b 882a c96d 0900 ff02 01fe 0101 0000  ...*.m..........
+000009c0: 0000 0900 ff03 0101 ff58 0000 fe00 0000  .........X......
+000009d0: 0000 0000                                ....
```

### Comparing `nml-0.7.2/regression/expected/020_recolour.nfo` & `nml-r1512/regression/expected/020_recolour.nfo`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d19
+0 * 4 \d19 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "W"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\20" "NML regression test" 00 "A test newgrf testing NML" 00
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "W" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
 // param[3] = param[\DR]
-3 * 9 0D 03 \D= \DR FE \dx000308FF
+3 * 9 0D 03 \D= \DR FE \dx000308FF 
 
-4 * 7 06
-03 02 FF \wx0003
-FF
-
-5 * 5 0A \b1 \b3 \w0
-
-6 * 257 00
-00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F
-10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F
-20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F
-30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F
-40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F
-50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F
-60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F
-70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F
-80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F
-90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F
-A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF
-B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF
-C0 C1 C2 C3 C4 C5 B2 D9 0A 0B 0C 0D 0E 0F CE CF
-D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF
-E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF
-F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF
-7 * 257 00
-00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F
-10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F
-20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F
-30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F
-40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F
-50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F
-60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F
-70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F
-80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F
-90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F
-A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF
-B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF
-C0 C1 C2 C3 C4 C5 3E 3F 40 41 42 43 44 45 CE CF
-D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF
-E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF
-F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF
-8 * 257 00
-00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F
-10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F
-20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F
-30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F
-40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F
-50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F
-60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F
-70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F
-80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F
-90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F
-A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF
-B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF
-C0 C1 C2 C3 C4 C5 9A 9B 9C 9D 9E 9F A0 A1 CE CF
-D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF
-E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF
-F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF
-
-9 * 6 01 01 \b1 FF \wx0008
-
-10 opengfx_generic_trams1.pcx 8bpp 48 56 8 18 -3 -10 normal
-11 opengfx_generic_trams1.pcx 8bpp 64 56 20 19 -14 -5 normal
-12 opengfx_generic_trams1.pcx 8bpp 96 56 28 15 -14 -8 normal
-13 opengfx_generic_trams1.pcx 8bpp 144 56 20 19 -6 -7 normal
-14 opengfx_generic_trams1.pcx 8bpp 176 56 8 18 -3 -10 normal
-15 opengfx_generic_trams1.pcx 8bpp 192 56 20 19 -14 -9 normal
-16 opengfx_generic_trams1.pcx 8bpp 224 56 28 15 -14 -8 normal
-17 opengfx_generic_trams1.pcx 8bpp 272 56 20 19 -6 -7 normal
-
-// Name: foster_express_group - feature 01
-18 * 9 02 01 FF \b1 \b1
-\w0
-\w0
+4 * 7 06 
+03 02 FF \wx0003 
+FF 
+
+5 * 5 0A \b1 \b3 \w0 
+
+6 * 257 00 
+00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F 
+10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F 
+20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F 
+30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F 
+40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F 
+50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F 
+60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F 
+70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F 
+80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F 
+90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F 
+A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF 
+B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF 
+C0 C1 C2 C3 C4 C5 B2 D9 0A 0B 0C 0D 0E 0F CE CF 
+D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF 
+E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF 
+F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF 
+7 * 257 00 
+00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F 
+10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F 
+20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F 
+30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F 
+40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F 
+50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F 
+60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F 
+70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F 
+80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F 
+90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F 
+A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF 
+B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF 
+C0 C1 C2 C3 C4 C5 3E 3F 40 41 42 43 44 45 CE CF 
+D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF 
+E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF 
+F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF 
+8 * 257 00 
+00 00 00 00 00 00 00 00 00 00 0A 0B 0C 0D 0E 0F 
+10 11 12 13 14 15 16 17 18 19 1A 1B 1C 1D 1E 1F 
+20 21 22 23 24 25 26 27 28 29 2A 2B 2C 2D 2E 2F 
+30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E 3F 
+40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E 4F 
+50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D 5E 5F 
+60 61 62 63 64 65 66 67 68 69 6A 6B 6C 6D 6E 6F 
+70 71 72 73 74 75 76 77 78 79 7A 7B 7C 7D 7E 7F 
+80 81 82 83 84 85 86 87 88 89 8A 8B 8C 8D 8E 8F 
+90 91 92 93 94 95 96 97 98 99 9A 9B 9C 9D 9E 9F 
+A0 A1 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AF 
+B0 B1 B2 B3 B4 B5 B6 B7 B8 B9 BA BB BC BD BE BF 
+C0 C1 C2 C3 C4 C5 9A 9B 9C 9D 9E 9F A0 A1 CE CF 
+D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 DA DB DC DD DE DF 
+E0 E1 E2 E3 E4 E5 E6 E7 E8 E9 EA EB EC ED EE EF 
+F0 F1 F2 F3 F4 F5 00 00 00 00 00 00 00 00 00 FF 
+
+9 * 6 01 01 \b1 FF \wx0008 
+
+10 opengfx_generic_trams1.pcx 48 56 01 18 8 -3 -10 
+11 opengfx_generic_trams1.pcx 64 56 01 19 20 -14 -5 
+12 opengfx_generic_trams1.pcx 96 56 01 15 28 -14 -8 
+13 opengfx_generic_trams1.pcx 144 56 01 19 20 -6 -7 
+14 opengfx_generic_trams1.pcx 176 56 01 18 8 -3 -10 
+15 opengfx_generic_trams1.pcx 192 56 01 19 20 -14 -9 
+16 opengfx_generic_trams1.pcx 224 56 01 15 28 -14 -8 
+17 opengfx_generic_trams1.pcx 272 56 01 19 20 -6 -7 
+
+// Name: foster_express_group
+18 * 9 02 01 FE \b1 \b1 
+\w0 
+\w0 
 
-19 * 9 03 01 01 FF \wx0058 \b0
-\wx00FF 	// foster_express_group;
+19 * 9 03 01 01 FF \wx0058 \b0 
+\wx00FE
```

### Comparing `nml-0.7.2/regression/expected/021_grf_parameter.grf` & `nml-r1512/regression/expected/021_grf_parameter.grf`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-00000000: 0000 4752 4682 0d0a 1a0a 8703 0000 0004  ..GRF...........
-00000010: 0000 00ff 0300 0000 3103 0000 ff14 4349  ........1.....CI
-00000020: 4e46 4f42 5652 534e 0400 0100 0000 424d  NFOBVRSN......BM
-00000030: 494e 5604 0000 0000 0042 4e50 4152 0100  INV......BNPAR..
-00000040: 0343 5041 5241 4300 0000 0054 4e41 4d45  .CPARAC....TNAME
-00000050: 7f44 6973 6162 6c65 2067 7269 646c 696e  .Disable gridlin
-00000060: 6573 0054 4445 5343 7f54 6869 7320 7365  es.TDESC.This se
-00000070: 7474 696e 6720 616c 6c6f 7773 2074 6f20  tting allows to 
-00000080: 7265 706c 6163 6520 616c 6c20 6772 6f75  replace all grou
-00000090: 6e64 2073 7072 6974 6573 2073 7563 6820  nd sprites such 
-000000a0: 7468 6174 2074 6865 206c 616e 6473 6361  that the landsca
-000000b0: 7065 2069 7320 7061 696e 7465 6420 286d  pe is painted (m
-000000c0: 6f73 746c 7929 2077 6974 686f 7574 2067  ostly) without g
-000000d0: 7269 6420 6c69 6e65 732e 204e 6f74 6520  rid lines. Note 
-000000e0: 7468 6174 2072 6f61 6473 2061 6e64 2074  that roads and t
-000000f0: 7261 696e 2074 7261 636b 7320 646f 6e27  rain tracks don'
-00000100: 7420 7965 7420 666f 6c6c 6f77 2074 6869  t yet follow thi
-00000110: 7320 7275 6c65 0042 5459 5045 0100 0142  s rule.BTYPE...B
-00000120: 4d41 534b 0300 0000 0142 4446 4c54 0400  MASK.....BDFLT..
-00000130: 0100 0000 0043 0100 0000 544e 414d 457f  .....C....TNAME.
-00000140: 5265 706c 6163 6520 7468 6520 7472 616e  Replace the tran
-00000150: 736d 6974 7465 7220 746f 7765 7220 6279  smitter tower by
-00000160: 2061 2072 6f63 6b00 5444 4553 437f 456e   a rock.TDESC.En
-00000170: 6162 6c65 2074 6f20 7265 706c 6163 6520  able to replace 
-00000180: 7468 6520 7472 616e 736d 6974 7465 7220  the transmitter 
-00000190: 746f 7765 7220 6279 2061 2072 6f63 6b20  tower by a rock 
-000001a0: 2875 7365 6675 6c20 666f 7220 6561 726c  (useful for earl
-000001b0: 7920 7363 656e 6172 696f 7320 7769 7468  y scenarios with
-000001c0: 6f75 7420 7465 6c65 636f 6d75 6e69 6361  out telecomunica
-000001d0: 7469 6f6e 2074 6f77 6572 7329 0042 5459  tion towers).BTY
-000001e0: 5045 0100 0142 4d41 534b 0300 0001 0142  PE...BMASK.....B
-000001f0: 4446 4c54 0400 0000 0000 0043 0200 0000  DFLT.......C....
-00000200: 544e 414d 457f 4c61 6e64 7363 6170 6520  TNAME.Landscape 
-00000210: 7479 7065 0054 4445 5343 7f53 656c 6563  type.TDESC.Selec
-00000220: 7420 7468 6520 6c61 6e64 7363 6170 6520  t the landscape 
-00000230: 2867 726f 756e 6420 7469 6c65 2920 7479  (ground tile) ty
-00000240: 7065 0042 4d41 534b 0100 0142 4c49 4d49  pe.BMASK...BLIMI
-00000250: 0800 0000 0000 0100 0000 4356 414c 5554  ..........CVALUT
-00000260: 0000 0000 7f6e 6f72 6d61 6c20 2861 6363  .....normal (acc
-00000270: 6f72 6469 6e67 2074 6f20 636c 696d 6174  ording to climat
-00000280: 6529 0054 0100 0000 7f61 6c70 696e 6520  e).T.....alpine 
-00000290: 2874 656d 7065 7261 7465 2067 7261 7373  (temperate grass
-000002a0: 2069 6e20 6172 6374 6963 2900 5402 0000   in arctic).T...
-000002b0: 007f 7465 6d70 6572 6174 6520 286e 6f74  ..temperate (not
-000002c0: 2069 6d70 6c65 6d65 6e74 6564 2900 5403   implemented).T.
-000002d0: 0000 007f 6172 6374 6963 2028 6e6f 7420  ....arctic (not 
-000002e0: 696d 706c 656d 656e 7465 6429 0054 0400  implemented).T..
-000002f0: 0000 7f74 726f 7069 6361 6c20 286e 6f74  ...tropical (not
-00000300: 2069 6d70 6c65 6d65 6e74 6564 2900 5405   implemented).T.
-00000310: 0000 007f 746f 796c 616e 6420 286e 6f74  ....toyland (not
-00000320: 2069 6d70 6c65 6d65 6e74 6564 2900 0042   implemented)..B
-00000330: 4446 4c54 0400 0000 0000 0000 4250 414c  DFLT........BPAL
-00000340: 5301 0041 4242 4c54 5201 0038 0000 3400  S..ABBLTR..8..4.
-00000350: 0000 ff08 084e 4d4c 214e 4d4c 2072 6567  .....NML!NML reg
-00000360: 7265 7373 696f 6e20 7465 7374 0041 2074  ression test.A t
-00000370: 6573 7420 6e65 7767 7266 2074 6573 7469  est newgrf testi
-00000380: 6e67 204e 4d4c 0005 0000 00ff 0d0a 0001  ng NML..........
-00000390: 0000 0000 0000 0000 00                   .........
+00000000: 0400 ff03 0000 0029 03ff 1443 494e 464f  .......)...CINFO
+00000010: 4256 5253 4e04 0001 0000 0042 4d49 4e56  BVRSN......BMINV
+00000020: 0400 0000 0000 424e 5041 5201 0003 4350  ......BNPAR...CP
+00000030: 4152 4143 0000 0000 544e 414d 457f 4469  ARAC....TNAME.Di
+00000040: 7361 626c 6520 6772 6964 6c69 6e65 7300  sable gridlines.
+00000050: 5444 4553 437f 5468 6973 2073 6574 7469  TDESC.This setti
+00000060: 6e67 2061 6c6c 6f77 7320 746f 2072 6570  ng allows to rep
+00000070: 6c61 6365 2061 6c6c 2067 726f 756e 6420  lace all ground 
+00000080: 7370 7269 7465 7320 7375 6368 2074 6861  sprites such tha
+00000090: 7420 7468 6520 6c61 6e64 7363 6170 6520  t the landscape 
+000000a0: 6973 2070 6169 6e74 6564 2028 6d6f 7374  is painted (most
+000000b0: 6c79 2920 7769 7468 6f75 7420 6772 6964  ly) without grid
+000000c0: 206c 696e 6573 2e20 4e6f 7465 2074 6861   lines. Note tha
+000000d0: 7420 726f 6164 7320 616e 6420 7472 6169  t roads and trai
+000000e0: 6e20 7472 6163 6b73 2064 6f6e 2774 2079  n tracks don't y
+000000f0: 6574 2066 6f6c 6c6f 7720 7468 6973 2072  et follow this r
+00000100: 756c 6500 4254 5950 4501 0001 424d 4153  ule.BTYPE...BMAS
+00000110: 4b03 0000 0001 4244 464c 5404 0001 0000  K.....BDFLT.....
+00000120: 0000 4301 0000 0054 4e41 4d45 7f52 6570  ..C....TNAME.Rep
+00000130: 6c61 6365 2074 6865 2074 7261 6e73 6d69  lace the transmi
+00000140: 7474 6572 2074 6f77 6572 2062 7920 6120  tter tower by a 
+00000150: 726f 636b 0054 4445 5343 7f45 6e61 626c  rock.TDESC.Enabl
+00000160: 6520 746f 2072 6570 6c61 6365 2074 6865  e to replace the
+00000170: 2074 7261 6e73 6d69 7474 6572 2074 6f77   transmitter tow
+00000180: 6572 2062 7920 6120 726f 636b 2028 7573  er by a rock (us
+00000190: 6566 756c 2066 6f72 2065 6172 6c79 2073  eful for early s
+000001a0: 6365 6e61 7269 6f73 2077 6974 686f 7574  cenarios without
+000001b0: 2074 656c 6563 6f6d 756e 6963 6174 696f   telecomunicatio
+000001c0: 6e20 746f 7765 7273 2900 4254 5950 4501  n towers).BTYPE.
+000001d0: 0001 424d 4153 4b03 0000 0101 4244 464c  ..BMASK.....BDFL
+000001e0: 5404 0000 0000 0000 4302 0000 0054 4e41  T.......C....TNA
+000001f0: 4d45 7f4c 616e 6473 6361 7065 2074 7970  ME.Landscape typ
+00000200: 6500 5444 4553 437f 5365 6c65 6374 2074  e.TDESC.Select t
+00000210: 6865 206c 616e 6473 6361 7065 2028 6772  he landscape (gr
+00000220: 6f75 6e64 2074 696c 6529 2074 7970 6500  ound tile) type.
+00000230: 424d 4153 4b01 0001 424c 494d 4908 0000  BMASK...BLIMI...
+00000240: 0000 0001 0000 0043 5641 4c55 5400 0000  .......CVALUT...
+00000250: 007f 6e6f 726d 616c 2028 6163 636f 7264  ..normal (accord
+00000260: 696e 6720 746f 2063 6c69 6d61 7465 2900  ing to climate).
+00000270: 5401 0000 007f 616c 7069 6e65 2028 7465  T.....alpine (te
+00000280: 6d70 6572 6174 6520 6772 6173 7320 696e  mperate grass in
+00000290: 2061 7263 7469 6329 0054 0200 0000 7f74   arctic).T.....t
+000002a0: 656d 7065 7261 7465 2028 6e6f 7420 696d  emperate (not im
+000002b0: 706c 656d 656e 7465 6429 0054 0300 0000  plemented).T....
+000002c0: 7f61 7263 7469 6320 286e 6f74 2069 6d70  .arctic (not imp
+000002d0: 6c65 6d65 6e74 6564 2900 5404 0000 007f  lemented).T.....
+000002e0: 7472 6f70 6963 616c 2028 6e6f 7420 696d  tropical (not im
+000002f0: 706c 656d 656e 7465 6429 0054 0500 0000  plemented).T....
+00000300: 7f74 6f79 6c61 6e64 2028 6e6f 7420 696d  .toyland (not im
+00000310: 706c 656d 656e 7465 6429 0000 4244 464c  plemented)..BDFL
+00000320: 5404 0000 0000 0000 0042 5041 4c53 0100  T........BPALS..
+00000330: 4100 0034 00ff 0807 7465 7374 4e4d 4c20  A..4....testNML 
+00000340: 7265 6772 6573 7369 6f6e 2074 6573 7400  regression test.
+00000350: 4120 7465 7374 206e 6577 6772 6620 7465  A test newgrf te
+00000360: 7374 696e 6720 4e4d 4c00 0500 ff0d 0a00  sting NML.......
+00000370: 0100 0000 0000 0000                      ........
```

### Comparing `nml-0.7.2/regression/expected/021_grf_parameter.nfo` & `nml-r1512/regression/expected/021_grf_parameter.nfo`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d3
+0 * 4 \d3 
 
-1 * 817 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000001
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 03
-"C" "PARA"
-"C" \d0
-"T" "NAME" 7F "Disable gridlines" 00
-"T" "DESC" 7F "This setting allows to replace all ground sprites such that the landscape is painted (mostly) without grid lines. Note that roads and train tracks don't yet follow this rule" 00
-"B" "TYPE" \w1 01
-"B" "MASK" \w3 \b0 \b0 \b1
-"B" "DFLT" \w4 \dx00000001
-00
-"C" \d1
-"T" "NAME" 7F "Replace the transmitter tower by a rock" 00
-"T" "DESC" 7F "Enable to replace the transmitter tower by a rock (useful for early scenarios without telecomunication towers)" 00
-"B" "TYPE" \w1 01
-"B" "MASK" \w3 \b0 \b1 \b1
-"B" "DFLT" \w4 \dx00000000
-00
-"C" \d2
-"T" "NAME" 7F "Landscape type" 00
-"T" "DESC" 7F "Select the landscape (ground tile) type" 00
-"B" "MASK" \w1 01
-"B" "LIMI" \w8 \d0 \d1
-"C" "VALU"
-"T" \d0 7F "normal (according to climate)" 00
-"T" \d1 7F "alpine (temperate grass in arctic)" 00
-"T" \d2 7F "temperate (not implemented)" 00
-"T" \d3 7F "arctic (not implemented)" 00
-"T" \d4 7F "tropical (not implemented)" 00
-"T" \d5 7F "toyland (not implemented)" 00
-00
-"B" "DFLT" \w4 \dx00000000
-00
-00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\21" "NML regression test" 00 "A test newgrf testing NML" 00
+1 * 809 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000001 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 03 
+"C" "PARA" 
+"C" \d0 
+"T" "NAME" 7F "Disable gridlines" 00 
+"T" "DESC" 7F "This setting allows to replace all ground sprites such that the landscape is painted (mostly) without grid lines. Note that roads and train tracks don't yet follow this rule" 00 
+"B" "TYPE" \w1 01 
+"B" "MASK" \w3 \b0 \b0 \b1 
+"B" "DFLT" \w4 \dx00000001 
+00 
+"C" \d1 
+"T" "NAME" 7F "Replace the transmitter tower by a rock" 00 
+"T" "DESC" 7F "Enable to replace the transmitter tower by a rock (useful for early scenarios without telecomunication towers)" 00 
+"B" "TYPE" \w1 01 
+"B" "MASK" \w3 \b0 \b1 \b1 
+"B" "DFLT" \w4 \dx00000000 
+00 
+"C" \d2 
+"T" "NAME" 7F "Landscape type" 00 
+"T" "DESC" 7F "Select the landscape (ground tile) type" 00 
+"B" "MASK" \w1 01 
+"B" "LIMI" \w8 \d0 \d1 
+"C" "VALU" 
+"T" \d0 7F "normal (according to climate)" 00 
+"T" \d1 7F "alpine (temperate grass in arctic)" 00 
+"T" \d2 7F "temperate (not implemented)" 00 
+"T" \d3 7F "arctic (not implemented)" 00 
+"T" \d4 7F "tropical (not implemented)" 00 
+"T" \d5 7F "toyland (not implemented)" 00 
+00 
+"B" "DFLT" \w4 \dx00000000 
+00 
+00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
 // param[10] = param[1]
-3 * 5 0D 0A \D= 01 00
+3 * 5 0D 0A \D= 01 00
```

### Comparing `nml-0.7.2/regression/expected/022_disable_item.nfo` & `nml-r1512/regression/expected/022_disable_item.nfo`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d5
+0 * 4 \d5 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\22" "NML regression test" 00 "A test newgrf testing NML" 00
-3 * 124 00 00 \b1 74 FF \wx0000
-06 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "A" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
+3 * 124 00 00 \b1 74 FF \wx0000 
+06 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 
 
-4 * 9 00 0A \b1 01 FF \wx000C
-08 FF
+4 * 7 00 0A \b1 01 0C 
+08 FF 
 
-5 * 24 00 0B \b2 03 FF \wx000A
-08 FF FF FF
-17 \dx00000000 \dx00000000 \dx00000000
+5 * 22 00 0B \b2 03 0A 
+08 FF FF FF 
+17 \dx00000000 \dx00000000 \dx00000000
```

### Comparing `nml-0.7.2/regression/expected/023_engine_override.nfo` & `nml-r1512/regression/expected/002_sounds.nfo`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d4
+// param[0] = 73
+0 * 9 0D 00 \D= FF 00 \dx00000049 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\23" "NML regression test" 00 "A test newgrf testing NML" 00
-3 * 16 00 08 \b1 01 FF \wx0000
-11 \dx74736574 \dx44434241
-
-4 * 16 00 08 \b1 01 FF \wx0000
-11 \dx234C4D4E \dx78563412
+// param[1] = 74
+1 * 9 0D 01 \D= FF 00 \dx0000004A 
 
+2 * 3 11 \w2 
+3 ** beef.wav
+4 * 8 FE 00 \dx87654321 \wx0003
```

### Comparing `nml-0.7.2/regression/expected/024_conditional.nfo` & `nml-r1512/regression/expected/009_replaceTTDsprite.nfo`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-// param[127] = param[0]
-0 * 5 0D 7F \D= 00 00
+0 * 4 \d5 
 
-1 * 9 09 7F 04 \7= \dx00000000 01
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "W" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
+3 * 5 0A \b1 \b2 \w3092 
 
-// param[1] = 1
-2 * 9 0D 01 \D= FF 00 \dx00000001
-
-// param[3] = 1
-3 * 9 0D 03 \D= FF 00 \dx00000001
+4 opengfx_generic_trams1.pcx 48 56 01 18 8 -3 -10 
+5 opengfx_generic_trams1.pcx 48 56 01 18 8 -3 4
```

### Comparing `nml-0.7.2/regression/expected/027_airport_layout.nfo` & `nml-r1512/regression/expected/027_airport_layout.nfo`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 6 01 11 \b1 FF \wx0001
+0 * 6 01 11 \b1 FF \wx0001 
 
-1 * 1 00
+1 * 1 00 
 
-// Name: small_airport_tile_layout - feature 11
-2 * 25 02 11 FF \b2 \dx80000000
-\dxC0008000 \b32 \b16 80
-\dx80000000 \b0 \b0 \b0 \b16 \b16 \b16
-
-3 * 16 00 11 \b4 01 FF \wx0000
-08 00
-0F \wx0103
-10 01
-11 01
-
-4 * 7 03 11 01 00 \b0
-\wx00FF 	// small_airport_tile_layout;
-
-5 * 36 00 0D \b2 01 FF \wx0000
-08 00
-0A \b1 \d21
-00 00 00 FE \wx0000
-01 00 FE \wx0000
-02 00 FE \wx0000
-03 00 46
-00 80
+// Name: small_airport_tile_layout
+2 * 25 02 11 FE \b2 \dx80000000 
+\dxC0008000 \b32 \b16 80 
+\dx80000000 \b0 \b0 \b0 \b16 \b16 \b16 
+
+3 * 16 00 11 \b5 01 00 
+08 00 
+0F \wx0103 
+10 01 
+11 01 
+0E 01 
+
+4 * 7 03 11 01 00 \b0 
+\wx00FE 
+
+5 * 34 00 0D \b2 01 00 
+08 00 
+0A \b1 \d21 
+00 00 00 FE \wx0000 
+01 00 FE \wx0000 
+02 00 FE \wx0000 
+03 00 46 
+00 80
```

### Comparing `nml-0.7.2/regression/expected/039_storage.nfo` & `nml-r1512/regression/expected/006_vehicle.nfo`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 // Automatically generated by GRFCODEC. Do not modify!
-// (Info version 32)
+// (Info version 7)
 // Escapes: 2+ 2- 2< 2> 2u< 2u> 2/ 2% 2u/ 2u% 2* 2& 2| 2^ 2sto = 2s 2rst = 2r 2psto 2ror = 2rot 2cmp 2ucmp 2<< 2u>> 2>>
 // Escapes: 71 70 7= 7! 7< 7> 7G 7g 7gG 7GG 7gg 7c 7C
 // Escapes: D= = DR D+ = DF D- = DC Du* = DM D* = DnF Du<< = DnC D<< = DO D& D| Du/ D/ Du% D%
-// Format: spritenum imagefile depth xpos ypos xsize ysize xrel yrel zoom flags
+// Format: spritenum pcxfile xpos ypos compression ysize xsize xrel yrel
 
-0 * 4 \d10
+0 * 4 \d20 
 
-1 * 54 14 "C" "INFO"
-"B" "VRSN" \w4 \dx00000000
-"B" "MINV" \w4 \dx00000000
-"B" "NPAR" \w1 00
-"B" "PALS" \w1 "A"
-"B" "BLTR" \w1 "8"
-00
-00
-2 * 52 08 08 "NML\39" "NML regression test" 00 "A test newgrf testing NML" 00
-// Name: switch_storage2
-3 * 96 02 0A FF 8A
-1A 20 \dxFFFFFFFF
-\2sto 1A 20 \dx00000100
-\2r 1A 20 \dx44495247
-\2sto 1A 20 \dx00000100
-\2r 7C 01 20 \dxFFFFFFFF
-\2sto 1A 20 \dx00000080
-\2r 1A 20 \dxFFFFFFFF
-\2sto 1A 20 \dx00000100
-\2r 7C 00 20 \dxFFFFFFFF
-\2+ 7D 80 20 \dxFFFFFFFF
-\2psto 1A 00 \dx00000000
-\b1
-\wx8000 \dx00000001 \dx00000000 	// Bogus range to avoid nvar == 0
-\wx8000 // default: return 0;
-
-// Name: switch_storage1
-4 * 38 02 0A FF 89
-7C 00 20 \dxFFFFFFFF
-\2+ 1A 20 \dx00000001
-\2psto 1A 00 \dx00000000
-\b1
-\wx8000 \dx00000001 \dx00000000 	// Bogus range to avoid nvar == 0
-\wx00FF // default: switch_storage2;
-
-5 * 11 00 0A \b2 01 FF \wx0000
-08 00
-09 00
-
-6 * 9 00 0A \b1 01 FF \wx0000
-21 20
-
-// Name: @CB_FAILED_PROD
-7 * 15 02 0A FE 00 \wx0000 \wx0000 \wx0000 \wx0000 \wx0000 00
-
-// Name: @CB_FAILED0A
-8 * 23 02 0A FE 89
-0C 00 \dx0000FFFF
-\b1
-\wx8000 \dx00000000 \dx00000000 	// graphics callback -> return 0
-\wx00FE // Non-graphics callback, return graphics result
-
-// Name: @action3_0
-9 * 23 02 0A FE 89
-0C 00 \dx0000FFFF
-\b1
-\wx00FF \dx00000035 \dx00000035 	// switch_storage1;
-\wx00FE // @CB_FAILED0A;
+1 * 46 14 "C" "INFO" 
+"B" "VRSN" \w4 \dx00000000 
+"B" "MINV" \w4 \dx00000000 
+"B" "NPAR" \w1 00 
+"B" "PALS" \w1 "W" 
+00 
+00 
+2 * 52 08 07 "test" "NML regression test" 00 "A test newgrf testing NML" 00 
+3 * 30 00 08 \b1 06 00 
+09 "PASS" "MAIL" "GOOD" "IORE" "GOLD" 
+"FOOD" 
+
+4 * 6 01 01 \b1 FF \wx0008 
+
+5 opengfx_generic_trams1.pcx 48 56 01 18 8 -3 -10 
+6 opengfx_generic_trams1.pcx 64 56 01 19 20 -14 -5 
+7 opengfx_generic_trams1.pcx 96 56 01 15 28 -14 -8 
+8 opengfx_generic_trams1.pcx 144 56 01 19 20 -6 -7 
+9 opengfx_generic_trams1.pcx 176 56 01 18 8 -3 -10 
+10 opengfx_generic_trams1.pcx 192 56 01 19 20 -14 -9 
+11 opengfx_generic_trams1.pcx 224 56 01 15 28 -14 -8 
+12 opengfx_generic_trams1.pcx 272 56 01 19 20 -6 -7 
+
+// Name: foster_express_group
+13 * 9 02 01 FE \b1 \b1 
+\w0 
+\w0 
+
+// param[0] = 9
+14 * 9 0D 00 \D= FF 00 \dx00000009 
+
+// param[64] = (param[0] * 5)
+15 * 9 0D 40 \D* 00 FF \dx00000005 
+
+16 * 7 06 
+40 01 FF \wx002C 
+FF 
+
+17 * 57 00 01 \b21 01 FF \wx0059 
+06 03 
+04 28 
+03 1E 
+1F \dx000AF386 
+02 01 
+0A \dx00004C48 
+09 87 
+11 8F 
+08 95 
+13 16 
+14 58 
+0E FF 
+07 10 
+18 4D 
+19 80 
+0F 00 
+1D \wx0003 
+10 FF 
+1E \wx0000 
+10 FF 
+1C 01 
 
-10 * 7 03 0A 01 00 \b0
-\wx00FE 	// @action3_0;
+18 * 27 04 01 7F 01 FF \wx0059 "Foster Express Tram" 00 
+
+19 * 23 04 01 1F 01 FF \wx0059 "Foster Sneltram" 00 
+
+20 * 9 03 01 01 FF \wx0059 \b0 
+\wx00FE
```

### Comparing `nml-0.7.2/regression/lang/english.lng` & `nml-r1512/regression/lang/english.lng`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 STR_NULL                       :
 STR_REGRESSION_NAME            :NML regression test
 STR_REGRESSION_DESC            :A test newgrf testing NML
 STR_REGRESSION_ERROR           :Something bad (tm) has happened.
 STR_REGRESSION_CARE            :care
 STR_ANSWER                     :42
 STR_NAME_FOSTER_EXPRESS_TRAM   :Foster Express Tram
-STR_NAME_FOSTER_TURBO_TRAM     :Foster Turbo Tram
-STR_NAME_PLANE                 :Test plane 0x14
 STR_NAME_BULK_WAGON            :NML Test bulk wagon
 STR_PARAM_NAME                 :Name of the int setting
 STR_PARAM_DESC                 :Description of a setting
 
 STR_PARAM_NOGRID               :Disable gridlines
 STR_PARAM_NOGRID_DESC          :This setting allows to replace all ground sprites such that the landscape is painted (mostly) without grid lines. Note that roads and train tracks don't yet follow this rule
 STR_PARAM_TRANSMITTER          :Replace the transmitter tower by a rock
@@ -21,23 +19,15 @@
 STR_PARAM_LANDSCAPE_NORMAL     :normal (according to climate)
 STR_PARAM_LANDSCAPE_ALPINE     :alpine (temperate grass in arctic)
 STR_PARAM_LANDSCAPE_TEMPERATE  :temperate (not implemented)
 STR_PARAM_LANDSCAPE_ARCTIC     :arctic (not implemented)
 STR_PARAM_LANDSCAPE_TROPICAL   :tropical (not implemented)
 STR_PARAM_LANDSCAPE_TOYLAND    :toyland (not implemented)
 
-STR_STATIONS                   :Teßt Stätiöµſ
-
-STR_STATION_TEST_CLASS         :Test
-STR_STATION_BASIC              :Basic station
-STR_STATION_BASIC2             :Basic station 2
+STR_STATIONS                   :Test Stations
 
 STR_OBJ_MISC_CLASS             :Miscellaneous
 STR_OBJ_BASIC                  :Basic object
 
-STR_COALMINE_EXTRA_TEXT        :{BLACK}Extra info for coal mine: {COMMA}
+STR_COALMINE_EXTRA_TEXT        :{BLACK}Extra info for coal mine: {DWORD_S}
 STR_COALMINE_MONTH_0_10        :{BLACK}coal
 STR_COALMINE_MONTH_11          :{BLACK}diamonds
-
-STR_BREWERY_NAME               :Brewery
-
-STR_032_HOUSE                  :Example house
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nml-0.7.2/regression/opengfx_generic_trams1.pcx` & `nml-r1512/regression/opengfx_generic_trams1.pcx`

 * *Files 14% similar despite different names*

```diff
@@ -1,904 +1,895 @@
-00000000: 0a05 0108 0000 0000 7201 9500 4800 4800  ........r...H.H.
+00000000: 0a05 0108 0000 0000 7201 9500 2c01 2c01  ........r...,.,.
 00000010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000040: 0001 7401 0100 0000 0000 0000 0000 0000  ..t.............
+00000040: 0001 7301 0100 0000 0000 0000 0000 0000  ..s.............
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: ffff ffff ffff ffff ffff f8ff 00ff ffff  ................
-00000090: ffff ffff ffff fff8 ff00 ffff ffff ffff  ................
-000000a0: ffff ffff f8ff 00ff ffff ffff ffff ffff  ................
-000000b0: fff8 ff00 ffff ffff ffff ffff ffff f8ff  ................
-000000c0: 00ff ffff ffff ffff ffff fff8 ff00 ffff  ................
-000000d0: ffff ffff ffff ffff f8ff 00ff ffff ffff  ................
-000000e0: ffff ffff fff8 ff00 ffff ffff ffff ffff  ................
-000000f0: ffff f8ff 00ff ffff ffff ffff ffff fff8  ................
-00000100: ff00 f0ff c800 c8ff d400 ccff c400 6ac1  ..............j.
-00000110: d8d6 00d4 ffc3 006a d000 ccff c300 6ac4  .......j......j.
-00000120: 00c8 ffd0 006a c300 ccff d700 c1d8 6ac3  .....j........j.
-00000130: 00d4 ffd4 00ff ffd0 ff00 f0ff c200 58c1  ..............X.
-00000140: d888 58c2 00c8 ffd4 00cc ffc6 00c2 d8d4  ..X.............
-00000150: 00d4 ffc4 00c1 d8cf 00cc ffc2 0058 c1d8  .............X..
-00000160: 8858 c200 c8ff cf00 c1d8 c400 ccff d500  .X..............
-00000170: c2d8 c500 d4ff c300 c288 58c3 d8cb 00ff  ..........X.....
-00000180: ffd0 ff00 f0ff 0088 58c2 8858 6a00 c8ff  ........X..Xj...
-00000190: d400 ccff c800 c2d8 d200 d4ff c500 c1d8  ................
-000001a0: ce00 ccff 0088 58c1 d888 586a 00c8 ffce  ......X...Xj....
-000001b0: 00c1 d8c5 00cc ffd3 00c2 d8c7 00d4 ff00  ................
-000001c0: 6a58 83c1 d8c2 88c1 d858 c2d8 c900 ffff  jX.......X......
-000001d0: d0ff 00f0 ffc5 8858 6a58 c8ff cb00 c3d8  .......XjX......
-000001e0: 58c2 88c3 00cc ffc4 00d5 d8c3 00d4 ffc3  X...............
-000001f0: 00c2 8858 c1d8 c26a cb00 ccff c388 c1d8  ...X...j........
-00000200: 8858 6a58 c8ff cb00 c3d8 58c2 88c3 00cc  .XjX......X.....
-00000210: ffc3 00d5 d8c4 00d4 ffc2 88c3 5883 c1d8  ............X...
-00000220: c288 c258 c2d8 c700 ffff d0ff 00f0 ffc1  ...X............
-00000230: d888 58c3 886a 58c8 ffc9 00c2 d858 c1d8  ..X..jX......X..
-00000240: c288 c1d8 83c2 5800 ccff c200 c2d8 88c1  ......X.........
-00000250: d888 c2d8 88c3 d888 c1d8 c288 c1d8 c488  ................
-00000260: 5888 c3d8 00d4 ff00 c1d8 5883 c1d8 c288  X.........X.....
-00000270: c1d8 58c2 6ac9 00cc ffc1 d888 58c1 d8c2  ..X.j.......X...
-00000280: 886a 58c8 ffc9 00c2 d858 c1d8 c288 c1d8  .jX......X......
-00000290: 83c2 5800 ccff 00c2 d888 c1d8 88c2 d888  ..X.............
-000002a0: c3d8 88c1 d8c2 88c1 d8c4 8858 88c3 d8c2  ...........X....
-000002b0: 00d4 ffc2 88c2 6ac3 5883 c1d8 c288 c258  ......j.X......X
-000002c0: c6d8 6aff ffd0 ff00 f0ff c1d8 8858 c1d8  ..j..........X..
-000002d0: c288 6a58 c8ff c700 c2d8 c258 c288 c1d8  ..jX.......X....
-000002e0: 83c3 58c2 6acc ff00 c4d8 88c1 d8c2 88c1  ..X.j...........
-000002f0: d888 c358 88c3 58c2 8858 6a58 c1d8 88c3  ...X..X..XjX....
-00000300: d8d4 ffc2 88c3 5883 c1d8 c288 c258 c26a  ......X......X.j
-00000310: c700 ccff c1d8 8858 c1d8 c288 6a58 c8ff  .......X....jX..
-00000320: c700 c2d8 c258 c288 c1d8 83c3 58c2 6acc  .....X......X.j.
-00000330: ffc4 d888 c1d8 c288 c1d8 88c3 5888 c358  ............X..X
-00000340: c288 586a 58c1 d888 c3d8 00d4 ff83 15c2  ..XjX...........
-00000350: 88c2 6ac3 5883 c1d8 c288 c258 c2d8 c300  ..j.X......X....
-00000360: ffff d0ff 00f0 ffc1 d888 c258 c288 6a58  ...........X..jX
-00000370: c8ff 6ac6 d8c2 58c2 88c1 d883 c358 c26a  ..j...X......X.j
-00000380: c288 ccff 00c1 d888 c1d8 c1c9 8483 c1c9  ................
-00000390: 8483 c1c9 8483 c1c9 8483 c1c9 8483 c1cb  ................
-000003a0: 8483 c1cb 8483 c1cb 88c1 d8d4 ffc2 88c1  ................
-000003b0: d86a c358 83c1 d8c2 88c2 58c2 6ac5 00cc  .j.X......X.j...
-000003c0: ffc1 d888 c258 c288 6a58 c8ff c500 c2d8  .....X..jX......
-000003d0: c258 c288 c1d8 83c3 58c2 6ac2 88cc ffc1  .X......X.j.....
-000003e0: d888 c1d8 c1c9 8483 c1c9 8483 c1c9 8483  ................
-000003f0: c1c9 8483 c1c9 8483 c1cb 8483 c1cb 8483  ................
-00000400: c1cb 88c1 d800 d4ff 840c 8315 c288 c26a  ...............j
-00000410: c358 83c1 d8c2 88c2 58c1 d8c2 00ff ffd0  .X......X.......
-00000420: ff00 f0ff c1d8 8858 c388 6a58 c8ff c300  .......X..jX....
-00000430: c2d8 c258 c288 c1d8 83c3 58c2 6ac2 880d  ...X......X.j...
-00000440: 85cc ff00 c2d8 88c8 586a c358 6a58 6a58  ........Xj.XjXjX
-00000450: 6a58 6ac2 5888 c2d8 d4ff 8315 c288 c1d8  jXj.X...........
-00000460: 6ac3 5883 c1d8 c288 c258 c26a c300 ccff  j.X......X.j....
-00000470: c1d8 8858 c388 6a58 c8ff c300 c2d8 c258  ...X..jX.......X
-00000480: c288 c1d8 83c3 58c2 6ac2 880d 85cc ffc2  ......X.j.......
-00000490: d888 c858 6ac3 586a 586a 586a 586a c258  ...Xj.XjXjXjXj.X
-000004a0: 88c2 d800 d4ff c2c8 840c 8315 c288 c26a  ...............j
-000004b0: c358 83c1 d888 c258 8800 ffff d0ff 00f0  .X.....X........
-000004c0: ffc1 d888 c258 c1d8 886a 58c8 ffc2 00c1  .....X...jX.....
-000004d0: d8c2 58c2 88c1 d883 c358 c26a c288 0d85  ..X......X.j....
-000004e0: 0c15 ccff 0081 88d2 6ac2 20c3 6a88 81d4  ........j. .j...
-000004f0: ff84 0c83 15c2 88c1 d86a c358 83c1 d8c2  .........j.X....
-00000500: 88c2 586a c200 ccff c1d8 88c2 58c2 886a  ..Xj........X..j
-00000510: 58c8 ffc2 00c1 d8c2 58c2 88c1 d883 c358  X.......X......X
-00000520: c26a c288 0d85 0c15 ccff 8188 d26a c220  .j...........j. 
-00000530: c36a 8881 00d4 ffc1 c8c1 d7c2 c984 0c83  .j..............
-00000540: 15c2 88c2 6ac3 58c5 88ff ffd0 ff00 f0ff  ....j.X.........
-00000550: c1d8 8858 88c1 d888 6a58 c8ff 0088 c258  ...X....jX.....X
-00000560: 88c1 d883 c358 c26a c288 0d85 0c15 c2cb  .....X.j........
-00000570: ccff 0080 8483 0d85 8483 0d85 8483 0d85  ................
-00000580: 8483 0d85 8483 0d85 8483 0d84 c283 d4ff  ................
-00000590: c2c8 840c 8315 c288 c1d8 6ac3 5883 c1d8  ..........j.X...
-000005a0: 88c2 5888 00cc ffc1 d888 58c3 886a 58c8  ..X.......X..jX.
-000005b0: ff00 88c2 5888 c1d8 83c3 58c2 6ac2 880d  ....X.....X.j...
-000005c0: 850c 15c2 cbcc ff80 8483 0d85 8483 0d85  ................
-000005d0: 8483 0d85 8483 0d85 8483 0d85 8483 0d84  ................
-000005e0: c283 00d4 ffc1 d758 c1d7 c1c9 c1c8 c1c9  .......X........
-000005f0: 840c 8315 c488 58c3 cac1 cb81 ffff d0ff  ......X.........
-00000600: 00f0 ffc1 d888 c258 c1d8 886a 58c8 ffc5  .......X...jX...
-00000610: 88c3 58c2 6ac2 880d 850c 15c2 cbc1 cac1  ..X.j...........
-00000620: cbcc ff00 c1ca 8584 0c15 8584 0c15 8584  ................
-00000630: 0c15 8584 0c15 8584 0c15 8584 0c85 84c1  ................
-00000640: ccd4 ffc1 c8c1 d7c2 c984 0c83 15c2 88c1  ................
-00000650: d86a c358 c588 ccff c1d8 88c2 58c2 886a  .j.X........X..j
-00000660: 58c8 ffc5 88c3 58c2 6ac2 880d 850c 15c2  X.....X.j.......
-00000670: cbc1 cac1 cbcc ffc1 ca85 840c 1585 840c  ................
-00000680: 1585 840c 1585 840c 1585 840c 1585 840c  ................
-00000690: 8584 c1cc 00d4 ff00 826a 58c1 d7c1 cac2  .........jX.....
-000006a0: c984 0c83 15c2 88c1 cac2 cb81 c283 ffff  ................
-000006b0: d0ff 00f0 ffc1 d888 c258 c1d8 886a 58c8  .........X...jX.
-000006c0: ffc1 d880 c1c9 88c2 58c2 6ac2 880d 850c  ........X.j.....
-000006d0: 15c2 cbc1 ca82 58c1 c9cc ff00 c1c9 d9cb  ......X.........
-000006e0: c1cc d4ff c1d7 58c1 d7c1 c9c1 c8c1 c984  ......X.........
-000006f0: 0c83 15c4 88c2 5888 c1cb 83c1 cbcc ffc1  ......X.........
-00000700: d888 c258 c288 6a58 c8ff c1d8 80c1 c988  ...X..jX........
-00000710: c258 c26a c288 0d85 0c15 c2cb c1ca 8258  .X.j...........X
-00000720: c1c9 ccff c1c9 d9cb c1cc 00d4 ffc3 0082  ................
-00000730: 6ac1 c7c1 cac1 cbc2 c984 0c83 1583 81c2  j...............
-00000740: 8384 c1cb ffff d0ff 00f0 ffc1 d881 c258  ...............X
-00000750: c1d8 886a 58c8 ffc1 d8c3 80c1 c958 c288  ...jX........X..
-00000760: 0d85 0c15 c1cb c1ca c1cc 8258 826a 00cc  ...........X.j..
-00000770: ff00 c1c9 c6cb c1c9 cbca c3cb c2ca c3cb  ................
-00000780: d4ff 0082 6a58 c1d7 c1ca c2c9 840c 8315  ....jX..........
-00000790: c1d8 8858 c1cb 8083 8083 ccff c1d8 81c2  ...X............
-000007a0: 58c2 886a 58c8 ffc1 d8c3 80c1 c958 c288  X..jX........X..
-000007b0: 0d85 0c15 c1cb c1ca c1cc 8258 826a 00cc  ...........X.j..
-000007c0: ffc1 c9c6 cbc1 c9cb cac3 cbc2 cac3 cb00  ................
-000007d0: d4ff c600 c1c7 c1c8 c1cb c1d7 c2c9 840c  ................
-000007e0: 8483 84c2 cac1 cbff ffd0 ff00 f0ff c1d8  ................
-000007f0: 81c2 88c1 d888 c258 c8ff c1d8 c280 c281  .......X........
-00000800: c1cc 0d85 0c15 c2cb c1cc c1cb c1c8 826a  ...............j
-00000810: c300 ccff c200 c2cb 82c4 58c1 d7c7 cbc2  ..........X.....
-00000820: cc82 c458 c1d7 c1cc c1cd 00d4 ffc3 0082  ...X............
-00000830: 6ac1 c7c1 cac1 cbc2 c984 0c83 15c1 ccc2  j...............
-00000840: 8183 80c1 cbcc ffc1 d881 c488 c258 c8ff  .............X..
-00000850: c1d8 c280 c281 c1cc 0d85 0c15 c2cb c1cc  ................
-00000860: c1cb c1c8 826a c300 ccff 00c2 cb82 c458  .....j.........X
-00000870: c1d7 c7cb c2cc 82c4 58c1 d7c1 ccc1 cdc2  ........X.......
-00000880: 00d4 ffc8 00c1 d758 c1d7 c1cb c2c9 c3ca  .......X........
-00000890: b5c1 cac1 c8ff ffd0 ff00 f0ff c1c9 c381  ................
-000008a0: 6a81 c2cb c8ff c1ca c1c9 81c2 83c1 cb0c  j...............
-000008b0: 15c1 cbc1 cac2 cbc1 c9c1 c8c6 00cc ffc4  ................
-000008c0: 0082 6ac2 8882 6ac9 0082 6ac2 8882 6ac3  ..j...j...j...j.
-000008d0: 00d4 ffc6 00c1 c7c1 c8c1 cbc1 d7c2 c984  ................
-000008e0: 0cc1 cbc2 8381 c1c9 c1ca ccff c1c9 c381  ................
-000008f0: 8081 c2cb c8ff c1ca c1c9 81c2 83c1 cb0c  ................
-00000900: 15c1 cbc1 cac2 cbc1 c9c1 c8c6 00cc ffc3  ................
-00000910: 0082 6ac2 8882 6ac9 0082 6ac2 8882 6ac4  ..j...j...j...j.
-00000920: 00d4 ffc9 0082 6a58 c1d7 c1cb c1ca c1cb  ......jX........
-00000930: c1ca c1c8 c200 ffff d0ff 00f0 ffc1 c9c2  ................
-00000940: 8180 c1d8 8384 c1cb c8ff 58c1 c8b5 c1c9  ..........X.....
-00000950: 84c1 c9c2 cac1 cb82 58c1 c8c8 00fc ffc8  ........X.......
-00000960: 00c1 d758 c1d7 c1cb c3c9 84c1 c934 c1c8  ...X.........4..
-00000970: 58cc ffc1 c9c2 8180 8183 84c1 cbc8 ff58  X..............X
-00000980: c1c8 43c1 c984 c1c9 c2ca c1cb 8258 c1c8  ..C..........X..
-00000990: c800 fcff cb00 826a c1c9 c1ca c1c8 c400  .......j........
-000009a0: ffff d0ff 00f0 ffc1 cac2 8081 83c2 84c1  ................
-000009b0: cbc8 ffc2 0058 6ac1 cac1 c9c1 cb82 5882  .....Xj.......X.
-000009c0: 6ac9 00fc ffc9 0082 6a58 c1d7 c1cb c1c9  j.......jX......
-000009d0: c1ca 6a58 c200 ccff c1ca c280 8183 c284  ..jX............
-000009e0: c1cb c8ff c200 586a c1ca c1c9 c1cb 8258  ......Xj.......X
-000009f0: 826a c900 fcff d400 ffff d0ff 00f0 ffc4  .j..............
-00000a00: c9c1 cac2 c9c1 cac8 ffc4 0058 6ac1 c982  ...........Xj...
-00000a10: 6acb 00fc ffcb 0082 6ac1 c96a 58c4 00cc  j.......j..jX...
-00000a20: ffc3 c9c2 34c2 c9c1 cac8 ffc4 0058 6ac1  ....4........Xj.
-00000a30: c982 6acb 00fc ffd4 00ff ffd0 ff00 f0ff  ..j.............
-00000a40: c3c9 c2b5 c3ca ffff f9ff c4c9 c4ca ffff  ................
-00000a50: ffff fdff 00f0 ff00 c6ca 00ff fff9 ffc2  ................
-00000a60: 586a c220 c228 c1f5 ffff ffff fdff 00f0  Xj. .(..........
-00000a70: ffc8 00ff fff9 ff00 c658 00ff ffff fffd  .........X......
-00000a80: ff00 ffff ffff ffff ffff ffff f8ff 00ff  ................
-00000a90: ffff ffff ffff ffff fff8 ff00 ffff ffff  ................
-00000aa0: ffff ffff ffff f8ff 00ff ffff ffff ffff  ................
-00000ab0: ffff fff8 ff00 ffff ffff ffff ffff ffff  ................
-00000ac0: f8ff 00ff ffff ffff ffff ffff fff8 ff00  ................
-00000ad0: d1ff c4d7 c1ff c4d7 d4ff c3d7 cdff c3d7  ................
-00000ae0: c5ff c2d7 c1ff c2d7 c1ff c4d7 e3ff c3d7  ................
-00000af0: d2ff c2d7 c1ff c2d7 c4ff c8d7 e1ff c3d7  ................
-00000b00: c4ff c4d7 c6ff c1d7 c3ff c4d7 cfff c3d7  ................
-00000b10: c2ff c4d7 c2ff c3d7 cbff c3d7 d2ff c1d7  ................
-00000b20: c3ff c4d7 ffff dcff 00d2 ffc2 d7c3 ffc2  ................
-00000b30: d7d4 ffc2 d7c1 ffc2 d7cd ffc2 d7c5 ffc2  ................
-00000b40: d7c1 ffc2 d7c2 ffc2 d7ca ffc1 d7da ffc2  ................
-00000b50: d7d2 ffc2 d7c1 ffc2 d7c4 ffc1 d7c2 ffc2  ................
-00000b60: d7c2 ffc1 d7e2 ffc2 d7c3 ffc2 d7c2 ffc2  ................
-00000b70: d7c4 ffc2 d7c2 ffc2 d7c2 ffc2 d7cd ffc2  ................
-00000b80: d7c3 ffc2 d7c2 ffc2 d7c2 ffc2 d7cc ffc2  ................
-00000b90: d7d1 ffc2 d7c2 ffc2 d7c2 ffc2 d7ff ffdb  ................
-00000ba0: ff00 d2ff c2d7 c3ff c2d7 d4ff c2d7 d0ff  ................
-00000bb0: c2d7 c5ff c2d7 c1ff c2d7 c2ff c2d7 caff  ................
-00000bc0: c1d7 daff c2d7 d2ff c2d7 c1ff c2d7 c7ff  ................
-00000bd0: c2d7 e5ff c2d7 c3ff c2d7 c2ff c2d7 c3ff  ................
-00000be0: c3d7 c2ff c2d7 c2ff c2d7 ccff c2d7 c4ff  ................
-00000bf0: c2d7 c2ff c2d7 c2ff c2d7 ccff c2d7 d0ff  ................
-00000c00: c3d7 c2ff c2d7 c2ff c2d7 ffff dbff 00d2  ................
-00000c10: ffc2 d7c3 ffc2 d7c2 ffc3 d7c2 ffc3 d7c1  ................
-00000c20: ffc2 d7c1 ffc3 d7c2 ffc4 d7c1 ffc3 d7c2  ................
-00000c30: ffc3 d7c1 ffc2 d7c1 ffc4 d7cc ffc2 d7c1  ................
-00000c40: ffc3 d7c1 ffc2 d7c1 ffc4 d7c1 ffc3 d7c2  ................
-00000c50: ffc3 d7c1 ffc5 d7c1 ffc2 d7c1 ffc3 d7c1  ................
-00000c60: ffc6 d7c3 ffc3 d7c2 ffc3 d7c1 ffc2 d7ce  ................
-00000c70: ffc2 d7c3 ffc3 d7c1 ffc2 d7c1 ffc3 d7c2  ................
-00000c80: ffc3 d7c1 ffc2 d7c1 ffc2 d7cd ffc2 d7c3  ................
-00000c90: ffc2 d7c2 ffc2 d7c3 ffc3 d7c2 ffc2 d7c2  ................
-00000ca0: ffc2 d7cb ffc5 d7c2 ffc2 d7c2 ffc2 d7c2  ................
-00000cb0: ffc2 d7c1 ffc8 d7c3 ffc2 d7c1 ffc2 d7cd  ................
-00000cc0: ffc3 d7c2 ffc2 d7c2 ffc2 d7c3 ffc5 d7c3  ................
-00000cd0: ffc3 d7c3 ffc4 d7c2 ffc4 d7c2 ffc3 d7c2  ................
-00000ce0: ffc3 d7c1 ffc2 d7c2 ffc5 d7c2 ffc3 d7c2  ................
-00000cf0: ffc3 d7c1 ffc2 d7c1 ffc4 d7d9 ff00 d2ff  ................
-00000d00: c7d7 c1ff c2d7 c1ff c2d7 c2ff c3d7 c1ff  ................
-00000d10: c3d7 c1ff c2d7 c2ff c2d7 c1ff c2d7 c1ff  ................
-00000d20: c2d7 c2ff c3d7 c1ff c3d7 c1ff c2d7 ccff  ................
-00000d30: c2d7 c2ff c5d7 c2ff c2d7 c1ff c2d7 c1ff  ................
-00000d40: c2d7 c2ff c3d7 c1ff c1d7 c1ff c2d7 c1ff  ................
-00000d50: c2d7 c2ff c3d7 c1ff c3d7 c1ff c2d7 c1ff  ................
-00000d60: c2d7 c1ff c2d7 c2ff c5d7 ceff c2d7 c4ff  ................
-00000d70: c3d7 c1ff c3d7 c1ff c2d7 c2ff c8d7 cdff  ................
-00000d80: c2d7 c3ff c2d7 c2ff c2d7 c2ff c1d7 c1ff  ................
-00000d90: c2d7 c2ff c2d7 c2ff c2d7 cbff c2d7 c2ff  ................
-00000da0: c2d7 c1ff c2d7 c2ff c2d7 c2ff c2d7 c1ff  ................
-00000db0: c1d7 c3ff c2d7 c1ff c2d7 c2ff c5d7 ccff  ................
-00000dc0: c1d7 c1ff c2d7 c2ff c2d7 c2ff c2d7 c4ff  ................
-00000dd0: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
-00000de0: c2d7 c2ff c1d7 c1ff c2d7 c2ff c1d7 c1ff  ................
-00000df0: c2d7 c1ff c2d7 c2ff c5d7 c1ff c2d7 c1ff  ................
-00000e00: c2d7 c2ff c2d7 c1ff c2d7 c2ff c3d7 c1ff  ................
-00000e10: c3d7 c2ff c1d7 d9ff 00d2 ffc2 d7c3 ffc2  ................
-00000e20: d7c1 ffc5 d7c2 ffc2 d7c3 ffc5 d7c2 ffc2  ................
-00000e30: d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2  ................
-00000e40: d7c1 ffc2 d7cc ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00000e50: d7c2 ffc2 d7c1 ffc5 d7c2 ffc2 d7c4 ffc2  ................
-00000e60: d7c1 ffc2 d7c2 ffc2 d7c3 ffc2 d7c1 ffc2  ................
-00000e70: d7c4 ffc2 d7c2 ffc2 d7c1 ffc2 d7ce ffc2  ................
-00000e80: d7c4 ffc2 d7c6 ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00000e90: d7c1 ffc2 d7cd ffc2 d7c4 ffc5 d7c1 ffc1  ................
-00000ea0: d7c2 ffc2 d7c2 ffc2 d7c2 ffc2 d7cb ffc2  ................
-00000eb0: d7c2 ffc2 d7c1 ffc2 d7c2 ffc2 d7c2 ffc4  ................
-00000ec0: d7c3 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00000ed0: d7cb ffc1 d7c2 ffc2 d7c2 ffc2 d7c2 ffc2  ................
-00000ee0: d7c4 ffc2 d7c1 ffc2 d7c4 ffc2 d7c1 ffc3  ................
-00000ef0: d7c3 ffc3 d7c3 ffc5 d7c2 ffc2 d7c1 ffc2  ................
-00000f00: d7c1 ffc2 d7c1 ffc2 d7c2 ffc5 d7c2 ffc2  ................
-00000f10: d7c3 ffc3 d7db ff00 d2ff c2d7 c3ff c2d7  ................
-00000f20: c1ff c2d7 c5ff c2d7 c3ff c2d7 c5ff c2d7  ................
-00000f30: c1ff c2d7 c1ff c2d7 c2ff c2d7 c3ff c2d7  ................
-00000f40: c1ff c2d7 ccff c2d7 c2ff c2d7 c1ff c2d7  ................
-00000f50: c2ff c2d7 c1ff c2d7 c5ff c2d7 c4ff c2d7  ................
-00000f60: c1ff c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7  ................
-00000f70: c2ff c4d7 c2ff c2d7 c1ff c2d7 ceff c2d7  ................
-00000f80: c4ff c2d7 c4ff c4d7 c2ff c2d7 c1ff c2d7  ................
-00000f90: c1ff c2d7 c4ff c3d7 c6ff c2d7 c6ff c2d7  ................
-00000fa0: c2ff c6d7 c1ff c2d7 c2ff c2d7 c4ff c3d7  ................
-00000fb0: c4ff c2d7 c2ff c2d7 c1ff c2d7 c2ff c2d7  ................
-00000fc0: c2ff c2d7 c1ff c2d7 c2ff c2d7 c1ff c2d7  ................
-00000fd0: c2ff c2d7 c1ff c2d7 c4ff c3d7 c4ff c6d7  ................
-00000fe0: c1ff c2d7 c2ff c2d7 c4ff c2d7 c1ff c2d7  ................
-00000ff0: c2ff c4d7 c3ff c3d7 c3ff c3d7 c1ff c2d7  ................
-00001000: c5ff c2d7 c1ff c2d7 c2ff c3d7 c3ff c2d7  ................
-00001010: c5ff c2d7 c5ff c3d7 d9ff 00d2 ffc2 d7c3  ................
-00001020: ffc2 d7c1 ffc2 d7c2 ffc1 d7c2 ffc2 d7c3  ................
-00001030: ffc2 d7c2 ffc1 d7c2 ffc2 d7c1 ffc2 d7c1  ................
-00001040: ffc2 d7c2 ffc2 d7c3 ffc2 d7c1 ffc2 d7cc  ................
-00001050: ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1  ................
-00001060: ffc2 d7c2 ffc1 d7c2 ffc2 d7c4 ffc2 d7c1  ................
-00001070: ffc2 d7c2 ffc2 d7c3 ffc2 d7c1 ffc2 d7c1  ................
-00001080: ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc2 d7ce  ................
-00001090: ffc2 d7c4 ffc2 d7c3 ffc2 d7c1 ffc2 d7c2  ................
-000010a0: ffc2 d7c1 ffc2 d7c1 ffc2 d7cd ffc2 d7c5  ................
-000010b0: ffc2 d7c6 ffc2 d7c2 ffc2 d7c2 ffc2 d7cb  ................
-000010c0: ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc2 d7c2  ................
-000010d0: ffc2 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
-000010e0: ffc2 d7c1 ffc2 d7ce ffc2 d7c2 ffc2 d7c2  ................
-000010f0: ffc2 d7c4 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1  ................
-00001100: ffc2 d7c1 ffc1 d7c2 ffc2 d7c1 ffc1 d7c2  ................
-00001110: ffc2 d7c1 ffc2 d7c2 ffc1 d7c2 ffc2 d7c1  ................
-00001120: ffc2 d7c1 ffc1 d7c6 ffc2 d7c2 ffc1 d7c2  ................
-00001130: ffc2 d7c3 ffc1 d7c2 ffc2 d7d9 ff00 d1ff  ................
-00001140: c4d7 c1ff c4d7 c1ff c3d7 c2ff c4d7 c3ff  ................
-00001150: c3d7 c2ff c4d7 c1ff c3d7 c2ff c4d7 c3ff  ................
-00001160: c5d7 caff c7d7 c1ff c3d7 c1ff c3d7 c1ff  ................
-00001170: c3d7 c2ff c4d7 c4ff c9d7 c2ff c1d7 c1ff  ................
-00001180: c2d7 c3ff c8d7 c1ff c3d7 ccff c4d7 c2ff  ................
-00001190: c4d7 c3ff c8d7 c1ff c2d7 c1ff c3d7 cbff  ................
-000011a0: c4d7 c2ff c3d7 c7ff c2d7 c3ff c4d7 cdff  ................
-000011b0: c4d7 c3ff c4d7 c2ff c4d7 c1ff c7d7 c2ff  ................
-000011c0: c3d7 c1ff c3d7 cdff c2d7 c3ff c4d7 c5ff  ................
-000011d0: c4d7 c3ff c9d7 c2ff c4d7 c3ff c3d7 c2ff  ................
-000011e0: c3d7 c1ff c8d7 c3ff c3d7 c2ff c4d7 c2ff  ................
-000011f0: c4d7 daff 00ff ffff ffff fff8 ffc2 d7e6  ................
-00001200: ffc2 d7e3 ffc6 d7eb ff00 ffff ffff ffff  ................
-00001210: f8ff c2d7 e6ff c2d7 e3ff c1d7 c4ff c1d7  ................
-00001220: ebff 00ff ffff ffff fff7 ffc4 d7e4 ffc4  ................
-00001230: d7e3 ffc4 d7ec ff00 ffff ffff ffff ffff  ................
-00001240: ffff f8ff 00ff ffff ffff ffff ffff fff8  ................
-00001250: ff00 ffff ffff ffff ffff ffff f8ff 00ff  ................
-00001260: ffff ffff ffff ffff fff8 ff00 ffff ffff  ................
-00001270: ffff ffff ffff f8ff 00ff ffff ffff ffff  ................
-00001280: ffff fff8 ff00 ffff ffff ffff ffff ffff  ................
-00001290: f8ff 00f0 ff00 c1c9 c2ca c2cb c1cc 00c8  ................
-000012a0: ffcc 00c1 c9c1 cac1 ccc1 cbc4 00cc ff6a  ...............j
-000012b0: c1d8 da00 d4ff c300 6ad0 00cc ffc3 006a  ........j......j
-000012c0: c400 c8ff d000 6ac3 00cc ffda 00c1 d86a  ......j........j
-000012d0: d4ff c400 c1cb c1ca c2cb cc00 ffff d0ff  ................
-000012e0: 00f0 ffc1 c7c1 c9c1 cac1 c9c1 cac1 cbc1  ................
-000012f0: ccc1 cbc8 ffca 00c1 c7c2 cac3 cbc1 ccc1  ................
-00001300: cbc2 00cc ffc2 00c2 d8d8 00d4 ffc4 00c1  ................
-00001310: d8cf 00cc ff00 c1c7 c1c9 c1d8 c1c9 c1ca  ................
-00001320: c1c9 00c8 ffcf 00c1 d8c4 00cc ffd8 00c2  ................
-00001330: d8c2 00d4 ffc2 00c1 cac4 cbc2 ccc1 cbca  ................
-00001340: 00ff ffd0 ff00 f0ff c1c7 c2c9 c2ca c2cc  ................
-00001350: c1cb c8ff c800 c1c7 c2c9 c1ca c4cb c3cc  ................
-00001360: 00cc ffc4 00c2 d8d6 00d4 ffc5 00c1 d8ce  ................
-00001370: 00cc ffc2 c7c1 c9c1 d8c1 c9c1 cac1 cbc1  ................
-00001380: c9c8 ffce 00c1 d8c5 00cc ffd6 00c2 d8c4  ................
-00001390: 00d4 ff00 c2ca c4cb c1cc c1cb c2cc c1cb  ................
-000013a0: c800 ffff d0ff 00f0 ffc1 c7c1 c9c1 cac1  ................
-000013b0: c9c2 cac1 ccc1 cac8 ffc6 00c1 c7c2 c9c2  ................
-000013c0: cac1 ccc1 cbc3 ccc4 cbcc ffc4 00c1 cac1  ................
-000013d0: c9c2 d8d2 c9c2 00d4 ffc5 00c1 ccc1 d8c1  ................
-000013e0: cbcc 00cc ffc1 c7c1 c9c1 cac1 d8c1 cac1  ................
-000013f0: cbc1 ccc1 cac8 ffcd 00c1 d8c1 c9c1 cbc4  ................
-00001400: 00cc ffc2 00d2 c9c2 d8c1 c9c1 cac4 00d4  ................
-00001410: ffc1 cac1 c9c3 cac1 cbc1 c9c2 cac1 cbc3  ................
-00001420: ccc1 cbc6 00ff ffd0 ff00 f0ff c1c7 c2c9  ................
-00001430: c2ca c1cb c1cc c1cb c8ff 6ac6 d8c1 cac3  ..........j.....
-00001440: cbc3 ccc1 cbc1 cac1 cbc1 ca84 83cc ffc2  ................
-00001450: 00c2 c9c2 cbc2 c9c2 d8c2 c9c1 cac1 c9c2  ................
-00001460: cac1 c9c4 cac1 cbc2 cac1 cbc2 ca00 d4ff  ................
-00001470: c200 c1ca c1c9 c1ca c2cb c1d8 c1cc c1cb  ................
-00001480: ca00 ccff c1c7 c1c9 c1ca c1d8 c2ca c1cc  ................
-00001490: c1ca c8ff ca00 c1c7 c1c9 c1d8 c2ca c3cb  ................
-000014a0: c200 ccff 00c2 cac1 cbc2 cac1 cbc4 cac1  ................
-000014b0: c9c2 cac1 c9c1 cac2 c9c2 d8c2 c9c4 cbc2  ................
-000014c0: 00d4 ff83 81c5 c9c1 cac1 c9c1 cac2 cbc2  ................
-000014d0: ccc5 d86a ffff d0ff 00f0 ffc1 c7c1 c9c1  ...j............
-000014e0: cac1 c9c1 cac1 cbc1 ccc1 cbc8 ffc2 00c1  ................
-000014f0: c7c2 c9c1 cac1 c9c1 cac1 cbc3 ccc1 cbc1  ................
-00001500: cac1 c9c1 ca84 8385 84cc ff00 c2ca c2cb  ................
-00001510: c1cc c2ca c1c9 c1ca c258 c1cb c1ca c3cb  .........X......
-00001520: c2ca c1cb c1cc c3cb c1cc c1cb c2cc d4ff  ................
-00001530: 00c2 c9c1 cac2 c9c1 cac1 cbc1 d8c2 ccc1  ................
-00001540: cbc8 00cc ffc1 c7c2 c9c2 cac1 cbc1 ccc1  ................
-00001550: cbc8 ffc8 00c1 c7c2 c9c1 d8c1 cbc1 ccc1  ................
-00001560: cbc3 ccc1 cb00 ccff c2cc c1cb c1cc c3cb  ................
-00001570: c1cc c1cb c2ca c3cb c1ca c1cb c258 c1ca  .............X..
-00001580: c1c9 c2ca c1cc c3cb c1ca 00d4 ff84 c283  ................
-00001590: 81c1 c9c1 c7c3 c9c1 cac1 cbc1 cac1 ccc1  ................
-000015a0: cbc3 ccc1 cbc2 00ff ffd0 ff00 f0ff c1c7  ................
-000015b0: c1c9 c2ca c1d8 c2cc c1cb c8ff 00c2 c9c1  ................
-000015c0: cac1 c9c2 cac3 ccc1 cbc1 cac1 c9c1 ca84  ................
-000015d0: 8385 8483 c1ca ccff c2cc c1cb c1cc c1cb  ................
-000015e0: c1cc c5cb c1cc c3cb c1cc c1cb c1cc c1cb  ................
-000015f0: c1cc c1cb c3cc c4ca d4ff c5c9 c1ca c1c9  ................
-00001600: c2ca c1cb c3cc c1cb c600 ccff c1c7 c1c9  ................
-00001610: c1ca c1c9 c1ca c1cb c1cc c1cb c8ff c600  ................
-00001620: c1c7 c2c9 c2ca c1cc c1cb c3cc c2cb c1cc  ................
-00001630: c1cb ccff c4ca c3cc c1cb c1cc c1cb c1cc  ................
-00001640: c1cb c1cc c3cb c1cc c5cb c1cc c4cb c1cc  ................
-00001650: d4ff c1c8 8384 c283 81c1 c9c1 c7c3 c9c1  ................
-00001660: cac2 cbc1 ccc1 cbc3 cc00 ffff d0ff 00f0  ................
-00001670: ffc1 c7c1 c9c1 cac1 cbc1 d8c1 cac1 ccc1  ................
-00001680: cbc8 ffc1 c7c1 c8c1 cac1 c9c1 cac3 ccc1  ................
-00001690: cbc1 cac1 c9c1 ca84 8385 84c4 cacc ffc4  ................
-000016a0: cad8 ccd4 ff83 81c5 c9c1 cac1 c9c1 cac2  ................
-000016b0: cbc3 ccc1 cbc4 00cc ffc1 c7c1 c9c1 cac1  ................
-000016c0: cbc1 ccc1 cac1 ccc1 cbc8 ffc4 00c1 c7c2  ................
-000016d0: c9c1 cac3 cbc3 ccc1 cbc3 ca84 83cc ffda  ................
-000016e0: ccc1 cbc1 ccd4 ffc1 c8c3 c984 c283 81c1  ................
-000016f0: c9c1 c7c3 c9c1 cac1 cbc3 ccc1 cbc1 ccff  ................
-00001700: ffd0 ff00 f0ff c1c7 c1c9 c1ca c1cb c1d8  ................
-00001710: c2cc c1cb c8ff c1c9 c2c8 c1c7 c2cc c1cb  ................
-00001720: c1ca c1c9 c1ca 8483 8584 c4ca c1c8 c1ca  ................
-00001730: ccff c4cc c1cb c1c9 c5ca c1cb c2ca cdcb  ................
-00001740: 80d4 ff84 c283 81c1 c9c1 c7c3 c9c1 cac1  ................
-00001750: cbc1 cac1 ccc1 cbc1 ccc1 cbc1 ccc1 cac2  ................
-00001760: 00cc ffc1 c7c1 c9c3 cac1 cbc1 ccc1 cbc8  ................
-00001770: ffc2 00c1 c9c1 cac1 ccc1 cac1 c9c1 cac1  ................
-00001780: cbc3 ccc1 cbc1 cac1 c9c1 ca84 8385 84cc  ................
-00001790: ff80 cdcb c2ca c1cb c5ca c1c9 c4cb c1cc  ................
-000017a0: d4ff c1c8 c1d7 c4c9 84c2 8381 c1c8 c1c7  ................
-000017b0: c3c9 c1cb c1ca c3cb ffff d0ff 00f0 ffc1  ................
-000017c0: c7c1 c9c1 cbc1 ccc1 d8c2 ccc1 cbc8 ff83  ................
-000017d0: 81c1 c9c1 c8c1 c7c1 cbc2 ca84 8385 84c4  ................
-000017e0: cac1 cb82 58c1 c8cc ff80 c1cb 8183 84c1  ....X...........
-000017f0: cb81 8384 c1cb 8183 84c1 cb81 8384 c1cb  ................
-00001800: 8183 84c1 cb81 8384 80c2 81d4 ffc1 c7c1  ................
-00001810: c984 c283 81c1 c9c1 c7c3 c9c1 cac4 cbc2  ................
-00001820: ccc1 ca00 ccff c1c9 c1c7 c1c9 c1ca c1cb  ................
-00001830: c2cc c1cb c8ff 00c2 cac3 cbc4 ccc1 cbc1  ................
-00001840: cac1 c9c1 ca84 8385 84c2 cbcc ffc2 8180  ................
-00001850: 8483 81c1 cb84 8381 c1cb 8483 81c1 cb84  ................
-00001860: 8381 c1cb 8483 81c1 cb84 83c1 cbc2 83d4  ................
-00001870: ffc1 d758 c1d7 c1c9 c1c8 c2c9 c1c8 84c2  ...X............
-00001880: 8381 c2c9 c4ca 8381 ffff d0ff 00f0 ffc1  ................
-00001890: c7c1 c9c2 cbc1 d8c2 ccc1 cbc8 ff84 83c3  ................
-000018a0: c9c1 c784 8385 84c4 cac1 cc82 5882 6a00  ............X.j.
-000018b0: ccff 85c1 cb83 8485 c1cb 8384 85c1 cb83  ................
-000018c0: 8485 c1cb 8384 85c1 cb83 8485 c1cb 8384  ................
-000018d0: 8581 80c1 cad4 ffc2 c8c2 c984 c283 81c1  ................
-000018e0: c9c1 c7c1 c9c3 cac3 cbc2 ccc1 cbcc ffc1  ................
-000018f0: c9c1 c7c1 c9c3 cac1 ccc1 cbc8 ffc2 c9c4  ................
-00001900: cbc3 ccc1 cac1 c9c1 ca84 8385 84c2 cbc1  ................
-00001910: cac1 cbcc ffc1 ca80 8185 8483 c1cb 8584  ................
-00001920: 83c1 cb85 8483 c1cb 8584 83c1 cb85 8483  ................
-00001930: c1cb 8584 83c1 cb85 d4ff 0082 6a58 c1d7  ............jX..
-00001940: c1ca c4c9 84c2 8381 c1ca 8381 c1ca 8483  ................
-00001950: ffff d0ff 00f0 ffc2 c7c1 c8c1 c9c1 d8c2  ................
-00001960: cbc1 ccc8 ffc1 c7c1 c8c1 c983 81c1 c785  ................
-00001970: 84c4 cac1 ccc1 cbc1 c982 6ac3 00cc ffc1  ..........j.....
-00001980: c9c3 cbc1 cac1 c8c5 cac1 cbc2 cacb cbc2  ................
-00001990: cac1 c9d4 ffc1 cac1 d7c1 c8c3 c984 c283  ................
-000019a0: 81c2 c9c3 cac1 cbc2 cc81 c1cb ccff c1c9  ................
-000019b0: c3ca c1cb c2cc c1cb c8ff c1c9 80c2 c9c2  ................
-000019c0: ccc4 cb84 8385 84c2 cbc2 cac2 cccc ffc1  ................
-000019d0: c9c2 cacb cbc2 cac1 cbc5 cac1 c8c1 cac3  ................
-000019e0: cbc1 c9d4 ffc3 0082 6ac1 c7c1 cac1 cbc4  ........j.......
-000019f0: c984 83c1 ca84 83c2 cac1 cbff ffd0 ff00  ................
-00001a00: f0ff c1c7 c1c8 c1c9 c1ca 6ac1 cac2 cbc8  ..........j.....
-00001a10: ffb5 c2c8 8483 c1c8 c3ca c1c9 c1c8 c1cb  ................
-00001a20: c1c9 c1c8 c600 ccff b5c6 cbc1 c9cb cac3  ................
-00001a30: cbc2 cac4 cbd4 ffc1 c758 c2d7 c1c8 c2c9  .........X......
-00001a40: c1c8 84c2 8381 c1c9 c1ca c1cb c1ca c1c7  ................
-00001a50: 8083 c1cb ccff c1ca c381 8081 c1cb c1cc  ................
-00001a60: c8ff c1c9 c380 c1c9 c2cb c1ca 8483 8584  ................
-00001a70: c1c9 c3ca c1cb 8258 c1c9 ccff c4cb c2ca  .......X........
-00001a80: c3cb cbca c1c9 c6cb c1c9 d4ff c600 c1c7  ................
-00001a90: c1c8 c1cb c1d7 c4c9 c5ca b5ff ffd0 ff00  ................
-00001aa0: f0ff c1c8 8381 c2ca 8381 c1cb c8ff c1c7  ................
-00001ab0: c3c8 c1c9 c1c8 c1c9 c1ca c1cb 8258 c1c8  .............X..
-00001ac0: c800 ccff 00c2 cb82 c458 c1d7 c7cb c2cc  .........X......
-00001ad0: 82c4 58c1 d7c1 ccc2 cd00 d4ff 0082 6a58  ..X...........jX
-00001ae0: c1d7 c1ca c4c9 84c2 8381 c1ca c1c7 8081  ................
-00001af0: 84c1 cacc ffc1 cac2 8180 8183 84c1 ccc8  ................
-00001b00: ffc1 c8c2 80c2 81c1 c984 8385 84c2 cbc2  ................
-00001b10: cac1 cc82 5882 6a00 ccff 00c2 cdc1 ccc1  ....X.j.........
-00001b20: d7c4 5882 c2cc c7cb c1d7 c458 82c2 cb00  ..X........X....
-00001b30: d4ff c800 c1d7 58c1 d7c1 c9c1 c8c1 c9c5  ......X.........
-00001b40: cac1 c8ff ffd0 ff00 f0ff c1c8 8483 c2ca  ................
-00001b50: 8483 c1cb c8ff c200 c1c7 c1c8 b5c1 c8c1  ................
-00001b60: cb82 5882 6ac9 00cc ffc3 0082 6ac2 8882  ..X.j.......j...
-00001b70: 6ac9 0082 6ac2 8882 6ac4 00d4 ffc3 0082  j...j...j.......
-00001b80: 6ac1 c7c1 cac1 cbc2 c9c1 c8c1 c984 83c1  j...............
-00001b90: cac1 c781 83c2 cacc ffc1 c9c2 8081 83c2  ................
-00001ba0: 84c1 cbc8 ffc1 c8c1 c981 c283 c1c9 8584  ................
-00001bb0: c4ca c1cc c1cb c1c8 826a c300 ccff c400  .........j......
-00001bc0: 6a82 c288 6a82 c900 6a82 c288 6a82 c300  j...j...j...j...
-00001bd0: d4ff c900 826a 58c1 d7c1 cbc1 cab5 c1ca  .....jX.........
-00001be0: c1c8 c200 ffff d0ff 00f0 ffc1 c7c1 c9c5  ................
-00001bf0: cac1 cbc8 ffc4 00c1 c7c1 c8c1 c982 6acb  ..............j.
-00001c00: 00fc ffc6 00c1 c6c1 c8c1 cbc1 d7c1 c8c1  ................
-00001c10: c9c1 c8c1 c9c1 ca80 c2ca c1cb c1ca ccff  ................
-00001c20: c1c9 c7ca c8ff c1c9 c1c8 c2c9 84c1 c9c1  ................
-00001c30: ca83 c2ca c2cb c1c9 c1c8 c600 fcff cb00  ................
-00001c40: 826a c1c9 c1ca c1c8 c400 ffff d0ff 00f0  .j..............
-00001c50: ffc1 c7b5 c1c9 c3ca b7c1 cbc8 ffd4 00fc  ................
-00001c60: ffc8 00c1 c858 c2d7 c2c9 c3ca 34c2 cacc  .....X......4...
-00001c70: ffc1 c9c2 cac2 34c3 cac8 ffc2 c943 c3c9  ......4......C..
-00001c80: c2ca c1cb 8258 c1c8 c800 fcff d400 ffff  .....X..........
-00001c90: d0ff 00f0 ff00 c1c7 c1c8 c1c9 c3ca 00c8  ................
-00001ca0: ffd4 00fc ffc9 0082 6a58 c1d7 c1c8 c1ca  ........jX......
-00001cb0: c1cb c2ca c1cb 00cc ffc4 c9c4 cac8 ffc2  ................
-00001cc0: 00c4 c9c1 ca82 5882 6ac9 00fc ffd4 00ff  ......X.j.......
-00001cd0: ffd0 ff00 ffff c1ff d400 fcff cb00 826a  ...............j
-00001ce0: c1c8 c2ca c1cb c300 ccff 58c5 c9c2 cbc8  ..........X.....
-00001cf0: ffc4 00c3 c982 6acb 00fc ffd4 00ff ffd0  ......j.........
-00001d00: ff00 ffff ffff ffff ffff ffff f8ff 00ff  ................
-00001d10: ffff ffff ffff ffff fff8 ff00 ffff ffff  ................
-00001d20: ffff ffff ffff f8ff 00d0 ffc7 d7e0 ffc2  ................
-00001d30: d7c1 ffc2 d7c1 ffc7 d7e5 ffc2 d7c1 ffc2  ................
-00001d40: d7c4 ffc8 d7e1 ffc3 d7c4 ffc4 d7c5 ffc3  ................
-00001d50: d7c3 ffc4 d7cc ffc5 d7c3 ffc4 d7c1 ffc3  ................
-00001d60: d7cb ffc3 d7d2 ffc1 d7c4 ffc4 d7ff fffa  ................
-00001d70: ff00 d1ff c2d7 c3ff c1d7 ceff c1d7 d1ff  ................
-00001d80: c2d7 c1ff c2d7 c2ff c2d7 c3ff c1d7 e5ff  ................
-00001d90: c2d7 c1ff c2d7 c4ff c1d7 c2ff c2d7 c2ff  ................
-00001da0: c1d7 e2ff c2d7 c3ff c2d7 c2ff c2d7 c3ff  ................
-00001db0: c2d7 c4ff c4d7 ccff c6d7 c2ff c4d7 c3ff  ................
-00001dc0: c2d7 ccff c2d7 d1ff c2d7 c3ff c4d7 ffff  ................
-00001dd0: fbff 00d1 ffc2 d7d2 ffc1 d7d1 ffc2 d7c1  ................
-00001de0: ffc2 d7c2 ffc2 d7e9 ffc2 d7c1 ffc2 d7c7  ................
-00001df0: ffc2 d7e5 ffc2 d7c3 ffc2 d7c2 ffc2 d7c2  ................
-00001e00: ffc2 d7c5 ffc1 d7cf ffc1 d7c3 ffc1 d7c3  ................
-00001e10: ffc1 d7c6 ffc2 d7cc ffc2 d7d0 ffc3 d7c3  ................
-00001e20: ffc1 d7ff fffe ff00 d1ff c2d7 c1ff c1d7  ................
-00001e30: c3ff c3d7 c3ff c4d7 c1ff c4d7 c1ff c3d7  ................
-00001e40: c2ff c3d7 c1ff c2d7 cbff c2d7 c1ff c1d7  ................
-00001e50: c2ff c3d7 c1ff c6d7 c2ff c3d7 c1ff c2d7  ................
-00001e60: c1ff c3d7 c3ff c4d7 c2ff c4d7 ceff c2d7  ................
-00001e70: c3ff c3d7 c1ff c2d7 c1ff c3d7 c2ff c3d7  ................
-00001e80: c1ff c2d7 c1ff c2d7 cdff c2d7 c3ff c2d7  ................
-00001e90: c2ff c2d7 c1ff c5d7 c3ff c4d7 d0ff c1d7  ................
-00001ea0: c3ff c4d7 c3ff c2d7 c1ff c8d7 c3ff c2d7  ................
-00001eb0: c1ff c2d7 cdff c3d7 c3ff c4d7 c4ff c5d7  ................
-00001ec0: c3ff c3d7 c3ff c4d7 c2ff c4d7 c2ff c3d7  ................
-00001ed0: c2ff c3d7 c1ff c2d7 c2ff c5d7 c2ff c3d7  ................
-00001ee0: c2ff c3d7 c1ff c2d7 c1ff c4d7 f8ff 00d1  ................
-00001ef0: ffc4 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
-00001f00: ffc1 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
-00001f10: ffc3 d7c1 ffc1 d7cb ffc4 d7c3 ffc3 d7c2  ................
-00001f20: ffc2 d7c1 ffc2 d7c2 ffc3 d7c1 ffc3 d7c1  ................
-00001f30: ffc2 d7c1 ffc2 d7c2 ffc1 d7c1 ffc2 d7c2  ................
-00001f40: ffc1 d7ce ffc2 d7c4 ffc3 d7c1 ffc3 d7c1  ................
-00001f50: ffc2 d7c2 ffc8 d7cd ffc2 d7c3 ffc2 d7c2  ................
-00001f60: ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc6 d7ce  ................
-00001f70: ffc1 d7c3 ffc6 d7c2 ffc2 d7c1 ffc1 d7c3  ................
-00001f80: ffc2 d7c1 ffc2 d7c2 ffc5 d7cc ffc1 d7c1  ................
-00001f90: ffc2 d7c2 ffc6 d7c4 ffc2 d7c1 ffc2 d7c1  ................
-00001fa0: ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc1 d7c1  ................
-00001fb0: ffc2 d7c2 ffc1 d7c1 ffc2 d7c1 ffc2 d7c2  ................
-00001fc0: ffc5 d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1  ................
-00001fd0: ffc2 d7c2 ffc3 d7c1 ffc3 d7c2 ffc1 d7f8  ................
-00001fe0: ff00 d1ff c2d7 c1ff c1d7 c2ff c2d7 c1ff  ................
-00001ff0: c2d7 c1ff c3d7 c4ff c2d7 c1ff c5d7 c2ff  ................
-00002000: c2d7 ceff c2d7 c1ff c1d7 c4ff c2d7 c2ff  ................
-00002010: c2d7 c1ff c2d7 c2ff c2d7 c3ff c5d7 c1ff  ................
-00002020: c3d7 c3ff c3d7 d0ff c2d7 c4ff c2d7 c6ff  ................
-00002030: c2d7 c2ff c2d7 c1ff c2d7 c1ff c2d7 cdff  ................
-00002040: c2d7 c4ff c5d7 c1ff c2d7 c2ff c2d7 c5ff  ................
-00002050: c2d7 ceff c1d7 c7ff c2d7 c2ff c4d7 c3ff  ................
-00002060: c2d7 c1ff c2d7 c2ff c2d7 c1ff c2d7 cbff  ................
-00002070: c1d7 c2ff c2d7 c6ff c2d7 c4ff c2d7 c1ff  ................
-00002080: c2d7 c4ff c2d7 c1ff c3d7 c3ff c3d7 c3ff  ................
-00002090: c5d7 c2ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
-000020a0: c2d7 c2ff c5d7 c2ff c2d7 c3ff c3d7 faff  ................
-000020b0: 00d1 ffc2 d7c4 ffc2 d7c1 ffc2 d7c3 ffc3  ................
-000020c0: d7c2 ffc2 d7c1 ffc2 d7c5 ffc2 d7ce ffc2  ................
-000020d0: d7c6 ffc3 d7c1 ffc2 d7c1 ffc2 d7c2 ffc2  ................
-000020e0: d7c3 ffc2 d7c6 ffc3 d7c3 ffc3 d7ce ffc2  ................
-000020f0: d7c4 ffc2 d7c4 ffc4 d7c2 ffc2 d7c1 ffc2  ................
-00002100: d7c1 ffc2 d7c4 ffc3 d7c6 ffc2 d7c6 ffc2  ................
-00002110: d7c2 ffc2 d7c2 ffc2 d7c6 ffc1 d7c4 ffc3  ................
-00002120: d7c7 ffc1 d7c8 ffc1 d7c2 ffc2 d7c1 ffc2  ................
-00002130: d7c2 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00002140: d7c4 ffc3 d7c4 ffc6 d7c6 ffc1 d7c4 ffc2  ................
-00002150: d7c1 ffc2 d7c2 ffc4 d7c3 ffc3 d7c3 ffc3  ................
-00002160: d7c1 ffc2 d7c5 ffc2 d7c1 ffc2 d7c2 ffc3  ................
-00002170: d7c3 ffc2 d7c5 ffc2 d7c5 ffc3 d7f8 ff00  ................
-00002180: d1ff c2d7 c4ff c2d7 c1ff c2d7 c1ff c1d7  ................
-00002190: c2ff c2d7 c2ff c2d7 c1ff c2d7 c2ff c1d7  ................
-000021a0: c2ff c2d7 ceff c2d7 c3ff c1d7 c1ff c1d7  ................
-000021b0: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c2d7  ................
-000021c0: c3ff c2d7 c2ff c1d7 c1ff c1d7 c2ff c2d7  ................
-000021d0: c1ff c1d7 c2ff c2d7 ceff c2d7 c4ff c2d7  ................
-000021e0: c3ff c2d7 c1ff c2d7 c2ff c2d7 c1ff c2d7  ................
-000021f0: c1ff c2d7 cdff c2d7 c5ff c2d7 c3ff c2d7  ................
-00002200: c2ff c2d7 c1ff c2d7 c2ff c1d7 ceff c1d7  ................
-00002210: c4ff c2d7 c2ff c1d7 c3ff c2d7 c2ff c2d7  ................
-00002220: c1ff c2d7 c1ff c2d7 c2ff c2d7 c1ff c2d7  ................
-00002230: ceff c2d7 c2ff c2d7 c2ff c1d7 c5ff c2d7  ................
-00002240: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c1d7  ................
-00002250: c2ff c2d7 c1ff c1d7 c2ff c2d7 c1ff c2d7  ................
-00002260: c2ff c1d7 c2ff c2d7 c1ff c2d7 c1ff c1d7  ................
-00002270: c6ff c2d7 c2ff c1d7 c2ff c2d7 c3ff c1d7  ................
-00002280: c2ff c2d7 f8ff 00d0 ffc4 d7c4 ffc3 d7c2  ................
-00002290: ffc4 d7c3 ffc3 d7c1 ffc3 d7c2 ffc4 d7cc  ................
-000022a0: ffc9 d7c1 ffc7 d7c2 ffc4 d7c3 ffc3 d7c2  ................
-000022b0: ffc4 d7c2 ffc4 d7ce ffc4 d7c2 ffc4 d7c3  ................
-000022c0: ffc8 d7c1 ffc2 d7c1 ffc3 d7cb ffc4 d7c2  ................
-000022d0: ffc3 d7c5 ffc4 d7c2 ffc4 d7cf ffc1 d7c4  ................
-000022e0: ffc4 d7c3 ffc4 d7c1 ffc7 d7c2 ffc3 d7c1  ................
-000022f0: ffc3 d7cd ffc2 d7c2 ffc4 d7c6 ffc4 d7c3  ................
-00002300: ffc9 d7c2 ffc4 d7c3 ffc3 d7c2 ffc3 d7c1  ................
-00002310: ffc8 d7c3 ffc3 d7c2 ffc4 d7c2 ffc4 d7f9  ................
-00002320: ff00 ffff cbff c2d7 ffff ffff ccff c2d7  ................
-00002330: e6ff c2d7 e3ff c6d7 ffff cbff 00ff ffcb  ................
-00002340: ffc2 d7ff ffff ffcc ffc2 d7e6 ffc2 d7e3  ................
-00002350: ffc1 d7c4 ffc1 d7ff ffcb ff00 ffff caff  ................
-00002360: c4d7 ffff ffff caff c4d7 e4ff c4d7 e3ff  ................
-00002370: c4d7 ffff ccff 00ff ffff ffff ffff ffff  ................
-00002380: fff8 ff00 ffff ffff ffff ffff ffff f8ff  ................
-00002390: 00ff ffff ffff ffff ffff fff8 ff00 ffff  ................
-000023a0: ffff ffff ffff ffff f8ff 00ff ffff ffff  ................
-000023b0: ffff ffff fff8 ff00 ffff ffff ffff ffff  ................
-000023c0: ffff f8ff 00ff ffff ffff ffff ffff fff8  ................
-000023d0: ff00 f0ff c800 c8ff d400 ccff ca00 c1f5  ................
-000023e0: d100 d4ff c600 c1f5 21cc 00cc ffc2 006a  ........!......j
-000023f0: 21c1 f584 c200 c8ff cc00 216a c600 ccff  !.........!j....
-00002400: d100 c1f5 ca00 d4ff d400 ffff d0ff 00f0  ................
-00002410: ffc8 00c8 ffc3 006a 21c6 00c1 cac1 cbc7  .......j!.......
-00002420: 00cc ffca 0021 88d0 00d4 ffc4 006a 21c1  .....!.......j!.
-00002430: d86a cc00 ccff 0084 0088 6a00 c1f5 00c8  .j........j.....
-00002440: ffcc 006a c1d8 21c1 f5c4 00cc ffd0 0088  ...j..!.........
-00002450: 21ca 00d4 ffc7 00c2 ccc6 0021 c1f5 c300  !..........!....
-00002460: ffff d0ff 00f0 ff00 c1ca c4cb c1cc 00c8  ................
-00002470: ffc4 00c1 d821 c1f5 00c1 c7c2 c9c2 cac1  .....!..........
-00002480: cbc1 ccc5 00cc ffca 006a c1d8 88cf 00d4  .........j......
-00002490: ffc5 00c1 d86a cd00 ccff 00c1 c7c1 c9c1  .....j..........
-000024a0: d86a c1ca c1c9 00c8 ffcd 006a c1d8 c500  .j.........j....
-000024b0: ccff cf00 88c1 d86a ca00 d4ff c500 c2cb  .......j........
-000024c0: c1cc c1cb c2cc c1cb 0021 6ac1 d8c4 00ff  .........!j.....
-000024d0: ffd0 ff00 f0ff c1c7 c1c9 c1ca c1c9 c2ca  ................
-000024e0: c1cc c1ca c8ff c400 c1d8 6ac1 c7c2 c9c2  ..........j.....
-000024f0: cac1 ccc1 cbc1 ccc1 cbc2 ccc3 00cc ffc2  ................
-00002500: 00ca c988 6acb c9c3 00d4 ffc2 00c1 cac1  ....j...........
-00002510: c9c1 d86a c1cb c2cc c1cb ca00 ccff c2c7  ...j............
-00002520: c1c9 88c1 d8c1 cac1 cbc1 c9c8 ffca 00c1  ................
-00002530: c7c2 c9c1 ca6a c1d8 c2cb c200 ccff c300  .....j..........
-00002540: cbc9 6a88 cac9 c200 d4ff c300 c2ca c1cb  ..j.............
-00002550: c1c9 c2ca c1cb c3cc c1cb 6ac1 d8c4 00ff  ..........j.....
-00002560: ffd0 ff00 f0ff c1c7 c2c9 c2ca c1cb c1cc  ................
-00002570: c1cb c8ff c300 c1d8 6ac2 c9c1 cac3 cbc3  ........j.......
-00002580: ccc1 cbc3 cac2 00cc ff00 c2ca c1cb c2ca  ................
-00002590: c1cb c2ca c1cb c36a c1ca c1c9 c1ca c3c9  .......j........
-000025a0: c1ca c3c9 c1ca c1c9 c1c7 c200 d4ff 00c2  ................
-000025b0: c9c1 cac1 c9c1 d86a c2cb c2cc c1cb c800  .......j........
-000025c0: ccff c1c7 c1c9 c1ca c1d8 6ac1 cbc1 ccc1  ..........j.....
-000025d0: cac8 ffc8 00c1 c7c2 c9c1 cac1 cb6a c1d8  .............j..
-000025e0: c3cc c1cb 00cc ffc2 00c1 c7c1 c9c1 cac3  ................
-000025f0: c9c1 cac3 c9c1 cac1 c9c1 cac3 6ac1 cbc2  ............j...
-00002600: cac1 cbc2 cac1 cbc2 ca00 d4ff c200 c5c9  ................
-00002610: c1ca c1c9 c1ca c2cb c3cc 6ac1 d8c3 00ff  ..........j.....
-00002620: ffd0 ff00 f0ff c1c7 c1c9 6a21 c1f5 84c1  ..........j!....
-00002630: ccc1 cbc8 ffc2 00c1 c7c1 c9c1 d86a c1c9  .............j..
-00002640: c1ca c1cb c3cc c1cb c1ca c1c9 c2ca 8081  ................
-00002650: 00cc ffc1 c9c1 ccc1 cbc1 ccc2 cbc1 ccc3  ................
-00002660: cbc1 d888 c3ca c3cb c1ca c1c9 c2cb c1ca  ................
-00002670: c1c9 c1ca 84c1 c700 d4ff c5c9 c1ca c1d8  ................
-00002680: c2ca c1cb c3cc c1cb c600 ccff c1c7 c1c9  ................
-00002690: c1ca c1c9 c2ca c1cc c1ca c8ff c600 c1c7  ................
-000026a0: c2c9 c2ca c1cc c1cb c1d8 c2cc c2cb c1cc  ................
-000026b0: c1cb ccff 00c2 c7c1 cac1 c9c1 cac2 cbc1  ................
-000026c0: c9c1 cac3 cbc3 ca88 c1d8 c3cb c1cc c2cb  ................
-000026d0: c1cc c1cb c2cc d4ff 00c2 80c2 c9c1 c7c3  ................
-000026e0: c9c1 cac1 cbc1 cac1 ccc1 cb6a c1d8 c1cc  ...........j....
-000026f0: c1cb c200 ffff d0ff 00f0 ffc1 c784 c1ca  ................
-00002700: 886a c1cc c1f5 c1cb c8ff 00c2 c9c1 cac1  .j..............
-00002710: c9c1 d8c1 cac3 ccc1 cbc1 cac1 c9c1 ca84  ................
-00002720: 83c1 ca81 8300 ccff c2c9 c1cc c1cb c2cc  ................
-00002730: c1cb c2cc c1cb c1cc c1cb c1cc c3cb c1cc  ................
-00002740: c3cb c1cc c4cb 8384 80d4 ff83 81c5 c9c1  ................
-00002750: cac1 c9c1 cac2 cbc3 ccc1 cbc4 00cc ffc1  ................
-00002760: c7c2 c9c2 cac1 cbc1 ccc1 cbc8 ffc4 00c1  ................
-00002770: c7c2 c9c1 cac3 cbc3 ccc1 cbc3 ca84 83cc  ................
-00002780: ffc3 80c4 cbc1 ccc3 cbc1 ccc3 cbc1 ccc1  ................
-00002790: cbc1 ccc1 cbc2 ccc1 cbc2 ccc1 cbc3 ccd4  ................
-000027a0: ff00 8081 c1c9 8381 c1c9 c1c7 c3c9 c1ca  ................
-000027b0: c2cb c1d8 c1cb c3cc 00ff ffd0 ff00 f0ff  ................
-000027c0: c1c7 c1c9 c1ca c1d8 6ac1 cac1 ccc1 cbc8  ........j.......
-000027d0: ffc1 c7c1 c8c1 cac1 c9c1 cac3 ccc1 cbc1  ................
-000027e0: cac1 c9c1 ca84 8385 84c1 ca83 c284 ccff  ................
-000027f0: c2c9 d7cc 8483 84d4 ff84 c283 81c1 c9c1  ................
-00002800: c7c3 c9c1 cac1 cbc1 cac1 ccc1 cbc3 ccc3  ................
-00002810: 00cc ffc1 c7c1 c9c1 cac1 c9c1 cac1 cbc1  ................
-00002820: ccc1 cbc8 ffc3 00c1 cac1 ccc1 cac1 c9c1  ................
-00002830: cac1 cbc3 ccc1 cbc1 cac1 c9c1 ca84 8385  ................
-00002840: 84cc ffc3 81d9 ccd4 ffc2 8183 c1c9 84c2  ................
-00002850: 8381 c1c9 c1c7 c3c9 c1ca c1cb c3cc c1cb  ................
-00002860: c1cc ffff d0ff 00f0 ffc1 c7c1 c9c1 ca88  ................
-00002870: c1d8 c2cc c1cb c8ff c1c9 c2c8 c1c7 c2cc  ................
-00002880: c1cb c1ca c1c9 c1ca 8483 8584 c4ca c1cb  ................
-00002890: c1ca ccff 8384 cccb c2ca c1cb c3ca c1cb  ................
-000028a0: c4ca 84c2 83d4 ffc1 c7c1 c984 c283 81c1  ................
-000028b0: c9c1 c7c3 c9c1 cac4 cbc1 ccc3 00cc ffc1  ................
-000028c0: c7c1 c9c2 cac1 cbc2 ccc1 cbc8 ffc2 00c1  ................
-000028d0: cac3 cbc4 ccc1 cbc1 cac1 c9c1 ca84 8385  ................
-000028e0: 84c2 cbcc ffc2 8381 c4ca c1cb c3ca c1cb  ................
-000028f0: c2ca cccb 8483 d4ff c2c8 c4c9 84c2 8381  ................
-00002900: c1c8 c1c7 c3c9 c1cb c1ca c3cb ffff d0ff  ................
-00002910: 00f0 ffc1 c7c1 c9c1 cbc1 d86a c2cc c1cb  ...........j....
-00002920: c8ff 8381 c1c9 c1c8 c1c7 c1cb c2ca 8483  ................
-00002930: 8584 c4ca c1c9 c1cb 82c1 d7cc ff84 8581  ................
-00002940: 8384 85c1 cb81 8384 85c1 cc81 8384 85c1  ................
-00002950: cb81 8384 c1cb 8183 8485 84c2 83d4 ffc2  ................
-00002960: c8c2 c984 c283 81c1 c9c1 c7c1 c9c3 cac1  ................
-00002970: cc80 8183 c200 ccff c1c7 c1c9 c1ca c1cb  ................
-00002980: c1cc c1ca c1cc c1cb c8ff c200 c3c7 c1cb  ................
-00002990: c3cc c1ca c1c9 c1ca 8483 8584 c2cb c1ca  ................
-000029a0: c1cb ccff c283 8185 8483 81c1 cb84 8381  ................
-000029b0: c1cb 8584 8381 c1cc 8584 8381 c1cb 8584  ................
-000029c0: 8381 8584 d4ff c1d7 82c1 c8c1 c9c1 c8c2  ................
-000029d0: c9c1 c884 c283 81c2 c9c4 ca83 81ff ffd0  ................
-000029e0: ff00 f0ff c1c7 c1c9 c2cb c3cc c1cb c8ff  ................
-000029f0: 8483 c3c9 c1c7 8483 8584 c4ca c2cc c1ca  ................
-00002a00: 826a 00cc ffc2 c983 8485 15c1 cc83 8485  .j..............
-00002a10: 15c1 cc83 8485 15c1 cc83 8485 c1cc 8384  ................
-00002a20: 8515 8083 84d4 ffc2 cac1 c8c3 c984 c283  ................
-00002a30: 81c2 c9c1 cac2 c781 8384 c200 ccff c1c7  ................
-00002a40: c1ca c4cb c1cc c1cb c8ff 00c2 c7c2 80c2  ................
-00002a50: 81c1 cbc1 cac1 cb84 8385 84c2 cbc2 cac2  ................
-00002a60: cccc ff84 8380 1585 8483 c1cc 8584 83c1  ................
-00002a70: cc15 8584 83c1 cc15 8584 83c1 cc15 8584  ................
-00002a80: 83c2 ccd4 ff00 82c1 d7c1 c7c2 cac4 c984  ................
-00002a90: c283 81c1 ca83 81c1 ca84 83ff ffd0 ff00  ................
-00002aa0: f0ff c2c7 c1c8 c1c9 c1ca c2cb c1cc c8ff  ................
-00002ab0: c1c7 c1c8 c1c9 8381 c1c7 8584 c4ca c1cc  ................
-00002ac0: c1cb c1c9 826a c300 ccff c1c9 c4ca c1cb  .....j..........
-00002ad0: c3ca c1cb c2ca cdcb c280 84d4 ffc2 c7c2  ................
-00002ae0: cac1 c8c2 c9c1 c884 83c1 c980 c2c7 8083  ................
-00002af0: c384 00cc ffc1 c9c3 cac4 cbc8 ff00 c280  ................
-00002b00: c281 c283 8480 c1ca 8584 c1c9 c3ca c1cb  ................
-00002b10: c1cc c1ca c1c9 ccff 84c2 80c4 cac1 cbc3  ................
-00002b20: cac1 cbc2 cacd cbc1 ccd4 ffc3 0082 c1d7  ................
-00002b30: c1c7 c1ca c1cb c4c9 8483 c1ca 8483 c2ca  ................
-00002b40: c1cb ffff d0ff 00f0 ffc1 c7c1 c8c1 c9c3  ................
-00002b50: cac2 cbc8 ffb5 c2c8 8483 c1c8 c3ca c1c9  ................
-00002b60: c2cb c1c9 c1c8 c600 ccff c1cb c1c9 d0ca  ................
-00002b70: c2cc c3ca c2cb c2ca 34d4 ff00 82c1 d782  ........4.......
-00002b80: c2ca c4c9 c1c8 8180 c1c7 81c4 8400 ccff  ................
-00002b90: c1c9 c2c7 8081 8384 c1cb c8ff 80c2 81c2  ................
-00002ba0: 83c2 8483 81c1 cac2 cbc2 cac1 ccc1 cb82  ................
-00002bb0: c1d7 6a00 ccff 43c2 cac1 c9d0 cac2 ccc3  ..j...C.........
-00002bc0: cac3 cbd4 ffc6 00c1 c7c1 c8c1 cbc1 c8c4  ................
-00002bd0: c9c5 cab5 ffff d0ff 00f0 ffc1 c883 81c2  ................
-00002be0: ca83 81c1 cbc8 ffc1 c7c3 c8c1 c9c1 c8c2  ................
-00002bf0: c9c2 cb82 c1d7 c800 ccff 00c1 cac7 c9c5  ................
-00002c00: cbc6 ccc1 cbc3 ccc1 cdc2 ca00 d4ff c300  ................
-00002c10: 82c1 d7c1 c7c1 cac1 cbc2 c9c1 c883 8180  ................
-00002c20: 83c5 84cc ffc2 c780 8183 c384 c8ff 81c2  ................
-00002c30: 83c4 8481 83c3 cac1 ccc1 cbc1 c8c1 d76a  ...............j
-00002c40: c300 ccff 00c3 cac7 c9c5 cbc6 ccc1 cbc3  ................
-00002c50: ccc1 cd00 d4ff c800 c1d7 82c1 c8c1 cbc2  ................
-00002c60: c9c5 cac1 c8ff ffd0 ff00 f0ff c1c8 8483  ................
-00002c70: c2ca 8483 c1cb c8ff c200 c1c7 c1c8 b5c1  ................
-00002c80: c8c2 cbc1 c982 6ac9 00cc ffc2 0082 6ac2  ......j.......j.
-00002c90: 8882 6aca c982 6ac2 8882 6ac2 c9c2 00d4  ..j...j...j.....
-00002ca0: ffc6 00c1 c6c1 c8c2 cbc2 c8c1 c9c2 81c3  ................
-00002cb0: 84c1 ca34 ccff c1c7 8081 83c4 84c8 ff43  ...4...........C
-00002cc0: c1c8 c484 83c3 cac2 cbc1 c9c1 c8c6 00cc  ................
-00002cd0: ffc2 00c2 c96a 82c2 886a 82ca c96a 82c2  .....j...j...j..
-00002ce0: 886a 82c2 00d4 ffc9 0082 c1d7 c1c8 c2cb  .j..............
-00002cf0: c1ca b5c1 cac1 c8c2 00ff ffd0 ff00 f0ff  ................
-00002d00: c1c7 c1c9 c5ca c1cb c8ff c400 c1c7 c1c8  ................
-00002d10: c1c9 82cc 00fc ffc8 00c1 c8c1 c9c1 c8c1  ................
-00002d20: cac2 c983 84c2 ca20 6acc ff80 8183 c584  ....... j.......
-00002d30: c8ff 586a c2c9 c284 c2ca c1cb c1ca c1c9  ..Xj............
-00002d40: c1c8 c800 fcff cb00 82c1 d7c1 c9c1 cac1  ................
-00002d50: c8c4 00ff ffd0 ff00 f0ff c1c7 b5c1 c9c3  ................
-00002d60: cab7 c1cb c8ff d400 fcff c900 82c1 d7c2  ................
-00002d70: cac1 c8c1 ca34 206a c200 ccff 8183 c684  .....4 j........
-00002d80: c8ff c200 586a 43c1 c9c1 cac1 cb82 c1d7  ....XjC.........
-00002d90: 6ac9 00fc ffd4 00ff ffd0 ff00 f0ff 00c1  j...............
-00002da0: c7c1 c8c1 c9c3 ca00 c8ff d400 fcff cb00  ................
-00002db0: 82c1 d7c1 c820 6ac4 00cc ffc1 c9c7 cac8  ..... j.........
-00002dc0: ffc4 0058 6ac1 c9c1 d76a cb00 fcff d400  ...Xj....j......
-00002dd0: ffff d0ff 00ff ffff fff2 ffc1 c943 c4ca  .............C..
-00002de0: 34c1 caff ffff fffd ff00 ffff ffff f2ff  4...............
-00002df0: 0058 6ac2 20c2 2800 ffff ffff fdff 00ff  .Xj. .(.........
-00002e00: ffff ffff ffff ffff fff8 ff00 ffff ffff  ................
-00002e10: ffff ffff ffff f8ff 00ff ffff ffff ffff  ................
-00002e20: ffff fff8 ff00 ffff ffff ffff ffff ffff  ................
-00002e30: f8ff 00ff ffff ffff ffff ffff fff8 ff00  ................
-00002e40: d1ff c7d7 e0ff c2d7 c1ff c2d7 c3ff c3d7  ................
-00002e50: c1ff c1d7 f5ff c2d7 c1ff c2d7 ccff c3d7  ................
-00002e60: c4ff c4d7 c3ff c4d7 c5ff c3d7 ccff c4d7  ................
-00002e70: c3ff c4d7 c2ff c3d7 cbff c3d7 d0ff c4d7  ................
-00002e80: c2ff c4d7 ffff ffff ccff 00d2 ffc2 d7c3  ................
-00002e90: ffc1 d7ce ffc1 d7d1 ffc2 d7c1 ffc2 d7c2  ................
-00002ea0: ffc2 d7c2 ffc2 d7dc ffc1 d7d8 ffc2 d7c1  ................
-00002eb0: ffc2 d7cd ffc2 d7c3 ffc2 d7c2 ffc2 d7c1  ................
-00002ec0: ffc2 d7c2 ffc2 d7c3 ffc2 d7cd ffc2 d7c2  ................
-00002ed0: ffc2 d7c1 ffc2 d7c2 ffc2 d7c2 ffc2 d7cc  ................
-00002ee0: ffc2 d7cf ffc4 d7c2 ffc2 d7c2 ffc2 d7ff  ................
-00002ef0: ffff ffcb ff00 d2ff c2d7 d2ff c1d7 d1ff  ................
-00002f00: c2d7 c1ff c2d7 c2ff c2d7 c3ff c1d7 dcff  ................
-00002f10: c1d7 d8ff c2d7 c1ff c2d7 cdff c2d7 c3ff  ................
-00002f20: c2d7 c2ff c2d7 c1ff c2d7 c2ff c2d7 c2ff  ................
-00002f30: c2d7 ceff c2d7 c2ff c2d7 c1ff c2d7 c2ff  ................
-00002f40: c2d7 c2ff c2d7 ccff c2d7 cfff c1d7 c5ff  ................
-00002f50: c2d7 c2ff c2d7 ffff ffff cbff 00d2 ffc2  ................
-00002f60: d7c1 ffc1 d7c3 ffc3 d7c3 ffc4 d7c1 ffc4  ................
-00002f70: d7c1 ffc3 d7c2 ffc3 d7c1 ffc2 d7cb ffc3  ................
-00002f80: d7c4 ffc3 d7c1 ffc7 d7c3 ffc3 d7c2 ffc3  ................
-00002f90: d7c1 ffc9 d7c1 ffc2 d7c1 ffc3 d7c2 ffc3  ................
-00002fa0: d7c1 ffc2 d7c1 ffc2 d7d4 ffc2 d7c3 ffc2  ................
-00002fb0: d7c2 ffc2 d7c1 ffc3 d7c1 ffc1 d7c2 ffc5  ................
-00002fc0: d7cc ffc3 d7c1 ffc1 d7c2 ffc2 d7c2 ffc2  ................
-00002fd0: d7c2 ffc2 d7c1 ffc8 d7c3 ffc2 d7c1 ffc2  ................
-00002fe0: d7cc ffc4 d7c2 ffc2 d7c2 ffc2 d7c3 ffc5  ................
-00002ff0: d7c3 ffc3 d7c3 ffc4 d7c2 ffc4 d7c2 ffc3  ................
-00003000: d7c2 ffc3 d7c1 ffc2 d7c2 ffc5 d7c2 ffc3  ................
-00003010: d7c2 ffc3 d7c1 ffc2 d7c1 ffc4 d7ff ffc9  ................
-00003020: ff00 d2ff c4d7 c2ff c2d7 c1ff c2d7 c1ff  ................
-00003030: c2d7 c2ff c1d7 c2ff c2d7 c1ff c2d7 c1ff  ................
-00003040: c2d7 c2ff c3d7 c1ff c1d7 cdff c3d7 c3ff  ................
-00003050: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
-00003060: c2d7 c1ff c2d7 c2ff c3d7 c1ff c1d7 c1ff  ................
-00003070: c2d7 c2ff c3d7 c1ff c3d7 c1ff c2d7 c2ff  ................
-00003080: c8d7 d4ff c2d7 c3ff c2d7 c2ff c2d7 c2ff  ................
-00003090: c4d7 c2ff c2d7 c2ff c2d7 ccff c4d7 c2ff  ................
-000030a0: c2d7 c2ff c2d7 c2ff c2d7 c1ff c1d7 c3ff  ................
-000030b0: c2d7 c1ff c2d7 c2ff c5d7 cbff c6d7 c1ff  ................
-000030c0: c2d7 c2ff c2d7 c4ff c2d7 c1ff c2d7 c1ff  ................
-000030d0: c2d7 c1ff c2d7 c1ff c2d7 c2ff c1d7 c1ff  ................
-000030e0: c2d7 c2ff c1d7 c1ff c2d7 c1ff c2d7 c2ff  ................
-000030f0: c5d7 c1ff c2d7 c1ff c2d7 c2ff c2d7 c1ff  ................
-00003100: c2d7 c2ff c3d7 c1ff c3d7 c2ff c1d7 ffff  ................
-00003110: c9ff 00d2 ffc2 d7c1 ffc1 d7c2 ffc2 d7c1  ................
-00003120: ffc2 d7c1 ffc3 d7c4 ffc2 d7c1 ffc5 d7c2  ................
-00003130: ffc2 d7d1 ffc3 d7c2 ffc2 d7c1 ffc2 d7c1  ................
-00003140: ffc2 d7c1 ffc2 d7c1 ffc5 d7c2 ffc2 d7c4  ................
-00003150: ffc2 d7c2 ffc2 d7c6 ffc2 d7c2 ffc2 d7c1  ................
-00003160: ffc2 d7c1 ffc2 d7d4 ffc2 d7c4 ffc5 d7c1  ................
-00003170: ffc2 d7c1 ffc3 d7c1 ffc2 d7c2 ffc2 d7cb  ................
-00003180: ffc2 d7c1 ffc3 d7c1 ffc2 d7c2 ffc2 d7c2  ................
-00003190: ffc4 d7c3 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1  ................
-000031a0: ffc2 d7cf ffc2 d7c1 ffc2 d7c2 ffc2 d7c4  ................
-000031b0: ffc2 d7c1 ffc2 d7c4 ffc2 d7c1 ffc3 d7c3  ................
-000031c0: ffc3 d7c3 ffc5 d7c2 ffc2 d7c1 ffc2 d7c1  ................
-000031d0: ffc2 d7c1 ffc2 d7c2 ffc5 d7c2 ffc2 d7c3  ................
-000031e0: ffc3 d7ff ffcb ff00 d2ff c2d7 c4ff c2d7  ................
-000031f0: c1ff c2d7 c3ff c3d7 c2ff c2d7 c1ff c2d7  ................
-00003200: c5ff c2d7 ceff c1d7 c3ff c2d7 c2ff c2d7  ................
-00003210: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
-00003220: c5ff c2d7 c4ff c2d7 c2ff c2d7 c4ff c4d7  ................
-00003230: c2ff c2d7 c1ff c2d7 c1ff c2d7 cbff c3d7  ................
-00003240: c6ff c2d7 c6ff c2d7 c2ff c2d7 c2ff c2d7  ................
-00003250: c1ff c2d7 c2ff c2d7 c4ff c3d7 c4ff c2d7  ................
-00003260: c2ff c2d7 c1ff c2d7 c2ff c2d7 c2ff c2d7  ................
-00003270: c1ff c2d7 c2ff c2d7 c1ff c2d7 c2ff c2d7  ................
-00003280: c1ff c2d7 c4ff c3d7 c9ff c1d7 c1ff c2d7  ................
-00003290: c2ff c2d7 c4ff c2d7 c1ff c2d7 c2ff c4d7  ................
-000032a0: c3ff c3d7 c3ff c3d7 c1ff c2d7 c5ff c2d7  ................
-000032b0: c1ff c2d7 c2ff c3d7 c3ff c2d7 c5ff c2d7  ................
-000032c0: c5ff c3d7 ffff c9ff 00d2 ffc2 d7c4 ffc2  ................
-000032d0: d7c1 ffc2 d7c1 ffc1 d7c2 ffc2 d7c2 ffc2  ................
-000032e0: d7c1 ffc2 d7c2 ffc1 d7c2 ffc2 d7ce ffc2  ................
-000032f0: d7c2 ffc2 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-00003300: d7c1 ffc2 d7c1 ffc2 d7c2 ffc1 d7c2 ffc2  ................
-00003310: d7c4 ffc2 d7c2 ffc2 d7c3 ffc2 d7c1 ffc2  ................
-00003320: d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7d4 ffc2  ................
-00003330: d7c5 ffc2 d7c3 ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00003340: d7c2 ffc2 d7cb ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00003350: d7c2 ffc2 d7c2 ffc2 d7c2 ffc2 d7c1 ffc2  ................
-00003360: d7c1 ffc2 d7c2 ffc2 d7c1 ffc2 d7cb ffc2  ................
-00003370: d7c2 ffc1 d7c2 ffc2 d7c2 ffc2 d7c4 ffc2  ................
-00003380: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc1  ................
-00003390: d7c2 ffc2 d7c1 ffc1 d7c2 ffc2 d7c1 ffc2  ................
-000033a0: d7c2 ffc1 d7c2 ffc2 d7c1 ffc2 d7c1 ffc1  ................
-000033b0: d7c6 ffc2 d7c2 ffc1 d7c2 ffc2 d7c3 ffc1  ................
-000033c0: d7c2 ffc2 d7ff ffc9 ff00 d1ff c4d7 c4ff  ................
-000033d0: c3d7 c2ff c4d7 c3ff c3d7 c1ff c3d7 c2ff  ................
-000033e0: c4d7 cdff c1d7 c1ff c3d7 c4ff c9d7 c3ff  ................
-000033f0: c3d7 c2ff c4d7 c3ff c7d7 c3ff c8d7 c1ff  ................
-00003400: c2d7 c1ff c3d7 d2ff c4d7 c2ff c3d7 c5ff  ................
-00003410: c4d7 c3ff c4d7 cdff c4d7 c3ff c4d7 c2ff  ................
-00003420: c4d7 c1ff c7d7 c2ff c3d7 c1ff c3d7 caff  ................
-00003430: c4d7 c4ff c4d7 c5ff c4d7 c3ff c9d7 c2ff  ................
-00003440: c4d7 c3ff c3d7 c2ff c3d7 c1ff c8d7 c3ff  ................
-00003450: c3d7 c2ff c4d7 c2ff c4d7 ffff caff 00ff  ................
-00003460: ffce ffc2 d7ff fff8 ffc2 d7e6 ffc2 d7e3  ................
-00003470: ffc6 d7ff ffdb ff00 ffff ceff c2d7 ffff  ................
-00003480: f8ff c2d7 e6ff c2d7 e3ff c1d7 c4ff c1d7  ................
-00003490: ffff dbff 00ff ffcd ffc4 d7ff fff6 ffc4  ................
-000034a0: d7e4 ffc4 d7e3 ffc4 d7ff ffdc ff00 ffff  ................
-000034b0: ffff ffff ffff ffff f8ff 00ff ffff ffff  ................
-000034c0: ffff ffff fff8 ff00 ffff ffff ffff ffff  ................
-000034d0: ffff f8ff 00ff ffff ffff ffff ffff fff8  ................
-000034e0: ff00 ffff ffff ffff ffff ffff f8ff 00ff  ................
-000034f0: ffff ffff ffff ffff fff8 ff00 ffff ffff  ................
-00003500: ffff ffff ffff f8ff 00ff ffff ffff ffff  ................
-00003510: ffff fff8 ff00 ffff ffff ffff ffff ffff  ................
-00003520: f8ff 00ff ffff ffff ffff ffff fff8 ff00  ................
-00003530: ffff ffff ffff ffff ffff f8ff 00ff ffff  ................
-00003540: ffff ffff ffff fff8 ff00 ffff ffff ffff  ................
-00003550: ffff ffff f8ff 00ff ffff ffff ffff ffff  ................
-00003560: fff8 ff00 ffff ffff ffff ffff ffff f8ff  ................
-00003570: 00ff ffff ffff ffff ffff fff8 ff00 0c00  ................
-00003580: 00ff ee00 eeef 00ef f000 f0f1 00f1 f200  ................
-00003590: f2f3 00f3 f400 f4f5 00f5 f600 f6a8 a8a8  ................
-000035a0: b8b8 b8c8 c8c8 d8d8 d8e8 e8e8 fcfc fc34  ...............4
-000035b0: 3c48 444c 5c58 6070 6c74 8484 8c98 9ca0  <HDL\X`plt......
-000035c0: acb0 b8c4 ccd0 dc30 2c04 403c 0c50 4c14  .......0,.@<.PL.
-000035d0: 605c 1c78 7840 9494 64b0 b084 cccc a864  `\.xx@..d......d
-000035e0: 6464 7474 7468 502c 7c68 4898 845c b8a0  ddttthP,|hH..\..
-000035f0: 78d4 bc94 f4dc b084 8484 5804 1070 1020  x.........X..p. 
-00003600: 8820 34a0 384c bc54 6ccc 687c dc84 90ec  . 4.8L.Tl.h|....
-00003610: 9ca4 fcbc c0fc d000 fce8 3cfc fc80 4c28  ..........<...L(
-00003620: 0060 3c08 7458 1c88 7438 9c88 50b0 9c6c  .`<.tX..t8..P..l
-00003630: c4b4 8844 1800 602c 0480 4408 9c60 10b8  ...D..`,..D..`..
-00003640: 7818 d49c 20e8 b810 fcd4 00fc f880 fcfc  x... ...........
-00003650: c020 0400 4014 0854 1c10 6c2c 1c80 3828  . ..@..T..l,..8(
-00003660: 9448 38a8 5c4c b86c 58c4 806c d494 8008  .H8.\L.lX..l....
-00003670: 3400 1040 0020 5004 3060 0440 700c 5484  4..@. P.0`.@p.T.
-00003680: 1468 941c 80a8 2c40 4040 2c44 203c 5830  .h....,@@@,D <X0
-00003690: 5068 3c68 7c4c 8094 5c98 b06c b4cc 7c10  Ph<h|L..\..l..|.
-000036a0: 3418 2048 2c38 6048 4c74 5860 886c 78a4  4. H,8`HLtX`.lx.
-000036b0: 8898 c0a8 b8dc c820 1800 381c 0050 5050  ....... ..8..PPP
-000036c0: 5834 0c68 4018 7c54 2c8c 6c40 a080 584c  X4.h@.|T,.l@..XL
-000036d0: 2810 6034 1874 4428 8854 38a4 6040 b870  (.`4.tD(.T8.`@.p
-000036e0: 50cc 8060 d494 70e0 a880 ecbc 9450 1c04  P..`..p......P..
-000036f0: 6428 1478 3828 8c4c 40a0 6460 b888 8824  d(.x8(.L@.d`...$
-00003700: 2844 3034 5440 4064 5050 7464 6488 8484  (D04T@@dPPtdd...
-00003710: a4ac acc0 d4d4 e030 3030 402c 9058 40ac  .......000@,.X@.
-00003720: 684c c478 58e0 8c68 fca0 88fc bca8 fc00  hL.xX..h........
-00003730: 186c 0024 8400 34a0 0048 b800 60d4 1878  .l.$..4..H..`..x
-00003740: dc38 90e8 58a8 f080 c4fc bce0 fc10 4060  .8..X.........@`
-00003750: 1850 6c28 6078 3470 8450 8ca0 74ac c09c  .Pl(`x4p.P..t...
-00003760: ccdc ccf0 fcac 3434 d434 34fc 3434 fc64  ......44.44.44.d
-00003770: 58fc 907c fcb8 a0fc d8c8 fcf4 ec48 1470  X..|.........H.p
-00003780: 5c2c 8c70 44a8 8c64 c4a8 88e0 c8b0 f8d0  \,.pD..d........
-00003790: b8ff e8d0 fc3c 0000 5c00 0080 0000 a000  .....<..\.......
-000037a0: 00c4 0000 e000 00fc 0000 fc50 00fc 6c00  ...........P..l.
-000037b0: fc88 00fc a400 fcc0 00fc dc00 fcfc 00cc  ................
-000037c0: 8808 e490 04fc 9c00 fcb0 30fc c464 fcd8  ..........0..d..
-000037d0: 9808 1858 0c24 6814 347c 1c44 8c28 5ca4  ...X.$h.4|.D.(\.
-000037e0: 3878 bc48 98d8 64ac e05c 9c34 6cb0 407c  8x.H..d..\.4l.@|
-000037f0: c84c 90e0 5ce0 f4fc c8ec f8b4 dcec 84bc  .L..\...........
-00003800: d858 98ac 1010 1020 2020 2044 7024 4874  .X.....    Dp$Ht
-00003810: 284c 782c 507c 3054 8048 6490 6484 a8d8  (Lx,P|0T.Hd.d...
-00003820: f4fc 6080 a444 608c 4c18 086c 2c18 9048  ..`..D`.L..l,..H
-00003830: 34b0 6c54 d292 7efc 3c00 fc54 00fc 6800  4.lT..~.<..T..h.
-00003840: fc7c 00fc 9400 fcac 00fc c400 4000 00ff  .|..........@...
-00003850: 0000 3030 0040 4000 5050 00ff ff00 9494  ..00.@@.PP......
-00003860: 94f7 00f7 f800 f8f9 00f9 fa00 fafb 00fb  ................
-00003870: fc00 fcfd 00fd fe00 feff 00ff ffff ff    ...............
+00000080: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+00000090: ffff ffff ffff f8ff ffff ffff ffff ffff  ................
+000000a0: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+000000b0: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+000000c0: ffff ffff ffff f8ff ffff ffff ffff ffff  ................
+000000d0: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+000000e0: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+000000f0: ffff ffff ffff f8ff f0ff c800 c8ff d400  ................
+00000100: ccff c400 6ac1 d8d6 00d4 ffc3 006a d000  ....j........j..
+00000110: ccff c300 6ac4 00c8 ffd0 006a c300 ccff  ....j......j....
+00000120: d700 c1d8 6ac3 00d4 ffd4 00ff ffd0 fff0  ....j...........
+00000130: ffc2 0058 c1d8 8858 c200 c8ff d400 ccff  ...X...X........
+00000140: c600 c2d8 d400 d4ff c400 c1d8 cf00 ccff  ................
+00000150: c200 58c1 d888 58c2 00c8 ffcf 00c1 d8c4  ..X...X.........
+00000160: 00cc ffd5 00c2 d8c5 00d4 ffc3 00c2 8858  ...............X
+00000170: c3d8 cb00 ffff d0ff f0ff 0088 58c2 8858  ............X..X
+00000180: 6a00 c8ff d400 ccff c800 c2d8 d200 d4ff  j...............
+00000190: c500 c1d8 ce00 ccff 0088 58c1 d888 586a  ..........X...Xj
+000001a0: 00c8 ffce 00c1 d8c5 00cc ffd3 00c2 d8c7  ................
+000001b0: 00d4 ff00 6a58 83c1 d8c2 88c1 d858 c2d8  ....jX.......X..
+000001c0: c900 ffff d0ff f0ff c588 586a 58c8 ffcb  ..........XjX...
+000001d0: 00c3 d858 c288 c300 ccff c400 d5d8 c300  ...X............
+000001e0: d4ff c300 c288 58c1 d8c2 6acb 00cc ffc3  ......X...j.....
+000001f0: 88c1 d888 586a 58c8 ffcb 00c3 d858 c288  ....XjX......X..
+00000200: c300 ccff c300 d5d8 c400 d4ff c288 c358  ...............X
+00000210: 83c1 d8c2 88c2 58c2 d8c7 00ff ffd0 fff0  ......X.........
+00000220: ffc1 d888 58c3 886a 58c8 ffc9 00c2 d858  ....X..jX......X
+00000230: c1d8 c288 c1d8 83c2 5800 ccff c200 c2d8  ........X.......
+00000240: 88c1 d888 c2d8 88c3 d888 c1d8 c288 c1d8  ................
+00000250: c488 5888 c3d8 00d4 ff00 c1d8 5883 c1d8  ..X.........X...
+00000260: c288 c1d8 58c2 6ac9 00cc ffc1 d888 58c1  ....X.j.......X.
+00000270: d8c2 886a 58c8 ffc9 00c2 d858 c1d8 c288  ...jX......X....
+00000280: c1d8 83c2 5800 ccff 00c2 d888 c1d8 88c2  ....X...........
+00000290: d888 c3d8 88c1 d8c2 88c1 d8c4 8858 88c3  .............X..
+000002a0: d8c2 00d4 ffc2 88c2 6ac3 5883 c1d8 c288  ........j.X.....
+000002b0: c258 c6d8 6aff ffd0 fff0 ffc1 d888 58c1  .X..j.........X.
+000002c0: d8c2 886a 58c8 ffc7 00c2 d8c2 58c2 88c1  ...jX.......X...
+000002d0: d883 c358 c26a ccff 00c4 d888 c1d8 c288  ...X.j..........
+000002e0: c1d8 88c3 5888 c358 c288 586a 58c1 d888  ....X..X..XjX...
+000002f0: c3d8 d4ff c288 c358 83c1 d8c2 88c2 58c2  .......X......X.
+00000300: 6ac7 00cc ffc1 d888 58c1 d8c2 886a 58c8  j.......X....jX.
+00000310: ffc7 00c2 d8c2 58c2 88c1 d883 c358 c26a  ......X......X.j
+00000320: ccff c4d8 88c1 d8c2 88c1 d888 c358 88c3  .............X..
+00000330: 58c2 8858 6a58 c1d8 88c3 d800 d4ff 8315  X..XjX..........
+00000340: c288 c26a c358 83c1 d8c2 88c2 58c2 d8c3  ...j.X......X...
+00000350: 00ff ffd0 fff0 ffc1 d888 c258 c288 6a58  ...........X..jX
+00000360: c8ff 6ac6 d8c2 58c2 88c1 d883 c358 c26a  ..j...X......X.j
+00000370: c288 ccff 00c1 d888 c1d8 c1c9 8483 c1c9  ................
+00000380: 8483 c1c9 8483 c1c9 8483 c1c9 8483 c1cb  ................
+00000390: 8483 c1cb 8483 c1cb 88c1 d8d4 ffc2 88c1  ................
+000003a0: d86a c358 83c1 d8c2 88c2 58c2 6ac5 00cc  .j.X......X.j...
+000003b0: ffc1 d888 c258 c288 6a58 c8ff c500 c2d8  .....X..jX......
+000003c0: c258 c288 c1d8 83c3 58c2 6ac2 88cc ffc1  .X......X.j.....
+000003d0: d888 c1d8 c1c9 8483 c1c9 8483 c1c9 8483  ................
+000003e0: c1c9 8483 c1c9 8483 c1cb 8483 c1cb 8483  ................
+000003f0: c1cb 88c1 d800 d4ff 840c 8315 c288 c26a  ...............j
+00000400: c358 83c1 d8c2 88c2 58c1 d8c2 00ff ffd0  .X......X.......
+00000410: fff0 ffc1 d888 58c3 886a 58c8 ffc3 00c2  ......X..jX.....
+00000420: d8c2 58c2 88c1 d883 c358 c26a c288 0d85  ..X......X.j....
+00000430: ccff 00c2 d888 c858 6ac3 586a 586a 586a  .......Xj.XjXjXj
+00000440: 586a c258 88c2 d8d4 ff83 15c2 88c1 d86a  Xj.X...........j
+00000450: c358 83c1 d8c2 88c2 58c2 6ac3 00cc ffc1  .X......X.j.....
+00000460: d888 58c3 886a 58c8 ffc3 00c2 d8c2 58c2  ..X..jX.......X.
+00000470: 88c1 d883 c358 c26a c288 0d85 ccff c2d8  .....X.j........
+00000480: 88c8 586a c358 6a58 6a58 6a58 6ac2 5888  ..Xj.XjXjXjXj.X.
+00000490: c2d8 00d4 ffc2 c884 0c83 15c2 88c2 6ac3  ..............j.
+000004a0: 5883 c1d8 88c2 5888 00ff ffd0 fff0 ffc1  X.....X.........
+000004b0: d888 c258 c1d8 886a 58c8 ffc2 00c1 d8c2  ...X...jX.......
+000004c0: 58c2 88c1 d883 c358 c26a c288 0d85 0c15  X......X.j......
+000004d0: ccff 0081 88d2 6ac2 20c3 6a88 81d4 ff84  ......j. .j.....
+000004e0: 0c83 15c2 88c1 d86a c358 83c1 d8c2 88c2  .......j.X......
+000004f0: 586a c200 ccff c1d8 88c2 58c2 886a 58c8  Xj........X..jX.
+00000500: ffc2 00c1 d8c2 58c2 88c1 d883 c358 c26a  ......X......X.j
+00000510: c288 0d85 0c15 ccff 8188 d26a c220 c36a  ...........j. .j
+00000520: 8881 00d4 ffc1 c8c1 d7c2 c984 0c83 15c2  ................
+00000530: 88c2 6ac3 58c5 88ff ffd0 fff0 ffc1 d888  ..j.X...........
+00000540: 5888 c1d8 886a 58c8 ff00 88c2 5888 c1d8  X....jX.....X...
+00000550: 83c3 58c2 6ac2 880d 850c 15c2 cbcc ff00  ..X.j...........
+00000560: 8084 830d 8584 830d 8584 830d 8584 830d  ................
+00000570: 8584 830d 8584 830d 84c2 83d4 ffc2 c884  ................
+00000580: 0c83 15c2 88c1 d86a c358 83c1 d888 c258  .......j.X.....X
+00000590: 8800 ccff c1d8 8858 c388 6a58 c8ff 0088  .......X..jX....
+000005a0: c258 88c1 d883 c358 c26a c288 0d85 0c15  .X.....X.j......
+000005b0: c2cb ccff 8084 830d 8584 830d 8584 830d  ................
+000005c0: 8584 830d 8584 830d 8584 830d 84c2 8300  ................
+000005d0: d4ff c1d7 58c1 d7c1 c9c1 c8c1 c984 0c83  ....X...........
+000005e0: 15c4 8858 c3ca c1cb 81ff ffd0 fff0 ffc1  ...X............
+000005f0: d888 c258 c1d8 886a 58c8 ffc5 88c3 58c2  ...X...jX.....X.
+00000600: 6ac2 880d 850c 15c2 cbc1 cac1 cbcc ff00  j...............
+00000610: c1ca 8584 0c15 8584 0c15 8584 0c15 8584  ................
+00000620: 0c15 8584 0c15 8584 0c85 84c1 ccd4 ffc1  ................
+00000630: c8c1 d7c2 c984 0c83 15c2 88c1 d86a c358  .............j.X
+00000640: c588 ccff c1d8 88c2 58c2 886a 58c8 ffc5  ........X..jX...
+00000650: 88c3 58c2 6ac2 880d 850c 15c2 cbc1 cac1  ..X.j...........
+00000660: cbcc ffc1 ca85 840c 1585 840c 1585 840c  ................
+00000670: 1585 840c 1585 840c 1585 840c 8584 c1cc  ................
+00000680: 00d4 ff00 826a 58c1 d7c1 cac2 c984 0c83  .....jX.........
+00000690: 15c2 88c1 cac2 cb81 c283 ffff d0ff f0ff  ................
+000006a0: c1d8 88c2 58c1 d888 6a58 c8ff c1d8 80c1  ....X...jX......
+000006b0: c988 c258 c26a c288 0d85 0c15 c2cb c1ca  ...X.j..........
+000006c0: 8258 c1c9 ccff 00c1 c9d9 cbc1 ccd4 ffc1  .X..............
+000006d0: d758 c1d7 c1c9 c1c8 c1c9 840c 8315 c488  .X..............
+000006e0: c258 88c1 cb83 c1cb ccff c1d8 88c2 58c2  .X............X.
+000006f0: 886a 58c8 ffc1 d880 c1c9 88c2 58c2 6ac2  .jX.........X.j.
+00000700: 880d 850c 15c2 cbc1 ca82 58c1 c9cc ffc1  ..........X.....
+00000710: c9d9 cbc1 cc00 d4ff c300 826a c1c7 c1ca  ...........j....
+00000720: c1cb c2c9 840c 8315 8381 c283 84c1 cbff  ................
+00000730: ffd0 fff0 ffc1 d881 c258 c1d8 886a 58c8  .........X...jX.
+00000740: ffc1 d8c3 80c1 c958 c288 0d85 0c15 c1cb  .......X........
+00000750: c1ca c1cc 8258 826a 00cc ff00 c1c9 c6cb  .....X.j........
+00000760: c1c9 cbca c3cb c2ca c3cb d4ff 0082 6a58  ..............jX
+00000770: c1d7 c1ca c2c9 840c 8315 c1d8 8858 c1cb  .............X..
+00000780: 8083 8083 ccff c1d8 81c2 58c2 886a 58c8  ..........X..jX.
+00000790: ffc1 d8c3 80c1 c958 c288 0d85 0c15 c1cb  .......X........
+000007a0: c1ca c1cc 8258 826a 00cc ffc1 c9c6 cbc1  .....X.j........
+000007b0: c9cb cac3 cbc2 cac3 cb00 d4ff c600 c1c7  ................
+000007c0: c1c8 c1cb c1d7 c2c9 840c 8483 84c2 cac1  ................
+000007d0: cbff ffd0 fff0 ffc1 d881 c288 c1d8 88c2  ................
+000007e0: 58c8 ffc1 d8c2 80c2 81c1 cc0d 850c 15c2  X...............
+000007f0: cbc1 ccc1 cbc1 c882 6ac3 00cc ffc2 00c2  ........j.......
+00000800: cb82 c458 c1d7 c7cb c2cc 82c4 58c1 d7c1  ...X........X...
+00000810: ccc1 cd00 d4ff c300 826a c1c7 c1ca c1cb  .........j......
+00000820: c2c9 840c 8315 c1cc c281 8380 c1cb ccff  ................
+00000830: c1d8 81c4 88c2 58c8 ffc1 d8c2 80c2 81c1  ......X.........
+00000840: cc0d 850c 15c2 cbc1 ccc1 cbc1 c882 6ac3  ..............j.
+00000850: 00cc ff00 c2cb 82c4 58c1 d7c7 cbc2 cc82  ........X.......
+00000860: c458 c1d7 c1cc c1cd c200 d4ff c800 c1d7  .X..............
+00000870: 58c1 d7c1 cbc2 c9c3 cab5 c1ca c1c8 ffff  X...............
+00000880: d0ff f0ff c1c9 c381 6a81 c2cb c8ff c1ca  ........j.......
+00000890: c1c9 81c2 83c1 cb0c 15c1 cbc1 cac2 cbc1  ................
+000008a0: c9c1 c8c6 00cc ffc4 0082 6ac2 8882 6ac9  ..........j...j.
+000008b0: 0082 6ac2 8882 6ac3 00d4 ffc6 00c1 c7c1  ..j...j.........
+000008c0: c8c1 cbc1 d7c2 c984 0cc1 cbc2 8381 c1c9  ................
+000008d0: c1ca ccff c1c9 c381 8081 c2cb c8ff c1ca  ................
+000008e0: c1c9 81c2 83c1 cb0c 15c1 cbc1 cac2 cbc1  ................
+000008f0: c9c1 c8c6 00cc ffc3 0082 6ac2 8882 6ac9  ..........j...j.
+00000900: 0082 6ac2 8882 6ac4 00d4 ffc9 0082 6a58  ..j...j.......jX
+00000910: c1d7 c1cb c1ca c1cb c1ca c1c8 c200 ffff  ................
+00000920: d0ff f0ff c1c9 c281 80c1 d883 84c1 cbc8  ................
+00000930: ff58 c1c8 b5c1 c984 c1c9 c2ca c1cb 8258  .X.............X
+00000940: c1c8 c800 fcff c800 c1d7 58c1 d7c1 cbc3  ..........X.....
+00000950: c984 c1c9 34c1 c858 ccff c1c9 c281 8081  ....4..X........
+00000960: 8384 c1cb c8ff 58c1 c843 c1c9 84c1 c9c2  ......X..C......
+00000970: cac1 cb82 58c1 c8c8 00fc ffcb 0082 6ac1  ....X.........j.
+00000980: c9c1 cac1 c8c4 00ff ffd0 fff0 ffc1 cac2  ................
+00000990: 8081 83c2 84c1 cbc8 ffc2 0058 6ac1 cac1  ...........Xj...
+000009a0: c9c1 cb82 5882 6ac9 00fc ffc9 0082 6a58  ....X.j.......jX
+000009b0: c1d7 c1cb c1c9 c1ca 6a58 c200 ccff c1ca  ........jX......
+000009c0: c280 8183 c284 c1cb c8ff c200 586a c1ca  ............Xj..
+000009d0: c1c9 c1cb 8258 826a c900 fcff d400 ffff  .....X.j........
+000009e0: d0ff f0ff c4c9 c1ca c2c9 c1ca c8ff c400  ................
+000009f0: 586a c1c9 826a cb00 fcff cb00 826a c1c9  Xj...j.......j..
+00000a00: 6a58 c400 ccff c3c9 c234 c2c9 c1ca c8ff  jX.......4......
+00000a10: c400 586a c1c9 826a cb00 fcff d400 ffff  ..Xj...j........
+00000a20: d0ff f0ff c3c9 c2b5 c3ca ffff f9ff c4c9  ................
+00000a30: c4ca ffff ffff fdff f0ff 00c6 ca00 ffff  ................
+00000a40: f9ff c258 6ac2 20c2 28c1 f5ff ffff fffd  ...Xj. .(.......
+00000a50: fff0 ffc8 00ff fff9 ff00 c658 00ff ffff  ...........X....
+00000a60: fffd ffff ffff ffff ffff ffff fff8 ffff  ................
+00000a70: ffff ffff ffff ffff fff8 ffff ffff ffff  ................
+00000a80: ffff ffff fff8 ffff ffff ffff ffff ffff  ................
+00000a90: fff8 ffff ffff ffff ffff ffff fff8 ffff  ................
+00000aa0: ffff ffff ffff ffff fff8 ffd1 ffc4 d7c1  ................
+00000ab0: ffc4 d7d4 ffc3 d7cd ffc3 d7c5 ffc2 d7c1  ................
+00000ac0: ffc2 d7c1 ffc4 d7e3 ffc3 d7d2 ffc2 d7c1  ................
+00000ad0: ffc2 d7c4 ffc8 d7e1 ffc3 d7c4 ffc4 d7c6  ................
+00000ae0: ffc1 d7c3 ffc4 d7cf ffc3 d7c2 ffc4 d7c2  ................
+00000af0: ffc3 d7cb ffc3 d7d2 ffc1 d7c3 ffc4 d7ff  ................
+00000b00: ffdc ffd2 ffc2 d7c3 ffc2 d7d4 ffc2 d7c1  ................
+00000b10: ffc2 d7cd ffc2 d7c5 ffc2 d7c1 ffc2 d7c2  ................
+00000b20: ffc2 d7ca ffc1 d7da ffc2 d7d2 ffc2 d7c1  ................
+00000b30: ffc2 d7c4 ffc1 d7c2 ffc2 d7c2 ffc1 d7e2  ................
+00000b40: ffc2 d7c3 ffc2 d7c2 ffc2 d7c4 ffc2 d7c2  ................
+00000b50: ffc2 d7c2 ffc2 d7cd ffc2 d7c3 ffc2 d7c2  ................
+00000b60: ffc2 d7c2 ffc2 d7cc ffc2 d7d1 ffc2 d7c2  ................
+00000b70: ffc2 d7c2 ffc2 d7ff ffdb ffd2 ffc2 d7c3  ................
+00000b80: ffc2 d7d4 ffc2 d7d0 ffc2 d7c5 ffc2 d7c1  ................
+00000b90: ffc2 d7c2 ffc2 d7ca ffc1 d7da ffc2 d7d2  ................
+00000ba0: ffc2 d7c1 ffc2 d7c7 ffc2 d7e5 ffc2 d7c3  ................
+00000bb0: ffc2 d7c2 ffc2 d7c3 ffc3 d7c2 ffc2 d7c2  ................
+00000bc0: ffc2 d7cc ffc2 d7c4 ffc2 d7c2 ffc2 d7c2  ................
+00000bd0: ffc2 d7cc ffc2 d7d0 ffc3 d7c2 ffc2 d7c2  ................
+00000be0: ffc2 d7ff ffdb ffd2 ffc2 d7c3 ffc2 d7c2  ................
+00000bf0: ffc3 d7c2 ffc3 d7c1 ffc2 d7c1 ffc3 d7c2  ................
+00000c00: ffc4 d7c1 ffc3 d7c2 ffc3 d7c1 ffc2 d7c1  ................
+00000c10: ffc4 d7cc ffc2 d7c1 ffc3 d7c1 ffc2 d7c1  ................
+00000c20: ffc4 d7c1 ffc3 d7c2 ffc3 d7c1 ffc5 d7c1  ................
+00000c30: ffc2 d7c1 ffc3 d7c1 ffc6 d7c3 ffc3 d7c2  ................
+00000c40: ffc3 d7c1 ffc2 d7ce ffc2 d7c3 ffc3 d7c1  ................
+00000c50: ffc2 d7c1 ffc3 d7c2 ffc3 d7c1 ffc2 d7c1  ................
+00000c60: ffc2 d7cd ffc2 d7c3 ffc2 d7c2 ffc2 d7c3  ................
+00000c70: ffc3 d7c2 ffc2 d7c2 ffc2 d7cb ffc5 d7c2  ................
+00000c80: ffc2 d7c2 ffc2 d7c2 ffc2 d7c1 ffc8 d7c3  ................
+00000c90: ffc2 d7c1 ffc2 d7cd ffc3 d7c2 ffc2 d7c2  ................
+00000ca0: ffc2 d7c3 ffc5 d7c3 ffc3 d7c3 ffc4 d7c2  ................
+00000cb0: ffc4 d7c2 ffc3 d7c2 ffc3 d7c1 ffc2 d7c2  ................
+00000cc0: ffc5 d7c2 ffc3 d7c2 ffc3 d7c1 ffc2 d7c1  ................
+00000cd0: ffc4 d7d9 ffd2 ffc7 d7c1 ffc2 d7c1 ffc2  ................
+00000ce0: d7c2 ffc3 d7c1 ffc3 d7c1 ffc2 d7c2 ffc2  ................
+00000cf0: d7c1 ffc2 d7c1 ffc2 d7c2 ffc3 d7c1 ffc3  ................
+00000d00: d7c1 ffc2 d7cc ffc2 d7c2 ffc5 d7c2 ffc2  ................
+00000d10: d7c1 ffc2 d7c1 ffc2 d7c2 ffc3 d7c1 ffc1  ................
+00000d20: d7c1 ffc2 d7c1 ffc2 d7c2 ffc3 d7c1 ffc3  ................
+00000d30: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc5  ................
+00000d40: d7ce ffc2 d7c4 ffc3 d7c1 ffc3 d7c1 ffc2  ................
+00000d50: d7c2 ffc8 d7cd ffc2 d7c3 ffc2 d7c2 ffc2  ................
+00000d60: d7c2 ffc1 d7c1 ffc2 d7c2 ffc2 d7c2 ffc2  ................
+00000d70: d7cb ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc2  ................
+00000d80: d7c2 ffc2 d7c1 ffc1 d7c3 ffc2 d7c1 ffc2  ................
+00000d90: d7c2 ffc5 d7cc ffc1 d7c1 ffc2 d7c2 ffc2  ................
+00000da0: d7c2 ffc2 d7c4 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+00000db0: d7c1 ffc2 d7c1 ffc2 d7c2 ffc1 d7c1 ffc2  ................
+00000dc0: d7c2 ffc1 d7c1 ffc2 d7c1 ffc2 d7c2 ffc5  ................
+00000dd0: d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00000de0: d7c2 ffc3 d7c1 ffc3 d7c2 ffc1 d7d9 ffd2  ................
+00000df0: ffc2 d7c3 ffc2 d7c1 ffc5 d7c2 ffc2 d7c3  ................
+00000e00: ffc5 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
+00000e10: ffc2 d7c3 ffc2 d7c1 ffc2 d7cc ffc2 d7c2  ................
+00000e20: ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc5 d7c2  ................
+00000e30: ffc2 d7c4 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3  ................
+00000e40: ffc2 d7c1 ffc2 d7c4 ffc2 d7c2 ffc2 d7c1  ................
+00000e50: ffc2 d7ce ffc2 d7c4 ffc2 d7c6 ffc2 d7c2  ................
+00000e60: ffc2 d7c1 ffc2 d7c1 ffc2 d7cd ffc2 d7c4  ................
+00000e70: ffc5 d7c1 ffc1 d7c2 ffc2 d7c2 ffc2 d7c2  ................
+00000e80: ffc2 d7cb ffc2 d7c2 ffc2 d7c1 ffc2 d7c2  ................
+00000e90: ffc2 d7c2 ffc4 d7c3 ffc2 d7c1 ffc2 d7c2  ................
+00000ea0: ffc2 d7c1 ffc2 d7cb ffc1 d7c2 ffc2 d7c2  ................
+00000eb0: ffc2 d7c2 ffc2 d7c4 ffc2 d7c1 ffc2 d7c4  ................
+00000ec0: ffc2 d7c1 ffc3 d7c3 ffc3 d7c3 ffc5 d7c2  ................
+00000ed0: ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
+00000ee0: ffc5 d7c2 ffc2 d7c3 ffc3 d7db ffd2 ffc2  ................
+00000ef0: d7c3 ffc2 d7c1 ffc2 d7c5 ffc2 d7c3 ffc2  ................
+00000f00: d7c5 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc2  ................
+00000f10: d7c3 ffc2 d7c1 ffc2 d7cc ffc2 d7c2 ffc2  ................
+00000f20: d7c1 ffc2 d7c2 ffc2 d7c1 ffc2 d7c5 ffc2  ................
+00000f30: d7c4 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2  ................
+00000f40: d7c1 ffc2 d7c2 ffc4 d7c2 ffc2 d7c1 ffc2  ................
+00000f50: d7ce ffc2 d7c4 ffc2 d7c4 ffc4 d7c2 ffc2  ................
+00000f60: d7c1 ffc2 d7c1 ffc2 d7c4 ffc3 d7c6 ffc2  ................
+00000f70: d7c6 ffc2 d7c2 ffc6 d7c1 ffc2 d7c2 ffc2  ................
+00000f80: d7c4 ffc3 d7c4 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00000f90: d7c2 ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc2  ................
+00000fa0: d7c1 ffc2 d7c2 ffc2 d7c1 ffc2 d7c4 ffc3  ................
+00000fb0: d7c4 ffc6 d7c1 ffc2 d7c2 ffc2 d7c4 ffc2  ................
+00000fc0: d7c1 ffc2 d7c2 ffc4 d7c3 ffc3 d7c3 ffc3  ................
+00000fd0: d7c1 ffc2 d7c5 ffc2 d7c1 ffc2 d7c2 ffc3  ................
+00000fe0: d7c3 ffc2 d7c5 ffc2 d7c5 ffc3 d7d9 ffd2  ................
+00000ff0: ffc2 d7c3 ffc2 d7c1 ffc2 d7c2 ffc1 d7c2  ................
+00001000: ffc2 d7c3 ffc2 d7c2 ffc1 d7c2 ffc2 d7c1  ................
+00001010: ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2 d7c1  ................
+00001020: ffc2 d7cc ffc2 d7c2 ffc2 d7c1 ffc2 d7c2  ................
+00001030: ffc2 d7c1 ffc2 d7c2 ffc1 d7c2 ffc2 d7c4  ................
+00001040: ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2 d7c1  ................
+00001050: ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1  ................
+00001060: ffc2 d7ce ffc2 d7c4 ffc2 d7c3 ffc2 d7c1  ................
+00001070: ffc2 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7cd  ................
+00001080: ffc2 d7c5 ffc2 d7c6 ffc2 d7c2 ffc2 d7c2  ................
+00001090: ffc2 d7cb ffc2 d7c2 ffc2 d7c1 ffc2 d7c2  ................
+000010a0: ffc2 d7c2 ffc2 d7c2 ffc2 d7c1 ffc2 d7c1  ................
+000010b0: ffc2 d7c2 ffc2 d7c1 ffc2 d7ce ffc2 d7c2  ................
+000010c0: ffc2 d7c2 ffc2 d7c4 ffc2 d7c1 ffc2 d7c1  ................
+000010d0: ffc2 d7c1 ffc2 d7c1 ffc1 d7c2 ffc2 d7c1  ................
+000010e0: ffc1 d7c2 ffc2 d7c1 ffc2 d7c2 ffc1 d7c2  ................
+000010f0: ffc2 d7c1 ffc2 d7c1 ffc1 d7c6 ffc2 d7c2  ................
+00001100: ffc1 d7c2 ffc2 d7c3 ffc1 d7c2 ffc2 d7d9  ................
+00001110: ffd1 ffc4 d7c1 ffc4 d7c1 ffc3 d7c2 ffc4  ................
+00001120: d7c3 ffc3 d7c2 ffc4 d7c1 ffc3 d7c2 ffc4  ................
+00001130: d7c3 ffc5 d7ca ffc7 d7c1 ffc3 d7c1 ffc3  ................
+00001140: d7c1 ffc3 d7c2 ffc4 d7c4 ffc9 d7c2 ffc1  ................
+00001150: d7c1 ffc2 d7c3 ffc8 d7c1 ffc3 d7cc ffc4  ................
+00001160: d7c2 ffc4 d7c3 ffc8 d7c1 ffc2 d7c1 ffc3  ................
+00001170: d7cb ffc4 d7c2 ffc3 d7c7 ffc2 d7c3 ffc4  ................
+00001180: d7cd ffc4 d7c3 ffc4 d7c2 ffc4 d7c1 ffc7  ................
+00001190: d7c2 ffc3 d7c1 ffc3 d7cd ffc2 d7c3 ffc4  ................
+000011a0: d7c5 ffc4 d7c3 ffc9 d7c2 ffc4 d7c3 ffc3  ................
+000011b0: d7c2 ffc3 d7c1 ffc8 d7c3 ffc3 d7c2 ffc4  ................
+000011c0: d7c2 ffc4 d7da ffff ffff ffff fff8 ffc2  ................
+000011d0: d7e6 ffc2 d7e3 ffc6 d7eb ffff ffff ffff  ................
+000011e0: fff8 ffc2 d7e6 ffc2 d7e3 ffc1 d7c4 ffc1  ................
+000011f0: d7eb ffff ffff ffff fff7 ffc4 d7e4 ffc4  ................
+00001200: d7e3 ffc4 d7ec ffff ffff ffff ffff ffff  ................
+00001210: fff8 ffff ffff ffff ffff ffff fff8 ffff  ................
+00001220: ffff ffff ffff ffff fff8 ffff ffff ffff  ................
+00001230: ffff ffff fff8 ffff ffff ffff ffff ffff  ................
+00001240: fff8 ffff ffff ffff ffff ffff fff8 ffff  ................
+00001250: ffff ffff ffff ffff fff8 fff0 ff00 c1c9  ................
+00001260: c2ca c2cb c1cc 00c8 ffcc 00c1 c9c1 cac1  ................
+00001270: ccc1 cbc4 00cc ff6a c1d8 da00 d4ff c300  .......j........
+00001280: 6ad0 00cc ffc3 006a c400 c8ff d000 6ac3  j......j......j.
+00001290: 00cc ffda 00c1 d86a d4ff c400 c1cb c1ca  .......j........
+000012a0: c2cb cc00 ffff d0ff f0ff c1c7 c1c9 c1ca  ................
+000012b0: c1c9 c1ca c1cb c1cc c1cb c8ff ca00 c1c7  ................
+000012c0: c2ca c3cb c1cc c1cb c200 ccff c200 c2d8  ................
+000012d0: d800 d4ff c400 c1d8 cf00 ccff 00c1 c7c1  ................
+000012e0: c9c1 d8c1 c9c1 cac1 c900 c8ff cf00 c1d8  ................
+000012f0: c400 ccff d800 c2d8 c200 d4ff c200 c1ca  ................
+00001300: c4cb c2cc c1cb ca00 ffff d0ff f0ff c1c7  ................
+00001310: c2c9 c2ca c2cc c1cb c8ff c800 c1c7 c2c9  ................
+00001320: c1ca c4cb c3cc 00cc ffc4 00c2 d8d6 00d4  ................
+00001330: ffc5 00c1 d8ce 00cc ffc2 c7c1 c9c1 d8c1  ................
+00001340: c9c1 cac1 cbc1 c9c8 ffce 00c1 d8c5 00cc  ................
+00001350: ffd6 00c2 d8c4 00d4 ff00 c2ca c4cb c1cc  ................
+00001360: c1cb c2cc c1cb c800 ffff d0ff f0ff c1c7  ................
+00001370: c1c9 c1ca c1c9 c2ca c1cc c1ca c8ff c600  ................
+00001380: c1c7 c2c9 c2ca c1cc c1cb c3cc c4cb ccff  ................
+00001390: c400 c1ca c1c9 c2d8 d2c9 c200 d4ff c500  ................
+000013a0: c1cc c1d8 c1cb cc00 ccff c1c7 c1c9 c1ca  ................
+000013b0: c1d8 c1ca c1cb c1cc c1ca c8ff cd00 c1d8  ................
+000013c0: c1c9 c1cb c400 ccff c200 d2c9 c2d8 c1c9  ................
+000013d0: c1ca c400 d4ff c1ca c1c9 c3ca c1cb c1c9  ................
+000013e0: c2ca c1cb c3cc c1cb c600 ffff d0ff f0ff  ................
+000013f0: c1c7 c2c9 c2ca c1cb c1cc c1cb c8ff 6ac6  ..............j.
+00001400: d8c1 cac3 cbc3 ccc1 cbc1 cac1 cbc1 ca84  ................
+00001410: 83cc ffc2 00c2 c9c2 cbc2 c9c2 d8c2 c9c1  ................
+00001420: cac1 c9c2 cac1 c9c4 cac1 cbc2 cac1 cbc2  ................
+00001430: ca00 d4ff c200 c1ca c1c9 c1ca c2cb c1d8  ................
+00001440: c1cc c1cb ca00 ccff c1c7 c1c9 c1ca c1d8  ................
+00001450: c2ca c1cc c1ca c8ff ca00 c1c7 c1c9 c1d8  ................
+00001460: c2ca c3cb c200 ccff 00c2 cac1 cbc2 cac1  ................
+00001470: cbc4 cac1 c9c2 cac1 c9c1 cac2 c9c2 d8c2  ................
+00001480: c9c4 cbc2 00d4 ff83 81c5 c9c1 cac1 c9c1  ................
+00001490: cac2 cbc2 ccc5 d86a ffff d0ff f0ff c1c7  .......j........
+000014a0: c1c9 c1ca c1c9 c1ca c1cb c1cc c1cb c8ff  ................
+000014b0: c200 c1c7 c2c9 c1ca c1c9 c1ca c1cb c3cc  ................
+000014c0: c1cb c1ca c1c9 c1ca 8483 8584 ccff 00c2  ................
+000014d0: cac2 cbc1 ccc2 cac1 c9c1 cac2 58c1 cbc1  ............X...
+000014e0: cac3 cbc2 cac1 cbc1 ccc3 cbc1 ccc1 cbc2  ................
+000014f0: ccd4 ff00 c2c9 c1ca c2c9 c1ca c1cb c1d8  ................
+00001500: c2cc c1cb c800 ccff c1c7 c2c9 c2ca c1cb  ................
+00001510: c1cc c1cb c8ff c800 c1c7 c2c9 c1d8 c1cb  ................
+00001520: c1cc c1cb c3cc c1cb 00cc ffc2 ccc1 cbc1  ................
+00001530: ccc3 cbc1 ccc1 cbc2 cac3 cbc1 cac1 cbc2  ................
+00001540: 58c1 cac1 c9c2 cac1 ccc3 cbc1 ca00 d4ff  X...............
+00001550: 84c2 8381 c1c9 c1c7 c3c9 c1ca c1cb c1ca  ................
+00001560: c1cc c1cb c3cc c1cb c200 ffff d0ff f0ff  ................
+00001570: c1c7 c1c9 c2ca c1d8 c2cc c1cb c8ff 00c2  ................
+00001580: c9c1 cac1 c9c2 cac3 ccc1 cbc1 cac1 c9c1  ................
+00001590: ca84 8385 8483 c1ca ccff c2cc c1cb c1cc  ................
+000015a0: c1cb c1cc c5cb c1cc c3cb c1cc c1cb c1cc  ................
+000015b0: c1cb c1cc c1cb c3cc c4ca d4ff c5c9 c1ca  ................
+000015c0: c1c9 c2ca c1cb c3cc c1cb c600 ccff c1c7  ................
+000015d0: c1c9 c1ca c1c9 c1ca c1cb c1cc c1cb c8ff  ................
+000015e0: c600 c1c7 c2c9 c2ca c1cc c1cb c3cc c2cb  ................
+000015f0: c1cc c1cb ccff c4ca c3cc c1cb c1cc c1cb  ................
+00001600: c1cc c1cb c1cc c3cb c1cc c5cb c1cc c4cb  ................
+00001610: c1cc d4ff c1c8 8384 c283 81c1 c9c1 c7c3  ................
+00001620: c9c1 cac2 cbc1 ccc1 cbc3 cc00 ffff d0ff  ................
+00001630: f0ff c1c7 c1c9 c1ca c1cb c1d8 c1ca c1cc  ................
+00001640: c1cb c8ff c1c7 c1c8 c1ca c1c9 c1ca c3cc  ................
+00001650: c1cb c1ca c1c9 c1ca 8483 8584 c4ca ccff  ................
+00001660: c4ca d8cc d4ff 8381 c5c9 c1ca c1c9 c1ca  ................
+00001670: c2cb c3cc c1cb c400 ccff c1c7 c1c9 c1ca  ................
+00001680: c1cb c1cc c1ca c1cc c1cb c8ff c400 c1c7  ................
+00001690: c2c9 c1ca c3cb c3cc c1cb c3ca 8483 ccff  ................
+000016a0: dacc c1cb c1cc d4ff c1c8 c3c9 84c2 8381  ................
+000016b0: c1c9 c1c7 c3c9 c1ca c1cb c3cc c1cb c1cc  ................
+000016c0: ffff d0ff f0ff c1c7 c1c9 c1ca c1cb c1d8  ................
+000016d0: c2cc c1cb c8ff c1c9 c2c8 c1c7 c2cc c1cb  ................
+000016e0: c1ca c1c9 c1ca 8483 8584 c4ca c1c8 c1ca  ................
+000016f0: ccff c4cc c1cb c1c9 c5ca c1cb c2ca cdcb  ................
+00001700: 80d4 ff84 c283 81c1 c9c1 c7c3 c9c1 cac1  ................
+00001710: cbc1 cac1 ccc1 cbc1 ccc1 cbc1 ccc1 cac2  ................
+00001720: 00cc ffc1 c7c1 c9c3 cac1 cbc1 ccc1 cbc8  ................
+00001730: ffc2 00c1 c9c1 cac1 ccc1 cac1 c9c1 cac1  ................
+00001740: cbc3 ccc1 cbc1 cac1 c9c1 ca84 8385 84cc  ................
+00001750: ff80 cdcb c2ca c1cb c5ca c1c9 c4cb c1cc  ................
+00001760: d4ff c1c8 c1d7 c4c9 84c2 8381 c1c8 c1c7  ................
+00001770: c3c9 c1cb c1ca c3cb ffff d0ff f0ff c1c7  ................
+00001780: c1c9 c1cb c1cc c1d8 c2cc c1cb c8ff 8381  ................
+00001790: c1c9 c1c8 c1c7 c1cb c2ca 8483 8584 c4ca  ................
+000017a0: c1cb 8258 c1c8 ccff 80c1 cb81 8384 c1cb  ...X............
+000017b0: 8183 84c1 cb81 8384 c1cb 8183 84c1 cb81  ................
+000017c0: 8384 c1cb 8183 8480 c281 d4ff c1c7 c1c9  ................
+000017d0: 84c2 8381 c1c9 c1c7 c3c9 c1ca c4cb c2cc  ................
+000017e0: c1ca 00cc ffc1 c9c1 c7c1 c9c1 cac1 cbc2  ................
+000017f0: ccc1 cbc8 ff00 c2ca c3cb c4cc c1cb c1ca  ................
+00001800: c1c9 c1ca 8483 8584 c2cb ccff c281 8084  ................
+00001810: 8381 c1cb 8483 81c1 cb84 8381 c1cb 8483  ................
+00001820: 81c1 cb84 8381 c1cb 8483 c1cb c283 d4ff  ................
+00001830: c1d7 58c1 d7c1 c9c1 c8c2 c9c1 c884 c283  ..X.............
+00001840: 81c2 c9c4 ca83 81ff ffd0 fff0 ffc1 c7c1  ................
+00001850: c9c2 cbc1 d8c2 ccc1 cbc8 ff84 83c3 c9c1  ................
+00001860: c784 8385 84c4 cac1 cc82 5882 6a00 ccff  ..........X.j...
+00001870: 85c1 cb83 8485 c1cb 8384 85c1 cb83 8485  ................
+00001880: c1cb 8384 85c1 cb83 8485 c1cb 8384 8581  ................
+00001890: 80c1 cad4 ffc2 c8c2 c984 c283 81c1 c9c1  ................
+000018a0: c7c1 c9c3 cac3 cbc2 ccc1 cbcc ffc1 c9c1  ................
+000018b0: c7c1 c9c3 cac1 ccc1 cbc8 ffc2 c9c4 cbc3  ................
+000018c0: ccc1 cac1 c9c1 ca84 8385 84c2 cbc1 cac1  ................
+000018d0: cbcc ffc1 ca80 8185 8483 c1cb 8584 83c1  ................
+000018e0: cb85 8483 c1cb 8584 83c1 cb85 8483 c1cb  ................
+000018f0: 8584 83c1 cb85 d4ff 0082 6a58 c1d7 c1ca  ..........jX....
+00001900: c4c9 84c2 8381 c1ca 8381 c1ca 8483 ffff  ................
+00001910: d0ff f0ff c2c7 c1c8 c1c9 c1d8 c2cb c1cc  ................
+00001920: c8ff c1c7 c1c8 c1c9 8381 c1c7 8584 c4ca  ................
+00001930: c1cc c1cb c1c9 826a c300 ccff c1c9 c3cb  .......j........
+00001940: c1ca c1c8 c5ca c1cb c2ca cbcb c2ca c1c9  ................
+00001950: d4ff c1ca c1d7 c1c8 c3c9 84c2 8381 c2c9  ................
+00001960: c3ca c1cb c2cc 81c1 cbcc ffc1 c9c3 cac1  ................
+00001970: cbc2 ccc1 cbc8 ffc1 c980 c2c9 c2cc c4cb  ................
+00001980: 8483 8584 c2cb c2ca c2cc ccff c1c9 c2ca  ................
+00001990: cbcb c2ca c1cb c5ca c1c8 c1ca c3cb c1c9  ................
+000019a0: d4ff c300 826a c1c7 c1ca c1cb c4c9 8483  .....j..........
+000019b0: c1ca 8483 c2ca c1cb ffff d0ff f0ff c1c7  ................
+000019c0: c1c8 c1c9 c1ca 6ac1 cac2 cbc8 ffb5 c2c8  ......j.........
+000019d0: 8483 c1c8 c3ca c1c9 c1c8 c1cb c1c9 c1c8  ................
+000019e0: c600 ccff b5c6 cbc1 c9cb cac3 cbc2 cac4  ................
+000019f0: cbd4 ffc1 c758 c2d7 c1c8 c2c9 c1c8 84c2  .....X..........
+00001a00: 8381 c1c9 c1ca c1cb c1ca c1c7 8083 c1cb  ................
+00001a10: ccff c1ca c381 8081 c1cb c1cc c8ff c1c9  ................
+00001a20: c380 c1c9 c2cb c1ca 8483 8584 c1c9 c3ca  ................
+00001a30: c1cb 8258 c1c9 ccff c4cb c2ca c3cb cbca  ...X............
+00001a40: c1c9 c6cb c1c9 d4ff c600 c1c7 c1c8 c1cb  ................
+00001a50: c1d7 c4c9 c5ca b5ff ffd0 fff0 ffc1 c883  ................
+00001a60: 81c2 ca83 81c1 cbc8 ffc1 c7c3 c8c1 c9c1  ................
+00001a70: c8c1 c9c1 cac1 cb82 58c1 c8c8 00cc ff00  ........X.......
+00001a80: c2cb 82c4 58c1 d7c7 cbc2 cc82 c458 c1d7  ....X........X..
+00001a90: c1cc c2cd 00d4 ff00 826a 58c1 d7c1 cac4  .........jX.....
+00001aa0: c984 c283 81c1 cac1 c780 8184 c1ca ccff  ................
+00001ab0: c1ca c281 8081 8384 c1cc c8ff c1c8 c280  ................
+00001ac0: c281 c1c9 8483 8584 c2cb c2ca c1cc 8258  ...............X
+00001ad0: 826a 00cc ff00 c2cd c1cc c1d7 c458 82c2  .j...........X..
+00001ae0: ccc7 cbc1 d7c4 5882 c2cb 00d4 ffc8 00c1  ......X.........
+00001af0: d758 c1d7 c1c9 c1c8 c1c9 c5ca c1c8 ffff  .X..............
+00001b00: d0ff f0ff c1c8 8483 c2ca 8483 c1cb c8ff  ................
+00001b10: c200 c1c7 c1c8 b5c1 c8c1 cb82 5882 6ac9  ............X.j.
+00001b20: 00cc ffc3 0082 6ac2 8882 6ac9 0082 6ac2  ......j...j...j.
+00001b30: 8882 6ac4 00d4 ffc3 0082 6ac1 c7c1 cac1  ..j.......j.....
+00001b40: cbc2 c9c1 c8c1 c984 83c1 cac1 c781 83c2  ................
+00001b50: cacc ffc1 c9c2 8081 83c2 84c1 cbc8 ffc1  ................
+00001b60: c8c1 c981 c283 c1c9 8584 c4ca c1cc c1cb  ................
+00001b70: c1c8 826a c300 ccff c400 6a82 c288 6a82  ...j......j...j.
+00001b80: c900 6a82 c288 6a82 c300 d4ff c900 826a  ..j...j........j
+00001b90: 58c1 d7c1 cbc1 cab5 c1ca c1c8 c200 ffff  X...............
+00001ba0: d0ff f0ff c1c7 c1c9 c5ca c1cb c8ff c400  ................
+00001bb0: c1c7 c1c8 c1c9 826a cb00 fcff c600 c1c6  .......j........
+00001bc0: c1c8 c1cb c1d7 c1c8 c1c9 c1c8 c1c9 c1ca  ................
+00001bd0: 80c2 cac1 cbc1 cacc ffc1 c9c7 cac8 ffc1  ................
+00001be0: c9c1 c8c2 c984 c1c9 c1ca 83c2 cac2 cbc1  ................
+00001bf0: c9c1 c8c6 00fc ffcb 0082 6ac1 c9c1 cac1  ..........j.....
+00001c00: c8c4 00ff ffd0 fff0 ffc1 c7b5 c1c9 c3ca  ................
+00001c10: b7c1 cbc8 ffd4 00fc ffc8 00c1 c858 c2d7  .............X..
+00001c20: c2c9 c3ca 34c2 cacc ffc1 c9c2 cac2 34c3  ....4.........4.
+00001c30: cac8 ffc2 c943 c3c9 c2ca c1cb 8258 c1c8  .....C.......X..
+00001c40: c800 fcff d400 ffff d0ff f0ff 00c1 c7c1  ................
+00001c50: c8c1 c9c3 ca00 c8ff d400 fcff c900 826a  ...............j
+00001c60: 58c1 d7c1 c8c1 cac1 cbc2 cac1 cb00 ccff  X...............
+00001c70: c4c9 c4ca c8ff c200 c4c9 c1ca 8258 826a  .............X.j
+00001c80: c900 fcff d400 ffff d0ff ffff c1ff d400  ................
+00001c90: fcff cb00 826a c1c8 c2ca c1cb c300 ccff  .....j..........
+00001ca0: 58c5 c9c2 cbc8 ffc4 00c3 c982 6acb 00fc  X...........j...
+00001cb0: ffd4 00ff ffd0 ffff ffff ffff ffff ffff  ................
+00001cc0: fff8 ffff ffff ffff ffff ffff fff8 ffff  ................
+00001cd0: ffff ffff ffff ffff fff8 ffd0 ffc7 d7e0  ................
+00001ce0: ffc2 d7c1 ffc2 d7c1 ffc7 d7e5 ffc2 d7c1  ................
+00001cf0: ffc2 d7c4 ffc8 d7e1 ffc3 d7c4 ffc4 d7c5  ................
+00001d00: ffc3 d7c3 ffc4 d7cc ffc5 d7c3 ffc4 d7c1  ................
+00001d10: ffc3 d7cb ffc3 d7d2 ffc1 d7c4 ffc4 d7ff  ................
+00001d20: fffa ffd1 ffc2 d7c3 ffc1 d7ce ffc1 d7d1  ................
+00001d30: ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc1 d7e5  ................
+00001d40: ffc2 d7c1 ffc2 d7c4 ffc1 d7c2 ffc2 d7c2  ................
+00001d50: ffc1 d7e2 ffc2 d7c3 ffc2 d7c2 ffc2 d7c3  ................
+00001d60: ffc2 d7c4 ffc4 d7cc ffc6 d7c2 ffc4 d7c3  ................
+00001d70: ffc2 d7cc ffc2 d7d1 ffc2 d7c3 ffc4 d7ff  ................
+00001d80: fffb ffd1 ffc2 d7d2 ffc1 d7d1 ffc2 d7c1  ................
+00001d90: ffc2 d7c2 ffc2 d7e9 ffc2 d7c1 ffc2 d7c7  ................
+00001da0: ffc2 d7e5 ffc2 d7c3 ffc2 d7c2 ffc2 d7c2  ................
+00001db0: ffc2 d7c5 ffc1 d7cf ffc1 d7c3 ffc1 d7c3  ................
+00001dc0: ffc1 d7c6 ffc2 d7cc ffc2 d7d0 ffc3 d7c3  ................
+00001dd0: ffc1 d7ff fffe ffd1 ffc2 d7c1 ffc1 d7c3  ................
+00001de0: ffc3 d7c3 ffc4 d7c1 ffc4 d7c1 ffc3 d7c2  ................
+00001df0: ffc3 d7c1 ffc2 d7cb ffc2 d7c1 ffc1 d7c2  ................
+00001e00: ffc3 d7c1 ffc6 d7c2 ffc3 d7c1 ffc2 d7c1  ................
+00001e10: ffc3 d7c3 ffc4 d7c2 ffc4 d7ce ffc2 d7c3  ................
+00001e20: ffc3 d7c1 ffc2 d7c1 ffc3 d7c2 ffc3 d7c1  ................
+00001e30: ffc2 d7c1 ffc2 d7cd ffc2 d7c3 ffc2 d7c2  ................
+00001e40: ffc2 d7c1 ffc5 d7c3 ffc4 d7d0 ffc1 d7c3  ................
+00001e50: ffc4 d7c3 ffc2 d7c1 ffc8 d7c3 ffc2 d7c1  ................
+00001e60: ffc2 d7cd ffc3 d7c3 ffc4 d7c4 ffc5 d7c3  ................
+00001e70: ffc3 d7c3 ffc4 d7c2 ffc4 d7c2 ffc3 d7c2  ................
+00001e80: ffc3 d7c1 ffc2 d7c2 ffc5 d7c2 ffc3 d7c2  ................
+00001e90: ffc3 d7c1 ffc2 d7c1 ffc4 d7f8 ffd1 ffc4  ................
+00001ea0: d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc1  ................
+00001eb0: d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2 ffc3  ................
+00001ec0: d7c1 ffc1 d7cb ffc4 d7c3 ffc3 d7c2 ffc2  ................
+00001ed0: d7c1 ffc2 d7c2 ffc3 d7c1 ffc3 d7c1 ffc2  ................
+00001ee0: d7c1 ffc2 d7c2 ffc1 d7c1 ffc2 d7c2 ffc1  ................
+00001ef0: d7ce ffc2 d7c4 ffc3 d7c1 ffc3 d7c1 ffc2  ................
+00001f00: d7c2 ffc8 d7cd ffc2 d7c3 ffc2 d7c2 ffc2  ................
+00001f10: d7c1 ffc2 d7c2 ffc2 d7c1 ffc6 d7ce ffc1  ................
+00001f20: d7c3 ffc6 d7c2 ffc2 d7c1 ffc1 d7c3 ffc2  ................
+00001f30: d7c1 ffc2 d7c2 ffc5 d7cc ffc1 d7c1 ffc2  ................
+00001f40: d7c2 ffc6 d7c4 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+00001f50: d7c1 ffc2 d7c1 ffc2 d7c2 ffc1 d7c1 ffc2  ................
+00001f60: d7c2 ffc1 d7c1 ffc2 d7c1 ffc2 d7c2 ffc5  ................
+00001f70: d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00001f80: d7c2 ffc3 d7c1 ffc3 d7c2 ffc1 d7f8 ffd1  ................
+00001f90: ffc2 d7c1 ffc1 d7c2 ffc2 d7c1 ffc2 d7c1  ................
+00001fa0: ffc3 d7c4 ffc2 d7c1 ffc5 d7c2 ffc2 d7ce  ................
+00001fb0: ffc2 d7c1 ffc1 d7c4 ffc2 d7c2 ffc2 d7c1  ................
+00001fc0: ffc2 d7c2 ffc2 d7c3 ffc5 d7c1 ffc3 d7c3  ................
+00001fd0: ffc3 d7d0 ffc2 d7c4 ffc2 d7c6 ffc2 d7c2  ................
+00001fe0: ffc2 d7c1 ffc2 d7c1 ffc2 d7cd ffc2 d7c4  ................
+00001ff0: ffc5 d7c1 ffc2 d7c2 ffc2 d7c5 ffc2 d7ce  ................
+00002000: ffc1 d7c7 ffc2 d7c2 ffc4 d7c3 ffc2 d7c1  ................
+00002010: ffc2 d7c2 ffc2 d7c1 ffc2 d7cb ffc1 d7c2  ................
+00002020: ffc2 d7c6 ffc2 d7c4 ffc2 d7c1 ffc2 d7c4  ................
+00002030: ffc2 d7c1 ffc3 d7c3 ffc3 d7c3 ffc5 d7c2  ................
+00002040: ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c2  ................
+00002050: ffc5 d7c2 ffc2 d7c3 ffc3 d7fa ffd1 ffc2  ................
+00002060: d7c4 ffc2 d7c1 ffc2 d7c3 ffc3 d7c2 ffc2  ................
+00002070: d7c1 ffc2 d7c5 ffc2 d7ce ffc2 d7c6 ffc3  ................
+00002080: d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2  ................
+00002090: d7c6 ffc3 d7c3 ffc3 d7ce ffc2 d7c4 ffc2  ................
+000020a0: d7c4 ffc4 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+000020b0: d7c4 ffc3 d7c6 ffc2 d7c6 ffc2 d7c2 ffc2  ................
+000020c0: d7c2 ffc2 d7c6 ffc1 d7c4 ffc3 d7c7 ffc1  ................
+000020d0: d7c8 ffc1 d7c2 ffc2 d7c1 ffc2 d7c2 ffc2  ................
+000020e0: d7c1 ffc2 d7c2 ffc2 d7c1 ffc2 d7c4 ffc3  ................
+000020f0: d7c4 ffc6 d7c6 ffc1 d7c4 ffc2 d7c1 ffc2  ................
+00002100: d7c2 ffc4 d7c3 ffc3 d7c3 ffc3 d7c1 ffc2  ................
+00002110: d7c5 ffc2 d7c1 ffc2 d7c2 ffc3 d7c3 ffc2  ................
+00002120: d7c5 ffc2 d7c5 ffc3 d7f8 ffd1 ffc2 d7c4  ................
+00002130: ffc2 d7c1 ffc2 d7c1 ffc1 d7c2 ffc2 d7c2  ................
+00002140: ffc2 d7c1 ffc2 d7c2 ffc1 d7c2 ffc2 d7ce  ................
+00002150: ffc2 d7c3 ffc1 d7c1 ffc1 d7c1 ffc2 d7c1  ................
+00002160: ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2 d7c2  ................
+00002170: ffc1 d7c1 ffc1 d7c2 ffc2 d7c1 ffc1 d7c2  ................
+00002180: ffc2 d7ce ffc2 d7c4 ffc2 d7c3 ffc2 d7c1  ................
+00002190: ffc2 d7c2 ffc2 d7c1 ffc2 d7c1 ffc2 d7cd  ................
+000021a0: ffc2 d7c5 ffc2 d7c3 ffc2 d7c2 ffc2 d7c1  ................
+000021b0: ffc2 d7c2 ffc1 d7ce ffc1 d7c4 ffc2 d7c2  ................
+000021c0: ffc1 d7c3 ffc2 d7c2 ffc2 d7c1 ffc2 d7c1  ................
+000021d0: ffc2 d7c2 ffc2 d7c1 ffc2 d7ce ffc2 d7c2  ................
+000021e0: ffc2 d7c2 ffc1 d7c5 ffc2 d7c1 ffc2 d7c1  ................
+000021f0: ffc2 d7c1 ffc2 d7c1 ffc1 d7c2 ffc2 d7c1  ................
+00002200: ffc1 d7c2 ffc2 d7c1 ffc2 d7c2 ffc1 d7c2  ................
+00002210: ffc2 d7c1 ffc2 d7c1 ffc1 d7c6 ffc2 d7c2  ................
+00002220: ffc1 d7c2 ffc2 d7c3 ffc1 d7c2 ffc2 d7f8  ................
+00002230: ffd0 ffc4 d7c4 ffc3 d7c2 ffc4 d7c3 ffc3  ................
+00002240: d7c1 ffc3 d7c2 ffc4 d7cc ffc9 d7c1 ffc7  ................
+00002250: d7c2 ffc4 d7c3 ffc3 d7c2 ffc4 d7c2 ffc4  ................
+00002260: d7ce ffc4 d7c2 ffc4 d7c3 ffc8 d7c1 ffc2  ................
+00002270: d7c1 ffc3 d7cb ffc4 d7c2 ffc3 d7c5 ffc4  ................
+00002280: d7c2 ffc4 d7cf ffc1 d7c4 ffc4 d7c3 ffc4  ................
+00002290: d7c1 ffc7 d7c2 ffc3 d7c1 ffc3 d7cd ffc2  ................
+000022a0: d7c2 ffc4 d7c6 ffc4 d7c3 ffc9 d7c2 ffc4  ................
+000022b0: d7c3 ffc3 d7c2 ffc3 d7c1 ffc8 d7c3 ffc3  ................
+000022c0: d7c2 ffc4 d7c2 ffc4 d7f9 ffff ffcb ffc2  ................
+000022d0: d7ff ffff ffcc ffc2 d7e6 ffc2 d7e3 ffc6  ................
+000022e0: d7ff ffcb ffff ffcb ffc2 d7ff ffff ffcc  ................
+000022f0: ffc2 d7e6 ffc2 d7e3 ffc1 d7c4 ffc1 d7ff  ................
+00002300: ffcb ffff ffca ffc4 d7ff ffff ffca ffc4  ................
+00002310: d7e4 ffc4 d7e3 ffc4 d7ff ffcc ffff ffff  ................
+00002320: ffff ffff ffff fff8 ffff ffff ffff ffff  ................
+00002330: ffff fff8 ffff ffff ffff ffff ffff fff8  ................
+00002340: ffff ffff ffff ffff ffff fff8 ffff ffff  ................
+00002350: ffff ffff ffff fff8 ffff ffff ffff ffff  ................
+00002360: ffff fff8 ffff ffff ffff ffff ffff fff8  ................
+00002370: fff0 ffc8 00c8 ffd4 00cc ffca 00c1 f5d1  ................
+00002380: 00d4 ffc6 00c1 f521 cc00 ccff c200 6a21  .......!......j!
+00002390: c1f5 84c2 00c8 ffcc 0021 6ac6 00cc ffd1  .........!j.....
+000023a0: 00c1 f5ca 00d4 ffd4 00ff ffd0 fff0 ffc8  ................
+000023b0: 00c8 ffc3 006a 21c6 00c1 cac1 cbc7 00cc  .....j!.........
+000023c0: ffca 0021 88d0 00d4 ffc4 006a 21c1 d86a  ...!.......j!..j
+000023d0: cc00 ccff 0084 0088 6a00 c1f5 00c8 ffcc  ........j.......
+000023e0: 006a c1d8 21c1 f5c4 00cc ffd0 0088 21ca  .j..!.........!.
+000023f0: 00d4 ffc7 00c2 ccc6 0021 c1f5 c300 ffff  .........!......
+00002400: d0ff f0ff 00c1 cac4 cbc1 cc00 c8ff c400  ................
+00002410: c1d8 21c1 f500 c1c7 c2c9 c2ca c1cb c1cc  ..!.............
+00002420: c500 ccff ca00 6ac1 d888 cf00 d4ff c500  ......j.........
+00002430: c1d8 6acd 00cc ff00 c1c7 c1c9 c1d8 6ac1  ..j...........j.
+00002440: cac1 c900 c8ff cd00 6ac1 d8c5 00cc ffcf  ........j.......
+00002450: 0088 c1d8 6aca 00d4 ffc5 00c2 cbc1 ccc1  ....j...........
+00002460: cbc2 ccc1 cb00 216a c1d8 c400 ffff d0ff  ......!j........
+00002470: f0ff c1c7 c1c9 c1ca c1c9 c2ca c1cc c1ca  ................
+00002480: c8ff c400 c1d8 6ac1 c7c2 c9c2 cac1 ccc1  ......j.........
+00002490: cbc1 ccc1 cbc2 ccc3 00cc ffc2 00ca c988  ................
+000024a0: 6acb c9c3 00d4 ffc2 00c1 cac1 c9c1 d86a  j..............j
+000024b0: c1cb c2cc c1cb ca00 ccff c2c7 c1c9 88c1  ................
+000024c0: d8c1 cac1 cbc1 c9c8 ffca 00c1 c7c2 c9c1  ................
+000024d0: ca6a c1d8 c2cb c200 ccff c300 cbc9 6a88  .j............j.
+000024e0: cac9 c200 d4ff c300 c2ca c1cb c1c9 c2ca  ................
+000024f0: c1cb c3cc c1cb 6ac1 d8c4 00ff ffd0 fff0  ......j.........
+00002500: ffc1 c7c2 c9c2 cac1 cbc1 ccc1 cbc8 ffc3  ................
+00002510: 00c1 d86a c2c9 c1ca c3cb c3cc c1cb c3ca  ...j............
+00002520: c200 ccff 00c2 cac1 cbc2 cac1 cbc2 cac1  ................
+00002530: cbc3 6ac1 cac1 c9c1 cac3 c9c1 cac3 c9c1  ..j.............
+00002540: cac1 c9c1 c7c2 00d4 ff00 c2c9 c1ca c1c9  ................
+00002550: c1d8 6ac2 cbc2 ccc1 cbc8 00cc ffc1 c7c1  ..j.............
+00002560: c9c1 cac1 d86a c1cb c1cc c1ca c8ff c800  .....j..........
+00002570: c1c7 c2c9 c1ca c1cb 6ac1 d8c3 ccc1 cb00  ........j.......
+00002580: ccff c200 c1c7 c1c9 c1ca c3c9 c1ca c3c9  ................
+00002590: c1ca c1c9 c1ca c36a c1cb c2ca c1cb c2ca  .......j........
+000025a0: c1cb c2ca 00d4 ffc2 00c5 c9c1 cac1 c9c1  ................
+000025b0: cac2 cbc3 cc6a c1d8 c300 ffff d0ff f0ff  .....j..........
+000025c0: c1c7 c1c9 6a21 c1f5 84c1 ccc1 cbc8 ffc2  ....j!..........
+000025d0: 00c1 c7c1 c9c1 d86a c1c9 c1ca c1cb c3cc  .......j........
+000025e0: c1cb c1ca c1c9 c2ca 8081 00cc ffc1 c9c1  ................
+000025f0: ccc1 cbc1 ccc2 cbc1 ccc3 cbc1 d888 c3ca  ................
+00002600: c3cb c1ca c1c9 c2cb c1ca c1c9 c1ca 84c1  ................
+00002610: c700 d4ff c5c9 c1ca c1d8 c2ca c1cb c3cc  ................
+00002620: c1cb c600 ccff c1c7 c1c9 c1ca c1c9 c2ca  ................
+00002630: c1cc c1ca c8ff c600 c1c7 c2c9 c2ca c1cc  ................
+00002640: c1cb c1d8 c2cc c2cb c1cc c1cb ccff 00c2  ................
+00002650: c7c1 cac1 c9c1 cac2 cbc1 c9c1 cac3 cbc3  ................
+00002660: ca88 c1d8 c3cb c1cc c2cb c1cc c1cb c2cc  ................
+00002670: d4ff 00c2 80c2 c9c1 c7c3 c9c1 cac1 cbc1  ................
+00002680: cac1 ccc1 cb6a c1d8 c1cc c1cb c200 ffff  .....j..........
+00002690: d0ff f0ff c1c7 84c1 ca88 6ac1 ccc1 f5c1  ..........j.....
+000026a0: cbc8 ff00 c2c9 c1ca c1c9 c1d8 c1ca c3cc  ................
+000026b0: c1cb c1ca c1c9 c1ca 8483 c1ca 8183 00cc  ................
+000026c0: ffc2 c9c1 ccc1 cbc2 ccc1 cbc2 ccc1 cbc1  ................
+000026d0: ccc1 cbc1 ccc3 cbc1 ccc3 cbc1 ccc4 cb83  ................
+000026e0: 8480 d4ff 8381 c5c9 c1ca c1c9 c1ca c2cb  ................
+000026f0: c3cc c1cb c400 ccff c1c7 c2c9 c2ca c1cb  ................
+00002700: c1cc c1cb c8ff c400 c1c7 c2c9 c1ca c3cb  ................
+00002710: c3cc c1cb c3ca 8483 ccff c380 c4cb c1cc  ................
+00002720: c3cb c1cc c3cb c1cc c1cb c1cc c1cb c2cc  ................
+00002730: c1cb c2cc c1cb c3cc d4ff 0080 81c1 c983  ................
+00002740: 81c1 c9c1 c7c3 c9c1 cac2 cbc1 d8c1 cbc3  ................
+00002750: cc00 ffff d0ff f0ff c1c7 c1c9 c1ca c1d8  ................
+00002760: 6ac1 cac1 ccc1 cbc8 ffc1 c7c1 c8c1 cac1  j...............
+00002770: c9c1 cac3 ccc1 cbc1 cac1 c9c1 ca84 8385  ................
+00002780: 84c1 ca83 c284 ccff c2c9 d7cc 8483 84d4  ................
+00002790: ff84 c283 81c1 c9c1 c7c3 c9c1 cac1 cbc1  ................
+000027a0: cac1 ccc1 cbc3 ccc3 00cc ffc1 c7c1 c9c1  ................
+000027b0: cac1 c9c1 cac1 cbc1 ccc1 cbc8 ffc3 00c1  ................
+000027c0: cac1 ccc1 cac1 c9c1 cac1 cbc3 ccc1 cbc1  ................
+000027d0: cac1 c9c1 ca84 8385 84cc ffc3 81d9 ccd4  ................
+000027e0: ffc2 8183 c1c9 84c2 8381 c1c9 c1c7 c3c9  ................
+000027f0: c1ca c1cb c3cc c1cb c1cc ffff d0ff f0ff  ................
+00002800: c1c7 c1c9 c1ca 88c1 d8c2 ccc1 cbc8 ffc1  ................
+00002810: c9c2 c8c1 c7c2 ccc1 cbc1 cac1 c9c1 ca84  ................
+00002820: 8385 84c4 cac1 cbc1 cacc ff83 84cc cbc2  ................
+00002830: cac1 cbc3 cac1 cbc4 ca84 c283 d4ff c1c7  ................
+00002840: c1c9 84c2 8381 c1c9 c1c7 c3c9 c1ca c4cb  ................
+00002850: c1cc c300 ccff c1c7 c1c9 c2ca c1cb c2cc  ................
+00002860: c1cb c8ff c200 c1ca c3cb c4cc c1cb c1ca  ................
+00002870: c1c9 c1ca 8483 8584 c2cb ccff c283 81c4  ................
+00002880: cac1 cbc3 cac1 cbc2 cacc cb84 83d4 ffc2  ................
+00002890: c8c4 c984 c283 81c1 c8c1 c7c3 c9c1 cbc1  ................
+000028a0: cac3 cbff ffd0 fff0 ffc1 c7c1 c9c1 cbc1  ................
+000028b0: d86a c2cc c1cb c8ff 8381 c1c9 c1c8 c1c7  .j..............
+000028c0: c1cb c2ca 8483 8584 c4ca c1c9 c1cb 82c1  ................
+000028d0: d7cc ff84 8581 8384 85c1 cb81 8384 85c1  ................
+000028e0: cc81 8384 85c1 cb81 8384 c1cb 8183 8485  ................
+000028f0: 84c2 83d4 ffc2 c8c2 c984 c283 81c1 c9c1  ................
+00002900: c7c1 c9c3 cac1 cc80 8183 c200 ccff c1c7  ................
+00002910: c1c9 c1ca c1cb c1cc c1ca c1cc c1cb c8ff  ................
+00002920: c200 c3c7 c1cb c3cc c1ca c1c9 c1ca 8483  ................
+00002930: 8584 c2cb c1ca c1cb ccff c283 8185 8483  ................
+00002940: 81c1 cb84 8381 c1cb 8584 8381 c1cc 8584  ................
+00002950: 8381 c1cb 8584 8381 8584 d4ff c1d7 82c1  ................
+00002960: c8c1 c9c1 c8c2 c9c1 c884 c283 81c2 c9c4  ................
+00002970: ca83 81ff ffd0 fff0 ffc1 c7c1 c9c2 cbc3  ................
+00002980: ccc1 cbc8 ff84 83c3 c9c1 c784 8385 84c4  ................
+00002990: cac2 ccc1 ca82 6a00 ccff c2c9 8384 8515  ......j.........
+000029a0: c1cc 8384 8515 c1cc 8384 8515 c1cc 8384  ................
+000029b0: 85c1 cc83 8485 1580 8384 d4ff c2ca c1c8  ................
+000029c0: c3c9 84c2 8381 c2c9 c1ca c2c7 8183 84c2  ................
+000029d0: 00cc ffc1 c7c1 cac4 cbc1 ccc1 cbc8 ff00  ................
+000029e0: c2c7 c280 c281 c1cb c1ca c1cb 8483 8584  ................
+000029f0: c2cb c2ca c2cc ccff 8483 8015 8584 83c1  ................
+00002a00: cc85 8483 c1cc 1585 8483 c1cc 1585 8483  ................
+00002a10: c1cc 1585 8483 c2cc d4ff 0082 c1d7 c1c7  ................
+00002a20: c2ca c4c9 84c2 8381 c1ca 8381 c1ca 8483  ................
+00002a30: ffff d0ff f0ff c2c7 c1c8 c1c9 c1ca c2cb  ................
+00002a40: c1cc c8ff c1c7 c1c8 c1c9 8381 c1c7 8584  ................
+00002a50: c4ca c1cc c1cb c1c9 826a c300 ccff c1c9  .........j......
+00002a60: c4ca c1cb c3ca c1cb c2ca cdcb c280 84d4  ................
+00002a70: ffc2 c7c2 cac1 c8c2 c9c1 c884 83c1 c980  ................
+00002a80: c2c7 8083 c384 00cc ffc1 c9c3 cac4 cbc8  ................
+00002a90: ff00 c280 c281 c283 8480 c1ca 8584 c1c9  ................
+00002aa0: c3ca c1cb c1cc c1ca c1c9 ccff 84c2 80c4  ................
+00002ab0: cac1 cbc3 cac1 cbc2 cacd cbc1 ccd4 ffc3  ................
+00002ac0: 0082 c1d7 c1c7 c1ca c1cb c4c9 8483 c1ca  ................
+00002ad0: 8483 c2ca c1cb ffff d0ff f0ff c1c7 c1c8  ................
+00002ae0: c1c9 c3ca c2cb c8ff b5c2 c884 83c1 c8c3  ................
+00002af0: cac1 c9c2 cbc1 c9c1 c8c6 00cc ffc1 cbc1  ................
+00002b00: c9d0 cac2 ccc3 cac2 cbc2 ca34 d4ff 0082  ...........4....
+00002b10: c1d7 82c2 cac4 c9c1 c881 80c1 c781 c484  ................
+00002b20: 00cc ffc1 c9c2 c780 8183 84c1 cbc8 ff80  ................
+00002b30: c281 c283 c284 8381 c1ca c2cb c2ca c1cc  ................
+00002b40: c1cb 82c1 d76a 00cc ff43 c2ca c1c9 d0ca  .....j...C......
+00002b50: c2cc c3ca c3cb d4ff c600 c1c7 c1c8 c1cb  ................
+00002b60: c1c8 c4c9 c5ca b5ff ffd0 fff0 ffc1 c883  ................
+00002b70: 81c2 ca83 81c1 cbc8 ffc1 c7c3 c8c1 c9c1  ................
+00002b80: c8c2 c9c2 cb82 c1d7 c800 ccff 00c1 cac7  ................
+00002b90: c9c5 cbc6 ccc1 cbc3 ccc1 cdc2 ca00 d4ff  ................
+00002ba0: c300 82c1 d7c1 c7c1 cac1 cbc2 c9c1 c883  ................
+00002bb0: 8180 83c5 84cc ffc2 c780 8183 c384 c8ff  ................
+00002bc0: 81c2 83c4 8481 83c3 cac1 ccc1 cbc1 c8c1  ................
+00002bd0: d76a c300 ccff 00c3 cac7 c9c5 cbc6 ccc1  .j..............
+00002be0: cbc3 ccc1 cd00 d4ff c800 c1d7 82c1 c8c1  ................
+00002bf0: cbc2 c9c5 cac1 c8ff ffd0 fff0 ffc1 c884  ................
+00002c00: 83c2 ca84 83c1 cbc8 ffc2 00c1 c7c1 c8b5  ................
+00002c10: c1c8 c2cb c1c9 826a c900 ccff c200 826a  .......j.......j
+00002c20: c288 826a cac9 826a c288 826a c2c9 c200  ...j...j...j....
+00002c30: d4ff c600 c1c6 c1c8 c2cb c2c8 c1c9 c281  ................
+00002c40: c384 c1ca 34cc ffc1 c780 8183 c484 c8ff  ....4...........
+00002c50: 43c1 c8c4 8483 c3ca c2cb c1c9 c1c8 c600  C...............
+00002c60: ccff c200 c2c9 6a82 c288 6a82 cac9 6a82  ......j...j...j.
+00002c70: c288 6a82 c200 d4ff c900 82c1 d7c1 c8c2  ..j.............
+00002c80: cbc1 cab5 c1ca c1c8 c200 ffff d0ff f0ff  ................
+00002c90: c1c7 c1c9 c5ca c1cb c8ff c400 c1c7 c1c8  ................
+00002ca0: c1c9 82cc 00fc ffc8 00c1 c8c1 c9c1 c8c1  ................
+00002cb0: cac2 c983 84c2 ca20 6acc ff80 8183 c584  ....... j.......
+00002cc0: c8ff 586a c2c9 c284 c2ca c1cb c1ca c1c9  ..Xj............
+00002cd0: c1c8 c800 fcff cb00 82c1 d7c1 c9c1 cac1  ................
+00002ce0: c8c4 00ff ffd0 fff0 ffc1 c7b5 c1c9 c3ca  ................
+00002cf0: b7c1 cbc8 ffd4 00fc ffc9 0082 c1d7 c2ca  ................
+00002d00: c1c8 c1ca 3420 6ac2 00cc ff81 83c6 84c8  ....4 j.........
+00002d10: ffc2 0058 6a43 c1c9 c1ca c1cb 82c1 d76a  ...XjC.........j
+00002d20: c900 fcff d400 ffff d0ff f0ff 00c1 c7c1  ................
+00002d30: c8c1 c9c3 ca00 c8ff d400 fcff cb00 82c1  ................
+00002d40: d7c1 c820 6ac4 00cc ffc1 c9c7 cac8 ffc4  ... j...........
+00002d50: 0058 6ac1 c9c1 d76a cb00 fcff d400 ffff  .Xj....j........
+00002d60: d0ff ffff ffff f2ff c1c9 43c4 ca34 c1ca  ..........C..4..
+00002d70: ffff ffff fdff ffff ffff f2ff 0058 6ac2  .............Xj.
+00002d80: 20c2 2800 ffff ffff fdff ffff ffff ffff   .(.............
+00002d90: ffff ffff f8ff ffff ffff ffff ffff ffff  ................
+00002da0: f8ff ffff ffff ffff ffff ffff f8ff ffff  ................
+00002db0: ffff ffff ffff ffff f8ff ffff ffff ffff  ................
+00002dc0: ffff ffff f8ff d1ff c7d7 e0ff c2d7 c1ff  ................
+00002dd0: c2d7 c3ff c3d7 c1ff c1d7 f5ff c2d7 c1ff  ................
+00002de0: c2d7 ccff c3d7 c4ff c4d7 c3ff c4d7 c5ff  ................
+00002df0: c3d7 ccff c4d7 c3ff c4d7 c2ff c3d7 cbff  ................
+00002e00: c3d7 d0ff c4d7 c2ff c4d7 ffff ffff ccff  ................
+00002e10: d2ff c2d7 c3ff c1d7 ceff c1d7 d1ff c2d7  ................
+00002e20: c1ff c2d7 c2ff c2d7 c2ff c2d7 dcff c1d7  ................
+00002e30: d8ff c2d7 c1ff c2d7 cdff c2d7 c3ff c2d7  ................
+00002e40: c2ff c2d7 c1ff c2d7 c2ff c2d7 c3ff c2d7  ................
+00002e50: cdff c2d7 c2ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00002e60: c2ff c2d7 ccff c2d7 cfff c4d7 c2ff c2d7  ................
+00002e70: c2ff c2d7 ffff ffff cbff d2ff c2d7 d2ff  ................
+00002e80: c1d7 d1ff c2d7 c1ff c2d7 c2ff c2d7 c3ff  ................
+00002e90: c1d7 dcff c1d7 d8ff c2d7 c1ff c2d7 cdff  ................
+00002ea0: c2d7 c3ff c2d7 c2ff c2d7 c1ff c2d7 c2ff  ................
+00002eb0: c2d7 c2ff c2d7 ceff c2d7 c2ff c2d7 c1ff  ................
+00002ec0: c2d7 c2ff c2d7 c2ff c2d7 ccff c2d7 cfff  ................
+00002ed0: c1d7 c5ff c2d7 c2ff c2d7 ffff ffff cbff  ................
+00002ee0: d2ff c2d7 c1ff c1d7 c3ff c3d7 c3ff c4d7  ................
+00002ef0: c1ff c4d7 c1ff c3d7 c2ff c3d7 c1ff c2d7  ................
+00002f00: cbff c3d7 c4ff c3d7 c1ff c7d7 c3ff c3d7  ................
+00002f10: c2ff c3d7 c1ff c9d7 c1ff c2d7 c1ff c3d7  ................
+00002f20: c2ff c3d7 c1ff c2d7 c1ff c2d7 d4ff c2d7  ................
+00002f30: c3ff c2d7 c2ff c2d7 c1ff c3d7 c1ff c1d7  ................
+00002f40: c2ff c5d7 ccff c3d7 c1ff c1d7 c2ff c2d7  ................
+00002f50: c2ff c2d7 c2ff c2d7 c1ff c8d7 c3ff c2d7  ................
+00002f60: c1ff c2d7 ccff c4d7 c2ff c2d7 c2ff c2d7  ................
+00002f70: c3ff c5d7 c3ff c3d7 c3ff c4d7 c2ff c4d7  ................
+00002f80: c2ff c3d7 c2ff c3d7 c1ff c2d7 c2ff c5d7  ................
+00002f90: c2ff c3d7 c2ff c3d7 c1ff c2d7 c1ff c4d7  ................
+00002fa0: ffff c9ff d2ff c4d7 c2ff c2d7 c1ff c2d7  ................
+00002fb0: c1ff c2d7 c2ff c1d7 c2ff c2d7 c1ff c2d7  ................
+00002fc0: c1ff c2d7 c2ff c3d7 c1ff c1d7 cdff c3d7  ................
+00002fd0: c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002fe0: c1ff c2d7 c1ff c2d7 c2ff c3d7 c1ff c1d7  ................
+00002ff0: c1ff c2d7 c2ff c3d7 c1ff c3d7 c1ff c2d7  ................
+00003000: c2ff c8d7 d4ff c2d7 c3ff c2d7 c2ff c2d7  ................
+00003010: c2ff c4d7 c2ff c2d7 c2ff c2d7 ccff c4d7  ................
+00003020: c2ff c2d7 c2ff c2d7 c2ff c2d7 c1ff c1d7  ................
+00003030: c3ff c2d7 c1ff c2d7 c2ff c5d7 cbff c6d7  ................
+00003040: c1ff c2d7 c2ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00003050: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c1d7  ................
+00003060: c1ff c2d7 c2ff c1d7 c1ff c2d7 c1ff c2d7  ................
+00003070: c2ff c5d7 c1ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00003080: c1ff c2d7 c2ff c3d7 c1ff c3d7 c2ff c1d7  ................
+00003090: ffff c9ff d2ff c2d7 c1ff c1d7 c2ff c2d7  ................
+000030a0: c1ff c2d7 c1ff c3d7 c4ff c2d7 c1ff c5d7  ................
+000030b0: c2ff c2d7 d1ff c3d7 c2ff c2d7 c1ff c2d7  ................
+000030c0: c1ff c2d7 c1ff c2d7 c1ff c5d7 c2ff c2d7  ................
+000030d0: c4ff c2d7 c2ff c2d7 c6ff c2d7 c2ff c2d7  ................
+000030e0: c1ff c2d7 c1ff c2d7 d4ff c2d7 c4ff c5d7  ................
+000030f0: c1ff c2d7 c1ff c3d7 c1ff c2d7 c2ff c2d7  ................
+00003100: cbff c2d7 c1ff c3d7 c1ff c2d7 c2ff c2d7  ................
+00003110: c2ff c4d7 c3ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00003120: c1ff c2d7 cfff c2d7 c1ff c2d7 c2ff c2d7  ................
+00003130: c4ff c2d7 c1ff c2d7 c4ff c2d7 c1ff c3d7  ................
+00003140: c3ff c3d7 c3ff c5d7 c2ff c2d7 c1ff c2d7  ................
+00003150: c1ff c2d7 c1ff c2d7 c2ff c5d7 c2ff c2d7  ................
+00003160: c3ff c3d7 ffff cbff d2ff c2d7 c4ff c2d7  ................
+00003170: c1ff c2d7 c3ff c3d7 c2ff c2d7 c1ff c2d7  ................
+00003180: c5ff c2d7 ceff c1d7 c3ff c2d7 c2ff c2d7  ................
+00003190: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
+000031a0: c5ff c2d7 c4ff c2d7 c2ff c2d7 c4ff c4d7  ................
+000031b0: c2ff c2d7 c1ff c2d7 c1ff c2d7 cbff c3d7  ................
+000031c0: c6ff c2d7 c6ff c2d7 c2ff c2d7 c2ff c2d7  ................
+000031d0: c1ff c2d7 c2ff c2d7 c4ff c3d7 c4ff c2d7  ................
+000031e0: c2ff c2d7 c1ff c2d7 c2ff c2d7 c2ff c2d7  ................
+000031f0: c1ff c2d7 c2ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00003200: c1ff c2d7 c4ff c3d7 c9ff c1d7 c1ff c2d7  ................
+00003210: c2ff c2d7 c4ff c2d7 c1ff c2d7 c2ff c4d7  ................
+00003220: c3ff c3d7 c3ff c3d7 c1ff c2d7 c5ff c2d7  ................
+00003230: c1ff c2d7 c2ff c3d7 c3ff c2d7 c5ff c2d7  ................
+00003240: c5ff c3d7 ffff c9ff d2ff c2d7 c4ff c2d7  ................
+00003250: c1ff c2d7 c1ff c1d7 c2ff c2d7 c2ff c2d7  ................
+00003260: c1ff c2d7 c2ff c1d7 c2ff c2d7 ceff c2d7  ................
+00003270: c2ff c2d7 c2ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00003280: c1ff c2d7 c1ff c2d7 c2ff c1d7 c2ff c2d7  ................
+00003290: c4ff c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7  ................
+000032a0: c2ff c2d7 c1ff c2d7 c1ff c2d7 d4ff c2d7  ................
+000032b0: c5ff c2d7 c3ff c2d7 c2ff c2d7 c1ff c2d7  ................
+000032c0: c2ff c2d7 cbff c2d7 c2ff c2d7 c1ff c2d7  ................
+000032d0: c2ff c2d7 c2ff c2d7 c2ff c2d7 c1ff c2d7  ................
+000032e0: c1ff c2d7 c2ff c2d7 c1ff c2d7 cbff c2d7  ................
+000032f0: c2ff c1d7 c2ff c2d7 c2ff c2d7 c4ff c2d7  ................
+00003300: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c1d7  ................
+00003310: c2ff c2d7 c1ff c1d7 c2ff c2d7 c1ff c2d7  ................
+00003320: c2ff c1d7 c2ff c2d7 c1ff c2d7 c1ff c1d7  ................
+00003330: c6ff c2d7 c2ff c1d7 c2ff c2d7 c3ff c1d7  ................
+00003340: c2ff c2d7 ffff c9ff d1ff c4d7 c4ff c3d7  ................
+00003350: c2ff c4d7 c3ff c3d7 c1ff c3d7 c2ff c4d7  ................
+00003360: cdff c1d7 c1ff c3d7 c4ff c9d7 c3ff c3d7  ................
+00003370: c2ff c4d7 c3ff c7d7 c3ff c8d7 c1ff c2d7  ................
+00003380: c1ff c3d7 d2ff c4d7 c2ff c3d7 c5ff c4d7  ................
+00003390: c3ff c4d7 cdff c4d7 c3ff c4d7 c2ff c4d7  ................
+000033a0: c1ff c7d7 c2ff c3d7 c1ff c3d7 caff c4d7  ................
+000033b0: c4ff c4d7 c5ff c4d7 c3ff c9d7 c2ff c4d7  ................
+000033c0: c3ff c3d7 c2ff c3d7 c1ff c8d7 c3ff c3d7  ................
+000033d0: c2ff c4d7 c2ff c4d7 ffff caff ffff ceff  ................
+000033e0: c2d7 ffff f8ff c2d7 e6ff c2d7 e3ff c6d7  ................
+000033f0: ffff dbff ffff ceff c2d7 ffff f8ff c2d7  ................
+00003400: e6ff c2d7 e3ff c1d7 c4ff c1d7 ffff dbff  ................
+00003410: ffff cdff c4d7 ffff f6ff c4d7 e4ff c4d7  ................
+00003420: e3ff c4d7 ffff dcff ffff ffff ffff ffff  ................
+00003430: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+00003440: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+00003450: ffff ffff ffff f8ff ffff ffff ffff ffff  ................
+00003460: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+00003470: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+00003480: ffff ffff ffff f8ff ffff ffff ffff ffff  ................
+00003490: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+000034a0: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+000034b0: ffff ffff ffff f8ff ffff ffff ffff ffff  ................
+000034c0: ffff f8ff ffff ffff ffff ffff ffff f8ff  ................
+000034d0: ffff ffff ffff ffff ffff f8ff ffff ffff  ................
+000034e0: ffff ffff ffff f8ff 0c00 00ff ee00 eeef  ................
+000034f0: 00ef f000 f0f1 00f1 f200 f2f3 00f3 f400  ................
+00003500: f4f5 00f5 f600 f6a8 a8a8 b8b8 b8c8 c8c8  ................
+00003510: d8d8 d8e8 e8e8 fcfc fc34 3c48 444c 5c58  .........4<HDL\X
+00003520: 6070 6c74 8484 8c98 9ca0 acb0 b8c4 ccd0  `plt............
+00003530: dc30 2c04 403c 0c50 4c14 605c 1c78 7840  .0,.@<.PL.`\.xx@
+00003540: 9494 64b0 b084 cccc a864 6464 7474 7468  ..d......dddttth
+00003550: 502c 7c68 4898 845c b8a0 78d4 bc94 f4dc  P,|hH..\..x.....
+00003560: b084 8484 5804 1070 1020 8820 34a0 384c  ....X..p. . 4.8L
+00003570: bc54 6ccc 687c dc84 90ec 9ca4 fcbc c0fc  .Tl.h|..........
+00003580: d000 fce8 3cfc fc80 4c28 0060 3c08 7458  ....<...L(.`<.tX
+00003590: 1c88 7438 9c88 50b0 9c6c c4b4 8844 1800  ..t8..P..l...D..
+000035a0: 602c 0480 4408 9c60 10b8 7818 d49c 20e8  `,..D..`..x... .
+000035b0: b810 fcd4 00fc f880 fcfc c020 0400 4014  ........... ..@.
+000035c0: 0854 1c10 6c2c 1c80 3828 9448 38a8 5c4c  .T..l,..8(.H8.\L
+000035d0: b86c 58c4 806c d494 8008 3400 1040 0020  .lX..l....4..@. 
+000035e0: 5004 3060 0440 700c 5484 1468 941c 80a8  P.0`.@p.T..h....
+000035f0: 2c40 4040 2c44 203c 5830 5068 3c68 7c4c  ,@@@,D <X0Ph<h|L
+00003600: 8094 5c98 b06c b4cc 7c10 3418 2048 2c38  ..\..l..|.4. H,8
+00003610: 6048 4c74 5860 886c 78a4 8898 c0a8 b8dc  `HLtX`.lx.......
+00003620: c820 1800 381c 0050 5050 5834 0c68 4018  . ..8..PPPX4.h@.
+00003630: 7c54 2c8c 6c40 a080 584c 2810 6034 1874  |T,.l@..XL(.`4.t
+00003640: 4428 8854 38a4 6040 b870 50cc 8060 d494  D(.T8.`@.pP..`..
+00003650: 70e0 a880 ecbc 9450 1c04 6428 1478 3828  p......P..d(.x8(
+00003660: 8c4c 40a0 6460 b888 8824 2844 3034 5440  .L@.d`...$(D04T@
+00003670: 4064 5050 7464 6488 8484 a4ac acc0 d4d4  @dPPtdd.........
+00003680: e030 3030 402c 9058 40ac 684c c478 58e0  .000@,.X@.hL.xX.
+00003690: 8c68 fca0 88fc bca8 fc00 186c 0024 8400  .h.........l.$..
+000036a0: 34a0 0048 b800 60d4 1878 dc38 90e8 58a8  4..H..`..x.8..X.
+000036b0: f080 c4fc bce0 fc10 4060 1850 6c28 6078  ........@`.Pl(`x
+000036c0: 3470 8450 8ca0 74ac c09c ccdc ccf0 fcac  4p.P..t.........
+000036d0: 3434 d434 34fc 3434 fc64 58fc 907c fcb8  44.44.44.dX..|..
+000036e0: a0fc d8c8 fcf4 ec48 1470 5c2c 8c70 44a8  .......H.p\,.pD.
+000036f0: 8c64 c4a8 88e0 c8b0 f8d0 b8ff e8d0 fc3c  .d.............<
+00003700: 0000 5c00 0080 0000 a000 00c4 0000 e000  ..\.............
+00003710: 00fc 0000 fc50 00fc 6c00 fc88 00fc a400  .....P..l.......
+00003720: fcc0 00fc dc00 fcfc 00cc 8808 e490 04fc  ................
+00003730: 9c00 fcb0 30fc c464 fcd8 9808 1858 0c24  ....0..d.....X.$
+00003740: 6814 347c 1c44 8c28 5ca4 3878 bc48 98d8  h.4|.D.(\.8x.H..
+00003750: 64ac e05c 9c34 6cb0 407c c84c 90e0 5ce0  d..\.4l.@|.L..\.
+00003760: f4fc c8ec f8b4 dcec 84bc d858 98ac 1010  ...........X....
+00003770: 1020 2020 2044 7024 4874 284c 782c 507c  .    Dp$Ht(Lx,P|
+00003780: 3054 8048 6490 6484 a8d8 f4fc 6080 a444  0T.Hd.d.....`..D
+00003790: 608c 4c18 086c 2c18 9048 34b0 6c54 d292  `.L..l,..H4.lT..
+000037a0: 7efc 3c00 fc54 00fc 6800 fc7c 00fc 9400  ~.<..T..h..|....
+000037b0: fcac 00fc c400 4000 00ff 0000 3030 0040  ......@.....00.@
+000037c0: 4000 5050 00ff ff00 9494 94f7 00f7 f800  @.PP............
+000037d0: f8f9 00f9 fa00 fafb 00fb fc00 fcfd 00fd  ................
+000037e0: fe00 feff 00ff ffff ff                   .........
```

### Comparing `nml-0.7.2/regression/opengfx_trains_start.pcx` & `nml-r1512/regression/opengfx_trains_start.pcx`

 * *Files 12% similar despite different names*

```diff
@@ -1,1040 +1,1027 @@
-00000000: 0a05 0108 0000 0000 9801 d100 4800 4800  ............H.H.
+00000000: 0a05 0108 0000 0000 9801 d100 2c01 2c01  ............,.,.
 00000010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000040: 0001 9a01 0100 0000 0000 0000 0000 0000  ................
+00000040: 0001 9901 0100 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-00000090: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-000000a0: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-000000b0: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-000000c0: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-000000d0: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-000000e0: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-000000f0: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-00000100: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-00000110: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-00000120: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-00000130: ffdf ff00 ffff ffff ffff ffff ffff ffff  ................
-00000140: dfff 00ff ffff ffff ffff ffff ffff ffdf  ................
-00000150: ff00 ffff ffff ffff ffff ffff ffff dfff  ................
-00000160: 00ff ffff ffff ffff ffff ffff ffdf ff00  ................
-00000170: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-00000180: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-00000190: ffff ffff ffff ffff ffff dfff 00d7 ffc8  ................
-000001a0: d7cf ffc3 d7d7 ffc3 d7c1 ffc5 d7c1 ffc3  ................
-000001b0: d7c1 ffc2 d7c1 ffc3 d7c1 ffc3 d7cc ffc3  ................
-000001c0: d7c7 ffc4 d7c7 ffc4 d7cc ff00 c6d7 00c8  ................
-000001d0: ffc7 00c1 d8c1 d758 c210 88c3 00d0 ffc8  .......X........
-000001e0: 00c1 d858 c1d7 c1d8 c1d7 c258 c2d7 c1d8  ...X.......X....
-000001f0: c200 ccff c400 c2d8 ca00 d0ff 00c3 d8c2  ................
-00000200: 8858 00c8 ffca 00c2 88c4 00d0 ffc2 00c1  .X..............
-00000210: d8c2 d7c2 58c1 d7c1 d8c1 d758 c1d8 c800  ....X......X....
-00000220: ccff c300 c1d7 c210 58c1 d7c1 d8c7 00f8  ........X.......
-00000230: ff00 d7ff c1d7 c2ff c2d7 c2ff c1d7 d0ff  ................
-00000240: c2d7 d8ff c2d7 c3ff c2d7 c3ff c1d7 c2ff  ................
-00000250: c2d7 c2ff c2d7 c2ff c2d7 cbff c5d7 c5ff  ................
-00000260: c2d7 c2ff c2d7 c5ff c2d7 c2ff c2d7 cbff  ................
-00000270: c1d7 c1d8 c1d7 c1d8 58c1 d758 c1d7 c8ff  ........X..X....
-00000280: c500 c1d8 8858 c288 c1d7 8810 88c1 d800  .....X..........
-00000290: d0ff c700 88c1 d8c1 d7c1 d8c1 d7c4 88c1  ................
-000002a0: d758 c1d7 00cc ffc2 00c2 88c2 58c2 d710  .X..........X...
-000002b0: c288 c500 d0ff c2d8 88c2 d7c3 58c8 ffc5  ............X...
-000002c0: 00c2 8810 c2d7 c1d8 58c2 88c2 00d0 ff00  ........X.......
-000002d0: c1d7 58c1 d7c4 88c1 d7c1 d8c1 d7c1 d888  ..X.............
-000002e0: c700 ccff 00c1 d788 1088 c2d7 8858 88c1  .............X..
-000002f0: d8c5 00f8 ff00 daff c2d7 d3ff c2d7 d8ff  ................
-00000300: c2d7 c3ff c2d7 c3ff c1d7 c6ff c2d7 c2ff  ................
-00000310: c2d7 caff c1d7 c3ff c2d7 c5ff c2d7 c2ff  ................
-00000320: c2d7 c5ff c2d7 c2ff c2d7 cbff c1d7 58c1  ..............X.
-00000330: d7c1 d8c3 88c1 d8c8 ffc4 00c2 d7c2 d888  ................
-00000340: 2088 6ac3 d888 d0ff 0058 88c1 d8c1 d788   .j......X......
-00000350: c1d8 c1d7 88c1 d788 c1d7 58c2 d758 c1d7  ..........X..X..
-00000360: 88c2 d7cc ffc2 d7c2 d8c2 d788 1088 c1d7  ................
-00000370: c1d8 5888 c300 d0ff c2d8 88c1 d888 c358  ..X............X
-00000380: c8ff c300 8858 c1d8 c1d7 8810 88c1 d8c1  .....X..........
-00000390: d7c2 6a58 88d0 ffc2 d788 c1d7 58c2 d758  ..jX........X..X
-000003a0: c1d7 88c1 d788 c1d7 c1d8 88c1 d7c1 d888  ................
-000003b0: 5800 ccff 88c1 d8c2 d76a 8820 88c2 d8c2  X........j. ....
-000003c0: d7c4 00f8 ff00 daff c2d7 c4ff c3d7 c2ff  ................
-000003d0: c3d7 c1ff c2d7 c2ff c4d7 c2ff c3d7 c2ff  ................
-000003e0: c3d7 c1ff c2d7 ccff c2d7 c2ff c2d7 c3ff  ................
-000003f0: c1d7 c1ff c3d7 c2ff c2d7 c2ff c2d7 c2ff  ................
-00000400: c4d7 c8ff c2d7 c5ff c3d7 c1ff c1d7 c6ff  ................
-00000410: c2d7 c2ff c2d7 cbff c2d7 58c1 d7c1 d8c1  ..........X.....
-00000420: d758 c1d8 c8ff c200 c288 c258 c2d7 c4d8  .X.........X....
-00000430: 8858 c1cb 0ad0 ff00 8858 88c1 d8c2 58c1  .X.......X....X.
-00000440: d788 58c1 d758 c1d7 c2d8 c1d7 c1d8 88c2  ..X..X..........
-00000450: d7cc ff20 c1c9 c2d7 c2d8 c1d7 c2d8 5888  ... ..........X.
-00000460: c3d8 8800 d0ff c2d8 88c1 d888 c358 c8ff  .............X..
-00000470: 00c1 d7c3 d888 58c2 d8c2 d788 c258 c1cb  ......X......X..
-00000480: 0ad0 ffc2 d788 c1d8 c1d7 c2d8 c1d7 58c1  ..............X.
-00000490: d758 88c1 d7c2 58c1 d888 5888 00cc ff21  .X....X...X....!
-000004a0: c1c9 c2d8 c2d7 c2d8 c2d7 c258 6a58 c200  ...........XjX..
-000004b0: f8ff 00da ffc2 d7c3 ffc2 d7c1 ffc2 d7c2  ................
-000004c0: ffc5 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1  ................
-000004d0: ffc2 d7c2 ffc3 d7c1 ffc1 d7cc ffc2 d7c1  ................
-000004e0: ffc1 d7c1 ffc2 d7c1 ffc1 d7c3 ffc2 d7c2  ................
-000004f0: ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc1 d7c8  ................
-00000500: ffc1 d7c7 ffc4 d7c6 ffc2 d7c2 ffc2 d7cb  ................
-00000510: ffc1 d7c3 88c1 d7c1 d8c1 d7c1 d8c8 ffc2  ................
-00000520: 88c2 58c2 886a 88c2 d7c1 d888 c2cb c1ca  ..X..j..........
-00000530: 0bd0 ff00 886a c288 6a58 88ca d7c2 d8cc  .....j..jX......
-00000540: ff21 c3c9 c2d7 8858 10c1 d8c2 10c1 d7c2  .!.....X........
-00000550: d8c1 d7d0 ffc8 d7c8 ffc1 d7c2 d8c1 d7c2  ................
-00000560: 10c1 d810 5888 c2d7 c2cb c1ca 28d0 ffc2  ....X.......(...
-00000570: d8ca d788 586a c288 6a88 00cc ff28 c3c9  ....Xj..j....(..
-00000580: c2d8 c2d7 886a c2d7 c388 58f8 ff00 daff  .....j....X.....
-00000590: c2d7 c3ff c5d7 c2ff c2d7 c1ff c2d7 c1ff  ................
-000005a0: c2d7 c1ff c2d7 c1ff c5d7 c2ff c2d7 cfff  ................
-000005b0: c2d7 c1ff c1d7 c1ff c2d7 c1ff c1d7 c3ff  ................
-000005c0: c2d7 c2ff c2d7 c2ff c2d7 c1ff c3d7 c9ff  ................
-000005d0: c1d7 c7ff c2d7 c1ff c3d7 c5ff c2d7 c2ff  ................
-000005e0: c2d7 cbff c1d7 58c1 d758 c1d7 88c1 d7c1  ......X..X......
-000005f0: d8c8 ffc2 d788 586a 20c2 58c1 d858 c2cb  ......Xj .X..X..
-00000600: c1ca c2cb 0bd0 ff00 c558 c1d7 cbd8 88c1  .........X......
-00000610: d8cc ff28 c2c9 c1ca c2c9 c3d7 10c2 d8c4  ...(............
-00000620: d7d0 ffc1 d758 c1d7 c1d8 c1d7 58c1 d8c1  .....X......X...
-00000630: d7c8 ffc4 d7c2 d810 c3d7 c5cb 0ad0 ffc1  ................
-00000640: d888 cbd8 c1d7 c558 00cc ff28 c2c9 c1ca  .......X...(....
-00000650: c2c9 c2d8 c258 886a c258 c1d8 88f8 ff00  .....X.j.X......
-00000660: daff c2d7 c3ff c2d7 c5ff c2d7 c1ff c2d7  ................
-00000670: c1ff c2d7 c1ff c2d7 c1ff c2d7 c5ff c2d7  ................
-00000680: c6ff c3d7 c7ff c2d7 c3ff c2d7 c4ff c2d7  ................
-00000690: c2ff c2d7 c2ff c2d7 c3ff c3d7 c6ff c1d7  ................
-000006a0: c4ff c3d7 c1ff c2d7 c2ff c2d7 c1ff c3d7  ................
-000006b0: c1ff c2d7 c2ff c2d7 cbff c2d7 c1d8 c1d7  ................
-000006c0: 58c1 d758 c1d8 c8ff c4d7 5888 c2d8 c2cb  X..X......X.....
-000006d0: c2ca c2cb c1ca 28d0 ff00 2888 c4ca c1c9  ......(...(.....
-000006e0: c2c8 c1c9 c7ca 8828 ccff 28c1 c9c1 c8c3  .......(..(.....
-000006f0: cac2 c9c5 d7c1 d8c2 d7d0 ffc2 d7c1 d8c1  ................
-00000700: d7c2 88c1 d8c1 d7c8 ffc2 d7c1 d8c5 d7c6  ................
-00000710: cbc1 ca0b d0ff 2888 c4ca c1c9 c2c8 c1c9  ......(.........
-00000720: c7ca 8828 00cc ff28 c1c9 c1c8 c1c9 c2ca  ...(...(........
-00000730: c2c9 c2d8 c258 c3d8 88f8 ff00 daff c2d7  .....X..........
-00000740: c3ff c2d7 c2ff c1d7 c2ff c2d7 c1ff c2d7  ................
-00000750: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c1d7  ................
-00000760: c2ff c2d7 d0ff c2d7 c3ff c2d7 c4ff c2d7  ................
-00000770: c2ff c2d7 c2ff c2d7 c1ff c1d7 c2ff c2d7  ................
-00000780: c5ff c5d7 c5ff c2d7 c2ff c2d7 c5ff c2d7  ................
-00000790: c2ff c2d7 cbff c1d7 c2d8 c288 c3d8 c8ff  ................
-000007a0: c6d7 88c1 cbc2 cac2 cbc1 cac1 cbc1 d8c1  ................
-000007b0: d7d0 ff00 0b88 c1ca c1c9 cdca 880b ccff  ................
-000007c0: c2d8 c2ca c1c8 c1c9 c1ca c2c9 c1d8 c3d7  ................
-000007d0: c1d8 c2d7 d0ff c1d8 c1d7 88c1 d758 c1d7  .............X..
-000007e0: 8858 c8ff c2d7 c1d8 c3d7 c1d8 c1cb c1ca  .X..............
-000007f0: c3cb c1ca c1cb 88c1 d8d0 ff0b 88c1 cac1  ................
-00000800: c9c3 cac4 cbc6 ca88 0b00 ccff c1d7 c1d8  ................
-00000810: c2c9 c1c8 c1c9 c1ca c2c9 88c1 d788 c3d8  ................
-00000820: c1d7 f8ff 00d9 ffc4 d7c3 ffc3 d7c2 ffc3  ................
-00000830: d7c1 ffc3 d7c1 ffc5 d7c1 ffc3 d7c2 ffc4  ................
-00000840: d7cf ffc2 d7c3 ffc2 d7c3 ffd0 d7c5 ffc6  ................
-00000850: d7c6 ffc4 d7c7 ffc4 d7cc ffc1 d7c1 d888  ................
-00000860: c2d7 c258 6ac8 ffc6 d70c c3cb c1ca c1cb  ...Xj...........
-00000870: c2d8 586a d0ff c1d7 0b88 c4ca c2c8 c1c9  ..Xj............
-00000880: c1ca c1c9 c2ca c1c9 c2ca c1cb 880b ccff  ................
-00000890: 58c2 88c1 d8c2 c9c1 c8c2 c921 c3d7 c1d8  X..........!....
-000008a0: c2d7 d0ff c1d8 58c1 d758 c1d7 c1d8 c258  ......X..X.....X
-000008b0: c8ff c2d7 c1d8 c3d7 28c3 cbc1 cac1 cb88  ........(.......
-000008c0: c1d8 6a58 d0ff 0b88 c4ca c2c8 c1c9 c1ca  ..jX............
-000008d0: c1c9 c2ca c1c9 c2ca c1cb c1d8 0bc1 d7cc  ................
-000008e0: ff6a 58c2 d8c2 c9c1 c8c2 c921 c2d7 c1d8  .jX........!....
-000008f0: 88c1 d8c1 d7f8 ff00 ffff ffff d3ff c1d7  ................
-00000900: 8858 88c2 58c2 6ac8 ffc6 d70b c1cb c1ca  .X..X.j.........
-00000910: c1cb 58c1 d858 6ac2 00d0 ffc1 d70a 88cf  ..X..Xj.........
-00000920: c888 0acc ffc2 0058 c288 c1d8 c2c9 c1c8  .......X........
-00000930: 28c3 d7c1 d8c2 d7d0 ffc1 d8c6 d758 c8ff  (............X..
-00000940: c2d7 c1d8 c3d7 0ac1 cbc1 cac1 cb88 c1d8  ................
-00000950: 6a58 c200 d0ff 0a88 cfc8 880a c1d7 ccff  jX..............
-00000960: c200 6a58 c1d8 58c2 c9c1 c828 c1d7 c2d8  ..jX..X....(....
-00000970: 88c1 d8c1 d7f8 ff00 ffff ffff d3ff 88c1  ................
-00000980: d7c1 d8c5 88c8 ffc2 d869 c3d7 0bc1 cb88  .........i......
-00000990: c1d8 c600 d0ff 0088 c1d8 88c3 d888 c3d8  ................
-000009a0: 88c1 d8c2 88c3 d888 c1d7 ccff c600 88c1  ................
-000009b0: d8c1 c928 c2d7 c2d8 c2d7 d0ff c8d7 c8ff  ...(............
-000009c0: c2d7 c1d8 c3d7 0bc1 cb88 c1d8 c600 d0ff  ................
-000009d0: c1d7 88c3 d8c2 88c1 d888 c3d8 88c3 d888  ................
-000009e0: c1d8 8800 ccff c600 c2d8 c1c9 28c1 d7c1  ............(...
-000009f0: d869 c2d7 c1d8 f8ff 00ff ffff ffd3 ffc3  .i..............
-00000a00: d8c5 88c8 ffc2 00c2 d8c2 d728 886a 58c6  ...........(.jX.
-00000a10: 00d0 ffc2 0058 6ac2 d758 6ac5 00c2 6ac2  .....Xj..Xj...j.
-00000a20: d758 6a00 ccff c600 6ac2 8828 c4d7 c200  .Xj.....j..(....
-00000a30: d0ff c2d7 c1d8 88c2 d8c2 d7c8 ffc2 00c4  ................
-00000a40: d728 c1d8 6a58 c600 d0ff 006a 58c2 d7c2  .(..jX.....jX...
-00000a50: 6ac5 006a 58c2 d76a 58c2 00cc ffc6 0058  j..jX..jX......X
-00000a60: 6a88 28c1 d8c3 d7c2 00f8 ff00 ffff ffff  j.(.............
-00000a70: d3ff c2d8 c288 c258 c288 c8ff c400 c2d8  .......X........
-00000a80: 6a58 c800 f0ff c800 6a88 c2d7 c400 d0ff  jX......j.......
-00000a90: c2d7 c1d8 88c2 d8c2 d7c8 ffc4 00c2 d76a  ...............j
-00000aa0: 58c8 00f0 ffc8 0058 6ac1 d788 c400 f8ff  X......Xj.......
-00000ab0: 00ff ffff ffd3 ffc1 d8c2 88c2 58c3 88ff  ............X...
+00000080: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00000090: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+000000a0: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+000000b0: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+000000c0: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+000000d0: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+000000e0: dfff ffff ffff ffff ffff ffff ffff dfff  ................
+000000f0: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00000100: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00000110: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+00000120: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+00000130: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+00000140: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+00000150: dfff ffff ffff ffff ffff ffff ffff dfff  ................
+00000160: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00000170: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00000180: ffff ffff ffff ffff dfff d7ff c8d7 cfff  ................
+00000190: c3d7 d7ff c3d7 c1ff c5d7 c1ff c3d7 c1ff  ................
+000001a0: c2d7 c1ff c3d7 c1ff c3d7 ccff c3d7 c7ff  ................
+000001b0: c4d7 c7ff c4d7 ccff 00c6 d700 c8ff c700  ................
+000001c0: c1d8 c1d7 58c2 1088 c300 d0ff c800 c1d8  ....X...........
+000001d0: 58c1 d7c1 d8c1 d7c2 58c2 d7c1 d8c2 00cc  X.......X.......
+000001e0: ffc4 00c2 d8ca 00d0 ff00 c3d8 c288 5800  ..............X.
+000001f0: c8ff ca00 c288 c400 d0ff c200 c1d8 c2d7  ................
+00000200: c258 c1d7 c1d8 c1d7 58c1 d8c8 00cc ffc3  .X......X.......
+00000210: 00c1 d7c2 1058 c1d7 c1d8 c700 f8ff d7ff  .....X..........
+00000220: c1d7 c2ff c2d7 c2ff c1d7 d0ff c2d7 d8ff  ................
+00000230: c2d7 c3ff c2d7 c3ff c1d7 c2ff c2d7 c2ff  ................
+00000240: c2d7 c2ff c2d7 cbff c5d7 c5ff c2d7 c2ff  ................
+00000250: c2d7 c5ff c2d7 c2ff c2d7 cbff c1d7 c1d8  ................
+00000260: c1d7 c1d8 58c1 d758 c1d7 c8ff c500 c1d8  ....X..X........
+00000270: 8858 c288 c1d7 8810 88c1 d800 d0ff c700  .X..............
+00000280: 88c1 d8c1 d7c1 d8c1 d7c4 88c1 d758 c1d7  .............X..
+00000290: 00cc ffc2 00c2 88c2 58c2 d710 c288 c500  ........X.......
+000002a0: d0ff c2d8 88c2 d7c3 58c8 ffc5 00c2 8810  ........X.......
+000002b0: c2d7 c1d8 58c2 88c2 00d0 ff00 c1d7 58c1  ....X.........X.
+000002c0: d7c4 88c1 d7c1 d8c1 d7c1 d888 c700 ccff  ................
+000002d0: 00c1 d788 1088 c2d7 8858 88c1 d8c5 00f8  .........X......
+000002e0: ffda ffc2 d7d3 ffc2 d7d8 ffc2 d7c3 ffc2  ................
+000002f0: d7c3 ffc1 d7c6 ffc2 d7c2 ffc2 d7ca ffc1  ................
+00000300: d7c3 ffc2 d7c5 ffc2 d7c2 ffc2 d7c5 ffc2  ................
+00000310: d7c2 ffc2 d7cb ffc1 d758 c1d7 c1d8 c388  .........X......
+00000320: c1d8 c8ff c400 c2d7 c2d8 8820 886a c3d8  ........... .j..
+00000330: 88d0 ff00 5888 c1d8 c1d7 88c1 d8c1 d788  ....X...........
+00000340: c1d7 88c1 d758 c2d7 58c1 d788 c2d7 ccff  .....X..X.......
+00000350: c2d7 c2d8 c2d7 8810 88c1 d7c1 d858 88c3  .............X..
+00000360: 00d0 ffc2 d888 c1d8 88c3 58c8 ffc3 0088  ..........X.....
+00000370: 58c1 d8c1 d788 1088 c1d8 c1d7 c26a 5888  X............jX.
+00000380: d0ff c2d7 88c1 d758 c2d7 58c1 d788 c1d7  .......X..X.....
+00000390: 88c1 d7c1 d888 c1d7 c1d8 8858 00cc ff88  ...........X....
+000003a0: c1d8 c2d7 6a88 2088 c2d8 c2d7 c400 f8ff  ....j. .........
+000003b0: daff c2d7 c4ff c3d7 c2ff c3d7 c1ff c2d7  ................
+000003c0: c2ff c4d7 c2ff c3d7 c2ff c3d7 c1ff c2d7  ................
+000003d0: ccff c2d7 c2ff c2d7 c3ff c1d7 c1ff c3d7  ................
+000003e0: c2ff c2d7 c2ff c2d7 c2ff c4d7 c8ff c2d7  ................
+000003f0: c5ff c3d7 c1ff c1d7 c6ff c2d7 c2ff c2d7  ................
+00000400: cbff c2d7 58c1 d7c1 d8c1 d758 c1d8 c8ff  ....X......X....
+00000410: c200 c288 c258 c2d7 c4d8 8858 c1cb 0ad0  .....X.....X....
+00000420: ff00 8858 88c1 d8c2 58c1 d788 58c1 d758  ...X....X...X..X
+00000430: c1d7 c2d8 c1d7 c1d8 88c2 d7cc ff20 c1c9  ............. ..
+00000440: c2d7 c2d8 c1d7 c2d8 5888 c3d8 8800 d0ff  ........X.......
+00000450: c2d8 88c1 d888 c358 c8ff 00c1 d7c3 d888  .......X........
+00000460: 58c2 d8c2 d788 c258 c1cb 0ad0 ffc2 d788  X......X........
+00000470: c1d8 c1d7 c2d8 c1d7 58c1 d758 88c1 d7c2  ........X..X....
+00000480: 58c1 d888 5888 00cc ff21 c1c9 c2d8 c2d7  X...X....!......
+00000490: c2d8 c2d7 c258 6a58 c200 f8ff daff c2d7  .....XjX........
+000004a0: c3ff c2d7 c1ff c2d7 c2ff c5d7 c1ff c2d7  ................
+000004b0: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c3d7  ................
+000004c0: c1ff c1d7 ccff c2d7 c1ff c1d7 c1ff c2d7  ................
+000004d0: c1ff c1d7 c3ff c2d7 c2ff c2d7 c2ff c2d7  ................
+000004e0: c1ff c2d7 c2ff c1d7 c8ff c1d7 c7ff c4d7  ................
+000004f0: c6ff c2d7 c2ff c2d7 cbff c1d7 c388 c1d7  ................
+00000500: c1d8 c1d7 c1d8 c8ff c288 c258 c288 6a88  ...........X..j.
+00000510: c2d7 c1d8 88c2 cbc1 ca0b d0ff 0088 6ac2  ..............j.
+00000520: 886a 5888 cad7 c2d8 ccff 21c3 c9c2 d788  .jX.......!.....
+00000530: 5810 c1d8 c210 c1d7 c2d8 c1d7 d0ff c8d7  X...............
+00000540: c8ff c1d7 c2d8 c1d7 c210 c1d8 1058 88c2  .............X..
+00000550: d7c2 cbc1 ca28 d0ff c2d8 cad7 8858 6ac2  .....(.......Xj.
+00000560: 886a 8800 ccff 28c3 c9c2 d8c2 d788 6ac2  .j....(.......j.
+00000570: d7c3 8858 f8ff daff c2d7 c3ff c5d7 c2ff  ...X............
+00000580: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
+00000590: c5d7 c2ff c2d7 cfff c2d7 c1ff c1d7 c1ff  ................
+000005a0: c2d7 c1ff c1d7 c3ff c2d7 c2ff c2d7 c2ff  ................
+000005b0: c2d7 c1ff c3d7 c9ff c1d7 c7ff c2d7 c1ff  ................
+000005c0: c3d7 c5ff c2d7 c2ff c2d7 cbff c1d7 58c1  ..............X.
+000005d0: d758 c1d7 88c1 d7c1 d8c8 ffc2 d788 586a  .X............Xj
+000005e0: 20c2 58c1 d858 c2cb c1ca c2cb 0bd0 ff00   .X..X..........
+000005f0: c558 c1d7 cbd8 88c1 d8cc ff28 c2c9 c1ca  .X.........(....
+00000600: c2c9 c3d7 10c2 d8c4 d7d0 ffc1 d758 c1d7  .............X..
+00000610: c1d8 c1d7 58c1 d8c1 d7c8 ffc4 d7c2 d810  ....X...........
+00000620: c3d7 c5cb 0ad0 ffc1 d888 cbd8 c1d7 c558  ...............X
+00000630: 00cc ff28 c2c9 c1ca c2c9 c2d8 c258 886a  ...(.........X.j
+00000640: c258 c1d8 88f8 ffda ffc2 d7c3 ffc2 d7c5  .X..............
+00000650: ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1  ................
+00000660: ffc2 d7c5 ffc2 d7c6 ffc3 d7c7 ffc2 d7c3  ................
+00000670: ffc2 d7c4 ffc2 d7c2 ffc2 d7c2 ffc2 d7c3  ................
+00000680: ffc3 d7c6 ffc1 d7c4 ffc3 d7c1 ffc2 d7c2  ................
+00000690: ffc2 d7c1 ffc3 d7c1 ffc2 d7c2 ffc2 d7cb  ................
+000006a0: ffc2 d7c1 d8c1 d758 c1d7 58c1 d8c8 ffc4  .......X..X.....
+000006b0: d758 88c2 d8c2 cbc2 cac2 cbc1 ca28 d0ff  .X...........(..
+000006c0: 0028 88c4 cac1 c9c2 c8c1 c9c7 ca88 28cc  .(............(.
+000006d0: ff28 c1c9 c1c8 c3ca c2c9 c5d7 c1d8 c2d7  .(..............
+000006e0: d0ff c2d7 c1d8 c1d7 c288 c1d8 c1d7 c8ff  ................
+000006f0: c2d7 c1d8 c5d7 c6cb c1ca 0bd0 ff28 88c4  .............(..
+00000700: cac1 c9c2 c8c1 c9c7 ca88 2800 ccff 28c1  ..........(...(.
+00000710: c9c1 c8c1 c9c2 cac2 c9c2 d8c2 58c3 d888  ............X...
+00000720: f8ff daff c2d7 c3ff c2d7 c2ff c1d7 c2ff  ................
+00000730: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
+00000740: c2d7 c2ff c1d7 c2ff c2d7 d0ff c2d7 c3ff  ................
+00000750: c2d7 c4ff c2d7 c2ff c2d7 c2ff c2d7 c1ff  ................
+00000760: c1d7 c2ff c2d7 c5ff c5d7 c5ff c2d7 c2ff  ................
+00000770: c2d7 c5ff c2d7 c2ff c2d7 cbff c1d7 c2d8  ................
+00000780: c288 c3d8 c8ff c6d7 88c1 cbc2 cac2 cbc1  ................
+00000790: cac1 cbc1 d8c1 d7d0 ff00 0b88 c1ca c1c9  ................
+000007a0: cdca 880b ccff c2d8 c2ca c1c8 c1c9 c1ca  ................
+000007b0: c2c9 c1d8 c3d7 c1d8 c2d7 d0ff c1d8 c1d7  ................
+000007c0: 88c1 d758 c1d7 8858 c8ff c2d7 c1d8 c3d7  ...X...X........
+000007d0: c1d8 c1cb c1ca c3cb c1ca c1cb 88c1 d8d0  ................
+000007e0: ff0b 88c1 cac1 c9c3 cac4 cbc6 ca88 0b00  ................
+000007f0: ccff c1d7 c1d8 c2c9 c1c8 c1c9 c1ca c2c9  ................
+00000800: 88c1 d788 c3d8 c1d7 f8ff d9ff c4d7 c3ff  ................
+00000810: c3d7 c2ff c3d7 c1ff c3d7 c1ff c5d7 c1ff  ................
+00000820: c3d7 c2ff c4d7 cfff c2d7 c3ff c2d7 c3ff  ................
+00000830: d0d7 c5ff c6d7 c6ff c4d7 c7ff c4d7 ccff  ................
+00000840: c1d7 c1d8 88c2 d7c2 586a c8ff c6d7 0cc3  ........Xj......
+00000850: cbc1 cac1 cbc2 d858 6ad0 ffc1 d70b 88c4  .......Xj.......
+00000860: cac2 c8c1 c9c1 cac1 c9c2 cac1 c9c2 cac1  ................
+00000870: cb88 0bcc ff58 c288 c1d8 c2c9 c1c8 c2c9  .....X..........
+00000880: 21c3 d7c1 d8c2 d7d0 ffc1 d858 c1d7 58c1  !..........X..X.
+00000890: d7c1 d8c2 58c8 ffc2 d7c1 d8c3 d728 c3cb  ....X........(..
+000008a0: c1ca c1cb 88c1 d86a 58d0 ff0b 88c4 cac2  .......jX.......
+000008b0: c8c1 c9c1 cac1 c9c2 cac1 c9c2 cac1 cbc1  ................
+000008c0: d80b c1d7 ccff 6a58 c2d8 c2c9 c1c8 c2c9  ......jX........
+000008d0: 21c2 d7c1 d888 c1d8 c1d7 f8ff ffff ffff  !...............
+000008e0: d3ff c1d7 8858 88c2 58c2 6ac8 ffc6 d70b  .....X..X.j.....
+000008f0: c1cb c1ca c1cb 58c1 d858 6ac2 00d0 ffc1  ......X..Xj.....
+00000900: d70a 88cf c888 0acc ffc2 0058 c288 c1d8  ...........X....
+00000910: c2c9 c1c8 28c3 d7c1 d8c2 d7d0 ffc1 d8c6  ....(...........
+00000920: d758 c8ff c2d7 c1d8 c3d7 0ac1 cbc1 cac1  .X..............
+00000930: cb88 c1d8 6a58 c200 d0ff 0a88 cfc8 880a  ....jX..........
+00000940: c1d7 ccff c200 6a58 c1d8 58c2 c9c1 c828  ......jX..X....(
+00000950: c1d7 c2d8 88c1 d8c1 d7f8 ffff ffff ffd3  ................
+00000960: ff88 c1d7 c1d8 c588 c8ff c2d8 69c3 d70b  ............i...
+00000970: c1cb 88c1 d8c6 00d0 ff00 88c1 d888 c3d8  ................
+00000980: 88c3 d888 c1d8 c288 c3d8 88c1 d7cc ffc6  ................
+00000990: 0088 c1d8 c1c9 28c2 d7c2 d8c2 d7d0 ffc8  ......(.........
+000009a0: d7c8 ffc2 d7c1 d8c3 d70b c1cb 88c1 d8c6  ................
+000009b0: 00d0 ffc1 d788 c3d8 c288 c1d8 88c3 d888  ................
+000009c0: c3d8 88c1 d888 00cc ffc6 00c2 d8c1 c928  ...............(
+000009d0: c1d7 c1d8 69c2 d7c1 d8f8 ffff ffff ffd3  ....i...........
+000009e0: ffc3 d8c5 88c8 ffc2 00c2 d8c2 d728 886a  .............(.j
+000009f0: 58c6 00d0 ffc2 0058 6ac2 d758 6ac5 00c2  X......Xj..Xj...
+00000a00: 6ac2 d758 6a00 ccff c600 6ac2 8828 c4d7  j..Xj.....j..(..
+00000a10: c200 d0ff c2d7 c1d8 88c2 d8c2 d7c8 ffc2  ................
+00000a20: 00c4 d728 c1d8 6a58 c600 d0ff 006a 58c2  ...(..jX.....jX.
+00000a30: d7c2 6ac5 006a 58c2 d76a 58c2 00cc ffc6  ..j..jX..jX.....
+00000a40: 0058 6a88 28c1 d8c3 d7c2 00f8 ffff ffff  .Xj.(...........
+00000a50: ffd3 ffc2 d8c2 88c2 58c2 88c8 ffc4 00c2  ........X.......
+00000a60: d86a 58c8 00f0 ffc8 006a 88c2 d7c4 00d0  .jX......j......
+00000a70: ffc2 d7c1 d888 c2d8 c2d7 c8ff c400 c2d7  ................
+00000a80: 6a58 c800 f0ff c800 586a c1d7 88c4 00f8  jX......Xj......
+00000a90: ffff ffff ffd3 ffc1 d8c2 88c2 58c3 88ff  ............X...
+00000aa0: ffe9 ffc2 d7c1 d888 c2d8 c2d7 ffff ffff  ................
+00000ab0: d2ff ffff ffff d3ff c1d8 88c2 58c4 88ff  ............X...
 00000ac0: ffe9 ffc2 d7c1 d888 c2d8 c2d7 ffff ffff  ................
-00000ad0: d2ff 00ff ffff ffd3 ffc1 d888 c258 c488  .............X..
-00000ae0: ffff e9ff c2d7 c1d8 88c2 d8c2 d7ff ffff  ................
-00000af0: ffd2 ff00 dbff c1d7 d5ff c2d7 ffff dfff  ................
-00000b00: c1d7 c1d8 c1d7 4669 c1d7 c1d8 c1d7 ffff  ......Fi........
-00000b10: e9ff c2d7 c1d8 88c2 d8c2 d7ff ffff ffd2  ................
-00000b20: ff00 daff c2d7 d2ff c1d7 c2ff c2d7 ffff  ................
-00000b30: dfff c2d7 c1d8 c2d7 c1d8 c2d7 ffff e9ff  ................
-00000b40: c8d8 ffff ffff d2ff 00da ffc3 d7d1 ffc1  ................
-00000b50: d7ff ffff ffff ffff ffff ffef ff00 d9ff  ................
-00000b60: c1d7 c1ff c2d7 c3ff c3d7 c1ff c2d7 c1ff  ................
-00000b70: c4d7 c1ff c7d7 c2ff c4d7 ffff ffff ffff  ................
-00000b80: ffff ffff e5ff 00d9 ffc1 d7c2 ffc2 d7c3  ................
-00000b90: ffc3 d7c1 ffc3 d7c1 ffc2 d7c2 ffc2 d7c2  ................
-00000ba0: ffc2 d7c1 ffc2 d7c1 ffc2 d7ff ffff ffff  ................
-00000bb0: ffff ffff ffe5 ff00 d9ff c5d7 c3ff c2d7  ................
-00000bc0: c3ff c2d7 c5ff c2d7 c2ff c2d7 c1ff c2d7  ................
-00000bd0: ffff ffff ffff ffff ffff e8ff 00d8 ffc1  ................
-00000be0: d7c3 ffc2 d7c3 ffc2 d7c3 ffc2 d7c5 ffc2  ................
-00000bf0: d7c2 ffc2 d7c1 ffc2 d7ff ffff ffff ffff  ................
-00000c00: ffff ffe8 ff00 d8ff c1d7 c4ff c2d7 c2ff  ................
-00000c10: c2d7 c3ff c2d7 c2ff c1d7 c2ff c2d7 c2ff  ................
-00000c20: c2d7 c1ff c2d7 c2ff c1d7 ffff ffff ffff  ................
-00000c30: ffff ffff e5ff 00d7 ffc3 d7c2 ffc8 d7c3  ................
-00000c40: ffc3 d7c3 ffc7 d7c1 ffc3 d7ff ffff ffff  ................
-00000c50: ffff ffff ffe6 ff00 ffff ffff ffff ffff  ................
-00000c60: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-00000c70: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-00000c80: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-00000c90: ffdf ff00 ffff ffff ffff ffff ffff ffff  ................
-00000ca0: dfff 00ff ffff ffd4 ffc8 00c8 ffd4 00cc  ................
-00000cb0: ffca 00c7 88cb 00d4 ffd4 00cc ffc8 00c8  ................
-00000cc0: ffd4 00cc ffcb 00c7 88ca 00d4 ffd4 00d3  ................
-00000cd0: ff00 ffff ffff d4ff c3d7 c288 5888 58c8  ............X.X.
-00000ce0: ffc9 00c1 d7c1 d8c9 00cc ffca 00c2 586a  ..............Xj
-00000cf0: 586a c258 cb00 d4ff c900 c1d8 c1d7 c900  Xj.X............
-00000d00: ccff c3d7 c288 5888 58c8 ffc9 00c1 d7c1  ......X.X.......
-00000d10: d8c9 00cc ffcb 00c2 586a 586a c258 ca00  ........XjXj.X..
-00000d20: d4ff c900 c1d8 c1d7 c900 d3ff 00ff ffff  ................
-00000d30: ffd4 ffc3 d7c1 d888 58c2 88c8 ffc7 00c1  ........X.......
-00000d40: d7c3 d888 c1d8 c1d7 88c5 00cc ffc2 00c1  ................
-00000d50: d7c2 d8c3 88c1 d8c1 d7c2 6a20 6a20 c26a  ..........j j .j
-00000d60: c688 c2d8 c300 d4ff c500 88c1 d7c1 d888  ................
-00000d70: c3d8 c1d7 c700 ccff c3d7 c1d8 8858 c288  .............X..
-00000d80: c8ff c700 c1d7 c3d8 88c1 d8c1 d788 c500  ................
-00000d90: ccff c300 c1d7 c2d8 c388 c1d8 c1d7 c26a  ...............j
-00000da0: 206a 20c2 6ac6 88c2 d8c2 00d4 ffc5 0088   j .j...........
-00000db0: c1d7 c1d8 88c3 d8c1 d7c7 00d3 ff00 ffff  ................
-00000dc0: ffff d4ff c2d7 c1d8 88c1 d76a 5888 c8ff  ...........jX...
-00000dd0: c500 c1d7 c3d8 c288 c1d8 88c1 d8c3 58c3  ..............X.
-00000de0: 00cc ffc2 00c1 d888 c558 c1d8 c720 586a  .........X... Xj
-00000df0: 586a c358 88c3 00d4 ffc3 00c3 58c1 d888  Xj.X........X...
-00000e00: c1d8 c288 c3d8 c1d7 c500 ccff c2d7 c1d8  ................
-00000e10: 88c1 d76a 5888 c8ff c500 c1d7 c3d8 c288  ...jX...........
-00000e20: c1d8 88c1 d8c3 58c3 00cc ffc3 00c1 d888  ......X.........
-00000e30: c558 c1d8 c720 586a 586a c358 88c2 00d4  .X... XjXj.X....
-00000e40: ffc3 00c3 58c1 d888 c1d8 c288 c3d8 c1d7  ....X...........
-00000e50: c500 d3ff 00ff ffff ffd4 ffc1 d8c2 88c2  ................
-00000e60: 58c2 20c1 d8c8 ffc5 00c1 c781 c288 c2d8  X. .............
-00000e70: 88c2 58c1 d8c2 88c2 5800 ccff c200 88c2  ..X.....X.......
-00000e80: 58c3 6a58 88c1 c8c1 c984 8381 c1c9 c1ca  X.jX............
-00000e90: 6a58 c46a c258 c300 d4ff 00c2 d8c2 88c1  jX.j.X..........
-00000ea0: d8c2 5888 c2d8 c288 81c1 ccc5 00cc ffc1  ..X.............
-00000eb0: d8c2 88c2 58c2 20c1 d8c8 ffc5 00c1 c781  ....X. .........
-00000ec0: c288 c2d8 88c2 58c1 d8c2 88c2 5800 ccff  ......X.....X...
-00000ed0: c300 88c2 58c3 6a58 88c1 c8c1 c984 8381  ....X.jX........
-00000ee0: c1c9 c1ca 6a58 c46a c258 c200 d4ff 00c2  ....jX.j.X......
-00000ef0: d8c2 88c1 d8c2 5888 c2d8 c288 81c1 ccc5  ......X.........
-00000f00: 00d3 ff00 ffff ffff d4ff c1d8 c288 c258  ...............X
-00000f10: 2058 6ac8 ffc5 00c1 c783 c1c8 c1c9 88c2   Xj.............
-00000f20: 58c2 d8c1 cbc2 58c2 d800 ccff c200 8858  X.....X........X
-00000f30: c56a 88c1 cac1 c983 8483 c1cb c1ca 206a  .j............ j
-00000f40: c320 c26a 58c3 00d4 ff00 c2d7 c2d8 c1c9  . .jX...........
-00000f50: c2d8 c258 88c2 ca83 c1cb c500 ccff c1d8  ...X............
-00000f60: c288 c258 2058 6ac8 ffc5 00c1 c783 c1c8  ...X Xj.........
-00000f70: c1c9 88c2 58c2 d8c1 cbc2 58c2 d800 ccff  ....X.....X.....
-00000f80: c300 8858 c56a 88c1 cac1 c983 8483 c1cb  ...X.j..........
-00000f90: c1ca 206a c320 c26a 58c2 00d4 ff00 c2d7  .. j. .jX.......
-00000fa0: c2d8 c1c9 c2d8 c258 88c2 ca83 c1cb c500  .......X........
-00000fb0: d3ff 00ff ffff ffd4 ffc1 d8c2 88c2 5820  ..............X 
-00000fc0: 58c1 d8c8 ffc3 00c1 d888 c1d7 c1d8 c1c7  X...............
-00000fd0: c1c8 81c1 c9c1 cb83 81c1 cbc2 d8c1 cac2  ................
-00000fe0: 00cc ffc2 0028 00c8 cac3 cbc8 ca00 28c3  .....(........(.
-00000ff0: 00d4 ffc2 00c1 cac2 d7c1 c981 83c1 c9c1  ................
-00001000: ca81 c1ca c1cb c1d8 c1d7 c2d8 c300 ccff  ................
-00001010: c1d8 c288 c258 2058 c1d8 c8ff c300 c1d8  .....X X........
-00001020: 88c1 d7c1 d8c1 c7c1 c881 c1c9 c1cb 8381  ................
-00001030: c1cb c2d8 c1ca c200 ccff c300 2800 c8ca  ............(...
-00001040: c3cb c8ca 0028 c200 d4ff c200 c1ca c2d7  .....(..........
-00001050: c1c9 8183 c1c9 c1ca 81c1 cac1 cbc1 d8c1  ................
-00001060: d7c2 d8c3 00d3 ff00 f5ff c1d7 d5ff c2d7  ................
-00001070: cdff c3d7 c1ff c1d7 c6ff c3d7 eaff c1c7  ................
-00001080: c3c8 c2c9 c2ca c8ff 00c2 d8c2 88c1 d7c2  ................
-00001090: 58c1 d883 c1c9 c1ca 8483 c1ca 8381 c1ca  X...............
-000010a0: 1500 ccff c200 2858 c1c9 8483 81c2 cac7  ......(X........
-000010b0: cbc2 cc84 8381 c1cc 6a28 c300 d4ff 0020  ........j(..... 
-000010c0: c1ca 8183 c1ca 8381 c1ca c1cb 83c1 d8c2  ................
-000010d0: 58c1 d7c2 88c2 d800 ccff c1c7 c3c8 c2c9  X...............
-000010e0: c2ca c8ff 00c2 d8c2 88c1 d7c2 58c1 d883  ............X...
-000010f0: c1c9 c1ca 8483 c1ca 8381 c1ca 1500 ccff  ................
-00001100: c300 2858 c1c9 8483 81c2 cac7 cbc2 cc84  ..(X............
-00001110: 8381 c1cc 6a28 c200 d4ff 0020 c1ca 8183  ....j(..... ....
-00001120: c1ca 8381 c1ca c1cb 83c1 d8c2 58c1 d7c2  ............X...
-00001130: 88c2 d800 d3ff 00f4 ffc2 d7d2 ffc1 d7c2  ................
-00001140: ffc2 d7cc ffc2 d7c2 ffc2 d7c7 ffc2 d7ea  ................
-00001150: ffc1 c883 81c2 c983 81c1 cac8 ffc2 00c1  ................
-00001160: c7c2 d858 c288 c258 c1cb c3ca c1cb 8483  ...X...X........
-00001170: 4328 00cc ffc2 0028 58c1 c983 8483 c1ca  C(.....(X.......
-00001180: c5cb c1cc c1cb c1cc c2cb 8384 83c1 cc6a  ...............j
-00001190: 28c3 00d4 ff00 2840 8381 c1c9 c1ca c1c9  (.....(@........
-000011a0: c1ca c1c9 c2d8 c288 58c2 d8c1 cac2 00cc  ........X.......
-000011b0: ffc1 c883 81c2 c983 81c1 cac8 ffc2 00c1  ................
-000011c0: c7c2 d858 c288 c258 c1cb c3ca c1cb 8483  ...X...X........
-000011d0: 4328 00cc ffc3 0028 58c1 c983 8483 c1ca  C(.....(X.......
-000011e0: c5cb c1cc c1cb c1cc c2cb 8384 83c1 cc6a  ...............j
-000011f0: 28c2 00d4 ff00 2840 8381 c1c9 c1ca c1c9  (.....(@........
-00001200: c1ca c1c9 c2d8 c288 58c2 d8c1 cac2 00d3  ........X.......
-00001210: ff00 f4ff c3d7 d1ff c1d7 cfff c2d7 c4ff  ................
-00001220: c1d7 c7ff c2d7 eaff c1d7 c1d8 8858 c26a  .............X.j
-00001230: 5888 c8ff c200 80c1 c7c1 d7c2 d8c2 58c2  X.............X.
-00001240: d8c4 ca42 43c1 c958 00cc ffc2 0028 58c2  ...BC..X.....(X.
-00001250: 40c2 41c5 42c6 4334 43c2 346a 2858 c200  @.A.B.C4C.4j(X..
-00001260: d4ff 0058 c1c9 4041 c2ca c1c9 c1ca c2d7  ...X..@A........
-00001270: c2d8 c288 c1d7 c1ca 80c2 00cc ffc1 d7c1  ................
-00001280: d888 58c2 6a58 88c8 ffc2 0080 c1c7 c1d7  ..X.jX..........
-00001290: c2d8 c258 c2d8 c4ca 4243 c1c9 5800 ccff  ...X....BC..X...
-000012a0: c200 5828 58c2 40c2 41c5 42c6 4334 43c2  ..X(X.@.A.B.C4C.
-000012b0: 346a 28c2 00d4 ff00 58c1 c940 41c2 cac1  4j(.....X..@A...
-000012c0: c9c1 cac2 d7c2 d8c2 88c1 d7c1 ca80 c200  ................
-000012d0: d3ff 00f3 ffc1 d7c1 ffc2 d7c3 ffc3 d7c1  ................
-000012e0: ffc2 d7c1 ffc4 d7c1 ffc7 d7c2 ffc4 d7c5  ................
-000012f0: ffc2 d7c7 ffc3 d7c2 ffc4 d7c3 ffc3 d7c3  ................
-00001300: ffc3 d7c3 ffc4 d7c2 ffc3 d7d0 ffc2 d888  ................
-00001310: 5888 6a58 88c8 ff00 c228 c1c7 c2d7 c1c7  X.jX.....(......
-00001320: c2d8 8381 c2ca c242 c2c9 c1d8 8800 ccff  .......B........
-00001330: c200 1558 d3cb 6a0b 58c2 00d4 ff00 88c1  ...X..j.X.......
-00001340: d8c2 c940 41c2 ca81 83c2 d7c1 cac2 d7c1  ...@A...........
-00001350: cac2 0b00 ccff c2d8 8858 886a 5888 c8ff  .........X.jX...
-00001360: 00c2 28c1 c7c2 d7c1 c7c2 d883 81c2 cac2  ..(.............
-00001370: 42c2 c9c1 d888 00cc ffc2 0058 1558 d3cb  B..........X.X..
-00001380: 6a0b c200 d4ff 0088 c1d8 c2c9 4041 c2ca  j...........@A..
-00001390: 8183 c2d7 c1ca c2d7 c1ca c20b 00d3 ff00  ................
-000013a0: f3ff c1d7 c2ff c2d7 c3ff c3d7 c1ff c3d7  ................
-000013b0: c1ff c2d7 c2ff c2d7 c2ff c2d7 c1ff c2d7  ................
-000013c0: c1ff c2d7 c5ff c2d7 c6ff c2d7 c1ff c2d7  ................
-000013d0: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
-000013e0: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c1d7  ................
-000013f0: c1ff c2d7 c1ff c2d7 cfff c1d7 8858 c46a  .............X.j
-00001400: 88c8 ff00 2820 c228 c1d7 80c1 c7c1 ca84  ....( .(........
-00001410: 83c2 41c2 c988 c1d8 c300 ccff c200 20d5  ..A........... .
-00001420: d820 c300 d4ff c300 c1d8 88c2 c940 4183  . ...........@A.
-00001430: 81c1 c9c1 ca80 c1d7 c20b 200b 00cc ffc1  .......... .....
-00001440: d788 58c4 6a88 c8ff 0028 20c2 28c1 d780  ..X.j....( .(...
-00001450: c1c7 c1ca 8483 c241 c2c9 88c1 d8c3 00cc  .......A........
-00001460: ffc3 0020 d5d8 20c2 00d4 ffc3 00c1 d888  ... .. .........
-00001470: c2c9 4041 8381 c1c9 c1ca 80c1 d7c2 0b20  ..@A........... 
-00001480: 0b00 d3ff 00f3 ffc5 d7c3 ffc2 d7c3 ffc2  ................
-00001490: d7c5 ffc2 d7c2 ffc2 d7c1 ffc2 d7c8 ffc2  ................
-000014a0: d7c9 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-000014b0: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc3  ................
-000014c0: d7c3 ffc5 d7cf ffc1 d788 586a 886a 5888  ..........Xj.jX.
-000014d0: c8ff 00c2 88c2 20c2 28c1 c7c1 cac2 41c2  ...... .(.....A.
-000014e0: c9c1 d7c6 00cc ffc2 00c1 d758 6ac1 d758  ...........Xj..X
-000014f0: 6ac1 d7c9 00c1 d858 6ac1 d758 6ac1 d7c3  j......Xj..Xj...
-00001500: 00d4 ffc6 00c1 d7c2 c940 41c1 c9c1 cac2  .........@A.....
-00001510: 0bc2 20c2 8800 ccff c1d7 8858 6a88 6a58  .. ........Xj.jX
-00001520: 88c8 ff00 c288 c220 c228 c1c7 c1ca c241  ....... .(.....A
-00001530: c2c9 c1d7 c600 ccff c300 c1d7 586a c1d7  ............Xj..
-00001540: 586a c1d7 c900 c1d8 586a c1d7 586a c1d7  Xj......Xj..Xj..
-00001550: c200 d4ff c600 c1d7 c2c9 4041 c1c9 c1ca  ..........@A....
-00001560: c20b c220 c288 00d3 ff00 f2ff c1d7 c3ff  ... ............
-00001570: c2d7 c3ff c2d7 c3ff c2d7 c5ff c2d7 c2ff  ................
-00001580: c2d7 c1ff c2d7 c8ff c2d7 c7ff c4d7 c1ff  ................
-00001590: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
-000015a0: c2d7 c1ff c2d7 c3ff c3d7 c1ff c2d7 d2ff  ................
-000015b0: 58c6 d758 c8ff 00c2 d8c2 8820 28c1 c740  X..X....... (..@
-000015c0: c2c9 c1d7 c800 fcff c800 c1d7 c2c9 40c1  ..............@.
-000015d0: ca0b 20c2 88c2 d800 ccff 58c6 d758 c8ff  .. .......X..X..
-000015e0: 00c2 d8c2 8820 28c1 c740 c2c9 c1d7 c800  ..... (..@......
-000015f0: fcff c800 c1d7 c2c9 40c1 ca0b 20c2 88c2  ........@... ...
-00001600: d800 d3ff 00f2 ffc1 d7c4 ffc2 d7c2 ffc2  ................
-00001610: d7c3 ffc2 d7c2 ffc1 d7c2 ffc2 d7c2 ffc2  ................
-00001620: d7c1 ffc2 d7c2 ffc1 d7c6 ffc2 d7c3 ffc1  ................
-00001630: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-00001640: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-00001650: d7c1 ffc1 d7c2 ffc2 d7c1 ffc2 d7c2 ffc1  ................
-00001660: d7cf ffc1 c780 c1c7 c1d7 c1d8 c1c7 81c1  ................
-00001670: c9c8 ffc3 00c2 d8c2 8858 c1c9 88c1 d8c9  .........X......
-00001680: 00fc ffc9 00c1 d888 c1c9 58c2 88c2 d8c3  ..........X.....
-00001690: 00cc ffc1 c780 c1c7 c1d7 c1d8 c1c7 81c1  ................
-000016a0: c9c8 ffc3 00c2 d8c2 8858 c1c9 88c1 d8c9  .........X......
-000016b0: 00fc ffc9 00c1 d888 c1c9 58c2 88c2 d8c3  ..........X.....
-000016c0: 00d3 ff00 f1ff c3d7 c2ff c8d7 c3ff c3d7  ................
-000016d0: c3ff c7d7 c1ff c3d7 c8ff c4d7 c3ff c6d7  ................
-000016e0: c1ff c2d7 c3ff c3d7 c3ff c3d7 c2ff c4d7  ................
-000016f0: c3ff c3d7 d0ff c3c7 c1d7 c1d8 c1c8 c2c9  ................
-00001700: c8ff c500 c2d8 88c1 d8cb 00fc ffcb 00c1  ................
-00001710: d888 c2d8 c500 ccff c3c7 c1d7 c1d8 c1c8  ................
-00001720: c2c9 c8ff c500 c2d8 88c1 d8cb 00fc ffcb  ................
-00001730: 00c1 d888 c2d8 c500 d3ff 00ff ffff ffd4  ................
-00001740: ff28 2028 c1d7 c1d8 c228 15ff fff9 ff28  .( (.....(.....(
-00001750: 2028 c1d7 c1d8 c228 15ff ffff ffc1 ff00   (.....(........
-00001760: ffff ffff d4ff 2028 20c2 6a20 1528 ffff  ...... ( .j .(..
-00001770: f9ff 2028 20c2 6a20 1528 ffff ffff c1ff  .. ( .j .(......
-00001780: 00ff ffff ffd4 ffc8 d8ff fff9 ffc8 d8ff  ................
-00001790: ffff ffc1 ff00 ffff ffff d4ff c358 c2d8  .............X..
-000017a0: c358 ffff f9ff c358 c2d8 c358 ffff ffff  .X.....X...X....
-000017b0: c1ff 00ff ffff ffff ffff ffff ffff ffdf  ................
-000017c0: ff00 ffff ffff ffff ffff ffff ffff dfff  ................
-000017d0: 00ff ffff ffff ffff ffff ffff ffdf ff00  ................
-000017e0: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-000017f0: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-00001800: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-00001810: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-00001820: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00001830: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00001840: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-00001850: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-00001860: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-00001870: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-00001880: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-00001890: ffdf ff00 ffff ffff ffff ffff ffff ffff  ................
-000018a0: dfff 00ff ffff ffff ffff ffff ffff ffdf  ................
-000018b0: ff00 ffff ffff ffff ffff ffff ffff dfff  ................
-000018c0: 00ff ffff ffff ffff ffff ffff ffdf ff00  ................
-000018d0: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-000018e0: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-000018f0: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-00001900: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-00001910: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00001920: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00001930: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-00001940: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-00001950: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-00001960: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-00001970: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-00001980: ffdf ff00 ffff ffff ffff ffff ffff ffff  ................
-00001990: dfff 00ff ffff ffff ffff ffff ffff ffdf  ................
-000019a0: ff00 ffff ffff ffff ffff ffff ffff dfff  ................
-000019b0: 00ff ffff ffff ffff ffff ffff ffdf ff00  ................
-000019c0: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-000019d0: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-000019e0: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-000019f0: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-00001a00: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00001a10: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00001a20: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-00001a30: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-00001a40: ffff ffff dfff 00ff ffff ffd0 ff00 c1c6  ................
-00001a50: c4c8 c1c7 00c8 ffcd 00c1 c7c2 c9c1 c8c4  ................
-00001a60: 00ca ffce 00c2 c728 20c1 c7c1 c9c1 c7c1  .......( .......
-00001a70: c9c1 c7c1 c9c1 c7c1 c9c1 c7c5 00d1 ffc4  ................
-00001a80: 00c1 c9d0 00cb ff00 c2c8 c4c9 00c8 ffd0  ................
-00001a90: 00c1 c6c4 00cb ffc5 00c9 c720 28c2 c7ce  ........... (...
-00001aa0: 00d0 ffc4 00c1 c6c1 c7c2 c8cd 00d6 ff00  ................
-00001ab0: ffff ffff d0ff c1c6 c1c8 c4ca c1c9 c1c8  ................
-00001ac0: c8ff cb00 c1c7 c1c9 c2ca c2cb c1ca c1c9  ................
-00001ad0: c200 caff cd00 10c4 c9c2 cac5 cbc1 cac1  ................
-00001ae0: c912 c400 d1ff c200 c4ca c1c9 ce00 cbff  ................
-00001af0: c1c7 c1c9 c2ca c1cb c2ca c1c9 c8ff ce00  ................
-00001b00: c1c6 c1c9 c2ca c1c9 c200 cbff c400 c1d8  ................
-00001b10: c1c7 c1c8 c1c9 c3ca c3cb c2c9 c2cb 12cd  ................
-00001b20: 00d0 ffc2 00c1 c7c1 c9c4 cac1 c9c1 c8cb  ................
-00001b30: 00d6 ff00 ffff ffff d0ff c1c6 c4ca c1cb  ................
-00001b40: c1ca c1c9 c8ff c900 c1c7 8812 c1ca c4cb  ................
-00001b50: c2ca c1cc 00ca ff00 c3c6 c6c7 c2c8 c1c7  ................
-00001b60: 10c1 c9c1 cb20 58c5 cbc2 ccc1 cbc1 ca13  ..... X.........
-00001b70: c2cb c200 d1ff 00c1 cac4 cbc2 cac1 c9cc  ................
-00001b80: 00cb ffc1 c7c1 c9c1 cac1 cbc1 ccc1 cbc2  ................
-00001b90: cac8 ffcc 00c1 c6c1 c9c2 cac2 cbc2 ca00  ................
-00001ba0: cbff c200 c2c9 10c1 c8c1 cac4 cbc3 cc20  ............... 
-00001bb0: 28c1 ccc1 cd13 c2c8 c4c6 c6c7 00d0 ff00  (...............
-00001bc0: 10c1 c6c1 c8c1 cac3 cbc1 ca12 88c1 c8c9  ................
-00001bd0: 00d6 ff00 cdff c8d7 e4ff c2d7 c1ff c2d7  ................
-00001be0: c1ff c8d7 ccff c3d7 cbff c2d7 c1ff c2d7  ................
-00001bf0: e8ff c1c7 c1cb c2ca c2cb c2ca c8ff c700  ................
-00001c00: c1c7 1312 c2ca 8812 c1cc c1cb c1ca c1cc  ................
-00001c10: 13c1 cc20 caff 88c1 cac5 cbc1 cac1 cbc1  ... ............
-00001c20: cac2 c9c1 c810 c1c9 c3ca c2cb c1cc c1cb  ................
-00001c30: c1cc c4cb 14c2 ccbe 00d1 ffc2 c9c2 cac3  ................
-00001c40: cbc2 cac1 c9c1 c8c2 c9c1 c8c7 00cb ffc1  ................
-00001c50: c7c1 c9c1 cac1 cbc1 ccc1 cbc1 cac1 c9c8  ................
-00001c60: ffc7 00c2 c8c1 c9c1 c8c2 cac3 cbc3 ccc1  ................
-00001c70: cbc1 cacb ff00 bec2 ca11 c3c9 c2ca c7cb  ................
-00001c80: c1ca 15c1 c8c2 c9c6 cbc1 cac1 cbc1 ca88  ................
-00001c90: d0ff c288 10c2 c8c2 cb13 88c2 cb13 12c1  ................
-00001ca0: c8c7 00d6 ff00 cdff c1d7 c2ff c2d7 c2ff  ................
-00001cb0: c1d7 e4ff c2d7 c1ff c2d7 c1ff c1d7 c2ff  ................
-00001cc0: c2d7 c2ff c1d7 cdff c2d7 cbff c2d7 c1ff  ................
-00001cd0: c2d7 e8ff c1c8 1011 c1cb c1cc 1011 c1ca  ................
-00001ce0: c8ff c700 c1c7 12c1 ca11 12c3 cbc1 cc13  ................
-00001cf0: c2cd 1620 caff 88c1 cbc2 ccc3 cdc1 ccc2  ... ............
-00001d00: cbc1 cac2 c911 c1ca 12c1 cb12 c1cc 13c1  ................
-00001d10: cc13 c1cd 14c1 cdc3 14c2 cdc1 f510 d1ff  ................
-00001d20: 11c3 c9c3 cac1 c9c1 c8c1 c9c2 ca10 12c1  ................
-00001d30: c9c1 c8c5 00cb ffc1 c8c1 c9c1 cac1 cbc1  ................
-00001d40: ccc1 cbc2 cac8 ffc5 00c1 c8c1 c910 11c1  ................
-00001d50: cbc1 c9c2 cac1 cbc2 ccc1 cdc1 ccc2 cbc1  ................
-00001d60: cacb ff58 21c2 cac2 1211 c1ca 12c1 cb12  ...X!...........
-00001d70: c1cc 13c1 cc13 c1cd 14c1 cd17 c2c9 c1ca  ................
-00001d80: c3cc c3cd c1cc c1cd c1cc 88d0 ffc1 d812  ................
-00001d90: 11c1 c810 c2ca c2cb 1614 c1cb 14c1 cac7  ................
-00001da0: 00d6 ff00 d0ff c2d7 e7ff c2d7 c1ff c2d7  ................
-00001db0: c4ff c2d7 d0ff c2d7 cbff c2d7 c1ff c2d7  ................
-00001dc0: e8ff c1c9 11c1 cac1 cbc1 ccc1 cb12 c1c9  ................
-00001dd0: c8ff c500 c1c6 c3c9 c1c8 c1ca 12c1 cac1  ................
-00001de0: cb13 c2cd 17c2 0d58 caff c1d8 c1ca c3cb  .......X........
-00001df0: c1ca c1cb c1ca c1cb c3ca c1cb c1ca c1cb  ................
-00001e00: c1ca c1cc c1ca c1cc 13c1 cd14 c1cd 16c1  ................
-00001e10: cdc2 16c1 ccc2 16be 6ad1 ff12 c1f5 10c4  ........j.......
-00001e20: c9c1 c6c1 c8c1 ca10 12c2 cbc2 cac1 c9c1  ................
-00001e30: c8c3 00cb ffc1 c8c1 c9c1 cac2 ccc2 cac1  ................
-00001e40: c9c8 ffc3 00c1 c6c2 c9c2 cac1 cb11 13c2  ................
-00001e50: c9c1 cac1 cbc2 ccc1 cbc1 cac2 15cb ff6a  ...............j
-00001e60: bec2 13c1 c912 11c1 cb12 c1cb 12c1 cc14  ................
-00001e70: c6cd c1cb c2ca c8cb c1ca c1d8 d0ff c1d8  ................
-00001e80: c221 12c1 c9c1 ca10 c2cb 15c1 cbc1 cac2  .!..............
-00001e90: c9c1 cac1 c9c5 00d6 ff00 d0ff c2d7 c3ff  ................
-00001ea0: c3d7 c1ff c2d7 c1ff c3d7 c1ff c5d7 c1ff  ................
-00001eb0: c2d7 c2ff c3d7 c2ff c3d7 c1ff c2d7 cdff  ................
-00001ec0: c2d7 c3ff c3d7 c1ff c2d7 c1ff c3d7 c1ff  ................
-00001ed0: c6d7 c3ff c3d7 f0ff c1c9 c1ca c4cb c1ca  ................
-00001ee0: c1cc c8ff c300 c1c6 c1c9 c2ca c2cb c1ca  ................
-00001ef0: c2c9 13c2 cc17 0d0e c20c c1d8 caff 20c2  .............. .
-00001f00: cdc2 ccc2 cdc1 ccc5 cdc1 ccc1 cdc2 ccc8  ................
-00001f10: cdc1 ccc2 cdc2 0c28 58d1 ffc2 2811 2810  .......(X...(.(.
-00001f20: c1c9 c1c6 c211 c1c8 c1ca c2cb c1cc c2cb  ................
-00001f30: c2ca c1c8 c200 cbff c1c7 c1c9 c3ca c1c9  ................
-00001f40: c2ca c8ff c300 c1c8 c1c9 c2ca c2cb c1cc  ................
-00001f50: c1cb c1ca c1cc c1cd c2cb 1513 1517 15cb  ................
-00001f60: ffc1 d821 c2f5 c3cb c7cc c1cd c2ca c1cc  ...!............
-00001f70: c1ca c1cb c1cc c1ca c1cb c1cc c1ca c1cb  ................
-00001f80: c1cc c1ca c1cb c2cc 20d0 ffc1 d8c2 20c2  ........ ..... .
-00001f90: 2113 c1c8 c1ca 10c1 cbc1 cac1 c9c1 cac2  !...............
-00001fa0: cbc2 cac1 c9c3 00d6 ff00 d0ff c2d7 c4ff  ................
-00001fb0: c2d7 c1ff c2d7 c2ff c3d7 c1ff c1d7 c1ff  ................
-00001fc0: c5d7 c1ff c2d7 c1ff c2d7 c2ff c3d7 c1ff  ................
-00001fd0: c1d7 cdff c2d7 c4ff c2d7 c1ff c2d7 c2ff  ................
-00001fe0: c3d7 c1ff c3d7 c1ff c2d7 c1ff c2d7 c1ff  ................
-00001ff0: c2d7 efff c214 c1ca 1413 c1ca 1214 c8ff  ................
-00002000: 00c1 c6c1 c9c2 cac2 cbc2 ccc1 cdc2 cbc1  ................
-00002010: cc16 140e 0d0c 0ac1 c900 caff 6a0c 0e15  ............j...
-00002020: 130e 1513 0f14 130f 1412 0e13 110e c90d  ................
-00002030: 0ec2 17c1 f588 d1ff 58c2 2128 1112 11c1  ........X.!(....
-00002040: cac1 c910 c3ca c2cb c1cc 14c1 cc13 c200  ................
-00002050: cbff c1c6 c1c8 c6c9 c8ff c200 10c1 c914  ................
-00002060: c2ca c1cc c1cb c1ca c1cb 13c1 cdc1 cc13  ................
-00002070: 1517 160d 0c28 cbff c1d7 28c2 15ca 0b0e  .....(....(.....
-00002080: 1113 0e12 140f 1314 0f13 150e 1315 0e0c  ................
-00002090: 6ad0 ff00 c1c8 c220 c221 1110 c2c8 c3c9  j...... .!......
-000020a0: c2ca c2cb c1ca c2c9 00d6 ff00 d0ff c2d7  ................
-000020b0: c4ff c2d7 c1ff c2d7 c2ff c2d7 c4ff c2d7  ................
-000020c0: c1ff c2d7 c1ff c5d7 c2ff c2d7 d0ff c2d7  ................
-000020d0: c4ff c2d7 c1ff c2d7 c2ff c2d7 c3ff c2d7  ................
-000020e0: c1ff c2d7 c1ff c2d7 c1ff c2d7 efff c1cb  ................
-000020f0: 13c1 c8c2 cac1 c913 c1cc c8ff c2c7 c1c8  ................
-00002100: c2ca c1cb c1cc c1cd c2cc c1cb c1ca 130c  ................
-00002110: 150c 0b28 c1d7 c1c7 00ca ff58 0c0e 1615  ...(.......X....
-00002120: 0e16 150e 1614 0d15 140d 1312 ca0d 0ec2  ................
-00002130: 0c28 c1d8 d1ff c1d7 58c2 2021 2812 2820  .(......X. !(.( 
-00002140: c1c9 c1ca 10c3 ca16 15c1 cbc1 cc28 00cb  .............(..
-00002150: ffc1 c610 11c1 cac1 cb10 11c1 c9c8 ff00  ................
-00002160: 12c2 cb12 14c1 cbc2 ca13 c2cd 120d 1517  ................
-00002170: 0d0b 0a21 c1d7 cbff c1d7 20c1 f515 ca0b  ...!...... .....
-00002180: 0d12 130d 1415 0d14 160e 1516 0e15 160e  ................
-00002190: 0c58 d0ff 00c1 c6c1 d758 c220 6a11 c210  .X.......X. j...
-000021a0: c1c8 c3c9 c2ca c2c9 c3ca d6ff 00d0 ffc2  ................
-000021b0: d7c4 ffc2 d7c1 ffc2 d7c2 ffc2 d7c4 ffc2  ................
-000021c0: d7c1 ffc2 d7c1 ffc2 d7c5 ffc2 d7d0 ffc2  ................
-000021d0: d7c4 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3 ffc2  ................
-000021e0: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7ef ffc1  ................
-000021f0: c6c1 c7c1 cac2 cbc3 cac8 ffc2 10c1 d8c2  ................
-00002200: c8c2 cbc1 ccc1 cbc1 ca16 0d0c 0bc1 f50a  ................
-00002210: 28c1 d7c3 00ca ffc1 d80a cd0b 2821 c90b  (...........(!..
-00002220: 0c0b c20a 58c1 d7d1 ffc2 0058 6a20 21c2  ....X......Xj !.
-00002230: 28c2 f514 c1c8 c1ca 1012 c3cc 16bf 6acb  (.............j.
-00002240: ffc1 c711 c1ca c1cb c1cc c1cb 12c1 cac8  ................
-00002250: ff88 bf28 14c1 cbc1 ccc2 13c2 cd0e 0f13  ...(............
-00002260: c20d 0b0a 216a c200 cbff c2d7 21c2 f5ca  ....!j......!...
-00002270: 0a20 21ce 0ac1 d8d0 ffc3 00c1 d758 c26a  . !..........X.j
-00002280: c220 1121 10c1 c9c1 c8c2 c9c1 cac2 d8c2  . .!............
-00002290: cad6 ff00 d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
-000022a0: c2ff c2d7 c4ff c2d7 c1ff c2d7 c1ff c2d7  ................
-000022b0: c2ff c1d7 c2ff c2d7 d0ff c2d7 c4ff c2d7  ................
-000022c0: c1ff c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7  ................
-000022d0: c1ff c2d7 c1ff c2d7 efff c1c6 c1c9 c1ca  ................
-000022e0: c1cb c1cc c1cb c1ca c1c9 c8ff 10c2 d7c1  ................
-000022f0: d8c2 c9c1 cbc1 ca13 16c2 0d0c c1f5 2120  ..............! 
-00002300: c500 caff c1d8 28cc 150a 2821 c40a c2f5  ......(...(!....
-00002310: c328 c1f5 28c2 13c1 c600 d1ff c400 586a  .(..(.........Xj
-00002320: c221 20c1 f515 c1f5 14c2 cac1 cc0c bf6a  .! ............j
-00002330: 2821 cbff c1c8 c1c9 c1ca c1cb c1cc c1cb  (!..............
-00002340: c1ca c1c9 c8ff 88c1 d858 bfc1 f516 c1cc  .........X......
-00002350: c1cd c20e 0f0e c1f5 0b0a 286a c400 cbff  ..........(j....
-00002360: 00c1 c611 2120 28c3 21c2 28c4 f520 21cd  ....! (.!.(.. !.
-00002370: f528 c1d8 d0ff c500 c258 6a20 c221 1128  .(.......Xj .!.(
-00002380: 10c2 c9c1 ca10 c2d8 c1c8 d6ff 00cf ffc4  ................
-00002390: d7c4 ffc9 d7c2 ffc3 d7c1 ffc3 d7c1 ffc3  ................
-000023a0: d7c2 ffc4 d7ce ffc4 d7c4 ffc9 d7c2 ffc1  ................
-000023b0: d7c1 ffc2 d7c3 ffc3 d7f0 ffc1 c6c1 c9c1  ................
-000023c0: cac1 cbc1 ccc1 cbc2 cac8 ffc1 d8c3 d710  ................
-000023d0: c1c7 150f 160d 0c0a 2820 c700 caff 6a58  ........( ....jX
-000023e0: c520 c821 c26a c421 8858 c3d7 c288 c1d7  . .!.j.!.X......
-000023f0: c1c8 c1c6 00d1 ffc6 0058 c26a c228 c1f5  .........X.j.(..
-00002400: 15c2 0a0c 6a20 5820 6acb ffc1 c9c2 cac3  ....j X j.......
-00002410: cbc2 cac8 ffc1 d888 c36a 0d0e c20f 0e0d  .........j......
-00002420: 0bc2 286a c600 cbff 00c1 c6c1 c8c1 d7c2  ..(j............
-00002430: 88c3 d7c2 88c4 20c2 6acd 2058 6ad0 ffc7  ...... .j. Xj...
-00002440: 0058 6ac2 2021 2812 28c1 cac1 c9c2 d8c1  .Xj. !(.(.......
-00002450: d7c1 d8d6 ff00 ffff ffff d0ff c1c6 c1c9  ................
-00002460: c1ca c2cc c2ca c1c9 c8ff c4d7 c1d8 1017  ................
-00002470: 0d0b 0ac1 f520 c900 fbff c800 5820 2128  ..... ......X !(
-00002480: c1f5 0a0b 0ac2 586a 58c1 d8cb ffc1 c9c5  ......XjX.......
-00002490: cac1 cbc1 c9c8 ffc1 d7c1 d8c3 880c c20e  ................
-000024a0: 0d0b 0a28 6ac8 00fb ffc9 0058 6ac2 2021  ...(j......Xj. !
-000024b0: 28c1 ca10 c1d8 c3d7 d6ff 00ff ffff ffd0  (...............
-000024c0: ffc1 c6c1 c8c2 cac2 cbc2 cac8 ffc2 00c3  ................
-000024d0: d7c1 c60c 0a21 20cb 00fb ffca 00c1 d888  .....! .........
-000024e0: 5828 c2f5 c2d8 88c1 d8c1 d7cb ffc1 ca11  X(..............
-000024f0: c1cb 1314 c1cc 0cc1 cbc8 ffc2 d7c3 d8c1  ................
-00002500: f50b 0c20 58c1 d8ca 00fb ffcb 0058 6a20  ... X........Xj 
-00002510: 21c1 c8c1 d8c2 d7c2 00d6 ff00 ffff ffff  !...............
-00002520: d0ff c1c7 c2c8 c2ca c2c9 c1ca c8ff c400  ................
-00002530: c2d7 88c1 d7cd 00fb ffcc 00c1 d7c1 c6c1  ................
-00002540: c888 c4d7 00cb ffc2 11c1 cb13 15c1 cc0c  ................
-00002550: 16c8 ff00 c4d7 10c1 c9c1 c8c1 d7cc 00fb  ................
-00002560: ffcd 0058 88c2 d7c4 00d6 ff00 ffff ffff  ...X............
-00002570: d0ff c1c8 c2c9 c2ca c1cb c1ca c1c9 ffff  ................
-00002580: d9ff cf00 c1c6 c500 cbff c1c8 c1c9 c2cb  ................
-00002590: c1cc c1cb c1ca c1c9 c8ff c500 c1c8 cf00  ................
-000025a0: ffff e7ff 00ff ffff ffd0 ffc1 c9c1 cac1  ................
-000025b0: cbc2 d7c1 cac1 cbc1 caff fff9 ffc1 c8c1  ................
-000025c0: c9c1 cbc3 ccc1 cac1 cbff ffff ffc5 ff00  ................
-000025d0: ffff ffff d0ff c1ca c1c9 c1d7 c1d8 c2d7  ................
-000025e0: 12c1 caff fff9 ffc1 c828 0ac2 0b0c 0ec1  .........(......
-000025f0: cbff ffff ffc5 ff00 ffff ffff d0ff c2c9  ................
-00002600: c1d7 c1d8 c2d7 10c1 c8ff fff9 ff20 6abf  ............. j.
-00002610: 5821 bf13 0cff ffff ffc5 ff00 ffff ffff  X!..............
-00002620: d0ff c2c7 c1d7 c1d8 c2d7 c1d8 c1c6 ffff  ................
-00002630: f9ff 20c2 886a 2013 6a0b ffff ffff c5ff  .. ..j .j.......
-00002640: 00ff ffff ffd0 ffc8 d7ff fff9 ff6a c1d8  .............j..
-00002650: 8858 c26a 8815 ffff ffff c5ff 00ff ffff  .X.j............
-00002660: ffd0 ffc8 d7ff fff9 ff88 c1d7 c1d8 8858  ...............X
-00002670: 88c1 d86a ffff ffff c5ff 00ff ffff ffff  ...j............
-00002680: ffff ffd2 ffc1 c7c1 d7c2 d888 c1d8 c1d7  ................
-00002690: c1c7 ffff ffff c5ff 00ff ffff ffff ffff  ................
-000026a0: ffd2 ffc2 00c4 d7c2 00ff ffff ffc5 ff00  ................
-000026b0: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-000026c0: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-000026d0: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-000026e0: ffd0 ff00 c2c8 c4c9 00c8 ffcf 00c1 c6c4  ................
-000026f0: 00cc ffc2 c6cb c7c2 c6c5 c7c1 c6c6 c700  ................
-00002700: d4ff c400 c1c9 cf00 ccff 00c2 c8c4 c900  ................
-00002710: c8ff cf00 c1c6 c400 ccff c2c6 cbc7 c2c6  ................
-00002720: c5c7 c1c6 c6c7 00d4 ffc4 00c1 c9cf 00d7  ................
-00002730: ff00 ffff ffff d0ff c1c7 c1c9 c2ca c1cb  ................
-00002740: c2ca c1c9 c8ff cd00 c1c6 c1c9 c2ca c1c9  ................
-00002750: c200 ccff c2ca d6cb c1ca c1cb c1ca c1d8  ................
-00002760: d4ff c200 c4ca c1c9 cd00 ccff c1c7 c1c9  ................
-00002770: c2ca c1cb c2ca c1c9 c8ff cd00 c1c6 c1c9  ................
-00002780: c2ca c1c9 c200 ccff c2ca d6cb c1ca c1cb  ................
-00002790: c1ca c1d8 d4ff c200 c4ca c1c9 cd00 d7ff  ................
-000027a0: 00ff ffff ffd0 ffc1 c7c1 c9c1 cac1 cbc1  ................
-000027b0: ccc1 cbc2 cac8 ffcb 00c1 c6c1 c9c2 cac2  ................
-000027c0: cbc2 ca00 ccff c1ca c1cb c1cc c3cd c3cc  ................
-000027d0: c3cd c3cc c1cd c2cc c1cd c2cc c3cd c2cc  ................
-000027e0: c1cb c1d8 d4ff 00c1 cac4 cbc2 cac1 c9cb  ................
-000027f0: 00cc ffc1 c7c1 c9c1 cac1 cbc1 ccc1 cbc2  ................
-00002800: cac8 ffcb 00c1 c6c1 c9c2 cac2 cbc2 ca00  ................
-00002810: ccff c1ca c1cb c1cc c3cd c3cc c3cd c3cc  ................
-00002820: c1cd c2cc c1cd c2cc c3cd c2cc c1cb c1d8  ................
-00002830: d4ff 00c1 cac4 cbc2 cac1 c9cb 00d7 ff00  ................
-00002840: ffff ffff d0ff c1c6 c1c9 c1ca c1cb c1cc  ................
-00002850: c1cb c1ca c1c9 c8ff c900 c1c7 c1c9 c2ca  ................
-00002860: c2cb c3cc c1cb c1ca ccff c1ca c3cb c1ca  ................
-00002870: d5cb c1ca 88d4 ffc2 c9c2 cac4 cbc2 cac1  ................
-00002880: c9c9 00cc ffc1 c6c1 c9c1 cac1 cbc1 ccc1  ................
-00002890: cbc1 cac1 c9c8 ffc9 00c1 c7c1 c9c2 cac2  ................
-000028a0: cbc3 ccc1 cbc1 cacc ffc1 cac3 cbc1 cad5  ................
-000028b0: cbc1 ca88 d4ff c2c9 c2ca c4cb c2ca c1c9  ................
-000028c0: c900 d7ff 00ff ffff ffd0 ffc1 c6c1 c9c1  ................
-000028d0: cac1 cbc1 ccc1 cbc2 cac8 ffc7 00c1 c7c1  ................
-000028e0: c9c2 cac2 cbc2 ccc1 cdc1 ccc2 cbc1 cacc  ................
-000028f0: ffc2 cdc2 ccc2 cdc1 cbc1 ccc1 cac1 cbc1  ................
-00002900: ccc1 cac1 cbc2 cac1 cbc1 ccc1 cac1 cbc1  ................
-00002910: ccc1 cac1 cbc1 ccc1 cac1 cbc2 cc20 d4ff  ............. ..
-00002920: 11c3 c9c2 cac4 cbc2 cac1 c9c7 00cc ffc1  ................
-00002930: c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8 ffc7  ................
-00002940: 00c1 c7c1 c9c2 cac2 cbc2 ccc1 cdc1 ccc2  ................
-00002950: cbc1 cacc ffc2 cdc2 ccc2 cdc1 cbc1 ccc1  ................
-00002960: cac1 cbc1 ccc1 cac1 cbc2 cac1 cbc1 ccc1  ................
-00002970: cac1 cbc1 ccc1 cac1 cbc1 ccc1 cac1 cbc2  ................
-00002980: cc20 d4ff 11c3 c9c2 cac4 cbc2 cac1 c9c7  . ..............
-00002990: 00d7 ff00 ffff ffff d0ff c1c6 c1c9 c1ca  ................
-000029a0: c1cb c1cc c1cb c1ca c1c9 c8ff c500 c1c6  ................
-000029b0: c1c9 c2ca c2cb c2cc c1cd c2cc c1cb c1ca  ................
-000029c0: c215 ccff 0f14 130e 1412 0d13 110c 1210  ................
-000029d0: 0cc2 100c 1210 0c12 110d 1312 0f13 0f21  ...............!
-000029e0: d4ff 12c1 f510 c3c9 c2ca c4cb c2ca c1c9  ................
-000029f0: c500 ccff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
-00002a00: c1ca c1c9 c8ff c500 c1c6 c1c9 c2ca c2cb  ................
-00002a10: c2cc c1cd c2cc c1cb c1ca c215 ccff 0f14  ................
-00002a20: 130e 1412 0d13 110c 1210 0cc2 100c 1210  ................
-00002a30: 0c12 110d 1312 0f13 0f21 d4ff 12c1 f510  .........!......
-00002a40: c3c9 c2ca c4cb c2ca c1c9 c500 d7ff 00cd  ................
-00002a50: ffc8 d7cc ffc3 d7d0 ffc3 d7c1 ffc1 d7d3  ................
-00002a60: ffc3 d7ff ffc1 c6c1 c9c1 cac1 cbc1 ccc1  ................
-00002a70: cbc2 cac8 ffc3 00c1 c6c1 c9c2 cac2 cbc2  ................
-00002a80: ccc1 cdc2 ccc1 cbc1 ca13 1517 15cc ff0f  ................
-00002a90: 1614 0d15 130c 1413 0c14 130c 1312 0c14  ................
-00002aa0: 130c 1413 0c15 140e 140e 20d4 ffc2 2811  .......... ...(.
-00002ab0: 2810 c3c9 c2ca c4cb c2ca c1c9 c300 ccff  (...............
-00002ac0: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
-00002ad0: c300 c1c6 c1c9 c2ca c2cb c2cc c1cd c2cc  ................
-00002ae0: c1cb c1ca 1315 1715 ccff 0f16 140d 1513  ................
-00002af0: 0c14 130c 1413 0c13 120c 1413 0c14 130c  ................
-00002b00: 1514 0e14 0e20 d4ff c228 1128 10c3 c9c2  ..... ...(.(....
-00002b10: cac4 cbc2 cac1 c9c3 00d7 ff00 cdff c1d7  ................
-00002b20: c2ff c2d7 c2ff c1d7 cdff c2d7 cfff c2d7  ................
-00002b30: c2ff c2d7 d4ff c2d7 ffff c1c6 c1c9 c1ca  ................
-00002b40: c1cb c1cc c1cb c1ca c1c9 c8ff 00c1 c6c1  ................
-00002b50: c9c2 cac2 cbc2 ccc1 cdc2 ccc1 cbc1 ca13  ................
-00002b60: 0d16 0d0c 28cc ffc4 0bc9 0a28 21c9 0ac3  ....(......(!...
-00002b70: 0b88 d4ff 58c2 2128 1128 11c1 c8c2 c9c3  ....X.!(.(......
-00002b80: cac3 cbc1 cac2 c900 ccff c1c6 c1c9 c1ca  ................
-00002b90: c1cb c1cc c1cb c1ca c1c9 c8ff 00c1 c6c1  ................
-00002ba0: c9c2 cac2 cbc2 ccc1 cdc2 ccc1 cbc1 ca13  ................
-00002bb0: 0d16 0d0c 28cc ffc4 0bc9 0a28 21c9 0ac3  ....(......(!...
-00002bc0: 0b88 d4ff 58c2 2128 1128 11c1 c8c2 c9c3  ....X.!(.(......
-00002bd0: cac3 cbc1 cac2 c900 d7ff 00d0 ffc2 d7d0  ................
-00002be0: ffc2 d7ce ffc2 d7c4 ffc1 d7d4 ffc2 d7ff  ................
-00002bf0: ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8  ................
-00002c00: ffc2 c7c1 c8c2 cac1 cbc1 ccc1 cdc2 ccc1  ................
-00002c10: cbc1 cac2 1516 0d0b 0a21 c1d7 ccff 2821  .........!....(!
-00002c20: cbf5 2120 caf5 2128 88d4 ffc1 d758 c220  ..! ..!(.....X. 
-00002c30: 2128 2111 10c4 c9c2 cac2 c9c3 cacc ffc1  !(!.............
-00002c40: c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8 ffc2  ................
-00002c50: c7c1 c8c2 cac1 cbc1 ccc1 cdc2 ccc1 cbc1  ................
-00002c60: cac2 1516 0d0b 0a21 c1d7 ccff 2821 cbf5  .......!....(!..
-00002c70: 2120 caf5 2128 88d4 ffc1 d758 c220 2128  ! ..!(.....X. !(
-00002c80: 2111 10c4 c9c2 cac2 c9c3 cad7 ff00 d0ff  !...............
-00002c90: c2d7 c3ff c3d7 c1ff c2d7 c1ff c3d7 c1ff  ................
-00002ca0: c6d7 c3ff c3d7 c6ff c2d7 c7ff c3d7 c3ff  ................
-00002cb0: c3d7 c3ff c4d7 c2ff c2d7 c1ff c2d7 fcff  ................
-00002cc0: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
-00002cd0: c8ff c210 c1d8 c2c8 c2cb c1cc c1cb c1ca  ................
-00002ce0: 0d14 160a 0b0a 216a c200 ccff c1d8 c1d7  ......!j........
-00002cf0: c258 d420 58c1 d7c1 d86a d4ff c200 586a  .X. X....j....Xj
-00002d00: c320 6a11 2810 c1c9 c1c8 c2c9 c1ca c2d8  . j.(...........
-00002d10: c2ca ccff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
-00002d20: c1ca c1c9 c8ff c210 c1d8 c2c8 c2cb c1cc  ................
-00002d30: c1cb c1ca 0d14 160a 0b0a 216a c200 ccff  ..........!j....
-00002d40: c1d8 c1d7 c258 d420 58c1 d7c1 d86a d4ff  .....X. X....j..
-00002d50: c200 586a c320 6a11 2810 c1c9 c1c8 c2c9  ..Xj. j.(.......
-00002d60: c1ca c2d8 c2ca d7ff 00d0 ffc2 d7c4 ffc2  ................
-00002d70: d7c1 ffc2 d7c2 ffc3 d7c1 ffc3 d7c1 ffc2  ................
-00002d80: d7c1 ffc2 d7c1 ffc2 d7c5 ffc2 d7c6 ffc2  ................
-00002d90: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-00002da0: d7c1 ffc2 d7c2 ffc5 d7fc ffc1 c6c1 c9c1  ................
-00002db0: cac1 cbc1 ccc1 cbc2 cac8 ff10 c2d7 c1d8  ................
-00002dc0: c2c9 c1cb c1ca 1316 c20d 0ac1 f521 6ac4  .............!j.
-00002dd0: 00fc ffc4 0058 c36a 2128 1128 13c2 c9c1  .....X.j!(.(....
-00002de0: ca10 c2d8 c1c8 ccff c1c6 c1c9 c1ca c1cb  ................
-00002df0: c1cc c1cb c2ca c8ff 10c2 d7c1 d8c2 c9c1  ................
-00002e00: cbc1 ca13 16c2 0d0a c1f5 216a c400 fcff  ..........!j....
-00002e10: c400 58c3 6a21 2811 2813 c2c9 c1ca 10c2  ..X.j!(.(.......
-00002e20: d8c1 c8d7 ff00 d0ff c2d7 c4ff c2d7 c1ff  ................
-00002e30: c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7 c1ff  ................
-00002e40: c2d7 c1ff c2d7 c5ff c2d7 c6ff c2d7 c1ff  ................
-00002e50: c2d7 c4ff c2d7 c1ff c2d7 c5ff c2d7 c1ff  ................
-00002e60: c2d7 fcff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
-00002e70: c1ca c1c9 c8ff c1d8 c3d7 10c1 c715 0f16  ................
-00002e80: 0d0b 0a20 6ac6 00fc ffc6 00c2 58c2 2021  ... j.......X. !
-00002e90: c328 c1ca c1c9 c2d8 c1d7 c1d8 ccff c1c6  .(..............
-00002ea0: c1c9 c1ca c1cb c1cc c1cb c1ca c1c9 c8ff  ................
-00002eb0: c1d8 c3d7 10c1 c715 0f16 0d0b 0a20 6ac6  ............. j.
-00002ec0: 00fc ffc6 00c2 58c2 2021 c328 c1ca c1c9  ......X. !.(....
-00002ed0: c2d8 c1d7 c1d8 d7ff 00d0 ffc2 d7c4 ffc2  ................
-00002ee0: d7c1 ffc2 d7c2 ffc2 d7c3 ffc2 d7c1 ffc2  ................
-00002ef0: d7c1 ffc2 d7c1 ffc2 d7c5 ffc2 d7c6 ffc2  ................
-00002f00: d7c1 ffc2 d7c2 ffc4 d7c1 ffc2 d7c5 ffc2  ................
-00002f10: d7c1 ffc2 d7fc ffc1 c6c1 c9c1 cac1 cbc1  ................
-00002f20: ccc1 cbc2 cac8 ffc4 d7c1 d810 170d 0b0a  ................
-00002f30: 216a c800 fcff c800 586a c220 2814 c1ca  !j......Xj. (...
-00002f40: 10c1 d8c3 d7cc ffc1 c6c1 c9c1 cac1 cbc1  ................
-00002f50: ccc1 cbc2 cac8 ffc4 d7c1 d810 170d 0b0a  ................
-00002f60: 216a c800 fcff c800 586a c220 2814 c1ca  !j......Xj. (...
-00002f70: 10c1 d8c3 d7d7 ff00 d0ff c2d7 c4ff c2d7  ................
-00002f80: c1ff c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7  ................
-00002f90: c1ff c2d7 c1ff c2d7 c6ff c2d7 c3ff c1d7  ................
-00002fa0: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
-00002fb0: c1ff c2d7 c2ff c1d7 c2ff c2d7 c1ff c2d7  ................
-00002fc0: fcff c1c7 c2c8 c2ca c2c9 c1ca c8ff c200  ................
-00002fd0: c3d7 c1c6 0c0a 2120 ca00 fcff ca00 586a  ......! ......Xj
-00002fe0: 2021 10c1 c6c3 d700 ccff c1c7 c2c8 c2ca   !..............
-00002ff0: c2c9 c1ca c8ff c200 c3d7 c1c6 0c0a 2120  ..............! 
-00003000: ca00 fcff ca00 586a 2021 10c1 c6c3 d700  ......Xj !......
-00003010: d7ff 00cf ffc4 d7c4 ffc9 d7c2 ffc1 d7c1  ................
-00003020: ffc2 d7c3 ffc3 d7c8 ffc4 d7c3 ffc3 d7c3  ................
-00003030: ffc5 d7c1 ffc3 d7c2 ffc3 d7c1 ffc3 d7fb  ................
-00003040: ffc1 c8c2 c9c2 cac1 cbc1 cac1 c9c8 ffc4  ................
-00003050: 00c2 d788 c1d7 cc00 fcff cc00 c1d7 c2d8  ................
-00003060: c2d7 c300 ccff c1c8 c2c9 c2ca c1cb c1ca  ................
-00003070: c1c9 c8ff c400 c2d7 88c1 d7cc 00fc ffcc  ................
-00003080: 00c1 d7c2 d8c2 d7c3 00d7 ff00 ffff ffff  ................
-00003090: d0ff c1c9 c1ca c1cb c2d7 c1ca c1cb c1ca  ................
-000030a0: ffff d9ff ce00 c1d7 c500 ccff c1c9 c1ca  ................
-000030b0: c1cb c2d7 c1ca c1cb c1ca ffff d9ff ce00  ................
-000030c0: c1d7 c500 d7ff 00ff ffff ffd0 ffc1 cac1  ................
-000030d0: c9c1 d7c1 d8c2 d712 c1ca ffff f9ff c1ca  ................
-000030e0: c1c9 c1d7 c1d8 c2d7 12c1 caff ffff ffc5  ................
-000030f0: ff00 ffff ffff d0ff c2c9 c1d7 c1d8 c2d7  ................
-00003100: 10c1 c8ff fff9 ffc2 c9c1 d7c1 d8c2 d710  ................
-00003110: c1c8 ffff ffff c5ff 00ff ffff ffd0 ffc2  ................
-00003120: c7c1 d7c1 d8c2 d7c1 d8c1 c6ff fff9 ffc2  ................
-00003130: c7c1 d7c1 d8c2 d7c1 d8c1 c6ff ffff ffc5  ................
-00003140: ff00 ffff ffff d0ff c8d7 ffff f9ff c8d7  ................
-00003150: ffff ffff c5ff 00ff ffff ffd0 ffc8 d7ff  ................
-00003160: fff9 ffc8 d7ff ffff ffc5 ff00 ffff ffff  ................
-00003170: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00003180: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00003190: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-000031a0: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-000031b0: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-000031c0: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-000031d0: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-000031e0: ffdf ff00 ffff ffff d0ff 00c2 c8c4 c900  ................
-000031f0: c8ff cf00 c1c6 c400 ccff c2c6 cbc7 c2c6  ................
-00003200: c5c7 c1c6 c6c7 00d4 ffc4 00c1 c9cf 00cc  ................
-00003210: ff00 c2c8 c4c9 00c8 ffcf 00c1 c6c4 00cc  ................
-00003220: ffc2 c6cb c7c2 c6c5 c7c1 c6c6 c700 d4ff  ................
-00003230: c400 c1c9 cf00 d7ff 00ff ffff ffd0 ffc1  ................
-00003240: c7c1 c9c2 cac1 cbc2 cac1 c9c8 ffcd 00c1  ................
-00003250: c6c1 c9c2 cac1 c9c2 00cc ffc2 cad6 cbc1  ................
-00003260: cac1 cbc1 cac1 d8d4 ffc2 00c4 cac1 c9cd  ................
-00003270: 00cc ffc1 c7c1 c9c2 cac1 cbc2 cac1 c9c8  ................
-00003280: ffcd 00c1 c6c1 c9c2 cac1 c9c2 00cc ffc2  ................
-00003290: cad6 cbc1 cac1 cbc1 cac1 d8d4 ffc2 00c4  ................
-000032a0: cac1 c9cd 00d7 ff00 ffff ffff d0ff c1c7  ................
-000032b0: c1c9 c1ca c1cb c1cc c1cb c2ca c8ff cb00  ................
-000032c0: c1c6 c1c9 c2ca c2cb c2ca 00cc ffc1 cac1  ................
-000032d0: cbc1 ccc3 cdc3 ccc3 cdc3 ccc1 cdc2 ccc1  ................
-000032e0: cdc2 ccc3 cdc2 ccc1 cbc1 d8d4 ff00 c1ca  ................
-000032f0: c4cb c2ca c1c9 cb00 ccff c1c7 c1c9 c1ca  ................
-00003300: c1cb c1cc c1cb c2ca c8ff cb00 c1c6 c1c9  ................
-00003310: c2ca c2cb c2ca 00cc ffc1 cac1 cbc1 ccc3  ................
-00003320: cdc3 ccc3 cdc3 ccc1 cdc2 ccc1 cdc2 ccc3  ................
-00003330: cdc2 ccc1 cbc1 d8d4 ff00 c1ca c4cb c2ca  ................
-00003340: c1c9 cb00 d7ff 00ff ffff ffd0 ffc1 c6c1  ................
-00003350: c9c1 cac1 cbc1 ccc1 cbc1 cac1 c9c8 ffc9  ................
-00003360: 00c1 c7c1 c9c2 cac2 cbc3 ccc1 cbc1 cacc  ................
-00003370: ffc1 cac3 cbc1 cad5 cbc1 ca88 d4ff c2c9  ................
-00003380: c2ca c4cb c2ca c1c9 c900 ccff c1c6 c1c9  ................
-00003390: c1ca c1cb c1cc c1cb c1ca c1c9 c8ff c900  ................
-000033a0: c1c7 c1c9 c2ca c2cb c3cc c1cb c1ca ccff  ................
-000033b0: c1ca c3cb c1ca d5cb c1ca 88d4 ffc2 c9c2  ................
-000033c0: cac4 cbc2 cac1 c9c9 00d7 ff00 ffff ffff  ................
-000033d0: d0ff c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca  ................
-000033e0: c8ff c700 c1c7 c1c9 c2ca c2cb c2cc c1cd  ................
-000033f0: c1cc c2cb c1ca ccff c5cc c1cb c1cc c3cb  ................
-00003400: c1cc c5ca c1cc c8cb c2cc 20d4 ff13 c3c9  .......... .....
-00003410: c2ca c4cb c2ca c1c9 c700 ccff c1c6 c1c9  ................
-00003420: c1ca c1cb c1cc c1cb c2ca c8ff c700 c1c7  ................
-00003430: c1c9 c2ca c2cb c2cc c1cd c1cc c2cb c1ca  ................
-00003440: ccff c5cc c1cb c1cc c3cb c1cc c5ca c1cc  ................
-00003450: c8cb c2cc 20d4 ff13 c3c9 c2ca c4cb c2ca  .... ...........
-00003460: c1c9 c700 d7ff 00ff ffff ffd0 ffc1 c6c1  ................
-00003470: c9c1 cac1 cbc1 ccc1 cbc1 cac1 c9c8 ffc5  ................
-00003480: 00c1 c6c1 c9c2 cac2 cbc2 ccc1 cdc2 ccc1  ................
-00003490: cbc1 ca0f 15cc ffc3 0fc2 0ec2 0d17 c20c  ................
-000034a0: 0ac5 0c0b c30c c20d c20e c30f 21d4 ffc2  ............!...
-000034b0: f513 c3c9 c2ca c4cb c2ca c1c9 c500 ccff  ................
-000034c0: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
-000034d0: c8ff c500 c1c6 c1c9 c2ca c2cb c2cc c1cd  ................
-000034e0: c2cc c1cb c1ca 0f15 ccff c30f c20e c20d  ................
-000034f0: 17c2 0c0a c50c 0bc3 0cc2 0dc2 0ec3 0f21  ...............!
-00003500: d4ff c2f5 13c3 c9c2 cac4 cbc2 cac1 c9c5  ................
-00003510: 00d7 ff00 ffff ffff d0ff c1c6 c1c9 c1ca  ................
-00003520: c1cb c1cc c1cb c2ca c8ff c300 c1c6 c1c9  ................
-00003530: c2ca c2cb c2cc c1cd c2cc c1cb c1ca c30f  ................
-00003540: 15cc ff0f c20e c20d 17c4 0cc1 f5c5 0cc1  ................
-00003550: f5c5 0cc2 0dc3 0e20 d4ff c228 c1f5 2813  ....... ...(..(.
-00003560: c3c9 c2ca c4cb c2ca c1c9 c300 ccff c1c6  ................
-00003570: c1c9 c1ca c1cb c1cc c1cb c2ca c8ff c300  ................
-00003580: c1c6 c1c9 c2ca c2cb c2cc c1cd c2cc c1cb  ................
-00003590: c1ca c30f 15cc ff0f c20e c20d 17c4 0cc1  ................
-000035a0: f5c5 0cc1 f5c5 0cc2 0dc3 0e20 d4ff c228  ........... ...(
-000035b0: c1f5 2813 c3c9 c2ca c4cb c2ca c1c9 c300  ..(.............
-000035c0: d7ff 00cd ffc8 d7cc ffc3 d7cd ffc4 d7c3  ................
-000035d0: ffc4 d7c7 ffc2 d7c1 ffc3 d7c7 ffc3 d7c1  ................
-000035e0: ffc1 d7f9 ffc1 c6c1 c9c1 cac1 cbc1 ccc1  ................
-000035f0: cbc1 cac1 c9c8 ff00 c1c6 c1c9 c2ca c2cb  ................
-00003600: c2cc c1cd c2cc c1cb c1ca 0d0f 0ec2 0d28  ...............(
-00003610: ccff c40b c20a 0b0a c20b 21c5 0a21 c40a  ..........!..!..
-00003620: 0b0a c40b 88d4 ff58 c221 c328 12c1 c8c2  .......X.!.(....
-00003630: c9c3 cac3 cbc1 cac2 c900 ccff c1c6 c1c9  ................
-00003640: c1ca c1cb c1cc c1cb c1ca c1c9 c8ff 00c1  ................
-00003650: c6c1 c9c2 cac2 cbc2 ccc1 cdc2 ccc1 cbc1  ................
-00003660: ca0d 0f0e c20d 28cc ffc4 0bc2 0a0b 0ac2  ......(.........
-00003670: 0b21 c50a 21c4 0a0b 0ac4 0b88 d4ff 58c2  .!..!.........X.
-00003680: 21c3 2812 c1c8 c2c9 c3ca c3cb c1ca c2c9  !.(.............
-00003690: 00d7 ff00 cdff c1d7 c2ff c2d7 c2ff c1d7  ................
-000036a0: cdff c2d7 ceff c3d7 c3ff c3d7 c8ff c2d7  ................
-000036b0: c2ff c2d7 c6ff c2d7 c2ff c2d7 f9ff c1c6  ................
-000036c0: c1c9 c1ca c1cb c1cc c1cb c2ca c8ff c2c7  ................
-000036d0: c1c8 c2ca c1cb c1cc c1cd c2cc c1cb c1ca  ................
-000036e0: 0e0f 0b0d 0c0a 21c1 d7cc ff28 21c4 f515  ......!....(!...
-000036f0: c1f5 c215 20c5 2820 c4f5 15c1 f5c2 1521  .... .( .......!
-00003700: 2888 d4ff c1d7 5820 c321 c228 12c4 c9c2  (.....X .!.(....
-00003710: cac2 c9c3 cacc ffc1 c6c1 c9c1 cac1 cbc1  ................
-00003720: ccc1 cbc2 cac8 ffc2 c7c1 c8c2 cac1 cbc1  ................
-00003730: ccc1 cdc2 ccc1 cbc1 ca0e 0f0b 0d0c 0a21  ...............!
-00003740: c1d7 ccff 2821 c4f5 15c1 f5c2 1520 c528  ....(!....... .(
-00003750: 20c4 f515 c1f5 c215 2128 88d4 ffc1 d758   .......!(.....X
-00003760: 20c3 21c2 2812 c4c9 c2ca c2c9 c3ca d7ff   .!.(...........
-00003770: 00d0 ffc2 d7d0 ffc2 d7ce ffc3 d7c3 ffc3  ................
-00003780: d7cc ffc2 d7c5 ffc2 d7c4 ffc1 d7f9 ffc1  ................
-00003790: c6c1 c9c1 cac1 cbc1 ccc1 cbc1 cac1 c9c8  ................
-000037a0: ffc2 10c1 d8c2 c8c2 cbc1 ccc1 cbc1 cac3  ................
-000037b0: 0e0c c1f5 0a21 6ac2 00cc ffc1 d8c1 d7c2  .....!j.........
-000037c0: 58d4 2058 c1d7 c1d8 6ad4 ffc2 00c1 d758  X. X....j......X
-000037d0: 206a 2128 2128 13c1 c9c1 c8c2 c9c1 cac2   j!(!(..........
-000037e0: d8c2 cacc ffc1 c6c1 c9c1 cac1 cbc1 ccc1  ................
-000037f0: cbc1 cac1 c9c8 ffc2 10c1 d8c2 c8c2 cbc1  ................
-00003800: ccc1 cbc1 cac3 0e0c c1f5 0a21 6ac2 00cc  ...........!j...
-00003810: ffc1 d8c1 d7c2 58d4 2058 c1d7 c1d8 6ad4  ......X. X....j.
-00003820: ffc2 00c1 d758 206a 2128 2128 13c1 c9c1  .....X j!(!(....
-00003830: c8c2 c9c1 cac2 d8c2 cad7 ff00 d0ff c2d7  ................
-00003840: c3ff c3d7 c1ff c2d7 c1ff c3d7 c1ff c6d7  ................
-00003850: c3ff c3d7 c6ff c1d7 c1ff c2d7 c1ff c1d7  ................
-00003860: c1ff c2d7 c2ff c3d7 c2ff c3d7 c2ff c2d7  ................
-00003870: c5ff c2d7 c7ff c3d7 c2ff c3d7 c1ff c2d7  ................
-00003880: ecff c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca  ................
-00003890: c8ff 10c2 d7c1 d8c2 c9c1 cbc1 cac2 0f0e  ................
-000038a0: 0b0a c1f5 206a c400 fcff c400 c1d7 886a  .... j.........j
-000038b0: c220 28c2 f513 c2c9 c1ca 10c2 d8c1 c8cc  . (.............
-000038c0: ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8  ................
-000038d0: ff10 c2d7 c1d8 c2c9 c1cb c1ca c20f 0e0b  ................
-000038e0: 0ac1 f520 6ac4 00fc ffc4 00c1 d788 6ac2  ... j.........j.
-000038f0: 2028 c2f5 13c2 c9c1 ca10 c2d8 c1c8 d7ff   (..............
-00003900: 00d0 ffc2 d7c4 ffc2 d7c1 ffc2 d7c2 ffc3  ................
-00003910: d7c1 ffc3 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
-00003920: d7c5 ffc1 d7c1 ffc2 d7c1 ffc1 d7c1 ffc2  ................
-00003930: d7c1 ffc2 d7c1 ffc2 d7c2 ffc2 d7c2 ffc2  ................
-00003940: d7c5 ffc2 d7c6 ffc2 d7c1 ffc2 d7c2 ffc3  ................
-00003950: d7c1 ffc1 d7ec ffc1 c6c1 c9c1 cac1 cbc1  ................
-00003960: ccc1 cbc1 cac1 c9c8 ffc1 d8c3 d710 c1c7  ................
-00003970: c20f 0e0d 1728 206a c600 fcff c600 c1d7  .....( j........
-00003980: 886a c221 28c2 f5c1 cac1 c9c2 d8c1 d7c1  .j.!(...........
-00003990: d8cc ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc1  ................
-000039a0: cac1 c9c8 ffc1 d8c3 d710 c1c7 c20f 0e0d  ................
-000039b0: 1728 206a c600 fcff c600 c1d7 886a c221  .( j.........j.!
-000039c0: 28c2 f5c1 cac1 c9c2 d8c1 d7c1 d8d7 ff00  (...............
-000039d0: d0ff c2d7 c4ff c2d7 c1ff c2d7 c2ff c2d7  ................
-000039e0: c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
-000039f0: c5ff c1d7 c1ff c2d7 c1ff c1d7 c1ff c2d7  ................
-00003a00: c4ff c2d7 c2ff c2d7 c2ff c2d7 c5ff c2d7  ................
-00003a10: c9ff c2d7 c2ff c2d7 efff c1c6 c1c9 c1ca  ................
-00003a20: c1cb c1cc c1cb c2ca c8ff c4d7 c1d8 100f  ................
-00003a30: 0d0c 0a21 6ac8 00fc ffc8 00c1 d758 2021  ...!j........X !
-00003a40: 28c1 f5c1 ca10 c1d8 c3d7 ccff c1c6 c1c9  (...............
-00003a50: c1ca c1cb c1cc c1cb c2ca c8ff c4d7 c1d8  ................
-00003a60: 100f 0d0c 0a21 6ac8 00fc ffc8 00c1 d758  .....!j........X
-00003a70: 2021 28c1 f5c1 ca10 c1d8 c3d7 d7ff 00d0   !(.............
-00003a80: ffc2 d7c4 ffc2 d7c1 ffc2 d7c2 ffc2 d7c3  ................
-00003a90: ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c5  ................
-00003aa0: ffc1 d7c2 ffc2 d7c2 ffc2 d7c2 ffc4 d7c2  ................
-00003ab0: ffc2 d7c2 ffc2 d7c5 ffc2 d7c7 ffc4 d7c2  ................
-00003ac0: ffc2 d7ef ffc1 c7c2 c8c2 cac2 c9c1 cac8  ................
-00003ad0: ffc2 00c3 d7c1 c60c 0a21 20ca 00fc ffca  .........! .....
-00003ae0: 00c1 d758 2021 10c1 c6c3 d700 ccff c1c7  ...X !..........
-00003af0: c2c8 c2ca c2c9 c1ca c8ff c200 c3d7 c1c6  ................
-00003b00: 0c0a 2120 ca00 fcff ca00 c1d7 5820 2110  ..! ........X !.
-00003b10: c1c6 c3d7 00d7 ff00 d0ff c2d7 c4ff c2d7  ................
-00003b20: c1ff c2d7 c2ff c2d7 c3ff c2d7 c1ff c2d7  ................
-00003b30: c1ff c2d7 c1ff c2d7 c5ff c1d7 c2ff c2d7  ................
-00003b40: c2ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c2d7  ................
-00003b50: c2ff c2d7 c6ff c2d7 c3ff c1d7 c1ff c2d7  ................
-00003b60: c1ff c2d7 c2ff c2d7 efff c1c8 c2c9 c2ca  ................
-00003b70: c1cb c1ca c1c9 c8ff c400 c2d7 88c1 d7cc  ................
-00003b80: 00fc ffcc 00c1 d7c2 d8c2 d7c3 00cc ffc1  ................
-00003b90: c8c2 c9c2 cac1 cbc1 cac1 c9c8 ffc4 00c2  ................
-00003ba0: d788 c1d7 cc00 fcff cc00 c1d7 c2d8 c2d7  ................
-00003bb0: c300 d7ff 00cf ffc4 d7c4 ffc9 d7c2 ffc1  ................
-00003bc0: d7c1 ffc2 d7c3 ffc3 d7c5 ffc3 d7c1 ffc2  ................
-00003bd0: d7c1 ffc4 d7c1 ffcd d7c6 ffc4 d7c3 ffc9  ................
-00003be0: d7ee ffc1 c9c1 cac1 cbc2 d7c1 cac1 cbc1  ................
-00003bf0: caff ffd9 ffce 00c1 d7c5 00cc ffc1 c9c1  ................
-00003c00: cac1 cbc2 d7c1 cac1 cbc1 caff ffd9 ffce  ................
-00003c10: 00c1 d7c5 00d7 ff00 ffff ffff d0ff c1ca  ................
-00003c20: c1c9 c1d7 c1d8 c2d7 12c1 caff fff9 ffc1  ................
-00003c30: cac1 c9c1 d7c1 d8c2 d712 c1ca ffff ffff  ................
-00003c40: c5ff 00ff ffff ffd0 ffc2 c9c1 d7c1 d8c2  ................
-00003c50: d710 c1c8 ffff f9ff c2c9 c1d7 c1d8 c2d7  ................
-00003c60: 10c1 c8ff ffff ffc5 ff00 ffff ffff d0ff  ................
-00003c70: c2c7 c1d7 c1d8 c2d7 c1d8 c1c6 ffff f9ff  ................
-00003c80: c2c7 c1d7 c1d8 c2d7 c1d8 c1c6 ffff ffff  ................
-00003c90: c5ff 00ff ffff ffd0 ffc8 d7ff fff9 ffc8  ................
-00003ca0: d7ff ffff ffc5 ff00 ffff ffff d0ff c8d7  ................
-00003cb0: ffff f9ff c8d7 ffff ffff c5ff 00ff ffff  ................
-00003cc0: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-00003cd0: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00003ce0: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00003cf0: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-00003d00: ffff ffff ffdf ff00 ffff ffff ffff ffff  ................
-00003d10: ffff ffff dfff 00ff ffff ffff ffff ffff  ................
-00003d20: ffff ffdf ff00 ffff ffff ffff ffff ffff  ................
-00003d30: ffff dfff 00ff ffff ffff ffff ffff ffff  ................
-00003d40: ffdf ff00 ffff ffff ffff ffff ffff ffff  ................
-00003d50: dfff 00ff ffff ffff ffff ffff ffff ffdf  ................
-00003d60: ff00 ffff ffff ffff ffff ffff ffff dfff  ................
-00003d70: 00ff ffff ffff ffff ffff ffff ffdf ff00  ................
-00003d80: ffff ffff ffff ffff ffff ffff dfff 00ff  ................
-00003d90: ffff ffff ffff ffff ffff ffdf ff00 ffff  ................
-00003da0: ffff ffff ffff ffff ffff dfff 00ff ffff  ................
-00003db0: ffff ffff ffff ffff ffdf ff00 ffff ffff  ................
-00003dc0: ffff ffff ffff ffff dfff 00ff ffff ffff  ................
-00003dd0: ffff ffff ffff ffdf ff00 ffff ffff ffff  ................
-00003de0: ffff ffff ffff dfff 00ff ffff ffff ffff  ................
-00003df0: ffff ffff ffdf ff00 0c00 00ff ee00 eeef  ................
-00003e00: 00ef f000 f0f1 00f1 f200 f2f3 00f3 f400  ................
-00003e10: f4f5 00f5 f600 f6a8 a8a8 b8b8 b8c8 c8c8  ................
-00003e20: d8d8 d8e8 e8e8 fcfc fc34 3c48 444c 5c58  .........4<HDL\X
-00003e30: 6070 6c74 8484 8c98 9ca0 acb0 b8c4 ccd0  `plt............
-00003e40: dc30 2c04 403c 0c50 4c14 605c 1c78 7840  .0,.@<.PL.`\.xx@
-00003e50: 9494 64b0 b084 cccc a864 6464 7474 7468  ..d......dddttth
-00003e60: 502c 7c68 4898 845c b8a0 78d4 bc94 f4dc  P,|hH..\..x.....
-00003e70: b084 8484 5804 1070 1020 8820 34a0 384c  ....X..p. . 4.8L
-00003e80: bc54 6ccc 687c dc84 90ec 9ca4 fcbc c0fc  .Tl.h|..........
-00003e90: d000 fce8 3cfc fc80 4c28 0060 3c08 7458  ....<...L(.`<.tX
-00003ea0: 1c88 7438 9c88 50b0 9c6c c4b4 8844 1800  ..t8..P..l...D..
-00003eb0: 602c 0480 4408 9c60 10b8 7818 d49c 20e8  `,..D..`..x... .
-00003ec0: b810 fcd4 00fc f880 fcfc c020 0400 4014  ........... ..@.
-00003ed0: 0854 1c10 6c2c 1c80 3828 9448 38a8 5c4c  .T..l,..8(.H8.\L
-00003ee0: b86c 58c4 806c d494 8008 3400 1040 0020  .lX..l....4..@. 
-00003ef0: 5004 3060 0440 700c 5484 1468 941c 80a8  P.0`.@p.T..h....
-00003f00: 2c40 4040 2c44 203c 5830 5068 3c68 7c4c  ,@@@,D <X0Ph<h|L
-00003f10: 8094 5c98 b06c b4cc 7c10 3418 2048 2c38  ..\..l..|.4. H,8
-00003f20: 6048 4c74 5860 886c 78a4 8898 c0a8 b8dc  `HLtX`.lx.......
-00003f30: c820 1800 381c 0050 5050 5834 0c68 4018  . ..8..PPPX4.h@.
-00003f40: 7c54 2c8c 6c40 a080 584c 2810 6034 1874  |T,.l@..XL(.`4.t
-00003f50: 4428 8854 38a4 6040 b870 50cc 8060 d494  D(.T8.`@.pP..`..
-00003f60: 70e0 a880 ecbc 9450 1c04 6428 1478 3828  p......P..d(.x8(
-00003f70: 8c4c 40a0 6460 b888 8824 2844 3034 5440  .L@.d`...$(D04T@
-00003f80: 4064 5050 7464 6488 8484 a4ac acc0 d4d4  @dPPtdd.........
-00003f90: e030 3030 402c 9058 40ac 684c c478 58e0  .000@,.X@.hL.xX.
-00003fa0: 8c68 fca0 88fc bca8 fc00 186c 0024 8400  .h.........l.$..
-00003fb0: 34a0 0048 b800 60d4 1878 dc38 90e8 58a8  4..H..`..x.8..X.
-00003fc0: f080 c4fc bce0 fc10 4060 1850 6c28 6078  ........@`.Pl(`x
-00003fd0: 3470 8450 8ca0 74ac c09c ccdc ccf0 fcac  4p.P..t.........
-00003fe0: 3434 d434 34fc 3434 fc64 58fc 907c fcb8  44.44.44.dX..|..
-00003ff0: a0fc d8c8 fcf4 ec48 1470 5c2c 8c70 44a8  .......H.p\,.pD.
-00004000: 8c64 c4a8 88e0 c8b0 f8d0 b8ff e8d0 fc3c  .d.............<
-00004010: 0000 5c00 0080 0000 a000 00c4 0000 e000  ..\.............
-00004020: 00fc 0000 fc50 00fc 6c00 fc88 00fc a400  .....P..l.......
-00004030: fcc0 00fc dc00 fcfc 00cc 8808 e490 04fc  ................
-00004040: 9c00 fcb0 30fc c464 fcd8 9808 1858 0c24  ....0..d.....X.$
-00004050: 6814 347c 1c44 8c28 5ca4 3878 bc48 98d8  h.4|.D.(\.8x.H..
-00004060: 64ac e05c 9c34 6cb0 407c c84c 90e0 5ce0  d..\.4l.@|.L..\.
-00004070: f4fc c8ec f8b4 dcec 84bc d858 98ac 1010  ...........X....
-00004080: 1020 2020 2044 7024 4874 284c 782c 507c  .    Dp$Ht(Lx,P|
-00004090: 3054 8048 6490 6484 a8d8 f4fc 6080 a444  0T.Hd.d.....`..D
-000040a0: 608c 4c18 086c 2c18 9048 34b0 6c54 d292  `.L..l,..H4.lT..
-000040b0: 7efc 3c00 fc54 00fc 6800 fc7c 00fc 9400  ~.<..T..h..|....
-000040c0: fcac 00fc c400 4000 00ff 0000 3030 0040  ......@.....00.@
-000040d0: 4000 5050 00ff ff00 9494 94f7 00f7 f800  @.PP............
-000040e0: f8f9 00f9 fa00 fafb 00fb fc00 fcfd 00fd  ................
-000040f0: fe00 feff 00ff ffff ff                   .........
+00000ad0: d2ff dbff c1d7 d5ff c2d7 ffff dfff c1d7  ................
+00000ae0: c1d8 c1d7 4669 c1d7 c1d8 c1d7 ffff e9ff  ....Fi..........
+00000af0: c2d7 c1d8 88c2 d8c2 d7ff ffff ffd2 ffda  ................
+00000b00: ffc2 d7d2 ffc1 d7c2 ffc2 d7ff ffdf ffc2  ................
+00000b10: d7c1 d8c2 d7c1 d8c2 d7ff ffe9 ffc8 d8ff  ................
+00000b20: ffff ffd2 ffda ffc3 d7d1 ffc1 d7ff ffff  ................
+00000b30: ffff ffff ffff ffef ffd9 ffc1 d7c1 ffc2  ................
+00000b40: d7c3 ffc3 d7c1 ffc2 d7c1 ffc4 d7c1 ffc7  ................
+00000b50: d7c2 ffc4 d7ff ffff ffff ffff ffff ffe5  ................
+00000b60: ffd9 ffc1 d7c2 ffc2 d7c3 ffc3 d7c1 ffc3  ................
+00000b70: d7c1 ffc2 d7c2 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00000b80: d7c1 ffc2 d7ff ffff ffff ffff ffff ffe5  ................
+00000b90: ffd9 ffc5 d7c3 ffc2 d7c3 ffc2 d7c5 ffc2  ................
+00000ba0: d7c2 ffc2 d7c1 ffc2 d7ff ffff ffff ffff  ................
+00000bb0: ffff ffe8 ffd8 ffc1 d7c3 ffc2 d7c3 ffc2  ................
+00000bc0: d7c3 ffc2 d7c5 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00000bd0: d7ff ffff ffff ffff ffff ffe8 ffd8 ffc1  ................
+00000be0: d7c4 ffc2 d7c2 ffc2 d7c3 ffc2 d7c2 ffc1  ................
+00000bf0: d7c2 ffc2 d7c2 ffc2 d7c1 ffc2 d7c2 ffc1  ................
+00000c00: d7ff ffff ffff ffff ffff ffe5 ffd7 ffc3  ................
+00000c10: d7c2 ffc8 d7c3 ffc3 d7c3 ffc7 d7c1 ffc3  ................
+00000c20: d7ff ffff ffff ffff ffff ffe6 ffff ffff  ................
+00000c30: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+00000c40: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+00000c50: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+00000c60: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+00000c70: ffdf ffff ffff ffd4 ffc8 00c8 ffd4 00cc  ................
+00000c80: ffca 00c7 88cb 00d4 ffd4 00cc ffc8 00c8  ................
+00000c90: ffd4 00cc ffcb 00c7 88ca 00d4 ffd4 00d3  ................
+00000ca0: ffff ffff ffd4 ffc3 d7c2 8858 8858 c8ff  ...........X.X..
+00000cb0: c900 c1d7 c1d8 c900 ccff ca00 c258 6a58  .............XjX
+00000cc0: 6ac2 58cb 00d4 ffc9 00c1 d8c1 d7c9 00cc  j.X.............
+00000cd0: ffc3 d7c2 8858 8858 c8ff c900 c1d7 c1d8  .....X.X........
+00000ce0: c900 ccff cb00 c258 6a58 6ac2 58ca 00d4  .......XjXj.X...
+00000cf0: ffc9 00c1 d8c1 d7c9 00d3 ffff ffff ffd4  ................
+00000d00: ffc3 d7c1 d888 58c2 88c8 ffc7 00c1 d7c3  ......X.........
+00000d10: d888 c1d8 c1d7 88c5 00cc ffc2 00c1 d7c2  ................
+00000d20: d8c3 88c1 d8c1 d7c2 6a20 6a20 c26a c688  ........j j .j..
+00000d30: c2d8 c300 d4ff c500 88c1 d7c1 d888 c3d8  ................
+00000d40: c1d7 c700 ccff c3d7 c1d8 8858 c288 c8ff  ...........X....
+00000d50: c700 c1d7 c3d8 88c1 d8c1 d788 c500 ccff  ................
+00000d60: c300 c1d7 c2d8 c388 c1d8 c1d7 c26a 206a  .............j j
+00000d70: 20c2 6ac6 88c2 d8c2 00d4 ffc5 0088 c1d7   .j.............
+00000d80: c1d8 88c3 d8c1 d7c7 00d3 ffff ffff ffd4  ................
+00000d90: ffc2 d7c1 d888 c1d7 6a58 88c8 ffc5 00c1  ........jX......
+00000da0: d7c3 d8c2 88c1 d888 c1d8 c358 c300 ccff  ...........X....
+00000db0: c200 c1d8 88c5 58c1 d8c7 2058 6a58 6ac3  ......X... XjXj.
+00000dc0: 5888 c300 d4ff c300 c358 c1d8 88c1 d8c2  X........X......
+00000dd0: 88c3 d8c1 d7c5 00cc ffc2 d7c1 d888 c1d7  ................
+00000de0: 6a58 88c8 ffc5 00c1 d7c3 d8c2 88c1 d888  jX..............
+00000df0: c1d8 c358 c300 ccff c300 c1d8 88c5 58c1  ...X..........X.
+00000e00: d8c7 2058 6a58 6ac3 5888 c200 d4ff c300  .. XjXj.X.......
+00000e10: c358 c1d8 88c1 d8c2 88c3 d8c1 d7c5 00d3  .X..............
+00000e20: ffff ffff ffd4 ffc1 d8c2 88c2 58c2 20c1  ............X. .
+00000e30: d8c8 ffc5 00c1 c781 c288 c2d8 88c2 58c1  ..............X.
+00000e40: d8c2 88c2 5800 ccff c200 88c2 58c3 6a58  ....X.......X.jX
+00000e50: 88c1 c8c1 c984 8381 c1c9 c1ca 6a58 c46a  ............jX.j
+00000e60: c258 c300 d4ff 00c2 d8c2 88c1 d8c2 5888  .X............X.
+00000e70: c2d8 c288 81c1 ccc5 00cc ffc1 d8c2 88c2  ................
+00000e80: 58c2 20c1 d8c8 ffc5 00c1 c781 c288 c2d8  X. .............
+00000e90: 88c2 58c1 d8c2 88c2 5800 ccff c300 88c2  ..X.....X.......
+00000ea0: 58c3 6a58 88c1 c8c1 c984 8381 c1c9 c1ca  X.jX............
+00000eb0: 6a58 c46a c258 c200 d4ff 00c2 d8c2 88c1  jX.j.X..........
+00000ec0: d8c2 5888 c2d8 c288 81c1 ccc5 00d3 ffff  ..X.............
+00000ed0: ffff ffd4 ffc1 d8c2 88c2 5820 586a c8ff  ..........X Xj..
+00000ee0: c500 c1c7 83c1 c8c1 c988 c258 c2d8 c1cb  ...........X....
+00000ef0: c258 c2d8 00cc ffc2 0088 58c5 6a88 c1ca  .X........X.j...
+00000f00: c1c9 8384 83c1 cbc1 ca20 6ac3 20c2 6a58  ......... j. .jX
+00000f10: c300 d4ff 00c2 d7c2 d8c1 c9c2 d8c2 5888  ..............X.
+00000f20: c2ca 83c1 cbc5 00cc ffc1 d8c2 88c2 5820  ..............X 
+00000f30: 586a c8ff c500 c1c7 83c1 c8c1 c988 c258  Xj.............X
+00000f40: c2d8 c1cb c258 c2d8 00cc ffc3 0088 58c5  .....X........X.
+00000f50: 6a88 c1ca c1c9 8384 83c1 cbc1 ca20 6ac3  j............ j.
+00000f60: 20c2 6a58 c200 d4ff 00c2 d7c2 d8c1 c9c2   .jX............
+00000f70: d8c2 5888 c2ca 83c1 cbc5 00d3 ffff ffff  ..X.............
+00000f80: ffd4 ffc1 d8c2 88c2 5820 58c1 d8c8 ffc3  ........X X.....
+00000f90: 00c1 d888 c1d7 c1d8 c1c7 c1c8 81c1 c9c1  ................
+00000fa0: cb83 81c1 cbc2 d8c1 cac2 00cc ffc2 0028  ...............(
+00000fb0: 00c8 cac3 cbc8 ca00 28c3 00d4 ffc2 00c1  ........(.......
+00000fc0: cac2 d7c1 c981 83c1 c9c1 ca81 c1ca c1cb  ................
+00000fd0: c1d8 c1d7 c2d8 c300 ccff c1d8 c288 c258  ...............X
+00000fe0: 2058 c1d8 c8ff c300 c1d8 88c1 d7c1 d8c1   X..............
+00000ff0: c7c1 c881 c1c9 c1cb 8381 c1cb c2d8 c1ca  ................
+00001000: c200 ccff c300 2800 c8ca c3cb c8ca 0028  ......(........(
+00001010: c200 d4ff c200 c1ca c2d7 c1c9 8183 c1c9  ................
+00001020: c1ca 81c1 cac1 cbc1 d8c1 d7c2 d8c3 00d3  ................
+00001030: fff5 ffc1 d7d5 ffc2 d7cd ffc3 d7c1 ffc1  ................
+00001040: d7c6 ffc3 d7ea ffc1 c7c3 c8c2 c9c2 cac8  ................
+00001050: ff00 c2d8 c288 c1d7 c258 c1d8 83c1 c9c1  .........X......
+00001060: ca84 83c1 ca83 81c1 ca15 00cc ffc2 0028  ...............(
+00001070: 58c1 c984 8381 c2ca c7cb c2cc 8483 81c1  X...............
+00001080: cc6a 28c3 00d4 ff00 20c1 ca81 83c1 ca83  .j(..... .......
+00001090: 81c1 cac1 cb83 c1d8 c258 c1d7 c288 c2d8  .........X......
+000010a0: 00cc ffc1 c7c3 c8c2 c9c2 cac8 ff00 c2d8  ................
+000010b0: c288 c1d7 c258 c1d8 83c1 c9c1 ca84 83c1  .....X..........
+000010c0: ca83 81c1 ca15 00cc ffc3 0028 58c1 c984  ...........(X...
+000010d0: 8381 c2ca c7cb c2cc 8483 81c1 cc6a 28c2  .............j(.
+000010e0: 00d4 ff00 20c1 ca81 83c1 ca83 81c1 cac1  .... ...........
+000010f0: cb83 c1d8 c258 c1d7 c288 c2d8 00d3 fff4  .....X..........
+00001100: ffc2 d7d2 ffc1 d7c2 ffc2 d7cc ffc2 d7c2  ................
+00001110: ffc2 d7c7 ffc2 d7ea ffc1 c883 81c2 c983  ................
+00001120: 81c1 cac8 ffc2 00c1 c7c2 d858 c288 c258  ...........X...X
+00001130: c1cb c3ca c1cb 8483 4328 00cc ffc2 0028  ........C(.....(
+00001140: 58c1 c983 8483 c1ca c5cb c1cc c1cb c1cc  X...............
+00001150: c2cb 8384 83c1 cc6a 28c3 00d4 ff00 2840  .......j(.....(@
+00001160: 8381 c1c9 c1ca c1c9 c1ca c1c9 c2d8 c288  ................
+00001170: 58c2 d8c1 cac2 00cc ffc1 c883 81c2 c983  X...............
+00001180: 81c1 cac8 ffc2 00c1 c7c2 d858 c288 c258  ...........X...X
+00001190: c1cb c3ca c1cb 8483 4328 00cc ffc3 0028  ........C(.....(
+000011a0: 58c1 c983 8483 c1ca c5cb c1cc c1cb c1cc  X...............
+000011b0: c2cb 8384 83c1 cc6a 28c2 00d4 ff00 2840  .......j(.....(@
+000011c0: 8381 c1c9 c1ca c1c9 c1ca c1c9 c2d8 c288  ................
+000011d0: 58c2 d8c1 cac2 00d3 fff4 ffc3 d7d1 ffc1  X...............
+000011e0: d7cf ffc2 d7c4 ffc1 d7c7 ffc2 d7ea ffc1  ................
+000011f0: d7c1 d888 58c2 6a58 88c8 ffc2 0080 c1c7  ....X.jX........
+00001200: c1d7 c2d8 c258 c2d8 c4ca 4243 c1c9 5800  .....X....BC..X.
+00001210: ccff c200 2858 c240 c241 c542 c643 3443  ....(X.@.A.B.C4C
+00001220: c234 6a28 58c2 00d4 ff00 58c1 c940 41c2  .4j(X.....X..@A.
+00001230: cac1 c9c1 cac2 d7c2 d8c2 88c1 d7c1 ca80  ................
+00001240: c200 ccff c1d7 c1d8 8858 c26a 5888 c8ff  .........X.jX...
+00001250: c200 80c1 c7c1 d7c2 d8c2 58c2 d8c4 ca42  ..........X....B
+00001260: 43c1 c958 00cc ffc2 0058 2858 c240 c241  C..X.....X(X.@.A
+00001270: c542 c643 3443 c234 6a28 c200 d4ff 0058  .B.C4C.4j(.....X
+00001280: c1c9 4041 c2ca c1c9 c1ca c2d7 c2d8 c288  ..@A............
+00001290: c1d7 c1ca 80c2 00d3 fff3 ffc1 d7c1 ffc2  ................
+000012a0: d7c3 ffc3 d7c1 ffc2 d7c1 ffc4 d7c1 ffc7  ................
+000012b0: d7c2 ffc4 d7c5 ffc2 d7c7 ffc3 d7c2 ffc4  ................
+000012c0: d7c3 ffc3 d7c3 ffc3 d7c3 ffc4 d7c2 ffc3  ................
+000012d0: d7d0 ffc2 d888 5888 6a58 88c8 ff00 c228  ......X.jX.....(
+000012e0: c1c7 c2d7 c1c7 c2d8 8381 c2ca c242 c2c9  .............B..
+000012f0: c1d8 8800 ccff c200 1558 d3cb 6a0b 58c2  .........X..j.X.
+00001300: 00d4 ff00 88c1 d8c2 c940 41c2 ca81 83c2  .........@A.....
+00001310: d7c1 cac2 d7c1 cac2 0b00 ccff c2d8 8858  ...............X
+00001320: 886a 5888 c8ff 00c2 28c1 c7c2 d7c1 c7c2  .jX.....(.......
+00001330: d883 81c2 cac2 42c2 c9c1 d888 00cc ffc2  ......B.........
+00001340: 0058 1558 d3cb 6a0b c200 d4ff 0088 c1d8  .X.X..j.........
+00001350: c2c9 4041 c2ca 8183 c2d7 c1ca c2d7 c1ca  ..@A............
+00001360: c20b 00d3 fff3 ffc1 d7c2 ffc2 d7c3 ffc3  ................
+00001370: d7c1 ffc3 d7c1 ffc2 d7c2 ffc2 d7c2 ffc2  ................
+00001380: d7c1 ffc2 d7c1 ffc2 d7c5 ffc2 d7c6 ffc2  ................
+00001390: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+000013a0: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+000013b0: d7c2 ffc1 d7c1 ffc2 d7c1 ffc2 d7cf ffc1  ................
+000013c0: d788 58c4 6a88 c8ff 0028 20c2 28c1 d780  ..X.j....( .(...
+000013d0: c1c7 c1ca 8483 c241 c2c9 88c1 d8c3 00cc  .......A........
+000013e0: ffc2 0020 d5d8 20c3 00d4 ffc3 00c1 d888  ... .. .........
+000013f0: c2c9 4041 8381 c1c9 c1ca 80c1 d7c2 0b20  ..@A........... 
+00001400: 0b00 ccff c1d7 8858 c46a 88c8 ff00 2820  .......X.j....( 
+00001410: c228 c1d7 80c1 c7c1 ca84 83c2 41c2 c988  .(..........A...
+00001420: c1d8 c300 ccff c300 20d5 d820 c200 d4ff  ........ .. ....
+00001430: c300 c1d8 88c2 c940 4183 81c1 c9c1 ca80  .......@A.......
+00001440: c1d7 c20b 200b 00d3 fff3 ffc5 d7c3 ffc2  .... ...........
+00001450: d7c3 ffc2 d7c5 ffc2 d7c2 ffc2 d7c1 ffc2  ................
+00001460: d7c8 ffc2 d7c9 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+00001470: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+00001480: d7c1 ffc3 d7c3 ffc5 d7cf ffc1 d788 586a  ..............Xj
+00001490: 886a 5888 c8ff 00c2 88c2 20c2 28c1 c7c1  .jX....... .(...
+000014a0: cac2 41c2 c9c1 d7c6 00cc ffc2 00c1 d758  ..A............X
+000014b0: 6ac1 d758 6ac1 d7c9 00c1 d858 6ac1 d758  j..Xj......Xj..X
+000014c0: 6ac1 d7c3 00d4 ffc6 00c1 d7c2 c940 41c1  j............@A.
+000014d0: c9c1 cac2 0bc2 20c2 8800 ccff c1d7 8858  ...... ........X
+000014e0: 6a88 6a58 88c8 ff00 c288 c220 c228 c1c7  j.jX....... .(..
+000014f0: c1ca c241 c2c9 c1d7 c600 ccff c300 c1d7  ...A............
+00001500: 586a c1d7 586a c1d7 c900 c1d8 586a c1d7  Xj..Xj......Xj..
+00001510: 586a c1d7 c200 d4ff c600 c1d7 c2c9 4041  Xj............@A
+00001520: c1c9 c1ca c20b c220 c288 00d3 fff2 ffc1  ....... ........
+00001530: d7c3 ffc2 d7c3 ffc2 d7c3 ffc2 d7c5 ffc2  ................
+00001540: d7c2 ffc2 d7c1 ffc2 d7c8 ffc2 d7c7 ffc4  ................
+00001550: d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2  ................
+00001560: d7c1 ffc2 d7c1 ffc2 d7c3 ffc3 d7c1 ffc2  ................
+00001570: d7d2 ff58 c6d7 58c8 ff00 c2d8 c288 2028  ...X..X....... (
+00001580: c1c7 40c2 c9c1 d7c8 00fc ffc8 00c1 d7c2  ..@.............
+00001590: c940 c1ca 0b20 c288 c2d8 00cc ff58 c6d7  .@... .......X..
+000015a0: 58c8 ff00 c2d8 c288 2028 c1c7 40c2 c9c1  X....... (..@...
+000015b0: d7c8 00fc ffc8 00c1 d7c2 c940 c1ca 0b20  ...........@... 
+000015c0: c288 c2d8 00d3 fff2 ffc1 d7c4 ffc2 d7c2  ................
+000015d0: ffc2 d7c3 ffc2 d7c2 ffc1 d7c2 ffc2 d7c2  ................
+000015e0: ffc2 d7c1 ffc2 d7c2 ffc1 d7c6 ffc2 d7c3  ................
+000015f0: ffc1 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1  ................
+00001600: ffc2 d7c1 ffc2 d7c1 ffc2 d7c1 ffc2 d7c1  ................
+00001610: ffc2 d7c1 ffc1 d7c2 ffc2 d7c1 ffc2 d7c2  ................
+00001620: ffc1 d7cf ffc1 c780 c1c7 c1d7 c1d8 c1c7  ................
+00001630: 81c1 c9c8 ffc3 00c2 d8c2 8858 c1c9 88c1  ...........X....
+00001640: d8c9 00fc ffc9 00c1 d888 c1c9 58c2 88c2  ............X...
+00001650: d8c3 00cc ffc1 c780 c1c7 c1d7 c1d8 c1c7  ................
+00001660: 81c1 c9c8 ffc3 00c2 d8c2 8858 c1c9 88c1  ...........X....
+00001670: d8c9 00fc ffc9 00c1 d888 c1c9 58c2 88c2  ............X...
+00001680: d8c3 00d3 fff1 ffc3 d7c2 ffc8 d7c3 ffc3  ................
+00001690: d7c3 ffc7 d7c1 ffc3 d7c8 ffc4 d7c3 ffc6  ................
+000016a0: d7c1 ffc2 d7c3 ffc3 d7c3 ffc3 d7c2 ffc4  ................
+000016b0: d7c3 ffc3 d7d0 ffc3 c7c1 d7c1 d8c1 c8c2  ................
+000016c0: c9c8 ffc5 00c2 d888 c1d8 cb00 fcff cb00  ................
+000016d0: c1d8 88c2 d8c5 00cc ffc3 c7c1 d7c1 d8c1  ................
+000016e0: c8c2 c9c8 ffc5 00c2 d888 c1d8 cb00 fcff  ................
+000016f0: cb00 c1d8 88c2 d8c5 00d3 ffff ffff ffd4  ................
+00001700: ff28 2028 c1d7 c1d8 c228 15ff fff9 ff28  .( (.....(.....(
+00001710: 2028 c1d7 c1d8 c228 15ff ffff ffc1 ffff   (.....(........
+00001720: ffff ffd4 ff20 2820 c26a 2015 28ff fff9  ..... ( .j .(...
+00001730: ff20 2820 c26a 2015 28ff ffff ffc1 ffff  . ( .j .(.......
+00001740: ffff ffd4 ffc8 d8ff fff9 ffc8 d8ff ffff  ................
+00001750: ffc1 ffff ffff ffd4 ffc3 58c2 d8c3 58ff  ..........X...X.
+00001760: fff9 ffc3 58c2 d8c3 58ff ffff ffc1 ffff  ....X...X.......
+00001770: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+00001780: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+00001790: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+000017a0: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+000017b0: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+000017c0: ffdf ffff ffff ffff ffff ffff ffff ffdf  ................
+000017d0: ffff ffff ffff ffff ffff ffff ffdf ffff  ................
+000017e0: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+000017f0: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+00001800: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+00001810: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+00001820: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+00001830: ffdf ffff ffff ffff ffff ffff ffff ffdf  ................
+00001840: ffff ffff ffff ffff ffff ffff ffdf ffff  ................
+00001850: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+00001860: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+00001870: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+00001880: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+00001890: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+000018a0: ffdf ffff ffff ffff ffff ffff ffff ffdf  ................
+000018b0: ffff ffff ffff ffff ffff ffff ffdf ffff  ................
+000018c0: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+000018d0: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+000018e0: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+000018f0: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+00001900: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+00001910: ffdf ffff ffff ffff ffff ffff ffff ffdf  ................
+00001920: ffff ffff ffff ffff ffff ffff ffdf ffff  ................
+00001930: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+00001940: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+00001950: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+00001960: ffff ffff ffdf ffff ffff ffff ffff ffff  ................
+00001970: ffff ffdf ffff ffff ffff ffff ffff ffff  ................
+00001980: ffdf ffff ffff ffff ffff ffff ffff ffdf  ................
+00001990: ffff ffff ffff ffff ffff ffff ffdf ffff  ................
+000019a0: ffff ffff ffff ffff ffff ffdf ffff ffff  ................
+000019b0: ffff ffff ffff ffff ffdf ffff ffff ffff  ................
+000019c0: ffff ffff ffff ffdf ffff ffff ffff ffff  ................
+000019d0: ffff ffff ffdf ffff ffff ffd0 ff00 c1c6  ................
+000019e0: c4c8 c1c7 00c8 ffcd 00c1 c7c2 c9c1 c8c4  ................
+000019f0: 00ca ffce 00c2 c728 20c1 c7c1 c9c1 c7c1  .......( .......
+00001a00: c9c1 c7c1 c9c1 c7c1 c9c1 c7c5 00d1 ffc4  ................
+00001a10: 00c1 c9d0 00cb ff00 c2c8 c4c9 00c8 ffd0  ................
+00001a20: 00c1 c6c4 00cb ffc5 00c9 c720 28c2 c7ce  ........... (...
+00001a30: 00d0 ffc4 00c1 c6c1 c7c2 c8cd 00d6 ffff  ................
+00001a40: ffff ffd0 ffc1 c6c1 c8c4 cac1 c9c1 c8c8  ................
+00001a50: ffcb 00c1 c7c1 c9c2 cac2 cbc1 cac1 c9c2  ................
+00001a60: 00ca ffcd 0010 c4c9 c2ca c5cb c1ca c1c9  ................
+00001a70: 12c4 00d1 ffc2 00c4 cac1 c9ce 00cb ffc1  ................
+00001a80: c7c1 c9c2 cac1 cbc2 cac1 c9c8 ffce 00c1  ................
+00001a90: c6c1 c9c2 cac1 c9c2 00cb ffc4 00c1 d8c1  ................
+00001aa0: c7c1 c8c1 c9c3 cac3 cbc2 c9c2 cb12 cd00  ................
+00001ab0: d0ff c200 c1c7 c1c9 c4ca c1c9 c1c8 cb00  ................
+00001ac0: d6ff ffff ffff d0ff c1c6 c4ca c1cb c1ca  ................
+00001ad0: c1c9 c8ff c900 c1c7 8812 c1ca c4cb c2ca  ................
+00001ae0: c1cc 00ca ff00 c3c6 c6c7 c2c8 c1c7 10c1  ................
+00001af0: c9c1 cb20 58c5 cbc2 ccc1 cbc1 ca13 c2cb  ... X...........
+00001b00: c200 d1ff 00c1 cac4 cbc2 cac1 c9cc 00cb  ................
+00001b10: ffc1 c7c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8  ................
+00001b20: ffcc 00c1 c6c1 c9c2 cac2 cbc2 ca00 cbff  ................
+00001b30: c200 c2c9 10c1 c8c1 cac4 cbc3 cc20 28c1  ............. (.
+00001b40: ccc1 cd13 c2c8 c4c6 c6c7 00d0 ff00 10c1  ................
+00001b50: c6c1 c8c1 cac3 cbc1 ca12 88c1 c8c9 00d6  ................
+00001b60: ffcd ffc8 d7e4 ffc2 d7c1 ffc2 d7c1 ffc8  ................
+00001b70: d7cc ffc3 d7cb ffc2 d7c1 ffc2 d7e8 ffc1  ................
+00001b80: c7c1 cbc2 cac2 cbc2 cac8 ffc7 00c1 c713  ................
+00001b90: 12c2 ca88 12c1 ccc1 cbc1 cac1 cc13 c1cc  ................
+00001ba0: 20ca ff88 c1ca c5cb c1ca c1cb c1ca c2c9   ...............
+00001bb0: c1c8 10c1 c9c3 cac2 cbc1 ccc1 cbc1 ccc4  ................
+00001bc0: cb14 c2cc be00 d1ff c2c9 c2ca c3cb c2ca  ................
+00001bd0: c1c9 c1c8 c2c9 c1c8 c700 cbff c1c7 c1c9  ................
+00001be0: c1ca c1cb c1cc c1cb c1ca c1c9 c8ff c700  ................
+00001bf0: c2c8 c1c9 c1c8 c2ca c3cb c3cc c1cb c1ca  ................
+00001c00: cbff 00be c2ca 11c3 c9c2 cac7 cbc1 ca15  ................
+00001c10: c1c8 c2c9 c6cb c1ca c1cb c1ca 88d0 ffc2  ................
+00001c20: 8810 c2c8 c2cb 1388 c2cb 1312 c1c8 c700  ................
+00001c30: d6ff cdff c1d7 c2ff c2d7 c2ff c1d7 e4ff  ................
+00001c40: c2d7 c1ff c2d7 c1ff c1d7 c2ff c2d7 c2ff  ................
+00001c50: c1d7 cdff c2d7 cbff c2d7 c1ff c2d7 e8ff  ................
+00001c60: c1c8 1011 c1cb c1cc 1011 c1ca c8ff c700  ................
+00001c70: c1c7 12c1 ca11 12c3 cbc1 cc13 c2cd 1620  ............... 
+00001c80: caff 88c1 cbc2 ccc3 cdc1 ccc2 cbc1 cac2  ................
+00001c90: c911 c1ca 12c1 cb12 c1cc 13c1 cc13 c1cd  ................
+00001ca0: 14c1 cdc3 14c2 cdc1 f510 d1ff 11c3 c9c3  ................
+00001cb0: cac1 c9c1 c8c1 c9c2 ca10 12c1 c9c1 c8c5  ................
+00001cc0: 00cb ffc1 c8c1 c9c1 cac1 cbc1 ccc1 cbc2  ................
+00001cd0: cac8 ffc5 00c1 c8c1 c910 11c1 cbc1 c9c2  ................
+00001ce0: cac1 cbc2 ccc1 cdc1 ccc2 cbc1 cacb ff58  ...............X
+00001cf0: 21c2 cac2 1211 c1ca 12c1 cb12 c1cc 13c1  !...............
+00001d00: cc13 c1cd 14c1 cd17 c2c9 c1ca c3cc c3cd  ................
+00001d10: c1cc c1cd c1cc 88d0 ffc1 d812 11c1 c810  ................
+00001d20: c2ca c2cb 1614 c1cb 14c1 cac7 00d6 ffd0  ................
+00001d30: ffc2 d7e7 ffc2 d7c1 ffc2 d7c4 ffc2 d7d0  ................
+00001d40: ffc2 d7cb ffc2 d7c1 ffc2 d7e8 ffc1 c911  ................
+00001d50: c1ca c1cb c1cc c1cb 12c1 c9c8 ffc5 00c1  ................
+00001d60: c6c3 c9c1 c8c1 ca12 c1ca c1cb 13c2 cd17  ................
+00001d70: c20d 58ca ffc1 d8c1 cac3 cbc1 cac1 cbc1  ..X.............
+00001d80: cac1 cbc3 cac1 cbc1 cac1 cbc1 cac1 ccc1  ................
+00001d90: cac1 cc13 c1cd 14c1 cd16 c1cd c216 c1cc  ................
+00001da0: c216 be6a d1ff 12c1 f510 c4c9 c1c6 c1c8  ...j............
+00001db0: c1ca 1012 c2cb c2ca c1c9 c1c8 c300 cbff  ................
+00001dc0: c1c8 c1c9 c1ca c2cc c2ca c1c9 c8ff c300  ................
+00001dd0: c1c6 c2c9 c2ca c1cb 1113 c2c9 c1ca c1cb  ................
+00001de0: c2cc c1cb c1ca c215 cbff 6abe c213 c1c9  ..........j.....
+00001df0: 1211 c1cb 12c1 cb12 c1cc 14c6 cdc1 cbc2  ................
+00001e00: cac8 cbc1 cac1 d8d0 ffc1 d8c2 2112 c1c9  ............!...
+00001e10: c1ca 10c2 cb15 c1cb c1ca c2c9 c1ca c1c9  ................
+00001e20: c500 d6ff d0ff c2d7 c3ff c3d7 c1ff c2d7  ................
+00001e30: c1ff c3d7 c1ff c5d7 c1ff c2d7 c2ff c3d7  ................
+00001e40: c2ff c3d7 c1ff c2d7 cdff c2d7 c3ff c3d7  ................
+00001e50: c1ff c2d7 c1ff c3d7 c1ff c6d7 c3ff c3d7  ................
+00001e60: f0ff c1c9 c1ca c4cb c1ca c1cc c8ff c300  ................
+00001e70: c1c6 c1c9 c2ca c2cb c1ca c2c9 13c2 cc17  ................
+00001e80: 0d0e c20c c1d8 caff 20c2 cdc2 ccc2 cdc1  ........ .......
+00001e90: ccc5 cdc1 ccc1 cdc2 ccc8 cdc1 ccc2 cdc2  ................
+00001ea0: 0c28 58d1 ffc2 2811 2810 c1c9 c1c6 c211  .(X...(.(.......
+00001eb0: c1c8 c1ca c2cb c1cc c2cb c2ca c1c8 c200  ................
+00001ec0: cbff c1c7 c1c9 c3ca c1c9 c2ca c8ff c300  ................
+00001ed0: c1c8 c1c9 c2ca c2cb c1cc c1cb c1ca c1cc  ................
+00001ee0: c1cd c2cb 1513 1517 15cb ffc1 d821 c2f5  .............!..
+00001ef0: c3cb c7cc c1cd c2ca c1cc c1ca c1cb c1cc  ................
+00001f00: c1ca c1cb c1cc c1ca c1cb c1cc c1ca c1cb  ................
+00001f10: c2cc 20d0 ffc1 d8c2 20c2 2113 c1c8 c1ca  .. ..... .!.....
+00001f20: 10c1 cbc1 cac1 c9c1 cac2 cbc2 cac1 c9c3  ................
+00001f30: 00d6 ffd0 ffc2 d7c4 ffc2 d7c1 ffc2 d7c2  ................
+00001f40: ffc3 d7c1 ffc1 d7c1 ffc5 d7c1 ffc2 d7c1  ................
+00001f50: ffc2 d7c2 ffc3 d7c1 ffc1 d7cd ffc2 d7c4  ................
+00001f60: ffc2 d7c1 ffc2 d7c2 ffc3 d7c1 ffc3 d7c1  ................
+00001f70: ffc2 d7c1 ffc2 d7c1 ffc2 d7ef ffc2 14c1  ................
+00001f80: ca14 13c1 ca12 14c8 ff00 c1c6 c1c9 c2ca  ................
+00001f90: c2cb c2cc c1cd c2cb c1cc 1614 0e0d 0c0a  ................
+00001fa0: c1c9 00ca ff6a 0c0e 1513 0e15 130f 1413  .....j..........
+00001fb0: 0f14 120e 1311 0ec9 0d0e c217 c1f5 88d1  ................
+00001fc0: ff58 c221 2811 1211 c1ca c1c9 10c3 cac2  .X.!(...........
+00001fd0: cbc1 cc14 c1cc 13c2 00cb ffc1 c6c1 c8c6  ................
+00001fe0: c9c8 ffc2 0010 c1c9 14c2 cac1 ccc1 cbc1  ................
+00001ff0: cac1 cb13 c1cd c1cc 1315 1716 0d0c 28cb  ..............(.
+00002000: ffc1 d728 c215 ca0b 0e11 130e 1214 0f13  ...(............
+00002010: 140f 1315 0e13 150e 0c6a d0ff 00c1 c8c2  .........j......
+00002020: 20c2 2111 10c2 c8c3 c9c2 cac2 cbc1 cac2   .!.............
+00002030: c900 d6ff d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00002040: c2ff c2d7 c4ff c2d7 c1ff c2d7 c1ff c5d7  ................
+00002050: c2ff c2d7 d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00002060: c2ff c2d7 c3ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002070: c1ff c2d7 efff c1cb 13c1 c8c2 cac1 c913  ................
+00002080: c1cc c8ff c2c7 c1c8 c2ca c1cb c1cc c1cd  ................
+00002090: c2cc c1cb c1ca 130c 150c 0b28 c1d7 c1c7  ...........(....
+000020a0: 00ca ff58 0c0e 1615 0e16 150e 1614 0d15  ...X............
+000020b0: 140d 1312 ca0d 0ec2 0c28 c1d8 d1ff c1d7  .........(......
+000020c0: 58c2 2021 2812 2820 c1c9 c1ca 10c3 ca16  X. !(.( ........
+000020d0: 15c1 cbc1 cc28 00cb ffc1 c610 11c1 cac1  .....(..........
+000020e0: cb10 11c1 c9c8 ff00 12c2 cb12 14c1 cbc2  ................
+000020f0: ca13 c2cd 120d 1517 0d0b 0a21 c1d7 cbff  ...........!....
+00002100: c1d7 20c1 f515 ca0b 0d12 130d 1415 0d14  .. .............
+00002110: 160e 1516 0e15 160e 0c58 d0ff 00c1 c6c1  .........X......
+00002120: d758 c220 6a11 c210 c1c8 c3c9 c2ca c2c9  .X. j...........
+00002130: c3ca d6ff d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00002140: c2ff c2d7 c4ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002150: c5ff c2d7 d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00002160: c2ff c2d7 c3ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002170: c1ff c2d7 efff c1c6 c1c7 c1ca c2cb c3ca  ................
+00002180: c8ff c210 c1d8 c2c8 c2cb c1cc c1cb c1ca  ................
+00002190: 160d 0c0b c1f5 0a28 c1d7 c300 caff c1d8  .......(........
+000021a0: 0acd 0b28 21c9 0b0c 0bc2 0a58 c1d7 d1ff  ...(!......X....
+000021b0: c200 586a 2021 c228 c2f5 14c1 c8c1 ca10  ..Xj !.(........
+000021c0: 12c3 cc16 bf6a cbff c1c7 11c1 cac1 cbc1  .....j..........
+000021d0: ccc1 cb12 c1ca c8ff 88bf 2814 c1cb c1cc  ..........(.....
+000021e0: c213 c2cd 0e0f 13c2 0d0b 0a21 6ac2 00cb  ...........!j...
+000021f0: ffc2 d721 c2f5 ca0a 2021 ce0a c1d8 d0ff  ...!.... !......
+00002200: c300 c1d7 58c2 6ac2 2011 2110 c1c9 c1c8  ....X.j. .!.....
+00002210: c2c9 c1ca c2d8 c2ca d6ff d0ff c2d7 c4ff  ................
+00002220: c2d7 c1ff c2d7 c2ff c2d7 c4ff c2d7 c1ff  ................
+00002230: c2d7 c1ff c2d7 c2ff c1d7 c2ff c2d7 d0ff  ................
+00002240: c2d7 c4ff c2d7 c1ff c2d7 c2ff c2d7 c3ff  ................
+00002250: c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 efff  ................
+00002260: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
+00002270: c8ff 10c2 d7c1 d8c2 c9c1 cbc1 ca13 16c2  ................
+00002280: 0d0c c1f5 2120 c500 caff c1d8 28cc 150a  ....! ......(...
+00002290: 2821 c40a c2f5 c328 c1f5 28c2 13c1 c600  (!.....(..(.....
+000022a0: d1ff c400 586a c221 20c1 f515 c1f5 14c2  ....Xj.! .......
+000022b0: cac1 cc0c bf6a 2821 cbff c1c8 c1c9 c1ca  .....j(!........
+000022c0: c1cb c1cc c1cb c1ca c1c9 c8ff 88c1 d858  ...............X
+000022d0: bfc1 f516 c1cc c1cd c20e 0f0e c1f5 0b0a  ................
+000022e0: 286a c400 cbff 00c1 c611 2120 28c3 21c2  (j........! (.!.
+000022f0: 28c4 f520 21cd f528 c1d8 d0ff c500 c258  (.. !..(.......X
+00002300: 6a20 c221 1128 10c2 c9c1 ca10 c2d8 c1c8  j .!.(..........
+00002310: d6ff cfff c4d7 c4ff c9d7 c2ff c3d7 c1ff  ................
+00002320: c3d7 c1ff c3d7 c2ff c4d7 ceff c4d7 c4ff  ................
+00002330: c9d7 c2ff c1d7 c1ff c2d7 c3ff c3d7 f0ff  ................
+00002340: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+00002350: c1d8 c3d7 10c1 c715 0f16 0d0c 0a28 20c7  .............( .
+00002360: 00ca ff6a 58c5 20c8 21c2 6ac4 2188 58c3  ...jX. .!.j.!.X.
+00002370: d7c2 88c1 d7c1 c8c1 c600 d1ff c600 58c2  ..............X.
+00002380: 6ac2 28c1 f515 c20a 0c6a 2058 206a cbff  j.(......j X j..
+00002390: c1c9 c2ca c3cb c2ca c8ff c1d8 88c3 6a0d  ..............j.
+000023a0: 0ec2 0f0e 0d0b c228 6ac6 00cb ff00 c1c6  .......(j.......
+000023b0: c1c8 c1d7 c288 c3d7 c288 c420 c26a cd20  ........... .j. 
+000023c0: 586a d0ff c700 586a c220 2128 1228 c1ca  Xj....Xj. !(.(..
+000023d0: c1c9 c2d8 c1d7 c1d8 d6ff ffff ffff d0ff  ................
+000023e0: c1c6 c1c9 c1ca c2cc c2ca c1c9 c8ff c4d7  ................
+000023f0: c1d8 1017 0d0b 0ac1 f520 c900 fbff c800  ......... ......
+00002400: 5820 2128 c1f5 0a0b 0ac2 586a 58c1 d8cb  X !(......XjX...
+00002410: ffc1 c9c5 cac1 cbc1 c9c8 ffc1 d7c1 d8c3  ................
+00002420: 880c c20e 0d0b 0a28 6ac8 00fb ffc9 0058  .......(j......X
+00002430: 6ac2 2021 28c1 ca10 c1d8 c3d7 d6ff ffff  j. !(...........
+00002440: ffff d0ff c1c6 c1c8 c2ca c2cb c2ca c8ff  ................
+00002450: c200 c3d7 c1c6 0c0a 2120 cb00 fbff ca00  ........! ......
+00002460: c1d8 8858 28c2 f5c2 d888 c1d8 c1d7 cbff  ...X(...........
+00002470: c1ca 11c1 cb13 14c1 cc0c c1cb c8ff c2d7  ................
+00002480: c3d8 c1f5 0b0c 2058 c1d8 ca00 fbff cb00  ...... X........
+00002490: 586a 2021 c1c8 c1d8 c2d7 c200 d6ff ffff  Xj !............
+000024a0: ffff d0ff c1c7 c2c8 c2ca c2c9 c1ca c8ff  ................
+000024b0: c400 c2d7 88c1 d7cd 00fb ffcc 00c1 d7c1  ................
+000024c0: c6c1 c888 c4d7 00cb ffc2 11c1 cb13 15c1  ................
+000024d0: cc0c 16c8 ff00 c4d7 10c1 c9c1 c8c1 d7cc  ................
+000024e0: 00fb ffcd 0058 88c2 d7c4 00d6 ffff ffff  .....X..........
+000024f0: ffd0 ffc1 c8c2 c9c2 cac1 cbc1 cac1 c9ff  ................
+00002500: ffd9 ffcf 00c1 c6c5 00cb ffc1 c8c1 c9c2  ................
+00002510: cbc1 ccc1 cbc1 cac1 c9c8 ffc5 00c1 c8cf  ................
+00002520: 00ff ffe7 ffff ffff ffd0 ffc1 c9c1 cac1  ................
+00002530: cbc2 d7c1 cac1 cbc1 caff fff9 ffc1 c8c1  ................
+00002540: c9c1 cbc3 ccc1 cac1 cbff ffff ffc5 ffff  ................
+00002550: ffff ffd0 ffc1 cac1 c9c1 d7c1 d8c2 d712  ................
+00002560: c1ca ffff f9ff c1c8 280a c20b 0c0e c1cb  ........(.......
+00002570: ffff ffff c5ff ffff ffff d0ff c2c9 c1d7  ................
+00002580: c1d8 c2d7 10c1 c8ff fff9 ff20 6abf 5821  ........... j.X!
+00002590: bf13 0cff ffff ffc5 ffff ffff ffd0 ffc2  ................
+000025a0: c7c1 d7c1 d8c2 d7c1 d8c1 c6ff fff9 ff20  ............... 
+000025b0: c288 6a20 136a 0bff ffff ffc5 ffff ffff  ..j .j..........
+000025c0: ffd0 ffc8 d7ff fff9 ff6a c1d8 8858 c26a  .........j...X.j
+000025d0: 8815 ffff ffff c5ff ffff ffff d0ff c8d7  ................
+000025e0: ffff f9ff 88c1 d7c1 d888 5888 c1d8 6aff  ..........X...j.
+000025f0: ffff ffc5 ffff ffff ffff ffff ffd2 ffc1  ................
+00002600: c7c1 d7c2 d888 c1d8 c1d7 c1c7 ffff ffff  ................
+00002610: c5ff ffff ffff ffff ffff d2ff c200 c4d7  ................
+00002620: c200 ffff ffff c5ff ffff ffff ffff ffff  ................
+00002630: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+00002640: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+00002650: dfff ffff ffff d0ff 00c2 c8c4 c900 c8ff  ................
+00002660: cf00 c1c6 c400 ccff c2c6 cbc7 c2c6 c5c7  ................
+00002670: c1c6 c6c7 00d4 ffc4 00c1 c9cf 00cc ff00  ................
+00002680: c2c8 c4c9 00c8 ffcf 00c1 c6c4 00cc ffc2  ................
+00002690: c6cb c7c2 c6c5 c7c1 c6c6 c700 d4ff c400  ................
+000026a0: c1c9 cf00 d7ff ffff ffff d0ff c1c7 c1c9  ................
+000026b0: c2ca c1cb c2ca c1c9 c8ff cd00 c1c6 c1c9  ................
+000026c0: c2ca c1c9 c200 ccff c2ca d6cb c1ca c1cb  ................
+000026d0: c1ca c1d8 d4ff c200 c4ca c1c9 cd00 ccff  ................
+000026e0: c1c7 c1c9 c2ca c1cb c2ca c1c9 c8ff cd00  ................
+000026f0: c1c6 c1c9 c2ca c1c9 c200 ccff c2ca d6cb  ................
+00002700: c1ca c1cb c1ca c1d8 d4ff c200 c4ca c1c9  ................
+00002710: cd00 d7ff ffff ffff d0ff c1c7 c1c9 c1ca  ................
+00002720: c1cb c1cc c1cb c2ca c8ff cb00 c1c6 c1c9  ................
+00002730: c2ca c2cb c2ca 00cc ffc1 cac1 cbc1 ccc3  ................
+00002740: cdc3 ccc3 cdc3 ccc1 cdc2 ccc1 cdc2 ccc3  ................
+00002750: cdc2 ccc1 cbc1 d8d4 ff00 c1ca c4cb c2ca  ................
+00002760: c1c9 cb00 ccff c1c7 c1c9 c1ca c1cb c1cc  ................
+00002770: c1cb c2ca c8ff cb00 c1c6 c1c9 c2ca c2cb  ................
+00002780: c2ca 00cc ffc1 cac1 cbc1 ccc3 cdc3 ccc3  ................
+00002790: cdc3 ccc1 cdc2 ccc1 cdc2 ccc3 cdc2 ccc1  ................
+000027a0: cbc1 d8d4 ff00 c1ca c4cb c2ca c1c9 cb00  ................
+000027b0: d7ff ffff ffff d0ff c1c6 c1c9 c1ca c1cb  ................
+000027c0: c1cc c1cb c1ca c1c9 c8ff c900 c1c7 c1c9  ................
+000027d0: c2ca c2cb c3cc c1cb c1ca ccff c1ca c3cb  ................
+000027e0: c1ca d5cb c1ca 88d4 ffc2 c9c2 cac4 cbc2  ................
+000027f0: cac1 c9c9 00cc ffc1 c6c1 c9c1 cac1 cbc1  ................
+00002800: ccc1 cbc1 cac1 c9c8 ffc9 00c1 c7c1 c9c2  ................
+00002810: cac2 cbc3 ccc1 cbc1 cacc ffc1 cac3 cbc1  ................
+00002820: cad5 cbc1 ca88 d4ff c2c9 c2ca c4cb c2ca  ................
+00002830: c1c9 c900 d7ff ffff ffff d0ff c1c6 c1c9  ................
+00002840: c1ca c1cb c1cc c1cb c2ca c8ff c700 c1c7  ................
+00002850: c1c9 c2ca c2cb c2cc c1cd c1cc c2cb c1ca  ................
+00002860: ccff c2cd c2cc c2cd c1cb c1cc c1ca c1cb  ................
+00002870: c1cc c1ca c1cb c2ca c1cb c1cc c1ca c1cb  ................
+00002880: c1cc c1ca c1cb c1cc c1ca c1cb c2cc 20d4  .............. .
+00002890: ff11 c3c9 c2ca c4cb c2ca c1c9 c700 ccff  ................
+000028a0: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+000028b0: c700 c1c7 c1c9 c2ca c2cb c2cc c1cd c1cc  ................
+000028c0: c2cb c1ca ccff c2cd c2cc c2cd c1cb c1cc  ................
+000028d0: c1ca c1cb c1cc c1ca c1cb c2ca c1cb c1cc  ................
+000028e0: c1ca c1cb c1cc c1ca c1cb c1cc c1ca c1cb  ................
+000028f0: c2cc 20d4 ff11 c3c9 c2ca c4cb c2ca c1c9  .. .............
+00002900: c700 d7ff ffff ffff d0ff c1c6 c1c9 c1ca  ................
+00002910: c1cb c1cc c1cb c1ca c1c9 c8ff c500 c1c6  ................
+00002920: c1c9 c2ca c2cb c2cc c1cd c2cc c1cb c1ca  ................
+00002930: c215 ccff 0f14 130e 1412 0d13 110c 1210  ................
+00002940: 0cc2 100c 1210 0c12 110d 1312 0f13 0f21  ...............!
+00002950: d4ff 12c1 f510 c3c9 c2ca c4cb c2ca c1c9  ................
+00002960: c500 ccff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
+00002970: c1ca c1c9 c8ff c500 c1c6 c1c9 c2ca c2cb  ................
+00002980: c2cc c1cd c2cc c1cb c1ca c215 ccff 0f14  ................
+00002990: 130e 1412 0d13 110c 1210 0cc2 100c 1210  ................
+000029a0: 0c12 110d 1312 0f13 0f21 d4ff 12c1 f510  .........!......
+000029b0: c3c9 c2ca c4cb c2ca c1c9 c500 d7ff cdff  ................
+000029c0: c8d7 ccff c3d7 d0ff c3d7 c1ff c1d7 d3ff  ................
+000029d0: c3d7 ffff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
+000029e0: c2ca c8ff c300 c1c6 c1c9 c2ca c2cb c2cc  ................
+000029f0: c1cd c2cc c1cb c1ca 1315 1715 ccff 0f16  ................
+00002a00: 140d 1513 0c14 130c 1413 0c13 120c 1413  ................
+00002a10: 0c14 130c 1514 0e14 0e20 d4ff c228 1128  ......... ...(.(
+00002a20: 10c3 c9c2 cac4 cbc2 cac1 c9c3 00cc ffc1  ................
+00002a30: c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8 ffc3  ................
+00002a40: 00c1 c6c1 c9c2 cac2 cbc2 ccc1 cdc2 ccc1  ................
+00002a50: cbc1 ca13 1517 15cc ff0f 1614 0d15 130c  ................
+00002a60: 1413 0c14 130c 1312 0c14 130c 1413 0c15  ................
+00002a70: 140e 140e 20d4 ffc2 2811 2810 c3c9 c2ca  .... ...(.(.....
+00002a80: c4cb c2ca c1c9 c300 d7ff cdff c1d7 c2ff  ................
+00002a90: c2d7 c2ff c1d7 cdff c2d7 cfff c2d7 c2ff  ................
+00002aa0: c2d7 d4ff c2d7 ffff c1c6 c1c9 c1ca c1cb  ................
+00002ab0: c1cc c1cb c1ca c1c9 c8ff 00c1 c6c1 c9c2  ................
+00002ac0: cac2 cbc2 ccc1 cdc2 ccc1 cbc1 ca13 0d16  ................
+00002ad0: 0d0c 28cc ffc4 0bc9 0a28 21c9 0ac3 0b88  ..(......(!.....
+00002ae0: d4ff 58c2 2128 1128 11c1 c8c2 c9c3 cac3  ..X.!(.(........
+00002af0: cbc1 cac2 c900 ccff c1c6 c1c9 c1ca c1cb  ................
+00002b00: c1cc c1cb c1ca c1c9 c8ff 00c1 c6c1 c9c2  ................
+00002b10: cac2 cbc2 ccc1 cdc2 ccc1 cbc1 ca13 0d16  ................
+00002b20: 0d0c 28cc ffc4 0bc9 0a28 21c9 0ac3 0b88  ..(......(!.....
+00002b30: d4ff 58c2 2128 1128 11c1 c8c2 c9c3 cac3  ..X.!(.(........
+00002b40: cbc1 cac2 c900 d7ff d0ff c2d7 d0ff c2d7  ................
+00002b50: ceff c2d7 c4ff c1d7 d4ff c2d7 ffff c1c6  ................
+00002b60: c1c9 c1ca c1cb c1cc c1cb c2ca c8ff c2c7  ................
+00002b70: c1c8 c2ca c1cb c1cc c1cd c2cc c1cb c1ca  ................
+00002b80: c215 160d 0b0a 21c1 d7cc ff28 21cb f521  ......!....(!..!
+00002b90: 20ca f521 2888 d4ff c1d7 58c2 2021 2821   ..!(.....X. !(!
+00002ba0: 1110 c4c9 c2ca c2c9 c3ca ccff c1c6 c1c9  ................
+00002bb0: c1ca c1cb c1cc c1cb c2ca c8ff c2c7 c1c8  ................
+00002bc0: c2ca c1cb c1cc c1cd c2cc c1cb c1ca c215  ................
+00002bd0: 160d 0b0a 21c1 d7cc ff28 21cb f521 20ca  ....!....(!..! .
+00002be0: f521 2888 d4ff c1d7 58c2 2021 2821 1110  .!(.....X. !(!..
+00002bf0: c4c9 c2ca c2c9 c3ca d7ff d0ff c2d7 c3ff  ................
+00002c00: c3d7 c1ff c2d7 c1ff c3d7 c1ff c6d7 c3ff  ................
+00002c10: c3d7 c6ff c2d7 c7ff c3d7 c3ff c3d7 c3ff  ................
+00002c20: c4d7 c2ff c2d7 c1ff c2d7 fcff c1c6 c1c9  ................
+00002c30: c1ca c1cb c1cc c1cb c1ca c1c9 c8ff c210  ................
+00002c40: c1d8 c2c8 c2cb c1cc c1cb c1ca 0d14 160a  ................
+00002c50: 0b0a 216a c200 ccff c1d8 c1d7 c258 d420  ..!j.........X. 
+00002c60: 58c1 d7c1 d86a d4ff c200 586a c320 6a11  X....j....Xj. j.
+00002c70: 2810 c1c9 c1c8 c2c9 c1ca c2d8 c2ca ccff  (...............
+00002c80: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
+00002c90: c8ff c210 c1d8 c2c8 c2cb c1cc c1cb c1ca  ................
+00002ca0: 0d14 160a 0b0a 216a c200 ccff c1d8 c1d7  ......!j........
+00002cb0: c258 d420 58c1 d7c1 d86a d4ff c200 586a  .X. X....j....Xj
+00002cc0: c320 6a11 2810 c1c9 c1c8 c2c9 c1ca c2d8  . j.(...........
+00002cd0: c2ca d7ff d0ff c2d7 c4ff c2d7 c1ff c2d7  ................
+00002ce0: c2ff c3d7 c1ff c3d7 c1ff c2d7 c1ff c2d7  ................
+00002cf0: c1ff c2d7 c5ff c2d7 c6ff c2d7 c1ff c2d7  ................
+00002d00: c1ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002d10: c2ff c5d7 fcff c1c6 c1c9 c1ca c1cb c1cc  ................
+00002d20: c1cb c2ca c8ff 10c2 d7c1 d8c2 c9c1 cbc1  ................
+00002d30: ca13 16c2 0d0a c1f5 216a c400 fcff c400  ........!j......
+00002d40: 58c3 6a21 2811 2813 c2c9 c1ca 10c2 d8c1  X.j!(.(.........
+00002d50: c8cc ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc2  ................
+00002d60: cac8 ff10 c2d7 c1d8 c2c9 c1cb c1ca 1316  ................
+00002d70: c20d 0ac1 f521 6ac4 00fc ffc4 0058 c36a  .....!j......X.j
+00002d80: 2128 1128 13c2 c9c1 ca10 c2d8 c1c8 d7ff  !(.(............
+00002d90: d0ff c2d7 c4ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00002da0: c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002db0: c5ff c2d7 c6ff c2d7 c1ff c2d7 c4ff c2d7  ................
+00002dc0: c1ff c2d7 c5ff c2d7 c1ff c2d7 fcff c1c6  ................
+00002dd0: c1c9 c1ca c1cb c1cc c1cb c1ca c1c9 c8ff  ................
+00002de0: c1d8 c3d7 10c1 c715 0f16 0d0b 0a20 6ac6  ............. j.
+00002df0: 00fc ffc6 00c2 58c2 2021 c328 c1ca c1c9  ......X. !.(....
+00002e00: c2d8 c1d7 c1d8 ccff c1c6 c1c9 c1ca c1cb  ................
+00002e10: c1cc c1cb c1ca c1c9 c8ff c1d8 c3d7 10c1  ................
+00002e20: c715 0f16 0d0b 0a20 6ac6 00fc ffc6 00c2  ....... j.......
+00002e30: 58c2 2021 c328 c1ca c1c9 c2d8 c1d7 c1d8  X. !.(..........
+00002e40: d7ff d0ff c2d7 c4ff c2d7 c1ff c2d7 c2ff  ................
+00002e50: c2d7 c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
+00002e60: c2d7 c5ff c2d7 c6ff c2d7 c1ff c2d7 c2ff  ................
+00002e70: c4d7 c1ff c2d7 c5ff c2d7 c1ff c2d7 fcff  ................
+00002e80: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+00002e90: c4d7 c1d8 1017 0d0b 0a21 6ac8 00fc ffc8  .........!j.....
+00002ea0: 0058 6ac2 2028 14c1 ca10 c1d8 c3d7 ccff  .Xj. (..........
+00002eb0: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+00002ec0: c4d7 c1d8 1017 0d0b 0a21 6ac8 00fc ffc8  .........!j.....
+00002ed0: 0058 6ac2 2028 14c1 ca10 c1d8 c3d7 d7ff  .Xj. (..........
+00002ee0: d0ff c2d7 c4ff c2d7 c1ff c2d7 c2ff c2d7  ................
+00002ef0: c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff c2d7  ................
+00002f00: c6ff c2d7 c3ff c1d7 c1ff c2d7 c1ff c2d7  ................
+00002f10: c1ff c2d7 c1ff c2d7 c1ff c2d7 c2ff c1d7  ................
+00002f20: c2ff c2d7 c1ff c2d7 fcff c1c7 c2c8 c2ca  ................
+00002f30: c2c9 c1ca c8ff c200 c3d7 c1c6 0c0a 2120  ..............! 
+00002f40: ca00 fcff ca00 586a 2021 10c1 c6c3 d700  ......Xj !......
+00002f50: ccff c1c7 c2c8 c2ca c2c9 c1ca c8ff c200  ................
+00002f60: c3d7 c1c6 0c0a 2120 ca00 fcff ca00 586a  ......! ......Xj
+00002f70: 2021 10c1 c6c3 d700 d7ff cfff c4d7 c4ff   !..............
+00002f80: c9d7 c2ff c1d7 c1ff c2d7 c3ff c3d7 c8ff  ................
+00002f90: c4d7 c3ff c3d7 c3ff c5d7 c1ff c3d7 c2ff  ................
+00002fa0: c3d7 c1ff c3d7 fbff c1c8 c2c9 c2ca c1cb  ................
+00002fb0: c1ca c1c9 c8ff c400 c2d7 88c1 d7cc 00fc  ................
+00002fc0: ffcc 00c1 d7c2 d8c2 d7c3 00cc ffc1 c8c2  ................
+00002fd0: c9c2 cac1 cbc1 cac1 c9c8 ffc4 00c2 d788  ................
+00002fe0: c1d7 cc00 fcff cc00 c1d7 c2d8 c2d7 c300  ................
+00002ff0: d7ff ffff ffff d0ff c1c9 c1ca c1cb c2d7  ................
+00003000: c1ca c1cb c1ca ffff d9ff ce00 c1d7 c500  ................
+00003010: ccff c1c9 c1ca c1cb c2d7 c1ca c1cb c1ca  ................
+00003020: ffff d9ff ce00 c1d7 c500 d7ff ffff ffff  ................
+00003030: d0ff c1ca c1c9 c1d7 c1d8 c2d7 12c1 caff  ................
+00003040: fff9 ffc1 cac1 c9c1 d7c1 d8c2 d712 c1ca  ................
+00003050: ffff ffff c5ff ffff ffff d0ff c2c9 c1d7  ................
+00003060: c1d8 c2d7 10c1 c8ff fff9 ffc2 c9c1 d7c1  ................
+00003070: d8c2 d710 c1c8 ffff ffff c5ff ffff ffff  ................
+00003080: d0ff c2c7 c1d7 c1d8 c2d7 c1d8 c1c6 ffff  ................
+00003090: f9ff c2c7 c1d7 c1d8 c2d7 c1d8 c1c6 ffff  ................
+000030a0: ffff c5ff ffff ffff d0ff c8d7 ffff f9ff  ................
+000030b0: c8d7 ffff ffff c5ff ffff ffff d0ff c8d7  ................
+000030c0: ffff f9ff c8d7 ffff ffff c5ff ffff ffff  ................
+000030d0: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+000030e0: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+000030f0: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+00003100: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+00003110: dfff ffff ffff ffff ffff ffff ffff dfff  ................
+00003120: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00003130: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00003140: d0ff 00c2 c8c4 c900 c8ff cf00 c1c6 c400  ................
+00003150: ccff c2c6 cbc7 c2c6 c5c7 c1c6 c6c7 00d4  ................
+00003160: ffc4 00c1 c9cf 00cc ff00 c2c8 c4c9 00c8  ................
+00003170: ffcf 00c1 c6c4 00cc ffc2 c6cb c7c2 c6c5  ................
+00003180: c7c1 c6c6 c700 d4ff c400 c1c9 cf00 d7ff  ................
+00003190: ffff ffff d0ff c1c7 c1c9 c2ca c1cb c2ca  ................
+000031a0: c1c9 c8ff cd00 c1c6 c1c9 c2ca c1c9 c200  ................
+000031b0: ccff c2ca d6cb c1ca c1cb c1ca c1d8 d4ff  ................
+000031c0: c200 c4ca c1c9 cd00 ccff c1c7 c1c9 c2ca  ................
+000031d0: c1cb c2ca c1c9 c8ff cd00 c1c6 c1c9 c2ca  ................
+000031e0: c1c9 c200 ccff c2ca d6cb c1ca c1cb c1ca  ................
+000031f0: c1d8 d4ff c200 c4ca c1c9 cd00 d7ff ffff  ................
+00003200: ffff d0ff c1c7 c1c9 c1ca c1cb c1cc c1cb  ................
+00003210: c2ca c8ff cb00 c1c6 c1c9 c2ca c2cb c2ca  ................
+00003220: 00cc ffc1 cac1 cbc1 ccc3 cdc3 ccc3 cdc3  ................
+00003230: ccc1 cdc2 ccc1 cdc2 ccc3 cdc2 ccc1 cbc1  ................
+00003240: d8d4 ff00 c1ca c4cb c2ca c1c9 cb00 ccff  ................
+00003250: c1c7 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+00003260: cb00 c1c6 c1c9 c2ca c2cb c2ca 00cc ffc1  ................
+00003270: cac1 cbc1 ccc3 cdc3 ccc3 cdc3 ccc1 cdc2  ................
+00003280: ccc1 cdc2 ccc3 cdc2 ccc1 cbc1 d8d4 ff00  ................
+00003290: c1ca c4cb c2ca c1c9 cb00 d7ff ffff ffff  ................
+000032a0: d0ff c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca  ................
+000032b0: c1c9 c8ff c900 c1c7 c1c9 c2ca c2cb c3cc  ................
+000032c0: c1cb c1ca ccff c1ca c3cb c1ca d5cb c1ca  ................
+000032d0: 88d4 ffc2 c9c2 cac4 cbc2 cac1 c9c9 00cc  ................
+000032e0: ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc1 cac1  ................
+000032f0: c9c8 ffc9 00c1 c7c1 c9c2 cac2 cbc3 ccc1  ................
+00003300: cbc1 cacc ffc1 cac3 cbc1 cad5 cbc1 ca88  ................
+00003310: d4ff c2c9 c2ca c4cb c2ca c1c9 c900 d7ff  ................
+00003320: ffff ffff d0ff c1c6 c1c9 c1ca c1cb c1cc  ................
+00003330: c1cb c2ca c8ff c700 c1c7 c1c9 c2ca c2cb  ................
+00003340: c2cc c1cd c1cc c2cb c1ca ccff c5cc c1cb  ................
+00003350: c1cc c3cb c1cc c5ca c1cc c8cb c2cc 20d4  .............. .
+00003360: ff13 c3c9 c2ca c4cb c2ca c1c9 c700 ccff  ................
+00003370: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+00003380: c700 c1c7 c1c9 c2ca c2cb c2cc c1cd c1cc  ................
+00003390: c2cb c1ca ccff c5cc c1cb c1cc c3cb c1cc  ................
+000033a0: c5ca c1cc c8cb c2cc 20d4 ff13 c3c9 c2ca  ........ .......
+000033b0: c4cb c2ca c1c9 c700 d7ff ffff ffff d0ff  ................
+000033c0: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
+000033d0: c8ff c500 c1c6 c1c9 c2ca c2cb c2cc c1cd  ................
+000033e0: c2cc c1cb c1ca 0f15 ccff c30f c20e c20d  ................
+000033f0: 17c2 0c0a c50c 0bc3 0cc2 0dc2 0ec3 0f21  ...............!
+00003400: d4ff c2f5 13c3 c9c2 cac4 cbc2 cac1 c9c5  ................
+00003410: 00cc ffc1 c6c1 c9c1 cac1 cbc1 ccc1 cbc1  ................
+00003420: cac1 c9c8 ffc5 00c1 c6c1 c9c2 cac2 cbc2  ................
+00003430: ccc1 cdc2 ccc1 cbc1 ca0f 15cc ffc3 0fc2  ................
+00003440: 0ec2 0d17 c20c 0ac5 0c0b c30c c20d c20e  ................
+00003450: c30f 21d4 ffc2 f513 c3c9 c2ca c4cb c2ca  ..!.............
+00003460: c1c9 c500 d7ff ffff ffff d0ff c1c6 c1c9  ................
+00003470: c1ca c1cb c1cc c1cb c2ca c8ff c300 c1c6  ................
+00003480: c1c9 c2ca c2cb c2cc c1cd c2cc c1cb c1ca  ................
+00003490: c30f 15cc ff0f c20e c20d 17c4 0cc1 f5c5  ................
+000034a0: 0cc1 f5c5 0cc2 0dc3 0e20 d4ff c228 c1f5  ......... ...(..
+000034b0: 2813 c3c9 c2ca c4cb c2ca c1c9 c300 ccff  (...............
+000034c0: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+000034d0: c300 c1c6 c1c9 c2ca c2cb c2cc c1cd c2cc  ................
+000034e0: c1cb c1ca c30f 15cc ff0f c20e c20d 17c4  ................
+000034f0: 0cc1 f5c5 0cc1 f5c5 0cc2 0dc3 0e20 d4ff  ............. ..
+00003500: c228 c1f5 2813 c3c9 c2ca c4cb c2ca c1c9  .(..(...........
+00003510: c300 d7ff cdff c8d7 ccff c3d7 cdff c4d7  ................
+00003520: c3ff c4d7 c7ff c2d7 c1ff c3d7 c7ff c3d7  ................
+00003530: c1ff c1d7 f9ff c1c6 c1c9 c1ca c1cb c1cc  ................
+00003540: c1cb c1ca c1c9 c8ff 00c1 c6c1 c9c2 cac2  ................
+00003550: cbc2 ccc1 cdc2 ccc1 cbc1 ca0d 0f0e c20d  ................
+00003560: 28cc ffc4 0bc2 0a0b 0ac2 0b21 c50a 21c4  (..........!..!.
+00003570: 0a0b 0ac4 0b88 d4ff 58c2 21c3 2812 c1c8  ........X.!.(...
+00003580: c2c9 c3ca c3cb c1ca c2c9 00cc ffc1 c6c1  ................
+00003590: c9c1 cac1 cbc1 ccc1 cbc1 cac1 c9c8 ff00  ................
+000035a0: c1c6 c1c9 c2ca c2cb c2cc c1cd c2cc c1cb  ................
+000035b0: c1ca 0d0f 0ec2 0d28 ccff c40b c20a 0b0a  .......(........
+000035c0: c20b 21c5 0a21 c40a 0b0a c40b 88d4 ff58  ..!..!.........X
+000035d0: c221 c328 12c1 c8c2 c9c3 cac3 cbc1 cac2  .!.(............
+000035e0: c900 d7ff cdff c1d7 c2ff c2d7 c2ff c1d7  ................
+000035f0: cdff c2d7 ceff c3d7 c3ff c3d7 c8ff c2d7  ................
+00003600: c2ff c2d7 c6ff c2d7 c2ff c2d7 f9ff c1c6  ................
+00003610: c1c9 c1ca c1cb c1cc c1cb c2ca c8ff c2c7  ................
+00003620: c1c8 c2ca c1cb c1cc c1cd c2cc c1cb c1ca  ................
+00003630: 0e0f 0b0d 0c0a 21c1 d7cc ff28 21c4 f515  ......!....(!...
+00003640: c1f5 c215 20c5 2820 c4f5 15c1 f5c2 1521  .... .( .......!
+00003650: 2888 d4ff c1d7 5820 c321 c228 12c4 c9c2  (.....X .!.(....
+00003660: cac2 c9c3 cacc ffc1 c6c1 c9c1 cac1 cbc1  ................
+00003670: ccc1 cbc2 cac8 ffc2 c7c1 c8c2 cac1 cbc1  ................
+00003680: ccc1 cdc2 ccc1 cbc1 ca0e 0f0b 0d0c 0a21  ...............!
+00003690: c1d7 ccff 2821 c4f5 15c1 f5c2 1520 c528  ....(!....... .(
+000036a0: 20c4 f515 c1f5 c215 2128 88d4 ffc1 d758   .......!(.....X
+000036b0: 20c3 21c2 2812 c4c9 c2ca c2c9 c3ca d7ff   .!.(...........
+000036c0: d0ff c2d7 d0ff c2d7 ceff c3d7 c3ff c3d7  ................
+000036d0: ccff c2d7 c5ff c2d7 c4ff c1d7 f9ff c1c6  ................
+000036e0: c1c9 c1ca c1cb c1cc c1cb c1ca c1c9 c8ff  ................
+000036f0: c210 c1d8 c2c8 c2cb c1cc c1cb c1ca c30e  ................
+00003700: 0cc1 f50a 216a c200 ccff c1d8 c1d7 c258  ....!j.........X
+00003710: d420 58c1 d7c1 d86a d4ff c200 c1d7 5820  . X....j......X 
+00003720: 6a21 2821 2813 c1c9 c1c8 c2c9 c1ca c2d8  j!(!(...........
+00003730: c2ca ccff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
+00003740: c1ca c1c9 c8ff c210 c1d8 c2c8 c2cb c1cc  ................
+00003750: c1cb c1ca c30e 0cc1 f50a 216a c200 ccff  ..........!j....
+00003760: c1d8 c1d7 c258 d420 58c1 d7c1 d86a d4ff  .....X. X....j..
+00003770: c200 c1d7 5820 6a21 2821 2813 c1c9 c1c8  ....X j!(!(.....
+00003780: c2c9 c1ca c2d8 c2ca d7ff d0ff c2d7 c3ff  ................
+00003790: c3d7 c1ff c2d7 c1ff c3d7 c1ff c6d7 c3ff  ................
+000037a0: c3d7 c6ff c1d7 c1ff c2d7 c1ff c1d7 c1ff  ................
+000037b0: c2d7 c2ff c3d7 c2ff c3d7 c2ff c2d7 c5ff  ................
+000037c0: c2d7 c7ff c3d7 c2ff c3d7 c1ff c2d7 ecff  ................
+000037d0: c1c6 c1c9 c1ca c1cb c1cc c1cb c2ca c8ff  ................
+000037e0: 10c2 d7c1 d8c2 c9c1 cbc1 cac2 0f0e 0b0a  ................
+000037f0: c1f5 206a c400 fcff c400 c1d7 886a c220  .. j.........j. 
+00003800: 28c2 f513 c2c9 c1ca 10c2 d8c1 c8cc ffc1  (...............
+00003810: c6c1 c9c1 cac1 cbc1 ccc1 cbc2 cac8 ff10  ................
+00003820: c2d7 c1d8 c2c9 c1cb c1ca c20f 0e0b 0ac1  ................
+00003830: f520 6ac4 00fc ffc4 00c1 d788 6ac2 2028  . j.........j. (
+00003840: c2f5 13c2 c9c1 ca10 c2d8 c1c8 d7ff d0ff  ................
+00003850: c2d7 c4ff c2d7 c1ff c2d7 c2ff c3d7 c1ff  ................
+00003860: c3d7 c1ff c2d7 c1ff c2d7 c1ff c2d7 c5ff  ................
+00003870: c1d7 c1ff c2d7 c1ff c1d7 c1ff c2d7 c1ff  ................
+00003880: c2d7 c1ff c2d7 c2ff c2d7 c2ff c2d7 c5ff  ................
+00003890: c2d7 c6ff c2d7 c1ff c2d7 c2ff c3d7 c1ff  ................
+000038a0: c1d7 ecff c1c6 c1c9 c1ca c1cb c1cc c1cb  ................
+000038b0: c1ca c1c9 c8ff c1d8 c3d7 10c1 c7c2 0f0e  ................
+000038c0: 0d17 2820 6ac6 00fc ffc6 00c1 d788 6ac2  ..( j.........j.
+000038d0: 2128 c2f5 c1ca c1c9 c2d8 c1d7 c1d8 ccff  !(..............
+000038e0: c1c6 c1c9 c1ca c1cb c1cc c1cb c1ca c1c9  ................
+000038f0: c8ff c1d8 c3d7 10c1 c7c2 0f0e 0d17 2820  ..............( 
+00003900: 6ac6 00fc ffc6 00c1 d788 6ac2 2128 c2f5  j.........j.!(..
+00003910: c1ca c1c9 c2d8 c1d7 c1d8 d7ff d0ff c2d7  ................
+00003920: c4ff c2d7 c1ff c2d7 c2ff c2d7 c3ff c2d7  ................
+00003930: c1ff c2d7 c1ff c2d7 c1ff c2d7 c5ff c1d7  ................
+00003940: c1ff c2d7 c1ff c1d7 c1ff c2d7 c4ff c2d7  ................
+00003950: c2ff c2d7 c2ff c2d7 c5ff c2d7 c9ff c2d7  ................
+00003960: c2ff c2d7 efff c1c6 c1c9 c1ca c1cb c1cc  ................
+00003970: c1cb c2ca c8ff c4d7 c1d8 100f 0d0c 0a21  ...............!
+00003980: 6ac8 00fc ffc8 00c1 d758 2021 28c1 f5c1  j........X !(...
+00003990: ca10 c1d8 c3d7 ccff c1c6 c1c9 c1ca c1cb  ................
+000039a0: c1cc c1cb c2ca c8ff c4d7 c1d8 100f 0d0c  ................
+000039b0: 0a21 6ac8 00fc ffc8 00c1 d758 2021 28c1  .!j........X !(.
+000039c0: f5c1 ca10 c1d8 c3d7 d7ff d0ff c2d7 c4ff  ................
+000039d0: c2d7 c1ff c2d7 c2ff c2d7 c3ff c2d7 c1ff  ................
+000039e0: c2d7 c1ff c2d7 c1ff c2d7 c5ff c1d7 c2ff  ................
+000039f0: c2d7 c2ff c2d7 c2ff c4d7 c2ff c2d7 c2ff  ................
+00003a00: c2d7 c5ff c2d7 c7ff c4d7 c2ff c2d7 efff  ................
+00003a10: c1c7 c2c8 c2ca c2c9 c1ca c8ff c200 c3d7  ................
+00003a20: c1c6 0c0a 2120 ca00 fcff ca00 c1d7 5820  ....! ........X 
+00003a30: 2110 c1c6 c3d7 00cc ffc1 c7c2 c8c2 cac2  !...............
+00003a40: c9c1 cac8 ffc2 00c3 d7c1 c60c 0a21 20ca  .............! .
+00003a50: 00fc ffca 00c1 d758 2021 10c1 c6c3 d700  .......X !......
+00003a60: d7ff d0ff c2d7 c4ff c2d7 c1ff c2d7 c2ff  ................
+00003a70: c2d7 c3ff c2d7 c1ff c2d7 c1ff c2d7 c1ff  ................
+00003a80: c2d7 c5ff c1d7 c2ff c2d7 c2ff c2d7 c1ff  ................
+00003a90: c2d7 c1ff c2d7 c2ff c2d7 c2ff c2d7 c6ff  ................
+00003aa0: c2d7 c3ff c1d7 c1ff c2d7 c1ff c2d7 c2ff  ................
+00003ab0: c2d7 efff c1c8 c2c9 c2ca c1cb c1ca c1c9  ................
+00003ac0: c8ff c400 c2d7 88c1 d7cc 00fc ffcc 00c1  ................
+00003ad0: d7c2 d8c2 d7c3 00cc ffc1 c8c2 c9c2 cac1  ................
+00003ae0: cbc1 cac1 c9c8 ffc4 00c2 d788 c1d7 cc00  ................
+00003af0: fcff cc00 c1d7 c2d8 c2d7 c300 d7ff cfff  ................
+00003b00: c4d7 c4ff c9d7 c2ff c1d7 c1ff c2d7 c3ff  ................
+00003b10: c3d7 c5ff c3d7 c1ff c2d7 c1ff c4d7 c1ff  ................
+00003b20: cdd7 c6ff c4d7 c3ff c9d7 eeff c1c9 c1ca  ................
+00003b30: c1cb c2d7 c1ca c1cb c1ca ffff d9ff ce00  ................
+00003b40: c1d7 c500 ccff c1c9 c1ca c1cb c2d7 c1ca  ................
+00003b50: c1cb c1ca ffff d9ff ce00 c1d7 c500 d7ff  ................
+00003b60: ffff ffff d0ff c1ca c1c9 c1d7 c1d8 c2d7  ................
+00003b70: 12c1 caff fff9 ffc1 cac1 c9c1 d7c1 d8c2  ................
+00003b80: d712 c1ca ffff ffff c5ff ffff ffff d0ff  ................
+00003b90: c2c9 c1d7 c1d8 c2d7 10c1 c8ff fff9 ffc2  ................
+00003ba0: c9c1 d7c1 d8c2 d710 c1c8 ffff ffff c5ff  ................
+00003bb0: ffff ffff d0ff c2c7 c1d7 c1d8 c2d7 c1d8  ................
+00003bc0: c1c6 ffff f9ff c2c7 c1d7 c1d8 c2d7 c1d8  ................
+00003bd0: c1c6 ffff ffff c5ff ffff ffff d0ff c8d7  ................
+00003be0: ffff f9ff c8d7 ffff ffff c5ff ffff ffff  ................
+00003bf0: d0ff c8d7 ffff f9ff c8d7 ffff ffff c5ff  ................
+00003c00: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00003c10: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00003c20: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+00003c30: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+00003c40: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+00003c50: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+00003c60: dfff ffff ffff ffff ffff ffff ffff dfff  ................
+00003c70: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00003c80: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00003c90: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+00003ca0: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+00003cb0: ffff ffff dfff ffff ffff ffff ffff ffff  ................
+00003cc0: ffff dfff ffff ffff ffff ffff ffff ffff  ................
+00003cd0: dfff ffff ffff ffff ffff ffff ffff dfff  ................
+00003ce0: ffff ffff ffff ffff ffff ffff dfff ffff  ................
+00003cf0: ffff ffff ffff ffff ffff dfff ffff ffff  ................
+00003d00: ffff ffff ffff ffff dfff ffff ffff ffff  ................
+00003d10: ffff ffff ffff dfff ffff ffff ffff ffff  ................
+00003d20: ffff ffff dfff 0c00 00ff ee00 eeef 00ef  ................
+00003d30: f000 f0f1 00f1 f200 f2f3 00f3 f400 f4f5  ................
+00003d40: 00f5 f600 f6a8 a8a8 b8b8 b8c8 c8c8 d8d8  ................
+00003d50: d8e8 e8e8 fcfc fc34 3c48 444c 5c58 6070  .......4<HDL\X`p
+00003d60: 6c74 8484 8c98 9ca0 acb0 b8c4 ccd0 dc30  lt.............0
+00003d70: 2c04 403c 0c50 4c14 605c 1c78 7840 9494  ,.@<.PL.`\.xx@..
+00003d80: 64b0 b084 cccc a864 6464 7474 7468 502c  d......dddttthP,
+00003d90: 7c68 4898 845c b8a0 78d4 bc94 f4dc b084  |hH..\..x.......
+00003da0: 8484 5804 1070 1020 8820 34a0 384c bc54  ..X..p. . 4.8L.T
+00003db0: 6ccc 687c dc84 90ec 9ca4 fcbc c0fc d000  l.h|............
+00003dc0: fce8 3cfc fc80 4c28 0060 3c08 7458 1c88  ..<...L(.`<.tX..
+00003dd0: 7438 9c88 50b0 9c6c c4b4 8844 1800 602c  t8..P..l...D..`,
+00003de0: 0480 4408 9c60 10b8 7818 d49c 20e8 b810  ..D..`..x... ...
+00003df0: fcd4 00fc f880 fcfc c020 0400 4014 0854  ......... ..@..T
+00003e00: 1c10 6c2c 1c80 3828 9448 38a8 5c4c b86c  ..l,..8(.H8.\L.l
+00003e10: 58c4 806c d494 8008 3400 1040 0020 5004  X..l....4..@. P.
+00003e20: 3060 0440 700c 5484 1468 941c 80a8 2c40  0`.@p.T..h....,@
+00003e30: 4040 2c44 203c 5830 5068 3c68 7c4c 8094  @@,D <X0Ph<h|L..
+00003e40: 5c98 b06c b4cc 7c10 3418 2048 2c38 6048  \..l..|.4. H,8`H
+00003e50: 4c74 5860 886c 78a4 8898 c0a8 b8dc c820  LtX`.lx........ 
+00003e60: 1800 381c 0050 5050 5834 0c68 4018 7c54  ..8..PPPX4.h@.|T
+00003e70: 2c8c 6c40 a080 584c 2810 6034 1874 4428  ,.l@..XL(.`4.tD(
+00003e80: 8854 38a4 6040 b870 50cc 8060 d494 70e0  .T8.`@.pP..`..p.
+00003e90: a880 ecbc 9450 1c04 6428 1478 3828 8c4c  .....P..d(.x8(.L
+00003ea0: 40a0 6460 b888 8824 2844 3034 5440 4064  @.d`...$(D04T@@d
+00003eb0: 5050 7464 6488 8484 a4ac acc0 d4d4 e030  PPtdd..........0
+00003ec0: 3030 402c 9058 40ac 684c c478 58e0 8c68  00@,.X@.hL.xX..h
+00003ed0: fca0 88fc bca8 fc00 186c 0024 8400 34a0  .........l.$..4.
+00003ee0: 0048 b800 60d4 1878 dc38 90e8 58a8 f080  .H..`..x.8..X...
+00003ef0: c4fc bce0 fc10 4060 1850 6c28 6078 3470  ......@`.Pl(`x4p
+00003f00: 8450 8ca0 74ac c09c ccdc ccf0 fcac 3434  .P..t.........44
+00003f10: d434 34fc 3434 fc64 58fc 907c fcb8 a0fc  .44.44.dX..|....
+00003f20: d8c8 fcf4 ec48 1470 5c2c 8c70 44a8 8c64  .....H.p\,.pD..d
+00003f30: c4a8 88e0 c8b0 f8d0 b8ff e8d0 fc3c 0000  .............<..
+00003f40: 5c00 0080 0000 a000 00c4 0000 e000 00fc  \...............
+00003f50: 0000 fc50 00fc 6c00 fc88 00fc a400 fcc0  ...P..l.........
+00003f60: 00fc dc00 fcfc 00cc 8808 e490 04fc 9c00  ................
+00003f70: fcb0 30fc c464 fcd8 9808 1858 0c24 6814  ..0..d.....X.$h.
+00003f80: 347c 1c44 8c28 5ca4 3878 bc48 98d8 64ac  4|.D.(\.8x.H..d.
+00003f90: e05c 9c34 6cb0 407c c84c 90e0 5ce0 f4fc  .\.4l.@|.L..\...
+00003fa0: c8ec f8b4 dcec 84bc d858 98ac 1010 1020  .........X..... 
+00003fb0: 2020 2044 7024 4874 284c 782c 507c 3054     Dp$Ht(Lx,P|0T
+00003fc0: 8048 6490 6484 a8d8 f4fc 6080 a444 608c  .Hd.d.....`..D`.
+00003fd0: 4c18 086c 2c18 9048 34b0 6c54 d292 7efc  L..l,..H4.lT..~.
+00003fe0: 3c00 fc54 00fc 6800 fc7c 00fc 9400 fcac  <..T..h..|......
+00003ff0: 00fc c400 4000 00ff 0000 3030 0040 4000  ....@.....00.@@.
+00004000: 5050 00ff ff00 9494 94f7 00f7 f800 f8f9  PP..............
+00004010: 00f9 fa00 fafb 00fb fc00 fcfd 00fd fe00  ................
+00004020: feff 00ff ffff ff                        .......
```

### Comparing `nml-0.7.2/regression/temperate_railwagons.png` & `nml-r1512/regression/temperate_railwagons.png`

 * *Files identical despite different names*

### Comparing `nml-0.7.2/regression/tram_foster_express.png` & `nml-r1512/regression/tram_foster_express.png`

 * *Files identical despite different names*

