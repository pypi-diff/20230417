# Comparing `tmp/btrack-0.5.4.tar.gz` & `tmp/btrack-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrack-0.5.4.tar", last modified: Mon Apr 17 14:42:12 2023, max compression
+gzip compressed data, was "btrack-0.5.5.tar", last modified: Mon Apr 17 14:48:20 2023, max compression
```

## Comparing `btrack-0.5.4.tar` & `btrack-0.5.5.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.853804 btrack-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.857804 btrack-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-17 14:42:01.000000 btrack-0.5.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-17 14:42:01.000000 btrack-0.5.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 14:42:01.000000 btrack-0.5.4/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-17 14:42:01.000000 btrack-0.5.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 14:42:01.000000 btrack-0.5.4/.github/workflows/update_project_board.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 14:42:01.000000 btrack-0.5.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.857804 btrack-0.5.4/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-17 14:42:01.000000 btrack-0.5.4/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 14:42:01.000000 btrack-0.5.4/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 14:42:01.000000 btrack-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 14:42:01.000000 btrack-0.5.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-17 14:42:01.000000 btrack-0.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 14:42:01.000000 btrack-0.5.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:42:01.000000 btrack-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-17 14:42:01.000000 btrack-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-17 14:42:12.869804 btrack-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-17 14:42:01.000000 btrack-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.857804 btrack-0.5.4/btrack/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/btypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/dataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/bayes.h
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/belief.h
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/hyperbin.h
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/hypothesis.h
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/inference.h
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/manager.h
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/motion.h
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/tracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/tracklet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/updates.h
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/include/wrapper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack/io/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack/libs/
--rw-r--r--   0 runner    (1001) docker     (123)   554624 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/libs/libtracker.so
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/libwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack/napari/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack/napari/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/examples/show_btrack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/btrack/napari/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/create_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari/widgets/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/btrack/optimise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/optimise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/optimise/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/optimise/optimiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/btrack/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/bayes.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/belief.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/hyperbin.cc
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/hypothesis.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/inference.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/interface.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/manager.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/motion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/tracker.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/tracklet.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/src/wrapper.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-04-17 14:42:01.000000 btrack-0.5.4/btrack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.861804 btrack-0.5.4/btrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 14:42:12.000000 btrack-0.5.4/btrack.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      348 2023-04-17 14:42:01.000000 btrack-0.5.4/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 14:42:01.000000 btrack-0.5.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/_static/btrack_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/docs/dev_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/dev_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.865804 btrack-0.5.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/large_datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/napari.rst
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/saving_tracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/simple_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 14:42:01.000000 btrack-0.5.4/docs/user_guide/using_features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 14:42:01.000000 btrack-0.5.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 14:42:01.000000 btrack-0.5.4/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   371913 2023-04-17 14:42:01.000000 btrack-0.5.4/examples/example_tracking_pipeline-features.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    46379 2023-04-17 14:42:01.000000 btrack-0.5.4/examples/example_tracking_pipeline.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-17 14:42:01.000000 btrack-0.5.4/models/cell_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-17 14:42:01.000000 btrack-0.5.4/models/cell_config_flat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 14:42:01.000000 btrack-0.5.4/models/particle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-17 14:42:01.000000 btrack-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 14:42:01.000000 btrack-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:42:12.869804 btrack-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/tests/_test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/_test_data/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/_test_data/test_graph.json
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/_test_data/test_ground_truth.json
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:12.869804 btrack-0.5.4/tests/napari/
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/napari/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/napari/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_tracklets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-17 14:42:01.000000 btrack-0.5.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.231222 btrack-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.203221 btrack-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.207222 btrack-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-17 14:48:04.000000 btrack-0.5.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-17 14:48:04.000000 btrack-0.5.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 14:48:04.000000 btrack-0.5.5/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-17 14:48:04.000000 btrack-0.5.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 14:48:04.000000 btrack-0.5.5/.github/workflows/update_project_board.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 14:48:04.000000 btrack-0.5.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.207222 btrack-0.5.5/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-17 14:48:04.000000 btrack-0.5.5/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 14:48:04.000000 btrack-0.5.5/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 14:48:04.000000 btrack-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 14:48:04.000000 btrack-0.5.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-17 14:48:04.000000 btrack-0.5.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 14:48:04.000000 btrack-0.5.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:48:04.000000 btrack-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-17 14:48:04.000000 btrack-0.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-17 14:48:20.231222 btrack-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-17 14:48:04.000000 btrack-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.211222 btrack-0.5.5/btrack/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/btypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.215222 btrack-0.5.5/btrack/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/bayes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/belief.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/hyperbin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/hypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/inference.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/motion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/tracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/tracklet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/updates.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/include/wrapper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.215222 btrack-0.5.5/btrack/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.215222 btrack-0.5.5/btrack/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)   554624 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/libs/libtracker.so
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/libwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.219221 btrack-0.5.5/btrack/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.219221 btrack-0.5.5/btrack/napari/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/examples/show_btrack_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.219221 btrack-0.5.5/btrack/napari/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/create_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari/widgets/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.219221 btrack-0.5.5/btrack/optimise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/optimise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/optimise/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/optimise/optimiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.223222 btrack-0.5.5/btrack/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/bayes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/belief.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/hyperbin.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/hypothesis.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/inference.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/interface.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/manager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/motion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/tracker.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/tracklet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/src/wrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-04-17 14:48:04.000000 btrack-0.5.5/btrack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.211222 btrack-0.5.5/btrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 14:48:20.000000 btrack-0.5.5/btrack.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      348 2023-04-17 14:48:04.000000 btrack-0.5.5/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 14:48:04.000000 btrack-0.5.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.223222 btrack-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.223222 btrack-0.5.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/_static/btrack_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.223222 btrack-0.5.5/docs/dev_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/dev_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.227222 btrack-0.5.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/large_datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/napari.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/saving_tracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/simple_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 14:48:04.000000 btrack-0.5.5/docs/user_guide/using_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 14:48:04.000000 btrack-0.5.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.227222 btrack-0.5.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 14:48:04.000000 btrack-0.5.5/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   371913 2023-04-17 14:48:04.000000 btrack-0.5.5/examples/example_tracking_pipeline-features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    46379 2023-04-17 14:48:04.000000 btrack-0.5.5/examples/example_tracking_pipeline.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.227222 btrack-0.5.5/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-17 14:48:04.000000 btrack-0.5.5/models/cell_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-17 14:48:04.000000 btrack-0.5.5/models/cell_config_flat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 14:48:04.000000 btrack-0.5.5/models/particle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-17 14:48:04.000000 btrack-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 14:48:04.000000 btrack-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:48:20.231222 btrack-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.231222 btrack-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.231222 btrack-0.5.5/tests/_test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/_test_data/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/_test_data/test_graph.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/_test_data/test_ground_truth.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:48:20.231222 btrack-0.5.5/tests/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/napari/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/napari/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_tracklets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-17 14:48:04.000000 btrack-0.5.5/tests/test_utils.py
```

### Comparing `btrack-0.5.4/.github/workflows/deploy.yml` & `btrack-0.5.5/.github/workflows/deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,20 @@
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TESTPYPI_SECRET }}
           repository-url: https://test.pypi.org/legacy/
 
   verify-testpypi-contains-binary:
     needs: deploy-to-testpypi
