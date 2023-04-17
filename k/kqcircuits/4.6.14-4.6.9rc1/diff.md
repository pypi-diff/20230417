# Comparing `tmp/kqcircuits-4.6.14.tar.gz` & `tmp/kqcircuits-4.6.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kqcircuits-4.6.14.tar", last modified: Mon Apr 17 07:09:33 2023, max compression
+gzip compressed data, was "kqcircuits-4.6.9rc1.tar", last modified: Tue Mar  7 09:28:44 2023, max compression
```

## Comparing `kqcircuits-4.6.14.tar` & `kqcircuits-4.6.9rc1.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.250589 kqcircuits-4.6.14/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/console_scripts/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/kqcircuits/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/kqcircuits/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.254589 kqcircuits-4.6.14/kqcircuits/chips/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/airbridge_crossings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/airbridge_dc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29434 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/crossing_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/daisy_woven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/dc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/demo_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/junction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/junction_test2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/lithography_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/lithography_test_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/quality_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/quality_factor_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/sample_holder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/single_xmons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/stripes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/tsv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/chips/xmons_direct_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/airbridge_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/airbridges/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/airbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge_multi_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/chip_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/circular_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/daisy_woven.oas
--rw-r--r--   0 runner    (1001) docker     (123)    28708 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/finger_capacitor_square.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/finger_capacitor_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/fluxlines/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/fluxlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline_straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/launcher_dc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/markers/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/markers/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/markers/marker_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/mask_marker_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/meander.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/smooth_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26823 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/spiral_resonator_polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/elements/tsvs/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/tsvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    41784 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_curved.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/junctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/junction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/manhattan_single_junction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/no_squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/junctions/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/klayout_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/layer_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/layer_config/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/layer_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/layer_config/default_layer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/layer_config/default_layer_props.lyp
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/layer_config/example_layer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.258589 kqcircuits-4.6.14/kqcircuits/masks/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/masks/mask_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/masks/mask_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/masks/mask_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/pya_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/qubits/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/qubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/qubits/double_pads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/qubits/double_pads_splines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/qubits/qubit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/qubits/swissmon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/airbridges_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/circular_capacitor_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/cross_section_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/double_pads_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/empty_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/export/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/export/ansys/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/ansys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/ansys/ansys_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/export/elmer/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/elmer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/elmer/elmer_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/export_and_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/simulation_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/sonnet_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/template.son
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.262589 kqcircuits-4.6.14/kqcircuits/simulations/export/xsection/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/xsection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/export/xsection/xsection_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/finger_capacitor_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/flip_chip_connector_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    46731 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/single_xmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/single_xmons_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/waveguides_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/simulations/xmons_direct_coupling_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/kqcircuits/test_structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/airbridge_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/cross_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/stripes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/test_structures/tsv_test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/kqcircuits/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/count_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/coupler_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/deep_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/edit_node_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/export_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/geometry_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/geometry_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/groundgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/gui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/import_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/layout_to_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/library_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/log_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/netlist_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/netlist_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/plugin_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/refpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/replace_squids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/kqcircuits/util/symmetric_polygons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:09:33.250589 kqcircuits-4.6.14/kqcircuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 07:09:33.000000 kqcircuits-4.6.14/kqcircuits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:09:33.266589 kqcircuits-4.6.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-17 07:09:18.000000 kqcircuits-4.6.14/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      206 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      528 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)       96 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.364674 kqcircuits-4.6.9rc1/console_scripts/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/console_scripts/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2819 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/console_scripts/run.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1347 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       64 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/_static_version.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6540 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/_version.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.372674 kqcircuits-4.6.9rc1/kqcircuits/chips/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1448 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6212 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_crossings.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3481 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_dc_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29396 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/chip.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6954 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/crossing_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3976 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/daisy_woven.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1216 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/dc_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11053 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/demo.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9794 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/demo_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2114 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/empty.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3381 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5588 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test2.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1535 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/launchers.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6092 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4930 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10434 2023-02-27 12:33:15.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12878 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/sample_holder_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16609 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/shaping.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3462 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/simple.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18962 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/single_xmons.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5103 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/stripes.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3527 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/tsv_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11979 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/xmons_direct_coupling.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10119 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/defaults.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.380674 kqcircuits-4.6.9rc1/kqcircuits/elements/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1921 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4504 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridge_connection.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.380674 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1238 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3723 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2932 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_multi_face.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2436 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_rectangular.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10793 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/chip_frame.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6556 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/circular_capacitor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3709 2023-01-25 07:43:18.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/daisy_woven.oas
+-rw-rw-r--   0 dave      (1000) dave      (1000)    28708 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/element.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9307 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_square.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5183 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_taper.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.384674 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1154 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2617 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1375 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6647 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.384674 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1167 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3424 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2805 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_straight.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3528 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/launcher.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2149 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/launcher_dc.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1124 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4691 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1302 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5221 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/mask_marker_fc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9555 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/meander.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9970 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/smooth_capacitor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    26823 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/spiral_resonator_polygon.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1134 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1751 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2729 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_ellipse.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1663 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    38661 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_composite.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12973 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6696 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_curved.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7614 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_splitter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2657 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_straight.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3661 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_taper.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/junctions/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1504 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2695 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/junction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13878 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8937 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan_single_junction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1653 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/no_squid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3131 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1660 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/squid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    19990 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/klayout_view.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1845 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_cluster.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.392674 kqcircuits-4.6.9rc1/kqcircuits/layer_config/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12093 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_config.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    35168 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5157 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/example_layer_config.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.396674 kqcircuits-4.6.9rc1/kqcircuits/masks/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1543 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17237 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    22122 2023-03-03 12:22:03.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_layout.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21747 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_set.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3012 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/pya_resolver.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.400674 kqcircuits-4.6.9rc1/kqcircuits/qubits/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1219 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10373 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5784 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads_splines.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5535 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/qubit.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8489 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/swissmon.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1270 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2122 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/airbridges_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1815 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/circular_capacitor_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6786 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/cross_section_simulation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3231 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/double_pads_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1170 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/empty_simulation.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1220 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18084 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/ansys_export.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9050 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/cross_section_elmer_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15549 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/elmer_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2735 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/export_and_run.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3291 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/simulation_export.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1092 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6954 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9707 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/sonnet_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1173 2023-01-25 07:43:18.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/template.son
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4332 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/util.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    22849 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/xsection_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1933 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/finger_capacitor_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2141 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/flip_chip_connector_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5226 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/port.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    46731 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/simulation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2629 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmon.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3914 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmons_full_chip_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4333 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/waveguides_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11433 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5213 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_sim.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/test_structures/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1248 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6820 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/airbridge_dc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3086 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/cross_test.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1157 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11388 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1613 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2651 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/stripes_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6489 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/test_structure.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2719 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/tsv_test_pattern.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/util/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1108 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3227 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/area.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2099 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/count_instances.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3141 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/coupler_lib.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1256 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/deep_delete.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2766 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/dependencies.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7786 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/edit_node_plugin.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8451 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/util/export_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15818 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/geometry_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1960 2023-02-15 17:44:05.000000 kqcircuits-4.6.9rc1/kqcircuits/util/geometry_json_encoder.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3261 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/groundgrid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8992 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/gui_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1579 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/import_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3995 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/label.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    19976 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/layout_to_code.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14347 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/util/library_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2708 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/log_router.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4700 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/util/merge.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13273 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/netlist_extraction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5443 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/netlist_graph.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10538 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/parameter_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6705 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/parameters.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1560 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/plugin_startup.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3615 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/refpoints.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9090 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/replace_squids.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2244 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/symmetric_polygons.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.364674 kqcircuits-4.6.9rc1/kqcircuits.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      528 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6424 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       48 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      344 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       27 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3038 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/setup.py
```

### Comparing `kqcircuits-4.6.14/console_scripts/__init__.py` & `kqcircuits-4.6.9rc1/console_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/console_scripts/run.py` & `kqcircuits-4.6.9rc1/console_scripts/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,62 +13,43 @@
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 import argparse
 import logging
 import sys
-import subprocess
 from pathlib import Path
 from kqcircuits.simulations.export.export_and_run import export_and_run
-from kqcircuits.defaults import TMP_PATH, SCRIPTS_PATH
+from kqcircuits.defaults import TMP_PATH, SIM_SCRIPT_PATH
 
 logging.basicConfig(level=logging.WARN, stream=sys.stdout)
 
+
 def run():
     parser = argparse.ArgumentParser(description='KQC console scripts')
 
     subparser = parser.add_subparsers(dest="command")
 
     simulate_parser = subparser.add_parser('simulate', help='KQC simulation \
             export and run script. Run and export with a single command!')
-    mask_parser = subparser.add_parser('mask', help='Build KQC Mask.')
 
     simulate_parser.add_argument('export_script', type=str, help='Name of the export script')
     simulate_parser.add_argument('--export-path-basename', type=str, default=None,
                                  help='The export folder will be `TMP_PATH / Path(export_path_basename)`, \
                                        if not given, then it will be `TMP_PATH / Path(args.export_script).stem`')
     simulate_parser.add_argument('-q', '--quiet', action="store_true", help='Quiet mode: No GUI')
 
-    mask_parser.add_argument('mask_script', type=str, help='Name of the mask script')
-    mask_parser.add_argument('-d', '--debug', action="store_true", help="Debug mode. Use a single process and "
-                             "print logs to standard output too.")
-    mask_parser.add_argument('-c N', action="store_true", help="Limit the number of used CPUs to 'N'")
-
     args, args_for_script = parser.parse_known_args()
 
     if args.command == "simulate":
         script_file = Path(args.export_script)
         if not script_file.is_file():
-            script_file = Path(SCRIPTS_PATH / "simulations" / args.export_script)
+            script_file = Path(SIM_SCRIPT_PATH / args.export_script)
             if not script_file.is_file():
-                logging.error(f"Export script not found at {args.export_script} or {script_file}")
+                logging.error(
+                        f"Export script not found at {args.export_script} or {SIM_SCRIPT_PATH / args.export_script}")
                 return
         if args.export_path_basename is not None:
             export_path = TMP_PATH / args.export_path_basename
         else:
             export_path = TMP_PATH / Path(args.export_script).stem
         export_and_run(script_file, export_path, args.quiet, args_for_script)
