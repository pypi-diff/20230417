# Comparing `tmp/dkist_processing_visp-2.0.0rc5.tar.gz` & `tmp/dkist_processing_visp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.0.0rc5.tar", last modified: Fri Mar 31 21:38:30 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.0.1.tar", last modified: Mon Apr 17 17:59:22 2023, max compression
```

## Comparing `dkist_processing_visp-2.0.0rc5.tar` & `dkist_processing_visp-2.0.1.tar`

### file list

```diff
@@ -1,108 +1,107 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    16806 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3548 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/104.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/105.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/106.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/107.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/108.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/109.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.119971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     9775 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.119971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    38179 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    23315 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5883 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10489 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4602 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28203 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6258 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16085 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    19981 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4490 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)    13876 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5633 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11821 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16323 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5489 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3572 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/requirements_table.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    19057 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10093 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.436338 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    38179 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    18995 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.436338 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10422 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    27922 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16170 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    17553 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    19981 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    13876 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    11145 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11821 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/dkist_processing_visp/workflows/single_task_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.432337 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-04-17 17:59:22.000000 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-04-17 17:59:22.000000 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 17:59:22.000000 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-17 17:59:22.000000 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-17 17:59:22.000000 dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-04-17 17:59:22.440338 dkist_processing_visp-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-04-17 17:59:17.000000 dkist_processing_visp-2.0.1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.0.0rc5/.gitignore` & `dkist_processing_visp-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/.pre-commit-config.yaml` & `dkist_processing_visp-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/CHANGELOG.rst` & `dkist_processing_visp-2.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,55 @@
+v2.0.1 (2023-04-17)
+===================
+
+Bugfixes
+--------
+
+- Correct the determination of which spectral lines should be present in L1 frames. (`#111 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/111>`__)
+
+
+v2.0.0 (2023-04-13)
+===================
+
+Features
+--------
+
+- Large improvements to gain algorithm. Primary improvement is usage of lamp gain images to help separate optical/spectral signals
+  and improve solar characteristic spectra removal from solar gain images. (`#105 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/105>`__)
+- Improve spatial residuals in polarimetric data by computing a demodulation matrix for every spatial pixel and then
+  smoothing the resulting demodulation matrices in the spatial dimension. (`#106 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/106>`__)
+- Normalize Q, U, and V polarimetric beams by their respective Stokes-I prior to beam combination, then multiply the combination
+  by the average Stokes-I data. (`#107 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/107>`__)
+- Improvement to accuracy of beam angle calculation. The angle is now measured directly from the hairlines instead of using a Hough transform,
+  which has less accuracy due to the width of the hairlines. (`#108 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/108>`__)
+- Use new and improved PAC fit mode for improved polarimetric accuracy. Also update code to support/interact with
+  `dkist-processing-pac` >= 2.0.0. This is mostly renaming kwargs on API calls. Also removed unneeded dummy dimensions
+  and renamed a matrix multiple function. (`#109 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/109>`__)
+
+
+Misc
+----
+
+- Replace `logging.[thing]` with `logging42.logger.[thing]` for logging bliss. (`#104 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/104>`__)
+
+
+Documentation
+-------------
+
+- Add machinery for a "Scientific" changelog that tracks only those changes that affect L1 output data. (`#110 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/110>`__)
+
+
+v1.6.1 (2023-04-10)
+===================
+
+Misc
+----
+- FITS header specification update to add spectral line keys.
+
+
 v1.6.0 (2023-03-16)
 ===================
 
 Misc
 ----
 - FITS header specification update to add new keys and change some units.
```

### Comparing `dkist_processing_visp-2.0.0rc5/PKG-INFO` & `dkist_processing_visp-2.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.0.0rc5
+Version: 2.0.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
@@ -110,7 +110,38 @@
     # Delete tags
     git tag -d vWHATEVER.THE.VERSION
     git push --delete origin vWHATEVER.THE.VERSION
 
     # Re-tag with the same version
     git tag vWHATEVER.THE.VERSION
     git push --tags origin main
+
+Science Changelog
+^^^^^^^^^^^^^^^^^
+
+Whenever a release involves changes to the scientific quality of L1 data, additional changelog fragment(s) should be
+created. These fragments are intended to be as verbose as is needed to accurately capture the scope of the change(s),
+so feel free to use all the fancy RST you want. Science fragments are placed in the same ``changelog/`` directory
+as other fragments, but are always called::
+
+  <PR NUMBER | +>.science[.<COUNTER>].rst
+
+In the case that a single pull request encapsulates the entirety of the scientific change then the first field should
+be that PR number (same as the normal CHANGELOG). If, however, there is not a simple mapping from a single PR to a scienctific
+change then use the character "+" instead; this will create a changelog entry with no associated PR. For example:
+
+.. code-block:: bash
+
+  $ ls changelog/
+  99.bugfix.rst    # This is a normal changelog fragment associated with a bugfix in PR 99
+  99.science.rst   # Apparently that bugfix also changed the scientific results, so that PR also gets a science fragment
+  +.science.rst    # This fragment is not associated with a PR
+
+
+When it comes time to build the SCIENCE_CHANGELOG, use the ``science_towncrier.sh`` script in this repo to do so.
+This script accepts all the same arguments as the default `towncrier`. For exmaple:
+
+.. code-block:: bash
+
+  ./science_towncrier.sh build --version vx.y.z
+
+This will update the SCIENCE_CHANGELOG and remove any science fragments from the changelog directory.
```

### Comparing `dkist_processing_visp-2.0.0rc5/bitbucket-pipelines.yml` & `dkist_processing_visp-2.0.1/bitbucket-pipelines.yml`

 * *Files 10% similar despite different names*

```diff
@@ -42,16 +42,15 @@
           - echo $SNYK_CLI_COMMAND
           - $SNYK_CLI_COMMAND
     - step: &test
         caches:
           - pip
         name: Test
         script:
-          # - pip install apache-airflow==2.0.0b3 # TODO how to keep in sync with infrastructure?
-          - pip install .[test] # TODO need ssh keys
+          - pip install .[test]
           - pytest -v -n auto --cov -m "not development" dkist_processing_visp
         services:
           - redis
     - step: &push_workflow
         caches:
           - pip
         name: Push Workflow
@@ -101,10 +100,10 @@
     'v*':
       - parallel:
         - step: *check_changelog
         - step: *lint
       - parallel:
         - step: *scan
         - step: *test
-#        - step: *docs
+        - step: *docs
       - step: *push_workflow
       - step: *push_code
```

### Comparing `dkist_processing_visp-2.0.0rc5/check_changelog_updated.sh` & `dkist_processing_visp-2.0.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.0.1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/models/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,18 +118,25 @@
     @property
     def geo_poly_fit_order(self):
         """Order of polynomial used to fit spectral shift as a function of slit position."""
         return self._find_most_recent_past_value("visp_geo_poly_fit_order")
 
     @property
     def solar_spectral_avg_window(self):
-        """Pixel sigma of Gaussian kernal used to compute characteristic solar spectra."""
+        """Pixel width of spatial median filter used to compute characteristic solar spectra."""
         return self._find_parameter_closest_wavelength("visp_solar_spectral_avg_window")
 
     @property
+    def solar_characteristic_spatial_normalization_percentile(self) -> float:
+        """Percentile to pass to `np.nanpercentile` when normalizing each spatial position of the characteristic spectra."""
+        return self._find_most_recent_past_value(
+            "visp_solar_characteristic_spatial_normalization_percentile"
+        )
+
+    @property
     def solar_zone_prominence(self):
         """Relative peak prominence threshold used to identify strong spectral features."""
         return self._find_parameter_closest_wavelength("visp_solar_zone_prominence")
 
     @property
     def solar_zone_width(self):
         """Pixel width used to search for strong spectral features."""
@@ -208,10 +215,9 @@
                 f"Cannot get wavelength dependent parameter {parameter_name} without wavelength"
             )
 
         parameter_dict = self._find_most_recent_past_value(parameter_name)
         wavelengths = np.array(parameter_dict["wavelength"])
         values = parameter_dict["values"]
         idx = np.argmin(np.abs(wavelengths - self._wavelength))
-        chosen_wave = wavelengths[idx]
         chosen_value = values[idx]
         return chosen_value
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-"""ViSP instrument polarization task."""
+"""ViSP instrument polarization task. See :doc:`this page </polarization_calibration>` for more information."""
 from collections import defaultdict
 
 import numpy as np
 import scipy.ndimage as spnd
 from astropy.io import fits
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
-from dkist_processing_pac.fitter.fitting_core import fill_modulation_matrix
-from dkist_processing_pac.fitter.fitting_core import generate_model_I
-from dkist_processing_pac.fitter.fitting_core import generate_S
 from dkist_processing_pac.fitter.polcal_fitter import PolcalFitter
 from dkist_processing_pac.input_data.drawer import Drawer
 from dkist_processing_pac.input_data.dresser import Dresser
 from logging42 import logger
 from sklearn.linear_model import RANSACRegressor
 from sklearn.pipeline import make_pipeline
 from sklearn.pipeline import Pipeline