-    runs-on: "ubuntu-latest"
+    name: ${{ matrix.os }}
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v4
         with:
```

### Comparing `btrack-0.5.4/.github/workflows/linting.yml` & `btrack-0.5.5/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/.github/workflows/napari-hub-preview.yml` & `btrack-0.5.5/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/.github/workflows/test.yml` & `btrack-0.5.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/.gitignore` & `btrack-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/.napari-hub/DESCRIPTION.md` & `btrack-0.5.5/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/.pre-commit-config.yaml` & `btrack-0.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/CHANGELOG.rst` & `btrack-0.5.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/LICENSE.md` & `btrack-0.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/Makefile` & `btrack-0.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/PKG-INFO` & `btrack-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrack
-Version: 0.5.4
+Version: 0.5.5
 Summary: A framework for Bayesian multi-object tracking
 Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2017 Alan R. Lowe (quantumjot)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `btrack-0.5.4/README.md` & `btrack-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/__init__.py` & `btrack-0.5.5/btrack/__init__.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/btypes.py` & `btrack-0.5.5/btrack/btypes.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/config.py` & `btrack-0.5.5/btrack/config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/constants.py` & `btrack-0.5.5/btrack/constants.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/core.py` & `btrack-0.5.5/btrack/core.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/datasets.py` & `btrack-0.5.5/btrack/datasets.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/bayes.h` & `btrack-0.5.5/btrack/include/bayes.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/belief.h` & `btrack-0.5.5/btrack/include/belief.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/defs.h` & `btrack-0.5.5/btrack/include/defs.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/hyperbin.h` & `btrack-0.5.5/btrack/include/hyperbin.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/hypothesis.h` & `btrack-0.5.5/btrack/include/hypothesis.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/inference.h` & `btrack-0.5.5/btrack/include/inference.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/manager.h` & `btrack-0.5.5/btrack/include/manager.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/motion.h` & `btrack-0.5.5/btrack/include/motion.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/pdf.h` & `btrack-0.5.5/btrack/include/pdf.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/tracker.h` & `btrack-0.5.5/btrack/include/tracker.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/tracklet.h` & `btrack-0.5.5/btrack/include/tracklet.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/types.h` & `btrack-0.5.5/btrack/include/types.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/updates.h` & `btrack-0.5.5/btrack/include/updates.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/include/wrapper.h` & `btrack-0.5.5/btrack/include/wrapper.h`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/io/_localization.py` & `btrack-0.5.5/btrack/io/_localization.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/io/exporters.py` & `btrack-0.5.5/btrack/io/exporters.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/io/hdf.py` & `btrack-0.5.5/btrack/io/hdf.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/io/importers.py` & `btrack-0.5.5/btrack/io/importers.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/io/utils.py` & `btrack-0.5.5/btrack/io/utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/libs/libtracker.so` & `btrack-0.5.5/btrack/libs/libtracker.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: f0251693656294cd2b03c917ce763d8c367a6771
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 89b08361d7c14f5f5604d524ed218688f16c7ac7
```

#### strings --all --bytes=8 {}

```diff
@@ -713,30 +713,30 @@
 []A\A]A^A_
 ]A\A]A^A_
 []A\A]A^A_
 []A\A]A^
 B}Tbasic_string::_M_construct null not valid
 vector::_M_realloc_insert
 Apr 17 2023
-14:40:40
+14:46:35
 0Cunsigned int count_state_track(TrackletPtr, unsigned int, bool)
 double Tracklet::duration() const
 double HypothesisEngine::P_dead(TrackletPtr, unsigned int) const
 p_apoptosis >= 0. && p_apoptosis <= 1.
 double HypothesisEngine::P_link(TrackletPtr, TrackletPtr, float, float) const
 HypothesisEngine::HypothesisEngine(unsigned int, unsigned int, const PyHypothesisParams&, TrackManager*)
 m_params.segmentation_miss_rate >= 0.0 && m_params.segmentation_miss_rate <= 1.0
 m_params.apoptosis_rate >= 0.0 && m_params.apoptosis_rate <= 1.0
 btrack/src/hypothesis.cc
 a_trk->length() > 0
 ./btrack/include/tracklet.h
 !track.empty()
 dt > 0.0
 Resetting hypothesis engine.
