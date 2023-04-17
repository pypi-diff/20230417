# Comparing `tmp/EModelRunner-1.1.7.tar.gz` & `tmp/EModelRunner-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EModelRunner-1.1.7.tar", last modified: Tue Jan 24 13:45:54 2023, max compression
+gzip compressed data, was "dist/EModelRunner-1.1.8.tar", last modified: Mon Apr 17 14:11:36 2023, max compression
```

## Comparing `EModelRunner-1.1.7.tar` & `EModelRunner-1.1.8.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.compile_mod.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.github/workflows/keep-alive.yml
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/EModelRunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   207165 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/images/GUI_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (123)   303675 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/doc/source/logo/BBP-eModelRunner.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42496 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/plotshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/GUI_utils/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/configuration/configparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/configuration/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/configuration/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/create_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/create_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25018 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/create_hoc_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/create_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/create_stimuli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/factsheets/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/experimental_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/ion_channel_mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/morphology_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/factsheets/physiology_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/json_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/morphology/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/morphology/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/parsing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/create_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/protocols_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46801 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/sscx_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/synplas_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/protocols/thalamus_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/run_pairsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/run_synplas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/stimuli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/emodelrunner/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/create_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/glusynapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/minis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/stimuli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synapses/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/emodelrunner/synplas_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_allsteps.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_factsheets.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_multiprotocols.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_recipe_protocols.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_singlestep.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_synapses.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_synapses_short.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/features/
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/features/units.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/RmpRiTau.json
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/allsteps.json
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/multiprotocols.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/singlestep.json
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/synapses.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/synapses_short.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/hoc_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/hoc_recordings/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/VecStim.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/python_recordings/.keep
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   177229 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/synapses/synconf.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7087 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/createsimulation.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/features.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/main_protocol.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/run_hoc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/sscx_sample_dir/templates/synapses.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/config_1Hz_10ms.ini
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/fit_params.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/GluSynapse.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/VecStim.mod
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/gap.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/optimized/
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   322804 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)   491533 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/protocols/stimuli_1Hz.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/run_pairsim.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/cpre_cpost.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/syn_extra_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/synapse_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/synconf.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/cell_info.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/compile_mechanisms.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/features/dNAD_ltb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/features/units.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/params/final.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_HH.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Kleak.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Naleak.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iL.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ic.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/ican.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   384138 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/python_recordings/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/examples/thalamus_sample_dir/synapses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 13:45:54.000000 EModelRunner-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-24 13:45:46.000000 EModelRunner-1.1.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.compile_mod.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/keep-alive.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/EModelRunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/EModelRunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   207165 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/images/GUI_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)   303675 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/logo/BBP-eModelRunner.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/plotshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25018 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_hoc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_stimuli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/factsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/experimental_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/ion_channel_mechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/morphology_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/physiology_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/json_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/parsing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/create_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/protocols_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46821 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/sscx_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16774 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/synplas_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35315 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/thalamus_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run_pairsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run_synplas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/stimuli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/create_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/glusynapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/minis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/stimuli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synplas_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_allsteps.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_factsheets.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_multiprotocols.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_recipe_protocols.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_singlestep.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses_short.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/units.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/RmpRiTau.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/allsteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/multiprotocols.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/singlestep.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/synapses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/synapses_short.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/hoc_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/hoc_recordings/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/VecStim.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/python_recordings/.keep
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   177229 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synconf.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7087 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/createsimulation.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/features.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/main_protocol.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/run_hoc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/synapses.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/config_1Hz_10ms.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/fit_params.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/GluSynapse.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/VecStim.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/gap.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/
+-rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   322804 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)   491533 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/stimuli_1Hz.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/run_pairsim.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/cpre_cpost.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/syn_extra_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapse_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synconf.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/cell_info.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/compile_mechanisms.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/dNAD_ltb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/units.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/final.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_HH.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kleak.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Naleak.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iL.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ic.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/ican.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   384138 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/python_recordings/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/synapses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/tox.ini
```

### Comparing `EModelRunner-1.1.7/.github/workflows/build.yml` & `EModelRunner-1.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/.github/workflows/keep-alive.yml` & `EModelRunner-1.1.8/.github/workflows/keep-alive.yml`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/.github/workflows/test.yml` & `EModelRunner-1.1.8/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   workflow_call:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `EModelRunner-1.1.7/.gitignore` & `EModelRunner-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/.pylintrc` & `EModelRunner-1.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/CONTRIBUTING.rst` & `EModelRunner-1.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/COPYING` & `EModelRunner-1.1.8/COPYING`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/EModelRunner.egg-info/PKG-INFO` & `EModelRunner-1.1.8/EModelRunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EModelRunner
-Version: 1.1.7
+Version: 1.1.8
 Summary: Runs cells from Blue Brain Project cell packages, such as sscx, synapse plasticity, etc.
 Home-page: https://github.com/BlueBrain/EModelRunner
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/EModelRunner/issues
 Project-URL: Source, https://github.com/BlueBrain/EModelRunner
 Project-URL: Documentation, https://emodelrunner.readthedocs.io/en/latest
```