@@ -64,15 +61,14 @@
             - Compute and save demodulation matrices
 
         Returns
         -------
         None
 
         """
-        # TODO: There might be a better way to skip this task
         if not self.constants.correct_for_polarization:
             return
 
         # Process the pol cal frames
         logger.info(
             f"Demodulation matrices will span FOV with shape 1 spectral bin "
             f"and median smoothing of {self.parameters.polcal_spatial_median_filter_width_px} px in the spatial dimension."
@@ -128,17 +124,14 @@
                     task="DEMOD_MATRICES",
                 )
 
             with self.apm_processing_step("Computing and recording polcal quality metrics"):
                 logger.info("Computing and storing PolCal quality metrics")
                 self.record_polcal_quality_metrics(beam, polcal_fitter=pac_fitter)
 
-            with self.apm_processing_step("Computing and saving intermediate polcal files"):
-                self.save_intermediate_polcal_files(beam, polcal_fitter=pac_fitter)
-
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_polcal_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
                     VispTag.task("POLCAL"),
                 ],
@@ -413,15 +406,14 @@
             logger.info(f"Single demodulation matrix detected")
             return demod_matrices[0, 0, :, :]
 
         target_shape = self.single_beam_shape + demod_shape
         logger.info(f"Target full-frame demodulation shape: {target_shape}")
         return self._resize_polcal_array(demod_matrices, target_shape)
 
-    # TODO: Add test coverage? (See note in *-common.tasks.mixin.quality._metrics._PolcalQualityMixin
     def record_polcal_quality_metrics(self, beam: int, polcal_fitter: PolcalFitter):
         """Record various quality metrics from PolCal fits."""
         self.quality_store_polcal_results(
             polcal_fitter=polcal_fitter,
             label=f"Beam {beam}",
             bins_1=1,  # Yes, this is actually hard-coded right now
             bins_2=self.single_beam_shape[1],
@@ -431,102 +423,14 @@
             # By using the ``skip_recording_constant_pars`` switch we DON'T record the "polcal constant parameters" metric
             # for beam 2. This is because both beam 1 and beam 2 will have the same table. The way `*-common` is built
             # it will look for all metrics for both beam 1 and beam 2 so if we did save that metric for beam 2 then the
             # table would show up twice in the quality report. The following line avoids that.
             skip_recording_constant_pars=beam != 1,
         )
 
-    def save_intermediate_polcal_files(
-        self,
-        beam: int,
-        polcal_fitter: PolcalFitter,
-    ) -> None:
-        """Save intermediate files for science-team analysis.
-
-        THIS FUNCTION IS ONLY TEMPORARY. It should probably be removed prior to production.
-        """
-        dresser = polcal_fitter.local_objects.dresser
-        ## Input flux
-        #############
-        input_flux_tags = [
-            VispTag.intermediate(),
-            VispTag.beam(beam),
-            VispTag.task("INPUT_FLUX"),
-        ]
-
-        # Put all flux into a single array
-        fov_shape = dresser.shape
-        socc_shape = (dresser.numdrawers, dresser.drawer_step_list[0], self.constants.num_modstates)
-        flux_shape = fov_shape + socc_shape
-        input_flux = np.zeros(flux_shape, dtype=np.float64)
-        for i in range(np.prod(fov_shape)):
-            idx = np.unravel_index(i, fov_shape)
-            I_cal, _ = dresser[idx]
-            input_flux[idx] = I_cal.T.reshape(socc_shape)
-
-        flux_hdl = fits.HDUList([fits.PrimaryHDU(input_flux)])
-        with self.apm_writing_step("Writing input flux"):
-            self.fits_data_write(hdu_list=flux_hdl, tags=input_flux_tags)
-            logger.info(
-                f"Wrote input flux with tags {input_flux_tags = } to {next(self.read(tags=input_flux_tags))}"
-            )
-
-        ## Calibration Unit best fit parameters
-        #######################################
-        # cmp_tags = [
-        #     VispTag.intermediate(),
-        #     VispTag.beam(beam),
-        #     VispTag.task("CU_FIT_PARS"),
-        # ]
-        # with self.apm_writing_step("Writing CU fit parameters"):
-        #     self.fits_data_write(hdu_list=dc_cmp.hdu_list, tags=cmp_tags)
-        #     logger.info(f"Wrote CU fits with {cmp_tags = } to {next(self.read(tags=cmp_tags))}")
-
-        ## Best-fix flux
-        ################
-        fit_flux_tags = [VispTag.intermediate(), VispTag.beam(beam), VispTag.task("BEST_FIT_FLUX")]
-        with self.apm_processing_step("Computing best-fit flux"):
-            best_fit_flux = self.compute_best_fit_flux(polcal_fitter)
-            best_fit_hdl = fits.HDUList([fits.PrimaryHDU(best_fit_flux)])
-
-        with self.apm_writing_step("Writing best-fit flux"):
-            self.fits_data_write(hdu_list=best_fit_hdl, tags=fit_flux_tags)
-            logger.info(
-                f"Wrote best-fit flux with {fit_flux_tags = } to {next(self.read(tags=fit_flux_tags))}"
-            )
-
-    # TODO: Test coverage? Hard to do.
-    def compute_best_fit_flux(self, polcal_fitter: PolcalFitter) -> np.ndarray:
-        """Calculate the best-fit SoCC flux from a set of fit parameters.
-
-        The output array has shape (1, num_spectral_bins, num_spatial_bins, 1, 4, num_modstate)
-        """
-        dresser = polcal_fitter.local_objects.dresser
-        fov_shape = dresser.shape
-        socc_shape = (dresser.numdrawers, dresser.drawer_step_list[0], self.constants.num_modstates)
-        flux_shape = fov_shape + socc_shape
-        best_fit_flux = np.zeros(flux_shape, dtype=np.float64)
-        num_points = np.prod(fov_shape)
-        for i in range(num_points):
-            idx = np.unravel_index(i, fov_shape)
-            I_cal, _ = dresser[idx]
-            CM = polcal_fitter.local_objects.calibration_unit
-            TM = polcal_fitter.local_objects.telescope
-            par_vals = polcal_fitter.fit_parameters[idx].valuesdict()
-            CM.load_pars_from_dict(par_vals)
-            TM.load_pars_from_dict(par_vals)
-            S = generate_S(TM=TM, CM=CM, use_M12=True)
-            O = fill_modulation_matrix(par_vals, np.zeros((dresser.nummod, 4)))
-            I_mod = generate_model_I(O, S)
-
-            # Save all data to associated arrays
-            best_fit_flux[idx] = I_mod.T.reshape(socc_shape)
-
-        return best_fit_flux
-
     def _set_original_beam_size(self, array: np.ndarray) -> None:
         """Record the shape of a single beam as a class property."""
         self.single_beam_shape = array.shape
 
     def _resize_polcal_array(self, array: np.ndarray, output_shape: tuple[int, ...]) -> np.ndarray:
         return next(
             resize_arrays(array, output_shape, order=self.parameters.polcal_demod_upsample_order)
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/lamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-"""ViSP lamp calibration task."""
+"""ViSP lamp calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
-import scipy.ndimage as spnd
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
@@ -136,26 +135,14 @@
             averaged_gain_data = average_numpy_arrays(input_lamp_gain_arrays)
             # subtract dark
             dark_corrected_gain_data = next(
                 subtract_array_from_arrays(averaged_gain_data, dark_array)
             )
             filtered_gain_data = self.corrections_mask_hairlines(dark_corrected_gain_data)
 