-14:40:42
+14:46:37
 void* Eigen::internal::aligned_malloc(std::size_t)
 ./btrack/include/eigen/Eigen/src/Core/util/Memory.h
 (size<16 || (std::size_t(result)%16)==0) && "System's malloc returned an unaligned pointer. Compile with EIGEN_MALLOC_ALREADY_ALIGNED=0 to fallback to handmade aligned memory allocator."
 constexpr void Eigen::PlainObjectBase<Derived>::resize(Eigen::Index, Eigen::Index) [with Derived = Eigen::Matrix<double, -1, 1>; Eigen::Index = long int]
 ./btrack/include/eigen/Eigen/src/Core/PlainObjectBase.h
 internal::check_implication(RowsAtCompileTime!=Dynamic, rows==RowsAtCompileTime) && internal::check_implication(ColsAtCompileTime!=Dynamic, cols==ColsAtCompileTime) && internal::check_implication(RowsAtCompileTime==Dynamic && MaxRowsAtCompileTime!=Dynamic, rows<=MaxRowsAtCompileTime) && internal::check_implication(ColsAtCompileTime==Dynamic && MaxColsAtCompileTime!=Dynamic, cols<=MaxColsAtCompileTime) && rows>=0 && cols>=0 && "Invalid sizes when resizing a matrix or array."
 Eigen::DenseCoeffsBase<Derived, 1>::Scalar& Eigen::DenseCoeffsBase<Derived, 1>::operator()(Eigen::Index) [with Derived = Eigen::Matrix<double, -1, 1>; Eigen::DenseCoeffsBase<Derived, 1>::Scalar = double; Eigen::Index = long int]
@@ -759,23 +759,23 @@
 ./btrack/include/eigen/Eigen/src/Core/Product.h
 lhs.cols() == rhs.rows() && "invalid matrix product" && "if you wanted a coeff-wise or a dot product use the respective explicit functions"
 constexpr void Eigen::PlainObjectBase<Derived>::resize(Eigen::Index, Eigen::Index) [with Derived = Eigen::Matrix<double, -1, -1>; Eigen::Index = long int]
 void Eigen::internal::resize_if_allowed(DstXprType&, const SrcXprType&, const Eigen::internal::assign_op<T1, T2>&) [with DstXprType = Eigen::Matrix<double, -1, 1>; SrcXprType = Eigen::Matrix<double, -1, -1>; T1 = double; T2 = double]
 ./btrack/include/eigen/Eigen/src/Core/AssignEvaluator.h
 dst.rows() == dstRows && dst.cols() == dstCols
 index >= 0 && index < size()
-14:40:46
-14:40:48
+14:46:41
+14:46:43
 Track ID: 
 Track not found.
 btrack/src/manager.cc
 a_idx < 0
 !m_dummies.empty()
 m_dummies[dummy_idx]->dummy
-14:40:51
+14:46:46
 TrackObjectPtr TrackManager::get_dummy(int) const
 void Eigen::internal::gemm_pack_rhs<Scalar, Index, DataMapper, nr, 0, Conjugate, PanelMode>::operator()(Scalar*, const DataMapper&, Index, Index, Index, Index) [with Scalar = double; Index = long int; DataMapper = Eigen::internal::const_blas_data_mapper<double, long int, 0>; int nr = 4; bool Conjugate = false; bool PanelMode = true]
 ./btrack/include/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
 ((!PanelMode) && stride==0 && offset==0) || (PanelMode && stride>=depth && offset<=stride)
 void Eigen::internal::gemm_pack_lhs<Scalar, Index, DataMapper, Pack1, Pack2, Packet, 0, Conjugate, PanelMode>::operator()(Scalar*, const DataMapper&, Index, Index, Index, Index) [with Scalar = double; Index = long int; DataMapper = Eigen::internal::blas_data_mapper<double, long int, 0, 0, 1>; int Pack1 = 4; int Pack2 = 2; Packet = __vector(2) double; bool Conjugate = false; bool PanelMode = true]
 Eigen::internal::blas_data_mapper<Scalar, Index, StorageOrder, AlignmentType, 1>::blas_data_mapper(Scalar*, Index, Index) [with Scalar = double; Index = long int; int StorageOrder = 0; int AlignmentType = 0]
 ./btrack/include/eigen/Eigen/src/Core/util/BlasUtil.h
@@ -827,15 +827,15 @@
 Eigen::Product<Lhs, Rhs, Option>::Product(const Lhs&, const Rhs&) [with Lhs_ = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, -1, -1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0> >; Rhs_ = Eigen::Matrix<double, -1, -1>; int Option = 0; Eigen::Product<Lhs, Rhs, Option>::Lhs = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, -1, -1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0> >; Eigen::Product<Lhs, Rhs, Option>::Rhs = Eigen::Matrix<double, -1, -1>]
 Eigen::Product<Lhs, Rhs, Option>::Product(const Lhs&, const Rhs&) [with Lhs_ = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, -1, -1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0> >; Rhs_ = Eigen::Matrix<double, -1, -1>; int Option = 1; Eigen::Product<Lhs, Rhs, Option>::Lhs = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, -1, -1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0> >; Eigen::Product<Lhs, Rhs, Option>::Rhs = Eigen::Matrix<double, -1, -1>]
 void Eigen::internal::resize_if_allowed(DstXprType&, const SrcXprType&, const Eigen::internal::assign_op<T1, T2>&) [with DstXprType = Eigen::Matrix<double, -1, -1>; SrcXprType = Eigen::Product<Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, -1, -1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0> >, Eigen::Matrix<double, -1, -1>, 1>; T1 = double; T2 = double]
 Eigen::MapBase<Derived, 0>::MapBase(Eigen::MapBase<Derived, 0>::PointerType, Eigen::Index) [with Derived = Eigen::Map<Eigen::Matrix<double, -1, 1>, 2, Eigen::Stride<0, 0> >; Eigen::MapBase<Derived, 0>::PointerType = double*; Eigen::Index = long int]
 vecSize >= 0
 btrack/src/motion.cc
 initialised