-    elif args.command == "mask":
-        script_file = Path(args.mask_script)
-        if not script_file.is_file():
-            script_file = Path(SCRIPTS_PATH / "masks" / args.mask_script)
-            if not script_file.is_file():
-                logging.error(f"Mask script not found at {args.mask_script} or {script_file}")
-                return
-        if args.debug:
-            subprocess.call([sys.executable, script_file, '-d'])
-        else:  # Windows needs this for multiprocessing
-            with open(script_file) as mask_file:
-                exec(mask_file.read())  # pylint: disable=exec-used
-    else:
-        parser.print_usage()
```

### Comparing `kqcircuits-4.6.14/kqcircuits/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/_version.py` & `kqcircuits-4.6.9rc1/kqcircuits/_version.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/airbridge_crossings.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_crossings.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/airbridge_dc_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/chip.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/chip.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from kqcircuits.util.groundgrid import make_grid
 from kqcircuits.elements.tsvs.tsv import Tsv
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_dc import FlipChipConnectorDc
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_rf import FlipChipConnectorRf
 
 
 @logged
-@add_parameters_from(Tsv, "tsv_type")
 @add_parameters_from(FlipChipConnectorRf, "connector_type")
 @add_parameter(ChipFrame, "box", hidden=True)
 @add_parameters_from(ChipFrame, "name_mask", "name_chip", "name_copy", "name_brand",
                      "dice_grid_margin", marker_types=[default_marker_type] * 8)
 class Chip(Element):
     """Base PCell declaration for chips.
 
@@ -268,15 +267,15 @@
                 frame_trans = pya.DTrans(0, 0)
             self.produce_frame(frame_parameters, frame_trans)
 
         if self.with_gnd_tsvs:
             self._produce_ground_tsvs(face_id=[0, 2])
         if self.with_face1_gnd_tsvs:
             tsv_box = self.get_box(1).enlarged(pya.DVector(-self.edge_from_tsv, -self.edge_from_tsv))
-            self._produce_ground_tsvs(face_id=[3, 1], tsv_box=tsv_box)
+            self._produce_ground_tsvs(face_id=[1, 3], tsv_box=tsv_box)
 
         if self.with_gnd_bumps:
             self._produce_ground_bumps()
 
     def get_box(self, face=0):
         """
         Get the chip frame box for the specified face, correctly resolving defaults.
```

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/crossing_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/crossing_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/daisy_woven.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/daisy_woven.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/dc_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/demo.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/demo.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/demo_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/demo_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/empty.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/empty.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/junction_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/junction_test2.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test2.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/launchers.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/launchers.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/lithography_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/lithography_test_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/quality_factor.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/quality_factor_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/sample_holder_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/sample_holder_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/shaping.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/shaping.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/simple.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/single_xmons.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/single_xmons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/stripes.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/stripes.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/tsv_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/tsv_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/chips/xmons_direct_coupling.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/xmons_direct_coupling.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/defaults.py` & `kqcircuits-4.6.9rc1/kqcircuits/defaults.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/airbridge_connection.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridge_connection.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/airbridges/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge_multi_face.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_multi_face.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/airbridges/airbridge_rectangular.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_rectangular.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/chip_frame.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/chip_frame.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/circular_capacitor.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/circular_capacitor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/daisy_woven.oas` & `kqcircuits-4.6.9rc1/kqcircuits/elements/daisy_woven.oas`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/element.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/element.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/finger_capacitor_square.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_square.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/finger_capacitor_taper.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_taper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/fluxlines/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/fluxlines/fluxline_straight.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_straight.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/launcher.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/launcher.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/launcher_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/launcher_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/markers/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/markers/marker.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/markers/marker_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/mask_marker_fc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/mask_marker_fc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/meander.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/meander.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/smooth_capacitor.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/smooth_capacitor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/spiral_resonator_polygon.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/spiral_resonator_polygon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/tsvs/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv_ellipse.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_ellipse.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,10 +57,8 @@
             pya.DPoint(numpy.abs(math.cos(a)) ** (2 / p1) * w * numpy.sign(math.cos(a)),
                        numpy.abs(math.sin(a)) ** (2 / p2) * r * numpy.sign(math.sin(a))) for
             a in (x / 32 * math.pi for x in range(0, 65))]
 
         shape = pya.DPolygon(tsv_pts_avoidance)
         # ground avoidance layer 1t1 face
         self.cell.shapes(self.get_layer("ground_grid_avoidance")).insert(shape)
-        self.cell.shapes(self.get_layer("ground_grid_avoidance", 1)).insert(shape)
-        self.cell.shapes(self.get_layer("through_silicon_via")).insert(pya.DPolygon(tsv_pts))
-        self.cell.shapes(self.get_layer("through_silicon_via", 1)).insert(pya.DPolygon(tsv_pts))
+        self.cell.shapes(self.get_layer("through_silicon_via")).insert(pya.DPolygon(tsv_pts))  # TSV only on 1t1 face
```

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/tsvs/tsv_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,12 +26,10 @@
 
     .. MARKERS_FOR_PNG 0,0
     """
 
     def build(self):
         tsv = circle_polygon(self.tsv_diameter / 2)
         self.cell.shapes(self.get_layer("through_silicon_via")).insert(tsv)
-        self.cell.shapes(self.get_layer("through_silicon_via", 1)).insert(tsv)
         margin = circle_polygon(self.tsv_diameter / 2 + self.margin)
         self.cell.shapes(self.get_layer("ground_grid_avoidance")).insert(margin)
-        self.cell.shapes(self.get_layer("ground_grid_avoidance", 1)).insert(margin)
         del self.refpoints['base']
```

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_composite.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_composite.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,79 +241,24 @@
 
         cell = super().create(layout, library, **parameters)
         setattr(cell, "segment_lengths", lambda: WaveguideComposite.get_segment_lengths(cell))
 
         return cell
 
     @staticmethod
-    def get_segment_cells(cell):
-        """Get the subcells of a ``WaveguideComposite`` cell, ordered by node index.
-
-        The subcells include ``WaveguideCoplanar``, ``WaveguideCoplanarTaper`` and ``Meander`` cells for straight,
-        tapered and meandering segments, respectively, and any element cells that were inserted explicitly
-        (``element`` argument) or implicitly (changing ``a``, ``b`` or ``face_id``) at any ``Node``.
-
-        The ``node_index`` returned with each subcell is an index to the ``nodes`` parameter of the
-        ``WaveguideComposite`` cell. It points to the node that _created_ the subcell, which is the node following a
-        segment for regular ``WaveguideCoplanar`` segments, and the node that specified the element or parameter change
-        otherwise.
-
-        Note that there may be multiple subcells per node, and some nodes may not have associated subcells (in
-        particular, regular ``WaveguideCoplanar`` segments are merged when possible). Subscells are returned in the
-        order in which they appear in the waveguide.
-
-        Args:
-            cell: A WaveguideComposite cell. Can be a PCell or static cell created from a PCell.
-
-        Returns: A list of tuples (node_index: int, subcell: pya.Cell) ordered by node_index.
-        """
-        layout = cell.layout()
-
-        segment_data = []
-
-        for inst in cell.each_inst():
-            # Note: Using layout.cell(inst.cell_index) instead of inst.cell to work around KLayout issue #235
-            child_cell = layout.cell(inst.cell_index)
-
-            node_index = inst.property("waveguide_composite_node_index")
-            if node_index is not None:
-                segment_data.append((node_index, child_cell))
-
-        return list(sorted(reversed(segment_data), key=lambda x: x[0]))
-
-    @staticmethod
     def get_segment_lengths(cell):
-        """ Retrieves the segment lengths of each waveguide segment in a WaveguideComposite cell.
-
-        Waveguide segments are ``WaveguideCoplanar``, ``WaveguideCoplanarTaper`` and ``Meander`` subcells.
-        This method returns a list with the same length as the ``nodes`` parameter, where each element is the total
-        length of all waveguides directly preceding and/or defined in that node. For example, for a taper node both the
-        preceding regular waveguide and the taper itself are counted.
-
-        Note that ``WaveguideComposite`` merges consecutive waveguide segments if they have no special elements. As
-        a consequence, the corresponding waveguide lengths all accumulate in the next index which has a taper, meander
-        or other element, and the length for nodes that contain ony ``WaveguideCoplanar`` is reported as 0.
-
-        Args:
-            cell: A WaveguideComposite cell. Can be a PCell or static cell created from a PCell.
-
-        Returns: A list waveguide lengths per node
+        """ Retreives the segment lengths of each waveguide segment in a WaveguideComposite cell
         """
 
         # Measure segment lengths, counting only "regular waveguides"
-        waveguide_segment_types = {"Waveguide Coplanar", "Waveguide Coplanar Taper", "Meander"}
-
-        segment_data = WaveguideComposite.get_segment_cells(cell)
-        if len(segment_data) == 0:
-            return []
-
-        segment_lengths = [0] * (segment_data[-1][0] + 1)
-        for node_index, child_cell in segment_data:
-            if child_cell.name.split('$')[0] in waveguide_segment_types:
-                segment_lengths[node_index] += get_cell_path_length(child_cell)
+        layout = cell.layout()
+        # Note: Using layout.cell(inst.cell_index) instead of inst.cell to work around KLayout issue #235
+        child_cells = [layout.cell(inst.cell_index) for inst in cell.each_inst()]
+        segment_lengths = [get_cell_path_length(child_cell) for child_cell in child_cells
+                           if child_cell.name.split('$')[0] == "Waveguide Coplanar"]
 
         return segment_lengths
 
     @staticmethod
     def produce_fixed_length_waveguide(chip, route_function, initial_guess=0.0, length=0.0, **waveguide_params):
         """
         Produce a waveguide composite with fixed length. `route_function` should be a single-argument function that