-            final_gain = self.remove_spatial_gradient(filtered_gain_data)
-
         with self.apm_writing_step(f"Writing gain array for {apm_str}"):
             self.intermediate_frame_helpers_write_arrays(
-                final_gain,
+                filtered_gain_data,
                 beam=beam,
                 task="LAMP_GAIN",
                 modstate=modstate,
             )
-
-    @staticmethod
-    def remove_spatial_gradient(array: np.ndarray) -> np.ndarray:
-        """Normalize each spatial pixel by its median.
-
-        This has the effect of removing any spatial gradients present in the image. We need to do this because the lamp
-        has a different illumination path than the rest of the data and this difference can (and does) introduce
-        gradients in the lamp gains that are not seen in other data.
-        """
-        return array / np.nanmedian(array, axis=0)
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper to manage intermediate data."""
+import itertools
 from typing import Generator
 from typing import Iterable
 from typing import TypeVar
 
 import numpy as np
 from astropy.io import fits
 from dkist_processing_common.models.fits_access import FitsAccessBase
@@ -224,16 +225,15 @@
             if t not in ["self", "arrays", "headers"] and v is not None:
                 tags.append(getattr(VispTag, t)(v))
 
         arrays = [arrays] if isinstance(arrays, np.ndarray) else arrays
         if headers is not None:
             headers = [headers] if isinstance(headers, fits.Header) else headers
         else:
-            # TODO: This len() stops us from passing arrays as a generator. Fix this.
-            headers = [None] * len(arrays)
+            headers = itertools.repeat(None)
 
         for array, header in zip(arrays, headers):
             hdul = fits.HDUList([fits.PrimaryHDU(data=array, header=header)])
             self.fits_data_write(hdu_list=hdul, tags=tags)
 
         filenames = [str(p) for p in self.read(tags=tags)]
         logger.info(f"Wrote intermediate file for {tags = } to {filenames}")
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from dkist_processing_visp.models.parameters import VispParameters
 from dkist_processing_visp.models.tags import VispStemName
 from dkist_processing_visp.parsers.map_repeats import MapScanFlower
 from dkist_processing_visp.parsers.map_repeats import NumMapScansBud
 from dkist_processing_visp.parsers.polarimeter_mode import PolarimeterModeBud
 from dkist_processing_visp.parsers.raster_step import RasterScanStepFlower
 from dkist_processing_visp.parsers.raster_step import TotalRasterStepsBud
-from dkist_processing_visp.parsers.spectral_line import SpectralLineBud
 from dkist_processing_visp.parsers.task import VispTaskTypeFlower
 from dkist_processing_visp.parsers.time import ObsIpStartTimeBud
 from dkist_processing_visp.parsers.time import VispTaskExposureTimesBud
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.parsers.wavelength import ObserveWavelengthBud
 
 S = TypeVar("S", bound=Stem)
@@ -66,15 +65,14 @@
     @property
     def constant_flowers(self) -> list[S]:
         """Add ViSP specific constants to common constants."""
         return super().constant_flowers + [
             NumMapScansBud(),
             TotalRasterStepsBud(),
             NumCSStepBud(self.parameters.max_cs_step_time_sec),
-            SpectralLineBud(),
             ObsIpStartTimeBud(),
             UniqueBud(
                 constant_name=BudName.num_modstates.value, metadata_key="number_of_modulator_states"
             ),
             ObserveWavelengthBud(),
             PolarimeterModeBud(),
             VispTaskExposureTimesBud(
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/science.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""ViSP science calibration task."""
+"""ViSP science calibration task. See :doc:`this page </science_calibration>` for more information."""
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Iterable
 
 import numpy as np
 from astropy.io import fits
@@ -544,27 +544,26 @@
         and v is a vector with dimensions ([n1, ...nn], D2).
 
         The higher-order dimensions (n1, ...nn) can be anything (or nothing), but they must be the same for M and v.
 
         Parameters
         ----------
         vector_stack : np.ndarray
-            ([n1, ...nn], D2) stack of corrected arrays with M modulation states
+            ([n1, ...nn], D2) ND stack of vectors with length D2
 
         matrix_stack : np.ndarray
-            ([n1, ...nn], D1, D2) stack of demodulation matrices with 4 stokes planes and M modulation states
+            ([n1, ...nn], D1, D2) ND stack of matrices with shape (D1, D2)
 
 
         Returns
         -------
         np.ndarray