-14:40:55
+14:46:50
 Eigen::Product<Lhs, Rhs, Option>::Product(const Lhs&, const Rhs&) [with Lhs_ = Eigen::Matrix<double, -1, -1>; Rhs_ = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, 3, 1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0> >; int Option = 1; Eigen::Product<Lhs, Rhs, Option>::Lhs = Eigen::Matrix<double, -1, -1>; Eigen::Product<Lhs, Rhs, Option>::Rhs = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, 3, 1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0> >]
 static void Eigen::internal::Assignment<DstXprType, Eigen::Product<Lhs, Rhs, Options>, Eigen::internal::sub_assign_op<Scalar, Scalar>, Eigen::internal::Dense2Dense, typename std::enable_if<((Options == Eigen::DefaultProduct) || (Options == Eigen::AliasFreeProduct)), void>::type>::run(DstXprType&, const SrcXprType&, const Eigen::internal::sub_assign_op<Scalar, Scalar>&) [with DstXprType = Eigen::Matrix<double, 3, 1>; Lhs = Eigen::Matrix<double, -1, -1>; Rhs = Eigen::Matrix<double, -1, 1>; int Options = 0; Scalar = double; Eigen::internal::Assignment<DstXprType, Eigen::Product<Lhs, Rhs, Options>, Eigen::internal::sub_assign_op<Scalar, Scalar>, Eigen::internal::Dense2Dense, typename std::enable_if<((Options == Eigen::DefaultProduct) || (Options == Eigen::AliasFreeProduct)), void>::type>::SrcXprType = Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0>]
 ./btrack/include/eigen/Eigen/src/Core/ProductEvaluators.h
 dst.rows() == src.rows() && dst.cols() == src.cols()
 void Eigen::internal::resize_if_allowed(DstXprType&, const SrcXprType&, const Functor&) [with DstXprType = Eigen::Matrix<double, -1, 1>; SrcXprType = Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, 3, 1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0> >, 1>; Functor = Eigen::internal::add_assign_op<double, double>]
 Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::CwiseBinaryOp(const Lhs&, const Rhs&, const BinaryOp&) [with BinaryOp = Eigen::internal::scalar_product_op<double, double>; LhsType = const Eigen::Transpose<const Eigen::Block<const Eigen::Matrix<double, -1, -1>, 1, -1, false> >; RhsType = const Eigen::Block<const Eigen::Matrix<double, 3, 1>, 3, 1, true>; Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::Lhs = Eigen::Transpose<const Eigen::Block<const Eigen::Matrix<double, -1, -1>, 1, -1, false> >; Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::Rhs = Eigen::Block<const Eigen::Matrix<double, 3, 1>, 3, 1, true>]
 static void Eigen::internal::Assignment<DstXprType, Eigen::Product<Lhs, Rhs, Options>, Eigen::internal::add_assign_op<Scalar, Scalar>, Eigen::internal::Dense2Dense, typename std::enable_if<((Options == Eigen::DefaultProduct) || (Options == Eigen::AliasFreeProduct)), void>::type>::run(DstXprType&, const SrcXprType&, const Eigen::internal::add_assign_op<Scalar, Scalar>&) [with DstXprType = Eigen::Matrix<double, -1, 1>; Lhs = Eigen::Matrix<double, -1, -1>; Rhs = Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, 3, 1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0> >; int Options = 0; Scalar = double; Eigen::internal::Assignment<DstXprType, Eigen::Product<Lhs, Rhs, Options>, Eigen::internal::add_assign_op<Scalar, Scalar>, Eigen::internal::Dense2Dense, typename std::enable_if<((Options == Eigen::DefaultProduct) || (Options == Eigen::AliasFreeProduct)), void>::type>::SrcXprType = Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<double, double>, const Eigen::Matrix<double, 3, 1>, const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, 1>, 0> >, 0>]
@@ -946,15 +946,15 @@
 static Eigen::internal::redux_impl<Func, Evaluator, 0, 0>::Scalar Eigen::internal::redux_impl<Func, Evaluator, 0, 0>::run(const Evaluator&, const Func&, const XprType&) [with XprType = Eigen::CwiseBinaryOp<Eigen::internal::scalar_conj_product_op<double, double>, const Eigen::Transpose<const Eigen::Block<const Eigen::Block<const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Transpose<Eigen::Matrix<double, -1, -1> >, 0>, 1, -1, false>, 1, -1, true> >, const Eigen::Block<const Eigen::Inverse<Eigen::CwiseBinaryOp<Eigen::internal::scalar_sum_op<double, double>, const Eigen::Product<Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0>, Eigen::Transpose<Eigen::Matrix<double, -1, -1> >, 0>, const Eigen::Matrix<double, -1, -1> > >, -1, 1, false> >; Func = Eigen::internal::scalar_sum_op<double, double>; Evaluator = Eigen::internal::redux_evaluator<Eigen::CwiseBinaryOp<Eigen::internal::scalar_conj_product_op<double, double>, const Eigen::Transpose<const Eigen::Block<const Eigen::Block<const Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Transpose<Eigen::Matrix<double, -1, -1> >, 0>, 1, -1, false>, 1, -1, true> >, const Eigen::Block<const Eigen::Inverse<Eigen::CwiseBinaryOp<Eigen::internal::scalar_sum_op<double, double>, const Eigen::Product<Eigen::Product<Eigen::Matrix<double, -1, -1>, Eigen::Matrix<double, -1, -1>, 0>, Eigen::Transpose<Eigen::Matrix<double, -1, -1> >, 0>, const Eigen::Matrix<double, -1, -1> > >, -1, 1, false> > >; Eigen::internal::redux_impl<Func, Evaluator, 0, 0>::Scalar = double]
 double ProbabilityDensityFunctions::multivariate_erf(const TrackletPtr&, const TrackObjectPtr&, double)
 typename Eigen::ScalarBinaryOpTraits<typename Eigen::internal::traits<T>::Scalar, typename Eigen::internal::traits<OtherDerived>::Scalar>::ReturnType Eigen::MatrixBase<Derived>::dot(const Eigen::MatrixBase<OtherDerived>&) const [with OtherDerived = Eigen::Matrix<double, -1, 1>; Derived = Eigen::Matrix<double, -1, 1>; typename Eigen::ScalarBinaryOpTraits<typename Eigen::internal::traits<T>::Scalar, typename Eigen::internal::traits<OtherDerived>::Scalar>::ReturnType = double; typename Eigen::internal::traits<OtherDerived>::Scalar = double; typename Eigen::internal::traits<T>::Scalar = double]
 typename Eigen::internal::traits<T>::Scalar Eigen::DenseBase<Derived>::redux(const Func&) const [with BinaryOp = Eigen::internal::scalar_sum_op<double, double>; Derived = Eigen::CwiseBinaryOp<Eigen::internal::scalar_conj_product_op<double, double>, const Eigen::Matrix<double, -1, 1>, const Eigen::Matrix<double, -1, 1> >; typename Eigen::internal::traits<T>::Scalar = double]
 typename Eigen::internal::traits<T>::Scalar Eigen::DenseBase<Derived>::redux(const Func&) const [with BinaryOp = Eigen::internal::scalar_sum_op<double, double>; Derived = Eigen::CwiseUnaryOp<Eigen::internal::scalar_abs2_op<double>, const Eigen::Matrix<double, -1, 1> >; typename Eigen::internal::traits<T>::Scalar = double]
 btrack/src/pdf.cc
 !std::isnan(phi)