@@ -568,16 +513,15 @@
         # Compute transformation for the cell
         waveguide_dir = self._node_entrance_direction(ind)
         trans = pya.DCplxTrans(1, get_angle(waveguide_dir) - get_angle(element_dir), False, self._nodes[ind].position)
         if ind in (0, len(self._nodes) - 1):
             trans *= pya.DTrans(-rel_ref[before if ind == 0 else after])
 
         # Insert element cell with computed transformation
-        cell_inst, ref = self.insert_cell(cell, trans)
-        cell_inst.set_property("waveguide_composite_node_index", ind)
+        _, ref = self.insert_cell(cell, trans)
         if inst_name is not None:
             for name, value in ref.items():
                 self._child_refpoints[f'{inst_name}_{name}'] = value
 
         # Add waveguide from previous element until this element
         self._add_waveguide(ind, ref[before], waveguide_dir)
 
@@ -603,16 +547,15 @@
             return
         params = {**self.pcell_params_by_name(WaveguideCoplanar), "path": points}
         if start_index != 0 or self._nodes[start_index].element:
             params['term1'] = 0
         if end_index != len(self._nodes) - 1 or self._nodes[end_index].element:
             params['term2'] = 0
         wg_cell = self.add_element(WaveguideCoplanar, **params)
-        cell_inst, _ = self.insert_cell(wg_cell)
-        cell_inst.set_property("waveguide_composite_node_index", end_index)
+        self.insert_cell(wg_cell)
 
     def _add_waveguide(self, end_index, end_pos=None, end_dir=None):
         """Creates waveguide from `self._wg_start_idx` until `end_index`.
 
         Args:
             end_index: the last node index taken into account in the waveguide
             end_pos: endpoint position of the waveguide (optional, overwrites `self._nodes[end_index].position`)
@@ -725,17 +668,16 @@
                     if n1 - 1 == start_index:
                         meander_len -= start_len + (points[0] - turn_start).length()
                     elif self._nodes[n1-1].angle is None:
                         meander_len -= start_len / 2
                     else:
                         meander_len -= start_len + (self._nodes[n1-1].position - turn_start).length()
 
-                cell_inst, _ = self.insert_cell(Meander, start=[meander_start.x, meander_start.y],
-                                                end=[meander_end.x, meander_end.y], length=meander_len, **node1.params)
-                cell_inst.set_property("waveguide_composite_node_index", end_index)
+                self.insert_cell(Meander, start=[meander_start.x, meander_start.y], end=[meander_end.x, meander_end.y],
+                                 length=meander_len, **node1.params)
                 wg_points = point0 + points[p0:p1] + ([] if start_len < 1e-4 else [meander_start])
                 self._insert_wg_cell(wg_points, n0, n1)
                 n0 = n1
                 p0 = p1
                 point0 = [] if end_len < 1e-4 else [meander_end]
             elif "n_bridges" in node1.params and node1.params["n_bridges"] > 0:
                 ab_len = node1.params['bridge_length'] if "bridge_length" in node1.params else None
```

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_curved.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_curved.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_splitter.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_splitter.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_straight.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_straight.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/elements/waveguide_coplanar_taper.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_taper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/junction.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/manhattan.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/manhattan_single_junction.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan_single_junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/no_squid.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/no_squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/junctions/squid.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/klayout_view.py` & `kqcircuits-4.6.9rc1/kqcircuits/klayout_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 
         if filename is None:
             filename = cell.name
         if layers_set is None:
             layers_set = [resolve_default_layer_info(layer_name) for layer_name in mask_bitmap_export_layers]
 
         if len(layers_set) == 1:
-            layer_str = "-" + layers_set[0].name
+            layer_str = " " + layers_set[0].name
         else:
             layer_str = ""
         cell_png_name = path / "{}{}.png".format(filename, layer_str)
 
         def export_callback():
             self.layout_view.save_image(str(cell_png_name), pngsize[0], pngsize[1])
```

### Comparing `kqcircuits-4.6.14/kqcircuits/layer_cluster.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_cluster.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/layer_config/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/layer_config/default_layer_config.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 # Top face layers
 _face_layers['2b1'] = {
     **_shift_layers(_common_b_t_layers, 0, 1),    # common layers at the "top"
 }
 
 # Ceiling face layers
 _face_layers['2t1'] = {
-    **_shift_layers(_common_b_t_layers, 128, 1),     # same common layers at the "ceiling"
+    **_shift_layers(_common_layers, 128, 1),     # same common layers at the "ceiling"
 }
 
 # Other auxiliary layers [Layer 220-229]
 _aux_layers_dict = {
     "annotations": (220, 0),
     "annotations_2": (221, 0),
     "instance_names": (222, 0),
@@ -135,23 +135,23 @@
 # default_faces[face_id] contains the face dictionary for the face determined by face_id.
 #
 # Each face dictionary should contain:
 #   - key "id" with value face_id (string)
 #   - for all the available layers in that face: key "Layer_name", value pya.LayerInfo object for that layer
 #
 default_faces = {}
-for f in ('1t1', '2b1', '1b1', '2t1'):
+for f in ('1b1', '1t1', '2b1', '2t1'):
     default_faces[f] = {n: pya.LayerInfo(i[0], i[1], f'{f}_{n}') for n, i in _face_layers[f].items()}
 
 # pya layer information
 default_layers = {n: pya.LayerInfo(i[0], i[1], n) for n, i in _aux_layers_dict.items()}
 for face, layers in default_faces.items():
     default_layers.update({f'{face}_{name}': li for name, li in layers.items()})
 
-for f in ('1t1', '2b1', '1b1', '2t1'):
+for f in ('1b1', '1t1', '2b1', '2t1'):
     default_faces[f]['id'] = f
 
 default_face_id = "1t1"  # face_id of the face that is used by default in some contexts
 
 # Layer names (without face prefix) for layers exported as individual .oas files during mask layout export.
 default_mask_export_layers = [
     "base_metal_gap",
@@ -203,27 +203,27 @@
 ]
 
 # Layer clusters used for exporting only certain layers together in the same file, when exporting individual chips
 # during mask layout export.
 # Dictionary with items "cluster name: LayerCluster".
 chip_export_layer_clusters = {
     # 1b1-face
-    "SIS-1b1": LayerCluster(["1b1_SIS_junction", "1b1_SIS_shadow", "1b1_SIS_junction_2"],
+    "SIS 1b1": LayerCluster(["1b1_SIS_junction", "1b1_SIS_shadow", "1b1_SIS_junction_2"],
                             ["1b1_base_metal_gap_for_EBL"], "1b1"),
-    "airbridges-1b1": LayerCluster(["1b1_airbridge_pads", "1b1_airbridge_flyover"],
+    "airbridges 1b1": LayerCluster(["1b1_airbridge_pads", "1b1_airbridge_flyover"],
                                    ["1b1_base_metal_gap_wo_grid"], "1b1"),
     # 1t1-face
-    "SIS-1t1": LayerCluster(["1t1_SIS_junction", "1t1_SIS_shadow", "1t1_SIS_junction_2"],
+    "SIS 1t1": LayerCluster(["1t1_SIS_junction", "1t1_SIS_shadow", "1t1_SIS_junction_2"],
                             ["1t1_base_metal_gap_for_EBL"], "1t1"),
-    "airbridges-1t1": LayerCluster(["1t1_airbridge_pads", "1t1_airbridge_flyover"],
+    "airbridges 1t1": LayerCluster(["1t1_airbridge_pads", "1t1_airbridge_flyover"],
                                    ["1t1_base_metal_gap_wo_grid"], "1t1"),
     # 2b1-face
-    "SIS-2b1": LayerCluster(["2b1_SIS_junction", "2b1_SIS_shadow", "2b1_SIS_junction_2"],
+    "SIS 2b1": LayerCluster(["2b1_SIS_junction", "2b1_SIS_shadow", "2b1_SIS_junction_2"],
                             ["2b1_base_metal_gap_for_EBL"], "2b1"),
-    "airbridges-2b1": LayerCluster(["2b1_airbridge_pads", "2b1_airbridge_flyover"],
+    "airbridges 2b1": LayerCluster(["2b1_airbridge_pads", "2b1_airbridge_flyover"],
                                    ["2b1_base_metal_gap_wo_grid"], "2b1"),
 }
 
 # default layers to use for calculating cell path lengths with get_cell_path_length()
 default_path_length_layers = [
     "1b1_waveguide_path",
     "1t1_waveguide_path",
```

### Comparing `kqcircuits-4.6.14/kqcircuits/layer_config/default_layer_props.lyp` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp`

 * *Files 8% similar despite different names*

#### Comparing `kqcircuits-4.6.14/kqcircuits/layer_config/default_layer_props.lyp` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp`

```diff
@@ -1015,235 +1015,14 @@
       <width>2</width>
       <marked>false</marked>
       <xfill>false</xfill>
       <animation>0</animation>
       <name/>
       <source>'2t1 ground grid avoidance' 133/2@1</source>
     </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 base metal gap for EBL' 134/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 waveguide path' 135/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS junction' 136/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS shadow' 137/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS junction 2' 139/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 airbridge pads' 146/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 airbridge flyover' 147/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 chip dicing' 158/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 underbump metallization' 148/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 indium bump' 149/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 through silicon via' 150/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 through silicon via avoidance' 153/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 ports' 154/2@1</source>
-    </group-members>
   </properties>
   <properties>
     <frame-color/>
     <fill-color/>
     <frame-brightness>0</frame-brightness>
     <fill-brightness>0</fill-brightness>
     <dither-pattern/>
```

### Comparing `kqcircuits-4.6.14/kqcircuits/layer_config/example_layer_config.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/example_layer_config.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/masks/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/masks/mask_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             # To transform the exported layer cluster chip correctly (e.g. mirroring for top chip),
             # an instance of the cell is inserted to a temporary cell with the correct transformation.
             # Was not able to get this working by just using static_cell.transform_into().
             temporary_cell = layout.create_cell(chip_name)
             temporary_cell.insert(pya.DCellInstArray(static_cell.cell_index(), default_mask_parameters[
                 layer_cluster.face_id]["chip_trans"]))
             layers_to_export = {name: layout.layer(default_layers[name]) for name in layer_cluster.all_layers()}
-            path = chip_dir / f"{chip_name}-{cluster_name}.gds"
+            path = chip_dir / "{} {}.gds".format(chip_name, cluster_name)
             _export_cell(path, temporary_cell, layers_to_export)
             temporary_cell.delete()
 
     # export drc report for the chip
     if export_drc:
         export_drc_report(chip_name, chip_dir)
 
@@ -171,15 +171,15 @@
         wafer = pya.Region(top_cell.begin_shapes_rec(layer)).merged()
         disc = pya.Region([circle_polygon(mask_layout.wafer_rad).to_itype(layout.dbu)])
         layout.copy_layer(layer, tmp_layer)
         layout.clear_layer(layer)
         top_cell.shapes(layer).insert(wafer ^ disc)
 
     layers_to_export = {layer_info.name: layer}
-    path = export_dir / (_get_mask_layout_full_name(mask_set, mask_layout) + f"-{layer_info.name}.oas")
+    path = export_dir / (_get_mask_layout_full_name(mask_set, mask_layout) + f" {layer_info.name}.oas")
     _export_cell(path, top_cell, layers_to_export)
 
     if invert:
         layout.clear_layer(layer)
         layout.copy_layer(tmp_layer, layer)
     layout.delete_layer(tmp_layer)
 
@@ -191,16 +191,16 @@
     with open(file_location, "w+", encoding="utf-8") as f:
         f.write("# Mask Set Name: {}\n".format(mask_set.name))
         f.write("Version: {}\n".format(mask_set.version))
 
         for mask_layout in mask_set.mask_layouts:
 
             f.write("## Mask Layout {}:\n".format(mask_layout.face_id + mask_layout.extra_id))
-            mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout)
-            f.write(f"![alt text]({mask_layout_str}/{mask_layout_str}-mask_graphical_rep.png)\n")
+            mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout).replace(" ", "%20")
+            f.write(f"![alt text]({mask_layout_str}/{mask_layout_str}%20mask_graphical_rep.png)\n")
 
             f.write("### Number of Chips in Mask Layout {}\n".format(mask_layout.face_id + mask_layout.extra_id))
 
             chip_counts = {}
 
             def count_chips(mlayout, counts):
 
@@ -292,21 +292,25 @@
         for mask_layout in mask_set.mask_layouts:
             mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout)
             mask_layout_path = mask_set._mask_set_dir / mask_layout_str
 
             f.write("### Mask Files:\n")
             for file_name in os.listdir(mask_layout_path):
                 if file_name.endswith(".oas"):
-                    f.write(" + [{}]({})\n".format(file_name, os.path.join(mask_layout_str, file_name)))
+                    # the spaces are replaced by "%20" to make links to filenames with spaces work
+                    f.write(" + [{}]({})\n".format(file_name,
+                                                   os.path.join(mask_layout_str, file_name).replace(" ", "%20")))
             f.write("\n")
 
             f.write("### Mask Images:\n")
             for file_name in os.listdir(mask_layout_path):
                 if file_name.endswith(".png"):
-                    f.write("+ [{}]({})\n".format(file_name, os.path.join(mask_layout_str, file_name)))
+                    # the spaces are replaced by "%20" to make links to filenames with spaces work
+                    f.write("+ [{}]({})\n".format(file_name,
+                                                  os.path.join(mask_layout_str, file_name).replace(" ", "%20")))
 
         f.close()
 
 
 @logged
 def export_bitmaps(mask_set, spec_layers=mask_bitmap_export_layers):
     """Exports bitmaps for the mask_set."""
@@ -383,8 +387,8 @@
 def _get_directory(directory):
     if not os.path.exists(str(directory)):
         os.mkdir(str(directory))
     return directory
 
 
 def _get_mask_layout_full_name(mask_set, mask_layout):
-    return f"{mask_set.name}_v{mask_set.version}-{mask_layout.face_id}{mask_layout.extra_id}"
+    return f"{mask_set.name}_v{mask_set.version} {mask_layout.face_id}{mask_layout.extra_id}"
```

### Comparing `kqcircuits-4.6.14/kqcircuits/masks/mask_layout.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.with_grid = with_grid
         self.face_id = face_id
         self.chips_map = chips_map
         self.chips_map_legend = None
 
         self.layers_to_mask = kwargs.get("layers_to_mask", default_layers_to_mask)
         self.covered_region_excluded_layers = kwargs.get("covered_region_excluded_layers",
-                                                        default_covered_region_excluded_layers) + ["mask_edge"]
+                                                        default_covered_region_excluded_layers)
         self.wafer_rad = kwargs.get("wafer_rad", default_mask_parameters[self.face_id]["wafer_rad"])
         self.wafer_center = (pya.DVector(0, 0))
         self.chips_map_offset = kwargs.get("chips_map_offset",
                                               default_mask_parameters[self.face_id]["chips_map_offset"])
         self.wafer_top_flat_length = kwargs.get("wafer_top_flat_length", 0)
         self.wafer_bottom_flat_length = kwargs.get("wafer_bottom_flat_length", 0)
         self.dice_width = kwargs.get("dice_width", default_mask_parameters[self.face_id]["dice_width"])
```

### Comparing `kqcircuits-4.6.14/kqcircuits/masks/mask_set.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,47 +13,46 @@
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 import copy
 import os
-import logging
-from sys import argv
+import subprocess
 from time import perf_counter
+from string import Template
 from inspect import isclass
-from multiprocessing import Pool
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
 from autologging import logged
 from tqdm import tqdm
 
-from kqcircuits.util.log_router import route_log
-from kqcircuits.pya_resolver import pya, is_standalone_session
-from kqcircuits.defaults import default_bar_format, TMP_PATH, default_face_id
+from kqcircuits.pya_resolver import pya, is_standalone_session, klayout_executable_command
+from kqcircuits.defaults import default_bar_format, TMP_PATH, STARTUPINFO, default_face_id
 from kqcircuits.masks.mask_export import export_chip, export_mask_set
 from kqcircuits.masks.mask_layout import MaskLayout
 from kqcircuits.klayout_view import KLayoutView
 
 
 @logged
 class MaskSet:
     """Class representing a set of masks for different chip faces.
 
     A mask set consists of one or more MaskLayouts, each of which is for a certain face.
 
     To create a mask, add mask layouts to the mask set using add_mask_layout() and add chips to these mask layouts using