-            ([n1, ...nn], 4) ndarray with the planes being IQUV
+            ([n1, ...nn], D1) ND stack of vectors with length D1
         """
-        demodulated_array = np.sum(matrix_stack * vector_stack[:, :, None, :], axis=3)
-        return demodulated_array
+        return np.sum(matrix_stack * vector_stack[:, :, None, :], axis=3)
 
     def telescope_polarization_correction(
         self,
         inst_demod_obj: VispL0FitsAccess,
     ) -> VispL0FitsAccess:
         """
         Apply a telescope polarization correction.
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""ViSP solar calibration task."""
+"""ViSP solar calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
 import peakutils
 import scipy.ndimage as spnd
 import scipy.optimize as spo
 import scipy.signal as sps
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
@@ -119,14 +119,18 @@
                     gain = self.remove_solar_signal(
                         char_solar_spectra=refined_char_spec, beam=beam, modstate=modstate
                     )
 
                 with self.apm_processing_step(f"Masking hairlines from {apm_str}"):
                     gain = self.corrections_mask_hairlines(gain)
 
+                self.intermediate_frame_helpers_write_arrays(
+                    arrays=gain, beam=beam, modstate=modstate, task="SC_DEBUG_PRE_EQ_SOLAR_GAIN"
+                )
+
                 pre_equalized_gain_dict[modstate] = gain
 
             with self.apm_processing_step(f"Equalizing modstates for {beam = }"):
                 logger.info(f"Equalizing modstate for {beam = }")
                 equalized_gain_dict = self.equalize_modstates(pre_equalized_gain_dict)
 
             for modstate in range(1, self.constants.num_modstates + 1):
@@ -329,17 +333,14 @@
             geo_corrected_array = next(
                 self.corrections_correct_geometry(lamp_corrected_solar_array, state_offset, angle)
             )
             # We need unshifted, but geo-corrected arrays for reshifting and normalization
             self.intermediate_frame_helpers_write_arrays(
                 arrays=geo_corrected_array, beam=beam, modstate=modstate, task="SC_GEO_NOSHIFT"
             )