-14:41:06
+14:47:01
 ?constexpr void Eigen::PlainObjectBase<Derived>::resize(Eigen::Index) [with Derived = Eigen::Matrix<double, -1, 1>; Eigen::Index = long int]
 Eigen::MapBase<Derived, 0>::MapBase(Eigen::MapBase<Derived, 0>::PointerType, Eigen::Index, Eigen::Index) [with Derived = Eigen::Block<Eigen::Ref<Eigen::Matrix<double, -1, -1> >, -1, 1, true>; Eigen::MapBase<Derived, 0>::PointerType = double*; Eigen::Index = long int]
 Eigen::Block<XprType, BlockRows, BlockCols, InnerPanel>::Block(XprType&, Eigen::Index) [with XprType = Eigen::Ref<Eigen::Matrix<double, -1, -1> >; int BlockRows = -1; int BlockCols = 1; bool InnerPanel = true; Eigen::Index = long int]
 Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::CwiseBinaryOp(const Lhs&, const Rhs&, const BinaryOp&) [with BinaryOp = Eigen::internal::scalar_product_op<double, double>; LhsType = const Eigen::ArrayWrapper<Eigen::Matrix<double, -1, 1> >; RhsType = const Eigen::ArrayWrapper<Eigen::Matrix<double, -1, 1> >; Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::Lhs = Eigen::ArrayWrapper<Eigen::Matrix<double, -1, 1> >; Eigen::CwiseBinaryOp<BinaryOp, Lhs, Rhs>::Rhs = Eigen::ArrayWrapper<Eigen::Matrix<double, -1, 1> >]
 void Eigen::DenseBase<Derived>::resize(Eigen::Index, Eigen::Index) [with Derived = Eigen::Block<Eigen::Ref<Eigen::Matrix<double, -1, -1> >, -1, 1, true>; Eigen::Index = long int]
 CUDA update method not currently supported, reverting to EXACT.
 Eigen::Vector3d Tracklet::position() const
@@ -962,32 +962,32 @@
 ERROR: Exhausted potential linkages.
 Tracking has already been performed. 
 No trackable frames have been found. 
 Eigen::DenseCoeffsBase<Derived, 1>::Scalar& Eigen::DenseCoeffsBase<Derived, 1>::operator[](Eigen::Index) [with Derived = Eigen::Matrix<double, -1, 1>; Eigen::DenseCoeffsBase<Derived, 1>::Scalar = double; Eigen::Index = long int]
 typename Eigen::internal::traits<T>::Scalar Eigen::DenseBase<Derived>::maxCoeff(IndexType*) const [with int NaNPropagation = 0; IndexType = long int; Derived = Eigen::Matrix<double, -1, 1>; typename Eigen::internal::traits<T>::Scalar = double]
 Writing: 
 Object queue is empty. 
-14:41:08
+14:47:03
 typename Eigen::internal::traits<T>::Scalar Eigen::DenseBase<Derived>::maxCoeff(IndexType*) const [with int NaNPropagation = 0; IndexType = long int; Derived = Eigen::Block<Eigen::Ref<Eigen::Matrix<double, -1, -1> >, -1, 1, true>; typename Eigen::internal::traits<T>::Scalar = double]
 St11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
 St19_Sp_make_shared_tag
 St16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
 St23_Sp_counted_ptr_inplaceI11TrackObjectSaIS0_ELN9__gnu_cxx12_Lock_policyE2EE
 St23_Sp_counted_ptr_inplaceI8TrackletSaIS0_ELN9__gnu_cxx12_Lock_policyE2EE
 Eigen::Block<XprType, BlockRows, BlockCols, InnerPanel>::Block(XprType&, Eigen::Index, Eigen::Index, Eigen::Index, Eigen::Index) [with XprType = Eigen::Matrix<double, -1, -1>; int BlockRows = -1; int BlockCols = -1; bool InnerPanel = false; Eigen::Index = long int]
-14:41:13
+14:47:10
 void ImagingVolume::set_volume(const double*)
 PyHypothesis Hypothesis::get_hypothesis() const
 this->hypothesis != TYPE_undef
 ./btrack/include/types.h
 a_volume[0] <= a_volume[1]
 a_volume[2] <= a_volume[3]
 a_volume[4] <= a_volume[5]
 ./btrack/include/hypothesis.h
-14:41:16
+14:47:12
 12TrackManager
 16InterfaceWrapper
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 _ZNSt8_Rb_treeI9HashIndexSt4pairIKS0_St6vectorISt10shared_ptrI8TrackletESaIS6_EEESt10_Select1stIS9_ESt4lessIS0_ESaIS9_EE8_M_eraseEPSt13_Rb_tree_nodeIS9_E.isra.0
 _ZNSt8_Rb_treeI9HashIndexSt4pairIKS0_St6vectorIS1_ISt10shared_ptrI11TrackObjectEjESaIS7_EEESt10_Select1stISA_ESt4lessIS0_ESaISA_EE8_M_eraseEPSt13_Rb_tree_nodeISA_E.isra.0
 _ZNK12HypercubeBin10hash_indexESt10shared_ptrI8TrackletEb.cold
 _ZNK9ObjectBin10hash_indexESt10shared_ptrI8TrackletEb.cold
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -2,15 +2,15 @@
 Hex dump of section '.rodata':
   0x0005e000 00000000 0000f03f 3ec3d84e 7d7f612b .......?>..N}.a+
   0x0005e010 2e9f87a2 ae427d54 62617369 635f7374 .....B}Tbasic_st
   0x0005e020 72696e67 3a3a5f4d 5f636f6e 73747275 ring::_M_constru
   0x0005e030 6374206e 756c6c20 6e6f7420 76616c69 ct null not vali
   0x0005e040 64007665 63746f72 3a3a5f4d 5f726561 d.vector::_M_rea
   0x0005e050 6c6c6f63 5f696e73 65727400 41707220 lloc_insert.Apr 
