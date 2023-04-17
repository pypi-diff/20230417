# Comparing `tmp/btrack-0.5.1.tar.gz` & `tmp/btrack-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrack-0.5.1.tar", last modified: Mon Apr  3 15:43:36 2023, max compression
+gzip compressed data, was "btrack-0.5.2.tar", last modified: Tue Apr  4 15:42:59 2023, max compression
```

## Comparing `btrack-0.5.1.tar` & `btrack-0.5.2.tar`

### file list

```diff
@@ -1,146 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.268341 btrack-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.268341 btrack-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-03 15:43:21.000000 btrack-0.5.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-03 15:43:21.000000 btrack-0.5.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-03 15:43:21.000000 btrack-0.5.1/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-03 15:43:21.000000 btrack-0.5.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-03 15:43:21.000000 btrack-0.5.1/.github/workflows/update_project_board.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-03 15:43:21.000000 btrack-0.5.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.268341 btrack-0.5.1/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-03 15:43:21.000000 btrack-0.5.1/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-03 15:43:21.000000 btrack-0.5.1/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-03 15:43:21.000000 btrack-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 15:43:21.000000 btrack-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-03 15:43:21.000000 btrack-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-03 15:43:21.000000 btrack-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-03 15:43:21.000000 btrack-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-03 15:43:36.280341 btrack-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-03 15:43:21.000000 btrack-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.272341 btrack-0.5.1/btrack/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/btypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/dataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.272341 btrack-0.5.1/btrack/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/bayes.h
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/belief.h
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/hyperbin.h
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/hypothesis.h
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/inference.h
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/manager.h
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/motion.h
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/tracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/tracklet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/updates.h
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/include/wrapper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.272341 btrack-0.5.1/btrack/io/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/libwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/btrack/napari/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/btrack/napari/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/examples/show_btrack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/btrack/napari/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/create_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari/widgets/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/btrack/optimise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/optimise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/optimise/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/optimise/optimiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/btrack/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/bayes.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/belief.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/hyperbin.cc
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/hypothesis.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/inference.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/interface.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/manager.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/motion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/tracker.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/tracklet.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/src/wrapper.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-04-03 15:43:21.000000 btrack-0.5.1/btrack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.272341 btrack-0.5.1/btrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-03 15:43:36.000000 btrack-0.5.1/btrack.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      348 2023-04-03 15:43:21.000000 btrack-0.5.1/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-03 15:43:21.000000 btrack-0.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/_static/btrack_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.276341 btrack-0.5.1/docs/dev_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/dev_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/large_datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/napari.rst
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/saving_tracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/simple_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-03 15:43:21.000000 btrack-0.5.1/docs/user_guide/using_features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-03 15:43:21.000000 btrack-0.5.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-03 15:43:21.000000 btrack-0.5.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   371913 2023-04-03 15:43:21.000000 btrack-0.5.1/examples/example_tracking_pipeline-features.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    46379 2023-04-03 15:43:21.000000 btrack-0.5.1/examples/example_tracking_pipeline.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-03 15:43:21.000000 btrack-0.5.1/models/cell_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-03 15:43:21.000000 btrack-0.5.1/models/cell_config_flat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-03 15:43:21.000000 btrack-0.5.1/models/particle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-03 15:43:21.000000 btrack-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-03 15:43:21.000000 btrack-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:43:36.280341 btrack-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/tests/_test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/_test_data/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/_test_data/test_graph.json
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/_test_data/test_ground_truth.json
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:43:36.280341 btrack-0.5.1/tests/napari/
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/napari/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/napari/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_tracklets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-03 15:43:21.000000 btrack-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.159651 btrack-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.127651 btrack-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.131651 btrack-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-04 15:42:41.000000 btrack-0.5.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-04 15:42:41.000000 btrack-0.5.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-04 15:42:41.000000 btrack-0.5.2/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-04 15:42:41.000000 btrack-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-04 15:42:41.000000 btrack-0.5.2/.github/workflows/update_project_board.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-04 15:42:41.000000 btrack-0.5.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.131651 btrack-0.5.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-04 15:42:41.000000 btrack-0.5.2/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-04 15:42:41.000000 btrack-0.5.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-04 15:42:41.000000 btrack-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-04 15:42:41.000000 btrack-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-04 15:42:41.000000 btrack-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-04 15:42:41.000000 btrack-0.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 15:42:41.000000 btrack-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-04 15:42:41.000000 btrack-0.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-04 15:42:59.155651 btrack-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-04 15:42:41.000000 btrack-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.135651 btrack-0.5.2/btrack/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 15:42:58.000000 btrack-0.5.2/btrack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/btypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.139651 btrack-0.5.2/btrack/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/bayes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/belief.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/hyperbin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/hypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/inference.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/motion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/tracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/tracklet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/updates.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/include/wrapper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.139651 btrack-0.5.2/btrack/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.143651 btrack-0.5.2/btrack/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)  3326687 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/libs/libtracker.DLL
+-rw-r--r--   0 runner    (1001) docker     (123)   909869 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/libs/libtracker.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)   554624 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/libs/libtracker.so
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/libwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.147651 btrack-0.5.2/btrack/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.147651 btrack-0.5.2/btrack/napari/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/examples/show_btrack_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.147651 btrack-0.5.2/btrack/napari/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/create_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari/widgets/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.147651 btrack-0.5.2/btrack/optimise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/optimise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/optimise/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/optimise/optimiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.151651 btrack-0.5.2/btrack/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/bayes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/belief.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/hyperbin.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/hypothesis.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/inference.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/interface.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/manager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/motion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/tracker.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/tracklet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/src/wrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-04-04 15:42:41.000000 btrack-0.5.2/btrack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.135651 btrack-0.5.2/btrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 15:42:59.000000 btrack-0.5.2/btrack.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      348 2023-04-04 15:42:41.000000 btrack-0.5.2/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 15:42:41.000000 btrack-0.5.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.151651 btrack-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.151651 btrack-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/_static/btrack_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.151651 btrack-0.5.2/docs/dev_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/dev_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.151651 btrack-0.5.2/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/large_datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/napari.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/saving_tracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/simple_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-04 15:42:41.000000 btrack-0.5.2/docs/user_guide/using_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-04 15:42:41.000000 btrack-0.5.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.155651 btrack-0.5.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-04 15:42:41.000000 btrack-0.5.2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   371913 2023-04-04 15:42:41.000000 btrack-0.5.2/examples/example_tracking_pipeline-features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    46379 2023-04-04 15:42:41.000000 btrack-0.5.2/examples/example_tracking_pipeline.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.155651 btrack-0.5.2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-04 15:42:41.000000 btrack-0.5.2/models/cell_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-04 15:42:41.000000 btrack-0.5.2/models/cell_config_flat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-04 15:42:41.000000 btrack-0.5.2/models/particle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-04 15:42:41.000000 btrack-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-04 15:42:41.000000 btrack-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:42:59.159651 btrack-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.155651 btrack-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.155651 btrack-0.5.2/tests/_test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/_test_data/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/_test_data/test_graph.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/_test_data/test_ground_truth.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:42:59.155651 btrack-0.5.2/tests/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/napari/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/napari/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_tracklets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-04 15:42:41.000000 btrack-0.5.2/tests/test_utils.py
```

### Comparing `btrack-0.5.1/.github/workflows/deploy.yml` & `btrack-0.5.2/.github/workflows/deploy.yml`

 * *Files 16% similar despite different names*

```diff
@@ -65,11 +65,17 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install build
 
       - name: Build distributions
         run: python -m build
 