-            # re_distorted_array = self.distort_characteristic_spectra(geo_corrected_array, beam=beam, modstate=modstate)
-            # self.intermediate_frame_helpers_write_arrays(arrays=re_distorted_array, beam=beam, modstate=modstate,
-            #                                              task="SC_DEBUG_REDISTORTED_OBS")
 
             # Now finish the spectral shift correction
             spectral_corrected_array = next(
                 self.corrections_remove_spec_geometry(geo_corrected_array, spec_shift)
             )
             self.intermediate_frame_helpers_write_arrays(
                 arrays=spectral_corrected_array, beam=beam, modstate=modstate, task="SC_GEO_ALL"
@@ -367,24 +368,31 @@
 
         Returns
         -------
         np.ndarray
             Characteristic spectra array
         """
         spectral_avg_window = self.parameters.solar_spectral_avg_window
+        normalization_percentile = (
+            self.parameters.solar_characteristic_spatial_normalization_percentile
+        )
         logger.info(
-            f"Computing characteristic spectra for {beam = } and {modstate = } with {spectral_avg_window = }"
+            f"Computing characteristic spectra for {beam = } and {modstate = } with {spectral_avg_window = } and {normalization_percentile = }"
         )
         full_spectra = self.geo_corrected_modstate_data(beam=beam, modstate=modstate)
 
         full_spectra = self.corrections_mask_hairlines(full_spectra)
-        char_spec = spnd.gaussian_filter1d(full_spectra, spectral_avg_window, axis=1)
+        # Normalize each spatial pixel by its own percentile. This removes large spatial gradients that are not solar
+        # signal.
+        normed_spectra = full_spectra / np.nanpercentile(
+            full_spectra, normalization_percentile, axis=0
+        )
 
-        # Normalize so that we preserve the absolute flux in the solar gains when we remove the characteristic spectra
-        char_spec /= np.nanmedian(char_spec)
+        # size = (1, window) means don't smooth in the spectra dimension
+        char_spec = spnd.median_filter(normed_spectra, size=(1, spectral_avg_window))
 
         return char_spec
 
     def refine_gain_shifts(self, char_spec: np.ndarray, beam: int, modstate: int) -> np.ndarray:
         """
         Refine the spectral shifts when matching characteristic spectra to the rectified input spectra.
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tasks/write_l1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Visp write L1 task."""
-import uuid
-from datetime import datetime
 from typing import Literal
 
-import numpy as np
+import astropy.units as u
 from astropy.io import fits
-from astropy.time import Time
 from dkist_processing_common.tasks import WriteL1Frame
+from dkist_processing_common.tasks.write_l1 import WavelengthRange
 from logging42 import logger
 
 from dkist_processing_visp.models.constants import VispConstants
 
 
 class VispWriteL1Frame(WriteL1Frame):
     """
@@ -128,15 +126,14 @@
 
         header["DNAXIS"] = num_axis
         header["DAAXES"] = 2  # Spectral, spatial
         header["DEAXES"] = num_axis - 2  # Total - detector axes
 
         # VISP has a wavelength axis in the frame and so FRAMEWAV is hard to define. Use LINEWAV.
         header["LEVEL"] = 1
-        header["WAVEBAND"] = self.constants.spectral_line
         header["WAVEUNIT"] = -9  # nanometers
         header["WAVEREF"] = "Air"
 
         # Binning headers
         header["NBIN1"] = 1
         header["NBIN2"] = 1
         header["NBIN3"] = 1
@@ -159,7 +156,32 @@
         try:
             return header["DATE-END"]
         except KeyError:
             raise KeyError(
                 f"The 'DATE-END' keyword was not found. "
                 f"Was supposed to be inserted during science calibration."
             )
+
+    def get_wavelength_range(self, header: fits.Header) -> WavelengthRange:
+        """
+        Return the wavelength range of this frame.
+
+        Range is the wavelength values of the pixels at the ends of the wavelength axis.
+        """
+        axis_types = [
+            self.constants.axis_1_type,
+            self.constants.axis_2_type,
+            self.constants.axis_3_type,
+        ]
+        wavelength_axis = axis_types.index("AWAV") + 1  # FITS axis numbering is 1-based, not 0
+        wavelength_unit = header[f"CUNIT{wavelength_axis}"]
+        minimum = header[f"CRVAL{wavelength_axis}"] - (
+            header[f"CRPIX{wavelength_axis}"] * header[f"CDELT{wavelength_axis}"]
+        )
+        maximum = header[f"CRVAL{wavelength_axis}"] + (
+            (header[f"NAXIS{wavelength_axis}"] - header[f"CRPIX{wavelength_axis}"])
+            * header[f"CDELT{wavelength_axis}"]
+        )
+        return WavelengthRange(
+            min=u.Quantity(minimum, unit=wavelength_unit),
+            max=u.Quantity(maximum, unit=wavelength_unit),
+        )
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     def date(self, key: str):
         return choice([1, 2])
 
     @property
     def fits_wcs(self):
         w = WCS(naxis=self.array_ndim)
         w.wcs.crpix = self.array_shape[2] / 2, self.array_shape[1] / 2, 1
-        w.wcs.crval = 0, 0, 0
-        w.wcs.cdelt = 1, 1, 1
+        w.wcs.crval = 0, 656.30, 0
+        w.wcs.cdelt = 1, 0.2, 1
         w.wcs.cunit = "arcsec", "nm", "arcsec"
         w.wcs.ctype = "HPLT-TAN", "AWAV", "HPLN-TAN"
         w.wcs.pc = np.identity(self.array_ndim)
         return w
 
 
 class VispHeadersValidDarkFrames(VispHeaders):
@@ -374,20 +374,21 @@
     visp_hairline_median_spatial_smoothing_width_px: int = 30
     visp_hairline_fraction: float = 0.11
     visp_hairline_mask_spatial_smoothing_width_px: float = 1.0
     visp_hairline_mask_gaussian_peak_cutoff_fraction: float = 0.02
     visp_geo_max_num_otsu: int = 6
     visp_geo_hairline_fit_width_px: int = 10
     visp_geo_max_beam_2_angle_refinement: float = np.deg2rad(0.1)
-    visp_geo_upsample_factor: float = 1000.0
+    visp_geo_upsample_factor: float = 10.0
     visp_geo_max_shift: float = 40.0
     visp_geo_poly_fit_order: int = 3
     visp_solar_spectral_avg_window: WavelengthParameter = WavelengthParameter(
-        values=(50, 50, 60, 110)
+        values=(800, 800, 800, 800)
     )
+    visp_solar_characteristic_spatial_normalization_percentile: float = 90.0
     visp_solar_zone_prominence: WavelengthParameter = WavelengthParameter(
         values=(0.2, 0.2, 0.3, 0.2)
     )
     visp_solar_zone_width: WavelengthParameter = WavelengthParameter(values=(7, 2, 3, 2))
     visp_solar_zone_bg_order: WavelengthParameter = WavelengthParameter(values=(21, 22, 11, 22))
     visp_solar_zone_normalization_percentile: WavelengthParameter = WavelengthParameter(
         values=(90, 99, 90, 90)
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/e2e_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_header_validator import spec214_validator
 from dkist_processing_common.manual import ManualProcessing
 from dkist_processing_common.tasks import QualityL1Metrics
 from dkist_processing_common.tasks import WorkflowTaskBase
-from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
-from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.assemble_movie import AssembleVispMovie
 from dkist_processing_visp.tasks.background_light import BackgroundLightCalibration
 from dkist_processing_visp.tasks.dark import DarkCalibration
@@ -359,16 +357,16 @@
         manual_processing_run.run_task(task=VispL1QualityMetrics)
         manual_processing_run.run_task(task=SubmitAndExposeQuality)
         manual_processing_run.run_task(task=ValidateL1Output)
         manual_processing_run.run_task(task=MakeVispMovieFrames)
         manual_processing_run.run_task(task=AssembleVispMovie)
 
         # Test some downstream services
-        make_dataset_asdf(recipe_run_id, scratch_path)
         make_pdf_report(scratch_path, recipe_run_id)
+        make_dataset_asdf(recipe_run_id, scratch_path)
 
         if any([load_dark, load_lamp, load_geometric, load_solar, load_inst_pol]):
             logger.info("NOT counting provenance records because some tasks were skipped")
         else:
             manual_processing_run.count_provenance()
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,14 @@
 
             mocker.patch(
                 "dkist_processing_visp.tasks.instrument_polarization.PolcalFitter",
                 new=DummyPolcalFitter,
             )
 
             # Don't test place-holder QA stuff for now
-            mocker.patch(
-                "dkist_processing_visp.tasks.instrument_polarization.InstrumentPolarizationCalibration.save_intermediate_polcal_files"
-            )
             quality_metric_mocker = mocker.patch(
                 "dkist_processing_visp.tasks.instrument_polarization.InstrumentPolarizationCalibration.quality_store_polcal_results"
             )
             # Create fake geometric objects
             angle = np.array([0.0])
             offset = np.array([0.0, 0.0])
             spec_shift = np.zeros(intermediate_shape[0])
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_lamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 VispTag.intermediate(),
                 VispTag.modstate(i + 1),
                 VispTag.beam(b),
             ]
             files = list(task.read(tags=tags))
             assert len(files) == 1
             hdu = fits.open(files[0])[0]
-            np.testing.assert_allclose(hdu.data, np.ones((10, 10)))
+            np.testing.assert_allclose(hdu.data, np.ones((10, 10)) * (1 + (0.1 * b)))
 
     tags = [
         VispTag.task("LAMP_GAIN"),
         VispTag.intermediate(),
     ]
     for filepath in task.read(tags=tags):
         assert filepath.exists()
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,14 @@
     parse_inputs_valid_task()
     # Then
     assert parse_inputs_valid_task.constants._db_dict["OBS_IP_START_TIME"] == "2022-11-28T13:55:00"
     assert parse_inputs_valid_task.constants._db_dict["NUM_MODSTATES"] == 2
     assert parse_inputs_valid_task.constants._db_dict["NUM_MAP_SCANS"] == 1
     assert parse_inputs_valid_task.constants._db_dict["NUM_RASTER_STEPS"] == 3
     assert parse_inputs_valid_task.constants._db_dict["WAVELENGTH"] == 656.28
-    assert parse_inputs_valid_task.constants._db_dict["SPECTRAL_LINE"] == "VISP H alpha"
     assert parse_inputs_valid_task.constants._db_dict["DARK_EXPOSURE_TIMES"] == [1.0]
     assert parse_inputs_valid_task.constants._db_dict["LAMP_EXPOSURE_TIMES"] == [10.0]
     assert parse_inputs_valid_task.constants._db_dict["SOLAR_EXPOSURE_TIMES"] == [20.0]
     assert parse_inputs_valid_task.constants._db_dict["POLCAL_EXPOSURE_TIMES"] == [0.01]
     assert parse_inputs_valid_task.constants._db_dict["OBSERVE_EXPOSURE_TIMES"] == [0.02, 0.03]
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,21 @@
         return_value=[(4, 7)],
     )
     task = solar_gain_calibration_task_that_completes
     task()
     for beam in range(1, task.constants.num_beams + 1):
         equalization_flux = np.nanmedian(
             [
-                np.ones((10, 10)) * (1 + beam + m) * (10 * beam * m) * np.mean(np.arange(1, 11) / 5)
+                np.ones((10, 10))
+                * (1 + beam + m)
+                * (10 * beam * m)
+                * np.nanpercentile(
+                    np.arange(1, 11) / 5,
+                    task.parameters.solar_characteristic_spatial_normalization_percentile,
+                )
                 for m in range(1, task.constants.num_modstates + 1)
             ],
             axis=0,
         )
 
         for modstate in range(1, task.constants.num_modstates + 1):
             # Gains aren't normalized so their expected value is weird. This expression comes from the math applied above. Sorry.
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,7 +129,12 @@
             assert header["DATE-AVG"] == date_avg
             assert isinstance(header["HLSVERS"], str)
             assert header["PROPID01"] == "PROPID1"
             assert header["PROPID02"] == "PROPID2"
             assert header["EXPRID01"] == "EXPERID1"
             assert header["EXPRID02"] == "EXPERID2"
             assert header["EXPRID03"] == "EXPERID3"