-  0x0005e060 31372032 30323300 31343a34 303a3430 17 2023.14:40:40
+  0x0005e060 31372032 30323300 31343a34 363a3335 17 2023.14:46:35
   0x0005e070 00000000 00000000 00000000 00000000 ................
   0x0005e080 ffff0000 ffff0000 ffff0000 ffff0000 ................
   0x0005e090 00008047 00008047 00008047 00008047 ...G...G...G...G
   0x0005e0a0 ffffffff ffffff7f 00000000 00000000 ................
   0x0005e0b0 00000000 00003043 756e7369 676e6564 ......0Cunsigned
   0x0005e0c0 20696e74 20636f75 6e745f73 74617465  int count_state
   0x0005e0d0 5f747261 636b2854 7261636b 6c657450 _track(TrackletP
@@ -50,15 +50,15 @@
   0x0005e2f0 7372632f 6879706f 74686573 69732e63 src/hypothesis.c
   0x0005e300 6300615f 74726b2d 3e6c656e 67746828 c.a_trk->length(
   0x0005e310 29203e20 30002e2f 62747261 636b2f69 ) > 0../btrack/i
   0x0005e320 6e636c75 64652f74 7261636b 6c65742e nclude/tracklet.
   0x0005e330 68002174 7261636b 2e656d70 74792829 h.!track.empty()
   0x0005e340 00647420 3e20302e 30005265 73657474 .dt > 0.0.Resett
   0x0005e350 696e6720 6879706f 74686573 69732065 ing hypothesis e
-  0x0005e360 6e67696e 652e0031 343a3430 3a343200 ngine..14:40:42.
+  0x0005e360 6e67696e 652e0031 343a3436 3a333700 ngine..14:46:37.
   0x0005e370 5e2ad6d5 912986c0 00000000 00000040 ^*...).........@
   0x0005e380 00000000 01000000 7b14ae47 e17a843f ........{..G.z.?
   0x0005e390 9a999999 9999b93f 00000000 00002440 .......?......$@
   0x0005e3a0 00000000 00001440 00000000 00000840 .......@.......@
   0x0005e3b0 00000000 0000e03f 0000807f ffff7f7f .......?........
   0x0005e3c0 0000803f 00002041 00000000 00000000 ...?.. A........
   0x0005e3d0 00000000 00000080 00000000 00000000 ................
@@ -349,24 +349,24 @@
   0x0005f5a0 2f656967 656e2f45 6967656e 2f737263 /eigen/Eigen/src
   0x0005f5b0 2f436f72 652f4173 7369676e 4576616c /Core/AssignEval
   0x0005f5c0 7561746f 722e6800 6473742e 726f7773 uator.h.dst.rows
   0x0005f5d0 2829203d 3d206473 74526f77 73202626 () == dstRows &&
   0x0005f5e0 20647374 2e636f6c 73282920 3d3d2064  dst.cols() == d
   0x0005f5f0 7374436f 6c730069 6e646578 203e3d20 stCols.index >= 
   0x0005f600 30202626 20696e64 6578203c 2073697a 0 && index < siz
-  0x0005f610 65282900 31343a34 303a3436 0031343a e().14:40:46.14:
-  0x0005f620 34303a34 38000a00 2c200000 00000000 40:48..., ......
+  0x0005f610 65282900 31343a34 363a3431 0031343a e().14:46:41.14:
+  0x0005f620 34363a34 33000a00 2c200000 00000000 46:43..., ......
   0x0005f630 ffffffff 01000000 54726163 6b204944 ........Track ID
   0x0005f640 3a200054 7261636b 206e6f74 20666f75 : .Track not fou
   0x0005f650 6e642e00 62747261 636b2f73 72632f6d nd..btrack/src/m
   0x0005f660 616e6167 65722e63 6300615f 69647820 anager.cc.a_idx 
   0x0005f670 3c203000 216d5f64 756d6d69 65732e65 < 0.!m_dummies.e
   0x0005f680 6d707479 2829006d 5f64756d 6d696573 mpty().m_dummies
   0x0005f690 5b64756d 6d795f69 64785d2d 3e64756d [dummy_idx]->dum
-  0x0005f6a0 6d790031 343a3430 3a353100 00000000 my.14:40:51.....
+  0x0005f6a0 6d790031 343a3436 3a343600 00000000 my.14:46:46.....
   0x0005f6b0 54726163 6b4f626a 65637450 74722054 TrackObjectPtr T
   0x0005f6c0 7261636b 4d616e61 6765723a 3a676574 rackManager::get
   0x0005f6d0 5f64756d 6d792869 6e742920 636f6e73 _dummy(int) cons
   0x0005f6e0 74000000 00000000 766f6964 20456967 t.......void Eig
   0x0005f6f0 656e3a3a 696e7465 726e616c 3a3a6765 en::internal::ge
   0x0005f700 6d6d5f70 61636b5f 7268733c 5363616c mm_pack_rhs<Scal
   0x0005f710 61722c20 496e6465 782c2044 6174614d ar, Index, DataM
@@ -1480,15 +1480,15 @@
   0x00063c50 42617365 3c446572 69766564 2c20303e Base<Derived, 0>
   0x00063c60 3a3a506f 696e7465 72547970 65203d20 ::PointerType = 
   0x00063c70 646f7562 6c652a3b 20456967 656e3a3a double*; Eigen::
   0x00063c80 496e6465 78203d20 6c6f6e67 20696e74 Index = long int
   0x00063c90 5d007665 6353697a 65203e3d 20300069 ].vecSize >= 0.i
   0x00063ca0 6e63723d 3d310062 74726163 6b2f7372 ncr==1.btrack/sr
   0x00063cb0 632f6d6f 74696f6e 2e636300 696e6974 c/motion.cc.init