-    add_chip(). These functions also export some files for each chip. Then call build() to create the
+    add_chips() or add_chip(). These functions also export some files for each chip. Then call build() to create the
     cell hierarchy of the entire mask, and finally export mask files by calling export().
 
     Example:
         mask = MaskSet(...)
         mask.add_mask_layout(...)
         mask.add_mask_layout(...)
-        mask.add_chip(...)
+        mask.add_chips(...)
         mask.build()
         mask.export()
 
     Attributes:
         layout: pya.Layout of this mask set
         name: Name of the mask set
         version: Version of the mask set
@@ -79,27 +78,20 @@
         self.version = version
         self.with_grid = with_grid
         self.export_drc = export_drc
         self.chips_map_legend = {}
         self.mask_layouts = []
         self.mask_export_layers = mask_export_layers if mask_export_layers is not None else []
         self.used_chips = {}
-        self._extra_params = {}
+        self.template_imports = []
+        self._thread_create_chip_parameters = {}
         self._mask_set_dir = Path(export_path)/f"{name}_v{version}"
 
         self._mask_set_dir.mkdir(parents=True, exist_ok=True)
 
-        self._extra_params["enable_debug"] = '-d' in argv
-        self._single_process = self._extra_params["enable_debug"] or not is_standalone_session()
-
-        self._cpu_override = 0
-        if '-c' in argv and len(argv) > argv.index('-c') + 1:
-            self._cpu_override = int(argv[argv.index('-c') + 1])
-
-
     def add_mask_layout(self, chips_map, face_id=default_face_id, mask_layout_type=MaskLayout, **kwargs):
         """Creates a mask layout from chips_map and adds it to self.mask_layouts.
 
         Args:
             chips_map: List of lists (2D-array) of strings, each string is a chip name (or --- for no chip)
             face_id: face_id of the mask layout
             mask_layout_type: type of the mask layout (MaskLayout or a child class of it)
@@ -112,101 +104,197 @@
             kwargs["mask_export_layers"] = self.mask_export_layers
 
         mask_layout = mask_layout_type(self.layout, self.name, self.version, self.with_grid, chips_map, face_id,
                                        **kwargs)
         self.mask_layouts.append(mask_layout)
         return mask_layout
 
-    def add_chip(self, chips, variant_name=None, cpus=None, **kwargs):
-        """Adds a chip (or list of chips) with parameters to self.chips_map_legend and exports the files for each chip.
+    def load_cell_from_file(self, file_name):
+        """Load GDS or OASIS cell from file.
+
+        Load a cell (usually a chip) from the specified file.
+
+        Args:
+            file_name: name of the file (with path) to be loaded
+
+        Returns:
+            the loaded cell
+        """
+        load_opts = pya.LoadLayoutOptions()
+        if hasattr(pya.LoadLayoutOptions, "CellConflictResolution"):
+            load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
+        self.layout.read(file_name, load_opts)
+        return self.layout.top_cells()[-1]
 
-        Note the complex polymorphism used here: ``chips`` is either a single chip class or a list of ``(chip, variant,
-        parameters)`` tuples. In the latter case the rest of the arguments (except ``cpus``) are ignored. Also,
-        ``chips`` (or the individual chip part of tuples) may be a simple file name to load a static .oas file instead.
-
-        Chips are created in parallel in separate processes but the user may choose to use a ``-d`` switch on
-        the command line for debugging with a single process. It is also possible to manually limit the number of
-        concurrently used CPUs for resource management purposes with the ``-c 4`` switch (to 4 in this example).
+    def add_chips(self, chips, threads=None):
+        """Adds a list of chips with parameters to self.chips_map_legend and exports the files for each chip.
 
         Args:
-            chip: A chip class. Or a list of tuples, like ``[(QualityFactor, "QDG", parameters),...]``,
-                  parameters are optional.
-            variant_name: Name for specific variant, the same as in the mask layout. Or None, if multiple
-                          chips are given
-            cpus: Number of parallel processes to use for chip generation. By default uses ``os.cpu_count()``
-                  or the number of chips, whichever is smaller.
-            **kwargs: Any parameters passed to the a single chip PCell. Not used with multiple chips.
+            chips: List of tuples that ``add_chip`` uses. Parameters are optional.
+                For example, ``(QualityFactor, "QDG", parameters)``.
+            threads: Number of parallel threads to use for generation. By default uses ``os.cpu_count()`` threads.
+                Uses subprocesses and consequently a lot of memory. In standalone python mode always uses 1 thread.
+
+        Warning:
+            It is advised to lower the thread number if your system has a lot of CPU cores but not a lot of memory.
+            The same applies for exporting large and complex geometry.
         """
         self._time['ADD_CHIPS'] = perf_counter()
 