+            assert header["WAVEBAND"] == "H alpha (656.28 nm)"
+            assert header["SPECLN01"] == "H alpha (656.28 nm)"
+            assert header["SPECLN02"] == "Ni I (676.78 nm)"
+            with pytest.raises(KeyError):
+                header["SPECLN03"]
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.0.1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.0.0rc5
+Version: 2.0.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
@@ -110,7 +110,38 @@
     # Delete tags
     git tag -d vWHATEVER.THE.VERSION
     git push --delete origin vWHATEVER.THE.VERSION
 
     # Re-tag with the same version
     git tag vWHATEVER.THE.VERSION
     git push --tags origin main
+
+Science Changelog
+^^^^^^^^^^^^^^^^^
+
+Whenever a release involves changes to the scientific quality of L1 data, additional changelog fragment(s) should be
+created. These fragments are intended to be as verbose as is needed to accurately capture the scope of the change(s),
+so feel free to use all the fancy RST you want. Science fragments are placed in the same ``changelog/`` directory
+as other fragments, but are always called::
+
+  <PR NUMBER | +>.science[.<COUNTER>].rst
+
+In the case that a single pull request encapsulates the entirety of the scientific change then the first field should
+be that PR number (same as the normal CHANGELOG). If, however, there is not a simple mapping from a single PR to a scienctific
+change then use the character "+" instead; this will create a changelog entry with no associated PR. For example:
+
+.. code-block:: bash
+
+  $ ls changelog/
+  99.bugfix.rst    # This is a normal changelog fragment associated with a bugfix in PR 99
+  99.science.rst   # Apparently that bugfix also changed the scientific results, so that PR also gets a science fragment
+  +.science.rst    # This fragment is not associated with a PR
+
+
+When it comes time to build the SCIENCE_CHANGELOG, use the ``science_towncrier.sh`` script in this repo to do so.
+This script accepts all the same arguments as the default `towncrier`. For exmaple:
+
+.. code-block:: bash
+
+  ./science_towncrier.sh build --version vx.y.z
+
+This will update the SCIENCE_CHANGELOG and remove any science fragments from the changelog directory.
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
 README.rst