-  0x00063cc0 69616c69 73656400 31343a34 303a3535 ialised.14:40:55
+  0x00063cc0 69616c69 73656400 31343a34 363a3530 ialised.14:46:50
   0x00063cd0 00000000 8c08fdff ac06fdff f406fdff ................
   0x00063ce0 ac06fdff af08fdff ac06fdff f406fdff ................
   0x00063cf0 ac06fdff ac06fdff ac06fdff ac06fdff ................
   0x00063d00 f406fdff ac06fdff ac06fdff ac06fdff ................
   0x00063d10 ac06fdff a408fdff ac06fdff ac06fdff ................
   0x00063d20 ac06fdff ac06fdff ac06fdff ac06fdff ................
   0x00063d30 ac06fdff dd08fdff d108fdff ac06fdff ................
@@ -4910,15 +4910,15 @@
   0x000712b0 67656e3a 3a4d6174 7269783c 646f7562 gen::Matrix<doub
   0x000712c0 6c652c20 2d312c20 313e203e 3b207479 le, -1, 1> >; ty
   0x000712d0 70656e61 6d652045 6967656e 3a3a696e pename Eigen::in
   0x000712e0 7465726e 616c3a3a 74726169 74733c54 ternal::traits<T
   0x000712f0 3e3a3a53 63616c61 72203d20 646f7562 >::Scalar = doub
   0x00071300 6c655d00 62747261 636b2f73 72632f70 le].btrack/src/p
   0x00071310 64662e63 63002173 74643a3a 69736e61 df.cc.!std::isna
-  0x00071320 6e287068 69290031 343a3431 3a303600 n(phi).14:41:06.
+  0x00071320 6e287068 69290031 343a3437 3a303100 n(phi).14:47:01.
   0x00071330 0527f61f 930d0440 cd3b7f66 9ea0f63f .'.....@.;.f...?
   0x00071340 636f6e73 74657870 7220766f 69642045 constexpr void E
   0x00071350 6967656e 3a3a506c 61696e4f 626a6563 igen::PlainObjec
   0x00071360 74426173 653c4465 72697665 643e3a3a tBase<Derived>::
   0x00071370 72657369 7a652845 6967656e 3a3a496e resize(Eigen::In
   0x00071380 64657829 205b7769 74682044 65726976 dex) [with Deriv
   0x00071390 6564203d 20456967 656e3a3a 4d617472 ed = Eigen::Matr
@@ -5046,15 +5046,15 @@
   0x00071b30 61747269 783c646f 75626c65 2c202d31 atrix<double, -1
   0x00071b40 2c20313e 3b207479 70656e61 6d652045 , 1>; typename E
   0x00071b50 6967656e 3a3a696e 7465726e 616c3a3a igen::internal::
   0x00071b60 74726169 74733c54 3e3a3a53 63616c61 traits<T>::Scala
   0x00071b70 72203d20 646f7562 6c655d00 57726974 r = double].Writ
   0x00071b80 696e673a 20004f62 6a656374 20717565 ing: .Object que
   0x00071b90 75652069 7320656d 7074792e 20003134 ue is empty. .14
-  0x00071ba0 3a34313a 30380000 74797065 6e616d65 :41:08..typename
+  0x00071ba0 3a34373a 30330000 74797065 6e616d65 :47:03..typename
   0x00071bb0 20456967 656e3a3a 696e7465 726e616c  Eigen::internal
   0x00071bc0 3a3a7472 61697473 3c543e3a 3a536361 ::traits<T>::Sca
   0x00071bd0 6c617220 45696765 6e3a3a44 656e7365 lar Eigen::Dense
   0x00071be0 42617365 3c446572 69766564 3e3a3a6d Base<Derived>::m
   0x00071bf0 6178436f 65666628 496e6465 78547970 axCoeff(IndexTyp
   0x00071c00 652a2920 636f6e73 74205b77 69746820 e*) const [with 
   0x00071c10 696e7420 4e614e50 726f7061 67617469 int NaNPropagati
@@ -5110,15 +5110,15 @@
   0x00071f30 312c202d 313e3b20 696e7420 426c6f63 1, -1>; int Bloc
   0x00071f40 6b526f77 73203d20 2d313b20 696e7420 kRows = -1; int 
   0x00071f50 426c6f63 6b436f6c 73203d20 2d313b20 BlockCols = -1; 
   0x00071f60 626f6f6c 20496e6e 65725061 6e656c20 bool InnerPanel 
   0x00071f70 3d206661 6c73653b 20456967 656e3a3a = false; Eigen::
   0x00071f80 496e6465 78203d20 6c6f6e67 20696e74 Index = long int
   0x00071f90 5d004c6f 73743a20 00206d61 783a2000 ].Lost: . max: .