-        if not isinstance(chips, list):  # only one chip
-            cpus = 1
-            chips = [(chips, variant_name, kwargs)]
-
-        if cpus is None:
-            cpus = min(len(chips), os.cpu_count())
-        if self._cpu_override > 0:
-            cpus = self._cpu_override
-
-        # Pool.map() needs all arguments packed into a single list
-        xargs = (self.name, self.with_grid, self._mask_set_dir, self.export_drc, self._extra_params)
-        chip_args = ((chip, xargs) for chip in chips)
-
-        file_names = []
-        if cpus == 1 or self._single_process:
-            file_names += map(self._create_chip, chip_args)
+        if threads is None:
+            threads = os.cpu_count()
+        if threads is None or threads < 1 or is_standalone_session():
+            threads = 1
+
+        if threads == 1:
+            for chip_class, variant_name, *params in tqdm(chips, desc='Building variants',
+                                                          bar_format=default_bar_format):
+                self.add_chip(chip_class, variant_name, **(params[0] if params else {}))
         else:
-            print(f"Building chip variants in parallel using {cpus} processes...")
-            with Pool(cpus) as pool:
-                file_names += pool.map(self._create_chip, chip_args)
-
-        # import chip cells exported by the parallel processes into the mask
-        for variant, file_name in tqdm(file_names, desc='Add chips into mask', bar_format=default_bar_format):
-            self._load_chip_into_mask(file_name, variant)
+            print(f"Building chip variants in parallel using {threads} threads...")
 
-    @staticmethod
-    def _create_chip(chip_arg):
-        """Create chip, possibly in a separate process."""
+            template = self._get_template()
 
-        chip, xargs = chip_arg
-        chip_class, variant_name, *chip_params = chip
-        name, with_grid, _mask_set_dir, export_drc, _extra_params = xargs
+            class ChipSubprocessException(Exception):
+                def __init__(self, err, chip_variant):
+                    super().__init__()
+                    self.err = err
+                    self.chip_variant = chip_variant
+                def __str__(self):
+                    return f'Building the {self.chip_variant} chip variant caused the following error:'\
+                    f'{os.linesep}{self.err}'
+
+            def _subprocess_worker(args):
+                with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                                      startupinfo=STARTUPINFO) as proc:
+                    _, errs = proc.communicate()
+                    # Process has error return code, return error stream
+                    if proc.returncode > 0:
+                        return errs.decode('UTF-8')
+                return None
+
+            def _params_to_str(params):  # flatten a parameters dictionary to a string
+                ps = ""
+                for n, v in params.items():
+                    if isinstance(v, str):
+                        ps += f",{n}={repr(v)}"
+                    elif isinstance(v, pya.DBox):
+                        ps += f",{n}=pya.DBox({v.p1.x}, {v.p1.y}, {v.p2.x}, {v.p2.y})"
+                    elif isinstance(v, pya.DVector):
+                        ps += f",{n}=pya.DVector({v.x}, {v.y})"
+                    elif isinstance(v, pya.DPoint):
+                        ps += f",{n}=pya.DPoint({v.x}, {v.y})"
+                    else:
+                        ps += f",{n}={v}"
+                return ps
+
+            tp = ThreadPool(threads)
+            file_names = []
+            processes = {}
+            for chip_class, variant_name, *param_list in chips:
+                # create the script for generating this chip with the correct parameters and exporting the chip files
+                params = {
+                    'name_chip': variant_name,
+                    'name_mask': self.name,
+                    'with_grid': self.with_grid,
+                    'merge_base_metal_gap': True,
+                    }
+                if param_list:
+                    params.update(param_list[0])
+
+                element_import = f'from {chip_class.__module__} import {chip_class.__name__}'
+                create_element = f'cell = {chip_class.__name__}.create(layout {_params_to_str(params)})'
+                chip_path = self._mask_set_dir/"Chips"/f"{variant_name}"
+                chip_path.mkdir(parents=True, exist_ok=True)
+                script_name = str(chip_path / f"{variant_name}.py")
+                file_names.append((variant_name, str(chip_path / f"{variant_name}.oas"), script_name))
+
+                substitution_parameters = {
+                    'name_mask': self.name,
+                    'chip_path': str(chip_path),
+                    'variant_name': variant_name,
+                    'chip_class': chip_class.__name__,
+                    'element_import': element_import,
+                    'create_element': create_element,
+                    'export_drc': self.export_drc
+                }
+                substitution_parameters.update(self._thread_create_chip_parameters)
+                result = template.substitute(**substitution_parameters)
+                with open(script_name, "w") as f:
+                    f.write(result)
+
+                # launch klayout process that runs the created script
+                try:  # pylint: disable=consider-using-with
+                    processes[variant_name] = tp.apply_async(_subprocess_worker,
+                                   ([klayout_executable_command(), "-e", "-z", "-nc", "-rm", script_name],)
+                                   )
+                except subprocess.CalledProcessError as e:
+                    self.__log.error(e.output)
+
+            # wait for processes to end
+            tp.close()
+            for variant_name, process in processes.items():
+                process_error = process.get()
+                if process_error is not None:
+                    raise ChipSubprocessException(process_error, variant_name)
+            tp.join()
+
+            # import chip cells exported by the parallel processes into the mask
+            for variant_name, file_name, script_name in tqdm(file_names, desc='Building variants (parallel)',
+                                                             bar_format=default_bar_format):
+                self._load_chip_into_mask(file_name, variant_name)
+                # remove the script that was used to generate the chip
+                if os.path.exists(script_name):
+                    os.remove(script_name)
 
-        chip_path = _mask_set_dir/"Chips"/f"{variant_name}"
+    def add_chip(self, chip, variant_name, **kwargs):
+        """Adds a chip with the given name and parameters to self.chips_map_legend and exports chip files.
+
+        Args:
+            chip: the chip type class (for PCell chip), or a chip cell (for manually designed chip)
+            variant_name: name for specific variant, the same as in the mask layout
+            **kwargs: any parameters passed to the chip PCell
+        """
+
+        chip_path = self._mask_set_dir/"Chips"/f"{variant_name}"
         chip_path.mkdir(parents=True, exist_ok=True)
 
-        logging.basicConfig(level=logging.DEBUG)  # this level is NOT actually used
-        route_log(filename=chip_path/f"{variant_name}.log", stdout=_extra_params["enable_debug"])
+        if isclass(chip):
+            cell = self.variant_definition(chip, variant_name, **kwargs)[variant_name]
+            export_chip(cell, variant_name, chip_path, self.layout, self.export_drc)
+            self.layout.delete_cell_rec(cell.cell_index())
+        else:
+            export_chip(chip, variant_name, chip_path, self.layout, self.export_drc)
 
-        view = KLayoutView()
-        layout = view.layout
+        self._load_chip_into_mask(str(chip_path / f"{variant_name}.oas"), variant_name)
 
-        if isclass(chip_class):
-            params = {
-                'name_chip': variant_name,
-                'name_mask': name,
-                'with_grid': with_grid,
-                'merge_base_metal_gap': True,
-                'display_name': variant_name,
-                'name_copy': None,
-            }
-            if chip_params:
-                params.update(chip_params[0])
-            cell = chip_class.create(layout, **params)
-        else:  # its a file name, load it
-            load_opts = pya.LoadLayoutOptions()
-            if hasattr(pya.LoadLayoutOptions, "CellConflictResolution"):
-                load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
-            layout.read(chip_class, load_opts)
-            cell = layout.top_cells()[-1]
+    def variant_definition(self, chip_class, variant_name, **kwargs):
+        """Returns chip variant definition with default mask specific parameters.
 
-        export_chip(cell, variant_name, chip_path, layout, export_drc)
-        view.close()
+        Args:
+            chip_class: the chip type class
+            variant_name: name for specific variant, the same as in the mask layout
+            **kwargs: any parameters passed to the chip PCell
 
-        return variant_name, str(chip_path / f"{variant_name}.oas")
+        Returns:
+            dictionary compatible with mask map structure
+        """
+        self.__log.info("Resolving %s", variant_name)
+
+        chip_parameters = {
+            "merge_base_metal_gap": True,
+            "name_chip": variant_name,
+            "display_name": variant_name,
+            "name_mask": self.name,
+            "name_copy": None,
+            "with_grid": self.with_grid,
+            **kwargs
+        }
+
+        return {variant_name: chip_class.create(self.layout, **chip_parameters)}
 
     def build(self, remove_guiding_shapes=True):
         """Builds the mask set.
 
         Creates cells for the mask based on self.mask_layouts and self.chips_map_legend. Optionally removes
         guiding shapes from the layout. Populates self.used_chips with the chips used in the mask layouts.
 
@@ -328,7 +416,60 @@
 
     def _load_chip_into_mask(self, file_name, variant_name):
         """Loads a chip from file_name to self.layout and adds it into self.chips_map_legend["variant_name"]"""
         load_opts = pya.LoadLayoutOptions()
         load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
         self.layout.read(file_name, load_opts)
         self.chips_map_legend.update({variant_name: self.layout.top_cells()[-1]})
+
+    def _get_template(self):
+        """Returns an updated template string."""
+
+        temp = _CREATE_CHIP_TEMPLATE
+        for i in self.template_imports:
+            temp = temp.replace('#TEMPLATE_IMPORT#', i, 1)
+        return Template(temp)
+
+
+# Template for creating and exporting a chip during mask generation.
+#
+# This is used in _get_template() to create a template used in add_chips() to create chips in
+# parallel. The "#TEMPLATE_IMPORT#" strings in it will be replaced by "template_imports" elements
+# to update the template itself.
+
+_CREATE_CHIP_TEMPLATE = """
+
+import logging
+import sys
+import traceback
+#TEMPLATE_IMPORT#
+from pathlib import Path
+from kqcircuits.masks.mask_export import export_chip
+from kqcircuits.pya_resolver import pya
+from kqcircuits.klayout_view import KLayoutView
+from kqcircuits.util.log_router import route_log
+${element_import}
+
+try:
+    logging.basicConfig(level=logging.DEBUG)  # this level is NOT actually used
+    chip_path = Path(r"${chip_path}")
+    route_log(filename=chip_path/"${variant_name}.log")
+
+    view = KLayoutView()
+    layout, top_cell = view.layout, view.top_cell
+
+    # cell definition and arbitrary code here
+    ${create_element}
+
+    top_cell.insert(pya.DCellInstArray(cell.cell_index(), pya.DTrans()))
+
+    # export chip files
+    export_chip(cell, "${variant_name}", chip_path, layout, ${export_drc})
+
+#TEMPLATE_IMPORT#
+
+except Exception as err:
+    print(traceback.format_exc(), file=sys.stderr)
+    pya.Application.instance().exit(1)
+pya.Application.instance().exit(0)
+
+"""
```

### Comparing `kqcircuits-4.6.14/kqcircuits/pya_resolver.py` & `kqcircuits-4.6.9rc1/kqcircuits/pya_resolver.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/qubits/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/qubits/double_pads.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,19 @@
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import math
 
 from kqcircuits.elements.element import Element
 from kqcircuits.junctions.squid import Squid
-from kqcircuits.junctions.manhattan import Manhattan
 from kqcircuits.util.parameters import Param, pdt, add_parameters_from
 from kqcircuits.qubits.qubit import Qubit
 from kqcircuits.pya_resolver import pya
 
 @add_parameters_from(Squid, junction_type="Manhattan Single Junction")
-@add_parameters_from(Manhattan)
 class DoublePads(Qubit):
     """A two-island qubit, consisting of two rounded rectangles shunted by a junction, with one capacitive coupler.
 
     Contains a coupler on the north edge and two separate qubit islands in the center
     joined by a junction or SQUID loaded from another library.
     Refpoint for a readout line at the opening to the coupler and a modifiable refpoint for
     a driveline outside of the rectangle.
