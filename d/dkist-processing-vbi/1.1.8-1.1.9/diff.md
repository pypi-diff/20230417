# Comparing `tmp/dkist_processing_vbi-1.1.8.tar.gz` & `tmp/dkist_processing_vbi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.1.8.tar", last modified: Mon Apr 10 21:28:45 2023, max compression
+gzip compressed data, was "dkist_processing_vbi-1.1.9.tar", last modified: Thu Apr 13 20:02:03 2023, max compression
```

## Comparing `dkist_processing_vbi-1.1.8.tar` & `dkist_processing_vbi-1.1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     8114 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3425 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.747611 dkist_processing_vbi-1.1.8/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.747611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.751611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.751611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8991 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/dsps_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/num_exp_per_dsp.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.751611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4428 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6456 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    13777 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.751611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5610 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.751611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/grogu_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     9856 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11423 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     3340 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8332 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.747611 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-10 21:28:45.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-04-10 21:28:45.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 21:28:45.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 21:28:45.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-10 21:28:45.000000 dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/docs/requirements_table.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-04-10 21:28:45.755611 dkist_processing_vbi-1.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-10 21:28:40.000000 dkist_processing_vbi-1.1.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8210 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4172 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8991 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/dsps_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/num_exp_per_dsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4428 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6456 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13777 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5610 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    12708 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/grogu_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     9856 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11423 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8332 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/requirements_table.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/setup.py
```

### Comparing `dkist_processing_vbi-1.1.8/.gitignore` & `dkist_processing_vbi-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/.pre-commit-config.yaml` & `dkist_processing_vbi-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/CHANGELOG.rst` & `dkist_processing_vbi-1.1.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v1.1.9 (2023-04-13)
+===================
+
+Misc
+----
+- Bump version of `dkist-processing-common`
+
 v1.1.8 (2023-04-10)
 ===================
 
 Misc
 ----
 - FITS header specification update to add spectral line keys.
```

### Comparing `dkist_processing_vbi-1.1.8/PKG-INFO` & `dkist_processing_vbi-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.1.8
+Version: 1.1.9
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.1.8/README.rst` & `dkist_processing_vbi-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.1.9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/check_changelog_updated.sh` & `dkist_processing_vbi-1.1.9/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/spectral_line.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/dsps_repeats.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/dsps_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/num_exp_per_dsp.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/num_exp_per_dsp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/spectral_line.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/process_summit_processed.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/quality_metrics.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/grogu_test.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/grogu_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_parse_summit.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.1.8
+Version: 1.1.9
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.1.8/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/docs/Makefile` & `dkist_processing_vbi-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/docs/conf.py` & `dkist_processing_vbi-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/docs/make.bat` & `dkist_processing_vbi-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/licenses/LICENSE.rst` & `dkist_processing_vbi-1.1.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/pyproject.toml` & `dkist_processing_vbi-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.8/setup.cfg` & `dkist_processing_vbi-1.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.3.0
+	dkist-processing-common == 2.4.0
 	dkist-processing-math == 1.0.1
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.5.0
 	astropy == 5.1.1
 	numpy == 1.23.1
 	sunpy == 4.0.3
 	scipy == 1.9.0
```