+      - name: Publish package to TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.TESTPYPI_SECRET }}
+          repository-url: https://test.pypi.org/legacy/
+
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `btrack-0.5.1/.github/workflows/linting.yml` & `btrack-0.5.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/.github/workflows/napari-hub-preview.yml` & `btrack-0.5.2/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/.github/workflows/test.yml` & `btrack-0.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/.gitignore` & `btrack-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/.napari-hub/DESCRIPTION.md` & `btrack-0.5.2/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/.pre-commit-config.yaml` & `btrack-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/CHANGELOG.rst` & `btrack-0.5.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/LICENSE.md` & `btrack-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/Makefile` & `btrack-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/PKG-INFO` & `btrack-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrack
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework for Bayesian multi-object tracking
 Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2017 Alan R. Lowe (quantumjot)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -53,21 +53,17 @@
 [![Downloads](https://pepy.tech/badge/btrack/month)](https://pepy.tech/project/btrack)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tests](https://github.com/quantumjot/btrack/actions/workflows/test.yml/badge.svg)](https://github.com/quantumjot/btrack/actions/workflows/test.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Documentation](https://readthedocs.org/projects/btrack/badge/?version=latest)](https://btrack.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/quantumjot/btrack/branch/main/graph/badge.svg?token=QCFC9AWK0R)](https://codecov.io/gh/quantumjot/btrack)
 
-[docs]: https://btrack.readthedocs.io/en/latest/
-[docs-dev]: https://btrack.readthedocs.io/en/latest/dev_guide/
-[cellx]: http://lowe.cs.ucl.ac.uk/cellx.html
+![logo](https://btrack.readthedocs.io/en/latest/_images/btrack_logo.png)
 
-![logo](./docs/_static/btrack_logo.png)
-
-# Bayesian Tracker (btrack) :microscope::computer:
+# Bayesian Tracker (btrack) 🔬💻
 
 `btrack` is a Python library for multi object tracking, used to reconstruct trajectories in crowded fields.
 Here, we use a probabilistic network of information to perform the trajectory linking.
 This method uses spatial information as well as appearance information for track linking.
 
 The tracking algorithm assembles reliable sections of track that do not contain splitting events (tracklets).
 Each new tracklet initiates a probabilistic model, and utilises this to predict future states (and error in states) of each of the objects in the field of view.
@@ -75,18 +71,14 @@
 
 The tracklets are then assembled into tracks by using multiple hypothesis testing and integer programming to identify a globally optimal solution.
 The likelihood of each hypothesis is calculated for some or all of the tracklets based on heuristics.
 The global solution identifies a sequence of high-likelihood hypotheses that accounts for all observations.
 
 We developed `btrack` for cell tracking in time-lapse microscopy data.
 
-[Read more about the science][cellx].
-
-You can also --> :star: :wink:
-
 ## Installation
 
 `btrack` has been tested with Python 3.8+ on OS X, Linux and Win10.
 
 
 #### Installing the latest stable version
 
@@ -102,15 +94,15 @@
 conda env create -f environment.yml
 conda activate btrack
 pip install btrack
 ```
 
 ## Usage examples
 