```

### Comparing `kqcircuits-4.6.14/kqcircuits/qubits/double_pads_splines.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads_splines.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/qubits/qubit.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/qubit.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/qubits/swissmon.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/swissmon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/airbridges_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/airbridges_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/circular_capacitor_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/circular_capacitor_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/cross_section_simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/cross_section_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/double_pads_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/double_pads_sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,8 +54,8 @@
                 InternalPort((port_i := port_i + 1), *self.etched_line(refp["port_squid_a"], refp["port_squid_b"]),
                     face=port_face, inductance=self.junction_inductance, capacitance=self.junction_capacitance,
                     junction=True
                 )
             )
 
         self.produce_waveguide_to_port(refp["port_cplr"], refp["port_cplr_corner"], (port_i := port_i + 1),
-            "top", waveguide_length=self.waveguide_length, face=port_face)
+            "top", waveguide_length=200, face=port_face)
```

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/empty_simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/empty_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/ansys/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/ansys/ansys_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/ansys_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/elmer/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/elmer/elmer_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/elmer_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from pathlib import Path
 from distutils.dir_util import copy_tree
 
 from kqcircuits.simulations.export.util import export_layers
 from kqcircuits.util.export_helper import write_commit_reference_file
 from kqcircuits.defaults import ELMER_SCRIPT_PATHS
 from kqcircuits.simulations.simulation import Simulation
-from kqcircuits.simulations.cross_section_simulation import CrossSectionSimulation
 from kqcircuits.util.geometry_json_encoder import GeometryJsonEncoder
 
 
 def copy_elmer_scripts_to_directory(path: Path):
     """
     Copies Elmer scripts into directory path.
 
@@ -41,88 +40,61 @@
         path: Location where to copy scripts folder.
     """
     if path.exists() and path.is_dir():
         for script_path in ELMER_SCRIPT_PATHS:
             copy_tree(str(script_path), str(path), update=1)
 
 
-def export_elmer_json(simulation,
+def export_elmer_json(simulation: Simulation,
                       path: Path,
                       tool='capacitance',
                       linear_system_method='bicgstab',
                       p_element_order=1,
                       frequency=5,
                       mesh_size=None,
-                      workflow=None,
-                      dielectric_surfaces=None,
-                      is_axisymmetric=False):
+                      workflow=None):
     """
     Export Elmer simulation into json and gds files.
 
     Args:
         simulation: The simulation to be exported.
         path: Location where to write json.
-        tool(str): Available: "capacitance", "wave_equation" and "cross-section" (Default: capacitance)
+        tool(str): Available: "capacitance" and "wave_equation" (Default: capacitance)
         linear_system_method(str): Available: 'bicgstab', 'mg' (Default: bicgstab)
         p_element_order(int): polynomial order of p-elements (Default: 1)
         frequency: Units are in GHz. To set up multifrequency analysis, use list of numbers.
         mesh_size(dict): Parameters to determine mesh element sizes
         workflow(dict): Parameters for simulation workflow
-        dielectric_surfaces: Loss tangents for dielectric interfaces, thickness and permittivity should be specified in
-            the simulation. The loss tangent is post-processed to the participation to get the quality factor.
-            Default is None. Input is of the form::
-
-                'substrate': {
-                    'tan_delta_surf': 5e-7
-                },
-                'layerMA': {  # metal–vacuum
-                    'tan_delta_surf': 0.001,  # loss tangent
-                },
-                'layerMS': { # metal–substrate
-                    'tan_delta_surf': 0.001,
-                },
-                'layerSA': { # substrate–vacuum
-                    'tan_delta_surf': 0.001,
-                }
-        is_axisymmetric(bool): Simulate with Axi Symmetric coordinates along :math:`y\\Big|_{x=0}` (Default: False)
 
     Returns:
          Path to exported json file.
     """
-    is_cross_section = isinstance(simulation, CrossSectionSimulation)
-
-    if simulation is None or not isinstance(simulation, (Simulation, CrossSectionSimulation)):
+    if simulation is None or not isinstance(simulation, Simulation):
         raise ValueError("Cannot export without simulation")
 
     # collect data for .json file
-    if is_cross_section:
-        layers = simulation.layer_dict
-
     json_data = {
         'tool': tool,
+        'linear_system_method': linear_system_method,
+        'p_element_order': p_element_order,
         **simulation.get_simulation_data(),
-        **({'layers': {k: (v.layer, v.datatype) for k, v in layers.items()}} if is_cross_section else {}),
         'mesh_size': {} if mesh_size is None else mesh_size,
         'workflow': {} if workflow is None else workflow,
         'frequency': frequency,
-        **({} if dielectric_surfaces is None else {'dielectric_surfaces': dielectric_surfaces}),
-        'linear_system_method': linear_system_method,
-        'p_element_order': p_element_order,
-        'is_axisymmetric': is_axisymmetric,
     }
 
     # write .json file
     json_filename = str(path.joinpath(simulation.name + '.json'))
     with open(json_filename, 'w') as fp:
         json.dump(json_data, fp, cls=GeometryJsonEncoder, indent=4)
 
     # write .gds file
     gds_filename = str(path.joinpath(simulation.name + '.gds'))
     export_layers(gds_filename, simulation.layout, [simulation.cell], output_format='GDS2',
-                  layers=layers.values() if is_cross_section else simulation.get_layers())
+                  layers=simulation.get_layers())
 
     return json_filename
 
 
 def export_elmer_script(json_filenames, path: Path, workflow=None, file_prefix='simulation',
         script_file='scripts/run.py'):
     """
@@ -283,55 +255,36 @@
     return main_script_filename
 
 
 def export_elmer(simulations: [],
                  path: Path,
                  tool='capacitance',
                  linear_system_method='bicgstab',
-                 p_element_order=3,
+                 p_element_order=1,
                  frequency=5,
                  file_prefix='simulation',
                  script_file='scripts/run.py',
                  mesh_size=None,
                  workflow=None,
-                 dielectric_surfaces=None,
-                 is_axisymmetric=False,
                  skip_errors=False):
     """
     Exports an elmer simulation model to the simulation path.
 
     Args:
 
         simulations(list(Simulation)): list of all the simulations
         path(Path): Location where to output the simulation model
-        tool(str): Available: "capacitance", "wave_equation" and "cross-section" (Default: capacitance)
+        tool(str): Available: "capacitance" and "wave_equation" (Default: capacitance)
         linear_system_method(str): Available: 'bicgstab', 'mg' (Default: bicgstab)
         p_element_order(int): polynomial order of p-elements (Default: 1)
         frequency: Units are in GHz. To set up multifrequency analysis, use list of numbers.
         file_prefix: File prefix of the script file to be created.
         script_file: Name of the script file to run.
         mesh_size(dict): Parameters to determine mesh element sizes
         workflow(dict): Parameters for simulation workflow
-        dielectric_surfaces: Loss tangents for dielectric interfaces, thickness and permittivity should be specified in
-            the simulation. The loss tangent is post-processed to the participation to get the quality factor.
-            Default is None. Input is of the form::
-
-                'substrate': {
-                    'tan_delta_surf': 5e-7
-                },
-                'layerMA': {  # metal–vacuum
-                    'tan_delta_surf': 0.001,  # loss tangent
-                },
-                'layerMS': { # metal–substrate
-                    'tan_delta_surf': 0.001,
-                },
-                'layerSA': { # substrate–vacuum
-                    'tan_delta_surf': 0.001,
-                }
-        is_axisymmetric(bool): Simulate with Axi Symmetric coordinates along :math:`y\\Big|_{x=0}` (Default: False)
         skip_errors(bool): Skip simulations that cause errors. (Default: False)
 
             .. warning::
 
                **Use this carefully**, some of your simulations might not make sense physically and
                you might end up wasting time on bad simulations.
 
@@ -353,24 +306,16 @@
             })
 
     write_commit_reference_file(path)
     copy_elmer_scripts_to_directory(path)
     json_filenames = []
     for simulation in simulations:
         try:
-            json_filenames.append(export_elmer_json(simulation=simulation,
-                                                    path=path,
-                                                    tool=tool,
-                                                    linear_system_method=linear_system_method,
-                                                    p_element_order=p_element_order,
-                                                    frequency=frequency,
-                                                    mesh_size=mesh_size,
-                                                    workflow=workflow,
-                                                    dielectric_surfaces=dielectric_surfaces,
-                                                    is_axisymmetric=is_axisymmetric))
+            json_filenames.append(export_elmer_json(simulation, path, tool, linear_system_method,
+                                                    p_element_order, frequency, mesh_size, workflow))
         except (IndexError, ValueError, Exception) as e:  # pylint: disable=broad-except
             if skip_errors:
                 logging.warning(
                     f'Simulation {simulation.name} skipped due to {e.args}. '\
                     'Some of your other simulations might not make sense geometrically. '\
                     'Disable `skip_errors` to see the full traceback.'
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/export_and_run.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/export_and_run.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/simulation_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/simulation_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/parser.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/parser.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/sonnet_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/sonnet_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/sonnet/template.son` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/template.son`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/util.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     Finds the edge closest to a point, and returns the edge as well as it's polygon and edge index
     """
     # Find closest edge to point
     edges = [(i, j, edge.to_dtype(dbu))
              for (i, polygon) in enumerate(polygons)
              for (j, edge) in enumerate(polygon.each_edge())
              ]
-    (distance, i, j, nearest_edge) = \
-        sorted([(edge.distance_abs(point), i, j, edge) for (i, j, edge) in edges])[0]
-    if distance < tolerance:
+    (sq_distance, i, j, nearest_edge) = \
+        sorted([(((edge.p1 + edge.p2)/2).sq_distance(point), i, j, edge) for (i, j, edge) in edges])[0]
+    if sq_distance < tolerance**2:
         return i, j, nearest_edge
     else:
-        raise ValueError(f"No edge found at {point=}, {nearest_edge=}, {distance=}")
+        raise ValueError(f"No edge found at {point=}, {nearest_edge=}, {sq_distance=}")
 
 
 def get_enclosing_polygon(points: List[List[float]]):
     """
     Order points in such a way that they form a polygon without intersecting
     lines. The ordering is clockwise starting from the left-most point.
```

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/xsection/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/export/xsection/xsection_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/xsection_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import ast
 import json