### Comparing `EModelRunner-1.1.7/EModelRunner.egg-info/SOURCES.txt` & `EModelRunner-1.1.8/EModelRunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/LICENSE.txt` & `EModelRunner-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/PKG-INFO` & `EModelRunner-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EModelRunner
-Version: 1.1.7
+Version: 1.1.8
 Summary: Runs cells from Blue Brain Project cell packages, such as sscx, synapse plasticity, etc.
 Home-page: https://github.com/BlueBrain/EModelRunner
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/EModelRunner/issues
 Project-URL: Source, https://github.com/BlueBrain/EModelRunner
 Project-URL: Documentation, https://emodelrunner.readthedocs.io/en/latest
```

### Comparing `EModelRunner-1.1.7/README.rst` & `EModelRunner-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/doc/Makefile` & `EModelRunner-1.1.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/doc/source/conf.py` & `EModelRunner-1.1.8/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/doc/source/images/GUI_screenshot.png` & `EModelRunner-1.1.8/doc/source/images/GUI_screenshot.png`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/doc/source/logo/BBP-eModelRunner.jpg` & `EModelRunner-1.1.8/doc/source/logo/BBP-eModelRunner.jpg`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI.py` & `EModelRunner-1.1.8/emodelrunner/GUI.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/__init__.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/frames.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/frames.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             font=style_dict["base_font"],
             width=style_dict["entry_width"],
         )
         self.entry.config(validate="key", validatecommand=(self.reg, "%P"))
 
         # grid
         self.label.grid(row=0, column=0, sticky=tk.W)
-        self.entry.grid(row=0, column=1, sticky=(tk.E))
+        self.entry.grid(row=0, column=1, sticky=tk.E)
 
         self.columnconfigure(1, weight=1)  # only center column grows
 
     def get_value(self, gui, attr_name):
         """Put input value in simulation attribute.
 
         Args:
```

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/interface.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/interface.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/plotshape.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/plotshape.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/simulator.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/simulator.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/GUI_utils/style.py` & `EModelRunner-1.1.8/emodelrunner/GUI_utils/style.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/__init__.py` & `EModelRunner-1.1.8/emodelrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/cell.py` & `EModelRunner-1.1.8/emodelrunner/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,20 +245,20 @@
 
           proc destroy() {localobj nil
             CellRef = nil
           }
 
 
         endtemplate %(template_name)s
-               """ % dict(
-            template_name=template_name,
-            objref_str=objref_str,
-            newseclist_str=newseclist_str,
-            secarrays_str=secarrays_str,
-        )
+               """ % {
+            "template_name": template_name,
+            "objref_str": objref_str,
+            "newseclist_str": newseclist_str,
+            "secarrays_str": secarrays_str,
+        }
         return template
 
     @staticmethod
     def create_empty_cell(name, sim, seclist_names=None, secarray_names=None):
         """Create an empty cell in Neuron.
 
         Args:
```

### Comparing `EModelRunner-1.1.7/emodelrunner/configuration/__init__.py` & `EModelRunner-1.1.8/emodelrunner/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/configuration/configparser.py` & `EModelRunner-1.1.8/emodelrunner/configuration/configparser.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/configuration/subgroups.py` & `EModelRunner-1.1.8/emodelrunner/configuration/subgroups.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/configuration/validator.py` & `EModelRunner-1.1.8/emodelrunner/configuration/validator.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/create_cells.py` & `EModelRunner-1.1.8/emodelrunner/create_cells.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/create_hoc.py` & `EModelRunner-1.1.8/emodelrunner/create_hoc.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/create_hoc_tools.py` & `EModelRunner-1.1.8/emodelrunner/create_hoc_tools.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/create_recordings.py` & `EModelRunner-1.1.8/emodelrunner/create_recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/create_stimuli.py` & `EModelRunner-1.1.8/emodelrunner/create_stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/__init__.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/experimental_features.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/experimental_features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/ion_channel_mechanisms.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/ion_channel_mechanisms.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/morphology_features.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/morphology_features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/output.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,28 +112,28 @@
         a tuple containing
 
         - current_amplitude (int or float): the amplitude current of the step protocol (mA)
         - stim_start (int or float): the start of the stimulus (ms)
         - stim_duration (int or float): the duration of the stimulus (ms)
 
     Raises:
-        Exception: If a step protocol with multiple steps has been provided
+        TypeError: If a step protocol with multiple steps has been provided
     """
     with open(prot_path, "r", encoding="utf-8") as protocol_file:
         protocol_definitions = json.load(protocol_file)
 
     prot = protocol_definitions[protocol_key]
     step_stim = prot["stimuli"]["step"]
 
     if isinstance(step_stim, list):
         exception_message = (
             "ME-type factsheet expects only one step stimulus "
             + "for protocol {key} at {filepath}"
         )
-        raise Exception(exception_message.format(key=protocol_key, filepath=prot_path))
+        raise TypeError(exception_message.format(key=protocol_key, filepath=prot_path))
 
     # get parameters from protocol
     current_amplitude = step_stim["amp"]
     stim_start = step_stim["delay"]
     stim_duration = step_stim["duration"]
 
     return current_amplitude, stim_start, stim_duration
```

### Comparing `EModelRunner-1.1.7/emodelrunner/factsheets/physiology_features.py` & `EModelRunner-1.1.8/emodelrunner/factsheets/physiology_features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/features.py` & `EModelRunner-1.1.8/emodelrunner/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
     if "strict_stim" in feature_config:
         strict_stim = feature_config["strict_stim"]
     else:
         strict_stim = True
 
     if hasattr(protocol, "stim_start"):
-
         stim_start = protocol.stim_start
 
         if "threshold" in feature_config:
             threshold = feature_config["threshold"]
         else:
             threshold = -30
 
@@ -117,15 +116,14 @@
         del feature_definitions["__comment"]
 
     efeatures = {}
 
     for protocol_name, locations in feature_definitions.items():
         for recording_name, feature_configs in locations.items():
             for feature_config in feature_configs:
-
                 feature_name, feature = get_feature(
                     feature_config,
                     main_protocol,
                     protocol_name,
                     recording_name,
                     prefix,
                 )
```

### Comparing `EModelRunner-1.1.7/emodelrunner/json_utilities.py` & `EModelRunner-1.1.8/emodelrunner/json_utilities.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/load.py` & `EModelRunner-1.1.8/emodelrunner/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
     """
     with open(mechs_path, "r", encoding="utf-8") as mechs_file:
         mechs = json.load(mechs_file)
     mech_definitions = mechs["mechanisms"]
 
     mechanisms_list = []
     for sectionlist, channels in mech_definitions.items():