+SCIENCE_CHANGELOG.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
+science_towncrier.sh
 setup.cfg
 setup.py
+towncrier_science.toml
 changelog/.gitempty
-changelog/104.misc.rst
-changelog/105.feature.rst
-changelog/106.feature.rst
-changelog/107.feature.rst
-changelog/108.feature.rst
-changelog/109.feature.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
 dkist_processing_visp/models/__init__.py
 dkist_processing_visp/models/constants.py
 dkist_processing_visp/models/parameters.py
-dkist_processing_visp/models/spectral_line.py
 dkist_processing_visp/models/tags.py
 dkist_processing_visp/parsers/__init__.py
 dkist_processing_visp/parsers/map_repeats.py
 dkist_processing_visp/parsers/polarimeter_mode.py
 dkist_processing_visp/parsers/raster_step.py
-dkist_processing_visp/parsers/spectral_line.py
 dkist_processing_visp/parsers/task.py
 dkist_processing_visp/parsers/time.py
 dkist_processing_visp/parsers/visp_l0_fits_access.py
 dkist_processing_visp/parsers/visp_l1_fits_access.py
 dkist_processing_visp/parsers/wavelength.py
 dkist_processing_visp/tasks/__init__.py
 dkist_processing_visp/tasks/assemble_movie.py
@@ -82,13 +77,17 @@
 dkist_processing_visp/workflows/__init__.py
 dkist_processing_visp/workflows/l0_processing.py
 dkist_processing_visp/workflows/single_task_workflows.py
 docs/Makefile
 docs/background_light.rst
 docs/changelog.rst
 docs/conf.py
+docs/gain_correction.rst
 docs/index.rst
 docs/l0_to_l1_visp.rst
 docs/make.bat
+docs/polarization_calibration.rst
 docs/requirements.txt
 docs/requirements_table.rst
+docs/science_calibration.rst
+docs/scientific_changelog.rst
 licenses/LICENSE.rst
```

### Comparing `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.0.1/dkist_processing_visp.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-dkist-processing-common==2.4.0rc1
+dkist-processing-common==2.4.1
 dkist-processing-math==1.0.1
-dkist-processing-pac==2.0.0rc5
+dkist-processing-pac==2.1.0
 dkist-header-validator==3.0.5
-dkist-fits-specifications==3.4.0
+dkist-fits-specifications==3.5.0
 astropy==5.1.1
 numpy==1.23.1
-sunpy==4.0.3
+sunpy==4.1.4
 scipy==1.9.0
 scikit-image==0.19.3
 scikit-learn==1.2.1
 peakutils==1.3.4
 Pillow==9.2.0
 moviepy==1.0.3
 logging42==0.0.8
+dkist-spectral-lines==1.0.0
 
 [docs]
 sphinx
 sphinx-astropy
-sphinx-changelog
+sphinx-changelog==1.3.0
 sphinx-autoapi
 pytest
-towncrier<22.12.0
+towncrier==22.12.0
 dkist-sphinx-theme
 packaging
 
 [grogu]
-dkist==1.0.0b9
+dkist==1.0.0b11
 pyparsing
-dkist-inventory==0.11.0
+dkist-inventory==0.16.0
 parfive<2.0.0
 
 [test]
 pytest
 pytest-cov
 pytest-xdist
 pytest-mock
```

### Comparing `dkist_processing_visp-2.0.0rc5/docs/Makefile` & `dkist_processing_visp-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/docs/background_light.rst` & `dkist_processing_visp-2.0.1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/docs/conf.py` & `dkist_processing_visp-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.0.1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/docs/make.bat` & `dkist_processing_visp-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/licenses/LICENSE.rst` & `dkist_processing_visp-2.0.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/pyproject.toml` & `dkist_processing_visp-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc5/setup.cfg` & `dkist_processing_visp-2.0.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,51 +15,52 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.4.0rc1
+	dkist-processing-common == 2.4.1
 	dkist-processing-math == 1.0.1
-	dkist-processing-pac == 2.0.0rc5
+	dkist-processing-pac == 2.1.0
 	dkist-header-validator == 3.0.5
-	dkist-fits-specifications == 3.4.0
+	dkist-fits-specifications == 3.5.0
 	astropy == 5.1.1
 	numpy == 1.23.1
-	sunpy == 4.0.3
+	sunpy == 4.1.4
 	scipy == 1.9.0
 	scikit-image == 0.19.3
 	scikit-learn == 1.2.1
 	peakutils == 1.3.4
 	Pillow == 9.2.0
 	moviepy == 1.0.3
 	logging42 == 0.0.8
+	dkist-spectral-lines == 1.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-xdist
 	pytest-mock
 	hypothesis
 	towncrier
 	dkist-data-simulator >= 2.1.0
 grogu = 
-	dkist == 1.0.0b9
+	dkist == 1.0.0b11
 	pyparsing
-	dkist-inventory == 0.11.0
+	dkist-inventory == 0.16.0
 	parfive < 2.0.0
 docs = 
 	sphinx
 	sphinx-astropy
-	sphinx-changelog
+	sphinx-changelog == 1.3.0
 	sphinx-autoapi
 	pytest
-	towncrier < 22.12.0
+	towncrier == 22.12.0
 	dkist-sphinx-theme
 	packaging
 
 [build_docs]
 source-dir = docs
 build-dir = docs/_build
 all_files = 1
```