+import logging
 import os
 import subprocess
 from pathlib import Path
 from typing import Callable, List, Tuple, Union
 from kqcircuits.defaults import STARTUPINFO, XSECTION_PROCESS_PATH
 from kqcircuits.pya_resolver import pya, klayout_executable_command
 from kqcircuits.simulations.export.util import export_layers
@@ -47,31 +48,28 @@
         klayout_dir_name = "KLayout"
     elif os.name == "posix":
         klayout_dir_name = ".klayout"
     else:
         raise SystemError("Error: unsupported operating system")
     xsection_plugin_path = os.path.join(os.path.expanduser("~"), klayout_dir_name, "salt/xsection/macros/xsection.lym")
     cut_string = f"{cut1.x},{cut1.y};{cut2.x},{cut2.y}"
-
-    if not klayout_executable_command():
-        raise Exception("Can't find klayout executable command!")
-    if not Path(xsection_plugin_path).is_file():
-        raise Exception("The 'xsection' plugin is missing in KLayout! Go to 'Tools->Manage Packages' to install it.")
-
-    # Hack: Weird prefix keeps getting added when path is converted to string which breaks the ruby plugin
-    xs_run = str(process_path).replace("\\\\?\\", "")
-    xs_params = str(parameters_path).replace("\\\\?\\", "")
-    # When debugging, remove '-z' argument to see ruby error messages
-    subprocess.run([klayout_executable_command(), input_oas.absolute(), '-z', '-nc', '-rx',
-                    '-r', xsection_plugin_path,
-                    '-rd', f'xs_run={xs_run}',
-                    '-rd', f'xs_params={xs_params}',
-                    '-rd', f'xs_cut={cut_string}',
-                    '-rd', f'xs_out={output_oas.absolute()}'],
-        check=True, startupinfo=STARTUPINFO)
+    try:
+        # Hack: Weird prefix keeps getting added when path is converted to string which breaks the ruby plugin
+        xs_run = str(process_path).replace("\\\\?\\", "")
+        xs_params = str(parameters_path).replace("\\\\?\\", "")
+        # When debugging, remove '-z' argument to see ruby error messages
+        subprocess.run([klayout_executable_command(), input_oas.absolute(), '-z', '-nc', '-rx',
+                        '-r', xsection_plugin_path,
+                        '-rd', f'xs_run={xs_run}',
+                        '-rd', f'xs_params={xs_params}',
+                        '-rd', f'xs_cut={cut_string}',
+                        '-rd', f'xs_out={output_oas.absolute()}'],
+            check=True, startupinfo=STARTUPINFO)
+    except FileNotFoundError:
+        logging.warning("Klayout executable not found.")
 
 
 # pylint: disable=dangerous-default-value
 def create_xsections_from_simulations(simulations: List[Simulation],
                                       output_path: Path,
                                       cuts: Union[Tuple[pya.DPoint, pya.DPoint], List[Tuple[pya.DPoint, pya.DPoint]]],
                                       process_path: Path = XSECTION_PROCESS_PATH,
```

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/finger_capacitor_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/finger_capacitor_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/flip_chip_connector_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/flip_chip_connector_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/port.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/port.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/single_xmon.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/single_xmons_full_chip_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmons_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/waveguides_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/waveguides_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     cpw_length = Param(pdt.TypeDouble, "Waveguide length", 100, unit="μm")
     n_guides = Param(pdt.TypeInt, "Number of guides", 5)
     spacing = Param(pdt.TypeDouble, "Parallel spacing", 100, unit="μm")
     guide_face_id = Param(pdt.TypeString, "Guide face id", '1t1')
     add_bumps = Param(pdt.TypeBoolean, "Add ground bumps", False)
     port_termination_end = Param(pdt.TypeBoolean, "Port termination end", True)
     use_edge_ports = Param(pdt.TypeBoolean, "Use edge ports", True)
-    etch_opposite_face = Param(pdt.TypeBoolean, "Remove the whole opposite face metal if flip chip", False)
-
 
     def build(self):
         self.produce_guides()
         if self.add_bumps:
             self.produce_ground_bumps()
 
     def produce_guides(self):
@@ -74,18 +72,14 @@
                 else:
                     self.produce_waveguide_to_port(p0, p1, i, waveguide_length=cpw_length/2.,
                                                    a=a, b=b, face=face_id[guide_face_id])
                     wg_cell = self.add_element(WaveguideCoplanar, path=pya.DPath([p0, p2], 0), term1=0,
                                                term2=self.b, face_ids=[guide_face_id])
                     self.insert_cell(wg_cell)
 
-            if self.etch_opposite_face:
-                region = pya.Region(self.box.to_itype(self.layout.dbu))
-                self.cell.shapes(self.get_layer("base_metal_gap_wo_grid", face_id=1)).insert(region)
-
     def produce_ground_bumps(self):
         n_guides = self.n_guides
         spacing = self.spacing
         tot_y = (n_guides-1)*spacing
         bump = self.add_element(FlipChipConnectorDc)
 
         for i in range(n_guides-1):
```

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/simulations/xmons_direct_coupling_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/airbridge_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/airbridge_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/cross_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/cross_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/stripes_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/stripes_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/test_structure.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/test_structure.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/test_structures/tsv_test_pattern.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/tsv_test_pattern.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/area.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/area.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/count_instances.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/count_instances.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/coupler_lib.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/coupler_lib.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/deep_delete.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/deep_delete.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/dependencies.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/edit_node_plugin.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/edit_node_plugin.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/export_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/export_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,18 +191,29 @@
     """
     Tries to open file with Klayout. If Klayout is not found, opens file with operating system's default application.
     Implementation supports Windows, macOS, and Linux.
     """
     if argv[-1] == "-q":  # quiet mode, do not run viewer
         return
 
-    exe = klayout_executable_command()
-    if not exe:
+    try:
+        subprocess.call((klayout_executable_command(), filepath))
+        return
+    except FileNotFoundError:
         logging.warning("Klayout executable not found.")
-    else:
-        subprocess.call((exe, filepath))
+
+    try:
+        if platform.system() == 'Windows':  # Windows
+            subprocess.call(filepath, shell=True, startupinfo=STARTUPINFO)
+        elif platform.system() == 'Darwin':  # macOS
+            subprocess.call(('open', filepath))
+        else:  # Linux
+            subprocess.call(('xdg-open', filepath))
+    except FileNotFoundError:
+        logging.warning("Unable to open file %s.", filepath)
+
 
 def get_klayout_version():
     if is_standalone_session():
         return f"KLayout {importlib.metadata.version('klayout')}"
     else:
         return pya.Application.instance().version()
```

### Comparing `kqcircuits-4.6.14/kqcircuits/util/geometry_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/groundgrid.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/groundgrid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/gui_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/gui_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/import_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/import_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/label.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/label.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/layout_to_code.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/layout_to_code.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/library_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/library_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/log_router.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/log_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import logging
 import sys
 
 
-def route_log(lowest_visible_level="INFO", remove_old_handlers=True, filename="", stdout=True):
-    """Routes the log output to stdout and/or the specified logfile.
+def route_log(lowest_visible_level="INFO", remove_old_handlers=True, filename=""):
+    """Routes the log output to stdout and to an optional file
 
     Enables monitoring the log in KLayout console. If requested it also appends logs to the
     specified file. By default removes old handlers from root logger to avoid output to other places
     than defined here.
 
     Arguments:
         lowest_visible_level (String): one of DEBUG, INFO, WARNING, ERROR, CRITICAL
         remove_old_handlers (Boolean): determines if old handlers are removed from the root logger
         filename: name of the file to append logs to
-        stdout: enable printing logs to standard output
     """
 
     root_logger = logging.getLogger()
 
     # To make sure that the logs are only output to the place defined here, old handlers must be removed from the
     # logger. This is needed for example if you want to set a different lowest_visible_level by re-running this.
     # Otherwise the old handlers would cause output with the old lowest_visible_level.
@@ -43,18 +42,18 @@
         while root_logger.hasHandlers():
             root_logger.removeHandler(root_logger.handlers[0])
 
     message_format = "%(asctime)s:%(levelname)s:%(name)s:%(funcName)s:%(message)s"
     date_format = "%Y-%m-%d %H:%M:%S"
     formatter = logging.Formatter(message_format, date_format)
 
-    if stdout:
-        handler = logging.StreamHandler(stream=sys.stdout)
-        handler.setFormatter(formatter)
-        handler.setLevel(lowest_visible_level)
-        root_logger.addHandler(handler)
+    handler = logging.StreamHandler(stream=sys.stdout)
+    handler.setFormatter(formatter)
+    handler.setLevel(lowest_visible_level)
+
+    root_logger.addHandler(handler)
 
     if filename:
         fh = logging.FileHandler(filename)
         fh.setFormatter(formatter)
         fh.setLevel(lowest_visible_level)
         root_logger.addHandler(fh)
```

### Comparing `kqcircuits-4.6.14/kqcircuits/util/merge.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/merge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/netlist_extraction.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/netlist_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,21 +42,18 @@
     The main conceptual difference is that waveguides, that would be analogous to wires, are also
     treated as components. Consequently, a net in the ``nets`` section usually contains exactly two
     overlapping pins that belong to two different components each identified by a unique
     ``subcircuit_id``. One of these is almost always a waveguide. Unconnected pins are not shown
     except for Launchers.
 
     The ``subcircuits`` section is a dictionary of the used cells: ``<subcircuit_id>: {"cell_name":
-    "...", "subcircuit_location": {"_pya_type": "DPoint", "x": <x>, "y": <y>}, ...}``.
-    Where ``cell_name`` is the name of the used Element
+    "...", "subcircuit_location": [<x>, <y>]}``. Where ``cell_name`` is the name of the used Element
     optionally appended with ``$<n>`` if there are more than one Elements of the same type.
     Different instances of the same cell will have different ``subcircuit_id`` but identical
-    ``cell_name``. ``subcircuit_location`` defines the center of the bounding box spanned by the
-    geometry in ``base_metal_gap_wo_grid`` layers, while ``subcircuit_origin`` defines the center
-    of the bounding box spanned by the netlist ports of the cell.
+    ``cell_name``.
 
     The ``circuits`` section maps ``cell_name`` to a dictionary of the named Element's parameters.
 
     If the Cell object is a Chip, the ``chip`` section contains bounding boxes of each face in the chip.
 
     Args:
         cell: pya Cell object
@@ -108,15 +105,15 @@
     """
     # first flatten subcircuits mentioned in elements to breakdown
     # TODO implement an efficient depth first search or similar solution
     for _ in range(internal_layout.top_cell().hierarchy_levels()):
         subcircuits = list(circuit.each_subcircuit())
         for subcircuit in subcircuits:
             internal_cell = internal_layout.cell(subcircuit.circuit_ref().cell_index)
-            if internal_cell.name.split('$')[0].replace('*', ' ') in default_netlist_breakdown:
+            if internal_cell.name.split('$')[0] in default_netlist_breakdown:
                 circuit.flatten_subcircuit(subcircuit)
 
     nets_for_export = {}
     for net in circuit.each_net():
         nets_for_export[net.expanded_name()] = extract_nets(net)
 
     subcircuits_for_export = {}
@@ -144,15 +141,15 @@
     for subcircuit in circuit.each_subcircuit():
         internal_cell = internal_layout.cell(subcircuit.circuit_ref().cell_index)
         if cell_mapping.has_mapping(internal_cell.cell_index()):
             original_cell_index = cell_mapping.cell_mapping(internal_cell.cell_index())
             possible_instances = [(i,i_trans) for i,i_trans in original_instances
                                                 if i.cell.cell_index() == original_cell_index]
         else:
-            log.info(('%s element has no cell mapping in %s between circuit layout and orignal layout,'
+            log.warning(('%s element has no cell mapping in %s between circuit layout and orignal layout,'
                     ' using subcircuit center point as subcircuit_location instead'), internal_cell.name, circuit.name)
             possible_instances = []
 
         used_internal_cells.add(internal_cell)
 
         if hasattr(subcircuit, "trans"):
             subcircuit_trans = subcircuit.trans
@@ -184,19 +181,19 @@
             if len(bboxes) > 0:
                 combined_bbox = pya.DBox(min([bbox.p1.x for bbox in bboxes]), min([bbox.p1.y for bbox in bboxes]),
                                          max([bbox.p2.x for bbox in bboxes]), max([bbox.p2.y for bbox in bboxes]))
                 # subcircuit_location is the center of geometry of all *_base_metal_gap_wo_grid layers in the cell
                 # we also transform the point by instance's predecessors' transformation
                 subcircuit_location = correct_instance_trans * combined_bbox.center()
             else:
-                log.info(('%s element has no bounding boxes in *_base_metal_gap_wo_grid layers in %s,'
+                log.warning(('%s element has no bounding boxes in *_base_metal_gap_wo_grid layers in %s,'
                     ' using subcircuit center point as subcircuit_location instead'),
                     internal_cell.name, circuit.name)
         elif possible_instances:
-            log.info(('Could not find a matching element for %s subcircuit in the orignal layout of %s,'
+            log.warning(('Could not find a matching element for %s subcircuit in the orignal layout of %s,'
                     ' using subcircuit center point as subcircuit_location instead'), internal_cell.name, circuit.name)
 
         subcircuits_for_export[subcircuit.id()] = {
             "cell_name": internal_cell.name,
             "instance_name": correct_instance.property('id') if correct_instance else None,
             "subcircuit_origin": subcircuit_trans.disp,
             "subcircuit_location": subcircuit_location,
```

### Comparing `kqcircuits-4.6.14/kqcircuits/util/netlist_graph.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/netlist_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,16 @@
     graph = nx.Graph()
     graph.add_edges_from(edges)
 
     # Add data to the nodes
     for subcircuit_id in used_subcircuit_ids:
         subcircuit = network["subcircuits"][str(subcircuit_id)]
         graph.nodes[subcircuit_id]["cell_name"] = subcircuit["cell_name"]
-        graph.nodes[subcircuit_id]["cell_type"] = subcircuit["cell_name"].split('$')[0].replace('*', ' ')
-        graph.nodes[subcircuit_id]["location"] = [  subcircuit["subcircuit_location"]["x"],
-                                                    subcircuit["subcircuit_location"]["y"]]
+        graph.nodes[subcircuit_id]["cell_type"] = subcircuit["cell_name"].split('$')[0]
+        graph.nodes[subcircuit_id]["location"] = subcircuit["subcircuit_location"]
         if "instance_name" in subcircuit and subcircuit["instance_name"] is not None:
             instance_name = subcircuit["instance_name"]
         else:
             instance_name = ""
         base_name = instance_name if instance_name != "" else str(subcircuit_id)
 
         # Define a unique name by suffixing with a number if needed
```

### Comparing `kqcircuits-4.6.14/kqcircuits/util/parameter_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/parameter_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/parameters.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/parameters.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/plugin_startup.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/plugin_startup.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/refpoints.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/refpoints.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/replace_squids.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/replace_squids.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits/util/symmetric_polygons.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/symmetric_polygons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.14/kqcircuits.egg-info/SOURCES.txt` & `kqcircuits-4.6.9rc1/kqcircuits.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 kqcircuits/simulations/export/__init__.py
 kqcircuits/simulations/export/export_and_run.py
 kqcircuits/simulations/export/simulation_export.py
 kqcircuits/simulations/export/util.py
 kqcircuits/simulations/export/ansys/__init__.py
 kqcircuits/simulations/export/ansys/ansys_export.py
 kqcircuits/simulations/export/elmer/__init__.py
+kqcircuits/simulations/export/elmer/cross_section_elmer_export.py
 kqcircuits/simulations/export/elmer/elmer_export.py
 kqcircuits/simulations/export/sonnet/__init__.py
 kqcircuits/simulations/export/sonnet/parser.py
 kqcircuits/simulations/export/sonnet/sonnet_export.py
 kqcircuits/simulations/export/sonnet/template.son
 kqcircuits/simulations/export/xsection/__init__.py
 kqcircuits/simulations/export/xsection/xsection_export.py
```

### Comparing `kqcircuits-4.6.14/setup.py` & `kqcircuits-4.6.9rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,28 @@
     author="IQM Finland Oy",
     author_email="kqcircuits@meetiqm.com",
     url="https://iqm-finland.github.io/KQCircuits/",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.9",
     install_requires=[                # Record dependencies in kqcircuits/util/dependencies.py too
-        "klayout>=0.28",
+        "klayout>=0.26",
         "numpy>=1.16",
         "Autologging~=1.3",
         "scipy>=1.2",
         "tqdm>=4.61",
         # psutil was considered when cpu_count(logical=False), was implemented in an alternative way
         # in elmer_export.py and gmsh_helpers.py, consider adding if more features are needed.
     ],
     extras_require={
         "docs": ["sphinx~=4.4", "sphinx-rtd-theme~=0.4", "networkx>=2.7", "matplotlib>=3.5.1"],
         "tests": ["pytest>=6.0.2", "pytest-cov~=2.8", "pytest-xdist>=2.1", "tox>=3.18", "pylint==2.9",
                   "networkx>=2.7", "matplotlib>=3.5.1", "nbqa~=1.3"],
         "notebooks": ["jupyter~=1.0.0", "klayout>=0.28"],
         "graphs": ["networkx>=2.7", "matplotlib>=3.5.1"],
-        "simulations": ["gmsh>=4.11.1", "pandas>=1.5.3"],
     },
     entry_points={
         'console_scripts':[
             'kqc = console_scripts.run:run',
             ]
         }
 )
```