-
         seclist_locs = multi_locations(sectionlist)
 
         for channel in channels["mech"]:
             mechanisms_list.append(
                 ephys.mechanisms.NrnMODMechanism(
                     name=f"{channel}.{sectionlist}",
                     mod_path=None,
@@ -169,15 +168,14 @@
 
     # set distributions
     distributions = collections.OrderedDict()
     distributions["uniform"] = ephys.parameterscalers.NrnSegmentLinearScaler()
 
     distributions_definitions = definitions["distributions"]
     for distribution, definition in distributions_definitions.items():
-
         if "parameters" in definition:
             dist_param_names = definition["parameters"]
         else:
             dist_param_names = None
         distributions[
             distribution
         ] = ephys.parameterscalers.NrnSegmentSomaDistanceScaler(
```

### Comparing `EModelRunner-1.1.7/emodelrunner/locations.py` & `EModelRunner-1.1.8/emodelrunner/locations.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/morphology/__init__.py` & `EModelRunner-1.1.8/emodelrunner/morphology/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/morphology/builder.py` & `EModelRunner-1.1.8/emodelrunner/morphology/builder.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/morphology/morphology.py` & `EModelRunner-1.1.8/emodelrunner/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/output.py` & `EModelRunner-1.1.8/emodelrunner/output.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/parsing_utilities.py` & `EModelRunner-1.1.8/emodelrunner/parsing_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--config_path",
         default=None,
         help="the path to the config file.",
     )
-    parser.add_argument("-v", "--verbose", action="count", dest="verbosity", default=0)
+    parser.add_argument("-v", "--verbose", type=int, dest="verbosity", default=1)
     return parser.parse_args()
 
 
 def set_verbosity(verbosity):
     """Set verbosity level.
 
     Args:
```

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/__init__.py` & `EModelRunner-1.1.8/emodelrunner/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/create_protocols.py` & `EModelRunner-1.1.8/emodelrunner/protocols/create_protocols.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/protocols_func.py` & `EModelRunner-1.1.8/emodelrunner/protocols/protocols_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,32 +54,32 @@
 
     Args:
         recording_definition (dict): contains the extra recording configuration data
         apical_point_isec (int): apical point section index.
             Should be given if the recording definition "type" is "somadistanceapic"
 
     Raises:
-        Exception: if the recording definition "type" is "somadistanceapic" and
+        ValueError: if the recording definition "type" is "somadistanceapic" and
             apical_point_isec is -1.
-        Exception: if the 'type' in the recording definition is neither
+        ValueError: if the 'type' in the recording definition is neither
             "somadistance", nor "somadistanceapic", nor "nrnseclistcomp"
 
     Returns:
         location of the extra recording
     """
     if recording_definition["type"] == "somadistance":
         location = ephys.locations.NrnSomaDistanceCompLocation(
             name=recording_definition["name"],
             soma_distance=recording_definition["somadistance"],
             seclist_name=recording_definition["seclist_name"],
         )
 
     elif recording_definition["type"] == "somadistanceapic":
         if apical_point_isec == -1:
-            raise Exception(
+            raise ValueError(
                 "Cannot record at a given distance from apical point"
                 f"if apical_point_isec is {apical_point_isec}."
             )
         location = ephys.locations.NrnSecSomaDistanceCompLocation(
             name=recording_definition["name"],
             soma_distance=recording_definition["somadistance"],
             seclist_name=seclist_to_sec[recording_definition["seclist_name"]],
@@ -91,15 +91,15 @@
             name=recording_definition["name"],
             comp_x=recording_definition["comp_x"],
             sec_index=recording_definition["sec_index"],
             seclist_name=recording_definition["seclist_name"],
         )
 
     else:
-        raise Exception(f"Recording type {recording_definition['type']} not supported")
+        raise ValueError(f"Recording type {recording_definition['type']} not supported")
 
     return location
 
 
 def get_recordings(protocol_name, protocol_definition, prefix, apical_point_isec=-1):
     """Get recordings from protocol definition.
 
@@ -121,15 +121,14 @@
             location=SOMA_LOC,
             variable="v",
         )
     )
 
     if "extra_recordings" in protocol_definition:
         for recording_definition in protocol_definition["extra_recordings"]:
-
             location = get_extra_recording_location(
                 recording_definition, apical_point_isec
             )
 
             var = recording_definition["var"]
             recording = RecordingCustom(
                 name=f"{prefix}.{protocol_name}.{location.name}.{var}",
@@ -144,25 +143,25 @@
 def check_for_forbidden_protocol(protocols_dict):
     """Check for unsupported protocol.
 
     Args:
         protocols_dict (dict): contains all protocols to be run
 
     Raises:
-        Exception: If a protocol that should only be used with MainProtocol is present
+        ValueError: If a protocol that should only be used with MainProtocol is present
             in protocols_dict
     """
     # Those protocols cannot be used if they are not in MainProtocol
     forbidden_prots = [
         "RatSSCxRinHoldcurrentProtocol",
         "RatSSCxThresholdDetectionProtocol",
         "StepThresholdProtocol",
         "RampThresholdProtocol",
     ]
     # check the class name of each protocol
     for prot in protocols_dict.values():
         if type(prot).__name__ in forbidden_prots:
             prot_name = type(prot).__name__
-            raise Exception(
-                "No MainProtocol found, but {prot} was found."
+            raise ValueError(
+                f"No MainProtocol found, but {prot_name} was found."
                 f"To use {prot_name}, please set MainProtocol."
             )
```

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/reader.py` & `EModelRunner-1.1.8/emodelrunner/protocols/reader.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/sscx_protocols.py` & `EModelRunner-1.1.8/emodelrunner/protocols/sscx_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1004,23 +1004,23 @@
             param_values (dict): optimized parameters
             sim (bluepyopt.ephys.NrnSimulator): neuron simulator
             isolate (bool): whether to isolate the run in a process with a timeout
                 to avoid bad cells running for too long
             timeout (float): maximum real time (s) the cell is allowed to run when isolated
 
         Raises:
-            Exception: if the threshold_current is not set to the cell model
+            AttributeError: if the threshold_current is not set to the cell model
 
         Returns:
             dict containing the responses for the step protocol
         """
         # pylint: disable=unused-argument
         responses = {}
         if not hasattr(cell_model, "threshold_current"):
-            raise Exception(
+            raise AttributeError(
                 "StepThresholdProtocol: running on cell_model "
                 f"that doesnt have threshold current value set: {cell_model}"
             )
 
         for step_stim in self.step_stimuli:
             step_stim.step_amplitude = cell_model.threshold_current * (
                 float(self.thresh_perc) / 100.0
@@ -1216,23 +1216,23 @@
             param_values (dict): optimized parameters
             sim (bluepyopt.ephys.NrnSimulator): neuron simulator
             isolate (bool): whether to isolate the run in a process with a timeout
                 to avoid bad cells running for too long
             timeout (float): maximum real time (s) the cell is allowed to run when isolated
 
         Raises:
-            Exception: if the threshold_current is not set to the cell model
+            AttributeError: if the threshold_current is not set to the cell model
 
         Returns:
             dict containing the responses for the ramp protocol
         """
         # pylint: disable=unused-argument
         responses = {}
         if not hasattr(cell_model, "threshold_current"):
-            raise Exception(
+            raise AttributeError(
                 "RampThresholdProtocol: running on cell_model "
                 f"that doesnt have threshold current value set: {cell_model}"
             )
 
         self.ramp_stimulus.ramp_amplitude_start = cell_model.threshold_current * (
             float(self.thresh_perc_start) / 100
         )
```

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/synplas_protocols.py` & `EModelRunner-1.1.8/emodelrunner/protocols/synplas_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         Args:
             cell_model (bluepyopt.ephys.models.CellModel): the cell model
             param_values (dict): optimized parameters
             sim (bluepyopt.ephys.NrnSimulator): neuron simulator
 
         Raises:
-            Exception: if the instantiation failed
+            RuntimeError: if the instantiation failed
 
         Returns:
             dict containing the responses
         """
         # pylint: disable=raise-missing-from
         try:
             cell_model.freeze(param_values)
@@ -135,15 +135,15 @@
 
             cell_model.destroy(sim=sim)
 
             cell_model.unfreeze(param_values.keys())
 
             return responses
         except BaseException:
-            raise Exception("".join(traceback.format_exception(*sys.exc_info())))
+            raise RuntimeError("".join(traceback.format_exception(*sys.exc_info())))
 
 
 class SweepProtocolPairSim(ephys.protocols.Protocol):
     """Sweep protocol for pair simulation with fastforwarding.
 
     Attributes:
         name (str): name of this object.
@@ -181,26 +181,26 @@
                 contain first the list for the presynaptic recording
                 and then the list for the postsynaptic recording.
             cvode_active (bool): whether to use variable time step
             fastforward (float): Time after which the synapses are fasforwarded.
                 Leave None for no fastforward.
 
         Raises:
-            Exception: if stimuli is not of size 2 and is not None
-            Exception: if recordings is not of size 2 and is not None
+            ValueError: if stimuli is not of size 2 and is not None
+            ValueError: if recordings is not of size 2 and is not None
         """
         super().__init__(name)
         if stimuli is not None and len(stimuli) != 2:
-            raise Exception(
+            raise ValueError(
                 "Stimuli should be of size 2 and contain"
                 "[presynaptic_stimuli, postsynaptic_stimuli]"
             )
         self.stimuli = stimuli
         if recordings is not None and len(stimuli) != 2:
-            raise Exception(
+            raise ValueError(
                 "Recordings should be of size 2 and contain"
                 "[presynaptic_recordings, postsynaptic_recordings]"
             )
         self.recordings = recordings
         self.cvode_active = cvode_active
         self.fastforward = fastforward
 
@@ -239,15 +239,15 @@
             precell_model (bluepyopt.ephys.models.CellModel): the presynaptic cell model
             postcell_model (bluepyopt.ephys.models.CellModel): the postsynaptic cell model
             pre_param_values (dict): optimized parameters of the presynaptic cell model
             post_param_values (dict): optimized parameters of the postsynaptic cell model
             sim (bluepyopt.ephys.NrnSimulator): neuron simulator
 
         Raises:
-            Exception: if the instantiation failed
+            RuntimeError: if the instantiation failed
 
         Returns:
             list of 2 dicts containing the responses of both the cells
 
             Has the structure [presynaptic response dict, postsynaptic response dict]
         """
         # pylint: disable=raise-missing-from
@@ -294,15 +294,15 @@
             postcell_model.destroy(sim=sim)
 
             precell_model.unfreeze(pre_param_values.keys())
             postcell_model.unfreeze(post_param_values.keys())
 
             return responses
         except BaseException:
-            raise Exception("".join(traceback.format_exception(*sys.exc_info())))
+            raise RuntimeError("".join(traceback.format_exception(*sys.exc_info())))
 
     def run(
         self,
         precell_model,
         postcell_model,
         pre_param_values,
         post_param_values,
@@ -389,15 +389,14 @@
             sim (bluepyopt.ephys.NrnSimulator): neuron simulator
             pre_icell (neuron cell): presynaptic cell instantiation in simulator
             post_icell (neuron cell): postsynaptic cell instantiation in simulator
         """
         icells = [pre_icell, post_icell]
 
         for i, icell in enumerate(icells):
-
             for stimulus in self.stimuli[i]:
                 stimulus.instantiate(sim=sim, icell=icell)
 
             for recording in self.recordings[i]:
                 try:
                     recording.instantiate(sim=sim, icell=icell)
                 except ephys.locations.EPhysLocInstantiateException:
```

### Comparing `EModelRunner-1.1.7/emodelrunner/protocols/thalamus_protocols.py` & `EModelRunner-1.1.8/emodelrunner/protocols/thalamus_protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 # pylint: disable=too-many-lines
 
 import collections
 import copy
 import logging
 import numpy as np
+
 from bluepyopt import ephys
+from tqdm import tqdm
 
 from emodelrunner.protocols.protocols_func import CurrentOutputKeyMixin
 
 logger = logging.getLogger(__name__)
 
 
 class RatSSCxMainProtocol(ephys.protocols.Protocol):
@@ -120,49 +122,54 @@
         """Run protocol."""
         # pylint: disable=unused-argument
         responses = collections.OrderedDict()
 
         cell_model.freeze(param_values)
 
         # Find resting membrane potential
+        logger.info("Running RMP protocol")
         rmp_response = self.rmp_protocol.run(cell_model, {}, sim=sim)
         responses.update(rmp_response)
         rmp = self.rmp_efeature.calculate_feature(rmp_response)
 
         # Find Rin and holding current
         if hasattr(self, "rinhold_protocol_dep"):
+            logger.info("Running Rinhold protocol (depolarizing)")
             rinhold_response_dep = self.rinhold_protocol_dep.run(
                 cell_model, {}, sim=sim, rmp=rmp
             )
             holding_current_dep = cell_model.holding_current_dep
 
             rin_dep = self.rin_efeature_dep.calculate_feature(rinhold_response_dep)
             responses.update(rinhold_response_dep)
 
+        logger.info("Running Rinhold protocol (hyperpolarizing)")
         rinhold_response_hyp = self.rinhold_protocol_hyp.run(
             cell_model, {}, sim=sim, rmp=rmp
         )
 
         if rinhold_response_hyp is not None:
             rin_hyp = self.rin_efeature_hyp.calculate_feature(rinhold_response_hyp)
 
             responses.update(rinhold_response_hyp)
 
             if hasattr(self, "thdetect_protocol_dep"):
+                logger.info("Running threshold detection protocol (depolarizing)")
                 responses.update(
                     self.thdetect_protocol_dep.run(
                         cell_model,
                         {},
                         sim=sim,
                         holdi=holding_current_dep,
                         rmp=rmp,
                         rin=rin_dep,
                     )
                 )
 
+            logger.info("Running threshold detection protocol (hyperpolarizing)")
             responses.update(
                 self.thdetect_protocol_hyp.run(
                     cell_model,
                     {},
                     sim=sim,
                     holdi=cell_model.holding_current_hyp,
                     rmp=rmp,
@@ -176,21 +183,23 @@
 
         cell_model.unfreeze(param_values.keys())
 
         return responses
 
     def _run_pre_protocols(self, cell_model, sim, responses):
         """Runs the pre_protocols and updates responses dict."""
-        for pre_protocol in self.pre_protocols:
+        logger.info("Running pre-protocols")
+        for pre_protocol in tqdm(self.pre_protocols):
             response = pre_protocol.run(cell_model, {}, sim=sim)
             responses.update(response)
 
     def _run_other_protocols(self, cell_model, sim, responses):
         """Runs the other_protocols and updates responses dict."""
-        for other_protocol in self.other_protocols:
+        logger.info("Running other protocols")
+        for other_protocol in tqdm(self.other_protocols):
             response = other_protocol.run(cell_model, {}, sim=sim)
             responses.update(response)
 
     def generate_current(
         self, thres_i_hyp, thres_i_dep, holding_i_hyp, holding_i_dep, dt
     ):
         """Generate current for all protocols except rin and threshold detection.
@@ -944,15 +953,15 @@
         self.stochkv_det = stochkv_det
 
     def run(self, cell_model, param_values, sim=None, isolate=None, timeout=None):
         """Run protocol."""
         logger.info("Running protocol %s", self.name)
         responses = {}
         if not hasattr(cell_model, "threshold_current_hyp"):
-            raise Exception(
+            raise AttributeError(
                 f"StepThresholdProtocol: running on cell_model "
                 f"that doesnt have threshold current value set: {str(cell_model)}",
             )
 
         if self.name.endswith("_hyp"):
             self.holding_stimulus.step_amplitude = cell_model.holding_current_hyp
```

### Comparing `EModelRunner-1.1.7/emodelrunner/recordings.py` & `EModelRunner-1.1.8/emodelrunner/recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/run.py` & `EModelRunner-1.1.8/emodelrunner/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         currents = protocols.get_thalamus_stim_currents(responses, mtype, dt)
 
     # write responses
     output_dir = config.get("Paths", "output_dir")
     write_responses(responses, output_dir)
     write_current(currents, output_dir)
 
-    logger.info("Python Recordings Done")
+    logger.info("Python Recordings Done.")
+    logger.info("Responses written to %s", output_dir)
 
 
 if __name__ == "__main__":
     args = get_parser_args()
     set_verbosity(args.verbosity)
 
     main(config_path=args.config_path)
```

### Comparing `EModelRunner-1.1.7/emodelrunner/run_pairsim.py` & `EModelRunner-1.1.8/emodelrunner/run_pairsim.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     syn_prop_path = config.get("Paths", "syn_prop_path")
     write_synplas_output(responses[1], pre_spike_train, output_path, syn_prop_path)
     write_synplas_precell_output(
         responses[0], presyn_protocol_name, precell_output_path
     )
 
     logger.info("Python Recordings Done.")
+    logger.info("Responses written to %s", output_path)
 
 
 if __name__ == "__main__":
     args = get_parser_args()
     set_verbosity(args.verbosity)
 
     run(config_path=args.config_path)
```

### Comparing `EModelRunner-1.1.7/emodelrunner/run_synplas.py` & `EModelRunner-1.1.8/emodelrunner/run_synplas.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
     # write responses
     output_path = config.get("Paths", "synplas_output_path")
     syn_prop_path = config.get("Paths", "syn_prop_path")
     write_synplas_output(responses, pre_spike_train, output_path, syn_prop_path)
 
     logger.info("Python Recordings Done.")
+    logger.info("Responses written to %s", output_path)
 
 
 if __name__ == "__main__":
     args = get_parser_args()
     set_verbosity(args.verbosity)
 
     run(config_path=args.config_path)
```

### Comparing `EModelRunner-1.1.7/emodelrunner/stimuli.py` & `EModelRunner-1.1.8/emodelrunner/stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/__init__.py` & `EModelRunner-1.1.8/emodelrunner/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/create_locations.py` & `EModelRunner-1.1.8/emodelrunner/synapses/create_locations.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/glusynapse.py` & `EModelRunner-1.1.8/emodelrunner/synapses/glusynapse.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/mechanism.py` & `EModelRunner-1.1.8/emodelrunner/synapses/mechanism.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/minis.py` & `EModelRunner-1.1.8/emodelrunner/synapses/minis.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             self.ips = {}
         if self.syn_mini_netcons is None:
             self.syn_mini_netcons = {}
 
         for location in self.locations:
             # self.connections[location.name] = []
             for synapse in location.instantiate(sim=sim, icell=icell):
-
                 sid = synapse.hsynapse.synapseID
 
                 if self.popids is None:
                     # Default values in Neurodamus
                     source_popid = 0
                     target_popid = 0
                 else:
```

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/recordings.py` & `EModelRunner-1.1.8/emodelrunner/synapses/recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/stimuli.py` & `EModelRunner-1.1.8/emodelrunner/synapses/stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synapses/synapse.py` & `EModelRunner-1.1.8/emodelrunner/synapses/synapse.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/emodelrunner/synplas_analysis.py` & `EModelRunner-1.1.8/emodelrunner/synplas_analysis.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/LICENSE.txt` & `EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_allsteps.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_allsteps.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_factsheets.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_factsheets.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_multiprotocols.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_multiprotocols.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_recipe_protocols.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_recipe_protocols.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_singlestep.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_singlestep.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_synapses.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/config_synapses_short.ini` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses_short.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/features/units.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/units.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/params/final.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/params/pyr.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/allsteps.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/allsteps.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/config/protocols/multiprotocols.json` & `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/multiprotocols.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/VecStim.mod` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/VecStim.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/mechanisms/notes.txt` & `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/synapses/synapses.tsv` & `EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/createsimulation.jinja2` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/createsimulation.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/features.hoc` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/features.hoc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/main_protocol.jinja2` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/main_protocol.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/run_hoc.jinja2` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/run_hoc.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/sscx_sample_dir/templates/synapses.jinja2` & `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/synapses.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/LICENSE.txt` & `EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/config/config_1Hz_10ms.ini` & `EModelRunner-1.1.8/examples/synplas_sample_dir/config/config_1Hz_10ms.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/config/params/final.json` & `EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/config/params/pyr.json` & `EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/GluSynapse.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/GluSynapse.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/VecStim.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/VecStim.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc` & `EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc` & `EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat` & `EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/protocols/stimuli_1Hz.json` & `EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/stimuli_1Hz.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/syn_extra_params.json` & `EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/syn_extra_params.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/synplas_sample_dir/synapses/synapse_properties.json` & `EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapse_properties.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/LICENSE.txt` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/features/dNAD_ltb.json` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/dNAD_ltb.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/features/units.json` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/units.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/params/final.json` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_HH.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_HH.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iA.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_iL.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iL.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ic.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ic.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/ican.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/ican.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc` & `EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/requirements_docs.txt` & `EModelRunner-1.1.8/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.7/setup.py` & `EModelRunner-1.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "bluepyopt>=1.13.168",
         "neurom>=3.1.0",
         "h5py",
         "matplotlib",
         "schema",
         "Pebble>=4.3.10",
         "importlib_metadata; python_version<'3.8'",
+        "tqdm>=4.65.0",
     ],
     packages=find_packages(exclude=["tests"]),
     python_requires=">=3.7",
     extras_require={"docs": ["sphinx", "sphinx-bluebrain-theme"]},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
```

### Comparing `EModelRunner-1.1.7/tox.ini` & `EModelRunner-1.1.8/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
 [gh-actions]
 python =
     3.7: py3
     3.8: check-packaging, lint, docs, py3
     3.9: py3
     3.10: py3
+    3.11: py3
 
 [testenv]
 envdir =
     py3{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py3
     py37{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py37
     py38{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py38
     py39{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py39
     py310{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py310
+    py311{-unit,-sscx,-synplas,-thalamus}: {toxworkdir}/py311
 deps = 
     {[base]testdeps}
     coverage
     pytest-cov
     pytest-xdist
     filelock
     hypothesis
```