-Visit [btrack documentation][docs] to learn how to use it and see other examples.
+Visit [btrack documentation](https://btrack.readthedocs.io) to learn how to use it and see other examples.
 
 ### Cell tracking in time-lapse imaging data
 
  We provide integration with Napari, including a plugin for graph visualization, [arboretum](https://btrack.readthedocs.io/en/latest/user_guide/napari.html).
 
 
 [![CellTracking](http://lowe.cs.ucl.ac.uk/images/youtube.png)](https://youtu.be/EjqluvrJGCg)  
@@ -121,15 +113,15 @@
 
 
 ---
 
 ## Development
 
 The tracker and hypothesis engine are mostly written in C++ with a Python wrapper.
-If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide][docs-dev].
+If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide](https://btrack.readthedocs.io/en/latest/dev_guide).
 
 
 ---
 ### Citation
 
 More details of how this type of tracking approach can be applied to tracking cells in time-lapse microscopy data can be found in the following publications:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `btrack-0.5.1/README.md` & `btrack-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 [![Downloads](https://pepy.tech/badge/btrack/month)](https://pepy.tech/project/btrack)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tests](https://github.com/quantumjot/btrack/actions/workflows/test.yml/badge.svg)](https://github.com/quantumjot/btrack/actions/workflows/test.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Documentation](https://readthedocs.org/projects/btrack/badge/?version=latest)](https://btrack.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/quantumjot/btrack/branch/main/graph/badge.svg?token=QCFC9AWK0R)](https://codecov.io/gh/quantumjot/btrack)
 
-[docs]: https://btrack.readthedocs.io/en/latest/
-[docs-dev]: https://btrack.readthedocs.io/en/latest/dev_guide/
-[cellx]: http://lowe.cs.ucl.ac.uk/cellx.html
+![logo](https://btrack.readthedocs.io/en/latest/_images/btrack_logo.png)
 
-![logo](./docs/_static/btrack_logo.png)
-
-# Bayesian Tracker (btrack) :microscope::computer:
+# Bayesian Tracker (btrack) 🔬💻
 
 `btrack` is a Python library for multi object tracking, used to reconstruct trajectories in crowded fields.
 Here, we use a probabilistic network of information to perform the trajectory linking.
 This method uses spatial information as well as appearance information for track linking.
 
 The tracking algorithm assembles reliable sections of track that do not contain splitting events (tracklets).
 Each new tracklet initiates a probabilistic model, and utilises this to predict future states (and error in states) of each of the objects in the field of view.
@@ -24,18 +20,14 @@
 
 The tracklets are then assembled into tracks by using multiple hypothesis testing and integer programming to identify a globally optimal solution.
 The likelihood of each hypothesis is calculated for some or all of the tracklets based on heuristics.
 The global solution identifies a sequence of high-likelihood hypotheses that accounts for all observations.
 
 We developed `btrack` for cell tracking in time-lapse microscopy data.
 
-[Read more about the science][cellx].
-
-You can also --> :star: :wink:
-
 ## Installation
 
 `btrack` has been tested with Python 3.8+ on OS X, Linux and Win10.
 
 
 #### Installing the latest stable version
 
@@ -51,15 +43,15 @@
 conda env create -f environment.yml
 conda activate btrack
 pip install btrack
 ```
 
 ## Usage examples
 
-Visit [btrack documentation][docs] to learn how to use it and see other examples.
+Visit [btrack documentation](https://btrack.readthedocs.io) to learn how to use it and see other examples.
 
 ### Cell tracking in time-lapse imaging data
 
  We provide integration with Napari, including a plugin for graph visualization, [arboretum](https://btrack.readthedocs.io/en/latest/user_guide/napari.html).
 
 
 [![CellTracking](http://lowe.cs.ucl.ac.uk/images/youtube.png)](https://youtu.be/EjqluvrJGCg)  
@@ -70,15 +62,15 @@
 
 
 ---
 
 ## Development
 
 The tracker and hypothesis engine are mostly written in C++ with a Python wrapper.
-If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide][docs-dev].
+If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide](https://btrack.readthedocs.io/en/latest/dev_guide).
 
 
 ---
 ### Citation
 
 More details of how this type of tracking approach can be applied to tracking cells in time-lapse microscopy data can be found in the following publications:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `btrack-0.5.1/btrack/__init__.py` & `btrack-0.5.2/btrack/__init__.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/btypes.py` & `btrack-0.5.2/btrack/btypes.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/config.py` & `btrack-0.5.2/btrack/config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/constants.py` & `btrack-0.5.2/btrack/constants.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/core.py` & `btrack-0.5.2/btrack/core.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/datasets.py` & `btrack-0.5.2/btrack/datasets.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/bayes.h` & `btrack-0.5.2/btrack/include/bayes.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/belief.h` & `btrack-0.5.2/btrack/include/belief.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/defs.h` & `btrack-0.5.2/btrack/include/defs.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/hyperbin.h` & `btrack-0.5.2/btrack/include/hyperbin.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/hypothesis.h` & `btrack-0.5.2/btrack/include/hypothesis.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/inference.h` & `btrack-0.5.2/btrack/include/inference.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/manager.h` & `btrack-0.5.2/btrack/include/manager.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/motion.h` & `btrack-0.5.2/btrack/include/motion.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/pdf.h` & `btrack-0.5.2/btrack/include/pdf.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/tracker.h` & `btrack-0.5.2/btrack/include/tracker.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/tracklet.h` & `btrack-0.5.2/btrack/include/tracklet.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/types.h` & `btrack-0.5.2/btrack/include/types.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/updates.h` & `btrack-0.5.2/btrack/include/updates.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/include/wrapper.h` & `btrack-0.5.2/btrack/include/wrapper.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/io/_localization.py` & `btrack-0.5.2/btrack/io/_localization.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/io/exporters.py` & `btrack-0.5.2/btrack/io/exporters.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/io/hdf.py` & `btrack-0.5.2/btrack/io/hdf.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/io/importers.py` & `btrack-0.5.2/btrack/io/importers.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/io/utils.py` & `btrack-0.5.2/btrack/io/utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/libwrapper.py` & `btrack-0.5.2/btrack/libwrapper.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/models.py` & `btrack-0.5.2/btrack/models.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/config.py` & `btrack-0.5.2/btrack/napari/config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/examples/show_btrack_widget.py` & `btrack-0.5.2/btrack/napari/examples/show_btrack_widget.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/main.py` & `btrack-0.5.2/btrack/napari/main.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/reader.py` & `btrack-0.5.2/btrack/napari/reader.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/sync.py` & `btrack-0.5.2/btrack/napari/sync.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/widgets/_general.py` & `btrack-0.5.2/btrack/napari/widgets/_general.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/widgets/_hypothesis.py` & `btrack-0.5.2/btrack/napari/widgets/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/widgets/_motion.py` & `btrack-0.5.2/btrack/napari/widgets/_motion.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/widgets/create_ui.py` & `btrack-0.5.2/btrack/napari/widgets/create_ui.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/napari/widgets/io.py` & `btrack-0.5.2/btrack/napari/widgets/io.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/optimise/hypothesis.py` & `btrack-0.5.2/btrack/optimise/hypothesis.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/optimise/optimiser.py` & `btrack-0.5.2/btrack/optimise/optimiser.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/bayes.cc` & `btrack-0.5.2/btrack/src/bayes.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/belief.cu` & `btrack-0.5.2/btrack/src/belief.cu`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/hyperbin.cc` & `btrack-0.5.2/btrack/src/hyperbin.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/hypothesis.cc` & `btrack-0.5.2/btrack/src/hypothesis.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/inference.cc` & `btrack-0.5.2/btrack/src/inference.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/interface.cc` & `btrack-0.5.2/btrack/src/interface.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/manager.cc` & `btrack-0.5.2/btrack/src/manager.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/motion.cc` & `btrack-0.5.2/btrack/src/motion.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/pdf.cc` & `btrack-0.5.2/btrack/src/pdf.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/tracker.cc` & `btrack-0.5.2/btrack/src/tracker.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/tracklet.cc` & `btrack-0.5.2/btrack/src/tracklet.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/src/wrapper.cc` & `btrack-0.5.2/btrack/src/wrapper.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack/utils.py` & `btrack-0.5.2/btrack/utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/btrack.egg-info/PKG-INFO` & `btrack-0.5.2/btrack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrack
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework for Bayesian multi-object tracking
 Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2017 Alan R. Lowe (quantumjot)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -53,21 +53,17 @@
 [![Downloads](https://pepy.tech/badge/btrack/month)](https://pepy.tech/project/btrack)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tests](https://github.com/quantumjot/btrack/actions/workflows/test.yml/badge.svg)](https://github.com/quantumjot/btrack/actions/workflows/test.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Documentation](https://readthedocs.org/projects/btrack/badge/?version=latest)](https://btrack.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/quantumjot/btrack/branch/main/graph/badge.svg?token=QCFC9AWK0R)](https://codecov.io/gh/quantumjot/btrack)
 
-[docs]: https://btrack.readthedocs.io/en/latest/
-[docs-dev]: https://btrack.readthedocs.io/en/latest/dev_guide/
-[cellx]: http://lowe.cs.ucl.ac.uk/cellx.html
+![logo](https://btrack.readthedocs.io/en/latest/_images/btrack_logo.png)
 
-![logo](./docs/_static/btrack_logo.png)
-
-# Bayesian Tracker (btrack) :microscope::computer:
+# Bayesian Tracker (btrack) 🔬💻
 
 `btrack` is a Python library for multi object tracking, used to reconstruct trajectories in crowded fields.
 Here, we use a probabilistic network of information to perform the trajectory linking.
 This method uses spatial information as well as appearance information for track linking.
 
 The tracking algorithm assembles reliable sections of track that do not contain splitting events (tracklets).
 Each new tracklet initiates a probabilistic model, and utilises this to predict future states (and error in states) of each of the objects in the field of view.
@@ -75,18 +71,14 @@
 
 The tracklets are then assembled into tracks by using multiple hypothesis testing and integer programming to identify a globally optimal solution.
 The likelihood of each hypothesis is calculated for some or all of the tracklets based on heuristics.
 The global solution identifies a sequence of high-likelihood hypotheses that accounts for all observations.
 
 We developed `btrack` for cell tracking in time-lapse microscopy data.
 
-[Read more about the science][cellx].
-
-You can also --> :star: :wink:
-
 ## Installation
 
 `btrack` has been tested with Python 3.8+ on OS X, Linux and Win10.
 
 
 #### Installing the latest stable version
 
@@ -102,15 +94,15 @@
 conda env create -f environment.yml
 conda activate btrack
 pip install btrack
 ```
 
 ## Usage examples
 
-Visit [btrack documentation][docs] to learn how to use it and see other examples.
+Visit [btrack documentation](https://btrack.readthedocs.io) to learn how to use it and see other examples.
 
 ### Cell tracking in time-lapse imaging data
 
  We provide integration with Napari, including a plugin for graph visualization, [arboretum](https://btrack.readthedocs.io/en/latest/user_guide/napari.html).
 
 
 [![CellTracking](http://lowe.cs.ucl.ac.uk/images/youtube.png)](https://youtu.be/EjqluvrJGCg)  
@@ -121,15 +113,15 @@
 
 
 ---
 
 ## Development
 
 The tracker and hypothesis engine are mostly written in C++ with a Python wrapper.
-If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide][docs-dev].
+If you would like to contribute to btrack, you will need to install the latest version from GitHub. Follow the [instructions on our developer guide](https://btrack.readthedocs.io/en/latest/dev_guide).
 
 
 ---
 ### Citation
 
 More details of how this type of tracking approach can be applied to tracking cells in time-lapse microscopy data can be found in the following publications:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `btrack-0.5.1/btrack.egg-info/SOURCES.txt` & `btrack-0.5.2/btrack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.rst
 LICENSE.md
+MANIFEST.in
 Makefile
 README.md
 build.sh
 codecov.yml
 environment.yml
 pyproject.toml
 requirements.txt
@@ -51,14 +52,17 @@
 btrack/include/wrapper.h
 btrack/io/__init__.py
 btrack/io/_localization.py
 btrack/io/exporters.py
 btrack/io/hdf.py
 btrack/io/importers.py
 btrack/io/utils.py
+btrack/libs/libtracker.DLL
+btrack/libs/libtracker.dylib
+btrack/libs/libtracker.so
 btrack/napari/__init__.py
 btrack/napari/config.py
 btrack/napari/constants.py
 btrack/napari/main.py
 btrack/napari/reader.py
 btrack/napari/sync.py
 btrack/napari/examples/show_btrack_widget.py
```

### Comparing `btrack-0.5.1/docs/Makefile` & `btrack-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/_static/btrack_logo.png` & `btrack-0.5.2/docs/_static/btrack_logo.png`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/about.rst` & `btrack-0.5.2/docs/about.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/conf.py` & `btrack-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/dev_guide/index.rst` & `btrack-0.5.2/docs/dev_guide/index.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/index.rst` & `btrack-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/make.bat` & `btrack-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/configuration.rst` & `btrack-0.5.2/docs/user_guide/configuration.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/installation.rst` & `btrack-0.5.2/docs/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/large_datasets.rst` & `btrack-0.5.2/docs/user_guide/large_datasets.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/napari.rst` & `btrack-0.5.2/docs/user_guide/napari.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/saving_tracks.rst` & `btrack-0.5.2/docs/user_guide/saving_tracks.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/simple_example.rst` & `btrack-0.5.2/docs/user_guide/simple_example.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/docs/user_guide/using_features.rst` & `btrack-0.5.2/docs/user_guide/using_features.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/examples/example_tracking_pipeline-features.ipynb` & `btrack-0.5.2/examples/example_tracking_pipeline-features.ipynb`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/examples/example_tracking_pipeline.ipynb` & `btrack-0.5.2/examples/example_tracking_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/models/cell_config.json` & `btrack-0.5.2/models/cell_config.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/models/cell_config_flat.json` & `btrack-0.5.2/models/cell_config_flat.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/models/particle_config.json` & `btrack-0.5.2/models/particle_config.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/pyproject.toml` & `btrack-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 ]
 
 [tool.setuptools]
 dynamic.dependencies.file = "requirements.txt"
 packages.find = {}
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
 write_to = "btrack/_version.py"
 
 [tool.tomlsort]
 sort_inline_arrays = false
 sort_inline_tables = true
 sort_table_keys = true
 spaces_indent_inline_array = 4
```

### Comparing `btrack-0.5.1/tests/_test_data/test_data.csv` & `btrack-0.5.2/tests/_test_data/test_data.csv`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/_test_data/test_ground_truth.json` & `btrack-0.5.2/tests/_test_data/test_ground_truth.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/_utils.py` & `btrack-0.5.2/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/conftest.py` & `btrack-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/napari/test_dock_widget.py` & `btrack-0.5.2/tests/napari/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_config.py` & `btrack-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_io.py` & `btrack-0.5.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_models.py` & `btrack-0.5.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_tracker.py` & `btrack-0.5.2/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_tracklets.py` & `btrack-0.5.2/tests/test_tracklets.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.1/tests/test_utils.py` & `btrack-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