-  0x00071fa0 31343a34 313a3133 00000000 00000000 14:41:13........
+  0x00071fa0 31343a34 373a3130 00000000 00000000 14:47:10........
   0x00071fb0 06000000 00000000 06000000 00000000 ................
   0x00071fc0 00000000 0000f03f 00000000 00000000 .......?........
   0x00071fd0 00000000 00000000 00000000 0000f03f ...............?
   0x00071fe0 03000000 00000000 03000000 00000000 ................
   0x00071ff0 e7030000 00000000 766f6964 20496d61 ........void Ima
   0x00072000 67696e67 566f6c75 6d653a3a 7365745f gingVolume::set_
   0x00072010 766f6c75 6d652863 6f6e7374 20646f75 volume(const dou
@@ -5132,12 +5132,12 @@
   0x00072090 615f766f 6c756d65 5b305d20 3c3d2061 a_volume[0] <= a
   0x000720a0 5f766f6c 756d655b 315d0061 5f766f6c _volume[1].a_vol
   0x000720b0 756d655b 325d203c 3d20615f 766f6c75 ume[2] <= a_volu
   0x000720c0 6d655b33 5d00615f 766f6c75 6d655b34 me[3].a_volume[4
   0x000720d0 5d203c3d 20615f76 6f6c756d 655b355d ] <= a_volume[5]
   0x000720e0 002e2f62 74726163 6b2f696e 636c7564 ../btrack/includ
   0x000720f0 652f6879 706f7468 65736973 2e680031 e/hypothesis.h.1
-  0x00072100 343a3431 3a313600 31325472 61636b4d 4:41:16.12TrackM
+  0x00072100 343a3437 3a313200 31325472 61636b4d 4:47:12.12TrackM
   0x00072110 616e6167 65720000 00000000 00000000 anager..........
   0x00072120 3136496e 74657266 61636557 72617070 16InterfaceWrapp
   0x00072130 657200                              er.
```

### Comparing `btrack-0.5.4/btrack/libwrapper.py` & `btrack-0.5.5/btrack/libwrapper.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/models.py` & `btrack-0.5.5/btrack/models.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/config.py` & `btrack-0.5.5/btrack/napari/config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/examples/show_btrack_widget.py` & `btrack-0.5.5/btrack/napari/examples/show_btrack_widget.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/main.py` & `btrack-0.5.5/btrack/napari/main.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/reader.py` & `btrack-0.5.5/btrack/napari/reader.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/sync.py` & `btrack-0.5.5/btrack/napari/sync.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/widgets/_general.py` & `btrack-0.5.5/btrack/napari/widgets/_general.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/widgets/_hypothesis.py` & `btrack-0.5.5/btrack/napari/widgets/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/widgets/_motion.py` & `btrack-0.5.5/btrack/napari/widgets/_motion.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/widgets/create_ui.py` & `btrack-0.5.5/btrack/napari/widgets/create_ui.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/napari/widgets/io.py` & `btrack-0.5.5/btrack/napari/widgets/io.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/optimise/hypothesis.py` & `btrack-0.5.5/btrack/optimise/hypothesis.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/optimise/optimiser.py` & `btrack-0.5.5/btrack/optimise/optimiser.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/bayes.cc` & `btrack-0.5.5/btrack/src/bayes.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/belief.cu` & `btrack-0.5.5/btrack/src/belief.cu`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/hyperbin.cc` & `btrack-0.5.5/btrack/src/hyperbin.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/hypothesis.cc` & `btrack-0.5.5/btrack/src/hypothesis.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/inference.cc` & `btrack-0.5.5/btrack/src/inference.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/interface.cc` & `btrack-0.5.5/btrack/src/interface.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/manager.cc` & `btrack-0.5.5/btrack/src/manager.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/motion.cc` & `btrack-0.5.5/btrack/src/motion.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/pdf.cc` & `btrack-0.5.5/btrack/src/pdf.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/tracker.cc` & `btrack-0.5.5/btrack/src/tracker.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/tracklet.cc` & `btrack-0.5.5/btrack/src/tracklet.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/src/wrapper.cc` & `btrack-0.5.5/btrack/src/wrapper.cc`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack/utils.py` & `btrack-0.5.5/btrack/utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/btrack.egg-info/PKG-INFO` & `btrack-0.5.5/btrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrack
-Version: 0.5.4
+Version: 0.5.5
 Summary: A framework for Bayesian multi-object tracking
 Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2017 Alan R. Lowe (quantumjot)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `btrack-0.5.4/btrack.egg-info/SOURCES.txt` & `btrack-0.5.5/btrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/Makefile` & `btrack-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/_static/btrack_logo.png` & `btrack-0.5.5/docs/_static/btrack_logo.png`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/about.rst` & `btrack-0.5.5/docs/about.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/conf.py` & `btrack-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/dev_guide/index.rst` & `btrack-0.5.5/docs/dev_guide/index.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/index.rst` & `btrack-0.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/make.bat` & `btrack-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/configuration.rst` & `btrack-0.5.5/docs/user_guide/configuration.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/installation.rst` & `btrack-0.5.5/docs/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/large_datasets.rst` & `btrack-0.5.5/docs/user_guide/large_datasets.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/napari.rst` & `btrack-0.5.5/docs/user_guide/napari.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/saving_tracks.rst` & `btrack-0.5.5/docs/user_guide/saving_tracks.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/simple_example.rst` & `btrack-0.5.5/docs/user_guide/simple_example.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/docs/user_guide/using_features.rst` & `btrack-0.5.5/docs/user_guide/using_features.rst`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/examples/example_tracking_pipeline-features.ipynb` & `btrack-0.5.5/examples/example_tracking_pipeline-features.ipynb`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/examples/example_tracking_pipeline.ipynb` & `btrack-0.5.5/examples/example_tracking_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/models/cell_config.json` & `btrack-0.5.5/models/cell_config.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/models/cell_config_flat.json` & `btrack-0.5.5/models/cell_config_flat.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/models/particle_config.json` & `btrack-0.5.5/models/particle_config.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/pyproject.toml` & `btrack-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/_test_data/test_data.csv` & `btrack-0.5.5/tests/_test_data/test_data.csv`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/_test_data/test_ground_truth.json` & `btrack-0.5.5/tests/_test_data/test_ground_truth.json`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/_utils.py` & `btrack-0.5.5/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/conftest.py` & `btrack-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/napari/test_dock_widget.py` & `btrack-0.5.5/tests/napari/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_config.py` & `btrack-0.5.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_io.py` & `btrack-0.5.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_models.py` & `btrack-0.5.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_tracker.py` & `btrack-0.5.5/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_tracklets.py` & `btrack-0.5.5/tests/test_tracklets.py`

 * *Files identical despite different names*

### Comparing `btrack-0.5.4/tests/test_utils.py` & `btrack-0.5.5/tests/test_utils.py`

 * *Files identical despite different names*

