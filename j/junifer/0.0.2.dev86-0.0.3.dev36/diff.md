# Comparing `tmp/junifer-0.0.2.dev86.tar.gz` & `tmp/junifer-0.0.3.dev36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.2.dev86.tar", last modified: Mon Jan 30 14:56:20 2023, max compression
+gzip compressed data, was "junifer-0.0.3.dev36.tar", last modified: Mon Apr 17 11:54:02 2023, max compression
```

## Comparing `junifer-0.0.2.dev86.tar` & `junifer-0.0.3.dev36.tar`

### file list

```diff
@@ -1,341 +1,365 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.769577 junifer-0.0.2.dev86/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.769577 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.765577 junifer-0.0.2.dev86/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.773577 junifer-0.0.2.dev86/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/changes/0.0.1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/changes/contributors.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/changes/latest.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/images/junifer_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/images/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    28509 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/images/pipeline/pipeline.001.png
--rw-r--r--   0 runner    (1001) docker     (123)   105281 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/images/pipeline/pipeline.002.png
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/docs/using/
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.777577 junifer-0.0.2.dev86/junifer/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer/configs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/configs/tests/test_juseless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.785577 junifer-0.0.2.dev86/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.765577 junifer-0.0.2.dev86/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.785577 junifer-0.0.2.dev86/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.765577 junifer-0.0.2.dev86/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.785577 junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.785577 junifer-0.0.2.dev86/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/hcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_hcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.789578 junifer-0.0.2.dev86/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.793578 junifer-0.0.2.dev86/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19349 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27747 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.797578 junifer-0.0.2.dev86/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.781577 junifer-0.0.2.dev86/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 14:56:20.000000 junifer-0.0.2.dev86/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:20.801578 junifer-0.0.2.dev86/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-30 14:56:11.000000 junifer-0.0.2.dev86/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.036880 junifer-0.0.3.dev36/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.036880 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.040880 junifer-0.0.3.dev36/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.040880 junifer-0.0.3.dev36/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.032880 junifer-0.0.3.dev36/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.040880 junifer-0.0.3.dev36/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.040880 junifer-0.0.3.dev36/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.040880 junifer-0.0.3.dev36/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/changes/newsfragments/220.doc
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.044880 junifer-0.0.3.dev36/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/configs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/configs/tests/test_juseless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.052880 junifer-0.0.3.dev36/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.032880 junifer-0.0.3.dev36/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.032880 junifer-0.0.3.dev36/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.056880 junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/hcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_hcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.032880 junifer-0.0.3.dev36/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-17 11:53:50.000000 junifer-0.0.3.dev36/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-04-17 11:53:50.000000 junifer-0.0.3.dev36/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 11:53:50.000000 junifer-0.0.3.dev36/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-17 11:53:50.000000 junifer-0.0.3.dev36/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-17 11:53:50.000000 junifer-0.0.3.dev36/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.060881 junifer-0.0.3.dev36/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.064880 junifer-0.0.3.dev36/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.068880 junifer-0.0.3.dev36/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.048880 junifer-0.0.3.dev36/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-04-17 11:54:02.000000 junifer-0.0.3.dev36/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 11:54:01.000000 junifer-0.0.3.dev36/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:02.072881 junifer-0.0.3.dev36/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-17 11:53:49.000000 junifer-0.0.3.dev36/tox.ini
```

### Comparing `junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.3.dev36/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/workflows/ci-docs.yml` & `junifer-0.0.3.dev36/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/workflows/ci.yml` & `junifer-0.0.3.dev36/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         bash -c "$(curl -fsSL http://neuro.debian.net/_files/neurodebian-travis.sh)"
         sudo apt-get -qq update
         sudo apt-get -qq install git-annex-standalone
     - name: Configure git for datalad
       run: |
         git config --global user.email "runner@github.com"
         git config --global user.name "GitHub Runner"
-    - uses: actions/checkout@v3
+    - name: Checkout repository
+      uses: actions/checkout@v3
+      with:
+        submodules: true
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Python dependencies
       run: |
         python -m pip install --upgrade pip setuptools wheel
```

### Comparing `junifer-0.0.2.dev86/.github/workflows/docs-preview.yml` & `junifer-0.0.3.dev36/.github/workflows/docs-preview.yml`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,20 @@
       - closed
 
 concurrency: preview-${{ github.ref }}
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-
     steps:
     - name: Checkout source
       uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+        submodules: true
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
     - name: Check for sudo
       shell: bash
       run: |
@@ -47,8 +47,8 @@
     - name: Test build docs
       run: |
         BUILDDIR=_build/main make -C docs/ local
     - name: Deploy preview
       if: github.event_name == 'pull_request'
       uses: rossjrw/pr-preview-action@v1
       with:
-        source-dir: docs/_build/main
+        source-dir: docs/_build/main
```

### Comparing `junifer-0.0.2.dev86/.github/workflows/docs.yml` & `junifer-0.0.3.dev36/.github/workflows/docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,21 @@
     # Sequence of patterns matched against refs/tags
     tags:
       - v*
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-
     steps:
     - name: Checkout source
       uses: actions/checkout@v3
       with:
         # require all of history to see all tagged versions' docs
         fetch-depth: 0
+        submodules: true
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
     - name: Check for sudo
       shell: bash
       run: |
@@ -33,14 +31,15 @@
     - name: Install dependencies
       run: |
         $SUDO bash -c "$(curl -fsSL http://neuro.debian.net/_files/neurodebian-travis.sh)"
         $SUDO apt-get update -qq
         $SUDO apt-get install git-annex-standalone
         python -m pip install --upgrade pip setuptools wheel
         python -m pip install -e .[docs]
+        python -m pip install git+https://github.com/dls-controls/sphinx-multiversion@only-arg
     - name: Configure git for datalad
       run: |
         git config --global user.email "runner@github.com"
         git config --global user.name "GITHUB CI Runner"
     - name: Checkout gh-pages
       # As we already did a deploy of gh-pages above, it is guaranteed to be there
       # so check it out so we can selectively build docs below
```

### Comparing `junifer-0.0.2.dev86/.github/workflows/lint.yml` & `junifer-0.0.3.dev36/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/.github/workflows/pypi.yml` & `junifer-0.0.3.dev36/.github/workflows/pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     tags:
       - 'v*'
 jobs:
   build-n-publish:
     name: Build and publish to PyPI
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@master
+    - name: Checkout source
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
+        submodules: true
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
     - name: Install build
       run:
         pip install build
@@ -27,8 +29,8 @@
     #   uses: pypa/gh-action-pypi-publish@master
     #   with:
     #     password: ${{ secrets.testpypi_token }}
     #     repository_url: https://test.pypi.org/legacy/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: ${{ secrets.pypi_token }}
+        password: ${{ secrets.pypi_token }}
```

### Comparing `junifer-0.0.2.dev86/.gitignore` & `junifer-0.0.3.dev36/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/LICENSE.md` & `junifer-0.0.3.dev36/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/PKG-INFO` & `junifer-0.0.3.dev36/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.2.dev86
+Version: 0.0.3.dev36
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -34,14 +34,15 @@
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is curently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.2.dev86/README.md` & `junifer-0.0.3.dev36/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is curently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.2.dev86/codecov.yml` & `junifer-0.0.3.dev36/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/docs/_templates/versions.html` & `junifer-0.0.3.dev36/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/docs/builtin.rst` & `junifer-0.0.3.dev36/docs/builtin.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .. include:: links.inc
 
-Built-in Pipeline steps and data
-================================
+.. _builtin:
 
+Built-in Pipeline Components
+============================
 
-Data Grabbers
--------------
+
+Data Grabber
+------------
 
 ..
     Provide a list of the DataGrabbers that are implemented or planned.
     Access: Valid options are
         - Open
         - Open with registration
         - Restricted
@@ -37,64 +39,69 @@
 
    * - Class
      - Description
      - Access
      - Type/Config
      - State
      - Version Added
-   * - :class:`junifer.datagrabber.DataladHCP1200`
+   * - :class:`.DataladHCP1200`
      - `HCP OpenAccess dataset <https://github.com/datalad-datasets/human-connectome-project-openaccess>`_
      - Open with registration
      - Built-in
      - Done
      - 0.0.1
-   * - :class:`junifer.configs.juseless.datagrabbers.JuselessDataladUKBVBM`
-     - UKB VBM dataset preprocessed with CAT. Available for Juseless only.
+   * - :class:`.JuselessDataladUKBVBM`
+     - | UKB VBM dataset preprocessed with CAT.
+       | Available for Juseless only.
      - Restricted
      - ``junifer.configs.juseless``
      - Done
      - 0.0.1
-   * - :class:`junifer.configs.juseless.datagrabbers.JuselessDataladCamCANVBM`
-     - CamCAN VBM dataset preprocessed with CAT. Available for Juseless only.
+   * - :class:`.JuselessDataladCamCANVBM`
+     - | CamCAN VBM dataset preprocessed with CAT.
+       | Available for Juseless only.
      - Restricted
      - ``junifer.configs.juseless``
      - Done
      - 0.0.1
-   * - :class:`junifer.datagrabber.DataladAOMICID1000`
+   * - :class:`.DataladAOMICID1000`
      - `AOMIC 1000 dataset <https://github.com/OpenNeuroDatasets/ds003097>`_
      - Open without registration
      - Built-in
      - Done
      - 0.0.1
-   * - :class:`junifer.datagrabber.DataladAOMICPIOP1`
+   * - :class:`.DataladAOMICPIOP1`
      - `AOMIC PIOP1 dataset <https://github.com/OpenNeuroDatasets/ds002785>`_
      - Open without registration
      - Built-in
      - Done
      - 0.0.1
-   * - :class:`junifer.datagrabber.DataladAOMICPIOP2`
+   * - :class:`.DataladAOMICPIOP2`
      - `AOMIC PIOP2 dataset <https://github.com/OpenNeuroDatasets/ds002790>`_
      - Open without registration
      - Built-in
      - Done
      - 0.0.1
-   * - :class:`junifer.configs.juseless.datagrabbers.JuselessDataladAOMICID1000VBM`
-     - AOMIC ID1000 VBM dataset. Available for Juseless only.
+   * - :class:`.JuselessDataladAOMICID1000VBM`
+     - | AOMIC ID1000 VBM dataset.
+       | Available for Juseless only.
      - Restricted
      - ``junifer.configs.juseless``
      - Done
      - 0.0.1
-   * - :class:`junifer.configs.juseless.datagrabbers.JuselessDataladIXIVBM`
-     - `IXI VBM dataset <https://brain-development.org/ixi-dataset/>`_. Available for Juseless only.
+   * - :class:`.JuselessDataladIXIVBM`
+     - | `IXI VBM dataset <https://brain-development.org/ixi-dataset/>`_.
+       | Available for Juseless only.
      - Restricted
      - ``junifer.configs.juseless``
      - Done
      - 0.0.1
-   * - :class:`junifer.configs.juseless.datagrabbers.JuselessUCLA`
-     - UCLA fMRIPrep dataset. Available for Juseless only.
+   * - :class:`.JuselessUCLA`
+     - | UCLA fMRIPrep dataset.
+       | Available for Juseless only.
      - Restricted
      - ``junifer.configs.juseless``
      - Done
      - 0.0.1
 
 Planned
 ~~~~~~~
@@ -111,16 +118,16 @@
    * - ENKI
      - ENKI dataset for Juseless
      - Restricted
      - ``junifer.configs.juseless``
      - :gh:`47`
 
 
-Markers
--------
+Marker
+------
 
 ..
     Provide a list of the Markers that are implemented or planned.
 
     State: this should indicate the state of the marker. Valid options are
     - Planned
     - In Progress
@@ -138,62 +145,73 @@
    :widths: auto
    :header-rows: 1
 
    * - Class
      - Description
      - State
      - Version Added
-   * - :class:`junifer.markers.ParcelAggregation`
+   * - :class:`.ParcelAggregation`
      - Apply parcellation and perform aggregation function
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.FunctionalConnectivityParcels`
+   * - :class:`.FunctionalConnectivityParcels`
      - Compute functional connectivity over parcellation
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.CrossParcellationFC`
+   * - :class:`.CrossParcellationFC`
      - Compute functional connectivity across two parcellations
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.SphereAggregation`
+   * - :class:`.SphereAggregation`
      - Spherical aggregation using mean
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.FunctionalConnectivitySpheres`
+   * - :class:`.FunctionalConnectivitySpheres`
      - Compute functional connectivity over spheres placed on coordinates
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.RSSETSMarker`
+   * - :class:`.RSSETSMarker`
      - Compute root sum of squares of edgewise timeseries
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.ReHoParcels`
+   * - :class:`.ReHoParcels`
      - Calculate regional homogeneity over parcellation
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.ReHoSpheres`
+   * - :class:`.ReHoSpheres`
      - Calculate regional homogeneity over spheres placed on coordinates
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.AmplitudeLowFrequencyFluctuationParcels`
+   * - :class:`.ALFFParcels`
      - Calculate (f)ALFF and aggregate using parcellations
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.AmplitudeLowFrequencyFluctuationSpheres`
+   * - :class:`.ALFFSpheres`
      - Calculate (f)ALFF and aggregate using spheres placed on coordinates
      - Done
      - 0.0.1
-   * - :class:`junifer.markers.EdgeCentricFCParcels`
-     - Calculate edge-centric functional connectivity over parcellation, as found in
-       `Jo et al. (2021) <https://doi.org/10.1016/j.neuroimage.2021.118204>`_
+   * - :class:`.EdgeCentricFCParcels`
+     - | Calculate edge-centric functional connectivity over parcellation, as
+       | found in
+       | `Jo et al. (2021) <https://doi.org/10.1016/j.neuroimage.2021.118204>`_
+     - Done
+     - 0.0.2
+   * - :class:`.EdgeCentricFCSpheres`
+     - | Calculate edge-centric functional connectivity over spheres placed on
+       | coordinates, as found in
+       | `Jo et al. (2021) <https://doi.org/10.1016/j.neuroimage.2021.118204>`_
      - Done
      - 0.0.2
-   * - :class:`junifer.markers.EdgeCentricFCSpheres`
-     - Calculate edge-centric functional connectivity over spheres placed on coordinates,
-       as found in `Jo et al. (2021) <https://doi.org/10.1016/j.neuroimage.2021.118204>`_
+   * - :class:`.TemporalSNRParcels`
+     - Calculate temporal signal-to-noise ratio using parcellations
+     - Done
+     - 0.0.2
+   * - :class:`.TemporalSNRSpheres`
+     - | Calculate temporal signal-to-noise ratio using spheres placed on
+       | coordinates
      - Done
      - 0.0.2
 
 Planned
 ~~~~~~~
 
 .. list-table::
@@ -203,19 +221,20 @@
    * - Name
      - Description
      - Reference
    * - Connectedness
      - Compute connectedness
      - :gh:`34`
    * - Permutation entropy, Range entropy, Multiscale entropy and Hurst exponent
-     - Calculate Permutation entropy, Range entropy, Multiscale entropy and Hurst exponent
+     - | Calculate Permutation entropy, Range entropy, Multiscale entropy and
+       | Hurst exponent
      - :gh:`61`
 
-Parcellations
--------------
+Parcellation
+------------
 
 ..
     Provide a list of the Parcellations that are implemented or planned.
 
     Version added: The Junifer version in which the parcellation was added.
 
 Available
@@ -252,16 +271,18 @@
        | https://doi.org/10.1016/j.neuroimage.2006.05.056
    * - TIAN
      - ``scale``, ``space``, ``magneticfield``
      - | ``TianxS1x3TxMNI6thgeneration``, ``TianxS1x7TxMNI6thgeneration``,
        | ``TianxS2x3TxMNI6thgeneration``, ``TianxS2x7TxMNI6thgeneration``,
        | ``TianxS3x3TxMNI6thgeneration``, ``TianxS3x7TxMNI6thgeneration``,
        | ``TianxS4x3TxMNI6thgeneration``, ``TianxS4x7TxMNI6thgeneration``,
-       | ``TianxS1x3TxMNInonlinear2009cAsym``, ``TianxS2x3TxMNInonlinear2009cAsym``,
-       | ``TianxS3x3TxMNInonlinear2009cAsym``, ``TianxS4x3TxMNInonlinear2009cAsym``
+       | ``TianxS1x3TxMNInonlinear2009cAsym``,
+       | ``TianxS2x3TxMNInonlinear2009cAsym``,
+       | ``TianxS3x3TxMNInonlinear2009cAsym``,
+       | ``TianxS4x3TxMNInonlinear2009cAsym``
      - 0.0.1
      - | Tian, Y., Margulies, D.S., Breakspear, M. et al.
        | Topographic organization of the human subcortex
        | unveiled with functional connectivity gradients.
        | Nature Neuroscience, Volume 23, Pages 1421–1432 (2020).
        | https://doi.org/10.1038/s41593-020-00711-6
 
@@ -295,15 +316,16 @@
      - | Shen, X., Tokoglu, F., Papademetris, X., Constable, R.T.
        | Groupwise whole-brain parcellation from resting-state fMRI data
        | for network node identification.
        | Neuroimage, Volume 82 (2013).
        | https://doi.org/10.1016/j.neuroimage.2013.05.081.
    * - Mindboggle 101
      - | Klein, A., & Tourville, J.
-       | 101 labeled brain images and a consistent human cortical labeling protocol.
+       | 101 labeled brain images and a consistent human cortical labeling
+       | protocol.
        | Frontiers in Neuroscience (2012).
        | http://doi.org/10.3389/fnins.2012.00171/abstract
    * - Destrieux
      - | Destrieux, C., Fischl, B., Dale, A., & Halgren, E.
        | Automatic parcellation of human cortical gyri and sulci using standard
        | anatomical nomenclature.
        | NeuroImage, Volume 53(1), Pages 1–15 (2010).
@@ -312,21 +334,21 @@
      - | Fan, L., Li, H., Zhuo, J. et al.
        | The human brainnetome atlas: a new brain atlas based on connectional
        | architecture.
        | Cerebral cortex, Volume 26(8), Pages 3508-3526 (2016).
        | https://doi.org/10.1093/cercor/bhw157
    * - Buckner
      - | Buckner, R.L., Krienen, F.M., Castellanos, A., Diaz, J.C., Yeo, B.T.T.
-       | The organization of the human cerebellum estimated by intrinsic functional
-       | connectivity.
+       | The organization of the human cerebellum estimated by intrinsic
+       | functional connectivity.
        | Journal of Neurophysiology, Volume 106(5), Pages 2322–2345 (2011).
        | https://doi.org/10.1152/jn.00339.2011
        | Yeo, B.T.T., Krienen, F.M., Sepulcre, J. et al.
-       | The organization of the human cerebral cortex estimated by intrinsic functional
-       | connectivity.
+       | The organization of the human cerebral cortex estimated by intrinsic
+       | functional connectivity.
        | Journal of Neurophysiology, Volume 106(3), Pages 1125–1165 (2011).
        | https://doi.org/10.1152/jn.00338.2011
 
 
 Coordinates
 -----------
 
@@ -345,56 +367,60 @@
    * - Name
      - Keys
      - Version added
      - Publication
    * - Cognitive action control
      - ``CogAC``
      - 0.0.1
-     - | Cieslik, E.C., Mueller, V.I., Eickhoff, C.R., Langner, R., Eickhoff, S.B.
-       | Three key regions for supervisory attentional control: Evidence from neuroimaging
-       | meta-analyses.
+     - | Cieslik, E.C., Mueller, V.I., Eickhoff, C.R., Langner, R.,
+       | Eickhoff, S.B.
+       | Three key regions for supervisory attentional control: Evidence from
+       | neuroimaging meta-analyses.
        | Neuroscience & Biobehavioral Reviews, Volume 48, Pages 22-34 (2015).
        | https://doi.org/10.1016/j.neubiorev.2014.11.003.
    * - Cognitive action regulation
      - ``CogAR``
      - 0.0.1
      - | Langner, R., Leiberg, S., Hoffstaedter, F., Eickhoff, S.B.
-       | Towards a human self-regulation system: Common and distinct neural signatures
-       | of emotional and behavioural control.
+       | Towards a human self-regulation system: Common and distinct neural
+       | signatures of emotional and behavioural control.
        | Neuroscience & Biobehavioral Reviews, Volume 90, Pages 400-410 (2018).
        | https://doi.org/10.1016/j.neubiorev.2018.04.022.
    * - Default mode network
      - ``DMNBuckner``
      - 0.0.1
      - | Van Dijk, K.R., Hedden, T., Venkataraman, A. et al.
        | Intrinsic functional connectivity as a tool for human connectomics:
        | theory, properties, and optimization.
        | Journal of neurophysiology, Volume 103(1), Pages 297-321 (2010).
        | https://doi.org/10.1152/jn.00783.2009
        | Buckner, R.L., Andrews‐Hanna, J.R., & Schacter, D.L.
-       | The brain's default network: anatomy, function, and relevance to disease.
-       | Annals of the New York Academy of Sciences, Volume 1124(1), Pages 1-38 (2008).
+       | The brain's default network: anatomy, function, and relevance to
+       | disease.
+       | Annals of the New York Academy of Sciences, Volume 1124(1), Pages 1-38
+       | (2008).
        | https://doi.org/10.1196/annals.1440.011
    * - Missing formal name
      - ``eMDN``
      - 0.0.1
      - Missing publication details
    * - Empathic processing
      - ``Empathy``
      - 0.0.1
      - | Bzdok, D., Schilbach, L., Vogeley, K. et al.
-       | Parsing the neural correlates of moral cognition: ALE meta-analysis on morality,
-       | theory of mind, and empathy.
+       | Parsing the neural correlates of moral cognition: ALE meta-analysis on
+       | morality, theory of mind, and empathy.
        | Brain Structure and Function, Volume 217(4), Pages 783-796 (2012).
        | https://doi.org/10.1007/s00429-012-0380-y
    * - Extended social-affective default
      - ``eSAD``
      - 0.0.1
      - | Amft, M., Bzdok, D., Laird, A.R. et al.
-       | Definition and characterization of an extended social-affective default network.
+       | Definition and characterization of an extended social-affective default
+       | network.
        | Brain structure & function, Volume 220, Pages 1031–1049 (2015).
        | https://doi.org/10.1007/s00429-013-0698-0
    * - Extended multiple-demand network
      - ``extMDN``
      - 0.0.1
      - | Camilleri, J.A., Müller, V.I., Fox, P. et al.
        | Definition and characterization of an extended multiple-demand network.
@@ -408,59 +434,63 @@
        | An ALE meta-analysis,
        | NeuroImage, Volume 42(1), Pages 343-356 (2008).
        | https://doi.org/10.1016/j.neuroimage.2008.04.025.
    * - Multitasking
      - ``MultiTask``
      - 0.0.1
      - | Worringer, B., Langner, R., Koch, I. et al.
-       | Common and distinct neural correlates of dual-tasking and task-switching:
-       | a meta-analytic review and a neuro-cognitive processing model of human multitasking.
+       | Common and distinct neural correlates of dual-tasking and
+       | task-switching: a meta-analytic review and a neuro-cognitive processing
+       | model of human multitasking.
        | Brain structure & function, Volume 224(5), Pages 1845–1869 (2019).
        | https://doi.org/10.1007/s00429-019-01870-4
    * - Physiological stress
      - ``PhysioStress``
      - 0.0.1
      - | Kogler, L., Müller, V.I., Chang, A. et al.
-       | Psychosocial versus physiological stress — Meta-analyses on deactivations and
-       | activations of the neural correlates of stress reactions.
+       | Psychosocial versus physiological stress — Meta-analyses on
+       | deactivations and activations of the neural correlates of stress
+       | reactions.
        | NeuroImage, Volume 119, Pages 235-251 (2015).
        | https://doi.org/10.1016/j.neuroimage.2015.06.059.
    * - Reward-related decision making
      - ``Rew``
      - 0.0.1
      - | Liu, X., Hairston, J., Schrier, M., Fan, J.
-       | Common and distinct networks underlying reward valence and processing stages:
-       | A meta-analysis of functional neuroimaging studies.
-       | Neuroscience & Biobehavioral Reviews, Volume 35(5), Pages 1219-1236 (2011).
+       | Common and distinct networks underlying reward valence and processing
+       | stages: A meta-analysis of functional neuroimaging studies.
+       | Neuroscience & Biobehavioral Reviews, Volume 35(5), Pages 1219-1236
+       | (2011).
        | https://doi.org/10.1016/j.neubiorev.2010.12.012.
    * - Missing formal name
      - ``Somatosensory``
      - 0.0.1
      - Missing publication details
    * - Theory-of-mind cognition
      - ``ToM``
      - 0.0.1
      - | Bzdok, D., Schilbach, L., Vogeley, K. et al.
-       | Parsing the neural correlates of moral cognition: ALE meta-analysis on morality,
-       | theory of mind, and empathy.
+       | Parsing the neural correlates of moral cognition: ALE meta-analysis on
+       | morality, theory of mind, and empathy.
        | Brain Structure and Function, Volume 217(4), Pages 783-796 (2012).
        | https://doi.org/10.1007/s00429-012-0380-y
    * - Vigilant attention
      - ``VigAtt``
      - 0.0.1
      - | Langner, R., & Eickhoff, S.B.
-       | Sustaining attention to simple tasks: a meta-analytic review of the neural
-       | mechanisms of vigilant attention.
+       | Sustaining attention to simple tasks: a meta-analytic review of the
+       | neural mechanisms of vigilant attention.
        | Psychological bulletin, Volume 139 4, Pages 870-900 (2013).
        | https://doi.org/10.1037/a0030694
    * - Working memory
      - ``WM``
      - 0.0.1
      - | Rottschy, C., Langner, R., Dogan, I. et al.
-       | Modelling neural correlates of working memory: A coordinate-based meta-analysis.
+       | Modelling neural correlates of working memory: A coordinate-based
+       | meta-analysis.
        | NeuroImage, Volume 60, Pages 830-846 (2012).
        | https://doi.org/10.1016/j.neuroimage.2011.11.050.
    * - Areal functional network from Power et al. (2011)
      - ``Power``
      - 0.0.2
      - | Power, J. D., Cohen, A. L., Nelson, S. M. et al.
        | Functional network organization of the human brain.
@@ -482,27 +512,28 @@
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Publication
    * - Emotional scene and face processing (EmoSF)
      - | Sabatinelli, D., Fortune, E.E., Li, Q. et al.
-       | Emotional perception: Meta-analyses of face and natural scene processing.
+       | Emotional perception: Meta-analyses of face and natural scene
+       | processing.
        | NeuroImage, Volume 54(3), Pages 2524-2533 (2011).
        | https://doi.org/10.1016/j.neuroimage.2010.10.011.
    * - Perceptuo-motor network
      - | Heckner, M.K., Cieslik, E.C., Eickhoff, S.B. et al.
-       | The Aging Brain and Executive Functions Revisited: Implications from Meta-analytic
-       | and Functional-Connectivity Evidence.
+       | The Aging Brain and Executive Functions Revisited: Implications from
+       | Meta-analytic and Functional-Connectivity Evidence.
        | Journal of Cognitive Neuroscience, Volume 33(9), Pages 1716–1752 (2021).
        | https://doi.org/10.1162/jocn_a_01616
 
 
-Masks
------
+Mask
+----
 
 ..
     Provide a list of the masks that are implemented or planned.
 
     Version added: The Junifer version in which the mask was added.
 
 Available
@@ -527,34 +558,37 @@
      - 0.0.1
      - | Vickery, Sam, & Patil, Kaustubh. (2022).
        | Chimpanzee and Human Gray Matter Masks [Data set]. Zenodo.
        | https://doi.org/10.5281/zenodo.6463123
    * - Nilearn's MNI152 1mm-resolution mask
      - | ``compute_brain_mask``
      - 0.0.2
-     - | Compute the whole-brain mask. This mask is calculated using MNI152 1mm-resolution template mask onto the 
-       | target image. See :func:`nilearn.masking.compute_brain_mask`
+     - | Compute the whole-brain mask. This mask is calculated using
+       | MNI152 1mm-resolution template mask onto the target image.
+       | See :func:`nilearn.masking.compute_brain_mask`
    * - Nilearn's mask computed from FMRI data
      - | ``compute_epi_mask``
      - 0.0.2
-     - | Compute a brain mask from fMRI data. This is based on an heuristic proposed by T.Nichols: find the least 
-       | dense point of the histogram, between fractions ``lower_cutoff`` and ``upper_cutoff`` of the total image 
-       | histogram. See :func:`nilearn.masking.compute_epi_mask`
+     - | Compute a brain mask from fMRI data. This is based on an heuristic
+       | proposed by T.Nichols: find the least dense point of the histogram,
+       | between fractions ``lower_cutoff`` and ``upper_cutoff`` of the total
+       | image histogram. See :func:`nilearn.masking.compute_epi_mask`
    * - Nilearn's background mask
      - | ``compute_background_mask``
      - 0.0.2
-     - | Compute a brain mask for the images by guessing the value of the background from the border of the image.
+     - | Compute a brain mask for the images by guessing the value of the
+       | background from the border of the image.
        | See :func:`nilearn.masking.compute_background_mask`
 
    * - Nilearn's ICBM152 template gray-matter mask
      - | ``fetch_icbm152_brain_gm_mask``
      - 0.0.2
-     - | Compute a gray-matter mask from the asymmetrical ICBM152 2009 template, release a.
+     - | Compute a gray-matter mask from the asymmetrical ICBM152 2009 template,
+       | release a.
        | See :func:`nilearn.datasets.fetch_icbm152_brain_gm_mask`
 
 
 Planned
 ~~~~~~~
 
-
 ..
   helpful site for creating tables: https://rest-sphinx-memo.readthedocs.io/en/latest/ReST.html#tables
```

### Comparing `junifer-0.0.2.dev86/docs/changes/contributors.inc` & `junifer-0.0.3.dev36/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/docs/conf.py` & `junifer-0.0.3.dev36/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,41 +15,52 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import sys
 from pathlib import Path
 
+# Check if sphinx-multiversion is installed
+use_multiversion = False
+try:
+    import sphinx_multiversion  # noqa: F401
+    use_multiversion = True
+except ImportError:
+    pass
 
 curdir = Path(__file__).parent
 sys.path.append((curdir / "sphinxext").as_posix())
 
 # -- Project information -----------------------------------------------------
 
 project = "junifer"
-copyright = "2022, Authors of junifer"
+copyright = "2023, Authors of junifer"
 author = "Fede Raimondo"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",  # include documentation from docstrings
     "sphinx.ext.autosummary",  # generate autodoc summaries
     "sphinx.ext.doctest",  # test snippets in the documentation
     "sphinx.ext.intersphinx",  # link to other projects’ documentation
     "sphinx.ext.mathjax",  # math support for HTML outputs in Sphinx
     "sphinx_gallery.gen_gallery",  # HTML gallery of examples
-    "sphinx_multiversion",  # self-hosted versioned documentation
     "numpydoc",  # support for NumPy style docstrings
     "gh_substitutions",  # custom GitHub substitutions
+    "sphinx_copybutton",  # copy button for code blocks
+    "sphinxcontrib.mermaid",  # mermaid support
 ]
 
+if use_multiversion:
+    extensions.append("sphinx_multiversion")
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = [
     "_templates",
 ]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
```

### Comparing `junifer-0.0.2.dev86/docs/contribution.rst` & `junifer-0.0.3.dev36/docs/contribution.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,112 +4,141 @@
 
 Contributing to junifer
 =======================
 
 Setting up the local development environment
 --------------------------------------------
 
-1. Fork the https://github.com/juaml/junifer repository on GitHub. If you
+#. Fork the https://github.com/juaml/junifer repository on GitHub. If you
    have never done this before, `follow the official guide
    <https://guides.github.com/activities/forking/>`_.
-2. Clone your fork locally as described in the same guide.
-3. Install your local copy into a Python virtual environment. You can `read
+#. Clone your fork locally as described in the same guide but also add the
+   flag to sync the submodules as well by appending the following to the
+   clone commmand:
+
+   .. code-block:: bash
+
+      ... --recurse-submodules
+
+#. Install your local copy into a Python virtual environment. You can `read
    this guide to learn more
    <https://realpython.com/python-virtual-environments-a-primer/>`_ about them
    and how to create one.
 
-   .. code-block:: console
+   .. code-block:: bash
 
        pip install -e ".[dev]"
 
-4. Create a branch for local development using the ``main`` branch as a
+#. Create a branch for local development using the ``main`` branch as a
    starting point. Use ``fix``, ``refactor``, or ``feat`` as a prefix.
 
-   .. code-block:: console
+   .. code-block:: bash
 
        git checkout main
        git checkout -b <prefix>/<name-of-your-branch>
 
    Now you can make your changes locally.
 
-5. When making changes locally, it is helpful to ``git commit`` your work
+#. When making changes locally, it is helpful to ``git commit`` your work
    regularly. On one hand to save your work and on the other hand, the smaller
    the steps, the easier it is to review your work later. Please use `semantic
    commit messages
    <http://karma-runner.github.io/2.0/dev/git-commit-msg.html>`_.
 
-   .. code-block:: console
+   .. code-block:: bash
 
        git add .
        git commit -m "<prefix>: <summary of changes>"
 
-6. When you're done making changes, check that your changes pass our test suite.
+#. When you're done making changes, check that your changes pass our test suite.
    This is all included with ``tox``.
 
-   .. code-block:: console
+   .. code-block:: bash
 
        tox
 
    You can also run all ``tox`` tests in parallel. As of ``tox 3.7``, you can run
 
-   .. code-block:: console
+   .. code-block:: bash
 
        tox --parallel
 
 
-7. Push your branch to GitHub.
+#. Push your branch to GitHub.
 
-   .. code-block:: console
+   .. code-block:: bash
 
        git push origin <prefix>/<name-of-your-branch>
 
-8. Open the link displayed in the message when pushing your new branch in order
+#. Open the link displayed in the message when pushing your new branch in order
    to submit a pull request. Please follow the template presented to you in the
    web interface to complete your pull request.
 
 
 GitHub Pull Request guidelines
 ------------------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests in the respective ``tests`` directory.
+#. The pull request should include tests in the respective ``tests`` directory.
    Except in rare circumstances, code coverage must not decrease (as reported
    by codecov which runs automatically when you submit your pull request).
-2. If the pull request adds functionality, the docs should be
+#. If the pull request adds functionality, the docs should be
    updated. Consider creating a Python file that demonstrates the usage in
    ``examples/`` directory.
-3. The pull request should also include a short one-liner of your contribution
-   in ``docs/changes/latest.inc``. If it's your first contribution, also add
-   yourself to ``docs/changes/contributors.inc``.
-4. The pull request will be tested against several Python versions.
-5. Someone from the core team will review your work and guide you to a successful
+#. Make sure to create a Draft Pull Request. If you are not sure how to do it,
+   check
+   `here <https://github.blog/2019-02-14-introducing-draft-pull-requests/>`_.
+#. Note the pull request ID assigned after completing the previous step and
+   create a short one-liner file of your contribution named as
+   ``<pull-request-ID>.<type>`` in ``docs/changes/newsfragments/``, ``<type>``
+   being as per the following convention:
+
+   * API change : ``change``
+   * Bug fix : ``bugfix``
+   * Enhancement : ``enh``
+   * Feature : ``feature``
+   * Documentation improvement : ``doc``
+   * Miscellaneous : ``misc``
+   * Deprecation and API removal : ``removal``
+
+   For example, a basic documentation improvement can be recorded in a file
+   ``101.doc`` with the content:
+
+   .. code-block::
+
+       Fixed a typo in intro by `junifer's biggest fan`_
+
+#. If it's your first contribution, also add yourself to
+   ``docs/changes/contributors.inc``.
+#. The pull request will be tested against several Python versions.
+#. Someone from the core team will review your work and guide you to a successful
    contribution.
 
 
 Running unit tests
 ------------------
 
 junifer uses `pytest <http://docs.pytest.org/en/latest/>`_ for its
 unit-tests and new features should in general always come with new
 tests that make sure that the code runs as intended.
 
 To run all tests
 
-.. code-block:: console
+.. code-block:: bash
 
     tox -e test
 
 
 Adding and building documentation
 ---------------------------------
 
 Building the documentation requires some extra packages and can be installed by
 
-.. code-block:: console
+.. code-block:: bash
 
     pip install -e ".[docs]"
 
 To build the docs
 
 .. code-block:: bash
 
@@ -123,17 +152,18 @@
 to clean up the already build files and then re-run ``make local``.
 
 
 Writing Examples
 ----------------
 
 The format used for text is reST. Check the `sphinx reST reference`_ for more
-details. The examples are run and displayed in HTML format using `sphinx gallery`_. To add an
-example, just create a ``.py`` file that starts either with ``plot_`` or ``run_``,
-dependending on whether the example generates a figure or not.
+details. The examples are run and displayed in HTML format using
+`sphinx gallery`_. To add an example, just create a ``.py`` file that starts
+either with ``plot_`` or ``run_``, dependending on whether the example generates
+a figure or not.
 
 The first lines of the example should be a Python block comment with a title,
 a description of the example, authors and license name.
 
 The following is an example of how to start an example
 
 .. code-block:: python
```

### Comparing `junifer-0.0.2.dev86/docs/extending/datagrabber.rst` & `junifer-0.0.3.dev36/docs/extending/datagrabber.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 
 Creating Data Grabbers
 ======================
 
 Data Grabbers are the first step of the pipeline. Its purpose is to interpret
 the structure of a dataset and provide two specific functionalities:
 
-1) Given an *element*, provide the path to each kind of data available for this
+#. Given an *element*, provide the path to each kind of data available for this
    element (e.g. the path to the T1 image, the path to the T2 image, etc.)
-2) Provide the list of *elements* available in the dataset.
+#. Provide the list of *elements* available in the dataset.
 
 In this section, we will see how to create a datagrabber for a dataset. Basic
-aspects of datagrabbers are covered in the 
+aspects of datagrabbers are covered in the
 :ref:`Understanding Data Grabbers <datagrabber>` section.
 
 .. _extending_datagrabbers_think:
 
 Step 1: Think about the element
 -------------------------------
 
 Like with any programming-related task, the first step is to think. When
 creating a Data Grabber, we need to first define what an *element* is.
 The *element* should be the smallest unit of data that can be processed. That
 is, for each element, there should be a set of data that can be processed, but
 only one of each *data type* (see :ref:`data_types`).
 
-For example, if we have a dataset from an fMRI study in which:
+For example, if we have a dataset from a fMRI study in which:
 
-a) both T1w and fMRI was acquired 
-b) 20 subjects went through an experiment twice
-c) the experiment included resting-stage fMRI and a task named *stroop*
+a. both T1w and fMRI was acquired
+b. 20 subjects went through an experiment twice
+c. the experiment included resting-stage fMRI and a task named *stroop*
 
 then the *element* should be composed of 3 items:
 
-*  ``subject``: The subject IDs, e.g. `sub001`, `sub002`, ... `sub020`
-*  ``session``: The sesion number, e.g. `ses1`, `ses2`
-*  ``task``: The task performed, e.g. `rest`, `stroop`
+* ``subject``: The subject IDs, e.g. `sub001`, `sub002`, ... `sub020`
+* ``session``: The sesion number, e.g. `ses1`, `ses2`
+* ``task``: The task performed, e.g. `rest`, `stroop`
 
 If any of these items were not part of the element, then we will have more than
-one ``T1w`` and/or ``BOLD`` image for each subject, which is not allowed.
+one ``T1w`` and / or ``BOLD`` image for each subject, which is not allowed.
 
 Importantly, nothing prevents that one image is part of two different elements.
 For example, it is usually the case that the ``T1w`` image is not acquired for
 each task, but once in the entire session. So in this case, the ``T1w`` image
 for the element (``sub001``, ``ses1``, ``rest``) will be the same as the
 ``T1w`` image for the element (``sub001``, ``ses1``, ``stroop``).
 
@@ -60,56 +60,53 @@
 the dataset. Mainly, because the structure of the dataset will determine how
 the Data Grabber needs to be implemented.
 
 Junifer provides an abstract class to deal with datasets that can be thought in
 terms of *patterns*. A *pattern* is a string that contains placeholders that are
 replaced by the actual values of the element. In our BIDS example, the path
 to the T1w image of subject `sub-01` and session `ses-01`, relative to the
-dataset location, is ``sub-01/ses-01/anat/sub-01_ses-01_T1w.nii.gz``. By 
+dataset location, is ``sub-01/ses-01/anat/sub-01_ses-01_T1w.nii.gz``. By
 replacing ``sub-01`` with ``sub-02``, we can obtain the T1w image of the first
 session of the second subject. Indeed, the path to the T1w images can be
 expressed as a pattern:
 
 ``{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz``
 
 where ``{subject}`` is the replacement for the subject id and ``{session}``
 is the replacement for the session id.
 
-Since it is a BIDS dataaset, the same happens with the BOLD images. The path to
+Since it is a BIDS dataset, the same happens with the BOLD images. The path to
 the BOLD images can be expressed as a pattern:
 
 ``{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz``
 
-
 This will be the norm in most of the datasets. If your dataset can be expressed
 in terms of patterns, then follow :ref:`extending_datagrabbers_pattern`.
 Otherwise, we recommend that you take time to re-think about your dataset
 structure and why it does not have clear *patterns*. Feel free to open a
 discussion in the `junifer Discussions`_ page. Most probably we can help you
 get your dataset in order.
 
 If there is no other way, then you can follow :ref:`extending_datagrabbers_base`
 to create a Data Grabber from scratch.
 
-
 .. _extending_datagrabbers_pattern:
 
 Step 3: Create a Data Grabber
 -----------------------------
 
 Option A: Extending from PatternDataGrabber
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The :py:class:`~junifer.datagrabber.PatternDataGrabber` class is an
-abstract class that has the functionality of understanding patterns embeded
-in it.
+The :class:`.PatternDataGrabber` class is an abstract class that has the
+functionality of understanding patterns embeded in it.
 
 Before creating the datagrabber, we need to define 3 variables:
 
-* ``types``: A list with the available :ref:`data_types` in our dataset 
+* ``types``: A list with the available :ref:`data_types` in our dataset.
 * ``patterns``: A dictionary that specifies the pattern for each data type.
 * ``replacements``: A list indicating which of the elements in the patterns
   should be replaced by the values of the element.
 
 For example, in our BIDS example, the variables will be:
 
 .. code-block:: python
@@ -121,98 +118,101 @@
     }
     replacements = ["subject", "session"]
 
 An additional fourth variable is the ``datadir``, which should be the path to
 where the dataset is located. For example, if the dataset is located in
 ``/data/project/test/data``, then ``datadir`` should be
 ``/data/project/test/data``. Or, if we want to allow the user to specify the
-location of the dataset, we can expose the variable in the constructor, as in 
-this example
+location of the dataset, we can expose the variable in the constructor, as in
+the following example.
 
-With this defined, we can now create our datagrabber, we will name it
+With the variables defined above, we can create our datagrabber and name it
 ``ExampleBIDSDataGrabber``:
 
-
 .. code-block:: python
 
-    from junifer.datagrabber.pattern import PatternDataGrabber
+    from pathlib import Path
+
+    from junifer.datagrabber import PatternDataGrabber
+
 
     class ExampleBIDSDataGrabber(PatternDataGrabber):
 
-        def __init__(self, datadir):
+        def __init__(self, datadir: str | Path) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
                "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
                "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
             }
             replacements = ["subject", "session"]
             super().__init__(
                datadir=datadir,
-               types=types, 
+               types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
 Our datagrabber is ready to be used by junifer. However, it is still unknown
 to the library. We need to register it in the library. To do so, we need to
-use the :py:func:`~junifer.api.decorators.register_datagrabber` decorator.
+use the :func:`.register_datagrabber` decorator.
 
 
 .. code-block:: python
 
-    from junifer.datagrabber.pattern import PatternDataGrabber
+    from pathlib import Path
+
     from junifer.api.decorators import register_datagrabber
+    from junifer.datagrabber import PatternDataGrabber
 
 
     @register_datagrabber
     class ExampleBIDSDataGrabber(PatternDataGrabber):
 
-        def __init__(self, datadir):
+        def __init__(self, datadir: str | Path) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
                "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
                "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
             }
             replacements = ["subject", "session"]
             super().__init__(
                datadir=datadir,
-               types=types, 
+               types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
 
 Now, we can use our datagrabber in junifer, by setting the ``datagrabber`` kind
 in the yaml file to ``ExampleBIDSDataGrabber``. Remember that we still need to
 set the ``datadir``.
 
 .. code-block:: yaml
-   
+
       datagrabber:
          kind: ExampleBIDSDataGrabber
          datadir: /data/project/test/data
 
 
-Optional: Using datalad 
-"""""""""""""""""""""""
+Optional: Using datalad
+~~~~~~~~~~~~~~~~~~~~~~~
 
-If you are using `datalad`_, you can use the 
-:py:class:`~junifer.datagrabber.PatternDataladDataGrabber` instead of the 
-:py:class:`~junifer.datagrabber.PatternDataGrabber`. This class will not only
-interpret patterns, but also use `datalad`_ to `clone` and `get` the data.
+If you are using `datalad`_, you can use the :class:`.PatternDataladDataGrabber`
+instead of the :class:`.PatternDataGrabber`. This class will not only
+interpret patterns, but also use `datalad`_ to ``clone`` and ``get`` the data.
 
 The main difference between the two is that the ``datadir`` is not the actual
-location of the dataset, but the location where the dataset will be cloned. It 
+location of the dataset, but the location where the dataset will be cloned. It
 can now be ``None``, which means that the data will be downloaded to a
 temporary directory. To set the location of the dataset, you can use the
 ``uri`` argument in the constructor. Additionally, a ``rootdir`` argument can
 be used to specify the path to the root directory of the dataset after doing
 ``datalad clone``.
 
-In the example, the dataset is hosted in gin 
+In the example, the dataset is hosted in gin
 (``https://gin.g-node.org/juaml/datalad-example-bids``).
 
 When we clone this dataset, we will see the following structure:
 
 .. code-block::
 
       .
@@ -235,190 +235,208 @@
 .. code-block:: python
 
     uri = "https://gin.g-node.org/juaml/datalad-example-bids"
     rootdir = "example_bids_ses"
 
 And we can create our datagrabber:
 
-
 .. code-block:: python
 
-    from junifer.datagrabber.pattern import PatternDataladDataGrabber
     from junifer.api.decorators import register_datagrabber
+    from junifer.datagrabber import PatternDataladDataGrabber
 
 
     @register_datagrabber
     class ExampleBIDSDataGrabber(PatternDataladDataGrabber):
 
-        def __init__(self):
+        def __init__(self) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
                "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
                "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
             }
             replacements = ["subject", "session"]
             uri = "https://gin.g-node.org/juaml/datalad-example-bids"
             rootdir = "example_bids_ses"
             super().__init__(
                datadir=None,
                uri=uri,
                rootdir=rootdir,
-               types=types, 
+               types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
 
 .. _extending_datagrabbers_base:
 
 Option B: Extending from BaseDataGrabber
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-While we could not think of a use case in which the pattern-based data grabber would not be suitable, it is still
-possible to create a datagrabber extending from the :py:class:`~junifer.datagrabber.base.BaseDataGrabber` class.
+While we could not think of a use case in which the pattern-based datagrabber
+would not be suitable, it is still possible to create a datagrabber extending
+from the :class:`.BaseDataGrabber` class.
 
-In order to create a datagrabber extending from :py:class:`~junifer.datagrabber.base.BaseDataGrabber`, we need to
-implement the following methods:
+In order to create a datagrabber extending from :class:`.BaseDataGrabber`, we
+need to implement the following methods:
 
 - ``get_item``: to get a single item from the dataset.
 - ``get_elements``: to get the list of all elements present in the dataset
 - ``get_element_keys``: to get the keys of the elements in the dataset.
 
 .. note::
-   The ``__init__`` method could also be implemented, but it is not mandatory. This is required if the datagrabber
-   requires any parameter.
 
-We will now implement our BIDS example with this method. 
+   The ``__init__`` method could also be implemented, but it is not mandatory.
+   This is required if the datagrabber requires any extra parameter.
+
+We will now implement our BIDS example with this method.
 
 The first method, ``get_item``, needs to obtain a single
-item from the dataset. Since this dataset requires two variables, ``subject`` and ``session``, we will use them
-as parameters of ``get_item``:
+item from the dataset. Since this dataset requires two variables, ``subject``
+and ``session``, we will use them as parameters of ``get_item``:
 
 .. code-block:: python
 
-   def get_item(self, subject, session):
+   def get_item(self, subject: str, session: str) -> dict[str, str]:
       out = {
          "T1w": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
          "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
       }
       return out
 
 
-The second method, ``get_elements``, needs to return a list of all the elements in the dataset. In this case, we
-know that the dataset contains 3 subjects and 3 sessions, so we can create a list of all the possible combinations.
-However, we need to remember that for session *ses-03* there is no BOLD data.
+The second method, ``get_elements``, needs to return a list of all the elements
+in the dataset. In this case, we know that the dataset contains 3 subjects and 3
+sessions, so we can create a list of all the possible combinations. However, we
+need to remember that for session *ses-03* there is no BOLD data.
 
 .. code-block:: python
 
-   def get_elements(self):
+   from itertools import product
+
+
+   def get_elements(self) -> list[str]:
       subjects = ["sub-01", "sub-02", "sub-03"]
       sessions = ["ses-01", "ses-02"]
 
       # If we are not working on BOLD data, we can add "ses-03"
       if "BOLD" not in self.types:
          sessions.append("ses-03")
       elements = []
-      for subject in subjects:
-         for session in sessions:
-            elements.append({"subject": subject, "session": session})
+      for subject, element in product(subjects, sessions):
+         elements.append({"subject": subject, "session": session})
       return elements
 
 
-And finally, we can implement the ``get_element_keys`` method. This method needs to return a list of the keys that
-represent each of the items in the element tuple. As a rule of thumb, they should be the parameters of the
-``get_item`` method, in the same order.
+And finally, we can implement the ``get_element_keys`` method. This method needs
+to return a list of the keys that represent each of the items in the element
+tuple. As a rule of thumb, they should be the parameters of the ``get_item``
+method, in the same order.
 
 .. code-block:: python
 
-   def get_element_keys(self):
+   def get_element_keys(self) -> list[str]:
       return ["subject", "session"]
 
 
 So, to summarize, our datagrabber will look like this:
 
 .. code-block:: python
 
-   from junifer.datagrabber.base import BaseDataGrabber
    from junifer.api.decorators import register_datagrabber
+   from junifer.datagrabber import BaseDataGrabber
+
 
    @register_datagrabber
    class ExampleBIDSDataGrabber(BaseDataGrabber):
 
-      def get_item(self, subject, session):
+      def get_item(self, subject: str, session: str) -> dict[str, str]:
          out = {
             "T1w": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
             "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
          }
       return out
 
-      def get_elements(self):
+      def get_elements(self) -> list[str]:
          subjects = ["sub-01", "sub-02", "sub-03"]
          sessions = ["ses-01", "ses-02"]
 
          # If we are not working on BOLD data, we can add "ses-03"
          if "BOLD" not in self.types:
             sessions.append("ses-03")
          elements = []
          for subject in subjects:
             for session in sessions:
                elements.append({"subject": subject, "session": session})
          return elements
 
-      def get_element_keys(self):
+      def get_element_keys(self) -> list[str]:
          return ["subject", "session"]
 
-Optional: Using datalad 
-"""""""""""""""""""""""
-
-If this dataset is in a datalad dataset, we can extend from :class:`junifer.datagrabber.DataladDataGrabber` instead of
-:class:`junifer.datagrabber.BaseDataGrabber`. This will allow us to use the datalad API to obtain the data.
+Optional: Using datalad
+~~~~~~~~~~~~~~~~~~~~~~~
 
+If this dataset is in a datalad dataset, we can extend from
+:class:`.DataladDataGrabber` instead of :class:`.BaseDataGrabber`. This will
+allow us to use the datalad API to obtain the data.
 
 Step 4: Optional: Adding *BOLD confounds*
 -----------------------------------------
 
-For some analyses, it is useful to have the confounds associated with the BOLD data. This corresponds to the
-``BOLD_confounds`` item in the :ref:`Data Object <data_object>` (see :ref:`data_types`). However, the ``BOLD_confounds``
-element does not only consists of a ``path``, but it requries more information about the format of the confounds file.
-Thus, the ``BOLD_confounds`` element is a dictionary with the following keys:
+For some analyses, it is useful to have the confounds associated with the BOLD
+data. This corresponds to the ``BOLD_confounds`` item in the
+:ref:`Data Object <data_object>` (see :ref:`data_types`). However, the
+``BOLD_confounds`` element does not only consists of a ``path``, but it requries
+more information about the format of the confounds file. Thus, the
+``BOLD_confounds`` element is a dictionary with the following keys:
 
 - ``path``: the path to the confounds file.
-- ``format``: the format of the confounds file. Currently, this can be either ``fmriprep`` or ``adhoc``.
+- ``format``: the format of the confounds file. Currently, this can be either
+  ``fmriprep`` or ``adhoc``.
 
-The ``fmriprep`` format corresponds to the format of the confounds files generated by `fMRIPrep`_. The
-``adhoc`` format corresponds to a format that is not standardized. 
+The ``fmriprep`` format corresponds to the format of the confounds files
+generated by `fMRIPrep`_. The ``adhoc`` format corresponds to a format that is
+not standardised.
 
 .. note::
-   The ``mappings`` key is only required if the ``format`` is ``adhoc``. If the ``format`` is ``fmriprep``, the
-   ``mappings`` key is not required.
 
+   The ``mappings`` key is only required if the ``format`` is ``adhoc``. If the
+   ``format`` is ``fmriprep``, the ``mappings`` key is not required.
 
-Currently, Junifer provides only one confound remover step
-(:class:`junifer.preprocess.fMRIPrepConfoundRemover`), which relies entirely on the ``fmriprep`` confound
-variable names. Thus, if the confounds are not in ``fmriprep`` format, the user will need to provide the mappings 
-between the *ad-hoc* variable names and the ``fmriprep`` variable names. 
-This is done by specifying the ``adhoc`` format and providing the mappings as a dictionary in the ``mappings`` key.
-
-In the following example, the confounds file has 3 variables that are not in the ``fmriprep`` format. Thus, we will
-provide the mappings for these variables to the ``fmriprep`` format.
+Currently, junifer provides only one confound remover step
+(:class:`.fMRIPrepConfoundRemover`), which relies entirely on the ``fmriprep``
+confound variable names. Thus, if the confounds are not in ``fmriprep`` format,
+the user will need to provide the mappings between the *ad-hoc* variable names
+and the ``fmriprep`` variable names. This is done by specifying the ``adhoc``
+format and providing the mappings as a dictionary in the ``mappings`` key.
+
+In the following example, the confounds file has 3 variables that are not in the
+``fmriprep`` format. Thus, we will provide the mappings for these variables to
+the ``fmriprep`` format. For example, the ``get_item`` method could look like
+this:
 
 .. code-block:: python
 
-   out["BOLD_confounds"]: {
-      "path": f"{subject}/{session}/func/{subject}_{session}_confounds.tsv",
-      "format": "adhoc",
-      "mappings": {
-         "fmriprep": {
-            "variable1": "rot_x",
-            "variable2": "rot_z",
-            "variable3": "rot_y",
-         }
-      },
-   }
-
+   def get_item(
+      self, subject: str, session: str
+   ) -> dict:
+      out = {
+         "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+         "BOLD_confounds": {
+            "path": f"{subject}/{session}/func/{subject}_{session}_confounds.tsv",
+            "format": "adhoc",
+            "mappings": {
+               "fmriprep": {
+                  "variable1": "rot_x",
+                  "variable2": "rot_z",
+                  "variable3": "rot_y",
+               }
+         },
+      }
 
 .. note::
-   Not all of the mappings need to be provided. For the moment, this is used only by the
-   :class:`junifer.preprocess.fMRIPrepConfoundRemover` step, which requires variables based on the
-   strategy selected. However, it is recommended to provide all the mappings, as this will allow the user to
-   choose different strategies with the same dataset.
 
+   Not all of the mappings need to be provided. For the moment, this is used
+   only by the :class:`.fMRIPrepConfoundRemover` step, which requires variables
+   based on the strategy selected. However, it is recommended to provide all the
+   mappings, as this will allow the user to choose different strategies with the
+   same dataset.
```

### Comparing `junifer-0.0.2.dev86/docs/extending/extension.rst` & `junifer-0.0.3.dev36/docs/extending/extension.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 .. include:: ../links.inc
 
 .. _extending_extension:
 
-Creating a Junifer extension
+Creating a junifer extension
 ============================
 
-Junifer is designed to be easily extensible. Through the use of a registry and decorators, we can easily add new
-functionality to junifer on runtime. This is done by creating a new python module and importing it before running
-junifer.
+Junifer is designed to be easily extensible. Through the use of a registry and
+decorators, you can easily add new functionality to junifer during runtime. This
+is done by creating a new Python module and importing it before running junifer.
+
+A special consideration has to be made when using the
+:ref:`code-less configuration<codeless>`. In this case, the
+``with`` statement can be used to import a module or run a Python file.
 
-A special consideration has to be made when using the :ref:`code-less configuration<codeless>`. In this case, the
-``with`` statement can be used to import a module or run a python ``.py`` file.
-
-In the following example, we instruct junifer to first import ``my_module`` and then run the ``my_file.py`` file.
+In the following example, we instruct junifer to first import ``my_module`` and
+then run the ``my_file.py`` file.
 
 .. code-block:: yaml
 
     with:
       - my_module
       - my_file.py
 
-Thus, the code from ``my_file.py`` will be executed before running junifer. This is the ideal place to create junifer
-extensions.
+Thus, the code from ``my_file.py`` will be executed before running junifer. This
+is the ideal place to include junifer extensions.
+
+.. important::
 
-.. important:: Some junifer commands will not consider files imported from files included in the ``with`` statement.
-   That is, if ``my_file.py`` imports ``my_other_file.py``, some of the junifer commands will not consider
-   ``my_other_file.py``. Either place all the code in one file or add multiple files to the ``with`` statement.
+   Some junifer commands will not consider files imported from files included
+   in the ``with`` statement. If ``my_file.py`` imports ``my_other_file.py``,
+   some of the junifer commands will not consider ``my_other_file.py``. Either
+   place all the code in one file or add multiple files to the ``with``
+   statement.
```

### Comparing `junifer-0.0.2.dev86/docs/extending/index.rst` & `junifer-0.0.3.dev36/docs/extending/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 .. _extending:
 
 Extending junifer
 =================
 
 While we aim to provide as many datasets and markers as possible, we are also
 interested in allowing users to extend the functionality with their own
-datagrabbers, preprocessing, markers, etc.
+datagrabbers, preprocessing, markers, etc., .
 
-This does not mean that the new functionality will have to be included in
-junifer before the user can use them. Instead, the user can simply
-create a new python file, code the desired functionality and use it with
-junifer. This is the first step towards including the new functionality in
-the junifer package.
+It's not necessary to have the new functionality included in junifer before
+the user can use them. The user can simply create a new Python file, code the
+desired functionality and use it with junifer. This is the first step towards
+including the new functionality in the junifer pipeline.
 
 In this section we will show how to extend junifer, by creating new
-datagrabbers, preprocessing and markers, following the *junifer* way.
+datagrabbers, preprocessing, markers, etc.,  following the *junifer* way.
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    extension
    datagrabber
-   marker
+   marker
+   parcellations
+   coordinates
+   masks
```

### Comparing `junifer-0.0.2.dev86/docs/extending/marker.rst` & `junifer-0.0.3.dev36/docs/extending/marker.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,151 @@
 .. include:: ../links.inc
 
 .. _extending_markers:
 
 Creating Markers
 ================
 
-Computing a marker (a.k.a. *feature*) is the main goal of junifer. While we aim to provide as many markers as possible,
-it might be the case that the marker you are looking for is not available. In this case, you can create your own marker
+Computing a marker (a.k.a. *feature*) is the main goal of junifer. While we aim
+to provide as many markers as possible, it might be the case that the marker you
+are looking for is not available. In this case, you can create your own marker
 by following this tutorial.
 
-Most of the functionality of a junifer marker has been taken care by the :class:`junifer.markers.BaseMarker` class. 
-Thus, only a few methods are required:
+Most of the functionality of a junifer marker has been taken care by the
+:class:`.BaseMarker` class. Thus, only a few methods are required:
 
-1. ``get_valid_inputs``: a method to obtain the list of valid inputs for the marker. This is used to check that the
-   inputs provided by the user are valid. This method should return a list of strings, representing 
-   :ref:`data types <data_types>`
-2. ``get_output_type``: a method to obtain the kind of output of the marker. This is used to check that the output
-   of the marker is compatible with the storage. This method should return a string, representing 
-   :ref:`storage types <storage_types>`
-3. ``compute``: the method that given the data, computes the marker.
-4. ``__init__``: the initialization method, where the marker is configured.
-
-As an example, we will develop a Parcel Mean marker, that is, a marker that first applies a parcellation and
-then computes the mean of the data in each parcel. This is a very simple example, but it will show you how to create
-a new marker.
+#. ``get_valid_inputs``: The method to obtain the list of valid inputs for the
+   marker. This is used to check that the inputs provided by the user are
+   valid. This method should return a list of strings, representing
+   :ref:`data types <data_types>`.
+#. ``get_output_type``: The method to obtain the kind of output of the marker.
+   This is used to check that the output of the marker is compatible with the
+   storage. This method should return a string, representing
+   :ref:`storage types <storage_types>`.
+#. ``compute``: The method that given the data, computes the marker.
+#. ``__init__``: The initialisation method, where the marker is configured.
+
+As an example, we will develop a ``ParcelMean`` marker, a marker that first
+applies a parcellation and then computes the mean of the data in each parcel.
+This is a very simple example, but it will show you how to create a new marker.
 
 .. _extending_markers_input_output:
 
 Step 1: Configure input and output
 ----------------------------------
 
-This step is quite simple: we need to define the input and output of the marker. Based on the current
-:ref:`data types <data_types>`, we can define as valid inputs ``BOLD``, ``VBM_WM`` and ``VBM_GM``.
+This step is quite simple: we need to define the input and output of the marker.
+Based on the current :ref:`data types <data_types>`, we can have ``BOLD``,
+``VBM_WM`` and ``VBM_GM`` as valid inputs.
 
 .. code-block:: python
 
-    def get_valid_inputs(self):
-        return ['BOLD', 'VBM_WM', 'VBM_GM']
+    def get_valid_inputs(self) -> list[str]:
+        return ["BOLD", "VBM_WM", "VBM_GM"]
 
-The output of the marker depends on the input. For ``BOLD``, it will be ``timeseries``, while for the rest of the inputs,
-it will be ``table``. Thus, we can define the output as:
+The output of the marker depends on the input. For ``BOLD``, it will be
+``timeseries``, while for the rest of the inputs, it will be ``vector``. Thus,
+we can define the output as:
 
 .. code-block:: python
 
-    def get_output_type(self, input_kind):
-        if input_kind == 'BOLD':
-            return 'timeseries'
+    def get_output_type(self, input_kind: str) -> str:
+        if input_kind == "BOLD":
+            return "timeseries"
         else:
-            return 'table'
+            return "vector"
 
 .. _extending_markers_init:
 
-Step 2: Initialize the marker
+Step 2: Initialise the marker
 -----------------------------
 
-In this step we need to define the parameters of the marker. That is, all the parameters that the user can provide
+In this step we need to define the parameters of the marker the user can provide
 to configure how the marker will behave.
 
-The parameters of the marker are defined in the ``__init__`` method. The :class:`junifer.markers.BaseMarker` class
-requires two optional parameters:
+The parameters of the marker are defined in the ``__init__`` method. The
+:class:`.BaseMarker` class requires two optional parameters:
 
-1. ``name``: the name of the marker. This is used to identify the marker in the configuration file.
-2. ``on``: a list or string with the data types that the marker will be applied to.
+1. ``name``: the name of the marker. This is used to identify the marker in the
+   configuration file.
+2. ``on``: a list or string with the data types that the marker will be applied
+   to.
+
+.. attention::
+
+   Only basic types (*int*, *bool* and *str*), lists, tuples and dictionaries
+   are allowed as parameters. This is because the parameters are stored in
+   JSON format, and JSON only supports these types.
 
-.. attention:: Only basic types (*int*, *bool* and *str*) as well as Lists, Tuples and Dictionaries are allowed as
-               parameters. This is because the parameters are stored in a JSON file, and JSON only supports these types.
-
-
-In this example, the is only paramater required for the computation is the name of the parcellation to use. Thus, we can
-define the ``__init__`` method as follows:
+In this example, only paramater required for the computation is the name of the
+parcellation to use. Thus, we can define the ``__init__`` method as follows:
 
 .. code-block:: python
-    
-    def __init__(self, parcellation_name, on=None, name=None):
-        self.parcellation_name = parcellation_name
+
+    def __init__(
+       self,
+       parcellation: str,
+       on: str | list[str] | None = None,
+       name: str | None = None,
+    ) -> None:
+        self.parcellation = parcellation
         super().__init__(on=on, name=name)
 
-.. caution:: Parameters of the marker must be stored as object attributes without using ``_`` as prefix. This is
-             because any attribute that starts with ``_`` will not be considered as a parameter and not stored as 
-             part of the metadata of the marker.
+.. caution::
 
+   Parameters of the marker must be stored as object attributes without using
+   ``_`` as prefix. This is because any attribute that starts with ``_`` will
+   not be considered as a parameter and not stored as part of the metadata of
+   the marker.
 
 .. _extending_markers_compute:
 
 Step 3: Compute the marker
 --------------------------
 
-In this step, we will define the method that computes the marker. This method will be called by junifer when needed,
-using the data provided by the datagrabber, as configured by the user. The function ``compute`` has two arguments:
-
-* ``input``: a dictionary with the data to be used to compute the marker. This will be the corresponding element in the 
-  :ref:`Data Object<data_object>` alredy indexing. Thus, the dictionary has at least two keys: ``data`` and ``path``.
-  The first one contains the data, while the second one contains the path to the data. The dictionary can also contain
-  other keys, depending on the data type.
-* ``extra_input``: the rest of the :ref:`Data Object<data_object>`. This is useful if you want to use other data to
-  compute the marker (e.g.: ``BOLD_confounds`` can be used to de-confound the ``BOLD`` data).
+In this step, we will define the method that computes the marker. This method
+will be called by junifer when needed, using the data provided by the
+datagrabber, as configured by the user. The method ``compute`` has two
+arguments:
+
+* ``input``: a dictionary with the data to be used to compute the marker. This
+  will be the corresponding element in the :ref:`Data Object<data_object>`
+  alredy indexed. Thus, the dictionary has at least two keys: ``data`` and
+  ``path``. The first one contains the data, while the second one contains the
+  path to the data. The dictionary can also contain other keys, depending on the
+  data type.
+* ``extra_input``: the rest of the :ref:`Data Object<data_object>`. This is
+  useful if you want to use other data to compute the marker
+  (e.g.: ``BOLD_confounds`` can be used to de-confound the ``BOLD`` data).
 
 Following the example, we will compute the mean of the data in each parcel using
-:class:`nilearn.maskers.NiftiLabelsMasker`. Importantly, the output of the compute function must be a dictionary.
-This dictionary will later be passed onto the ``store`` method.
-
-.. hint:: To simplify the ``store`` method, define keys of the dictionary based on the corresponding store functions
-          in the :ref:`storage types <storage_types>`. For example, if the output is a ``table``, the keys of the
-          dictionary should be ``data`` and ``columns``.
+:class:`nilearn.maskers.NiftiLabelsMasker`. Importantly, the output of the
+compute function must be a dictionary. This dictionary will later be passed onto
+the ``store`` method.
+
+.. hint::
+
+   To simplify the ``store`` method, define keys of the dictionary based on the
+   corresponding store functions in the :ref:`storage types <storage_types>`.
+   For example, if the output is a ``vector``, the keys of the dictionary should
+   be ``data`` and ``col_names``.
 
 .. code-block:: python
 
-    from nilearn.maskers import NiftiLabelsMasker
+    from typing import Any
+
     from junifer.data import load_parcellation
+    from nilearn.maskers import NiftiLabelsMasker
+
 
-    def compute(self, input, extra_input):
+    def compute(
+       self,
+       input: dict[str, Any],
+       extra_input: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
         # Get the data
         data = input["data"]
 
         # Get the min of the voxels sizes and use it as the resolution
         resolution = np.min(data.header.get_zooms()[:3])
 
         # Load the parcellation
@@ -122,75 +154,87 @@
             resolution=resolution,
         )
 
         # Create a masker
         masker = NiftiLabelsMasker(
             labels_img=t_parcellation,
             standardize=True,
-            memory='nilearn_cache',
+            memory="nilearn_cache",
             verbose=5,
         )
 
         # mask the data
         out_values = masker.fit_transform([data])
 
         # Create the output dictionary
-        out = {"data": out_values, "columns": t_labels}
+        out = {"data": out_values, "col_names": t_labels}
 
-        # If its 3D (BOLD), name each row as "scan"
-        if out_values.shape[0] > 1:
-            out["row_names"] = "scan"
         return out
 
 
 .. _extending_markers_finalize:
 
-Step 4: Finalize the marker
+Step 4: Finalise the marker
 ---------------------------
 
-Once all of the above steps are done, we just need to give our marker a name, state its *dependencies* and register it
-using the ``@register_marker`` decorator.
-
-The *dependencies* are the core packages that are required to compute the marker. This will be later used to keep track
-of the versions of the packages used to compute the marker. To inform junifer about the dependencies of a marker,
-we need to define a ``_DEPENDENCIES`` attribute in the class. This attribute must be a set, with the names of the
-packages as strings. For example, the ``ParcelMean`` marker has the following dependencies:
+Once all of the above steps are done, we just need to give our marker a name,
+state its *dependencies* and register it using the ``@register_marker``
+decorator.
+
+The *dependencies* are the core packages that are required to compute the marker.
+This will be later used to keep track of the versions of the packages used to
+compute the marker. To inform junifer about the dependencies of a marker, we need
+to define a ``_DEPENDENCIES`` attribute in the class. This attribute must be a
+set, with the names of the packages as strings. For example, the ``ParcelMean``
+marker has the following dependencies:
 
 .. code-block:: python
 
-    _DEPENDENCIES = {"nilearn"}
+    _DEPENDENCIES = {"nilearn", "numpy"}
 
-Finally, we need to register the marker using the ``@register_marker`` decorator. This decorator takes the name of the
+Finally, we need to register the marker using the ``@register_marker`` decorator.
 
 .. code-block:: python
 
-    from nilearn.maskers import NiftiLabelsMasker
-    from junifer.data import load_parcellation
+    from typing import Any
+
     from junifer.api.decorators import register_marker
+    from junifer.data import load_parcellation
     from junifer.markers.base import BaseMarker
+    from nilearn.maskers import NiftiLabelsMasker
+
 
     @register_marker
     class ParcelMean(BaseMarker):
 
-         _DEPENDENCIES = {"nilearn", "numpy"}
+        _DEPENDENCIES = {"nilearn", "numpy"}
 
-        def __init__(self, parcellation_name, on=None, name=None):
-            self.parcellation_name = parcellation_name
+        def __init__(
+           self,
+           parcellation: str,
+           on: str | list[str] | None = None,
+           name: str | None = None,
+        ) -> None:
+            self.parcellation = parcellation
             super().__init__(on=on, name=name)
-        
-        def get_valid_inputs(self):
-            return ['BOLD', 'VBM_WM', 'VBM_GM']
 
-        def get_output_type(self, input_kind):
-            if input_kind == 'BOLD':
-                return 'timeseries'
+        def get_valid_inputs(self) -> list[str]:
+            return ["BOLD", "VBM_WM", "VBM_GM"]
+
+        def get_output_type(self, input_kind: str) -> str:
+            if input_kind == "BOLD":
+                return "timeseries"
             else:
-                return 'table'
+                return "vector"
 
-        def compute(self, input, extra_input):
+        def compute(
+           self,
+           input: dict[str, Any],
+           extra_input: dict[str, Any] | None = None,
+        ) -> dict[str, Any]:
             # Get the data
             data = input["data"]
 
             # Get the min of the voxels sizes and use it as the resolution
             resolution = np.min(data.header.get_zooms()[:3])
 
             # Load the parcellation
@@ -199,55 +243,53 @@
                 resolution=resolution,
             )
 
             # Create a masker
             masker = NiftiLabelsMasker(
                 labels_img=t_parcellation,
                 standardize=True,
-                memory='nilearn_cache',
+                memory="nilearn_cache",
                 verbose=5,
             )
 
             # mask the data
             out_values = masker.fit_transform([data])
 
             # Create the output dictionary
-            out = {"data": out_values, "columns": t_labels}
+            out = {"data": out_values, "col_names": t_labels}
 
-            # If its 3D (BOLD), name each row as "scan"
-            if out_values.shape[0] > 1:
-                out["row_names"] = "scan"
             return out
 
 
 .. _extending_markers_template:
 
 Template for a custom Marker
 ----------------------------
 
 .. code-block:: python
 
     from junifer.api.decorators import register_marker
-    from junifer.markers.base import BaseMarker
+    from junifer.markers import BaseMarker
+
 
     @register_marker
     class TemplateMarker(BaseMarker):
 
         def __init__(self, on=None, name=None):
             # TODO: add marker-specific parameters
             super().__init__(on=on, name=name)
-        
+
         def get_valid_inputs(self):
             # TODO: Complete with the valid inputs
             valid = []
             return valid
 
         def get_output_type(self, input_kind):
             # TODO: Return the valid output kind for each input kind
             pass
 
         def compute(self, input, extra_input):
             # TODO: compute the marker and create the output dictionary
 
             # Create the output dictionary
-            out = {"data": None, "columns": None}
+            out = {"data": None, "col_names": None}
             return out
```

### Comparing `junifer-0.0.2.dev86/docs/faq.rst` & `junifer-0.0.3.dev36/docs/faq.rst`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 The following steps are specific to VSCode and you can choose to go with it:
 
 1. After forking the repository on GitHub, you can clone the forked repository
    using the internal version control tool.
 
 2. We recommend using ``conda`` to create your virtual environment
 
-   .. code-block:: console
+   .. code-block:: bash
 
-       conda env create -n <your-environment-name> -f conda-env.yml python=3.9
+       conda env create -n <your-environment-name> -f conda-env.yml python=3.10
        conda activate <your-environment-name>
 
    The ``conda-env.yml`` can be found at the root of the repository.
 
 The required development tools should be installed and you should be good to go.
```

### Comparing `junifer-0.0.2.dev86/docs/images/junifer_logo.png` & `junifer-0.0.3.dev36/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/docs/index.rst` & `junifer-0.0.3.dev36/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 
 .. toctree::
    :numbered: 3
    :maxdepth: 2
    :caption: Contents:
 
    installation
+   starting
    understanding/index.rst
    using/index.rst
    builtin
    extending/index.rst
    auto_examples/index.rst
    api/index.rst
+   help
    contribution
    maintaining
    faq
    whats_new
 
 
 Indices and tables
@@ -43,10 +45,12 @@
 * :ref:`search`
 
 
 Funding
 =======
 
 We thank the `Helmholtz Imaging Platform <https://helmholtz-imaging.de/>`_,
-`SMHB <https://www.fz-juelich.de/en/smhb>`_ and `eBRAIN Health <https://www.ebrain-health.eu/>`_ 
-(HORIZON-INFRA-2021-TECH-01) for supporting development of Junifer.
-(The funding sources had no role in the design, implementation and evaluation of the pipeline.)
+`SMHB <https://www.fz-juelich.de/en/smhb>`_ and
+`eBRAIN Health <https://www.ebrain-health.eu/>`_  (HORIZON-INFRA-2021-TECH-01)
+for supporting development of Junifer.
+(The funding sources had no role in the design, implementation and evaluation of
+the pipeline.)
```

### Comparing `junifer-0.0.2.dev86/docs/installation.rst` & `junifer-0.0.3.dev36/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,38 @@
 Requirements
 ------------
 
 junifer is compatible with `Python`_ >= 3.8 and requires the following packages:
 
 * ``click>=8.1.3,<8.2``
 * ``numpy>=1.22,<1.24``
-* ``datalad>=0.15.4,<0.18``
+* ``datalad>=0.15.4,<0.19``
 * ``pandas>=1.4.0,<1.6``
 * ``nibabel>=3.2.0,<4.1``
-* ``nilearn>=0.9.0,<1.0``
+* ``nilearn>=0.9.0,<=0.10.0``
 * ``sqlalchemy>=1.4.27,<= 1.5.0``
 * ``pyyaml>=5.1.2,<7.0``
+* ``h5py>=3.8.0,<3.9``
 
-Depending on the installation method, these packages might be installed automatically.
+Depending on the installation method, these packages might be installed
+automatically.
 
 Installation
 ------------
 
 Depending on your use-case, junifer can be installed differently:
 
 * Install the :ref:`install_latest_release`. This is the most suitable approach
   for end users.
 * Install from :ref:`install_development_git`. This is the most suitable approach
   for developers.
 
 
-Either way, we strongly recommend using `virtual environments <https://realpython.com/python-virtual-environments-a-primer>`_.
+Either way, we strongly recommend using
+`virtual environments <https://realpython.com/python-virtual-environments-a-primer>`_.
 
 
 .. _install_latest_release:
 
 Stable release
 ~~~~~~~~~~~~~~
 
@@ -55,44 +58,51 @@
 
 
 .. _installation_ext:
 
 Installing external dependencies
 ================================
 
-Some markers will require optional external dependencies to be installed. In this section you will
-find a list of all external dependencies that are required for specific markers.
+Some markers will require optional external dependencies to be installed. In
+this section you will find a list of all external dependencies that are required
+for specific markers.
 
 AFNI
 ----
 
 To install AFNI, you can always follow the `AFNI official instructions
-<https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/background_install/main_toc.html>`_. Additionally, you can also follow
-the following steps to install and configure the AFNI Docker container in your local system.
+<https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/background_install/main_toc.html>`_.
+Additionally, you can also follow the following steps to install and configure
+the AFNI Docker container in your local system.
 
 .. important::
 
-  The AFNI Docker container wrappers add the commands required by junifer. Using these commands have
-  some limitations, mostly related to handling files and paths. Junifer knows about this and uses these
-  commands in the proper way. Keep this in mind if you try to use the AFNI Docker wrappers outside of junifer.
-  These caveats and limitations are not documented.
+   The AFNI Docker container wrappers add the commands required by junifer. Using
+   these commands have some limitations, mostly related to handling files and
+   paths. Junifer knows about this and uses these commands in the proper way.
+   Keep this in mind if you try to use the AFNI Docker wrappers outside of
+   junifer. These caveats and limitations are not documented.
+
+1. Install Docker. You can follow the
+   `Docker official instructions <https://docs.docker.com/get-docker/>`_.
+2. Pull the AFNI Docker image from
+   `Docker Hub <https://hub.docker.com/r/afni/afni>`_:
 
-1. Install Docker. You can follow the `Docker official instructions <https://docs.docker.com/get-docker/>`_.
-2. Pull the AFNI Docker image from `Docker Hub <https://hub.docker.com/r/afni/afni>`_:
-
-.. code-block:: shell
+.. code-block:: bash
 
   docker pull afni/afni_make_build
 
-3. Add the Junifer AFNI scripts to your PATH environmental variable. Run the following command:
+3. Add the Junifer AFNI scripts to your PATH environmental variable. Run the
+   following command:
 
-.. code-block:: shell
+.. code-block:: bash
 
   junifer setup afni-docker
 
 Take the last line and copy it to your ``.bashrc`` or ``.zshrc`` file.
 
-Or, alternatively, you can exceute this command which will update the ``~/.bashrc`` for you:
+Or, alternatively, you can exceute this command which will update the
+``~/.bashrc`` for you:
 
-.. code-block:: shell
+.. code-block:: bash
 
   junifer setup afni-docker | grep "PATH=" | xargs | >> ~/.bashrc
```

### Comparing `junifer-0.0.2.dev86/docs/links.inc` & `junifer-0.0.3.dev36/docs/links.inc`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 .. _`venv`: https://docs.python.org/3/tutorial/venv.html
 .. _`conda env`: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
 
 .. _`Github`: https://github.com/
 .. _`junifer Github`: https://github.com/juaml/junifer
 .. _`junifer Discussions`: https://github.com/juaml/junifer/discussions
+.. _`junifer matrix channel`: https://matrix.to/#/#junifer-gen:inm7.de
 
 .. _`Wikipedia`: https://wikipedia.org
 .. _`YAML`: https://yaml.org
 
 .. _`setuptools_scm`: https://github.com/pypa/setuptools_scm/
 
 .. _`sphinx gallery`: https://sphinx-gallery.github.io/stable/index.html
```

### Comparing `junifer-0.0.2.dev86/docs/maintaining.rst` & `junifer-0.0.3.dev36/docs/maintaining.rst`

 * *Files 11% similar despite different names*

```diff
@@ -20,47 +20,68 @@
 version "X.Y.Z". Additionally, for every push to main, it will be published
 as pre-release to PyPI.
 
 Releasing a new version
 -----------------------
 
 Once the milestone is reached (all issues closed), it is time to do a new
-release.
+release. Make sure you have
+`towncrier <https://towncrier.readthedocs.io/en/stable/index.html>`_ installed
+before proceeding.
 
-1. Open a PR to update documentation:
-    - `docs/changes/latest.inc` should now be renamed to the version to be
-      released.
-    - `docs/whats_new.rst` must update the link to the new version.
+#. Make sure you are in sync with the main branch.
 
-2. Merge PR
+.. code-block:: bash
+
+    git checkout main
+    git pull --rebase origin main
+
+#. Run the following to check changelog is properly generated:
+
+.. code-block:: bash
+
+   towncrier build --draft
+
+#. Then, run:
+
+.. code-block:: bash
+
+   towncrier
+
+to generate the proper changelog that should be reflected in
+``docs/whats_new.rst``.
+
+#. Commit the chages, make a PR and merge via a merge commit.
 
-3. Make sure you are in sync with the main branch.
+#. Make sure you are in sync with the main branch.
 
 .. code-block:: bash
 
     git checkout main
     git pull --rebase origin main
 
-4. Create tag (replace ``X.Y.Z`` with the proper version).
+#. Create tag (replace ``X.Y.Z`` with the proper version) on the merged PR's
+   merge commit.
 
 .. code-block:: bash
 
     git tag -a vX.Y.Z -m "Release X.Y.Z"
 
-5. Check that the build system is creating the proper version
+#. Check that the build system is creating the proper version
 
 .. code-block:: bash
 
     SETUPTOOLS_SCM_DEBUG=1 python -m build --source --binary --out-dir dist/ .
 
-6. Push the tag
+#. Push the tag
 
 .. code-block:: bash
 
     git push origin --follow-tags
 
-7. Optional: bump the *MAJOR* or *MINOR* segment of next release (replace ``D.E.0`` with the proper version).
+#. Optional: bump the *MAJOR* or *MINOR* segment of next release (replace
+   ``D.E.0`` with the proper version).
 
 .. code-block:: bash
 
     git tag -a vD.E.0.dev -m "Set next release to D.E.0"
     git push origin --follow-tags
```

### Comparing `junifer-0.0.2.dev86/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.3.dev36/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/docs/understanding/datagrabber.rst` & `junifer-0.0.3.dev36/docs/understanding/datagrabber.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,51 +4,62 @@
 
 Data Grabber
 ============
 
 Description
 -----------
 
-The *Data Grabber* is an object that can provide an interface to datasets you want to work with in junifer.
-Every concrete implementation of a datagrabber is aware of a particular dataset's structure and thus allows
-you to fetch specific elements of interest from the dataset. It adds the ``path`` key to each :ref:`data type <data_types>`
-in the :ref:`Data object <data_object>`.
-
-Datagrabbers are intended to be used as context managers. When used within a context, a datagrabber takes care
-of any pre and post steps for interacting with the dataset, for example, downloading and cleaning up. As the interface
+The ``DataGrabber`` is an object that can provide an interface to datasets you
+want to work with in junifer. Every concrete implementation of a datagrabber is
+aware of a particular dataset's structure and thus allows you to fetch specific
+elements of interest from the dataset. It adds the ``path`` key to each
+:ref:`data type <data_types>` in the :ref:`Data object <data_object>`.
+
+Datagrabbers are intended to be used as context managers. When used within a
+context, a datagrabber takes care of any pre and post steps for interacting with
+the dataset, for example, downloading and cleaning up. As the interface
 is consistent, you always use the same procedure to interact with the datagrabber.
 
-For example, a concrete implementation of :class:`junifer.datagrabber.DataladDataGrabber` can provide junifer
-with data from a Datalad dataset. Of course, datagrabbers are not only meant to work with Datalad datasets but
-any dataset.
-
-If you are interested in using already provided datagrabbers, please go to :doc:`../builtin`. And, if you want
-to implement your own datagrabber, you need to provide concrete implementations of base classes already
-provided.
+For example, a concrete implementation of :class:`.DataladDataGrabber` can
+provide junifer with data from a Datalad dataset. Of course, datagrabbers are not
+only meant to work with Datalad datasets but any dataset.
+
+If you are interested in using already provided datagrabbers, please go to
+:doc:`../builtin`. And, if you want to implement your own datagrabber, you need
+to provide concrete implementations of base classes already provided.
 
-Base classes
+Base Classes
 ------------
 
-In this section, we showcase different abstract base classes you might want to use to implement your own datagrabber.
+In this section, we showcase different abstract base classes you might want to
+use to implement your own datagrabber.
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Description
-   * - :class:`junifer.datagrabber.BaseDataGrabber`
-     - | The abstract base class providing you an interface to implement your own datagrabber.
-       | You should try to avoid using this directly and instead use
-       | :class:`junifer.datagrabber.PatternDataGrabber` or :class:`junifer.datagrabber.DataladDataGrabber`.
-       | To build your own custom *low-level* datagrabber, you need to at least implement the ``get_elements`` method,
-       | but most of the time you should also override other existing methods like ``__enter__`` and ``__exit__``.
-   * - :class:`junifer.datagrabber.PatternDataGrabber`
-     - | It implements functionality to help you define the pattern of the dataset you want to get. For example,
-       | you know that T1 images are found in a directory following this pattern ``{subject}/anat/{subject}_T1w.nii.gz``
-       | inside of the dataset. Now you can provide this to the **PatternDataGrabber** and it will be able to get the file.
-   * - :class:`junifer.datagrabber.DataladDataGrabber`
-     - | It implements functionality to deal with Datalad datasets. Specifically, the ``__enter__`` and ``__exit__`` methods
-       | take care of cloning and removing the Datalad dataset.
-   * - :class:`junifer.datagrabber.PatternDataladDataGrabber`
-     - | It is a combination of :class:`junifer.datagrabber.PatternDataladDataGrabber` and
-       | :class:`junifer.datagrabber.DataladDataGrabber`. This is probably the class you are looking for when using Datalad.
+   * - :class:`.BaseDataGrabber`
+     - | The abstract base class providing you an interface to implement your
+       | own datagrabber. You should try to avoid using this directly and
+       | instead use :class:`.PatternDataGrabber` or
+       | :class:`.DataladDataGrabber`. To build your own custom *low-level*
+       | datagrabber, you need to override the ``get_elements_keys``,
+       | ``get_elements`` and ``get_item`` methods, and most of the time you
+       | should also override other existing methods like ``__enter__`` and
+       | ``__exit__``.
+   * - :class:`.PatternDataGrabber`
+     - | It implements functionality to help you define the pattern of the
+       | dataset you want to get. For example, you know that T1 images are
+       | found in a directory following the pattern:
+       | ``{subject}/anat/{subject}_T1w.nii.gz`` inside of the dataset. Now you
+       | can provide this to the :class:`.PatternDataGrabber` and it will be
+       | able to get the file.
+   * - :class:`.DataladDataGrabber`
+     - | It implements functionality to deal with Datalad datasets. Specifically,
+       | the ``__enter__`` and ``__exit__`` methods take care of cloning and
+       | removing the Datalad dataset.
+   * - :class:`.PatternDataladDataGrabber`
+     - | It is a combination of :class:`.PatternDataGrabber` and
+       | :class:`.DataladDataGrabber`. This is probably the class you are looking
+       | for when using Datalad datasets.
```

### Comparing `junifer-0.0.2.dev86/docs/understanding/datareader.rst` & `junifer-0.0.3.dev36/docs/understanding/datareader.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 
 Data Reader
 ===========
 
 Description
 -----------
 
-The *Data Reader* is an object that is responsible for actually reading data files in junifer.
-It reads the value of the key ``path`` for each :ref:`data type <data_types>` in the :ref:`Data object <data_object>`
-and loads them to memory. After reading the data into memory, it adds the key ``data`` to the same level as ``path``
-and the value is the actual data in the memory.
-
-Datareaders are meant to be used inside the datagrabber context but you can operate on them outside the context as long
-as the actual data is in the memory and the Python runtime has not garbage-collected it.
+The ``DataReader`` is an object that is responsible for actually reading data
+files in junifer. It reads the value of the key ``path`` for each
+:ref:`data type <data_types>` in the :ref:`Data object <data_object>` and loads
+them into memory. After reading the data into memory, it adds the key ``data``
+to the same level as ``path`` and the value is the actual data in the memory.
+
+Datareaders are meant to be used inside the datagrabber context but you can
+operate on them outside the context as long as the actual data is in the memory
+and the Python runtime has not garbage-collected it.
 
-For data formats not supported by junifer yet, you can either make your own *Data Reader* or open an issue on
-`junifer Github`_ and we can help you out.
+For data formats not supported by junifer yet, you can either make your own
+*Data Reader* or open an issue on `junifer Github`_ and we can help you out.
 
-Currently supported file-formats
---------------------------------
+File Formats
+------------
 
-We already provide a concrete implementation :class:`junifer.datareader.DefaultDataReader` which knows how to
-read the following file formats:
+We already provide a concrete implementation :class:`.DefaultDataReader` which
+knows how to read the following file formats:
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - File extension
      - File type
```

### Comparing `junifer-0.0.2.dev86/docs/understanding/index.rst` & `junifer-0.0.3.dev36/docs/understanding/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 =====================
 
 Before you start, you should understand how junifer works. Junifer is a
 tool conceived to extract features from neuroimaging data in an easy-to-use
 manner, with minimal coding and minimal user expertise in the internal aspects.
 
 Unlike other tools like FSL, SPM, AFNI, etc., junifer is not a toolbox to
-pre-process data, but a toolbox to extract features from previously pre-processed
-data.
+pre-process data, but a toolbox to extract features from previously
+pre-processed data.
 
 The main idea is that you have a set of images (e.g. a set of functional MRI,
 structural MRI, diffusion MRI, etc.) and you want to extract features to
 later use in statistical analyses or machine learning (for example, using
 julearn_).
 
-.. important:: Junifer is not a toolbox to create pipelines, but a tool to configure the junifer pipeline, which is
-   intended to be fixed and not to be changed. If you want to create a pipeline, you should use
-   other tools like nipype_.
+.. important::
+
+   Junifer is not a toolbox to create pipelines, but a tool to configure the
+   junifer pipeline, which is intended to be fixed and not to be changed. If you
+   want to create a pipeline, you should use other tools like nipype_.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    pipeline
    data
```

### Comparing `junifer-0.0.2.dev86/docs/understanding/marker.rst` & `junifer-0.0.3.dev36/docs/understanding/marker.rst`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,29 @@
 
 Marker
 ======
 
 Description
 -----------
 
-The ``Marker`` is an object that is responsible for feature extraction. It primarily operates on data loaded
-in memory by :ref:`Data Reader <datareader>` and stored in the ``data`` key of each :ref:`data type <data_types>`
-in the :ref:`Data object <data_object>`. In some cases, it can also operate on pre-processed data as obtained
-from the :ref:`Preprocess <preprocess>` step of the pipeline. It is important to note that this pre-process is
-not similar to pre-processing done by tools like FSL, SPM, AFNI, etc. . For example, one can perform confound
-removal on loaded data and then perform feature extraction.
-
-Markers are meant to be used inside the datagrabber context but you can operate on them outside the context as long
-as the actual data is in the memory and the Python runtime has not garbage-collected it.
-
-If you are interested in using already provided markers, please go to :doc:`../builtin`. And, if you want to implement
-your own marker, you need to provide concrete implementation of :class:`junifer.markers.BaseMarker`. Specifically, you
-need to override ``get_output_type``, ``store`` and ``compute`` methods.
+The ``Marker`` is an object that is responsible for feature extraction. It
+primarily operates on data loaded into memory by :ref:`Data Reader <datareader>`
+and stored in the ``data`` key of each :ref:`data type <data_types>` in the
+:ref:`Data object <data_object>`. In some cases, it can also operate on
+pre-processed data as obtained from the :ref:`Preprocess <preprocess>` step of
+the pipeline.
+
+.. important::
+
+   This pre-process is not similar to pre-processing done by tools like FSL,
+   SPM, AFNI, etc., . For example, one can perform confound removal on loaded
+   data and then perform feature extraction.
+
+Markers are meant to be used inside the datagrabber context but you can operate
+on them outside the context as long as the actual data is in the memory and the
+Python runtime has not garbage-collected it.
+
+If you are interested in using already provided markers, please go to
+:doc:`../builtin`. And, if you want to implement your own marker, you need to
+provide concrete implementation of :class:`.BaseMarker`. Specifically, you
+need to override ``get_valid_inputs``, ``get_output_type`` and ``compute``
+methods.
```

### Comparing `junifer-0.0.2.dev86/docs/understanding/preprocess.rst` & `junifer-0.0.3.dev36/docs/understanding/preprocess.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,101 +4,113 @@
 
 Preprocess
 ==========
 
 Description
 -----------
 
-The ``Preprocess`` step of the pipeline is meant for pre-processing before or after :ref:`Marker <marker>` step
-depending on the use-case. For example, you might want to perform confound removal on ``BOLD`` data before
-feature extraction.
+The ``Preprocess`` is an object meant for pre-processing before or after
+:ref:`Marker <marker>` step depending on the use-case. For example, you might
+want to perform confound removal on ``BOLD`` data before feature extraction.
 
-This step is still under development and is an optional one for the pipeline to work.
+
+.. note::
+
+   This step is optional for the pipeline to work.
 
 .. _preprocess_confounds:
 
 Confound Removal
 ----------------
 
-The *Confound Removal* step is meant to remove *confounds* from the ``BOLD`` data. The confounds are
-extracted from the ``BOLD_confounds`` data (must be provided by the :ref:`Data Grabber <datagrabber>`).
-The confounds are then regressed out from the ``BOLD`` data using :func:`nilearn.image.clean_img`.
-
-Currently, junifer supports only one confound removal class: 
-:class:`junifer.preprocess.fMRIPrepConfoundRemover`. This class is meant to remove confounds as described
-before, using the output of `fMRIPrep`_ as reference.
+The *Confound Removal* step is meant to remove *confounds* from the ``BOLD``
+data. The confounds are extracted from the ``BOLD_confounds`` data (must be
+provided by the :ref:`Data Grabber <datagrabber>`). The confounds are then
+regressed out from the ``BOLD`` data using :func:`nilearn.image.clean_img`.
+
+Currently, junifer supports only one confound removal class:
+:class:`.fMRIPrepConfoundRemover`. This class is meant to remove confounds as
+described before, using the output of `fMRIPrep`_ as reference.
 
 Strategy
 ~~~~~~~~
 
-This confound remover uses the `nilearn`_ API from :func:`nilearn.interfaces.fmriprep.load_confounds`. That is,
-define a *strategy* to extract the confounds from the ``BOLD_confounds`` data. The *strategy* is defined
-by choosing the *noise components* to be used and the *confounds* to be extracted from each noise components.
-The *noise components* currently supported are:
+This confound remover uses the `nilearn`_ API from
+:func:`nilearn.interfaces.fmriprep.load_confounds`. That is, define a *strategy*
+to extract the confounds from the ``BOLD_confounds`` data. The *strategy* is
+defined by choosing the *noise components* to be used and the *confounds* to be
+extracted from each noise components. The *noise components* currently supported
+are:
 
 * ``motion``
 * ``wm_csf``
 * ``global_signal``
 
 The confounds options for each *noise component* are:
 
-* ``basic``: the basic confounds for each *noise component*. For example, for ``motion``, the basic confounds
-  are the 6 motion parameters (3 translations and 3 rotations). For ``wm_csf``, the basic
-  confounds are the mean signal of the white matter and CSF regions. For ``global_signal``, the basic confound
+* ``basic``: the basic confounds for each *noise component*. For example, for
+  ``motion``, the basic confounds are the 6 motion parameters (3 translations
+  and 3 rotations). For ``wm_csf``, the basic confounds are the mean signal of
+  the white matter and CSF regions. For ``global_signal``, the basic confound
   is the mean signal of the whole brain.
 * ``power2``: the basic confounds plus the square of each basic confound.
-* ``derivatives``: the basic confounds plus the derivative of each basic confound.
-* ``full``: the basic confounds, the derivative of each basic confound, the square of each basic confound and the
-  square of each derivative of each basic confound.
+* ``derivatives``: the basic confounds plus the derivative of each basic
+  confound.
+* ``full``: the basic confounds, the derivative of each basic confound, the
+  square of each basic confound and the square of each derivative of each basic
+  confound.
 
-The *strategy* is defined as a dictionary, with the *noise components* as keys and the *confounds* as values.
+The *strategy* is defined as a dictionary, with the *noise components* as keys
+and the *confounds* as values.
 
 Example in python format:
 
-.. code-block:: 
+.. code-block:: python
 
     strategy = {
         "motion": "basic",
         "wm_csf": "full",
         "global_signal": "derivatives"
     }
 
 or in YAML format:
 
-.. code-block:: 
-    
+.. code-block:: yaml
+
     strategy:
         motion: basic
         wm_csf: full
         global_signal: derivatives
 
 The default value is to use all the *noise components* with the ``full`` *confounds*:
 
-.. code-block:: 
+.. code-block:: python
 
     strategy = {
         "motion": "full",
         "wm_csf": "full",
         "global_signal": "full"
     }
 
-Other parameters
+Other Parameters
 ~~~~~~~~~~~~~~~~
 
-Additionaly, the :class:`junifer.preprocess.fMRIPrepConfoundRemover` supports the following parameters:
+Additionaly, the :class:`.fMRIPrepConfoundRemover` supports the following
+parameters:
 
 .. list-table::
-   :widths: 10, 30, 5
+   :widths: auto
    :header-rows: 1
 
    * - Parameter
      - Description
      - Default
    * - ``spike``
-     - Add a spike regressor in the timepoints when the framewise displacement exceeds this threshold.
+     - | Add a spike regressor in the timepoints when the framewise
+       | displacement exceeds this threshold.
      - deactivated
    * - ``detrend``
      - Apply detrending on timeseries, before confound removal.
      - activated
    * - ``standardize``
      - Scale signals to unit variance.
      - activated
@@ -108,9 +120,11 @@
    * - ``high_pass``
      - High cutoff frequencies, in Hertz.
      - deactivated
    * - ``t_r``
      - Repetition time, in second (sampling period).
      - from nifti header
    * - ``mask``
-     - If provided, signal is only cleaned from voxels inside the mask. If not, a mask is computed using :func:`nilearn.masking.compute_brain_mask`.
-     - compute
+     - | If provided, signal is only cleaned from voxels inside the mask.
+       | If not, a mask is computed using
+       | :func:`nilearn.masking.compute_brain_mask`.
+     - compute
```

### Comparing `junifer-0.0.2.dev86/docs/understanding/storage.rst` & `junifer-0.0.3.dev36/docs/understanding/storage.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,67 +4,76 @@
 
 Storage
 =======
 
 Description
 -----------
 
-The ``Storage`` is an object that is responsible for storing extracted features as computed from :ref:`Marker <marker>`
-step of the pipeline. If the pipeline is provided with a ``storage-like`` object, the extracted features are stored via
+The ``Storage`` is an object that is responsible for storing extracted features
+as computed from :ref:`Marker <marker>` step of the pipeline. If the pipeline is
+provided with a ``storage-like`` object, the extracted features are stored via
 that object else they are kept in memory.
 
-Storage is meant to be used inside the datagrabber context but you can operate on them outside the context as long
-as the processed data is in the memory and the Python runtime has not garbage-collected it.
-
-The :ref:`Markers <marker>` are responsible for defining what *storage kind* (``matrix``, ``table``, ``timeseries``)
-they support for which :ref:`data type <data_types>` by overriding its ``store`` method. The storage object in turn
-declares and provides implementation for specific *storage kind*. For example, :class:`junifer.storage.SQLiteFeatureStorage`
-supports saving ``matrix``, ``table`` and ``timeseries`` via ``store_matrix``, ``store_table`` and ``store_timeseries``
-methods respectively.
-
-For storage interfaces not supported by junifer yet, you can either make your own ``Storage`` by providing a concrete
-implementation of :class:`junifer.storage.BaseFeatureStorage` or open an issue on `junifer Github`_ and we can help you out.
-
+Storage is meant to be used inside the datagrabber context but you can operate
+on them outside the context as long as the processed data is in the memory and
+the Python runtime has not garbage-collected it.
+
+The :ref:`Markers <marker>` are responsible for defining what *storage kind*
+(``matrix``, ``vector``, ``timeseries``) they support for which
+:ref:`data type <data_types>` by overriding its ``get_output_type`` method. The
+storage object in turn declares and provides implementation for specific
+*storage kind*. For example, :class:`.SQLiteFeatureStorage` supports saving
+``matrix``, ``vector`` and ``timeseries`` via ``store_matrix``, ``store_vector``
+and ``store_timeseries`` methods respectively.
+
+For storage interfaces not supported by junifer yet, you can either make your
+own ``Storage`` by providing a concrete implementation of
+:class:`.BaseFeatureStorage` or open an issue on `junifer Github`_ and we can
+help you out.
 
 .. _storage_types:
 
-Currently supported storage types
----------------------------------
+Storage Types
+-------------
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Storage Type
      - Description
      - Options
      - Reference
    * - ``matrix``
      - A 2D matrix with row and column names
      -  ``col_names``, ``row_names``, ``matrix_kind``, ``diagonal``
-     -  :meth:`junifer.storage.BaseFeatureStorage.store_matrix`
-   * - ``table``
-     - A vector of values with column names
-     - ``columns``, ``row_names``
-     -  :meth:`junifer.storage.BaseFeatureStorage.store_table`
+     -  :meth:`.BaseFeatureStorage.store_matrix`
+   * - ``vector``
+     - A 1D row vector of values with column names
+     - ``col_names``
+     -  :meth:`.BaseFeatureStorage.store_vector`
    * - ``timeseries``
      - A 2D matrix of values with column names
-     - ``columns``, ``row_names``
-     -  :meth:`junifer.storage.BaseFeatureStorage.store_timeseries`
-  
+     - ``col_names``
+     -  :meth:`.BaseFeatureStorage.store_timeseries`
+
 .. _storage_interfaces:
 
-Currently supported storage interfaces
---------------------------------------
+Storage Interfaces
+------------------
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Storage class
      - File extension
      - File type
      - Storage kinds
-   * - :class:`junifer.storage.SQLiteFeatureStorage`
+   * - :class:`.SQLiteFeatureStorage`
      - ``.sqlite``
      - SQLite
-     - ``matrix``, ``table``, ``timeseries``
+     - ``matrix``, ``vector``, ``timeseries``
+   * - :class:`.HDF5FeatureStorage`
+     - ``.hdf5``
+     - HDF5
+     - ``matrix``, ``vector``, ``timeseries``
```

### Comparing `junifer-0.0.2.dev86/docs/using/codeless.rst` & `junifer-0.0.3.dev36/docs/using/codeless.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,145 +1,172 @@
 .. include:: ../links.inc
 
 .. _codeless:
 
-Code-less configuration
+Code-less Configuration
 =======================
 
-On of the most important features of junifer is its capacity to run without writing a single line of code. This is
-achieved by using a configuration file that is written in YAML_. In this file, we configure the different steps of
+On of the most important features of junifer is its capacity to run without
+writing a single line of code. This is achieved by using a configuration file
+that is written in YAML_. In this file, we configure the different steps of
 :ref:`pipeline`.
 
 As a reminder, this is how the pipeline looks like:
 
-.. image:: ../images/pipeline/pipeline.001.png
+.. mermaid::
 
-Thus, the configuration file must configure each of the sections of the pipeline, as well as some general parameters.
-
-As an example, we will generate the configuration file for a pipeline that will extract the mean ``VBM_GM`` values
-using two different parcellations and one set of coordinates, from the *Oasis VBM Testing dataset* included in
-junifer.
+   flowchart LR
+     dg[Data Grabber]
+     dr[Data Reader]
+     pp[Pre-processing]
+     mc[Marker Computation]
+     st[Storage]
+     dg --> dr
+     dr --> pp
+     pp --> mc
+     mc --> st
+
+
+Thus, the configuration file must configure each of the sections of the pipeline,
+as well as some general parameters.
+
+As an example, we will generate the configuration file for a pipeline that will
+extract the mean ``VBM_GM`` values using two different parcellations and one set
+of coordinates, from the ``Oasis VBM Testing dataset`` included in junifer.
 
 
 General Parameters
 ------------------
 
-The general parameters are the ones that are not specific to any of the sections of the pipeline, but configure
-junifer as a whole. These parameters are:
+The general parameters are the ones that are not specific to any of the sections
+of the pipeline, but configure junifer as a whole. These parameters are:
 
 * ``with``: A section used to specify modules and junifer extensions to use.
 * ``workdir``: The working directory where junifer will store temporary files.
 
-Since the example uses a specific datagrabber for testing, we need to add ``junifer.testing.registry`` to the
-``with`` section. This will allow junifer to find the datagrabber. We will set the ``workdir`` to ``/tmp``.
+Since the example uses a specific datagrabber for testing, we need to add
+``junifer.testing.registry`` to the ``with`` section. This will allow junifer
+to find the datagrabber. We will set the ``workdir`` to ``/tmp``.
 
 .. code-block:: yaml
 
   with: junifer.testing.registry
+
   workdir: /tmp
 
-Step-by-step configuration
+Step-by-step Configuration
 --------------------------
 
 In order to configure the pipeline, we need to configure each step:
 
 * ``datagrabber``
 * ``datareader``
 * ``preprocess``
 * ``markers``
 * ``storage``
 
-.. important:: The datareader step configuration is optional, as junifer only provides one datareader. Nevertheless,
-    it is possible to extend junifer with custom datareaders, and thus, it is also possible to configure this step.
+.. important::
+
+   The datareader step configuration is optional, as junifer only provides one
+   datareader. Nevertheless, it is possible to extend junifer with custom
+   datareaders, and thus, it is also possible to configure this step.
 
 
 Data Grabber
 ^^^^^^^^^^^^
 
-The ``datagrabber`` section must be configured using the ``kind`` key to specify the datagrabber to use. Additional
-keys correspond to the parameters of the datagrabber.
+The ``datagrabber`` section must be configured using the ``kind`` key to specify
+the datagrabber to use. Additional keys correspond to the parameters of the
+datagrabber.
 
-For example, to use the :class:`junifer.datagrabber.DataladAOMICPIOP1` datagrabber, we just need to
+For example, to use the :class:`.DataladAOMICPIOP1` datagrabber, we just need to
 specify its name as the ``kind`` key.
 
 .. code-block:: yaml
 
   datagrabber:
     kind: DataladAOMICPIOP1
 
-However, it is also possible to pass parameters to the datagrabber. In this case, we can restrict the datagrabber to
-fetch only the  ``restingstate`` task.
+However, it is also possible to pass parameters to the datagrabber. In this case,
+we can restrict the datagrabber to fetch only the ``restingstate`` task.
 
 .. code-block:: yaml
 
   datagrabber:
     kind: DataladAOMICPIOP1
     tasks: restingstate
 
-In the *Oasis VBM Testing dataset* example, the section will look like this:
+In the ``Oasis VBM Testing dataset`` example, the section will look like this:
 
 .. code-block:: yaml
 
   datagrabber:
-    kind: OasisVBMTesting
+    kind: OasisVBMTestingDatagrabber
 
 
 Data Reader
 ^^^^^^^^^^^
 
-As mentioned before, this section is entirely optional, as junifer only provides one data reader
-(:class:`junifer.datareader.DefaultDataReader`), which is the default in case the section is not specified.
-
-In any case, the syntax of the section is the same as for the ``datagrabber`` section, using the ``kind`` key to
-specify the data reader to use, and additional keys to pass parameters to the data reader:
+As mentioned before, this section is entirely optional, as junifer only provides
+one data reader (:class:`.DefaultDataReader`), which is the default in case the
+section is not specified.
+
+In any case, the syntax of the section is the same as for the ``datagrabber``
+section, using the ``kind`` key to specify the datareader to use, and additional
+keys to pass parameters to the datareader:
 
 .. code-block:: yaml
 
     datareader:
       kind: DefaultDataReader
 
 
-For the *Oasis VBM Testing dataset* example, we will not specify a ``datareader`` step.
+For the ``Oasis VBM Testing dataset`` example, we will not specify a
+``datareader`` step.
 
-Preprocessing
-^^^^^^^^^^^^^
+Preprocess
+^^^^^^^^^^
 
-Preprocessing is also an optional step, as it might be the case that no pre-processing is needed. In the case that
-preprocessing is needed, the section must be configured using the ``kind`` key to specify the preprocessor to use,
+Pre-processing is also an optional step, as it might be the case that no
+pre-processing is needed. In the case that pre-processing is needed, the section
+must be configured using the ``kind`` key to specify the preprocessor to use,
 and additional keys to pass parameters to the preprocessor.
 
-For example, to use the :class:`junifer.preprocess.fMRIPrepConfoundRemover` preprocessor, we just need to specify its
-name as the ``kind`` key, as well as its parameters.
-
+For example, to use the :class:`.fMRIPrepConfoundRemover` preprocessor, we just
+need to specify its name as the ``kind`` key, as well as its parameters.
 
 .. code-block:: yaml
 
   preprocess:
     kind: fMRIPrepConfoundRemover
     strategy:
       motion: full
       wm_csf: full
       global_signal: basic
     spike: 0.2
     detrend: false
     standardize: true
 
 
-For the *Oasis VBM Testing dataset* example, we will not specify a preprocessing step.
-
+For the ``Oasis VBM Testing dataset`` example, we will not specify a
+preprocessing step.
 
-Markers
-^^^^^^^
 
-The ``markers`` section diverges from the previous ones, as we need to specify a list of markers. Each marker has a
-name that we can use to refer to it later, and a set of parameters that will be passed to the marker.
+Marker
+^^^^^^
 
-For the *Oasis VBM Testing dataset* example, we want to compute the mean ``VBM_GM`` value for each parcel using the
-Schaefer parcellation (100 parcels, 7 networks), Schaefer parcellation (200 parcels, 7 networks), and the *DMNBuckner*
-network, using 5mm spheres. Thus, we will configure the ``markers`` section as follows:
+The ``markers`` section diverges from the previous ones, as we need to specify
+a list of markers. Each marker has a name that we can use to refer to it later,
+and a set of parameters that will be passed to the marker.
+
+For the ``Oasis VBM Testing dataset`` example, we want to compute the mean
+``VBM_GM`` value for each parcel using the ``Schaefer parcellation (100 parcels,
+7 networks)``, ``Schaefer parcellation (200 parcels, 7 networks)``, and the
+``DMNBuckner`` network, using ``5mm`` spheres. Thus, we will configure the
+``markers`` section as follows:
 
 .. code-block:: yaml
 
   markers:
     - name: Schaefer100x7_mean
       kind: ParcelAggregation
       parcellation: Schaefer100x7
@@ -154,39 +181,42 @@
       radius: 5
       method: mean
 
 
 Storage
 ^^^^^^^
 
-Finally, we need to define how and where the results will be stored. This is done using the ``storage`` section,
-which must be configured using the ``kind`` key to specify the storage to use, and additional keys to pass parameters.
+Finally, we need to define how and where the results will be stored. This is
+done using the ``storage`` section, which must be configured using the ``kind``
+key to specify the storage to use, and additional keys to pass parameters.
 
-For example, to use the :class:`junifer.storage.SQLiteFeatureStorage` storage, we just need to specify where we want
-to store the results:
+For example, to use the :class:`.SQLiteFeatureStorage` storage, we just need to
+specify where we want to store the results:
 
 .. code-block:: yaml
 
     storage:
       kind: SQLiteFeatureStorage
       uri: /data/junifer/example/oasis_vbm_testing.sqlite
 
 
-The full example
+Complete Example
 ----------------
 
-This is how the full *Oasis VBM Testing dataset* example configuration file looks like:
+This is how the full ``Oasis VBM Testing dataset`` example configuration file
+looks like:
 
 .. code-block:: yaml
 
   with: junifer.testing.registry
+
   workdir: /tmp
 
   datagrabber:
-    kind: OasisVBMTesting
+    kind: OasisVBMTestingDatagrabber
 
   markers:
     - name: Schaefer100x7_mean
       kind: ParcelAggregation
       parcellation: Schaefer100x7
       method: mean
     - name: Schaefer200x7_mean
```

### Comparing `junifer-0.0.2.dev86/docs/using/queueing.rst` & `junifer-0.0.3.dev36/docs/using/queueing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 .. include:: ../links.inc
 
 .. _queueing:
 
-Queueing jobs (HPC, HTC)
+Queueing Jobs (HPC, HTC)
 ========================
 
-Yet another interesting feature of junifer is the ability to queue jobs on computational clusters. This is done by
-adding the ``queue`` section in the :ref:`codeless` file and executing the  ``junifer queue`` command.
-
-While junifer is meant to support `HTCondor`_, `SLURM`_ and local queueing using `GNU Parallel`_, only HTCondor is
-currently supported. This will be implemented in future relases of junifer. If you are in immediate need of any of these
-schedulers, please create an issue on the `junifer github`_ repository.
-
-The ``queue`` section of the :ref:`codeless` must start by defining the following general parameters:
-
-* ``jobname``: name of the job to be queued. This will be used to name the folder where the job files will be created,
-  as well as any relevant file. Depending on the scheduler, it will also be listed in the queueing system with this
-  name.
-* ``kind``: The kind of scheduler to be used. Currently, only ``HTCondor`` is supported.
+Yet another interesting feature of junifer is the ability to queue jobs on
+computational clusters. This is done by adding the ``queue`` section in the
+:ref:`codeless` file and executing the  ``junifer queue`` command.
+
+While junifer is meant to support `HTCondor`_, `SLURM`_ and local queueing
+using `GNU Parallel`_, only HTCondor is currently supported. This will be
+implemented in future relases of junifer. If you are in immediate need of any of
+these schedulers, please create an issue on the `junifer github`_ repository.
+
+The ``queue`` section of the :ref:`codeless` must start by defining the
+following general parameters:
+
+* ``jobname``: Name of the job to be queued. This will be used to name the
+  folder where the job files will be created, as well as any relevant file.
+  Depending on the scheduler, it will also be listed in the queueing system
+  with this name.
+* ``kind``: The kind of scheduler to be used. Currently, only ``HTCondor`` is
+  supported.
 
 Example:
 
 .. code-block:: yaml
 
   queue:
     jobname: TestHTCondorQueue
@@ -31,59 +36,77 @@
 The rest of the parameters depend on the scheduler you are using.
 
 .. _queueing_condor:
 
 HTCondor
 --------
 
-When using HTCondor, junifer will use a DAG to queue one job per element (``junifer run``). As an option, the DAG can
-include a final job (``junifer collect``) to collect the results once all of the individual element jobs are finished.
+When using HTCondor, junifer will use a DAG to queue one job per element
+(``junifer run``). As an option, the DAG can include a final job
+(``junifer collect``) to collect the results once all of the individual element
+jobs are finished.
 
 The following parameters are avilable for HTCondor:
 
-* ``env``: Definition of the Python enviroment. It must provide two variables: ``kind`` and ``name``. The ``kind``
-  corresponds to the kind of virtual environment to use: ``conda``,  ``virtualenv`` (not yet supported) or 
-  ``local`` (no virtual enviroment). The ``name`` is the name of the enviroment to use in case a virtual environment
-  is used.
-* ``mem``: Memory to be used by the job. It must be provided as a string with the units (e.g. ``2GB``).
+* ``env``: Definition of the Python enviroment. It must provide two variables:
+
+  * ``kind``: This is the kind of virtual environment to use:
+
+    * ``conda``
+    * ``virtualenv`` (not yet supported)
+    * ``local`` (no virtual enviroment)
+
+  * ``name``: This is the name of the enviroment to use in case a virtual
+    environment is used.
+
+* ``mem``: Memory to be used by the job. It must be provided as a string with
+  the units (e.g. ``2GB``).
 * ``cpus``: Number of CPUs to be used by the job. It must be provided as an int.
-* ``disk``: Disk space to be used by the job. It must be provided as a string with the units (e.g. ``2GB``). Keep in 
-  mind that junifer uses a local working directory for each job, and datalad datasets might be cloned in this temporary
+* ``disk``: Disk space to be used by the job. It must be provided as a string
+  with the units (e.g. ``2GB``). Keep in mind that junifer uses a local working
+  directory for each job, and datalad datasets might be cloned in this temporary
   directory.
-* ``extra_preamble``: Extra lines to be added to the HTCondor submit file. This can be used to add
-  extra parameters to the job, such as ``requirements``.
-* ``collect``: If ``true``, a final job will be added to the DAG to collect the results once all of the individual
-  element jobs are finished. This is useful if you want to run a ``junifer collect`` job only once all of the
-  individual element jobs are finished. If not specified, it will default to ``true``.
+* ``extra_preamble``: Extra lines to be added to the HTCondor submit file. This
+  can be used to add extra parameters to the job, such as ``requirements``.
+* ``collect``: This parameter allows to include a collect to the DAG to collect
+  the results once all of the individual element jobs are finished. This is
+  useful if you want to run a ``junifer collect`` job only once all of the
+  individual element jobs are finished. Valid options are:
+
+  * ``yes``: Include a collect job in the DAG that will be executed even if some
+    of the individual element jobs fail.
+  * ``on_success_only``: Include a collect job to the DAG, but will only run if
+    all of the individual element jobs are successful.
+  * ``no``: Do not include a collect job to the DAG.
 
 
 Example:
 
 .. code-block:: yaml
 
   queue:
     jobname: TestHTCondorQueue
     kind: HTCondor
     env:
       kind: conda
       name: junifer
     mem: 8G
-    disk: 2GB
-    collect: true
-
+    disk: 2G
+    collect: "yes"  # wrap it in string to avoid boolean
 
-Once the :ref:`codeless` file is ready, including the ``queue`` section, you can queue the jobs by executing 
-the ``junifer queue`` command. 
+Once the :ref:`codeless` file is ready, including the ``queue`` section, you can
+queue the jobs by executing the ``junifer queue`` command.
 
-The ``queue`` command will create a folder with the name of the job (``jobname``) under the ``junifer_jobs`` directory
-in the current working directory.
+The ``queue`` command will create a folder with the name of the job (``jobname``)
+under the ``junifer_jobs`` directory in the current working directory.
 
 The ``queue`` command accepts the following arguments:
 
 * ``--help``: Show a help message.
-* ``--verbose`` Set the verbosity level. Options are ``warning``, ``info``, ``debug``.
-* ``--submit``: Submit the jobs to the queueing system. If not specified, the job submit files will be created but not
-  submitted.
-* ``--overwrite``: Overwrite the job folder if it already exists. If not specified, the command will fail if the job
-  folder already exists.
-* ``--element``: Queue only the specified element(s). If not specified, all elements will be queued.
-
+* ``--verbose``: Set the verbosity level. Options are ``warning``, ``info``,
+  ``debug``.
+* ``--submit``: Submit the jobs to the queueing system. If not specified, the
+  job submit files will be created but not submitted.
+* ``--overwrite``: Overwrite the job folder if it already exists. If not
+  specified, the command will fail if the job folder already exists.
+* ``--element``: Queue only the specified element(s). If not specified, all
+  elements will be queued.
```

### Comparing `junifer-0.0.2.dev86/examples/norun_hcpfc_pearson.py` & `junifer-0.0.3.dev36/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/norun_ukbvm_gmd.py` & `junifer-0.0.3.dev36/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/run_compute_parcel_mean.py` & `junifer-0.0.3.dev36/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.3.dev36/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/run_ets_rss_marker.py` & `junifer-0.0.3.dev36/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/run_junifer_julearn.py` & `junifer-0.0.3.dev36/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/run_run_gmd_mean.py` & `junifer-0.0.3.dev36/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/yamls/gmd_mean.yaml` & `junifer-0.0.3.dev36/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.3.dev36/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/api/cli.py` & `junifer-0.0.3.dev36/junifer/api/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,14 +70,53 @@
                 "The 'elements' key is set in the configuration, but its value"
                 " is 'None'. It is likely that there is an empty 'elements' "
                 "section in the yaml configuration file."
             )
     return elements
 
 
+def _validate_verbose(
+    ctx: click.Context, param: str, value: str
+) -> Union[str, int]:
+    """Validate verbose option.
+
+    Parameters
+    ----------
+    ctx : click.Context
+        The context of the command.
+    param : str
+        The parameter to validate.
+    value : str
+        The value to validate.
+
+    Returns
+    -------
+    str or int
+        The validated value.
+    """
+    if isinstance(value, int):
+        return value
+
+    valid_strings = ["error", "warning", "info", "debug"]
+    if isinstance(value, str) and value.lower() in valid_strings:
+        return value.upper()
+
+    try:
+        value = int(value)  # type: ignore
+        return value
+    except ValueError:
+        # If we get here, the value is not a valid integer.
+        pass
+
+    # If we get here, the value is not valid.
+    raise click.BadParameter(
+        f"verbose must be one of {valid_strings} or an integer"
+    )
+
+
 @click.group()
 def cli() -> None:  # pragma: no cover
     """CLI for JUelich NeuroImaging FEature extractoR."""
 
 
 @cli.command()
 @click.argument(
@@ -86,31 +125,32 @@
         exists=True, readable=True, dir_okay=False, path_type=pathlib.Path
     ),
 )
 @click.option("--element", type=str, multiple=True)
 @click.option(
     "-v",
     "--verbose",
-    type=click.Choice(["warning", "info", "debug"], case_sensitive=False),
+    type=click.UNPROCESSED,
+    callback=_validate_verbose,
     default="info",
 )
-def run(filepath: click.Path, element: str, verbose: click.Choice) -> None:
+def run(filepath: click.Path, element: str, verbose: Union[str, int]) -> None:
     """Run command for CLI.
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
     element : str
         The element to operate using.
     verbose : click.Choice
         The verbosity level: warning, info or debug (default "info").
 
     """
-    configure_logging(level=str(verbose).upper())
+    configure_logging(level=verbose)
     # TODO: add validation
     config = parse_yaml(filepath)  # type: ignore
     workdir = config["workdir"]
     datagrabber = config["datagrabber"]
     markers = config["markers"]
     storage = config["storage"]
     preprocessor = config.get("preprocess")
@@ -132,29 +172,30 @@
     type=click.Path(
         exists=True, readable=True, dir_okay=False, path_type=pathlib.Path
     ),
 )
 @click.option(
     "-v",
     "--verbose",
-    type=click.Choice(["warning", "info", "debug"], case_sensitive=False),
+    type=click.UNPROCESSED,
+    callback=_validate_verbose,
     default="info",
 )
-def collect(filepath: click.Path, verbose: click.Choice) -> None:
+def collect(filepath: click.Path, verbose: Union[str, int]) -> None:
     """Collect command for CLI.
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
     verbose : click.Choice
         The verbosity level: warning, info or debug (default "info").
 
     """
-    configure_logging(level=str(verbose).upper())
+    configure_logging(level=verbose)
     # TODO: add validation
     config = parse_yaml(filepath)  # type: ignore
     storage = config["storage"]
     # Perform operation
     api_collect(storage=storage)
 
 
@@ -167,23 +208,24 @@
 )
 @click.option("--element", type=str, multiple=True)
 @click.option("--overwrite", is_flag=True)
 @click.option("--submit", is_flag=True)
 @click.option(
     "-v",
     "--verbose",
-    type=click.Choice(["warning", "info", "debug"], case_sensitive=False),
+    type=click.UNPROCESSED,
+    callback=_validate_verbose,
     default="info",
 )
 def queue(
     filepath: click.Path,
     element: str,
     overwrite: bool,
     submit: bool,
-    verbose: click.Choice,
+    verbose: Union[str, int],
 ) -> None:
     """Queue command for CLI.
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
@@ -193,15 +235,15 @@
         Whether to overwrite existing directory.
     submit : bool
         Whether to submit the job.
     verbose : click.Choice
         The verbosity level: warning, info or debug (default "info").
 
     """
-    configure_logging(level=str(verbose).upper())
+    configure_logging(level=verbose)
     # TODO: add validation
     config = parse_yaml(filepath)  # type: ignore
     elements = _parse_elements(element, config)
     if "queue" not in config:
         raise_error(f"No queue configuration found in {filepath}.")
     queue_config = config.pop("queue")
     kind = queue_config.pop("kind")
```

### Comparing `junifer-0.0.2.dev86/junifer/api/decorators.py` & `junifer-0.0.3.dev36/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/api/functions.py` & `junifer-0.0.3.dev36/junifer/api/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -321,16 +321,17 @@
     elements: List[Union[str, Tuple]],
     config: Dict,
     env: Optional[Dict[str, str]] = None,
     mem: str = "8G",
     cpus: int = 1,
     disk: str = "1G",
     extra_preamble: str = "",
+    pre_run: Optional[str] = None,
     verbose: str = "info",
-    collect: bool = True,
+    collect: str = "yes",
     submit: bool = False,
 ) -> None:
     """Submit job to HTCondor.
 
     Parameters
     ----------
     jobname : str
@@ -349,18 +350,28 @@
         The size of memory (RAM) to use (default "8G").
     cpus : int, optional
         The number of CPU cores to use (default 1).
     disk : str, optional
         The size of disk (HDD or SSD) to use (default "1G").
     extra_preamble : str, optional
         Extra commands to pass to HTCondor (default "").
+    pre_run : str, optional
+        Extra bash commands to source before the job (default None).
     verbose : str, optional
         The level of verbosity (default "info").
-    collect : bool, optional
-        Whether to submit "collect" task for junifer (default True).
+    collect : str, optional
+        Whether to submit "collect" task for junifer (default "yes").
+        Valid options are:
+
+            * "yes": Submit "collect" task and run even if some of the jobs
+                fail.
+            * "on_success_only": Submit "collect" task and run only if all jobs
+                succeed.
+            * "no": Do not submit "collect" task.
+
     submit : bool, optional
         Whether to submit the jobs. In any case, .dag files will be created
         for submission (default False).
 
     Raises
     ------
     ValueError
@@ -372,14 +383,21 @@
         f"run {str(yaml_config.absolute())} "
         f"--verbose {verbose} --element $(element)"
     )
     collect_junifer_args = (
         f"collect {str(yaml_config.absolute())} --verbose {verbose} "
     )
 
+    if not isinstance(collect, str):
+        raise_error("collect must be a string")
+
+    collect = collect.lower()
+    if collect not in ["yes", "no", "on_success_only"]:
+        raise_error(f"Invalid value for collect: {collect}")
+
     # Set up the env_name, executable and arguments according to the
     # environment type
     if env is None:
         env = {"kind": "local"}
     if env["kind"] == "conda":
         env_name = env["name"]
         executable = "run_conda.sh"
@@ -395,14 +413,24 @@
         # TODO: Copy run_venv.sh to jobdir
     elif env["kind"] == "local":
         executable = "junifer"
         arguments = ""
     else:
         raise ValueError(f'Unknown env kind: {env["kind"]}')
 
+    logger.info("Writing pre_run.sh to jobdir")
+    pre_run_fname = jobdir / "pre_run.sh"
+    with open(pre_run_fname, "w") as f:
+        f.write("#!/bin/bash\n\n")
+        f.write("# Force datalad to run in non-interactive mode\n")
+        f.write("DATALAD_UI_INTERACTIVE=false\n\n")
+        if pre_run is not None:
+            f.write(pre_run)
+    make_executable(pre_run_fname)
+
     # Create log directory
     log_dir = jobdir / "logs"
     log_dir.mkdir(exist_ok=True, parents=True)
 
     # Add preamble data
     run_preamble = f"""
         # The environment
@@ -478,18 +506,32 @@
                 "_".join(t_elem) if isinstance(t_elem, tuple) else t_elem
             )
             dag_file.write(f"JOB run{i_job} {submit_run_fname}\n")
             dag_file.write(
                 f'VARS run{i_job} element="{str_elem}" '
                 f'log_element="{log_elem}"\n\n'
             )
-        if collect is True:
+        if collect == "yes":
+            dag_file.write(f"FINAL collect {submit_collect_fname}\n")
+            collect_pre_fname = jobdir / "collect_pre.sh"
+            dag_file.write(
+                f"SCRIPT PRE collect {collect_pre_fname.as_posix()} "
+                "$DAG_STATUS\n"
+            )
+            with open(collect_pre_fname, "w") as pre_file:
+                pre_file.write("#!/bin/bash\n\n")
+                pre_file.write('if [ "${1}" == "4" ]; then\n')
+                pre_file.write("    exit 1\n")
+                pre_file.write("fi\n")
+
+            make_executable(collect_pre_fname)
+        elif collect == "on_success_only":
             dag_file.write(f"JOB collect {submit_collect_fname}\n")
             dag_file.write("PARENT ")
-            for i_job, _t_elem in enumerate(elements):
+            for i_job, _ in enumerate(elements):
                 dag_file.write(f"run{i_job} ")
             dag_file.write("CHILD collect\n\n")
 
     # Submit job(s)
     if submit is True:
         logger.info("Submitting HTCondor job")
         subprocess.run(["condor_submit_dag", dag_fname])
```

### Comparing `junifer-0.0.2.dev86/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.3.dev36/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/api/tests/test_api_utils.py` & `junifer-0.0.3.dev36/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/api/tests/test_cli.py` & `junifer-0.0.3.dev36/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/api/tests/test_functions.py` & `junifer-0.0.3.dev36/junifer/api/tests/test_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import logging
+import stat
 from pathlib import Path
 from typing import List, Tuple, Union
 
 import pytest
 import yaml
 
 import junifer.testing.registry  # noqa: F401
@@ -535,25 +536,61 @@
             queue(
                 config={"elements": "sub-001"},
                 kind="HTCondor",
                 jobname="conda_env_check",
                 env={"kind": "conda", "name": "conda-env"},
             )
             assert "Copying" in caplog.text
-            assert (
-                Path(
-                    tmp_path
-                    / "junifer_jobs"
-                    / "conda_env_check"
-                    / "run_conda.sh"
-                )
-                .stat()
-                .st_mode
-                == 33261
+            fname = (
+                tmp_path / "junifer_jobs" / "conda_env_check" / "run_conda.sh"
+            )
+            assert fname.is_file()
+            assert stat.S_IMODE(fname.stat().st_mode) & stat.S_IEXEC != 0
+
+
+def test_queue_condor_conda_pre_run_python(
+    tmp_path: Path,
+    monkeypatch: pytest.MonkeyPatch,
+    caplog: pytest.LogCaptureFixture,
+) -> None:
+    """Test conda Python environment check for HTCondor.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+    monkeypatch : pytest.MonkeyPatch
+        The monkeypatch object.
+    caplog : pytest.LogCaptureFixture
+        The logcapturefixture object.
+
+    """
+    with monkeypatch.context() as m:
+        m.chdir(tmp_path)
+        with caplog.at_level(logging.INFO):
+            queue(
+                config={"elements": "sub-001"},
+                kind="HTCondor",
+                jobname="conda_env_check",
+                env={"kind": "conda", "name": "conda-env"},
+                pre_run="echo testing",
             )
+            assert "Copying" in caplog.text
+
+            fname = (
+                tmp_path / "junifer_jobs" / "conda_env_check" / "run_conda.sh"
+            )
+            assert fname.is_file()
+            assert stat.S_IMODE(fname.stat().st_mode) & stat.S_IEXEC != 0
+
+            fname = (
+                tmp_path / "junifer_jobs" / "conda_env_check" / "pre_run.sh"
+            )
+            assert fname.is_file()
+            assert stat.S_IMODE(fname.stat().st_mode) & stat.S_IEXEC != 0
 
 
 def test_queue_condor_venv_python(
     tmp_path: Path,
     monkeypatch: pytest.MonkeyPatch,
     caplog: pytest.LogCaptureFixture,
 ) -> None:
@@ -585,37 +622,45 @@
     [
         (
             ["sub-001"],
             {"kind": "conda", "name": "conda-env"},
             "4G",
             4,
             "4G",
-            True,
+            "yes",
+        ),
+        (
+            ["sub-001"],
+            {"kind": "conda", "name": "conda-env"},
+            "4G",
+            4,
+            "4G",
+            "on_success_only",
         ),
         (
             ["sub-001"],
             {"kind": "venv", "name": "venv-env"},
             "8G",
             8,
             "8G",
-            False,
+            "no",
         ),
-        (["sub-001"], {"kind": "local"}, "12G", 12, "12G", True),
+        (["sub-001"], {"kind": "local"}, "12G", 12, "12G", "yes"),
     ],
 )
 def test_queue_condor_assets_generation(
     tmp_path: Path,
     monkeypatch: pytest.MonkeyPatch,
     caplog: pytest.LogCaptureFixture,
     elements: str,
     env: str,
     mem: str,
     cpus: int,
     disk: str,
-    collect: bool,
+    collect: str,
 ) -> None:
     """Test HTCondor generated assets.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
@@ -629,15 +674,15 @@
         The parametrized env names.
     mem : str
         The parametrized memory size.
     cpus : int
         The parametrized CPUs.
     disk : str
         The parametrized disk size.
-    collect : bool
+    collect : str
         The parametrized collect option.
 
     """
     jobname = "condor_assets_gen_check"
     with monkeypatch.context() as m:
         m.chdir(tmp_path)
         with caplog.at_level(logging.INFO):
@@ -682,28 +727,47 @@
                 tmp_path / "junifer_jobs" / jobname / f"{jobname}.dag"
             )
             # Check junifer dag file
             assert dag_file_path.is_file()
             # Read dag file to check if collect job is found
             element_count = 0
             has_collect_job = False
+            has_final_collect_job = False
             with open(dag_file_path, "r") as f:
                 for line in f.read().splitlines():
                     if "JOB" in line:
                         element_count += 1
                     if "collect" in line:
                         has_collect_job = True
+                    if "FINAL" in line:
+                        has_final_collect_job = True
 
-            if collect:
+            if collect == "yes":
+                assert len(elements) == element_count
+                assert has_collect_job is True
+                assert has_final_collect_job is True
+            elif collect == "on_success_only":
                 assert len(elements) == element_count - 1
                 assert has_collect_job is True
+                assert has_final_collect_job is False
             else:
                 assert len(elements) == element_count
                 assert has_collect_job is False
 
+            if has_final_collect_job is True:
+                pre_collect_fname = Path(
+                    tmp_path / "junifer_jobs" / jobname / "collect_pre.sh"
+                )
+                assert pre_collect_fname.exists()
+                assert (
+                    stat.S_IMODE(pre_collect_fname.stat().st_mode)
+                    & stat.S_IEXEC
+                    != 0
+                )
+
             # Check submit log
             assert (
                 "HTCondor job files created, to submit the job, run"
                 in caplog.text
             )
```

### Comparing `junifer-0.0.2.dev86/junifer/api/utils.py` & `junifer-0.0.3.dev36/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.3.dev36/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/configs/tests/test_juseless.py` & `junifer-0.0.3.dev36/junifer/configs/tests/test_juseless.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.3.dev36/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.3.dev36/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.3.dev36/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.3.dev36/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/coordinates.py` & `junifer-0.0.3.dev36/junifer/data/coordinates.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,18 @@
     """Register coordinates.
 
     Parameters
     ----------
     name : str
         The name of the coordinates.
     coordinates : numpy.ndarray
-        The coordinates.
+        The coordinates. This should be a 2-dimensional array with three
+        columns. Each row corresponds to a volume-of-interest (VOI) and each
+        column corresponds to a spatial dimension (i.e. x, y, and
+        z-coordinates).
     voi_names : list of str
         The names of the VOIs.
     overwrite : bool, optional
         If True, overwrite an existing list of coordinates with the same name.
         Does not apply to built-in coordinates (default False).
     """
     if name in _available_coordinates:
```

### Comparing `junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.3.dev36/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/masks.py` & `junifer-0.0.3.dev36/junifer/data/masks.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,45 +3,48 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
-    Callable,
 )
 
-import numpy as np
-
 import nibabel as nib
+import numpy as np
+from nilearn.datasets import fetch_icbm152_brain_gm_mask
+from nilearn.image import resample_to_img
 from nilearn.masking import (
-    compute_brain_mask,
     compute_background_mask,
+    compute_brain_mask,
     compute_epi_mask,
+    intersect_masks,
 )
-from nilearn.datasets import fetch_icbm152_brain_gm_mask
-from nilearn.image import resample_to_img
 
 from ..utils.logging import logger, raise_error
 from .utils import closest_resolution
 
 
 if TYPE_CHECKING:
     from nibabel import Nifti1Image
 
 # Path to the VOIs
 _masks_path = Path(__file__).parent / "masks"
 
 
-def _fetch_icbm152_brain_gm_mask(target_img: "Nifti1Image", **kwargs):
+def _fetch_icbm152_brain_gm_mask(
+    target_img: "Nifti1Image",
+    **kwargs,
+):
     """Fetch ICBM152 brain mask and resample.
 
     Parameters
     ----------
     target_img : nibabel.Nifti1Image
         The image to which the mask will be resampled.
     **kwargs : dict
@@ -62,14 +65,17 @@
 
 """
 A dictionary containing all supported masks and their respective file or
 data.
 
 The built-in masks are files that are shipped with the package in the
 data/masks directory. The user can also register their own masks.
+
+Callable masks should be functions that take at least one parameter:
+* `target_img`: the image to which the mask will be applied.
 """
 _available_masks: Dict[str, Dict[str, Any]] = {
     "GM_prob0.2": {"family": "Vickery-Patil"},
     "GM_prob0.2_cortex": {"family": "Vickery-Patil"},
     "compute_brain_mask": {
         "family": "Callable",
         "func": compute_brain_mask,
@@ -143,66 +149,131 @@
     list of str
         A list with all available masks names.
     """
     return sorted(_available_masks.keys())
 
 
 def get_mask(
-    mask: Union[str, Dict],
+    masks: Union[str, Dict, List[Union[Dict, str]]],
     target_data: Dict[str, Any],
+    extra_input: Optional[Dict[str, Any]] = None,
 ) -> "Nifti1Image":
     """Get mask, tailored for the target image.
 
     Parameters
     ----------
-    masks : str or dict
+    masks : str, dict or list of dict or str
         The name of the mask, or the name of a callable mask and the parameters
-        of the mask.
+        of the mask as a dictionary. Several masks can be passed as a list.
     target_data : dict
         The corresponding item of the data object to which the mask will be
         applied.
+    extra_input : dict, optional
+        The other fields in the data object. Useful for accessing other data
+        kinds that needs to be used in the computation of masks (default None).
 
     Returns
     -------
     Nifti1Image
         The mask image.
     """
     # Get the min of the voxels sizes and use it as the resolution
     target_img = target_data["data"]
+    inherited_mask_item = target_data.get("mask_item", None)
     resolution = np.min(target_img.header.get_zooms()[:3])
 
-    if isinstance(mask, dict):
-        if len(mask) != 1:
-            raise_error(
-                "The mask dictionary must have only one key, "
-                "the name of the mask."
-            )
-        mask_name = list(mask.keys())[0]
-        mask_params = mask[mask_name]
-    else:
-        mask_name = mask
-        mask_params = None
+    if not isinstance(masks, list):
+        masks = [masks]
 
-    mask_object, _ = load_mask(
-        mask_name, path_only=False, resolution=resolution
-    )
-    if callable(mask_object):
-        if mask_params is None:
-            mask_params = {}
-        mask_img = mask_object(target_img, **mask_params)
-    else:  # Mask is a Nifti1Image
-        if mask_params is not None:
-            raise_error("Cannot pass callable params to a non-callable mask.")
-        mask_img = resample_to_img(
-            mask_object,
-            target_img,
-            interpolation="nearest",
-            copy=True,
+    # Check that dicts have only one key
+    invalid_elements = [
+        x for x in masks if isinstance(x, dict) and len(x) != 1
+    ]
+    if len(invalid_elements) > 0:
+        raise_error(
+            "Each of the masks dictionary must have only one key, "
+            "the name of the mask. The following dictionaries are invalid: "
+            f"{invalid_elements}"
         )
 
+    # Check params for the intersection function
+    intersect_params = {}
+    true_masks = []
+    for t_mask in masks:
+        if isinstance(t_mask, dict):
+            if "threshold" in t_mask:
+                intersect_params["threshold"] = t_mask["threshold"]
+                continue
+            elif "connected" in t_mask:
+                intersect_params["connected"] = t_mask["connected"]
+                continue
+        # All the other elements are masks
+        true_masks.append(t_mask)
+
+    if len(true_masks) == 0:
+        raise_error("No mask was passed. At least one mask is required.")
+    # Get all the masks
+    all_masks = []
+    for t_mask in true_masks:
+        if isinstance(t_mask, dict):
+            mask_name = list(t_mask.keys())[0]
+            mask_params = t_mask[mask_name]
+        else:
+            mask_name = t_mask
+            mask_params = None
+
+        if mask_name == "inherit":
+            if extra_input is None:
+                raise_error(
+                    "Cannot inherit mask from another data item "
+                    "because no extra data was passed."
+                )
+            if inherited_mask_item is None:
+                raise_error(
+                    "Cannot inherit mask from another data item "
+                    "because no mask item was specified "
+                    "(missing `mask_item` key in the data object)."
+                )
+            if inherited_mask_item not in extra_input:
+                raise_error(
+                    "Cannot inherit mask from another data item "
+                    f"because the item ({inherited_mask_item}) does not exist."
+                )
+            mask_img = extra_input[inherited_mask_item]["data"]
+        else:
+            mask_object, _ = load_mask(
+                mask_name, path_only=False, resolution=resolution
+            )
+            if callable(mask_object):
+                if mask_params is None:
+                    mask_params = {}
+                mask_img = mask_object(target_img, **mask_params)
+            else:  # Mask is a Nifti1Image
+                if mask_params is not None:
+                    raise_error(
+                        "Cannot pass callable params to a non-callable mask."
+                    )
+                mask_img = resample_to_img(
+                    mask_object,
+                    target_img,
+                    interpolation="nearest",
+                    copy=True,
+                )
+        all_masks.append(mask_img)
+    if len(all_masks) > 1:
+        mask_img = intersect_masks(all_masks, **intersect_params)
+    else:
+        if len(intersect_params) > 0:
+            # Yes, I'm this strict!
+            raise_error(
+                "Cannot pass parameters to the intersection function "
+                "when there is only one mask."
+            )
+        mask_img = all_masks[0]
+
     return mask_img
 
 
 def load_mask(
     name: str,
     resolution: Optional[float] = None,
     path_only: bool = False,
```

### Comparing `junifer-0.0.2.dev86/junifer/data/parcellations.py` & `junifer-0.0.3.dev36/junifer/data/parcellations.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import nibabel as nib
 import numpy as np
 import pandas as pd
 import requests
-from nilearn import datasets
+from nilearn import datasets, image
 
-from ..utils.logging import logger, raise_error
+from ..utils.logging import logger, raise_error, warn_with_log
 from .utils import closest_resolution
 
 
 if TYPE_CHECKING:
     from nibabel import Nifti1Image
 
 
@@ -163,15 +163,15 @@
     If it is a built-in parcellaions and file is not present in the
     `parcellations_dir` directory, it will be downloaded.
 
     Parameters
     ----------
     name : str
         The name of the parcellation. Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     parcellations_dir : str or pathlib.Path, optional
         Path where the parcellations files are stored. The default location is
         "$HOME/junifer/data/parcellations" (default None).
     resolution : float, optional
         The desired resolution of the parcellation to load. If it is not
         available, the closest resolution will be loaded. Preferably, use a
         resolution higher than the desired one. By default, will load the
@@ -696,7 +696,88 @@
             raise_error("There was a problem fetching the parcellations.")
 
     labels = pd.read_csv(parcellation_lname, sep="\t", usecols=["name"])[
         "name"
     ].to_list()
 
     return parcellation_fname, labels
+
+
+def merge_parcellations(
+    parcellations_list: List["Nifti1Image"],
+    parcellations_names: List[str],
+    labels_lists: List[List[str]],
+) -> Tuple["Nifti1Image", List[str]]:
+    """Merge all parcellations from a list into one parcellation.
+
+    Parameters
+    ----------
+    parcellations_list : list of niimg-like object
+        List of parcellations to merge.
+    parcellations_names: list of str
+        List of names for parcellations at the corresponding indices.
+    labels_lists : list of list of str
+        A list of lists. Each list in the list contains the labels for the
+        parcellation at the corresponding index.
+
+    Returns
+    -------
+    parcellation : niimg-like object
+        The parcellation that results from merging the list of input
+        parcellations.
+    labels : list of str
+        List of labels for the resultant parcellation.
+
+    """
+    # Check for duplicated labels
+    labels_lists_flat = [item for sublist in labels_lists for item in sublist]
+    if len(labels_lists_flat) != len(set(labels_lists_flat)):
+        warn_with_log(
+            "The parcellations have duplicated labels. "
+            "Each label will be prefixed with the parcellation name."
+        )
+        for i_parcellation, t_labels in enumerate(labels_lists):
+            labels_lists[i_parcellation] = [
+                f"{parcellations_names[i_parcellation]}_{t_label}"
+                for t_label in t_labels
+            ]
+    overlapping_voxels = False
+    ref_parc = parcellations_list[0]
+    parc_data = ref_parc.get_fdata()
+
+    labels = labels_lists[0]
+
+    for t_parc, t_labels in zip(parcellations_list[1:], labels_lists[1:]):
+        if t_parc.shape != ref_parc.shape:
+            warn_with_log(
+                "The parcellations have different resolutions!"
+                "Resampling all parcellations to the first one in the list."
+            )
+            t_parc = image.resample_to_img(
+                t_parc, ref_parc, interpolation="nearest", copy=True
+            )
+
+        # Get the data from this parcellation
+        t_parc_data = t_parc.get_fdata().copy()  # must be copied
+        # Increase the values of each ROI to match the labels
+        t_parc_data[t_parc_data != 0] += len(labels)
+
+        # Only set new values for the voxels that are 0
+        # This makes sure that the voxels that are in multiple
+        # parcellations are assigned to the parcellation that was
+        # first in the list.
+        if np.any(parc_data[t_parc_data != 0] != 0):
+            overlapping_voxels = True
+
+        parc_data[parc_data == 0] += t_parc_data[parc_data == 0]
+        labels.extend(t_labels)
+
+    if overlapping_voxels:
+        warn_with_log(
+            "The parcellations have overlapping voxels. "
+            "The overlapping voxels will be assigned to the "
+            "parcellation that was first in the list."
+        )
+
+    parcellation_img_res = image.new_img_like(parcellations_list[0], parc_data)
+
+    return parcellation_img_res, labels
```

### Comparing `junifer-0.0.2.dev86/junifer/data/tests/test_coordinates.py` & `junifer-0.0.3.dev36/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/tests/test_data_utils.py` & `junifer-0.0.3.dev36/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/data/tests/test_parcellations.py` & `junifer-0.0.3.dev36/junifer/data/tests/test_parcellations.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 from typing import List
 
 import nibabel as nib
+import numpy as np
 import pytest
 from nilearn.image import new_img_like
 from numpy.testing import assert_array_almost_equal, assert_array_equal
 
 from junifer.data.parcellations import (
     _retrieve_parcellation,
     _retrieve_schaefer,
     _retrieve_suit,
     _retrieve_tian,
     list_parcellations,
     load_parcellation,
+    merge_parcellations,
     register_parcellation,
 )
 
 
 def test_register_parcellation_built_in_check() -> None:
     """Test parcellation registration check for built-in parcellations."""
     with pytest.raises(ValueError, match=r"built-in parcellation"):
@@ -232,50 +234,42 @@
 
     # Test with Path
     img, lbl, fname = load_parcellation(
         name="Schaefer100x7", parcellations_dir=tmp_path
     )
     # Load parcellation
     img2, lbl, fname = load_parcellation(
-        name="Schaefer100x7",
-        parcellations_dir=tmp_path,
-        resolution=3,
+        name="Schaefer100x7", parcellations_dir=tmp_path, resolution=3
     )
     # Check parcellation values
     assert fname.name == fname2
     assert len(lbl) == 100
     assert img2 is not None
     assert_array_equal(img2.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
     # Load parcellation
     img2, lbl, fname = load_parcellation(
-        "Schaefer100x7",
-        parcellations_dir=tmp_path,
-        resolution=2.1,
+        "Schaefer100x7", parcellations_dir=tmp_path, resolution=2.1
     )
     # Check parcellation values
     assert fname.name == fname2
     assert len(lbl) == 100
     assert img2 is not None
     assert_array_equal(img2.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
     # Load parcellation
     img2, lbl, fname = load_parcellation(
-        "Schaefer100x7",
-        parcellations_dir=tmp_path,
-        resolution=1.99,
+        "Schaefer100x7", parcellations_dir=tmp_path, resolution=1.99
     )
     # Check parcellation values
     assert fname.name == fname1
     assert len(lbl) == 100
     assert img2 is not None
     assert_array_equal(img2.header["pixdim"][1:4], [1, 1, 1])  # type: ignore
     # Load parcellation
     img2, lbl, fname = load_parcellation(
-        "Schaefer100x7",
-        parcellations_dir=tmp_path,
-        resolution=0.5,
+        "Schaefer100x7", parcellations_dir=tmp_path, resolution=0.5
     )
     # Check parcellation values
     assert fname.name == fname1
     assert len(lbl) == 100
     assert img2 is not None
     assert_array_equal(img2.header["pixdim"][1:4], [1, 1, 1])  # type: ignore
 
@@ -379,26 +373,18 @@
 
     """
     with pytest.raises(ValueError, match=r"The parameter `space`"):
         _retrieve_suit(parcellations_dir=tmp_path, resolution=1, space="wrong")
 
 
 @pytest.mark.parametrize(
-    "scale, n_label",
-    [
-        (1, 16),
-        (2, 32),
-        (3, 50),
-        (4, 54),
-    ],
+    "scale, n_label", [(1, 16), (2, 32), (3, 50), (4, 54)]
 )
 def test_tian_3T_6thgeneration(
-    tmp_path: Path,
-    scale: int,
-    n_label: int,
+    tmp_path: Path, scale: int, n_label: int
 ) -> None:
     """Test Tian parcellation.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
@@ -411,16 +397,15 @@
     parcellations = list_parcellations()
     assert "TianxS1x3TxMNI6thgeneration" in parcellations
     assert "TianxS2x3TxMNI6thgeneration" in parcellations
     assert "TianxS3x3TxMNI6thgeneration" in parcellations
     assert "TianxS4x3TxMNI6thgeneration" in parcellations
     # Load parcellation
     img, lbl, fname = load_parcellation(
-        name=f"TianxS{scale}x3TxMNI6thgeneration",
-        parcellations_dir=tmp_path,
+        name=f"TianxS{scale}x3TxMNI6thgeneration", parcellations_dir=tmp_path
     )
     fname1 = f"Tian_Subcortex_S{scale}_3T_1mm.nii.gz"
     assert img is not None
     assert fname.name == fname1
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [1, 1, 1])  # type: ignore
     # Load parcellation
@@ -433,26 +418,18 @@
     assert img is not None
     assert fname.name == fname1
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
 
 
 @pytest.mark.parametrize(
-    "scale, n_label",
-    [
-        (1, 16),
-        (2, 32),
-        (3, 50),
-        (4, 54),
-    ],
+    "scale, n_label", [(1, 16), (2, 32), (3, 50), (4, 54)]
 )
 def test_tian_3T_nonlinear2009cAsym(
-    tmp_path: Path,
-    scale: int,
-    n_label: int,
+    tmp_path: Path, scale: int, n_label: int
 ) -> None:
     """Test Tian parcellation.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
@@ -476,26 +453,18 @@
     assert img is not None
     assert fname.name == fname1
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
 
 
 @pytest.mark.parametrize(
-    "scale, n_label",
-    [
-        (1, 16),
-        (2, 34),
-        (3, 54),
-        (4, 62),
-    ],
+    "scale, n_label", [(1, 16), (2, 34), (3, 54), (4, 62)]
 )
 def test_tian_7T_6thgeneration(
-    tmp_path: Path,
-    scale: int,
-    n_label: int,
+    tmp_path: Path, scale: int, n_label: int
 ) -> None:
     """Test Tian parcellation.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
@@ -530,18 +499,15 @@
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
     with pytest.raises(ValueError, match=r"The parameter `space`"):
         _retrieve_tian(
-            parcellations_dir=tmp_path,
-            resolution=1,
-            scale=1,
-            space="wrong",
+            parcellations_dir=tmp_path, resolution=1, scale=1, space="wrong"
         )
 
     with pytest.raises(ValueError, match=r"MNI6thgeneration"):
         _retrieve_tian(
             parcellations_dir=tmp_path,
             resolution=1,
             scale=1,
@@ -580,7 +546,166 @@
     with pytest.raises(ValueError, match=r"The parameter `scale`"):
         _retrieve_tian(
             parcellations_dir=tmp_path,
             resolution=1,
             scale=5,
             space="MNI6thgeneration",
         )
+
+
+def test_merge_parcellations() -> None:
+    """Test merging parcellations."""
+    # load some parcellations for testing
+    schaefer_parcellation, schaefer_labels, _ = load_parcellation(
+        "Schaefer100x17"
+    )
+    tian_parcellation, tian_labels, _ = load_parcellation(
+        "TianxS2x3TxMNInonlinear2009cAsym"
+    )
+    # prepare the list of the actual parcellations
+    parcellation_list = [schaefer_parcellation, tian_parcellation]
+    # prepare a list of names
+    names = ["Schaefer100x17", "TianxS2x3TxMNInonlinear2009cAsym"]
+    # prepare a list of label lists
+    labels_lists = [schaefer_labels, tian_labels]
+    # merge the parcellations
+    merged_parc, labels = merge_parcellations(
+        parcellation_list, names, labels_lists
+    )
+
+    # we should have 132 integer labels plus 1 for background
+    parc_data = merged_parc.get_fdata()
+    assert len(np.unique(parc_data)) == 133
+    # no background label, so labels is one less
+    assert len(labels) == 132
+
+
+def test_merge_parcellations_3D_multiple_non_overlapping(
+    tmp_path: Path,
+) -> None:
+    """Test merge_parcellations with multiple non-overlapping parcellations.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+    # Get the testing parcellation
+    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+
+    assert parcellation is not None
+
+    # Create two parcellations from it
+    parcellation_data = parcellation.get_fdata()
+    parcellation1_data = parcellation_data.copy()
+    parcellation1_data[parcellation1_data > 50] = 0
+    parcellation2_data = parcellation_data.copy()
+    parcellation2_data[parcellation2_data <= 50] = 0
+    parcellation2_data[parcellation2_data > 0] -= 50
+    labels1 = labels[:50]
+    labels2 = labels[50:]
+
+    parcellation1_img = new_img_like(parcellation, parcellation1_data)
+    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+
+    parcellation_list = [parcellation1_img, parcellation2_img]
+    names = ["high", "low"]
+    labels_lists = [labels1, labels2]
+
+    merged_parc, merged_labels = merge_parcellations(
+        parcellation_list, names, labels_lists
+    )
+
+    parc_data = parcellation.get_fdata()
+    assert_array_equal(parc_data, merged_parc.get_fdata())
+    assert len(labels) == 100
+    assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
+
+
+def test_merge_parcellations_3D_multiple_overlapping(tmp_path: Path) -> None:
+    """Test merge_parcellations with multiple overlapping parcellations.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+
+    # Get the testing parcellation
+    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+
+    assert parcellation is not None
+
+    # Create two parcellations from it
+    parcellation_data = parcellation.get_fdata()
+    parcellation1_data = parcellation_data.copy()
+    parcellation1_data[parcellation1_data > 50] = 0
+    parcellation2_data = parcellation_data.copy()
+
+    # Make the second parcellation overlap with the first
+    parcellation2_data[parcellation2_data <= 45] = 0
+    parcellation2_data[parcellation2_data > 0] -= 45
+    labels1 = [f"low_{x}" for x in labels[:50]]  # Change the labels
+    labels2 = [f"high_{x}" for x in labels[45:]]  # Change the labels
+
+    parcellation1_img = new_img_like(parcellation, parcellation1_data)
+    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+
+    parcellation_list = [parcellation1_img, parcellation2_img]
+    names = ["high", "low"]
+    labels_lists = [labels1, labels2]
+
+    with pytest.warns(RuntimeWarning, match="overlapping voxels"):
+        merged_parc, merged_labels = merge_parcellations(
+            parcellation_list, names, labels_lists
+        )
+
+    parc_data = parcellation.get_fdata()
+    assert len(labels) == 100
+    assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
+
+
+def test_merge_parcellations_3D_multiple_duplicated_labels(
+    tmp_path: Path,
+) -> None:
+    """Test merge_parcellations with two parcellations with duplicated labels.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+
+    # Get the testing parcellation
+    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+
+    assert parcellation is not None
+
+    # Create two parcellations from it
+    parcellation_data = parcellation.get_fdata()
+    parcellation1_data = parcellation_data.copy()
+    parcellation1_data[parcellation1_data > 50] = 0
+    parcellation2_data = parcellation_data.copy()
+    parcellation2_data[parcellation2_data <= 50] = 0
+    parcellation2_data[parcellation2_data > 0] -= 50
+    labels1 = labels[:50]
+    labels2 = labels[49:-1]  # One label is duplicated
+
+    parcellation1_img = new_img_like(parcellation, parcellation1_data)
+    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+
+    parcellation_list = [parcellation1_img, parcellation2_img]
+    names = ["high", "low"]
+    labels_lists = [labels1, labels2]
+
+    with pytest.warns(RuntimeWarning, match="duplicated labels."):
+        merged_parc, merged_labels = merge_parcellations(
+            parcellation_list, names, labels_lists
+        )
+
+    parc_data = parcellation.get_fdata()
+    assert_array_equal(parc_data, merged_parc.get_fdata())
+    assert len(labels) == 100
+    assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
```

### Comparing `junifer-0.0.2.dev86/junifer/data/utils.py` & `junifer-0.0.3.dev36/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/__init__.py` & `junifer-0.0.3.dev36/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/id1000.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Xuan Li <xu.li@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
-from typing import Union
+from typing import Dict, Union
 
 from junifer.datagrabber import PatternDataladDataGrabber
 
 from ...api.decorators import register_datagrabber
 
 
 @register_datagrabber
@@ -30,15 +30,17 @@
         self,
         datadir: Union[str, Path, None] = None,
     ) -> None:
         # The types of data
         types = [
             "BOLD",
             "BOLD_confounds",
+            "BOLD_mask",
             "T1w",
+            "T1w_mask",
             "probseg_CSF",
             "probseg_GM",
             "probseg_WM",
             "DWI",
         ]
         # The patterns
         patterns = {
@@ -48,19 +50,30 @@
                 "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
             ),
             "BOLD_confounds": (
                 "derivatives/fmriprep/sub-{subject}/func/"
                 "sub-{subject}_task-moviewatching_"
                 "desc-confounds_regressors.tsv"
             ),
+            "BOLD_mask": (
+                "derivatives/fmriprep/sub-{subject}/func/"
+                "sub-{subject}_task-moviewatching_"
+                "space-MNI152NLin2009cAsym_"
+                "desc-brain_mask.nii.gz"
+            ),
             "T1w": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_"
                 "desc-preproc_T1w.nii.gz"
             ),
+            "T1w_mask": (
+                "derivatives/fmriprep/sub-{subject}/anat/"
+                "sub-{subject}_space-MNI152NLin2009cAsym_"
+                "desc-brain_mask.nii.gz"
+            ),
             "probseg_CSF": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_label-"
                 "CSF_probseg.nii.gz"
             ),
             "probseg_GM": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
@@ -84,7 +97,26 @@
             types=types,
             datadir=datadir,
             uri=uri,
             patterns=patterns,
             replacements=replacements,
             confounds_format="fmriprep",
         )
+
+    def get_item(self, subject: str) -> Dict:
+        """Index one element in the dataset.
+
+        Parameters
+        ----------
+        subject : str
+            The subject ID.
+
+        Returns
+        -------
+        out : dict
+            Dictionary of paths for each type of data required for the
+            specified element.
+        """
+        out = super().get_item(subject=subject)
+        out["BOLD"]["mask_item"] = "BOLD_mask"
+        out["T1w"]["mask_item"] = "T1w_mask"
+        return out
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/piop1.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,17 @@
         datadir: Union[str, Path, None] = None,
         tasks: Union[str, List[str], None] = None,
     ) -> None:
         # The types of data
         types = [
             "BOLD",
             "BOLD_confounds",
+            "BOLD_mask",
             "T1w",
+            "T1w_mask",
             "probseg_CSF",
             "probseg_GM",
             "probseg_WM",
             "DWI",
         ]
 
         if isinstance(tasks, str):
@@ -79,19 +81,29 @@
                 "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
             ),
             "BOLD_confounds": (
                 "derivatives/fmriprep/sub-{subject}/func/"
                 "sub-{subject}_task-{task}_"
                 "desc-confounds_regressors.tsv"
             ),
+            "BOLD_mask": (
+                "derivatives/fmriprep/sub-{subject}/func/"
+                "sub-{subject}_task-{task}_"
+                "space-MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
+            ),
             "T1w": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_"
                 "desc-preproc_T1w.nii.gz"
             ),
+            "T1w_mask": (
+                "derivatives/fmriprep/sub-{subject}/anat/"
+                "sub-{subject}_space-MNI152NLin2009cAsym_"
+                "desc-brain_mask.nii.gz"
+            ),
             "probseg_CSF": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_label-"
                 "CSF_probseg.nii.gz"
             ),
             "probseg_GM": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
@@ -145,14 +157,16 @@
             "restingstate": "mb3",
             "workingmemory": "seq",
         }
         acq = task_acqs[task]
         new_task = f"{task}_acq-{acq}"
 
         out = super().get_item(subject=subject, task=new_task)
+        out["BOLD"]["mask_item"] = "BOLD_mask"
+        out["T1w"]["mask_item"] = "T1w_mask"
         return out
 
     def get_elements(self) -> List:
         """Implement fetching list of subjects in the dataset.
 
         Returns
         -------
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/piop2.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Xuan Li <xu.li@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
-from typing import List, Union
+from typing import Dict, List, Union
 
 from junifer.datagrabber import PatternDataladDataGrabber
 
 from ...api.decorators import register_datagrabber
 from ...utils import raise_error
 
 
@@ -36,15 +36,17 @@
         datadir: Union[str, Path, None] = None,
         tasks: Union[str, List[str], None] = None,
     ) -> None:
         # The types of data
         types = [
             "BOLD",
             "BOLD_confounds",
+            "BOLD_mask",
             "T1w",
+            "T1w_mask",
             "probseg_CSF",
             "probseg_GM",
             "probseg_WM",
             "DWI",
         ]
 
         if isinstance(tasks, str):
@@ -76,19 +78,29 @@
                 "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
             ),
             "BOLD_confounds": (
                 "derivatives/fmriprep/sub-{subject}/func/"
                 "sub-{subject}_task-{task}_acq-seq_"
                 "desc-confounds_regressors.tsv"
             ),
+            "BOLD_mask": (
+                "derivatives/fmriprep/sub-{subject}/func/"
+                "sub-{subject}_task-{task}_acq-seq_space"
+                "-MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
+            ),
             "T1w": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_"
                 "desc-preproc_T1w.nii.gz"
             ),
+            "T1w_mask": (
+                "derivatives/fmriprep/sub-{subject}/anat/"
+                "sub-{subject}_space-MNI152NLin2009cAsym_"
+                "desc-brain_mask.nii.gz"
+            ),
             "probseg_CSF": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
                 "sub-{subject}_space-MNI152NLin2009cAsym_label-"
                 "CSF_probseg.nii.gz"
             ),
             "probseg_GM": (
                 "derivatives/fmriprep/sub-{subject}/anat/"
@@ -123,7 +135,29 @@
         -------
         list
             The list of elements that can be grabbed in the dataset after
             imposing constraints based on specified tasks.
         """
         all_elements = super().get_elements()
         return [x for x in all_elements if x[1] in self.tasks]
+
+    def get_item(self, subject: str, task: str) -> Dict:
+        """Index one element in the dataset.
+
+        Parameters
+        ----------
+        subject : str
+            The subject ID.
+        task : str
+            The task to get. Possible values are:
+            {"restingstate", "stopsignal", "emomatching", "workingmemory"}
+
+        Returns
+        -------
+        out : dict
+            Dictionary of paths for each type of data required for the
+            specified element.
+        """
+        out = super().get_item(subject=subject, task=task)
+        out["BOLD"]["mask_item"] = "BOLD_mask"
+        out["T1w"]["mask_item"] = "T1w_mask"
+        return out
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,26 +47,32 @@
             == f"sub-{test_element}_task-moviewatching_"
             "desc-confounds_regressors.tsv"
         )
 
         assert out["BOLD_confounds"]["path"].exists()
         assert out["BOLD_confounds"]["path"].is_file()
 
+        # assert BOLD_mask
+        assert out["BOLD_mask"]["path"].exists()
+
         # asserts type "T1w"
         assert "T1w" in out
 
         assert (
             out["T1w"]["path"].name
             == f"sub-{test_element}_space-MNI152NLin2009cAsym_"
             "desc-preproc_T1w.nii.gz"
         )
 
         assert out["T1w"]["path"].exists()
         assert out["T1w"]["path"].is_file()
 
+        # asserts T1w_mask
+        assert out["T1w_mask"]["path"].exists()
+
         # asserts type "probseg_CSF"
         assert "probseg_CSF" in out
 
         assert (
             out["probseg_CSF"]["path"].name
             == f"sub-{test_element}_space-MNI152NLin2009cAsym_label-"
             "CSF_probseg.nii.gz"
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,26 +62,32 @@
                 == f"sub-{sub}_task-{new_task}_"
                 "desc-confounds_regressors.tsv"
             )
 
             assert out["BOLD_confounds"]["path"].exists()
             assert out["BOLD_confounds"]["path"].is_file()
 
+            # assert BOLD_mask
+            assert out["BOLD_mask"]["path"].exists()
+
             # asserts type "T1w"
             assert "T1w" in out
 
             assert (
                 out["T1w"]["path"].name
                 == f"sub-{sub}_space-MNI152NLin2009cAsym_"
                 "desc-preproc_T1w.nii.gz"
             )
 
             assert out["T1w"]["path"].exists()
             assert out["T1w"]["path"].is_file()
 
+            # asserts T1w_mask
+            assert out["T1w_mask"]["path"].exists()
+
             # asserts type "probseg_CSF"
             assert "probseg_CSF" in out
 
             assert (
                 out["probseg_CSF"]["path"].name
                 == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
                 "CSF_probseg.nii.gz"
@@ -137,9 +143,8 @@
     with pytest.raises(
         ValueError,
         match=(
             "thisisnotarealtask is not a valid task in "
             "the AOMIC PIOP1 dataset!"
         ),
     ):
-
         DataladAOMICPIOP1(tasks="thisisnotarealtask")
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.3.dev36/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,28 @@
     """Test datalad AOMICPIOP2 datagrabber."""
     configure_logging(level="DEBUG")
 
     uri_PIOP2 = "https://gin.g-node.org/juaml/datalad-example-aomicpiop2"
     task_params = [None, "restingstate"]
 
     for task_param in task_params:
-
         dg = DataladAOMICPIOP2(tasks=task_param)
 
         # change uri here to use fake data instead of real dataset
         dg.uri = uri_PIOP2
 
         with dg:
             all_elements = dg.get_elements()
 
             if task_param == "restingstate":
                 for el in all_elements:
                     assert el[1] == "restingstate"
 
             test_element = all_elements[0]
             sub, task = test_element
-
             out = dg[test_element]
 
             # asserts type "BOLD"
             assert "BOLD" in out
 
             new_task = f"{task}_acq-seq"
             assert (
@@ -58,26 +56,32 @@
                 == f"sub-{sub}_task-{new_task}_"
                 "desc-confounds_regressors.tsv"
             )
 
             assert out["BOLD_confounds"]["path"].exists()
             assert out["BOLD_confounds"]["path"].is_file()
 
+            # assert BOLD_mask
+            assert out["BOLD_mask"]["path"].exists()
+
             # asserts type "T1w"
             assert "T1w" in out
 
             assert (
                 out["T1w"]["path"].name
                 == f"sub-{sub}_space-MNI152NLin2009cAsym_"
                 "desc-preproc_T1w.nii.gz"
             )
 
             assert out["T1w"]["path"].exists()
             assert out["T1w"]["path"].is_file()
 
+            # asserts T1w_mask
+            assert out["T1w_mask"]["path"].exists()
+
             # asserts type "probseg_CSF"
             assert "probseg_CSF" in out
 
             assert (
                 out["probseg_CSF"]["path"].name
                 == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
                 "CSF_probseg.nii.gz"
@@ -133,9 +137,8 @@
     with pytest.raises(
         ValueError,
         match=(
             "thisisnotarealtask is not a valid task in "
             "the AOMIC PIOP2 dataset!"
         ),
     ):
-
         DataladAOMICPIOP2(tasks="thisisnotarealtask")
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/base.py` & `junifer-0.0.3.dev36/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/datalad_base.py` & `junifer-0.0.3.dev36/junifer/datagrabber/datalad_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Provide abstract base class for datalad datagrabber."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
+import atexit
+import os
+import shutil
 import tempfile
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
+import datalad
 import datalad.api as dl
+from datalad.support.exceptions import IncompleteResultsError
 from datalad.support.gitrepo import GitRepo
 
 from ..api.decorators import register_datagrabber
 from ..utils import logger, raise_error, warn_with_log
 from .base import BaseDataGrabber
 
 
@@ -63,32 +68,69 @@
         self,
         rootdir: Union[str, Path] = ".",
         datadir: Union[str, Path, None] = None,
         uri: Optional[str] = None,
         **kwargs,
     ):
         if datadir is None:
-            logger.warning("`datadir` is None, creating a temporary directory")
+            logger.info("`datadir` is None, creating a temporary directory")
             # Create temporary directory
-            datadir = tempfile.mkdtemp()
+            tmpdir = Path(tempfile.mkdtemp())
+            datadir = tmpdir / "datadir"
+            datadir.mkdir(parents=True, exist_ok=False)
             logger.info(f"`datadir` set to {datadir}")
+            cache_dir = tmpdir / ".datalad_cache"
+            sockets_dir = cache_dir / "sockets"
+            locks_dir = cache_dir / "locks"
+            sockets_dir.mkdir(parents=True, exist_ok=False)
+            locks_dir.mkdir(parents=True, exist_ok=False)
+            logger.debug(f"Setting datalad cache to {cache_dir}")
+            os.environ["DATALAD_LOCATIONS_CACHE"] = cache_dir.as_posix()
+            os.environ["DATALAD_LOCATIONS_SOCKETS"] = sockets_dir.as_posix()
+            os.environ["DATALAD_LOCATIONS_LOCKS"] = locks_dir.as_posix()
+            datalad.cfg.reload()
+            logger.debug(
+                "Datalad cache set to "
+                f"{datalad.cfg.get('datalad.locations.cache')}"
+            )
+            logger.debug(
+                "Datalad sockets set to "
+                f"{datalad.cfg.get('datalad.locations.sockets')}"
+            )
+            logger.debug(
+                "Datalad locks set to "
+                f"{datalad.cfg.get('datalad.locations.locks')}"
+            )
+            self._tmpdir = tmpdir
+            atexit.register(self._rmtmpdir)
         # TODO: uri can be converted to a positional argument
         if uri is None:
             raise_error("`uri` must be provided")
 
         super().__init__(datadir=datadir, **kwargs)
         logger.debug("Initializing DataladDataGrabber")
         logger.debug(f"\turi = {uri}")
         logger.debug(f"\t_rootdir = {rootdir}")
         self.uri = uri
         self._rootdir = rootdir
         # Flag to indicate if the dataset was cloned before and it might be
         # dirty
         self.datalad_dirty = False
 
+    def __del__(self) -> None:
+        """Destructor."""
+        if hasattr(self, "_tmpdir"):
+            self._rmtmpdir()
+
+    def _rmtmpdir(self) -> None:
+        """Remove temporary directory if it exists."""
+        if self._tmpdir.exists():
+            logger.debug("Removing temporary directory")
+            shutil.rmtree(self._tmpdir)
+
     @property
     def datadir(self) -> Path:
         """Get data directory path."""
         return super().datadir / self._rootdir
 
     def _get_dataset_id_remote(self) -> str:
         """Get the dataset id from the remote.
@@ -129,15 +171,18 @@
         to_get = [v["path"] for v in out.values() if "path" in v]
 
         if len(to_get) > 0:
             logger.debug(f"Getting {len(to_get)} files using datalad:")
             for fname in to_get:
                 logger.debug(f"\t: {fname}")
 
-            dl_out = self._dataset.get(to_get, result_renderer="disabled")
+            try:
+                dl_out = self._dataset.get(to_get, result_renderer="disabled")
+            except IncompleteResultsError as e:
+                raise_error(f"Failed to get from dataset: {e.failed}")
             if not self._was_cloned:
                 # If the dataset was already installed, check that the
                 # file was actually downloaded to avoid removing a
                 # file that was already there.
                 for t_out in dl_out:
                     t_path = Path(t_out["path"])
                     if t_out["status"] == "ok":
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/hcp.py` & `junifer-0.0.3.dev36/junifer/datagrabber/hcp.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,28 @@
     tasks : {"REST1", "REST2", "SOCIAL", "WM", "RELATIONAL", "EMOTION", \
             "LANGUAGE", "GAMBLING", "MOTOR"} or list of the options, optional
         HCP task sessions. If None, all available task sessions are selected
         (default None).
     phase_encodings : {"LR", "RL"} or list of the options, optional
         HCP phase encoding directions. If None, both will be used
         (default None).
+    ica_fix : bool, optional
+        Whether to retrieve data that was processed with ICA+FIX.
+        Only 'REST1' and 'REST2' tasks are available with ICA+FIX (default
+        False).
     **kwargs
         Keyword arguments passed to superclass.
-
     """
 
     def __init__(
         self,
         datadir: Union[str, Path],
         tasks: Union[str, List[str], None] = None,
         phase_encodings: Union[str, List[str], None] = None,
+        ica_fix: bool = False,
         **kwargs,
     ) -> None:
         # All tasks
         all_tasks = [
             "REST1",
             "REST2",
             "SOCIAL",
@@ -78,22 +82,29 @@
             if pe not in all_phase_encodings:
                 raise_error(
                     f"'{pe}' is not a valid HCP-YA phase encoding. "
                     "Valid phase encoding can be any or all of "
                     f"{all_phase_encodings}."
                 )
 
+        if ica_fix:
+            if not all([task in ["REST1", "REST2"] for task in self.tasks]):
+                raise_error(
+                    "ICA+FIX is only available for 'REST1' and 'REST2' tasks."
+                )
+        suffix = "_hp2000_clean" if ica_fix else ""
         # The types of data
         types = ["BOLD"]
         # The patterns
         patterns = {
             "BOLD": (
                 "{subject}/MNINonLinear/Results/"
                 "{task}_{phase_encoding}/"
-                "{task}_{phase_encoding}_hp2000_clean.nii.gz"
+                "{task}_{phase_encoding}"
+                f"{suffix}.nii.gz"
             )
         }
         # The replacements
         replacements = ["subject", "task", "phase_encoding"]
         super().__init__(
             types=types,
             datadir=datadir,
@@ -169,32 +180,38 @@
     tasks : {"REST1", "REST2", "SOCIAL", "WM", "RELATIONAL", "EMOTION", \
             "LANGUAGE", "GAMBLING", "MOTOR"} or list of the options, optional
         HCP task sessions. If None, all available task sessions are selected
         (default None).
     phase_encodings : {"LR", "RL"} or list of the options, optional
         HCP phase encoding directions. If None, both will be used
         (default None).
+    ica_fix : bool, optional
+        Whether to retrieve data that was processed with ICA+FIX.
+        Only 'REST1' and 'REST2' tasks are available with ICA+FIX (default
+        False).
     """
 
     def __init__(
         self,
         datadir: Union[str, Path, None] = None,
         tasks: Union[str, List[str], None] = None,
         phase_encodings: Union[str, List[str], None] = None,
+        ica_fix: bool = False,
     ) -> None:
         uri = (
             "https://github.com/datalad-datasets/"
             "human-connectome-project-openaccess.git"
         )
         rootdir = "HCP1200"
         super().__init__(
             datadir=datadir,
             tasks=tasks,
             phase_encodings=phase_encodings,
             uri=uri,
             rootdir=rootdir,
+            ica_fix=ica_fix,
         )
 
     @property
     def skip_file_check(self) -> bool:
         """Skip file check existence."""
         return True
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/multiple.py` & `junifer-0.0.3.dev36/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/pattern.py` & `junifer-0.0.3.dev36/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.3.dev36/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """Test BaseDataGrabber is abstract base class."""
     with pytest.raises(TypeError, match=r"abstract"):
         BaseDataGrabber(datadir="/tmp", types=["func"])  # type: ignore
 
 
 def test_BaseDataGrabber() -> None:
     """Test BaseDataGrabber."""
+
     # Create concrete class.
     class MyDataGrabber(BaseDataGrabber):
         def get_item(self, subject):
             return {"BOLD": {}}
 
         def get_elements(self):
             return super().get_elements()
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,57 @@
         assert elem1_t1w.is_file() is True
         assert elem1_t1w.is_symlink() is True
 
     assert datadir.exists() is False
     assert len(list(datadir.glob("*"))) == 0
 
 
+def test_datalad_clone_create_cleanup(concrete_datagrabber: Type) -> None:
+    """Test datalad base tempdir clone and remove.
+
+    Parameters
+    ----------
+    concrete_datagrabber : DataladDataGrabber
+        A concrete datagrabber class to use.
+    """
+
+    # Clone whole dataset
+    uri = _testing_dataset["example_bids"]["uri"]
+    with concrete_datagrabber(datadir=None, uri=uri) as dg:
+        datadir = dg._tmpdir / "datadir"
+        elem1_bold = (
+            datadir / "example_bids/sub-01/func/sub-01_task-rest_bold.nii.gz"
+        )
+        elem1_t1w = datadir / "example_bids/sub-01/anat/sub-01_T1w.nii.gz"
+
+        assert elem1_bold.is_file() is False
+        assert elem1_t1w.is_file() is False
+        assert datadir.exists() is True
+        assert dg._was_cloned is True
+        assert elem1_bold.is_file() is False
+        assert elem1_bold.is_symlink() is True
+        assert elem1_t1w.is_file() is False
+        assert elem1_t1w.is_symlink() is True
+        elem1 = dg["sub-01"]
+        assert "meta" in elem1["BOLD"]
+        meta = elem1["BOLD"]["meta"]
+        assert "datagrabber" in meta
+        assert "datalad_dirty" in meta["datagrabber"]
+        assert meta["datagrabber"]["datalad_dirty"] is False
+        assert hasattr(dg, "_got_files") is False
+        assert datadir.exists() is True
+        assert elem1_bold.is_file() is True
+        assert elem1_bold.is_symlink() is True
+        assert elem1_t1w.is_file() is True
+        assert elem1_t1w.is_symlink() is True
+
+    assert datadir.exists() is False
+    assert len(list(datadir.glob("*"))) == 0
+
+
 def test_datalad_previously_cloned(
     tmp_path: Path, concrete_datagrabber: Type
 ) -> None:
     """Test datalad base on cloned dataset.
 
     Parameters
     ----------
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_hcp.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_hcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Provide tests for HCP1200."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Optional, Iterable
+from typing import Iterable, Optional
 
 import pytest
 
-from junifer.datagrabber.hcp import DataladHCP1200, HCP1200
+from junifer.datagrabber.hcp import HCP1200, DataladHCP1200
 from junifer.utils import configure_logging
 
 
 URI = "https://gin.g-node.org/juaml/datalad-example-hcp1200"
 
 
 @pytest.fixture(scope="module")
@@ -25,63 +25,71 @@
     with dg:
         for t_elem in dg.get_elements():
             dg[t_elem]
         yield dg
 
 
 @pytest.mark.parametrize(
-    "tasks, phase_encodings, expected_path_name",
+    "tasks, phase_encodings, ica_fix, expected_path_name",
     [
-        (None, None, "rfMRI_REST1_LR_hp2000_clean.nii.gz"),
-        ("REST1", "LR", "rfMRI_REST1_LR_hp2000_clean.nii.gz"),
-        ("REST1", "RL", "rfMRI_REST1_RL_hp2000_clean.nii.gz"),
-        ("REST2", "LR", "rfMRI_REST2_LR_hp2000_clean.nii.gz"),
-        ("REST2", "RL", "rfMRI_REST2_RL_hp2000_clean.nii.gz"),
-        ("SOCIAL", "LR", "tfMRI_SOCIAL_LR_hp2000_clean.nii.gz"),
-        ("SOCIAL", "RL", "tfMRI_SOCIAL_RL_hp2000_clean.nii.gz"),
-        ("WM", "LR", "tfMRI_WM_LR_hp2000_clean.nii.gz"),
-        ("WM", "RL", "tfMRI_WM_RL_hp2000_clean.nii.gz"),
-        ("RELATIONAL", "LR", "tfMRI_RELATIONAL_LR_hp2000_clean.nii.gz"),
-        ("RELATIONAL", "RL", "tfMRI_RELATIONAL_RL_hp2000_clean.nii.gz"),
-        ("EMOTION", "LR", "tfMRI_EMOTION_LR_hp2000_clean.nii.gz"),
-        ("EMOTION", "RL", "tfMRI_EMOTION_RL_hp2000_clean.nii.gz"),
-        ("LANGUAGE", "LR", "tfMRI_LANGUAGE_LR_hp2000_clean.nii.gz"),
-        ("LANGUAGE", "RL", "tfMRI_LANGUAGE_RL_hp2000_clean.nii.gz"),
-        ("GAMBLING", "LR", "tfMRI_GAMBLING_LR_hp2000_clean.nii.gz"),
-        ("GAMBLING", "RL", "tfMRI_GAMBLING_RL_hp2000_clean.nii.gz"),
-        ("MOTOR", "LR", "tfMRI_MOTOR_LR_hp2000_clean.nii.gz"),
-        ("MOTOR", "RL", "tfMRI_MOTOR_RL_hp2000_clean.nii.gz"),
+        (None, None, False, "rfMRI_REST1_LR.nii.gz"),
+        ("REST1", "LR", False, "rfMRI_REST1_LR.nii.gz"),
+        ("REST1", "RL", False, "rfMRI_REST1_RL.nii.gz"),
+        ("REST2", "LR", False, "rfMRI_REST2_LR.nii.gz"),
+        ("REST2", "RL", False, "rfMRI_REST2_RL.nii.gz"),
+        ("SOCIAL", "LR", False, "tfMRI_SOCIAL_LR.nii.gz"),
+        ("SOCIAL", "RL", False, "tfMRI_SOCIAL_RL.nii.gz"),
+        ("WM", "LR", False, "tfMRI_WM_LR.nii.gz"),
+        ("WM", "RL", False, "tfMRI_WM_RL.nii.gz"),
+        ("RELATIONAL", "LR", False, "tfMRI_RELATIONAL_LR.nii.gz"),
+        ("RELATIONAL", "RL", False, "tfMRI_RELATIONAL_RL.nii.gz"),
+        ("EMOTION", "LR", False, "tfMRI_EMOTION_LR.nii.gz"),
+        ("EMOTION", "RL", False, "tfMRI_EMOTION_RL.nii.gz"),
+        ("LANGUAGE", "LR", False, "tfMRI_LANGUAGE_LR.nii.gz"),
+        ("LANGUAGE", "RL", False, "tfMRI_LANGUAGE_RL.nii.gz"),
+        ("GAMBLING", "LR", False, "tfMRI_GAMBLING_LR.nii.gz"),
+        ("GAMBLING", "RL", False, "tfMRI_GAMBLING_RL.nii.gz"),
+        ("MOTOR", "LR", False, "tfMRI_MOTOR_LR.nii.gz"),
+        ("MOTOR", "RL", False, "tfMRI_MOTOR_RL.nii.gz"),
+        ("REST1", "LR", True, "rfMRI_REST1_LR_hp2000_clean.nii.gz"),
+        ("REST1", "RL", True, "rfMRI_REST1_RL_hp2000_clean.nii.gz"),
+        ("REST2", "LR", True, "rfMRI_REST2_LR_hp2000_clean.nii.gz"),
+        ("REST2", "RL", True, "rfMRI_REST2_RL_hp2000_clean.nii.gz"),
     ],
 )
 def test_hcp1200_datagrabber(
     hcpdg: DataladHCP1200,
     tasks: Optional[str],
     phase_encodings: Optional[str],
+    ica_fix: bool,
     expected_path_name: str,
 ) -> None:
     """Test HCP1200 datagrabber.
 
     Parameters
     ----------
     hcpdg : DataladHCP1200
         The Datalad version of the datagrabber with the first subject
         already cloned.
     tasks : str
         The parametrized tasks.
     phase_encodings : str
         The parametrized phase encodings.
+    ica_fix : bool
+        The parametrized ICA-FIX flag.
     expected_path_name : str
         The parametrized expected path name.
 
     """
     configure_logging(level="DEBUG")
     dg = HCP1200(
         datadir=hcpdg.datadir,
         tasks=tasks,
         phase_encodings=phase_encodings,
+        ica_fix=ica_fix,
     )
     # Get all elements
     all_elements = dg.get_elements()
     # Get test element
     test_element = all_elements[0]
     # Get test element data
     out = dg[test_element]
@@ -328,19 +336,51 @@
     dg = HCP1200(
         datadir=hcpdg.datadir,
         tasks="REST1",
         phase_encodings="LR",
     )
     with dg:
         # Get all elements
-        expected_subjects = [
-            f"sub-{x:02d}" for x in range(1, 10)
-        ]
+        expected_subjects = [f"sub-{x:02d}" for x in range(1, 10)]
         found_subjects = []
         all_elements = dg.get_elements()
         # Check only specified task and phase encoding are found
         for element in all_elements:
             found_subjects.append(element[0])
             assert element[1] == "REST1"
             assert element[2] in ["LR", "RL"]
 
         assert set(found_subjects) == set(expected_subjects)
+
+
+@pytest.mark.parametrize(
+    "tasks, ica_fix",
+    [
+        ("SOCIAL", True),
+        ("WM", True),
+        ("RELATIONAL", True),
+        ("EMOTION", True),
+        ("LANGUAGE", True),
+        ("GAMBLING", True),
+        ("MOTOR", True),
+    ],
+)
+def test_hcp1200_datagrabber_incorrect_access_icafix(
+    tasks: Optional[str], ica_fix: bool
+) -> None:
+    """Test HCP1200 datagrabber incorrect access for icafix.
+
+    Parameters
+    ----------
+    tasks : str
+        The parametrized tasks.
+    ica_fix : bool
+        The parametrized ICA-FIX flag.
+
+    """
+    configure_logging(level="DEBUG")
+    with pytest.raises(ValueError, match="is only available for"):
+        _ = HCP1200(
+            datadir=".",
+            tasks=tasks,
+            ica_fix=ica_fix,
+        )
```

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.3.dev36/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datagrabber/utils.py` & `junifer-0.0.3.dev36/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/datareader/default.py` & `junifer-0.0.3.dev36/junifer/datareader/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,31 @@
 _readers["TSV"] = {"func": pd.read_csv, "params": {"sep": "\t"}}
 
 
 @register_datareader
 class DefaultDataReader(PipelineStepMixin, UpdateMetaMixin):
     """Mixin class for default data reader."""
 
-    def validate_input(self, input: List[str]) -> None:
+    def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data dictionary keys.
 
+        Returns
+        -------
+        list of str
+            The actual elements of the input that will be processed by this
+            pipeline step.
         """
         # Nothing to validate, any input is fine
-        pass
+        return input
 
     def get_output_type(self, input: List[str]) -> List[str]:
         """Get output type.
 
         Parameters
         ----------
         input : list of str
```

### Comparing `junifer-0.0.2.dev86/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.3.dev36/junifer/datareader/tests/test_default_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Parameters
     ----------
     type_ : list of str or str or None
         The parametrized type_ of data.
 
     """
     reader = DefaultDataReader()
-    assert reader.validate_input(type_) is None
+    assert reader.validate_input(type_) == type_
     assert reader.get_output_type(type_) == type_
     assert reader.validate(type_) == type_
 
 
 def test_meta() -> None:
     """Test reader metadata."""
     reader = DefaultDataReader()
```

### Comparing `junifer-0.0.2.dev86/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev36/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import TYPE_CHECKING, Callable, List, Optional, Tuple, Union
 
 import numpy as np
+from nilearn import image, masking
 from nilearn._utils.class_inspect import get_params
 from nilearn._utils.niimg import img_data_dtype
-from nilearn._utils.niimg_conversions import check_niimg_4d
+from nilearn._utils.niimg_conversions import (
+    _safe_get_data,
+    check_niimg_3d,
+    check_niimg_4d,
+)
 from nilearn.maskers import NiftiSpheresMasker
 from nilearn.maskers.base_masker import _filter_and_extract
-from nilearn.maskers.nifti_spheres_masker import _iter_signals_from_spheres
+from sklearn import neighbors
 
-from ...utils import raise_error
+from ...utils import raise_error, warn_with_log
 
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from nibabel import Nifti1Image, Nifti2Image
     from numpy.typing import ArrayLike, DTypeLike
@@ -55,14 +60,163 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
 DAMAGE.
 """
 
 
+def _apply_mask_and_get_affinity(
+    seeds, niimg, radius, allow_overlap, mask_img=None
+):
+    """Apply mask and get affinity matrix for given seeds.
+
+    Utility function to get only the rows which are occupied by sphere at
+    given seed locations and the provided radius. Rows are in target_affine and
+    target_shape space.
+
+    Parameters
+    ----------
+    seeds : List of triplets of coordinates in native space
+        Seed definitions. List of coordinates of the seeds in the same space
+        as target_affine.
+    niimg : 3D/4D Niimg-like object
+        See :ref:`extracting_data`.
+        Images to process.
+        If a 3D niimg is provided, a singleton dimension will be added to
+        the output to represent the single scan in the niimg.
+    radius : float
+        Indicates, in millimeters, the radius for the sphere around the seed.
+    allow_overlap : boolean
+        If False, a ValueError is raised if VOIs overlap
+    mask_img : Niimg-like object, optional
+        Mask to apply to regions before extracting signals. If niimg is None,
+        mask_img is used as a reference space in which the spheres 'indices are
+        placed.
+    Returns
+    -------
+    X : 2D numpy.ndarray
+        Signal for each brain voxel in the (masked) niimgs.
+        shape: (number of scans, number of voxels)
+    A : scipy.sparse.lil_matrix
+        Contains the boolean indices for each sphere.
+        shape: (number of seeds, number of voxels)
+    """
+    seeds = list(seeds)
+
+    # Compute world coordinates of all in-mask voxels.
+    if niimg is None:
+        mask, affine = masking._load_mask_img(mask_img)
+        # Get coordinate for all voxels inside of mask
+        mask_coords = np.asarray(np.nonzero(mask)).T.tolist()
+        X = None
+
+    elif mask_img is not None:
+        affine = niimg.affine
+        mask_img = check_niimg_3d(mask_img)
+        mask_img = image.resample_img(
+            mask_img,
+            target_affine=affine,
+            target_shape=niimg.shape[:3],
+            interpolation="nearest",
+        )
+        mask, _ = masking._load_mask_img(mask_img)
+        mask_coords = list(zip(*np.where(mask != 0)))
+
+        X = masking._apply_mask_fmri(niimg, mask_img)
+
+    elif niimg is not None:
+        affine = niimg.affine
+        if np.isnan(np.sum(_safe_get_data(niimg))):
+            warn_with_log(
+                "The imgs you have fed into fit_transform() contains NaN "
+                "values which will be converted to zeroes."
+            )
+            X = _safe_get_data(niimg, True).reshape([-1, niimg.shape[3]]).T
+        else:
+            X = _safe_get_data(niimg).reshape([-1, niimg.shape[3]]).T
+
+        mask_coords = list(np.ndindex(niimg.shape[:3]))
+
+    else:
+        raise_error("Either a niimg or a mask_img must be provided.")
+
+    # For each seed, get coordinates of nearest voxel
+    nearests = []
+    for sx, sy, sz in seeds:
+        nearest = np.round(
+            image.resampling.coord_transform(sx, sy, sz, np.linalg.inv(affine))
+        )
+        nearest = nearest.astype(int)
+        nearest = (nearest[0], nearest[1], nearest[2])
+        try:
+            nearests.append(mask_coords.index(nearest))
+        except ValueError:
+            nearests.append(None)
+
+    mask_coords = np.asarray(list(zip(*mask_coords)))
+    mask_coords = image.resampling.coord_transform(
+        mask_coords[0], mask_coords[1], mask_coords[2], affine
+    )
+    mask_coords = np.asarray(mask_coords).T
+
+    clf = neighbors.NearestNeighbors(radius=radius)
+    A = clf.fit(mask_coords).radius_neighbors_graph(seeds)
+    A = A.tolil()
+    for i, nearest in enumerate(nearests):
+        if nearest is None:
+            continue
+
+        A[i, nearest] = True
+
+    # Include the voxel containing the seed itself if not masked
+    mask_coords = mask_coords.astype(int).tolist()
+    for i, seed in enumerate(seeds):
+        try:
+            A[i, mask_coords.index(list(map(int, seed)))] = True
+        except ValueError:
+            # seed is not in the mask
+            pass
+
+    if (not allow_overlap) and np.any(A.sum(axis=0) >= 2):
+        raise_error("Overlap detected between spheres")
+
+    return X, A
+
+
+def _iter_signals_from_spheres(
+    seeds, niimg, radius, allow_overlap, mask_img=None
+):
+    """Iterate over spheres.
+
+    Parameters
+    ----------
+    seeds : :obj:`list` of triplets of coordinates in native space
+        Seed definitions. List of coordinates of the seeds in the same space
+        as the images (typically MNI or TAL).
+    niimg : 3D/4D Niimg-like object
+        See :ref:`extracting_data`.
+        Images to process.
+        If a 3D niimg is provided, a singleton dimension will be added to
+        the output to represent the single scan in the niimg.
+    radius: float
+        Indicates, in millimeters, the radius for the sphere around the seed.
+    allow_overlap: boolean
+        If False, an error is raised if the maps overlaps (ie at least two
+        maps have a non-zero value for the same voxel).
+    mask_img : Niimg-like object, optional
+        See :ref:`extracting_data`.
+        Mask to apply to regions before extracting signals.
+    """
+    X, A = _apply_mask_and_get_affinity(
+        seeds, niimg, radius, allow_overlap, mask_img=mask_img
+    )
+    for _, row in enumerate(A.rows):
+        yield X[:, row]
+
+
 class _JuniferExtractionFunctor:
     """Functor to extract signals from spheres.
 
     Parameters
     ----------
     seeds_ : list of triple of coordinates in native space
         Seed definitions. List of coordinates of the seeds in the same space
@@ -145,35 +299,42 @@
             signals[:, i] = self.agg_func(sphere, axis=1)
         return signals, None
 
 
 class JuniferNiftiSpheresMasker(NiftiSpheresMasker):
     """Class for custom NiftiSpheresMasker.
 
+    Differs from :class:`nilearn.maskers.NiftiSpheresMasker` in the following
+    ways:
+
+    * it allows to pass any callable as the ``agg_func`` parameter.
+    * empty spheres do not create an error. Instead, ``agg_func`` is applied to
+      an empty array and the result is passed.
+
     Parameters
     ----------
-    seeds : list of triplet of coordinates in native space
+    seeds : list of float
         Seed definitions. List of coordinates of the seeds in the same space
         as the images (typically MNI or TAL).
     radius : float, optional
         Indicates, in millimeters, the radius for the sphere around the seed.
         If None, signal is extracted on a single voxel (default None).
     mask_img : Niimg-like object, optional
         Mask to apply to regions before extracting signals (default None).
     agg_func : callable, optional
         The function to aggregate signals using (default numpy.mean).
     allow_overlap : bool, optional
         If False, an error is raised if the maps overlap (default None).
-    dtype : any type that can be coerced into a numpy dtype or "auto", optional
+    dtype : numpy.dtype or "auto", optional
         The dtype for the extraction. If "auto", the data will be converted to
         int32 if dtype is discrete and float32 if it is continuous
         (default None).
     **kwargs
         Keyword arguments are passed to the
-        :func:`nilearn.maskers.NiftiSpheresMasker`.
+        :class:`nilearn.maskers.NiftiSpheresMasker`.
 
     """
 
     def __init__(
         self,
         seeds: "ArrayLike",
         radius: Optional[float] = None,
@@ -204,19 +365,19 @@
 
         Parameters
         ----------
         imgs : 3D/4D Niimg-like object
             Images to process.
             If a 3D niimg is provided, a singleton dimension will be added to
             the output to represent the single scan in the niimg.
-        confounds : CSV file or array-like or pandas.DataFrame, optional
+        confounds : pandas.DataFrame, optional
             This parameter is passed to :func:`nilearn.signal.clean`.
             Please see the related documentation for details.
             shape: (number of scans, number of confounds)
-        sample_mask : Any type compatible with numpy-array indexing, optional
+        sample_mask : np.ndarray, list or tuple, optional
             Masks the niimgs along time/fourth dimension to perform scrubbing
             (remove volumes with high motion) and/or non-steady-state volumes.
             This parameter is passed to :func:`nilearn.signal.clean`.
             shape: (number of scans - number of volumes removed, )
 
         Returns
         -------
```

### Comparing `junifer-0.0.2.dev86/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev36/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,16 +212,17 @@
     mask[1, 1, 0] = 1
 
     masker = JuniferNiftiSpheresMasker(
         seeds=[seed],
         radius=0.1,
         mask_img=nibabel.Nifti1Image(mask, affine),
     )
-    with pytest.raises(ValueError, match="These spheres are empty"):
-        masker.fit_transform(nibabel.Nifti1Image(data, affine))
+
+    out = masker.fit_transform(nibabel.Nifti1Image(data, affine))
+    assert np.isnan(out).all()
 
     masker = JuniferNiftiSpheresMasker(
         seeds=[seed],
         radius=1.6,
         mask_img=nibabel.Nifti1Image(mask, affine),
     )
     masker.fit_transform(nibabel.Nifti1Image(data, affine))
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/base.py` & `junifer-0.0.3.dev36/junifer/markers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,48 +41,56 @@
         self.name = self.__class__.__name__ if name is None else name
 
         if any(x not in self.get_valid_inputs() for x in on):
             wrong_on = [x for x in on if x not in self.get_valid_inputs()]
             raise ValueError(f"{self.name} cannot be computed on {wrong_on}")
         self._on = on
 
+    @abstractmethod
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
         """
         raise_error(
             msg="Concrete classes need to implement get_valid_inputs().",
             klass=NotImplementedError,
         )
 
-    def validate_input(self, input: List[str]) -> None:
+    def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data dictionary keys.
 
+        Returns
+        -------
+        list of str
+            The actual elements of the input that will be processed by this
+            pipeline step.
+
         Raises
         ------
         ValueError
             If the input does not have the required data.
 
         """
         if not any(x in input for x in self._on):
             raise_error(
                 "Input does not have the required data."
                 f"\t Input: {input}"
                 f"\t Required (any of): {self._on}"
             )
+        return [x for x in self._on if x in input]
 
     @abstractmethod
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/collection.py` & `junifer-0.0.3.dev36/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/ets_rss.py` & `junifer-0.0.3.dev36/junifer/markers/ets_rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,45 +21,45 @@
 class RSSETSMarker(BaseMarker):
     """Class for root sum of squares of edgewise timeseries.
 
     Parameters
     ----------
     parcellation : str or list of str
         The name(s) of the parcellation(s). Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     agg_method : str, optional
         The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default "mean").
+        :func:`.get_aggfunc_by_name` (default "mean").
     agg_method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+        :func:`.get_aggfunc_by_name` (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     """
 
     _DEPENDENCIES = {"nilearn"}
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.parcellation = parcellation
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
-        self.mask = mask
+        self.masks = masks
         super().__init__(name=name)
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
@@ -106,16 +106,15 @@
         Returns
         -------
         dict
             The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
-            * ``row_names`` (if more than one row is present in data): "scan"
+            * ``col_names`` : the column labels for the computed values as list
 
         References
         ----------
         .. [1] Zamani Esfahlani et al. (2020)
                High-amplitude cofluctuations in cortical activity drive
                functional connectivity
                doi: 10.1073/pnas.2005531117
@@ -123,17 +122,19 @@
         """
         logger.debug("Calculating root sum of squares of edgewise timeseries.")
         # Initialize a ParcelAggregation
         parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
-            mask=self.mask,
+            masks=self.masks,
         )
         # Compute the parcel aggregation
         out = parcel_aggregation.compute(input=input, extra_input=extra_input)
-        edge_ts = _ets(out["data"])
+        edge_ts, _ = _ets(out["data"])
         # Compute the RSS
         out["data"] = np.sum(edge_ts**2, 1) ** 0.5
+        # Make it 2D
+        out["data"] = out["data"][:, np.newaxis]
         # Set correct column label
-        out["columns"] = ["root_sum_of_squares_ets"]
+        out["col_names"] = ["root_sum_of_squares_ets"]
         return out
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/falff_base.py` & `junifer-0.0.3.dev36/junifer/markers/falff/falff_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # License: AGPL
 
 from abc import abstractmethod
 from typing import Dict, List, Optional
 
 from ...utils.logging import raise_error
 from ..base import BaseMarker
-from .falff_estimator import AmplitudeLowFrequencyFluctuationEstimator
+from .falff_estimator import ALFFEstimator
 
 
-class AmplitudeLowFrequencyFluctuationBase(BaseMarker):
+class ALFFBase(BaseMarker):
     """Base class for (fractional) Amplitude Low Frequency Fluctuation.
 
     Parameters
     ----------
     fractional : bool
         Whether to compute fractional ALFF.
     highpass : positive float
@@ -57,16 +57,16 @@
         fractional: bool,
         highpass: float,
         lowpass: float,
         tr: Optional[float] = None,
         use_afni: Optional[bool] = None,
         name: Optional[str] = None,
     ) -> None:
-        if highpass <= 0:
-            raise_error("Highpass must be positive")
+        if highpass < 0:
+            raise_error("Highpass must be positive or 0")
         if lowpass <= 0:
             raise_error("Lowpass must be positive")
         if highpass >= lowpass:
             raise_error("Highpass must be lower than lowpass")
         self.highpass = highpass
         self.lowpass = lowpass
         self.tr = tr
@@ -100,15 +100,15 @@
 
         Returns
         -------
         str
             The storage type output by the marker.
 
         """
-        return "table"
+        return "vector"
 
     def compute(
         self,
         input: Dict[str, Dict],
         extra_input: Optional[Dict] = None,
     ) -> Dict:
         """Compute.
@@ -128,52 +128,57 @@
         -------
         dict
             The computed result as dictionary. This will be either returned
             to the user or stored in the storage by calling the store method
             with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
-            * ``row_names`` (if more than one row is present in data): "scan"
+            * ``col_names`` : the column labels for the computed values as list
 
         """
         if self.use_afni is None:
             raise_error(
                 "Parameter `use_afni` must be set to True or False in order "
                 "to compute this marker. It is currently set to None (default "
                 "behaviour). This is intended to be for auto-detection. In "
                 "order for that to happen, please call the `validate` method "
                 "before calling the `compute` method."
             )
 
-        estimator = AmplitudeLowFrequencyFluctuationEstimator()
+        estimator = ALFFEstimator()
 
         alff, falff = estimator.fit_transform(
             use_afni=self.use_afni,
             input_data=input,
             highpass=self.highpass,
             lowpass=self.lowpass,
             tr=self.tr,
         )
         post_data = falff if self.fractional else alff
 
-        post_input = {
-            "data": post_data,
-            "path": None,
-        }
+        post_input = {k: v for k, v in input.items()}
+        post_input["data"] = post_data
+        post_input["path"] = None
 
-        out = self._postprocess(post_input)
+        out = self._postprocess(post_input, extra_input=extra_input)
 
         return out
 
     @abstractmethod
-    def _postprocess(self, input: Dict) -> Dict:
+    def _postprocess(
+        self, input: Dict, extra_input: Optional[Dict] = None
+    ) -> Dict:
         """Postprocess the output of the estimator.
 
         Parameters
         ----------
         input : dict
             The output of the estimator. It must have the following
+        extra_input : dict, optional
+            The other fields in the pipeline data object. Useful for accessing
+            other data kind that needs to be used in the computation. For
+            example, the functional connectivity markers can make use of the
+            confounds if available (default None).
         """
         raise_error(
             "_postprocess must be implemented", klass=NotImplementedError
         )
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.3.dev36/junifer/markers/falff/falff_estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,23 @@
 
 
 if TYPE_CHECKING:
     from nibabel import Nifti1Image, Nifti2Image
 
 
 @singleton
-class AmplitudeLowFrequencyFluctuationEstimator:
-    """Estimator class for AmplitudeLowFrequencyFluctuationBase.
+class ALFFEstimator:
+    """Estimator class for (fractional) Amplitude Low Frequency Fluctuation.
 
     This class is a singleton and is used for efficient computation of fALFF,
     by caching the voxel-wise ALFF map for a given set of file path and
     computation parameters.
 
-    .. warning:: This class can only be used via
-    :class:`junifer.markers.falff.AmplitudeLowFrequencyFluctuationBase`
-    as it serves a specific purpose.
+    .. warning:: This class can only be used via :class:`.ALFFBase` as it
+    serves a specific purpose.
 
     Parameters
     ----------
     use_afni : bool
         Whether to use afni for computation. If False, will use python.
 
     """
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/falff/falff_parcels.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,50 +5,49 @@
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
 # License: AGPL
 
 from typing import Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
 from .. import ParcelAggregation
-from .falff_base import AmplitudeLowFrequencyFluctuationBase
+from .falff_base import ALFFBase
 
 
 @register_marker
-class AmplitudeLowFrequencyFluctuationParcels(
-    AmplitudeLowFrequencyFluctuationBase
-):
+class ALFFParcels(ALFFBase):
     """Class for computing fALFF/ALFF on parcels.
 
     Parameters
     ----------
     parcellation : str or list of str
         The name(s) of the parcellation(s). Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     fractional : bool
         Whether to compute fractional ALFF.
     highpass : positive float, optional
-        The highpass cutoff frequency for the bandpass filter (default 0.01).
+        The highpass cutoff frequency for the bandpass filter. If 0,
+        it will not apply a highpass filter (default 0.01).
     lowpass : positive float, optional
         The lowpass cutoff frequency for the bandpass filter (default 0.1).
     tr : positive float, optional
         The Repetition Time of the BOLD data. If None, will extract
         the TR from NIFTI header (default None).
     use_afni : bool, optional
         Whether to use AFNI for computing. If None, will use AFNI only
         if available (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     method : str, optional
         The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default "mean").
+        :func:`.get_aggfunc_by_name` (default "mean").
     method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name`.
+        :func:`.get_aggfunc_by_name`.
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     Notes
     -----
     The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
@@ -66,33 +65,35 @@
         self,
         parcellation: Union[str, List[str]],
         fractional: bool,
         highpass: float = 0.01,
         lowpass: float = 0.1,
         tr: Optional[float] = None,
         use_afni: Optional[bool] = None,
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         method: str = "mean",
         method_params: Optional[Dict] = None,
         name: Optional[str] = None,
     ) -> None:
         self.parcellation = parcellation
-        self.mask = mask
+        self.masks = masks
         self.method = method
         self.method_params = method_params
         super().__init__(
             fractional=fractional,
             highpass=highpass,
             lowpass=lowpass,
             tr=tr,
             name=name,
             use_afni=use_afni,
         )
 
-    def _postprocess(self, input: Dict) -> Dict:
+    def _postprocess(
+        self, input: Dict, extra_input: Optional[Dict] = None
+    ) -> Dict:
         """Compute ALFF and fALFF.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
             the marker.
@@ -105,22 +106,22 @@
         Returns
         -------
         dict
             The computed ALFF as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
+            * ``col_names`` : the column labels for the computed values as list
 
         """
         pa = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.method,
             method_params=self.method_params,
-            mask=self.mask,
+            masks=self.masks,
             on="fALFF",
         )
 
         # get the 2D timeseries after parcel aggregation
-        out = pa.compute(input)
+        out = pa.compute(input, extra_input=extra_input)
 
         return out
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,91 @@
-"""Provide class for computing fALFF on spheres."""
+"""Provide class for functional connectivity using spheres."""
 
-# Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
-#          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
+# Authors: Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
-from .. import SphereAggregation
-from .falff_base import AmplitudeLowFrequencyFluctuationBase
+from ..sphere_aggregation import SphereAggregation
+from ..utils import raise_error
+from .functional_connectivity_base import FunctionalConnectivityBase
 
 
 @register_marker
-class AmplitudeLowFrequencyFluctuationSpheres(
-    AmplitudeLowFrequencyFluctuationBase
-):
-    """Class for computing fALFF/ALFF on spheres.
+class FunctionalConnectivitySpheres(FunctionalConnectivityBase):
+    """Class for functional connectivity using coordinates (spheres).
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
-        :func:`junifer.data.coordinates.list_coordinates` for options.
+        :func:`.list_coordinates` for options.
     radius : float, optional
         The radius of the sphere in mm. If None, the signal will be extracted
         from a single voxel. See :class:`nilearn.maskers.NiftiSpheresMasker`
         for more information (default None).
-    fractional : bool
-        Whether to compute fractional ALFF.
-    highpass : positive float, optional
-        The highpass cutoff frequency for the bandpass filter (default 0.01).
-    lowpass : positive float, optional
-        The lowpass cutoff frequency for the bandpass filter (default 0.1).
-    tr : positive float, optional
-        The Repetition Time of the BOLD data. If None, will extract
-        the TR from NIFTI header (default None).
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
+    allow_overlap : bool, optional
+        Whether to allow overlapping spheres. If False, an error is raised if
+        the spheres overlap (default is False).
+    agg_method : str, optional
+        The aggregation method to use.
+        See :func:`.get_aggfunc_by_name` for more information
         (default None).
-    method : str, optional
-        The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default "mean").
-    method_params : dict, optional
-        Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name`.
+    agg_method_params : dict, optional
+        The parameters to pass to the aggregation method (default None).
+    cor_method : str, optional
+        The method to perform correlation using. Check valid options in
+        :class:`nilearn.connectome.ConnectivityMeasure` (default "covariance").
+    cor_method_params : dict, optional
+        Parameters to pass to the correlation function. Check valid options in
+        :class:`nilearn.connectome.ConnectivityMeasure` (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
-        The name of the marker. If None, will use the class name (default
-        None).
+        The name of the marker. By default, it will use
+        KIND_FunctionalConnectivitySpheres where KIND is the kind of data it
+        was applied to (default None).
 
-    Notes
-    -----
-    The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
-    computation. If a dataset is correctly preprocessed, the TR should be
-    extracted from the NIFTI without any issue. However, it has been
-    reported that some preprocessed data might not have the correct TR in
-    the NIFTI header.
-
-    ALFF/fALFF are computed using a bandpass butterworth filter. See
-    :func:`scipy.signal.butter` and :func:`scipy.signal.filtfilt` for more
-    details.
     """
 
     def __init__(
         self,
         coords: str,
-        fractional: bool,
         radius: Optional[float] = None,
-        highpass: float = 0.01,
-        lowpass: float = 0.1,
-        tr: Optional[float] = None,
-        use_afni: Optional[bool] = None,
-        mask: Union[str, Dict, None] = None,
-        method: str = "mean",
-        method_params: Optional[Dict] = None,
+        allow_overlap: bool = False,
+        agg_method: str = "mean",
+        agg_method_params: Optional[Dict] = None,
+        cor_method: str = "covariance",
+        cor_method_params: Optional[Dict] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.coords = coords
         self.radius = radius
-        self.mask = mask
-        self.method = method
-        self.method_params = method_params
+        self.allow_overlap = allow_overlap
+        if radius is None or radius <= 0:
+            raise_error(f"radius should be > 0: provided {radius}")
         super().__init__(
-            fractional=fractional,
-            highpass=highpass,
-            lowpass=lowpass,
-            tr=tr,
+            agg_method=agg_method,
+            agg_method_params=agg_method_params,
+            cor_method=cor_method,
+            cor_method_params=cor_method_params,
+            masks=masks,
             name=name,
-            use_afni=use_afni,
         )
 
-    def _postprocess(self, input: Dict) -> Dict:
-        """Compute ALFF and fALFF.
+    def aggregate(
+        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
+    ) -> Dict:
+        """Perform sphere aggregation.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
             the marker.
         extra_input : dict, optional
@@ -107,27 +93,26 @@
             other data kind that needs to be used in the computation. For
             example, the functional connectivity markers can make use of the
             confounds if available (default None).
 
         Returns
         -------
         dict
-            The computed ALFF as dictionary. The dictionary has the following
-            keys:
+            The computed result as dictionary. This will be either returned
+            to the user or stored in the storage by calling the store method
+            with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
+            * ``col_names`` : the column labels for the computed values as list
 
         """
-        pa = SphereAggregation(
+        sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
-            method=self.method,
-            method_params=self.method_params,
-            mask=self.mask,
-            on="fALFF",
+            allow_overlap=self.allow_overlap,
+            method=self.agg_method,
+            method_params=self.agg_method_params,
+            masks=self.masks,
+            on="BOLD",
         )
-
-        # get the 2D timeseries after parcel aggregation
-        out = pa.compute(input)
-
-        return out
+        # Return the 2D timeseries after sphere aggregation
+        return sphere_aggregation.compute(input, extra_input=extra_input)
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.3.dev36/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 import time
 
 import pytest
 from nibabel import Nifti1Image
 from scipy.stats import pearsonr
 
 from junifer.datareader import DefaultDataReader
-from junifer.markers.falff.falff_estimator import (
-    AmplitudeLowFrequencyFluctuationEstimator,
-)
+from junifer.markers.falff.falff_estimator import ALFFEstimator
 from junifer.pipeline.utils import _check_afni
 from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
 from junifer.utils import logger
 
 
-def test_AmplitudeLowFrequencyFluctuationEstimator_cache_python() -> None:
+def test_ALFFEstimator_cache_python() -> None:
     """Test that the cache works properly when using python."""
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
 
-    estimator = AmplitudeLowFrequencyFluctuationEstimator()
+    estimator = ALFFEstimator()
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=False,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
@@ -107,22 +105,22 @@
     n_files = len([x for x in estimator.temp_dir_path.glob("*")])
     assert n_files == 0  # no files in python
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
-def test_AmplitudeLowFrequencyFluctuationEstimator_cache_afni() -> None:
+def test_ALFFEstimator_cache_afni() -> None:
     """Test that the cache works properly when using afni."""
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
 
-    estimator = AmplitudeLowFrequencyFluctuationEstimator()
+    estimator = ALFFEstimator()
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=True,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
@@ -200,21 +198,21 @@
     n_files = len([x for x in estimator.temp_dir_path.glob("*")])
     assert n_files == 3  # input + alff + falff
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
-def test_AmplitudeLowFrequencyFluctuationEstimator_afni_vs_python() -> None:
+def test_ALFFEstimator_afni_vs_python() -> None:
     """Test that the cache works properly when using afni."""
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
-    estimator = AmplitudeLowFrequencyFluctuationEstimator()
+    estimator = ALFFEstimator()
 
     # Use an arbitrary TR to test the AFNI vs Python implementation
     afni_alff, afni_falff = estimator.fit_transform(
         use_afni=True,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,160 @@
-"""Provide test for parcel-aggregated (f)ALFF."""
+"""Provide test for sphere-aggregated (f)ALFF."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
 import pytest
 from numpy.testing import assert_array_equal
 from scipy.stats import pearsonr
 
 from junifer.datareader import DefaultDataReader
-from junifer.markers.falff import AmplitudeLowFrequencyFluctuationParcels
+from junifer.markers.falff import ALFFSpheres
 from junifer.pipeline.utils import _check_afni
 from junifer.storage import SQLiteFeatureStorage
 from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
 from junifer.utils import logger
 
 
-_PARCELLATION = "Schaefer100x7"
+_COORDINATES = "DMNBuckner"
 
 
-def test_AmplitudeLowFrequencyFluctuationParcels_python() -> None:
-    """Test AmplitudeLowFrequencyFluctuationParcels using python."""
+def test_ALFFSpheres_python() -> None:
+    """Test ALFFSpheres using python."""
     # Get the SPM auditory data:
 
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
     # Create ParcelAggregation object
-    marker = AmplitudeLowFrequencyFluctuationParcels(
-        parcellation=_PARCELLATION,
+    marker = ALFFSpheres(
+        coords=_COORDINATES,
+        radius=5,
         method="mean",
         use_afni=False,
         fractional=False,
     )
     python_values = marker.fit_transform(input)["BOLD"]["data"]
 
     assert marker.use_afni is False
     assert python_values.ndim == 2
-    assert python_values.shape == (1, 100)
+    assert python_values.shape == (1, 6)
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
-def test_AmplitudeLowFrequencyFluctuationParcels_afni() -> None:
-    """Test AmplitudeLowFrequencyFluctuationParcels using afni."""
+def test_ALFFSpheres_afni() -> None:
+    """Test ALFFSpheres using afni."""
     # Get the SPM auditory data:
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
     # Create ParcelAggregation object
-    marker = AmplitudeLowFrequencyFluctuationParcels(
-        parcellation=_PARCELLATION,
+    marker = ALFFSpheres(
+        coords=_COORDINATES,
+        radius=5,
         method="mean",
         use_afni=True,
         fractional=False,
     )
     assert marker.use_afni is True
     afni_values = marker.fit_transform(input)["BOLD"]["data"]
 
     assert afni_values.ndim == 2
-    assert afni_values.shape == (1, 100)
+    assert afni_values.shape == (1, 6)
 
     # Again, should be blazing fast
-    marker = AmplitudeLowFrequencyFluctuationParcels(
-        parcellation=_PARCELLATION, method="mean", fractional=False
+    marker = ALFFSpheres(
+        coords=_COORDINATES,
+        radius=5,
+        method="mean",
+        fractional=False,
     )
     assert marker.use_afni is None
     afni_values2 = marker.fit_transform(input)["BOLD"]["data"]
     assert marker.use_afni is True
     assert_array_equal(afni_values, afni_values2)
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
 @pytest.mark.parametrize(
     "fractional", [True, False], ids=["fractional", "non-fractional"]
 )
-def test_AmplitudeLowFrequencyFluctuationParcels_python_vs_afni(
+def test_ALFFSpheres_python_vs_afni(
     fractional: bool,
 ) -> None:
-    """Test AmplitudeLowFrequencyFluctuationParcels using python.
+    """Test ALFFSpheres python vs afni results.
 
     Parameters
     ----------
-    factional : bool
+    fractional : bool
         Whether to compute fractional ALFF or not.
     """
-
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
     # Create ParcelAggregation object
-    marker_python = AmplitudeLowFrequencyFluctuationParcels(
-        parcellation=_PARCELLATION,
+    marker_python = ALFFSpheres(
+        coords=_COORDINATES,
+        radius=5,
         method="mean",
         use_afni=False,
         fractional=fractional,
     )
     python_values = marker_python.fit_transform(input)["BOLD"]["data"]
 
     assert marker_python.use_afni is False
     assert python_values.ndim == 2
-    assert python_values.shape == (1, 100)
+    assert python_values.shape == (1, 6)
 
-    marker_afni = AmplitudeLowFrequencyFluctuationParcels(
-        parcellation=_PARCELLATION,
+    marker_afni = ALFFSpheres(
+        coords=_COORDINATES,
+        radius=5,
         method="mean",
         use_afni=True,
         fractional=fractional,
     )
     afni_values = marker_afni.fit_transform(input)["BOLD"]["data"]
 
     assert marker_afni.use_afni is True
     assert afni_values.ndim == 2
-    assert afni_values.shape == (1, 100)
+    assert afni_values.shape == (1, 6)
 
     r, p = pearsonr(python_values[0], afni_values[0])
     logger.info(f"Correlation between python and afni: {r} (p={p})")
     assert r > 0.99
 
 
-def test_AmplitudeLowFrequencyFluctuationParcels_storage(
+def test_ALFFSpheres_storage(
     tmp_path: Path,
 ) -> None:
-    """Test AmplitudeLowFrequencyFluctuationParcels storage.
+    """Test ALFFSpheres storage.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
     """
     with PartlyCloudyTestingDataGrabber() as dg:
         # Use first subject
         input = dg["sub-01"]
         input = DefaultDataReader().fit_transform(input)
         # Create ParcelAggregation object
-        marker = AmplitudeLowFrequencyFluctuationParcels(
-            parcellation=_PARCELLATION,
+        marker = ALFFSpheres(
+            coords=_COORDINATES,
+            radius=5,
             method="mean",
             use_afni=False,
             fractional=True,
         )
         storage = SQLiteFeatureStorage(tmp_path / "alff_parcels.sqlite")
 
         # Fit transform marker on data with storage
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,43 +26,43 @@
     parcellation_two : str
         The name of the second parcellation.
     aggregation_method : str, optional
         The aggregation method (default "mean").
     correlation_method : str, optional
         Any method that can be passed to
         :any:`pandas.DataFrame.corr` (default "pearson").
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name
         (default None).
     """
 
     _DEPENDENCIES = {"nilearn"}
 
     def __init__(
         self,
         parcellation_one: str,
         parcellation_two: str,
         aggregation_method: str = "mean",
         correlation_method: str = "pearson",
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         if parcellation_one == parcellation_two:
             raise_error(
                 "The two parcellations must be different.",
             )
         self.parcellation_one = parcellation_one
         self.parcellation_two = parcellation_two
         self.aggregation_method = aggregation_method
         self.correlation_method = correlation_method
-        self.mask = mask
+        self.masks = masks
         super().__init__(on=["BOLD"], name=name)
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
@@ -125,31 +125,31 @@
             f" {self.parcellation_one} and "
             f"{self.parcellation_two} parcellations."
         )
         # Initialize a ParcelAggregation
         parcellation_one_dict = ParcelAggregation(
             parcellation=self.parcellation_one,
             method=self.aggregation_method,
-            mask=self.mask,
-        ).compute(input)
+            masks=self.masks,
+        ).compute(input, extra_input=extra_input)
         parcellation_two_dict = ParcelAggregation(
             parcellation=self.parcellation_two,
             method=self.aggregation_method,
-            mask=self.mask,
-        ).compute(input)
+            masks=self.masks,
+        ).compute(input, extra_input=extra_input)
 
         parcellated_ts_one = parcellation_one_dict["data"]
         parcellated_ts_two = parcellation_two_dict["data"]
         # columns should be named after parcellation 1
         # rows should be named after parcellation 2
 
         result = _correlate_dataframes(
             pd.DataFrame(parcellated_ts_one),
             pd.DataFrame(parcellated_ts_two),
             method=self.correlation_method,
         ).values
 
         return {
             "data": result,
-            "col_names": parcellation_one_dict["columns"],
-            "row_names": parcellation_two_dict["columns"],
+            "col_names": parcellation_one_dict["col_names"],
+            "row_names": parcellation_two_dict["col_names"],
         }
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,89 @@
-"""Provide class for edge-centric functional connectivity using parcels."""
+"""Provide class for temporal SNR using parcels."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
-#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
 from ..parcel_aggregation import ParcelAggregation
-from ..utils import _ets
-from .functional_connectivity_base import FunctionalConnectivityBase
+from .temporal_snr_base import TemporalSNRBase
 
 
 @register_marker
-class EdgeCentricFCParcels(FunctionalConnectivityBase):
-    """Class for edge-centric FC using parcellations.
+class TemporalSNRParcels(TemporalSNRBase):
+    """Class for temporal signal-to-noise ratio using parcellations.
 
     Parameters
     ----------
     parcellation : str or list of str
         The name(s) of the parcellation(s). Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     agg_method : str, optional
-        The method to perform aggregation of BOLD time series.
-        Check valid options in :func:`junifer.stats.get_aggfunc_by_name`
-        (default "mean").
+        The method to perform aggregation using. Check valid options in
+        :func:`.get_aggfunc_by_name` (default "mean").
     agg_method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default None).
-    cor_method : str, optional
-        The method to perform correlation. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure`
-        (default "covariance").
-    cor_method_params : dict, optional
-        Parameters to pass to the correlation function. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure` (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+        :func:`.get_aggfunc_by_name` (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
-    References
-    ----------
-    .. [1] Jo et al. (2021)
-            Subject identification using
-            edge-centric functional connectivity
-            doi: https://doi.org/10.1016/j.neuroimage.2021.118204
-
     """
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        cor_method: str = "covariance",
-        cor_method_params: Optional[Dict] = None,
-        mask: Optional[str] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.parcellation = parcellation
         super().__init__(
             agg_method=agg_method,
             agg_method_params=agg_method_params,
-            cor_method=cor_method,
-            cor_method_params=cor_method_params,
-            mask=mask,
+            masks=masks,
             name=name,
         )
 
-    def aggregate(self, input: Dict[str, Any]) -> Dict:
-        """Perform parcel aggregation."""
+    def aggregate(
+        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
+    ) -> Dict:
+        """Perform parcel aggregation.
+
+        Parameters
+        ----------
+        input : dict
+            A single input from the pipeline data object in which the data
+            is the voxelwise temporal SNR map.
+        extra_input : dict, optional
+            The other fields in the pipeline data object. Useful for accessing
+            other data kind that needs to be used in the computation. For
+            example, the functional connectivity markers can make use of the
+            confounds if available (default None).
+
+        Returns
+        -------
+        dict
+            The computed result as dictionary. This will be either returned
+            to the user or stored in the storage by calling the store method
+            with this as a parameter. The dictionary has the following keys:
+
+            * ``data`` : ROI-wise temporal SNR as a ``numpy.ndarray``
+            * ``col_names`` : the ROI labels for the computed values as list
+
+        """
         parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
-            mask=self.mask,
+            masks=self.masks,
             on="BOLD",
         )
-
-        bold_aggregated = parcel_aggregation.compute(input)
-        ets, edge_names = _ets(
-            bold_aggregated["data"], bold_aggregated["columns"]
-        )
-
-        return dict(data=ets, columns=edge_names)
+        # Return the 2D timeseries after parcel aggregation
+        return parcel_aggregation.compute(input=input, extra_input=extra_input)
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-"""Provide class for edge-centric functional connectivity using spheres."""
+"""Provide class for temporal SNR using spheres."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
-#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
 from ..sphere_aggregation import SphereAggregation
-from ..utils import _ets, raise_error
-from .functional_connectivity_base import FunctionalConnectivityBase
+from ..utils import raise_error
+from .temporal_snr_base import TemporalSNRBase
 
 
 @register_marker
-class EdgeCentricFCSpheres(FunctionalConnectivityBase):
-    """Class for edge-centric FC using coordinates (spheres).
+class TemporalSNRSpheres(TemporalSNRBase):
+    """Class for temporal signal-to-noise ratio using coordinates (spheres).
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
-        :func:`junifer.data.coordinates.list_coordinates` for options.
+        :func:`.list_coordinates` for options.
     radius : float, optional
         The radius of the sphere in mm. If None, the signal will be extracted
         from a single voxel. See :class:`nilearn.maskers.NiftiSpheresMasker`
         for more information (default None).
+    allow_overlap : bool, optional
+        Whether to allow overlapping spheres. If False, an error is raised if
+        the spheres overlap (default is False).
     agg_method : str, optional
         The aggregation method to use.
-        See :func:`junifer.stats.get_aggfunc_by_name` for more information
+        See :func:`.get_aggfunc_by_name` for more information
         (default None).
     agg_method_params : dict, optional
         The parameters to pass to the aggregation method (default None).
-    cor_method : str, optional
-        The method to perform correlation using. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure` (default "covariance").
-    cor_method_params : dict, optional
-        Parameters to pass to the correlation function. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure` (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. By default, it will use
-        KIND_EdgeCentricFCSpheres where KIND is the kind of data it
+        KIND_FunctionalConnectivitySpheres where KIND is the kind of data it
         was applied to (default None).
 
-    References
-    ----------
-    .. [1] Jo et al. (2021)
-            Subject identification using
-            edge-centric functional connectivity
-            doi: https://doi.org/10.1016/j.neuroimage.2021.118204
-
     """
 
     def __init__(
         self,
         coords: str,
         radius: Optional[float] = None,
+        allow_overlap: bool = False,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        cor_method: str = "covariance",
-        cor_method_params: Optional[Dict] = None,
-        mask: Optional[str] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.coords = coords
         self.radius = radius
+        self.allow_overlap = allow_overlap
         if radius is None or radius <= 0:
             raise_error(f"radius should be > 0: provided {radius}")
         super().__init__(
             agg_method=agg_method,
             agg_method_params=agg_method_params,
-            cor_method=cor_method,
-            cor_method_params=cor_method_params,
-            mask=mask,
+            masks=masks,
             name=name,
         )
 
-    def aggregate(self, input: Dict[str, Any]) -> Dict:
-        """Perform sphere aggregation."""
+    def aggregate(
+        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
+    ) -> Dict:
+        """Perform sphere aggregation.
+
+        Parameters
+        ----------
+        input : dict
+            A single input from the pipeline data object in which the data
+            is the voxelwise temporal SNR map.
+        extra_input : dict, optional
+            The other fields in the pipeline data object. Useful for accessing
+            other data kind that needs to be used in the computation. For
+            example, the functional connectivity markers can make use of the
+            confounds if available (default None).
+
+        Returns
+        -------
+        dict
+            The computed result as dictionary. This will be either returned
+            to the user or stored in the storage by calling the store method
+            with this as a parameter. The dictionary has the following keys:
+
+            * ``data`` : VOI-wise temporal SNR as a ``numpy.ndarray``
+            * ``col_names`` : the VOI labels for the computed values as list
+
+        """
         sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
+            allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
-            mask=self.mask,
+            masks=self.masks,
             on="BOLD",
         )
-        bold_aggregated = sphere_aggregation.compute(input)
-        ets, edge_names = _ets(
-            bold_aggregated["data"], bold_aggregated["columns"]
-        )
-
-        return dict(data=ets, columns=edge_names)
+        # Return the 2D timeseries after sphere aggregation
+        return sphere_aggregation.compute(input=input, extra_input=extra_input)
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,60 +17,64 @@
 class FunctionalConnectivityBase(BaseMarker):
     """Abstract base class for functional connectivity markers.
 
     Parameters
     ----------
     agg_method : str, optional
         The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default "mean").
+        :func:`.get_aggfunc_by_name` (default "mean").
     agg_method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default None).
+        :func:`.get_aggfunc_by_name` (default None).
     cor_method : str, optional
         The method to perform correlation using. Check valid options in
         :class:`nilearn.connectome.ConnectivityMeasure`
         (default "covariance").
     cor_method_params : dict, optional
         Parameters to pass to the correlation function. Check valid options in
         :class:`nilearn.connectome.ConnectivityMeasure` (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     """
 
     _DEPENDENCIES = {"nilearn", "scikit-learn"}
 
     def __init__(
         self,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         cor_method: str = "covariance",
         cor_method_params: Optional[Dict] = None,
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
         self.cor_method = cor_method
         self.cor_method_params = cor_method_params or {}
 
         # default to nilearn behavior
         self.cor_method_params["empirical"] = self.cor_method_params.get(
             "empirical", False
         )
-        self.mask = mask
+        self.masks = masks
         super().__init__(on="BOLD", name=name)
 
     @abstractmethod
-    def aggregate(self, input: Dict[str, Any]) -> Dict[str, Any]:
+    def aggregate(
+        self,
+        input: Dict[str, Any],
+        extra_input: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
         """Perform aggregation."""
         raise_error(
             msg="Concrete classes need to implement aggregate().",
             klass=NotImplementedError,
         )
 
     def get_valid_inputs(self) -> List[str]:
@@ -126,24 +130,24 @@
             * ``data`` : functional connectivity matrix as a ``numpy.ndarray``.
             * ``row_names`` : row names as a list
             * ``col_names`` : column names as a list
             * ``matrix_kind`` : the kind of matrix (tril, triu or full)
 
         """
         # Perform necessary aggregation
-        aggregation = self.aggregate(input)
+        aggregation = self.aggregate(input, extra_input=extra_input)
         # Compute correlation
         if self.cor_method_params["empirical"]:
             connectivity = ConnectivityMeasure(
-                cov_estimator=EmpiricalCovariance(),
+                cov_estimator=EmpiricalCovariance(),  # type: ignore
                 kind=self.cor_method,
             )
         else:
             connectivity = ConnectivityMeasure(kind=self.cor_method)
         # Create dictionary for output
         out = {}
         out["data"] = connectivity.fit_transform([aggregation["data"]])[0]
         # Create column names
-        out["row_names"] = aggregation["columns"]
-        out["col_names"] = aggregation["columns"]
+        out["row_names"] = aggregation["col_names"]
+        out["col_names"] = aggregation["col_names"]
         out["matrix_kind"] = "tril"
         return out
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/parcel_aggregation.py` & `junifer-0.0.3.dev36/junifer/markers/parcel_aggregation.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
-from nilearn.image import math_img, new_img_like, resample_to_img
+from nilearn.image import math_img, resample_to_img
 from nilearn.maskers import NiftiMasker
 
 from ..api.decorators import register_marker
-from ..data import get_mask, load_parcellation
+from ..data import get_mask, load_parcellation, merge_parcellations
 from ..stats import get_aggfunc_by_name
-from ..utils import logger
+from ..utils import logger, raise_error, warn_with_log
 from .base import BaseMarker
 
 
 @register_marker
 class ParcelAggregation(BaseMarker):
     """Class for parcel aggregation.
 
     Parameters
     ----------
     parcellation : str or list of str
         The name(s) of the parcellation(s). Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     method : str
         The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name`.
+        :func:`.get_aggfunc_by_name`.
     method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name`.
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+        :func:`.get_aggfunc_by_name`.
+    time_method : str, optional
+        The method to use to aggregate the time series over the time points,
+        after applying :term:`method` (only applicable to BOLD data). If None,
+        it will not operate on the time dimension (default None).
+    time_method_params : dict, optional
+        The parameters to pass to the time aggregation method (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     on : {"T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"} \
          or list of the options, optional
         The data types to apply the marker to. If None, will work on all
         available data (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
@@ -48,26 +54,42 @@
     _DEPENDENCIES = {"nilearn", "numpy"}
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         method: str,
         method_params: Optional[Dict[str, Any]] = None,
-        mask: Union[str, Dict, None] = None,
+        time_method: Optional[str] = None,
+        time_method_params: Optional[Dict[str, Any]] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         on: Union[List[str], str, None] = None,
         name: Optional[str] = None,
     ) -> None:
         if not isinstance(parcellation, list):
             parcellation = [parcellation]
         self.parcellation = parcellation
         self.method = method
         self.method_params = method_params or {}
-        self.mask = mask
+        self.masks = masks
         super().__init__(on=on, name=name)
 
+        # Verify after super init so self._on is set
+        if "BOLD" not in self._on and time_method is not None:
+            raise_error(
+                "`time_method` can only be used with BOLD data. "
+                "Please remove `time_method` parameter."
+            )
+        if time_method is None and time_method_params is not None:
+            raise_error(
+                "`time_method_params` can only be used with `time_method`. "
+                "Please remove `time_method_params` parameter."
+            )
+        self.time_method = time_method
+        self.time_method_params = time_method_params or {}
+
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
@@ -87,24 +109,22 @@
         -------
         str
             The storage type output by the marker.
 
         """
 
         if input_type in ["VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]:
-            return "table"
+            return "vector"
         elif input_type == "BOLD":
             return "timeseries"
         else:
             raise ValueError(f"Unknown input kind for {input_type}")
 
     def compute(
-        self,
-        input: Dict[str, Any],
-        extra_input: Optional[Dict] = None,
+        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
     ) -> Dict:
         """Compute.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
@@ -119,78 +139,56 @@
         -------
         dict
             The computed result as dictionary. This will be either returned
             to the user or stored in the storage by calling the store method
             with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
+            * ``col_names`` : the column labels for the computed values as list
 
         """
         t_input_img = input["data"]
         logger.debug(f"Parcel aggregation using {self.method}")
         agg_func = get_aggfunc_by_name(
-            name=self.method,
-            func_params=self.method_params,
+            name=self.method, func_params=self.method_params
         )
         # Get the min of the voxels sizes and use it as the resolution
         resolution = np.min(t_input_img.header.get_zooms()[:3])
 
         # Load the parcellations
         all_parcelations = []
         all_labels = []
         for t_parc_name in self.parcellation:
             t_parcellation, t_labels, _ = load_parcellation(
-                name=t_parc_name,
-                resolution=resolution,
+                name=t_parc_name, resolution=resolution
             )
             # Resample all of them to the image
             t_parcellation_img_res = resample_to_img(
-                t_parcellation,
-                t_input_img,
-                interpolation="nearest",
-                copy=True,
+                t_parcellation, t_input_img, interpolation="nearest", copy=True
             )
             all_parcelations.append(t_parcellation_img_res)
             all_labels.append(t_labels)
 
         # Avoid merging if there is only one parcellation
         if len(all_parcelations) == 1:
             parcellation_img_res = all_parcelations[0]
             labels = all_labels[0]
         else:
             # Merge the parcellations
-            parc_data = all_parcelations[0].get_fdata()
-            labels = all_labels[0]
-            for t_parc, t_labels in zip(all_parcelations[1:], all_labels[1:]):
-                # Get the data from this parcellation
-                t_parc_data = t_parc.get_fdata().copy()  # must be copied
-                # Increase the values of each ROI to match the labels
-                t_parc_data[t_parc_data != 0] += len(labels)
-
-                # Only set new values for the voxels that are 0
-                # This makes sure that the voxels that are in multiple
-                # parcellations are assigned to the parcellation that was
-                # first in the list.
-                parc_data[parc_data == 0] += t_parc_data[parc_data == 0]
-                labels.extend(t_labels)
-
-            parcellation_img_res = new_img_like(
-                all_parcelations[0],
-                parc_data,
-            )
-
-        parcellation_bin = math_img(
-            "img != 0",
-            img=parcellation_img_res,
-        )
+            parcellation_img_res, labels = merge_parcellations(
+                all_parcelations, self.parcellation, all_labels
+            )
 
-        if self.mask is not None:
-            logger.debug(f"Masking with {self.mask}")
-            mask_img = get_mask(mask=self.mask, target_data=input)
+        parcellation_bin = math_img("img != 0", img=parcellation_img_res)
+
+        if self.masks is not None:
+            logger.debug(f"Masking with {self.masks}")
+            mask_img = get_mask(
+                masks=self.masks, target_data=input, extra_input=extra_input
+            )
 
             parcellation_bin = math_img(
                 "np.logical_and(img, mask)",
                 img=parcellation_bin,
                 mask=mask_img,
             )
 
@@ -202,21 +200,31 @@
         # Mask the input data and the parcellation
         data = masker.fit_transform(t_input_img)
         parcellation_values = masker.transform(parcellation_img_res)
         parcellation_values = np.squeeze(parcellation_values).astype(int)
 
         # Get the values for each parcel and apply agg function
         logger.debug("Computing ROI means")
-        parcellation_roi_vals = sorted(np.unique(parcellation_values))
-        out_labels = []
         out_values = []
         # Iterate over the parcels (existing)
-        for t_v in parcellation_roi_vals:
+        for t_v in range(1, len(labels) + 1):
             t_values = agg_func(data[:, parcellation_values == t_v], axis=-1)
             out_values.append(t_values)
             # Update the labels just in case a parcel has no voxels
             # in it
-            out_labels.append(labels[t_v - 1])
 
         out_values = np.array(out_values).T
-        out = {"data": out_values, "columns": out_labels}
+
+        if self.time_method is not None:
+            if out_values.shape[0] > 1:
+                logger.debug("Aggregating time dimension")
+                time_agg_func = get_aggfunc_by_name(
+                    self.time_method, func_params=self.time_method_params
+                )
+                out_values = time_agg_func(out_values, axis=0)
+            else:
+                warn_with_log(
+                    "No time dimension to aggregate as only one time point is "
+                    "available."
+                )
+        out = {"data": out_values, "col_names": labels}
         return out
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/reho_base.py` & `junifer-0.0.3.dev36/junifer/markers/reho/reho_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         Returns
         -------
         str
             The storage type output by the marker.
 
         """
-        return "table"
+        return "vector"
 
     def compute_reho_map(
         self,
         input: Dict[str, Any],
         **reho_params: Any,
     ) -> "Nifti1Image":
         """Compute.
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.3.dev36/junifer/markers/reho/reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/reho/reho_parcels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide class for regional homogeneity (ReHo) on parcels."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 
 from ...api.decorators import register_marker
 from ...utils import logger
 from ..parcel_aggregation import ParcelAggregation
 from .reho_base import ReHoBase
@@ -18,15 +18,15 @@
 class ReHoParcels(ReHoBase):
     """Class for regional homogeneity on parcels.
 
     Parameters
     ----------
     parcellation : str
         The name of the parcellation. Check valid options by calling
-        :func:`junifer.data.parcellations.list_parcellations`.
+        :func:`.list_parcellations`.
     use_afni : bool, optional
         Whether to use AFNI for computing. If None, will use AFNI only
         if available (default None).
     reho_params : dict, optional
         Extra parameters for computing ReHo map as a dictionary (default None).
         If ``use_afni = True``, then the valid keys are:
 
@@ -66,43 +66,43 @@
             * 7 : for facewise neighbours only
             * 19 : for face- and edge-wise nieghbours
             * 27 : for face-, edge-, and node-wise neighbors
             * 125 : for 5x5 cuboidal volume
 
     agg_method : str, optional
         The method to perform aggregation using. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default "mean").
+        :func:`.get_aggfunc_by_name` (default "mean").
     agg_method_params : dict, optional
         Parameters to pass to the aggregation function. Check valid options in
-        :func:`junifer.stats.get_aggfunc_by_name` (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+        :func:`.get_aggfunc_by_name` (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, it will use the class name
         (default None).
 
     """
 
     def __init__(
         self,
         parcellation: str,
         use_afni: Optional[bool] = None,
         reho_params: Optional[Dict] = None,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.parcellation = parcellation
         self.reho_params = reho_params
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
-        self.mask = mask
+        self.masks = masks
         super().__init__(use_afni=use_afni, name=name)
 
     def compute(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
@@ -118,31 +118,36 @@
         Returns
         -------
         dict
             The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a 1D numpy.ndarray
-            * ``columns`` : the column labels for the parcels as a list
-            * ``row_names`` : ``None``
+            * ``col_names`` : the column labels for the parcels as a list
 
         """
         logger.info("Calculating ReHo for parcels.")
         # Calculate reho map
         if self.reho_params is not None:
             reho_map = self.compute_reho_map(input=input, **self.reho_params)
         else:
             reho_map = self.compute_reho_map(input=input)
         # Initialize parcel aggregation
         parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
-            mask=self.mask,
+            masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
-        parcel_aggregation_input = {"data": reho_map}
-        output = parcel_aggregation.compute(input=parcel_aggregation_input)
+        parcel_aggregation_input = {k: v for k, v in input.items()}
+        parcel_aggregation_input["data"] = reho_map
+        parcel_aggregation_input["path"] = None
+
+        output = parcel_aggregation.compute(
+            input=parcel_aggregation_input,
+            extra_input=extra_input,
+        )
         # Only use the first row and expand row dimension
         output["data"] = output["data"][0][np.newaxis, :]
         return output
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/reho/reho_spheres.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide class for regional homogeneity (ReHo) on spheres."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 
 from ...api.decorators import register_marker
 from ...utils import logger
 from ..sphere_aggregation import SphereAggregation
 from .reho_base import ReHoBase
@@ -18,20 +18,23 @@
 class ReHoSpheres(ReHoBase):
     """Class for regional homogeneity on spheres.
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
-        :func:`junifer.data.coordinates.list_coordinates` for options.
+        :func:`.list_coordinates` for options.
     radius : float, optional
         The radius of the sphere in millimeters. If None, the signal will be
         extracted from a single voxel. See
         :class:`nilearn.maskers.NiftiSpheresMasker` for more information
         (default None).
+    allow_overlap : bool, optional
+        Whether to allow overlapping spheres. If False, an error is raised if
+        the spheres overlap (default is False).
     use_afni : bool, optional
         Whether to use AFNI for computing. If None, will use AFNI only
         if available (default None).
     reho_params : dict, optional
         Extra parameters for computing ReHo map as a dictionary (default None).
         If ``use_afni = True``, then the valid keys are:
 
@@ -71,45 +74,47 @@
             * 7 : for facewise neighbours only
             * 19 : for face- and edge-wise nieghbours
             * 27 : for face-, edge-, and node-wise neighbors
             * 125 : for 5x5 cuboidal volume
 
     agg_method : str, optional
         The aggregation method to use.
-        See :func:`junifer.stats.get_aggfunc_by_name` for more information
+        See :func:`.get_aggfunc_by_name` for more information
         (default None).
     agg_method_params : dict, optional
         The parameters to pass to the aggregation method (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, it will use the class name
         (default None).
 
     """
 
     def __init__(
         self,
         coords: str,
         radius: Optional[float] = None,
+        allow_overlap: bool = False,
         use_afni: Optional[bool] = None,
         reho_params: Optional[Dict] = None,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        mask: Union[str, Dict, None] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
         self.coords = coords
         self.radius = radius
+        self.allow_overlap = allow_overlap
         self.reho_params = reho_params
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
-        self.mask = mask
+        self.masks = masks
         super().__init__(use_afni=use_afni, name=name)
 
     def compute(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
@@ -125,32 +130,36 @@
         Returns
         -------
         dict
             The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a 1D numpy.ndarray
-            * ``columns`` : the column labels for the spheres as a list
-            * ``rows_col_name`` : ``None``
+            * ``col_names`` : the column labels for the spheres as a list
 
         """
         logger.info("Calculating ReHo for spheres.")
         # Calculate reho map
         if self.reho_params is not None:
             reho_map = self.compute_reho_map(input=input, **self.reho_params)
         else:
             reho_map = self.compute_reho_map(input=input)
         # Initialize sphere aggregation
         sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
+            allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
-            mask=self.mask,
+            masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
-        sphere_aggregation_input = {"data": reho_map}
-        output = sphere_aggregation.compute(input=sphere_aggregation_input)
+        sphere_aggregation_input = {k: v for k, v in input.items()}
+        sphere_aggregation_input["data"] = reho_map
+        sphere_aggregation_input["path"] = None
+        output = sphere_aggregation.compute(
+            input=sphere_aggregation_input, extra_input=extra_input
+        )
         # Only use the first row and expand row dimension
         output["data"] = output["data"][0][np.newaxis, :]
         return output
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         reho_parcels_output = reho_parcels_marker.fit_transform(
             {"BOLD": {"path": "/tmp", "data": fmri_img, "meta": {}}}
         )
         # Get BOLD output
         reho_parcels_output_bold = reho_parcels_output["BOLD"]
         # Assert BOLD output keys
         assert "data" in reho_parcels_output_bold
-        assert "columns" in reho_parcels_output_bold
+        assert "col_names" in reho_parcels_output_bold
 
         reho_parcels_output_bold_data = reho_parcels_output_bold["data"]
         # Assert BOLD output data dimension
         assert reho_parcels_output_bold_data.ndim == 2
         # Assert BOLD output data is normalized
         assert (reho_parcels_output_bold_data > 0).all() and (
             reho_parcels_output_bold_data < 1
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.3.dev36/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         reho_spheres_output = reho_spheres_marker.fit_transform(
             {"BOLD": {"path": "/tmp", "data": fmri_img, "meta": {}}}
         )
         # Get BOLD output
         reho_spheres_output_bold = reho_spheres_output["BOLD"]
         # Assert BOLD output keys
         assert "data" in reho_spheres_output_bold
-        assert "columns" in reho_spheres_output_bold
+        assert "col_names" in reho_spheres_output_bold
 
         reho_spheres_output_bold_data = reho_spheres_output_bold["data"]
         # Assert BOLD output data dimension
         assert reho_spheres_output_bold_data.ndim == 2
         # Assert BOLD output data is normalized
         assert (reho_spheres_output_bold_data > 0).all() and (
             reho_spheres_output_bold_data < 1
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/sphere_aggregation.py` & `junifer-0.0.3.dev36/junifer/markers/falff/falff_spheres.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,111 @@
-"""Provide class for sphere aggregation."""
+"""Provide class for computing fALFF on spheres."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
-#          Synchon Mandal <s.mandal@fz-juelich.de>
+#          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
+#          Kaustubh R. Patil <k.patil@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
-from ..api.decorators import register_marker
-from ..data import load_coordinates, get_mask
-from ..external.nilearn import JuniferNiftiSpheresMasker
-from ..stats import get_aggfunc_by_name
-from ..utils import logger
-from .base import BaseMarker
+from ...api.decorators import register_marker
+from .. import SphereAggregation
+from .falff_base import ALFFBase
 
 
 @register_marker
-class SphereAggregation(BaseMarker):
-    """Class for sphere aggregation.
+class ALFFSpheres(ALFFBase):
+    """Class for computing fALFF/ALFF on spheres.
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
-        :func:`junifer.data.coordinates.list_coordinates` for options.
+        :func:`.list_coordinates` for options.
     radius : float, optional
-        The radius of the sphere in millimeters. If None, the signal will be
-        extracted from a single voxel. See
-        :class:`nilearn.maskers.NiftiSpheresMasker` for more information
-        (default None).
+        The radius of the sphere in mm. If None, the signal will be extracted
+        from a single voxel. See :class:`nilearn.maskers.NiftiSpheresMasker`
+        for more information (default None).
+    allow_overlap : bool, optional
+        Whether to allow overlapping spheres. If False, an error is raised if
+        the spheres overlap (default is False).
+    fractional : bool
+        Whether to compute fractional ALFF.
+    highpass : positive float, optional
+        The highpass cutoff frequency for the bandpass filter. If 0,
+        it will not apply a highpass filter (default 0.01).
+    lowpass : positive float, optional
+        The lowpass cutoff frequency for the bandpass filter (default 0.1).
+    tr : positive float, optional
+        The Repetition Time of the BOLD data. If None, will extract
+        the TR from NIFTI header (default None).
+    use_afni : bool, optional
+        Whether to use AFNI for computing. If None, will use AFNI only
+        if available (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
     method : str, optional
-        The aggregation method to use.
-        See :func:`junifer.stats.get_aggfunc_by_name` for more information
-        (default "mean").
+        The method to perform aggregation using. Check valid options in
+        :func:`.get_aggfunc_by_name` (default "mean").
     method_params : dict, optional
-        The parameters to pass to the aggregation method (default None).
-    mask : str, optional
-        The name of the mask to apply to regions before extracting signals.
-        Check valid options by calling :func:`junifer.data.masks.list_masks`
-        (default None).
-    on : {"T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"} or \
-         list of the options, optional
-        The data types to apply the marker to. If None, will work on all
-        available data (default None).
+        Parameters to pass to the aggregation function. Check valid options in
+        :func:`.get_aggfunc_by_name`.
     name : str, optional
-        The name of the marker. By default, it will use KIND_SphereAggregation
-        where KIND is the kind of data it was applied to (default None).
+        The name of the marker. If None, will use the class name (default
+        None).
 
+    Notes
+    -----
+    The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
+    computation. If a dataset is correctly preprocessed, the TR should be
+    extracted from the NIFTI without any issue. However, it has been
+    reported that some preprocessed data might not have the correct TR in
+    the NIFTI header.
+
+    ALFF/fALFF are computed using a bandpass butterworth filter. See
+    :func:`scipy.signal.butter` and :func:`scipy.signal.filtfilt` for more
+    details.
     """
 
-    _DEPENDENCIES = {"nilearn", "numpy"}
-
     def __init__(
         self,
         coords: str,
+        fractional: bool,
         radius: Optional[float] = None,
+        allow_overlap: bool = False,
+        highpass: float = 0.01,
+        lowpass: float = 0.1,
+        tr: Optional[float] = None,
+        use_afni: Optional[bool] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         method: str = "mean",
-        method_params: Optional[Dict[str, Any]] = None,
-        mask: Union[str, Dict, None] = None,
-        on: Union[List[str], str, None] = None,
+        method_params: Optional[Dict] = None,
         name: Optional[str] = None,
     ) -> None:
         self.coords = coords
         self.radius = radius
+        self.allow_overlap = allow_overlap
+        self.masks = masks
         self.method = method
-        self.method_params = method_params or {}
-        self.mask = mask
-        super().__init__(on=on, name=name)
-
-    def get_valid_inputs(self) -> List[str]:
-        """Get valid data types for input.
-
-        Returns
-        -------
-        list of str
-            The list of data types that can be used as input for this marker.
-
-        """
-        return ["T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]
-
-    def get_output_type(self, input_type: str) -> str:
-        """Get output type.
-
-        Parameters
-        ----------
-        input_type : str
-            The data type input to the marker.
-
-        Returns
-        -------
-        str
-            The storage type output by the marker.
-
-        """
-
-        if input_type in ["VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]:
-            return "table"
-        elif input_type == "BOLD":
-            return "timeseries"
-        else:
-            raise ValueError(f"Unknown input kind for {input_type}")
+        self.method_params = method_params
+        super().__init__(
+            fractional=fractional,
+            highpass=highpass,
+            lowpass=lowpass,
+            tr=tr,
+            name=name,
+            use_afni=use_afni,
+        )
 
-    def compute(
-        self,
-        input: Dict[str, Any],
-        extra_input: Optional[Dict] = None,
+    def _postprocess(
+        self, input: Dict, extra_input: Optional[Dict] = None
     ) -> Dict:
-        """Compute.
+        """Compute ALFF and fALFF.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
             the marker.
         extra_input : dict, optional
@@ -117,39 +113,28 @@
             other data kind that needs to be used in the computation. For
             example, the functional connectivity markers can make use of the
             confounds if available (default None).
 
         Returns
         -------
         dict
-            The computed result as dictionary. This will be either returned
-            to the user or stored in the storage by calling the store method
-            with this as a parameter. The dictionary has the following keys:
+            The computed ALFF as dictionary. The dictionary has the following
+            keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
-            * ``columns`` : the column labels for the computed values as a list
+            * ``col_names`` : the column labels for the computed values as list
 
         """
-        t_input_img = input["data"]
-        logger.debug(f"Sphere aggregation using {self.method}")
-        # Get aggregation function
-        agg_func = get_aggfunc_by_name(
-            self.method, func_params=self.method_params
-        )
-        # Load mask
-        mask_img = None
-        if self.mask is not None:
-            logger.debug(f"Masking with {self.mask}")
-            mask_img = get_mask(mask=self.mask, target_data=input)
-        # Get seeds and labels
-        coords, out_labels = load_coordinates(name=self.coords)
-        masker = JuniferNiftiSpheresMasker(
-            seeds=coords,
+        pa = SphereAggregation(
+            coords=self.coords,
             radius=self.radius,
-            mask_img=mask_img,
-            agg_func=agg_func,
+            allow_overlap=self.allow_overlap,
+            method=self.method,
+            method_params=self.method_params,
+            masks=self.masks,
+            on="fALFF",
         )
-        # Fit and transform the marker on the data
-        out_values = masker.fit_transform(t_input_img)
-        # Format the output
-        out = {"data": out_values, "columns": out_labels}
+
+        # get the 2D timeseries after sphere aggregation
+        out = pa.compute(input, extra_input=extra_input)
+
         return out
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_collection.py` & `junifer-0.0.3.dev36/junifer/markers/tests/test_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         ParcelAggregation(
             parcellation="Schaefer100x7",
             method="mean",
             name="gmd_schaefer100x7_mean",
         ),
     ]
     with pytest.raises(ValueError, match=r"must have different names"):
-        MarkerCollection(wrong_markers)
+        MarkerCollection(wrong_markers)  # type: ignore
 
 
 def test_marker_collection() -> None:
     """Test MarkerCollection."""
     markers = [
         ParcelAggregation(
             parcellation="Schaefer100x7",
@@ -58,15 +58,15 @@
         ParcelAggregation(
             parcellation="Schaefer100x7",
             method="trim_mean",
             method_params={"proportiontocut": 0.1},
             name="gmd_schaefer100x7_trim_mean90",
         ),
     ]
-    mc = MarkerCollection(markers=markers)
+    mc = MarkerCollection(markers=markers)  # type: ignore
     assert mc._markers == markers
     assert mc._preprocessing is None
     assert mc._storage is None
     assert isinstance(mc._datareader, DefaultDataReader)
 
     # Create testing datagrabber
     dg = OasisVBMTestingDatagrabber()
@@ -83,24 +83,24 @@
         assert "gmd_schaefer100x7_trim_mean90" in out
 
         for t_marker in markers:
             t_name = t_marker.name
             assert "VBM_GM" in out[t_name]
             t_vbm = out[t_name]["VBM_GM"]
             assert "data" in t_vbm
-            assert "columns" in t_vbm
+            assert "col_names" in t_vbm
             assert "meta" in t_vbm
 
     # Test preprocessing
     class BypassPreprocessing(PipelineStepMixin):
         def fit_transform(self, input):
             return input
 
     mc2 = MarkerCollection(
-        markers=markers,
+        markers=markers,  # type: ignore
         preprocessing=BypassPreprocessing(),
         datareader=DefaultDataReader(),
     )
     assert isinstance(mc2._datareader, DefaultDataReader)
     with dg:
         input = dg["sub-01"]
         out2 = mc2.fit(input)
@@ -123,15 +123,15 @@
         FunctionalConnectivityParcels(
             parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             agg_method="mean",
             name="TianxS2x3TxMNInonlinear2009cAsym_mean_FC",
         ),
     ]
     mc = MarkerCollection(
-        markers=markers,
+        markers=markers,  # type: ignore
         preprocessing=fMRIPrepConfoundRemover(),
     )
     assert mc._markers == markers
     assert mc._preprocessing is not None
     assert mc._storage is None
     assert isinstance(mc._datareader, DefaultDataReader)
 
@@ -169,49 +169,51 @@
     ]
     # Test storage
     dg = OasisVBMTestingDatagrabber()
 
     uri = tmp_path / "test_marker_collection_storage.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     mc = MarkerCollection(
-        markers=markers,
+        markers=markers,  # type: ignore
         storage=storage,
         datareader=DefaultDataReader(),
     )
     mc.validate(dg)
     assert mc._storage is not None
     assert mc._storage.uri == storage.uri
     with dg:
         input = dg["sub-01"]
         out = mc.fit(input)
         assert out is None
 
-    mc2 = MarkerCollection(markers=markers, datareader=DefaultDataReader())
+    mc2 = MarkerCollection(
+        markers=markers, datareader=DefaultDataReader()  # type: ignore
+    )
     mc2.validate(dg)
     assert mc2._storage is None
 
     with dg:
         input = dg["sub-01"]
         out = mc2.fit(input)
 
     features = storage.list_features()
     assert len(features) == 3
     feature_md5 = list(features.keys())[0]
     t_feature = storage.read_df(feature_md5=feature_md5)
     fname = "gmd_schaefer100x7_mean"
     t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["columns"]  # type: ignore
+    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
 
     feature_md5 = list(features.keys())[1]
     t_feature = storage.read_df(feature_md5=feature_md5)
     fname = "gmd_schaefer100x7_std"
     t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["columns"]  # type: ignore
+    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
 
     feature_md5 = list(features.keys())[2]
     t_feature = storage.read_df(feature_md5=feature_md5)
     fname = "gmd_schaefer100x7_trim_mean90"
     t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["columns"]  # type: ignore
+    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.3.dev36/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.3.dev36/junifer/markers/tests/test_marker_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,22 @@
         ]
     ).T
 
     n_time, n_rois = bold_ts.shape
     n_edges = int(n_rois * (n_rois - 1) / 2)
 
     # test without labels
-    edge_ts = _ets(bold_ts)
+    edge_ts, _ = _ets(bold_ts)
     assert edge_ts.shape == (n_time, n_edges)
 
     # test with labels
     roi_labels = [f"Label_{x}" for x in range(n_rois)]
     edge_ts, edge_labels = _ets(bold_ts, roi_labels)
     assert edge_ts.shape == (n_time, n_edges)
+    assert edge_labels is not None
     assert len(edge_labels) == n_edges
 
 
 def test_ets_incorrect_label_list() -> None:
     """Test edge-wise timeseries computing function with incorrect labels."""
     bold_ts = np.arange(30).reshape(10, 3)
     # one label is missing, the bold time series suggests three ROIs
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.3.dev36/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,86 @@
-"""Provide tests for base marker."""
+"""Provide tests for BasePreprocessor."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import pytest
 
-from junifer.markers.base import BaseMarker
+from junifer.preprocess.base import BasePreprocessor
 
 
-def test_base_marker_abstractness() -> None:
-    """Test BaseMarker is abstract base class."""
+def test_base_preprocessor_abstractness() -> None:
+    """Test BasePreprocessor is abstract base class."""
     with pytest.raises(TypeError, match=r"abstract"):
-        BaseMarker(on=["BOLD"])  # type: ignore
+        BasePreprocessor(on=["BOLD"])  # type: ignore
 
 
-def test_base_marker_subclassing() -> None:
-    """Test proper subclassing of BaseMarker."""
+def test_base_preprocessor_subclassing() -> None:
+    """Test proper subclassing of BasePreprocessor."""
+
     # Create concrete class
-    class MyBaseMarker(BaseMarker):
-        def __init__(self, on, name=None) -> None:
+    class MyBasePreprocessor(BasePreprocessor):
+        def __init__(self, on):
             self.parameter = 1
-            super().__init__(on, name)
+            super().__init__(on=on)
 
         def get_valid_inputs(self):
             return ["BOLD", "T1w"]
 
         def get_output_type(self, input):
             return ["timeseries"]
 
-        def compute(self, input, extra_input):
-            return {
-                "data": "data",
-                "columns": "columns",
-                "row_names": "row_names",
-            }
+        def preprocess(self, input, extra_input):
+            input["data"] = f"mofidied_{input['data']}"
+            return "BOLD", input
+
+    with pytest.raises(ValueError, match=r"cannot be computed on \['T2w'\]"):
+        MyBasePreprocessor(on=["BOLD", "T2w"])
 
     with pytest.raises(ValueError, match=r"cannot be computed on \['T2w'\]"):
-        MyBaseMarker(on=["BOLD", "T2w"])
+        MyBasePreprocessor(on="T2w")
 
     # Create input for marker
     input_ = {
         "BOLD": {
             "path": ".",
             "data": "data",
             "meta": {
                 "datagrabber": "dg",
                 "element": "elem",
                 "datareader": "dr",
             },
         },
+        "T1w": {
+            "path": ".",
+            "data": "data",
+            "meta": {
+                "datagrabber": "dg",
+                "element": "elem",
+                "datareader": "dr",
+            },
+        },
     }
-    marker = MyBaseMarker(on=["BOLD"])
+    prep = MyBasePreprocessor(on=["BOLD"])
 
     with pytest.raises(ValueError, match="not have the required data"):
-        marker.validate_input(["T1w"])
+        prep.validate_input(["T1w"])
 
-    output = marker.fit_transform(input=input_)  # process
+    output = prep.fit_transform(input=input_)  # process
     # Check output
     assert "BOLD" in output
     assert "data" in output["BOLD"]
-    assert "columns" in output["BOLD"]
-    assert "row_names" in output["BOLD"]
-
+    assert output["BOLD"]["data"] == "mofidied_data"
+    assert "path" in output["BOLD"]
     assert "meta" in output["BOLD"]
-    meta = output["BOLD"]["meta"]
-    assert "datagrabber" in meta
-    assert "element" in meta
-    assert "datareader" in meta
-    assert "marker" in meta
-    assert "name" in meta["marker"]
-    assert "parameter" in meta["marker"]
-    assert meta["marker"]["parameter"] == 1
 
-    # Check attributes
-    assert marker.name == "MyBaseMarker"
+    meta = output["BOLD"]["meta"]
+    assert "preprocess" in meta
+    assert "class" in meta["preprocess"]
+    assert "MyBasePreprocessor" == meta["preprocess"]["class"]
+    assert "parameter" in meta["preprocess"]
+    assert 1 == meta["preprocess"]["parameter"]
+
+    assert "T1w" in output
+    assert "data" in output["T1w"]
+    assert output["T1w"]["data"] == "data"
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.3.dev36/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Provide test for parcel aggregation."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
+import warnings
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 import pytest
 from nilearn import datasets
 from nilearn.image import concat_imgs, math_img, new_img_like, resample_to_img
@@ -22,15 +23,15 @@
 
 
 def test_ParcelAggregation_input_output() -> None:
     """Test ParcelAggregation input and output types."""
     marker = ParcelAggregation(
         parcellation="Schaefer100x7", method="mean", on="VBM_GM"
     )
-    for in_, out_ in [("VBM_GM", "table"), ("BOLD", "timeseries")]:
+    for in_, out_ in [("VBM_GM", "vector"), ("BOLD", "timeseries")]:
         assert marker.get_output_type(in_) == out_
 
     with pytest.raises(ValueError, match="Unknown input"):
         marker.get_output_type("unknown")
 
 
 def test_ParcelAggregation_3D() -> None:
@@ -225,15 +226,15 @@
     )
     auto = nifti_masker.fit_transform(img)
 
     # Use the ParcelAggregation object
     marker = ParcelAggregation(
         parcellation="Schaefer100x7",
         method="mean",
-        mask="GM_prob0.2",
+        masks="GM_prob0.2",
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
     )  # Test passing "on" as a keyword argument
     input = {"VBM_GM": {"data": img, "meta": {}}}
     jun_values3d_mean = marker.fit_transform(input)["VBM_GM"]["data"]
 
     assert jun_values3d_mean.ndim == 2
@@ -270,15 +271,15 @@
     )
     auto_bad = nifti_masker.fit_transform(img)
 
     # Use the ParcelAggregation object
     marker = ParcelAggregation(
         parcellation="Schaefer100x7",
         method="mean",
-        mask={"compute_brain_mask": {"threshold": 0.2}},
+        masks={"compute_brain_mask": {"threshold": 0.2}},
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
     )  # Test passing "on" as a keyword argument
     input = {"VBM_GM": {"data": img, "meta": {}}}
     jun_values3d_mean = marker.fit_transform(input)["VBM_GM"]["data"]
 
     assert jun_values3d_mean.ndim == 2
@@ -324,16 +325,20 @@
 
     parcellation1_path = tmp_path / "parcellation1.nii.gz"
     parcellation2_path = tmp_path / "parcellation2.nii.gz"
 
     nib.save(parcellation1_img, parcellation1_path)
     nib.save(parcellation2_img, parcellation2_path)
 
-    register_parcellation("Schaefer100x7_low", parcellation1_path, labels1)
-    register_parcellation("Schaefer100x7_high", parcellation2_path, labels2)
+    register_parcellation(
+        "Schaefer100x7_low", parcellation1_path, labels1, overwrite=True
+    )
+    register_parcellation(
+        "Schaefer100x7_high", parcellation2_path, labels2, overwrite=True
+    )
 
     # Use the ParcelAggregation object on the original parcellation
     marker_original = ParcelAggregation(
         parcellation="Schaefer100x7",
         method="mean",
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
@@ -351,24 +356,28 @@
     marker_split = ParcelAggregation(
         parcellation=["Schaefer100x7_low", "Schaefer100x7_high"],
         method="mean",
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
     )  # Test passing "on" as a keyword argument
     input = {"VBM_GM": {"data": img, "meta": {}}}
-    split_mean = marker_split.fit_transform(input)["VBM_GM"]
+
+    # No warnings should be raised
+    with warnings.catch_warnings():
+        warnings.simplefilter("error", category=UserWarning)
+        split_mean = marker_split.fit_transform(input)["VBM_GM"]
     split_mean_data = split_mean["data"]
 
     assert split_mean_data.ndim == 2
     assert split_mean_data.shape[0] == 1
     assert split_mean_data.shape[1] == 100
 
     # Data and labels should be the same
     assert_array_equal(orig_mean_data, split_mean_data)
-    assert orig_mean["columns"] == split_mean["columns"]
+    assert orig_mean["col_names"] == split_mean["col_names"]
 
 
 def test_ParcelAggregation_3D_multiple_overlapping(tmp_path: Path) -> None:
     """Test ParcelAggregation with multiple overlapping parcellations.
 
     Parameters
     ----------
@@ -404,16 +413,20 @@
 
     parcellation1_path = tmp_path / "parcellation1.nii.gz"
     parcellation2_path = tmp_path / "parcellation2.nii.gz"
 
     nib.save(parcellation1_img, parcellation1_path)
     nib.save(parcellation2_img, parcellation2_path)
 
-    register_parcellation("Schaefer100x7_low2", parcellation1_path, labels1)
-    register_parcellation("Schaefer100x7_high2", parcellation2_path, labels2)
+    register_parcellation(
+        "Schaefer100x7_low2", parcellation1_path, labels1, overwrite=True
+    )
+    register_parcellation(
+        "Schaefer100x7_high2", parcellation2_path, labels2, overwrite=True
+    )
 
     # Use the ParcelAggregation object on the original parcellation
     marker_original = ParcelAggregation(
         parcellation="Schaefer100x7",
         method="mean",
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
@@ -431,20 +444,181 @@
     marker_split = ParcelAggregation(
         parcellation=["Schaefer100x7_low2", "Schaefer100x7_high2"],
         method="mean",
         name="gmd_schaefer100x7_mean",
         on="VBM_GM",
     )  # Test passing "on" as a keyword argument
     input = {"VBM_GM": {"data": img, "meta": {}}}
-    split_mean = marker_split.fit_transform(input)["VBM_GM"]
+    with pytest.warns(RuntimeWarning, match="overlapping voxels"):
+        split_mean = marker_split.fit_transform(input)["VBM_GM"]
+    split_mean_data = split_mean["data"]
+
+    assert split_mean_data.ndim == 2
+    assert split_mean_data.shape[0] == 1
+    assert split_mean_data.shape[1] == 105
+
+    # Overlapping voxels should be NaN
+    assert np.isnan(split_mean_data[:, 50:55]).all()
+
+    non_nan = split_mean_data[~np.isnan(split_mean_data)]
+    # Data should be the same
+    assert_array_equal(orig_mean_data, non_nan[None, :])
+
+    # Labels should be "low" for the first 50 and "high" for the second 50
+    assert all(x.startswith("low") for x in split_mean["col_names"][:50])
+    assert all(x.startswith("high") for x in split_mean["col_names"][50:])
+
+
+def test_ParcelAggregation_3D_multiple_duplicated_labels(
+    tmp_path: Path,
+) -> None:
+    """Test ParcelAggregation with two parcellations with duplicated labels.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+
+    # Get the testing parcellation
+    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+
+    assert parcellation is not None
+
+    # Get the oasis VBM data
+    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
+    vbm = oasis_dataset.gray_matter_maps[0]
+    img = nib.load(vbm)
+
+    # Create two parcellations from it
+    parcellation_data = parcellation.get_fdata()
+    parcellation1_data = parcellation_data.copy()
+    parcellation1_data[parcellation1_data > 50] = 0
+    parcellation2_data = parcellation_data.copy()
+    parcellation2_data[parcellation2_data <= 50] = 0
+    parcellation2_data[parcellation2_data > 0] -= 50
+    labels1 = labels[:50]
+    labels2 = labels[49:-1]  # One label is duplicated
+
+    parcellation1_img = new_img_like(parcellation, parcellation1_data)
+    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+
+    parcellation1_path = tmp_path / "parcellation1.nii.gz"
+    parcellation2_path = tmp_path / "parcellation2.nii.gz"
+
+    nib.save(parcellation1_img, parcellation1_path)
+    nib.save(parcellation2_img, parcellation2_path)
+
+    register_parcellation(
+        "Schaefer100x7_low", parcellation1_path, labels1, overwrite=True
+    )
+    register_parcellation(
+        "Schaefer100x7_high", parcellation2_path, labels2, overwrite=True
+    )
+
+    # Use the ParcelAggregation object on the original parcellation
+    marker_original = ParcelAggregation(
+        parcellation="Schaefer100x7",
+        method="mean",
+        name="gmd_schaefer100x7_mean",
+        on="VBM_GM",
+    )  # Test passing "on" as a keyword argument
+    input = {"VBM_GM": {"data": img, "meta": {}}}
+    orig_mean = marker_original.fit_transform(input)["VBM_GM"]
+
+    orig_mean_data = orig_mean["data"]
+    assert orig_mean_data.ndim == 2
+    assert orig_mean_data.shape[0] == 1
+    assert orig_mean_data.shape[1] == 100
+    # assert_array_almost_equal(auto, jun_values3d_mean)
+
+    # Use the ParcelAggregation object on the two parcellations
+    marker_split = ParcelAggregation(
+        parcellation=["Schaefer100x7_low", "Schaefer100x7_high"],
+        method="mean",
+        name="gmd_schaefer100x7_mean",
+        on="VBM_GM",
+    )  # Test passing "on" as a keyword argument
+    input = {"VBM_GM": {"data": img, "meta": {}}}
+
+    with pytest.warns(RuntimeWarning, match="duplicated labels."):
+        split_mean = marker_split.fit_transform(input)["VBM_GM"]
     split_mean_data = split_mean["data"]
 
     assert split_mean_data.ndim == 2
     assert split_mean_data.shape[0] == 1
     assert split_mean_data.shape[1] == 100
 
     # Data should be the same
     assert_array_equal(orig_mean_data, split_mean_data)
 
-    # Labels should be "low" for the first 50 and "high" for the second 50
-    assert all(x.startswith("low") for x in split_mean["columns"][:50])
-    assert all(x.startswith("high") for x in split_mean["columns"][50:])
+    # Labels should be prefixed with the parcellation name
+    col_names = [f"Schaefer100x7_low_{x}" for x in labels1]
+    col_names += [f"Schaefer100x7_high_{x}" for x in labels2]
+    assert col_names == split_mean["col_names"]
+
+
+def test_ParcelAggregation_4D_agg_time():
+    """Test ParcelAggregation object on 4D images, aggregating time."""
+    # Get the testing parcellation (for nilearn)
+    parcellation = datasets.fetch_atlas_schaefer_2018(
+        n_rois=100, yeo_networks=7, resolution_mm=2
+    )
+
+    # Get the SPM auditory data:
+    subject_data = datasets.fetch_spm_auditory()
+    fmri_img = concat_imgs(subject_data.func)  # type: ignore
+
+    # Create NiftiLabelsMasker
+    nifti_masker = NiftiLabelsMasker(labels_img=parcellation.maps)
+    auto4d = nifti_masker.fit_transform(fmri_img)
+    auto_mean = auto4d.mean(axis=0)
+
+    # Create ParcelAggregation object
+    marker = ParcelAggregation(
+        parcellation="Schaefer100x7", method="mean", time_method="mean"
+    )
+    input = {"BOLD": {"data": fmri_img, "meta": {}}}
+    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
+
+    assert jun_values4d.ndim == 1
+    assert_array_equal(auto_mean.shape, jun_values4d.shape)
+    assert_array_almost_equal(auto_mean, jun_values4d, decimal=2)
+
+    auto_pick_0 = auto4d[:1, :]
+    marker = ParcelAggregation(
+        parcellation="Schaefer100x7",
+        method="mean",
+        time_method="select",
+        time_method_params={"pick": [0]},
+    )
+
+    input = {"BOLD": {"data": fmri_img, "meta": {}}}
+    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
+
+    assert jun_values4d.ndim == 2
+    assert_array_equal(auto_pick_0.shape, jun_values4d.shape)
+    assert_array_equal(auto_pick_0, jun_values4d)
+
+    with pytest.raises(ValueError, match="can only be used with BOLD data"):
+        ParcelAggregation(
+            parcellation="Schaefer100x7",
+            method="mean",
+            time_method="select",
+            time_method_params={"pick": [0]},
+            on="VBM_GM",
+        )
+
+    with pytest.raises(
+        ValueError, match="can only be used with `time_method`"
+    ):
+        ParcelAggregation(
+            parcellation="Schaefer100x7",
+            method="mean",
+            time_method_params={"pick": [0]},
+            on="VBM_GM",
+        )
+
+    with pytest.warns(RuntimeWarning, match="No time dimension to aggregate"):
+        input = {"BOLD": {"data": fmri_img.slicer[..., 0:1], "meta": {}}}
+        marker.fit_transform(input)
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.3.dev36/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 COORDS = "DMNBuckner"
 RADIUS = 8
 
 
 def test_SphereAggregation_input_output() -> None:
     """Test SphereAggregation input and output types."""
     marker = SphereAggregation(coords="DMNBuckner", method="mean", on="VBM_GM")
-    for in_, out_ in [("VBM_GM", "table"), ("BOLD", "timeseries")]:
+    for in_, out_ in [("VBM_GM", "vector"), ("BOLD", "timeseries")]:
         assert marker.get_output_type(in_) == out_
 
     with pytest.raises(ValueError, match="Unknown input"):
         marker.get_output_type("unknown")
 
 
 def test_SphereAggregation_3D() -> None:
@@ -155,15 +155,82 @@
 
     # Create SphereAggregation object
     marker = SphereAggregation(
         coords=COORDS,
         method="mean",
         radius=RADIUS,
         on="VBM_GM",
-        mask="GM_prob0.2",
+        masks="GM_prob0.2",
     )
     input = {"VBM_GM": {"data": img, "meta": {}}}
     jun_values4d = marker.fit_transform(input)["VBM_GM"]["data"]
 
     assert jun_values4d.ndim == 2
     assert_array_equal(auto4d.shape, jun_values4d.shape)
     assert_array_equal(auto4d, jun_values4d)
+
+
+def test_SphereAggregation_4D_agg_time() -> None:
+    """Test SphereAggregation object on 4D images, aggregating time."""
+    # Get the testing coordinates (for nilearn)
+    coordinates, _ = load_coordinates(COORDS)
+
+    # Get the SPM auditory data
+    subject_data = datasets.fetch_spm_auditory()
+    fmri_img = concat_imgs(subject_data.func)  # type: ignore
+
+    # Create NiftSpheresMasker
+    nifti_masker = NiftiSpheresMasker(seeds=coordinates, radius=RADIUS)
+    auto4d = nifti_masker.fit_transform(fmri_img)
+    auto_mean = auto4d.mean(axis=0)
+
+    # Create SphereAggregation object
+    marker = SphereAggregation(
+        coords=COORDS, method="mean", radius=RADIUS, time_method="mean"
+    )
+    input = {"BOLD": {"data": fmri_img, "meta": {}}}
+    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
+
+    assert jun_values4d.ndim == 1
+    assert_array_equal(auto_mean.shape, jun_values4d.shape)
+    assert_array_equal(auto_mean, jun_values4d)
+
+    auto_pick_0 = auto4d[:1, :]
+    marker = SphereAggregation(
+        coords=COORDS,
+        method="mean",
+        radius=RADIUS,
+        time_method="select",
+        time_method_params={"pick": [0]},
+    )
+
+    input = {"BOLD": {"data": fmri_img, "meta": {}}}
+    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
+
+    assert jun_values4d.ndim == 2
+    assert_array_equal(auto_pick_0.shape, jun_values4d.shape)
+    assert_array_equal(auto_pick_0, jun_values4d)
+
+    with pytest.raises(ValueError, match="can only be used with BOLD data"):
+        SphereAggregation(
+            coords=COORDS,
+            method="mean",
+            radius=RADIUS,
+            time_method="pick",
+            time_method_params={"pick": [0]},
+            on="VBM_GM",
+        )
+
+    with pytest.raises(
+        ValueError, match="can only be used with `time_method`"
+    ):
+        SphereAggregation(
+            coords=COORDS,
+            method="mean",
+            radius=RADIUS,
+            time_method_params={"pick": [0]},
+            on="VBM_GM",
+        )
+
+    with pytest.warns(RuntimeWarning, match="No time dimension to aggregate"):
+        input = {"BOLD": {"data": fmri_img.slicer[..., 0:1], "meta": {}}}
+        marker.fit_transform(input)
```

### Comparing `junifer-0.0.2.dev86/junifer/markers/utils.py` & `junifer-0.0.3.dev36/junifer/markers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Nicolás Nieto <n.nieto@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 #          Federico Raimondo <f.raimondo@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Callable, Dict, List, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import zscore
 
 from ..utils import raise_error
 
@@ -52,16 +52,17 @@
             instances[cls] = cls(*args, **kwargs)
         return instances[cls]
 
     return get_instance
 
 
 def _ets(
-    bold_ts: np.ndarray, roi_names: Union[None, List[str]] = None
-) -> np.ndarray:
+    bold_ts: np.ndarray,
+    roi_names: Union[None, List[str]] = None,
+) -> Tuple[np.ndarray, Optional[List[str]]]:
     """Compute the edge-wise time series based on BOLD time series.
 
     Take a timeseries of brain areas, and calculate timeseries for each
     edge according to the method outlined in [1]_. For more information,
     check https://github.com/brain-networks/edge-ts/blob/master/main.m
 
     Parameters
@@ -76,17 +77,16 @@
 
     Returns
     -------
     ets : np.ndarray
         edge-wise time series, i.e. estimate of functional connectivity at each
         time point.
     edge_names : List[str]
-        List of edge names corresponding to columns in the
-        edge-wise time series. This is only returned if the roi_names
-        are specified.
+        List of edge names corresponding to columns in the edge-wise time
+        series. If roi_names are not specified, this is None.
 
     References
     ----------
     .. [1] Zamani Esfahlani et al. (2020)
             High-amplitude cofluctuations in cortical activity drive
             functional connectivity
             doi: 10.1073/pnas.2005531117
@@ -98,26 +98,26 @@
     _, n_roi = timeseries.shape
     # indices of unique edges (lower triangle)
     u, v = np.tril_indices(n_roi, k=-1)
     # Compute the ETS
     ets = timeseries[:, u] * timeseries[:, v]
     # Obtain the corresponding edge labels if specified else return
     if roi_names is None:
-        return ets
+        return ets, None
     else:
         if len(roi_names) != n_roi:
             raise_error(
                 "List of roi names does not correspond "
                 "to the number of ROIs in the timeseries!"
             )
-        roi_names = np.array(roi_names)
+        _roi_names = np.array(roi_names)
         edge_names = [
-            "~".join([x, y]) for x, y in zip(roi_names[u], roi_names[v])
+            "~".join([x, y]) for x, y in zip(_roi_names[u], _roi_names[v])
         ]
-        return ets, list(edge_names)
+        return ets, edge_names
 
 
 def _correlate_dataframes(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     method: Union[str, Callable] = "pearson",
 ) -> pd.DataFrame:
```

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.3.dev36/junifer/pipeline/pipeline_step_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 from ..utils import raise_error
 from .utils import check_ext_dependencies
 
 
 class PipelineStepMixin:
     """Mixin class for a pipeline step."""
 
-    def validate_input(self, input: List[str]) -> None:
+    def validate_input(self, input: List[str]) -> List[str]:
         """Validate the input to the pipeline step.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data dictionary keys.
 
+        Returns
+        -------
+        list of str
+            The actual elements of the input that will be processed by this
+            pipeline step.
+
         Raises
         ------
         ValueError
             If the input does not have the required data.
 
         """
         raise_error(
@@ -128,16 +134,16 @@
         if hasattr(self, "_EXT_DEPENDENCIES"):
             for dependency in self._EXT_DEPENDENCIES:  # type: ignore
                 out = check_ext_dependencies(**dependency)
                 if getattr(self, f"use_{dependency['name']}", None) is None:
                     # Set attribute for using external tools
                     setattr(self, f"use_{dependency['name']}", out)
 
-        self.validate_input(input=input)
-        outputs = [self.get_output_type(t_input) for t_input in input]
+        fit_input = self.validate_input(input=input)
+        outputs = [self.get_output_type(t_input) for t_input in fit_input]
         return outputs
 
     def fit_transform(
         self, input: Dict[str, Dict], **kwargs: Any
     ) -> Dict[str, Dict]:
         """Fit and transform.
```

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/registry.py` & `junifer-0.0.3.dev36/junifer/pipeline/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,17 +128,27 @@
         base class.
 
     """
     # Set default init parameters
     if init_params is None:
         init_params = {}
     # Get class of the registered function
+    logger.debug(f"Building {step}/{name}")
     klass = get_class(step=step, name=name)
-    # Create instance of the class
-    object_ = klass(**init_params)
+    logger.debug(f"\tClass: {klass.__name__}")
+    logger.debug(f"\tInit params: {init_params}")
+    try:
+        # Create instance of the class
+        object_ = klass(**init_params)
+    except Exception as e:
+        raise_error(
+            msg=(f"Failed to create {step} ({name}). " f"Error: {e}"),
+            klass=RuntimeError,
+            exception=e,
+        )
     # Verify created instance belongs to the base class
     if not isinstance(object_, baseclass):
         raise_error(
             msg=(
                 f"Invalid {step} ({object_.__class__.__name__}). "
                 f"Must inherit from {baseclass.__name__}"
             ),
```

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.3.dev36/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     """Test validate with correct dependencies."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _DEPENDENCIES = {"setuptools"}
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
 
@@ -49,16 +49,16 @@
     """Test validate with incorrect dependencies."""
 
     class IncorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _DEPENDENCIES = {"foobar"}
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
 
@@ -74,16 +74,16 @@
     """Test validate with correct external dependencies."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _EXT_DEPENDENCIES = [{"name": "afni", "optional": False}]
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
 
@@ -100,16 +100,16 @@
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _EXT_DEPENDENCIES = [
             {"name": "afni", "optional": False, "commands": ["3dReHo"]}
         ]
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
 
@@ -128,16 +128,16 @@
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _EXT_DEPENDENCIES = [
             {"name": "afni", "optional": False, "commands": ["3d"]}
         ]
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
 
@@ -150,16 +150,16 @@
     """Test validate with incorrect external dependencies."""
 
     class IncorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
         _EXT_DEPENDENCIES = [{"name": "foobar", "optional": True}]
 
-        def validate_input(self, input: List[str]) -> None:
-            print(input)
+        def validate_input(self, input: List[str]) -> List[str]:
+            return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
         def fit_transform(self, input: Dict[str, Dict]) -> Dict[str, Dict]:
             return {"input": input}
```

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.3.dev36/junifer/pipeline/tests/test_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,7 +135,16 @@
     )
     assert isinstance(obj, ConcreteClass)
     assert obj.value == 2
 
     # Check error
     with pytest.raises(ValueError, match="Must inherit"):
         build(step="datagrabber", name="concrete", baseclass=np.ndarray)
+
+    # Check error
+    with pytest.raises(RuntimeError, match="Failed to create"):
+        build(
+            step="datagrabber",
+            name="concrete",
+            baseclass=SuperClass,
+            init_params={"wrong": 2},
+        )
```

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.3.dev36/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.3.dev36/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/pipeline/utils.py` & `junifer-0.0.3.dev36/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/preprocess/base.py` & `junifer-0.0.3.dev36/junifer/preprocess/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,34 +32,41 @@
 
         if any(x not in self.get_valid_inputs() for x in on):
             name = self.__class__.__name__
             wrong_on = [x for x in on if x not in self.get_valid_inputs()]
             raise ValueError(f"{name} cannot be computed on {wrong_on}")
         self._on = on
 
-    def validate_input(self, input: List[str]) -> None:
+    def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data dictionary keys.
 
+        Returns
+        -------
+        list of str
+            The actual elements of the input that will be processed by this
+            pipeline step.
+
         Raises
         ------
         ValueError
             If the input does not have the required data.
         """
         if not any(x in input for x in self._on):
             raise_error(
                 "Input does not have the required data."
                 f"\t Input: {input}"
                 f"\t Required (any of): {self._on}"
             )
+        return [x for x in self._on if x in input]
 
     @abstractmethod
     def get_output_type(self, input: List[str]) -> List[str]:
         """Get output type.
 
         Parameters
         ----------
@@ -75,14 +82,15 @@
 
         """
         raise_error(
             msg="Concrete classes need to implement get_output_type().",
             klass=NotImplementedError,
         )
 
+    @abstractmethod
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this
@@ -109,22 +117,37 @@
         dict
             The processed output as a dictionary.
 
         """
         out = input
         for type_ in self._on:
             if type_ in input.keys():
-                logger.info(f"Computing {type_}")
+                logger.info(f"Preprocessing {type_}")
                 t_input = input[type_]
-                extra_input = input.copy()
+
+                # Pass the other data types as extra input, removing
+                # the current type
+                extra_input = input
                 extra_input.pop(type_)
+                logger.debug(
+                    f"Extra input for preprocess: {extra_input.keys()}"
+                )
                 key, t_out = self.preprocess(
                     input=t_input, extra_input=extra_input
                 )
+
+                # Add the output to the Junifer Data object
+                logger.debug(f"Adding {key} to output")
                 out[key] = t_out
+
+                # In case we are creating a new type, re-add the original input
+                if key != type_:
+                    logger.debug("Adding original input back to output")
+                    out[type_] = t_input
+
                 self.update_meta(out[key], "preprocess")
         return out
 
     @abstractmethod
     def preprocess(
         self,
         input: Dict[str, Any],
```

### Comparing `junifer-0.0.2.dev86/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.3.dev36/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from nilearn._utils.niimg_conversions import check_niimg_4d
 from nilearn.image import clean_img
-from nilearn.masking import compute_brain_mask
 
 from ...api.decorators import register_preprocessor
+from ...data import get_mask
 from ...utils import logger, raise_error
 from ..base import BasePreprocessor
 
 
 if TYPE_CHECKING:
     from nibabel import MGHImage, Nifti1Image, Nifti2Image
 
@@ -130,34 +130,33 @@
         (default None).
     high_pass : float, optional
         High cutoff frequencies, in Hertz. If None, no filtering is
         applied (default None).
     t_r : float, optional
         Repetition time, in second (sampling period).
         If None, it will use t_r from nifti header (default None).
-    mask_img: Niimg-like object, optional
-        If provided, signal is only cleaned from voxels inside the mask.
-        If mask is provided, it should have same shape and affine as imgs.
-        If not provided, a mask is computed using
-        :func:`nilearn.masking.compute_brain_mask` (default None).
+    masks : str, dict or list of dict or str, optional
+        The specification of the masks to apply to regions before extracting
+        signals. Check :ref:`Using Masks <using_masks>` for more details.
+        If None, will not apply any mask (default None).
 
     """
 
     _DEPENDENCIES = {"numpy", "nilearn"}
 
     def __init__(
         self,
         strategy: Optional[Dict[str, str]] = None,
         spike: Optional[float] = None,
         detrend: bool = True,
         standardize: bool = True,
         low_pass: Optional[float] = None,
         high_pass: Optional[float] = None,
         t_r: Optional[float] = None,
-        mask_img: Optional["Nifti1Image"] = None,
+        masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
     ) -> None:
         """Initialise the class."""
         if strategy is None:
             strategy = {
                 "motion": "full",
                 "wm_csf": "full",
                 "global_signal": "full",
@@ -165,15 +164,15 @@
         self.strategy = strategy
         self.spike = spike
         self.detrend = detrend
         self.standardize = standardize
         self.low_pass = low_pass
         self.high_pass = high_pass
         self.t_r = t_r
-        self.mask_img = mask_img
+        self.masks = masks
 
         self._valid_components = ["motion", "wm_csf", "global_signal"]
         self._valid_confounds = ["basic", "power2", "derivatives", "full"]
 
         if any(not isinstance(k, str) for k in strategy.keys()):
             raise_error("Strategy keys must be strings", ValueError)
 
@@ -197,22 +196,27 @@
                 f"If any of them is a valid parameter in "
                 "nilearn.interfaces.fmriprep.load_confounds we may "
                 "include it in the future",
                 klass=ValueError,
             )
         super().__init__()
 
-    def validate_input(self, input: List[str]) -> None:
+    def validate_input(self, input: List[str]) -> List[str]:
         """Validate the input to the pipeline step.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data object keys.
+        Returns
+        -------
+        list of str
+            The actual elements of the input that will be processed by this
+            pipeline step.
 
         Raises
         ------
         ValueError
             If the input does not have the required data.
 
         """
@@ -221,14 +225,16 @@
             raise_error(
                 msg="Input does not have the required data. \n"
                 f"Input: {input} \n"
                 f"Required (all off): {_required_inputs} \n",
                 klass=ValueError,
             )
 
+        return [x for x in self._on if x in input]
+
     def get_output_type(self, input: List[str]) -> List[str]:
         """Get the kind of the pipeline step.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
@@ -517,49 +523,61 @@
                     "Check if this file matches the adhoc specification for "
                     "this dataset."
                 )
         elif t_format != "fmriprep":
             raise ValueError(f"Invalid confounds format {t_format}")
 
     def _remove_confounds(
-        self, bold_img: "Nifti1Image", confounds_df: pd.DataFrame
+        self,
+        input: Dict[str, Any],
+        extra_input: Optional[Dict[str, Any]] = None,
     ) -> Union["Nifti1Image", "Nifti2Image", "MGHImage", List]:
         """Remove confounds from the BOLD image.
 
         Parameters
         ----------
-        bold_img : Niimg-like object
-            4D image. The signals in the last dimension are filtered
-            (see http://nilearn.github.io/manipulating_images/input_output.html
-            for a detailed description of the valid input types).
-        confounds_df : pd.DataFrame
-            Dataframe containing confounds to remove. Number of rows should
-            correspond to number of volumes in the BOLD image.
+        input : dict
+            Dictionary containing the ``BOLD`` value from the
+            Junifer Data object.
+        extra_input : dict, optional
+            Dictionary containing the rest of the Junifer Data object. Must
+            include the ``BOLD_confounds`` key.
 
         Returns
         --------
         Niimg-like object
             Input image with confounds removed.
 
         """
+        assert extra_input is not None  # Not the case, data is validated
+        confounds_df = self._pick_confounds(extra_input["BOLD_confounds"])
         confounds_array = confounds_df.values
 
+        bold_img = input["data"]
         t_r = self.t_r
         if t_r is None:
             logger.info("No `t_r` specified, using t_r from nifti header")
             zooms = bold_img.header.get_zooms()  # type: ignore
             t_r = zooms[3]
             logger.info(
                 f"Read t_r from nifti header: {t_r}",
             )
 
-        mask_img = self.mask_img
-        if mask_img is None:
-            logger.info("Computing brain mask from image")
-            mask_img = compute_brain_mask(bold_img)
+        mask_img = None
+        if self.masks is not None:
+            logger.debug(f"Masking with {self.masks}")
+            mask_img = get_mask(
+                masks=self.masks, target_data=input, extra_input=extra_input
+            )
+            # Save the mask in the extra input and link it to the bold data
+            # this allows to use "inherit" down the pipeline
+            if extra_input is not None:
+                logger.debug("Setting mask_item")
+                extra_input["BOLD_mask"] = {"data": mask_img}
+                input["mask_item"] = "BOLD_mask"
 
         logger.info("Cleaning image")
         logger.debug(f"\tdetrend: {self.detrend}")
         logger.debug(f"\tstandardize: {self.standardize}")
         logger.debug(f"\tlow_pass: {self.low_pass}")
         logger.debug(f"\thigh_pass: {self.high_pass}")
         clean_bold = clean_img(
@@ -596,12 +614,9 @@
             The key to store the output in the Junifer Data object.
         object : dict
             The computed result as dictionary. This will be stored in the
             Junifer Data object under the key ``key``.
 
         """
         self._validate_data(input, extra_input)
-        assert extra_input is not None
-        bold_img = input["data"]
-        confounds_df = self._pick_confounds(extra_input["BOLD_confounds"])
-        input["data"] = self._remove_confounds(bold_img, confounds_df)
+        input["data"] = self._remove_confounds(input, extra_input=extra_input)
         return "BOLD", input
```

### Comparing `junifer-0.0.2.dev86/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.3.dev36/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files 6% similar despite different names*

```diff
@@ -448,18 +448,18 @@
     confound_remover = fMRIPrepConfoundRemover(
         strategy={"wm_csf": "full"}, spike=0.2
     )
     reader = DefaultDataReader()
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
         input = dg["sub-01"]
         input = reader.fit_transform(input)
-        confounds = confound_remover._pick_confounds(input["BOLD_confounds"])
         raw_bold = input["BOLD"]["data"]
+        extra_input = {k: v for k, v in input.items() if k != "BOLD"}
         clean_bold = confound_remover._remove_confounds(
-            bold_img=raw_bold, confounds_df=confounds
+            input=input["BOLD"], extra_input=extra_input
         )
         clean_bold = typing.cast(nib.Nifti1Image, clean_bold)
         # TODO: Find a better way to test functionality here
         assert (
             clean_bold.header.get_zooms()  # type: ignore
             == raw_bold.header.get_zooms()  # type: ignore
         )
@@ -529,12 +529,68 @@
         assert t_meta["strategy"] == confound_remover.strategy
         assert t_meta["spike"] is None
         assert t_meta["detrend"] is True
         assert t_meta["standardize"] is True
         assert t_meta["low_pass"] is None
         assert t_meta["high_pass"] is None
         assert t_meta["t_r"] is None
-        assert t_meta["mask_img"] is None
+        assert t_meta["masks"] is None
+
+        assert "dependencies" in output["BOLD"]["meta"]
+        dependencies = output["BOLD"]["meta"]["dependencies"]
+        assert dependencies == {"numpy", "nilearn"}
+
+
+def test_fMRIPrepConfoundRemover_fit_transform_masks() -> None:
+    """Test fMRIPrepConfoundRemover with all confounds present."""
+
+    # need reader for the data
+    reader = DefaultDataReader()
+    # All strategies full, no spike
+    confound_remover = fMRIPrepConfoundRemover(
+        masks={"compute_brain_mask": {"threshold": 0.2}}
+    )
+
+    with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
+        input = dg["sub-01"]
+        input = reader.fit_transform(input)
+        orig_bold = input["BOLD"]["data"].get_fdata().copy()
+        output = confound_remover.fit_transform(input)
+        trans_bold = output["BOLD"]["data"].get_fdata()
+        # Transformation is in place
+        assert_array_equal(trans_bold, input["BOLD"]["data"].get_fdata())
+
+        # Data should have the same shape
+        assert orig_bold.shape == trans_bold.shape
+
+        # but be different
+        assert_raises(
+            AssertionError, assert_array_equal, orig_bold, trans_bold
+        )
+
+        assert "meta" in output["BOLD"]
+        assert "preprocess" in output["BOLD"]["meta"]
+        t_meta = output["BOLD"]["meta"]["preprocess"]
+        assert t_meta["class"] == "fMRIPrepConfoundRemover"
+        # It should have all the default parameters
+        assert t_meta["strategy"] == confound_remover.strategy
+        assert t_meta["spike"] is None
+        assert t_meta["detrend"] is True
+        assert t_meta["standardize"] is True
+        assert t_meta["low_pass"] is None
+        assert t_meta["high_pass"] is None
+        assert t_meta["t_r"] is None
+        assert isinstance(t_meta["masks"], dict)
+        assert t_meta["masks"] is not None
+        assert len(t_meta["masks"]) == 1
+        assert "compute_brain_mask" in t_meta["masks"]
+        assert len(t_meta["masks"]["compute_brain_mask"]) == 1
+        assert "threshold" in t_meta["masks"]["compute_brain_mask"]
+        assert t_meta["masks"]["compute_brain_mask"]["threshold"] == 0.2
+
+        assert "BOLD_mask" in output
+        assert "mask_item" in output["BOLD"]
+        assert output["BOLD"]["mask_item"] == "BOLD_mask"
 
         assert "dependencies" in output["BOLD"]["meta"]
         dependencies = output["BOLD"]["meta"]["dependencies"]
         assert dependencies == {"numpy", "nilearn"}
```

### Comparing `junifer-0.0.2.dev86/junifer/storage/base.py` & `junifer-0.0.3.dev36/junifer/storage/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from ..utils import raise_error
 from .utils import process_meta
 
@@ -53,16 +53,17 @@
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid storage types for input.
 
         Returns
         -------
         list of str
-            The list of storage types that can be used as input for this "
-            "storage.
+            The list of storage types that can be used as input for this
+            storage interface.
+
         """
         raise_error(
             msg="Concrete classes need to implement get_valid_inputs().",
             klass=NotImplementedError,
         )
 
     def validate(self, input_: List[str]) -> None:
@@ -83,35 +84,35 @@
             raise_error(
                 "Input does not have the required data."
                 f"\t Input: {input}"
                 f"\t Required (any of): {self._valid_inputs}"
             )
 
     @abstractmethod
-    def list_features(self) -> Dict:
+    def list_features(self) -> Dict[str, Dict[str, Any]]:
         """List the features in the storage.
 
         Returns
         -------
         dict
-            List of features in the storage. The keys are the feature names to
-            be used in read_features() and the values are the metadata of each
+            List of features in the storage. The keys are the feature MD5 to
+            be used in :meth:`.read_df` and the values are the metadata of each
             feature.
 
         """
         raise_error(
             msg="Concrete classes need to implement list_features().",
             klass=NotImplementedError,
         )
 
     @abstractmethod
     def read_df(
         self,
         feature_name: Optional[str] = None,
-        feature_md5: Optional[bool] = None,
+        feature_md5: Optional[str] = None,
     ) -> pd.DataFrame:
         """Read feature into a pandas DataFrame.
 
         Parameters
         ----------
         feature_name : str, optional
             Name of the feature to read (default None).
@@ -148,15 +149,15 @@
         )
 
     def store(self, kind: str, **kwargs) -> None:
         """Store extracted features data.
 
         Parameters
         ----------
-        kind : {"matrix", "timeseries", "table"}
+        kind : {"matrix", "timeseries", "vector"}
             The storage kind.
         **kwargs
             The keyword arguments.
 
         Raises
         ------
         ValueError
@@ -175,109 +176,105 @@
         self.store_metadata(meta_md5=meta_md5, element=t_element, meta=t_meta)
         if kind == "matrix":
             self.store_matrix(meta_md5=meta_md5, element=t_element, **kwargs)
         elif kind == "timeseries":
             self.store_timeseries(
                 meta_md5=meta_md5, element=t_element, **kwargs
             )
-        elif kind == "table":
-            self.store_table(meta_md5=meta_md5, element=t_element, **kwargs)
+        elif kind == "vector":
+            self.store_vector(meta_md5=meta_md5, element=t_element, **kwargs)
 
     def store_matrix(
         self,
         meta_md5: str,
         element: Dict,
         data: np.ndarray,
         col_names: Optional[Iterable[str]] = None,
         row_names: Optional[Iterable[str]] = None,
-        matrix_kind: Optional[str] = "full",
+        matrix_kind: str = "full",
         diagonal: bool = True,
     ) -> None:
         """Store matrix.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         data : numpy.ndarray
             The matrix data to store.
         col_names : list or tuple of str, optional
-            The column names (default None).
+            The column labels (default None).
         row_names : str, optional
-            The column name to use in case number of rows greater than 1.
-            If None and number of rows greater than 1, then the name will be
-            "index" (default None).
+            The row labels (default None).
         matrix_kind : str, optional
             The kind of matrix:
 
             * ``triu`` : store upper triangular only
             * ``tril`` : store lower triangular
             * ``full`` : full matrix
 
             (default "full").
         diagonal : bool, optional
-            Whether to store the diagonal. If `matrix_kind` is "full", setting
+            Whether to store the diagonal. If ``matrix_kind = full``, setting
             this to False will raise an error (default True).
+
         """
         raise_error(
-            msg="Concrete classes need to implement store_matrix2d().",
+            msg="Concrete classes need to implement store_matrix().",
             klass=NotImplementedError,
         )
 
-    def store_table(
+    def store_vector(
         self,
         meta_md5: str,
         element: Dict,
         data: Union[np.ndarray, List],
-        columns: Optional[Iterable[str]] = None,
-        rows_col_name: Optional[str] = None,
+        col_names: Optional[Iterable[str]] = None,
     ) -> None:
-        """Store table.
+        """Store vector.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         data : numpy.ndarray or list
-            The table data to store.
-        columns : list or tuple of str, optional
-            The columns (default None).
-        rows_col_name : str, optional
-            The column name to use in case number of rows greater than 1.
-            If None and number of rows greater than 1, then the name will be
-            "index" (default None).
+            The vector data to store.
+        col_names : list or tuple of str, optional
+            The column labels (default None).
+
         """
         raise_error(
-            msg="Concrete classes need to implement store_table().",
+            msg="Concrete classes need to implement store_vector().",
             klass=NotImplementedError,
         )
 
     def store_timeseries(
         self,
         meta_md5: str,
         element: Dict,
         data: np.ndarray,
-        columns: Optional[Iterable[str]] = None,
+        col_names: Optional[Iterable[str]] = None,
     ) -> None:
-        """Implement timeseries storing.
+        """Store timeseries.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         data : numpy.ndarray
             The timeseries data to store.
-        columns : list or tuple of str, optional
+        col_names : list or tuple of str, optional
             The column labels (default None).
+
         """
         raise_error(
             msg="Concrete classes need to implement store_timeseries().",
             klass=NotImplementedError,
         )
 
     @abstractmethod
```

### Comparing `junifer-0.0.2.dev86/junifer/storage/pandas_base.py` & `junifer-0.0.3.dev36/junifer/storage/pandas_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import json
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
+from ..utils import raise_error
 from .base import BaseFeatureStorage
 
 
 class PandasBaseFeatureStorage(BaseFeatureStorage):
     """Abstract base class for feature storage via pandas.
 
     For every interface that is required, one needs to provide a concrete
@@ -42,18 +43,19 @@
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid storage types for input.
 
         Returns
         -------
         list of str
-            The list of storage types that can be used as input for this "
-            "storage.
+            The list of storage types that can be used as input for this
+            storage interface.
+
         """
-        return ["matrix", "table", "timeseries"]
+        return ["matrix", "vector", "timeseries"]
 
     def _meta_row(self, meta: Dict, meta_md5: str) -> pd.DataFrame:
         """Convert the metadata to a pandas DataFrame.
 
         Parameters
         ----------
         meta : dict
@@ -72,49 +74,58 @@
         df = pd.DataFrame(data_df, index=[meta_md5])
         df.index.name = "meta_md5"
         return df
 
     @staticmethod
     def element_to_index(
         element: Dict, n_rows: int = 1, rows_col_name: Optional[str] = None
-    ) -> pd.MultiIndex:
+    ) -> Union[pd.Index, pd.MultiIndex]:
         """Convert the element metadata to index.
 
         Parameters
         ----------
         element : dict
             The element as a dictionary.
         n_rows : int, optional
             Number of rows to create (default 1).
         rows_col_name: str, optional
-            The column name to use in case `n_rows` > 1. If None and
-            n_rows > 1, the name will be "idx" (default None).
+            The column name to use in case ``n_rows`` > 1. If None and
+            ``n_rows`` > 1, the name will be "idx" (default None).
 
         Returns
         -------
-        pandas.MultiIndex
+        pandas.Index or pandas.MultiIndex
             The index of the dataframe to store.
 
-        Raises
-        ------
-        ValueError
-            If `meta` does not contain the key "element".
-
         """
-        # Check rows_col_name
-        if rows_col_name is None:
-            rows_col_name = "idx"
-        elem_idx: Dict[Any, Any] = {
+        # Make mapping between element access keys and values
+        elem_idx: Dict[str, Iterable[str]] = {
             k: [v] * n_rows for k, v in element.items()
         }
-        elem_idx[rows_col_name] = np.arange(n_rows)
-        # Create index
-        index = pd.MultiIndex.from_frame(
-            pd.DataFrame(elem_idx, index=range(n_rows))
-        )
+
+        # Set rows_col_name if n_rows > 1 (timeseries)
+        if n_rows > 1:
+            # Set rows_col_name if None
+            if rows_col_name is None:
+                rows_col_name = "idx"
+            # Set extra column for variable number of rows per element
+            elem_idx[rows_col_name] = np.arange(n_rows)
+
+        # Create correct index for elements with single access variable
+        if len(elem_idx) == 1:
+            # Create normal index for vector
+            index = pd.Index(
+                data=list(elem_idx.values())[0], name=list(elem_idx.keys())[0]
+            )
+        else:
+            # Create multiindex for timeseries
+            index = pd.MultiIndex.from_frame(
+                pd.DataFrame(elem_idx, index=range(n_rows))
+            )
+
         return index
 
     def store_df(
         self, meta_md5: str, element: Dict, df: Union[pd.DataFrame, pd.Series]
     ) -> None:
         """Implement pandas DataFrame storing.
 
@@ -128,107 +139,115 @@
         Raises
         ------
         ValueError
             If the dataframe index has items that are not in the index
             generated from the metadata.
 
         """
-        raise NotImplementedError("Implement in subclass.")
+        raise_error(
+            msg="Concrete classes need to implement store_df().",
+            klass=NotImplementedError,
+        )
 
     def _store_2d(
         self,
         meta_md5: str,
         element: Dict,
         data: Union[np.ndarray, List],
-        columns: Optional[Iterable[str]] = None,
+        col_names: Optional[Iterable[str]] = None,
         rows_col_name: Optional[str] = None,
     ) -> None:
-        """Store 2D dataframe.
+        """Store 2D data.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
-        data : numpy.ndarray or List
+        data : numpy.ndarray or list
             The data to store.
-        columns : list or tuple of str, optional
-            The columns (default None).
+        col_names : list or tuple of str, optional
+            The column labels (default None).
         rows_col_name : str, optional
             The column name to use in case number of rows greater than 1.
             If None and number of rows greater than 1, then the name will be
-            "index" (default None).
+            "idx" (default None).
 
         """
-        n_rows = len(data)
         # Convert element metadata to index
         idx = self.element_to_index(
-            element=element, n_rows=n_rows, rows_col_name=rows_col_name
+            element=element, n_rows=len(data), rows_col_name=rows_col_name
         )
         # Prepare new dataframe
-        data_df = pd.DataFrame(  # type: ignore
-            data, columns=columns, index=idx  # type: ignore
+        df = pd.DataFrame(
+            data=data, columns=col_names, index=idx  # type: ignore
         )
         # Store dataframe
-        self.store_df(meta_md5=meta_md5, element=element, df=data_df)
+        self.store_df(meta_md5=meta_md5, element=element, df=df)
 
-    def store_table(
+    def store_vector(
         self,
         meta_md5: str,
         element: Dict,
         data: Union[np.ndarray, List],
-        columns: Optional[Iterable[str]] = None,
-        rows_col_name: Optional[str] = None,
+        col_names: Optional[Iterable[str]] = None,
     ) -> None:
-        """Implement table storing.
+        """Store vector.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
-        data : numpy.ndarray or List
-            The table data to store.
-        columns : list or tuple of str, optional
-            The columns (default None).
-        rows_col_name : str, optional
-            The column name to use in case number of rows greater than 1.
-            If None and number of rows greater than 1, then the name will be
-            "index" (default None).
+        data : numpy.ndarray or list
+            The vector data to store.
+        col_names : list or tuple of str, optional
+            The column labels (default None).
+
         """
+        if isinstance(data, list):
+            # Flatten out list and convert to np.ndarray
+            processed_data = np.array(np.ravel(data))
+        elif isinstance(data, np.ndarray):
+            # Flatten out array
+            processed_data = data.ravel()
+
+        # Make it 2D
+        processed_data = processed_data[np.newaxis, :]
+
         self._store_2d(
             meta_md5=meta_md5,
             element=element,
             data=data,
-            columns=columns,
-            rows_col_name=rows_col_name,
+            col_names=col_names,
         )
 
     def store_timeseries(
         self,
         meta_md5: str,
         element: Dict,
         data: np.ndarray,
-        columns: Optional[Iterable[str]] = None,
+        col_names: Optional[Iterable[str]] = None,
     ) -> None:
-        """Implement timeseries storing.
+        """Store timeseries.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         data : numpy.ndarray
             The timeseries data to store.
-        columns : list or tuple of str, optional
+        col_names : list or tuple of str, optional
             The column labels (default None).
+
         """
         self._store_2d(
             meta_md5=meta_md5,
             element=element,
             data=data,
-            columns=columns,
+            col_names=col_names,
             rows_col_name="timepoint",
         )
```

### Comparing `junifer-0.0.2.dev86/junifer/storage/sqlite.py` & `junifer-0.0.3.dev36/junifer/storage/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import json
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from pandas.core.base import NoNewAttributesMixin
 from pandas.io.sql import pandasSQL_builder  # type: ignore
 from sqlalchemy import create_engine, inspect
 from tqdm import tqdm
 
 from ..api.decorators import register_storage
 from ..utils import logger, raise_error, warn_with_log
 from .pandas_base import PandasBaseFeatureStorage
-from .utils import element_to_prefix
+from .utils import element_to_prefix, matrix_to_vector, store_matrix_checks
 
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Engine
 
 
 @register_storage
@@ -30,29 +30,30 @@
     """Concrete implementation for feature storage via SQLite.
 
     Parameters
     ----------
     uri : str or pathlib.Path
         The path to the file to be used.
     single_output : bool, optional
-        If False, will create one file per element. The name
+        If False, will create one SQLite file per element. The name
         of the file will be prefixed with the respective element.
-        If True, will create only one file as specified in the `uri` and
-        store all the elements in the same file. This behaviour is only
-        suitable for non-parallel executions. SQLite does not support
-        concurrency (default True).
+        If True, will create only one SQLite file as specified in the
+        ``uri`` and store all the elements in the same file. This behaviour
+        is only suitable for non-parallel executions. SQLite does not
+        support concurrency (default True).
     upsert : {"ignore", "update"}, optional
         Upsert mode. If "ignore" is used, the existing elements are ignored.
         If "update", the existing elements are updated (default "update").
     **kwargs : dict
             The keyword arguments passed to the superclass.
 
     See Also
     --------
     PandasBaseFeatureStorage : The base class for Pandas-based feature storage.
+    HDF5FeatureStorage : The concrete class for HDF5-based feature storage.
 
     """
 
     def __init__(
         self,
         uri: Union[str, Path],
         single_output: bool = True,
@@ -74,31 +75,31 @@
         if not uri.parent.exists():
             logger.info(
                 f"Output directory ({str(uri.parent.absolute())}) "
                 "does not exist, creating now."
             )
             uri.parent.mkdir(parents=True, exist_ok=True)
         # Available storage kinds
-        storage_types = ["table", "timeseries", "matrix"]
+        storage_types = ["vector", "timeseries", "matrix"]
         super().__init__(
             uri=uri,
             storage_types=storage_types,
             single_output=single_output,
             **kwargs,
         )
         # Set upsert
         self._upsert = upsert
 
     def get_engine(self, element: Optional[Dict] = None) -> "Engine":
         """Get engine.
 
         Parameters
         ----------
-        meta : dict, optional
-            The metadata as dictionary (default None).
+        element : dict, optional
+            The element as dictionary (default None).
 
         Returns
         -------
         sqlalchemy.engine.Engine
             The sqlalchemy engine.
 
         """
@@ -201,32 +202,38 @@
                     # is present or not.
                     raise_error(msg=f"Table ({name}) already exists.")
                 else:
                     raise_error(
                         msg=f"Invalid option {if_exists} for if_exists."
                     )
 
-    def list_features(self) -> Dict:
+    def list_features(self) -> Dict[str, Dict[str, Any]]:
         """List the features in the storage.
 
         Returns
         -------
         dict
-            List of features in the storage. The keys are the feature names to
-            be used in read_features() and the values are the metadata of each
+            List of features in the storage. The keys are the feature MD5 to
+            be used in :meth:`.read_df` and the values are the metadata of each
             feature.
 
         """
+        # Retrieve meta table from storage
         meta_df = pd.read_sql(
             sql="meta",
             con=self.get_engine(),
             index_col="meta_md5",
         )
+        # Format index names for retrieved data
         meta_df.index = meta_df.index.str.replace(r"meta_", "")
-        out = meta_df.to_dict(orient="index")  # type: ignore
+        # Convert dataframe to dictionary
+        out: Dict[str, Dict[str, str]] = meta_df.to_dict(
+            orient="index"
+        )  # type: ignore
+        # Format output
         for md5, t_meta in out.items():
             for k, v in t_meta.items():
                 out[md5][k] = json.loads(v)
         return out
 
     def read_df(
         self,
@@ -389,105 +396,81 @@
     def store_matrix(
         self,
         meta_md5: str,
         element: Dict,
         data: np.ndarray,
         col_names: Optional[List[str]] = None,
         row_names: Optional[List[str]] = None,
-        matrix_kind: Optional[str] = "full",
+        matrix_kind: str = "full",
         diagonal: bool = True,
     ) -> None:
-        """Implement matrix storing.
+        """Store matrix.
 
         Parameters
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         data : numpy.ndarray
             The matrix data to store.
         meta : dict
             The metadata as a dictionary.
         col_names : list or tuple of str, optional
-            The column names (default None).
+            The column labels (default None).
         row_names : str, optional
-            The column name to use in case number of rows greater than 1.
-            If None and number of rows greater than 1, then the name will be
-            "index" (default None).
+            The row labels (optional None).
         matrix_kind : str, optional
             The kind of matrix:
 
             * ``triu`` : store upper triangular only
             * ``tril`` : store lower triangular
             * ``full`` : full matrix
 
             (default "full").
         diagonal : bool, optional
-            Whether to store the diagonal. If `matrix_kind` is "full", setting
+            Whether to store the diagonal. If ``matrix_kind = full``, setting
             this to False will raise an error (default True).
 
         """
-        if diagonal is False and matrix_kind not in ["triu", "tril"]:
-            raise_error(
-                msg="Diagonal cannot be False if kind is not full",
-                klass=ValueError,
-            )
-
-        if matrix_kind in ["triu", "tril"]:
-            if data.shape[0] != data.shape[1]:
-                raise_error(
-                    "Cannot store a non-square matrix as a triangular matrix",
-                    klass=ValueError,
-                )
-
-        if matrix_kind == "triu":
-            k = 0 if diagonal is True else 1
-            data_idx = np.triu_indices(data.shape[0], k=k)
-        elif matrix_kind == "tril":
-            k = 0 if diagonal is True else -1
-            data_idx = np.tril_indices(data.shape[0], k=k)
-        elif matrix_kind == "full":
-            data_idx = (
-                np.repeat(np.arange(data.shape[0]), data.shape[1]),
-                np.tile(np.arange(data.shape[1]), data.shape[0]),
-            )
-        else:
-            raise_error(msg=f"Invalid kind {matrix_kind}", klass=ValueError)
-
+        # Row data validation
         if row_names is None:
             row_names = [f"r{i}" for i in range(data.shape[0])]
-        elif len(row_names) != data.shape[0]:
-            raise_error(
-                msg="Number of row names does not match number of rows",
-                klass=ValueError,
-            )
-
+        # Column data validation
         if col_names is None:
             col_names = [f"c{i}" for i in range(data.shape[1])]
-        elif len(col_names) != data.shape[1]:
-            raise_error(
-                msg="Number of column names does not match number of columns",
-                klass=ValueError,
-            )
-
-        flat_data = data[data_idx]
-        columns = [
-            f"{row_names[i]}~{col_names[j]}"
-            for i, j in zip(data_idx[0], data_idx[1])
-        ]
+        # Parameter checks
+        store_matrix_checks(
+            matrix_kind=matrix_kind,
+            diagonal=diagonal,
+            data_shape=data.shape,
+            row_names_len=len(row_names),  # type: ignore
+            col_names_len=len(col_names),  # type: ignore
+        )
+        # Matrix to vector conversion
+        flat_data, columns = matrix_to_vector(
+            data=data,
+            col_names=col_names,
+            row_names=row_names,
+            matrix_kind=matrix_kind,
+            diagonal=diagonal,
+        )
 
         # Convert element metadata to index
         n_rows = 1
         idx = self.element_to_index(
             element=element, n_rows=n_rows, rows_col_name=None
         )
         # Prepare new dataframe
-        data_df = pd.DataFrame(flat_data[None, :], columns=columns, index=idx)
+        data_df = pd.DataFrame(
+            flat_data[np.newaxis, :], columns=columns, index=idx
+        )
 
+        # SQLite's SQLITE_MAX_COLUMN is 2000, so if more than that,
+        # convert it to long format
         if len(columns) > 2000:
             warn_with_log(
                 msg="The number of columns is greater than 2000. "
                 "The data will be stored in long format. "
                 "This will make it slower to collect the data. "
                 "Future versions of junifer will provide additional storage "
                 "options that will not raise this warning.",
@@ -506,15 +489,18 @@
         Raises
         ------
         NotImplementedError
             If ``single_output`` is True.
 
         """
         if self.single_output is True:
-            raise_error(msg="collect() is not implemented for single output.")
+            raise_error(
+                msg="collect() is not implemented for single output.",
+                klass=IOError,
+            )
         logger.info(
             "Collecting data from "
             f"{self.uri.parent}/*{self.uri.name}"  # type: ignore
         )
         # Create new instance
         out_storage = SQLiteFeatureStorage(uri=self.uri, upsert="ignore")
         # Glob files
```

### Comparing `junifer-0.0.2.dev86/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.3.dev36/junifer/storage/tests/test_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provide tests for sqlite."""
+"""Provide tests for SQLite storage interface."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 from typing import List, Union
@@ -357,24 +357,24 @@
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
     features = storage.list_features()
     feature_md5 = list(features.keys())[0]
     assert meta_md5 == feature_md5
 
 
-def test_store_table(tmp_path: Path) -> None:
-    """Test table store.
+def test_store_vector(tmp_path: Path) -> None:
+    """Test vector store.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    uri = tmp_path / "test_store_table.sqlite"
+    uri = tmp_path / "test_store_vector.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Metadata to store
     element = {"subject": "test"}
     dependencies = ["numpy"]
     meta = {
         "element": element,
         "dependencies": dependencies,
@@ -385,79 +385,48 @@
     meta_md5, meta_to_store, element_to_store = process_meta(meta)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
 
     # Data to store
-    data = [
-        [1, 10],
-        [2, 20],
-        [3, 30],
-        [4, 40],
-        [5, 50],
-    ]
+    data = [[10, 20, 30, 40, 50]]
+    col_names = ["f1", "f2", "f3", "f4", "f5"]
     # Convert element to index
-    idx = storage.element_to_index(element, n_rows=5, rows_col_name="scan")
+    idx = storage.element_to_index(element=element)
     # Create dataframe
-    df = pd.DataFrame(data, columns=["f1", "f2"], index=idx)
+    df = pd.DataFrame(data=data, columns=col_names, index=idx)
 
     # Store table
-    storage.store_table(
+    storage.store_vector(
         meta_md5=meta_md5,
         element=element_to_store,
         data=data,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=col_names,
     )
     # Read stored table
     c_df = _read_sql(
         table_name=f"meta_{meta_md5}",
         uri=uri.as_posix(),
-        index_col=["subject", "scan"],
+        index_col=["subject"],
     )
     # Check if dataframes are equal
     assert_frame_equal(df, c_df)
 
-    # New data to store
-    data_new = [[1, 10], [2, 20], [3, 300], [4, 40], [5, 50], [6, 600]]
-    # Convert element to index
-    idx_new = storage.element_to_index(element, n_rows=6, rows_col_name="scan")
-    # Create dataframe
-    df_new = pd.DataFrame(data_new, columns=["f1", "f2"], index=idx_new)
-    # Check warning
-    with pytest.warns(RuntimeWarning, match=r"Some rows"):
-        # Store table
-        storage.store_table(
-            meta_md5=meta_md5,
-            element=element_to_store,
-            data=data_new,
-            columns=["f1", "f2"],
-            rows_col_name="scan",
-        )
-    # Read stored table
-    c_df_new = _read_sql(
-        table_name=f"meta_{meta_md5}",
-        uri=uri.as_posix(),
-        index_col=["subject", "scan"],
-    )
-    # Check if dataframes are equal
-    assert_frame_equal(df_new, c_df_new)
-
 
 def test_store_matrix(tmp_path: Path) -> None:
     """Test matrix store.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    uri = tmp_path / "test_store_table.sqlite"
+    uri = tmp_path / "test_store_matrix.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Metadata to store
     element = {"subject": "test"}
     dependencies = ["numpy"]
     meta = {
         "element": element,
         "dependencies": dependencies,
@@ -474,15 +443,15 @@
     # Store 4 x 3 full matrix
     data = np.array(
         [[1, 2, 3], [11, 22, 33], [111, 222, 333], [1111, 2222, 3333]]
     )
     row_names = ["row1", "row2", "row3", "row4"]
     col_names = ["col1", "col2", "col3"]
 
-    # Store table
+    # Store matrix
     storage.store_matrix(
         meta_md5=meta_md5,
         element=element_to_store,
         data=data,
         row_names=row_names,
         col_names=col_names,
     )
@@ -493,21 +462,21 @@
     assert "BOLD_fc" == features[feature_md5]["name"]
 
     read_df = storage.read_df(feature_md5=feature_md5)
     assert read_df.shape == (1, 12)
     assert_array_equal(read_df.values[0], data.flatten())
     assert list(read_df.columns) == stored_names
     # Store without row and column names
-    uri = tmp_path / "test_store_table_nonames.sqlite"
+    uri = tmp_path / "test_store_matrix_nonames.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
-    # Store table
+    # Store matrix
     storage.store_matrix(
         meta_md5=meta_md5, element=element_to_store, data=data
     )
     stored_names = [
         f"r{i}~c{j}"
         for i in range(data.shape[0])
         for j in range(data.shape[1])
@@ -549,15 +518,15 @@
             diagonal=False,
         )
 
     # Store upper triangular matrix
     data = np.array([[1, 2, 3], [11, 22, 33], [111, 222, 333]])
     row_names = ["row1", "row2", "row3"]
     col_names = ["col1", "col2", "col3"]
-    uri = tmp_path / "test_store_table_triu.sqlite"
+    uri = tmp_path / "test_store_matrix_triu.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
     storage.store_matrix(
         meta_md5=meta_md5,
@@ -583,15 +552,15 @@
     read_df = storage.read_df(feature_md5=feature_md5)
     assert list(read_df.columns) == stored_names
     assert_array_equal(
         read_df.values, data[np.triu_indices(n=data.shape[0])][None, :]
     )
 
     # Store upper triangular matrix without diagonal
-    uri = tmp_path / "test_store_table_triu_nodiagonal.sqlite"
+    uri = tmp_path / "test_store_matrix_triu_nodiagonal.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
     storage.store_matrix(
         meta_md5=meta_md5,
@@ -618,15 +587,15 @@
         read_df.values, data[np.triu_indices(n=data.shape[0], k=1)][None, :]
     )
 
     # Store lower triangular matrix
     data = np.array([[1, 2, 3], [11, 22, 33], [111, 222, 333]])
     row_names = ["row1", "row2", "row3"]
     col_names = ["col1", "col2", "col3"]
-    uri = tmp_path / "test_store_table_tril.sqlite"
+    uri = tmp_path / "test_store_matrix_tril.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
     storage.store_matrix(
         meta_md5=meta_md5,
@@ -652,15 +621,15 @@
     read_df = storage.read_df(feature_md5=feature_md5)
     assert list(read_df.columns) == stored_names
     assert_array_equal(
         read_df.values, data[np.tril_indices(n=data.shape[0])][None, :]
     )
 
     # Store lower triangular matrix without diagonal
-    uri = tmp_path / "test_store_table_tril_nodiagonal.sqlite"
+    uri = tmp_path / "test_store_matrix_tril_nodiagonal.sqlite"
     storage = SQLiteFeatureStorage(uri=uri)
     # Store metadata
     storage.store_metadata(
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
     storage.store_matrix(
         meta_md5=meta_md5,
@@ -683,14 +652,68 @@
     read_df = storage.read_df(feature_md5=feature_md5)
     assert list(read_df.columns) == stored_names
     assert_array_equal(
         read_df.values, data[np.tril_indices(n=data.shape[0], k=-1)][None, :]
     )
 
 
+def test_store_timeseries(tmp_path: Path) -> None:
+    """Test timeseries store.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+    uri = tmp_path / "test_store_timeseries.sqlite"
+    storage = SQLiteFeatureStorage(uri=uri)
+    # Metadata to store
+    element = {"subject": "test"}
+    dependencies = ["numpy"]
+    meta = {
+        "element": element,
+        "dependencies": dependencies,
+        "marker": {"name": "fc"},
+        "type": "BOLD",
+    }
+
+    meta_md5, meta_to_store, element_to_store = process_meta(meta)
+    # Store metadata
+    storage.store_metadata(
+        meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
+    )
+
+    # Data to store
+    data = np.array([[10], [20], [30], [40], [50]])
+    col_names = ["signal"]
+    # Convert element to index
+    idx = storage.element_to_index(
+        element=element, n_rows=5, rows_col_name="timepoint"
+    )
+    # Create dataframe
+    df = pd.DataFrame(data=data, columns=col_names, index=idx)
+
+    # Store table
+    storage.store_timeseries(
+        meta_md5=meta_md5,
+        element=element_to_store,
+        data=data,
+        col_names=col_names,
+    )
+    # Read stored table
+    c_df = _read_sql(
+        table_name=f"meta_{meta_md5}",
+        uri=uri.as_posix(),
+        index_col=["subject", "timepoint"],
+    )
+    # Check if dataframes are equal
+    assert_frame_equal(df, c_df)
+
+
 # TODO: can the test be parametrized?
 def test_store_multiple_output(tmp_path: Path):
     """Test storing using single_output=False.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
@@ -715,82 +738,66 @@
     meta3 = {
         "element": {"subject": "test-01", "session": "ses-02"},
         "dependencies": ["numpy"],
         "marker": {"name": "fc"},
         "type": "BOLD",
     }
     # Data to store
-    data1 = np.array(
-        [
-            [1, 10],
-            [2, 20],
-            [3, 30],
-            [4, 40],
-            [5, 50],
-        ]
-    )
+    data1 = np.array([[10, 20, 30, 40, 50]])
     data2 = data1 * 10
     data3 = data1 * 20
+    col_names = ["f1", "f2", "f3", "f4", "f5"]
     # Process metadata for storage
     hash1, meta_to_store1, element_to_store1 = process_meta(meta1)
     # Convert element to index
-    idx1 = storage.element_to_index(
-        element_to_store1, n_rows=5, rows_col_name="scan"
-    )
+    idx1 = storage.element_to_index(element=element_to_store1)
     # Create dataframe
-    df1 = pd.DataFrame(data1, columns=["f1", "f2"], index=idx1)
+    df1 = pd.DataFrame(data1, columns=col_names, index=idx1)
     # Process metadata for storage
     hash2, meta_to_store2, element_to_store2 = process_meta(meta2)
     # Convert element to index
-    idx2 = storage.element_to_index(
-        element_to_store2, n_rows=5, rows_col_name="scan"
-    )
+    idx2 = storage.element_to_index(element=element_to_store2)
     # Create dataframe
-    df2 = pd.DataFrame(data2, columns=["f1", "f2"], index=idx2)
+    df2 = pd.DataFrame(data2, columns=col_names, index=idx2)
     # Process metadata for storage
     hash3, meta_to_store3, element_to_store3 = process_meta(meta3)
     # Convert element to index
-    idx3 = storage.element_to_index(
-        element_to_store3, n_rows=5, rows_col_name="scan"
-    )
+    idx3 = storage.element_to_index(element=element_to_store3)
     # Create dataframe
-    df3 = pd.DataFrame(data3, columns=["f1", "f2"], index=idx3)
+    df3 = pd.DataFrame(data3, columns=col_names, index=idx3)
     # Check hash equality
     assert hash1 == hash2
     assert hash2 == hash3
     # Store tables
     storage.store_metadata(
         meta_md5=hash1, element=element_to_store1, meta=meta_to_store1
     )
     storage.store_metadata(
         meta_md5=hash2, element=element_to_store2, meta=meta_to_store2
     )
     storage.store_metadata(
         meta_md5=hash3, element=element_to_store3, meta=meta_to_store3
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash1,
         element=element_to_store1,
         data=data1,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=col_names,
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash2,
         element=element_to_store2,
         data=data2,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=col_names,
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash3,
         element=element_to_store3,
         data=data3,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=col_names,
     )
     # Check that URI does not exist yet
     assert not uri.exists()
     # Convert element to preifx
     prefix1 = element_to_prefix(meta1["element"])
     prefix2 = element_to_prefix(meta2["element"])
     prefix3 = element_to_prefix(meta3["element"])
@@ -799,20 +806,20 @@
     uri2 = uri.parent / f"{prefix2}{uri.name}"
     uri3 = uri.parent / f"{prefix3}{uri.name}"
     # Check URIs for data storage exist
     assert uri1.exists()
     assert uri2.exists()
     assert uri3.exists()
     # Set index columns
-    cols = ["subject", "session", "scan"]
+    idx_cols = ["subject", "session"]
     table_name = f"meta_{hash1}"
     # Read stored tables
-    cdf1 = _read_sql(table_name, uri1.as_posix(), index_col=cols)
-    cdf2 = _read_sql(table_name, uri2.as_posix(), index_col=cols)
-    cdf3 = _read_sql(table_name, uri3.as_posix(), index_col=cols)
+    cdf1 = _read_sql(table_name, uri1.as_posix(), index_col=idx_cols)
+    cdf2 = _read_sql(table_name, uri2.as_posix(), index_col=idx_cols)
+    cdf3 = _read_sql(table_name, uri3.as_posix(), index_col=idx_cols)
     # Check if dataframes are equal
     assert_frame_equal(df1, cdf1)
     assert_frame_equal(df2, cdf2)
     assert_frame_equal(df3, cdf3)
 
 
 # TODO: can test be paramtrized?
@@ -867,34 +874,31 @@
     )
     storage.store_metadata(
         meta_md5=hash2, element=element_to_store2, meta=meta_to_store2
     )
     storage.store_metadata(
         meta_md5=hash3, element=element_to_store3, meta=meta_to_store3
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash1,
         element=element_to_store1,
         data=data1,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=["f1", "f2"],
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash2,
         element=element_to_store2,
         data=data2,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=["f1", "f2"],
     )
-    storage.store_table(
+    storage.store_vector(
         meta_md5=hash3,
         element=element_to_store3,
         data=data3,
-        columns=["f1", "f2"],
-        rows_col_name="scan",
+        col_names=["f1", "f2"],
     )
     # Convert element to prefix
     prefix1 = element_to_prefix(meta1["element"])
     prefix2 = element_to_prefix(meta2["element"])
     prefix3 = element_to_prefix(meta3["element"])
     # URIs for data storage
     uri1 = uri.parent / f"{prefix1}{uri.name}"
@@ -907,15 +911,15 @@
     # Check that URI does not exist yet
     assert not uri.exists()
     # Collect data
     storage.collect()
     # Check that URI exists now
     assert uri.exists()
     # Set index columns
-    cols = ["subject", "session", "scan"]
+    cols = ["subject", "session"]
     # Store metadata
     table_name = f"meta_{hash1}"
     # Read stored tables
     all_df = _read_sql(table_name, uri.as_posix(), index_col=cols)
     cdf1 = _read_sql(table_name, uri1.as_posix(), index_col=cols)
     cdf2 = _read_sql(table_name, uri2.as_posix(), index_col=cols)
     cdf3 = _read_sql(table_name, uri3.as_posix(), index_col=cols)
```

### Comparing `junifer-0.0.2.dev86/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.3.dev36/junifer/storage/tests/test_storage_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 from junifer.storage.base import BaseFeatureStorage
 
 
 def test_BaseFeatureStorage_abstractness() -> None:
     """Test BaseFeatureStorage is abstract base class."""
     with pytest.raises(TypeError, match=r"abstract"):
-        BaseFeatureStorage(uri="/tm", storage_types=["matrix"])  # type: ignore
+        BaseFeatureStorage(
+            uri="/tmp", storage_types=["matrix"]  # type: ignore
+        )
 
 
 def test_BaseFeatureStorage() -> None:
     """Test proper subclassing of BaseFeatureStorage."""
+
     # Create concrete class
     class MyFeatureStorage(BaseFeatureStorage):
         """Implement concrete class."""
 
-        def __init__(self, uri, single_output=False):
-            storage_types = ["matrix", "table", "timeseries"]
+        def __init__(self, uri, single_output=True):
+            storage_types = ["matrix", "vector", "timeseries"]
             super().__init__(
                 uri=uri,
                 storage_types=storage_types,
                 single_output=single_output,
             )
 
         def get_valid_inputs(self):
-            return ["matrix", "table", "timeseries"]
+            return ["matrix", "vector", "timeseries"]
 
         def list_features(self):
             super().list_features()
 
         def read_df(self, feature_name=None, feature_md5=None):
             super().read_df(
                 feature_name=feature_name,
@@ -44,15 +47,15 @@
         def store_metadata(self, meta_md5, meta, element):
             super().store_metadata(meta_md5, meta, element)
 
         def collect(self):
             return super().collect()
 
     # Check single_output is False
-    st = MyFeatureStorage(uri="/tmp")
+    st = MyFeatureStorage(uri="/tmp", single_output=False)
     assert st.single_output is False
     # Check single_output is True
     st = MyFeatureStorage(uri="/tmp", single_output=True)
     assert st.single_output is True
 
     # Check validate with valid argument
     st.validate(input_=["matrix"])
@@ -62,19 +65,17 @@
 
     with pytest.raises(NotImplementedError):
         st.list_features()
 
     with pytest.raises(NotImplementedError):
         st.read_df(None)
 
-    element = {"subject": "test"}
-    dependencies = ["numpy"]
     meta = {
-        "element": element,
-        "dependencies": dependencies,
+        "element": {"subject": "test"},
+        "dependencies": ["numpy"],
         "marker": {"name": "fc"},
         "type": "BOLD",
     }
 
     with pytest.raises(NotImplementedError):
         st.store(kind="matrix", meta=meta)
 
@@ -84,13 +85,13 @@
     with pytest.raises(NotImplementedError):
         st.collect()
 
     with pytest.raises(NotImplementedError):
         st.store(kind="timeseries", meta=meta)
 
     with pytest.raises(NotImplementedError):
-        st.store(kind="table", meta=meta)
+        st.store(kind="vector", meta=meta)
 
     with pytest.raises(ValueError):
         st.store(kind="lego", meta=meta)
 
     assert st.uri == "/tmp"
```

### Comparing `junifer-0.0.2.dev86/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.3.dev36/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/datagrabbers.py` & `junifer-0.0.3.dev36/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/registry.py` & `junifer-0.0.3.dev36/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.3.dev36/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.3.dev36/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.3.dev36/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.3.dev36/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/testing/utils.py` & `junifer-0.0.3.dev36/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/utils/logging.py` & `junifer-0.0.3.dev36/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer/utils/tests/test_fs.py` & `junifer-0.0.3.dev36/junifer/utils/tests/test_fs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Provide tests for filesystem manipulation."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
-
+import stat
 from pathlib import Path
 
 from junifer.utils.fs import make_executable
 
 
 def test_make_executable(tmp_path: Path) -> None:
     """Test making path executable.
@@ -18,13 +18,13 @@
         The path to the test directory.
 
     """
     test_file_path = tmp_path / "make_me_executable.txt"
     test_file_path.write_bytes(b"umm")
     test_file_stat_initial = test_file_path.stat()
     # Check initial file mode
-    assert test_file_stat_initial.st_mode == 33188
+    assert stat.S_IMODE(test_file_stat_initial.st_mode) & stat.S_IEXEC == 0
     # Make the path executable
     make_executable(test_file_path)
     test_file_stat_final = test_file_path.stat()
     # Check final file mode
-    assert test_file_stat_final.st_mode == 33252
+    assert stat.S_IMODE(test_file_stat_final.st_mode) & stat.S_IEXEC != 0
```

### Comparing `junifer-0.0.2.dev86/junifer/utils/tests/test_logging.py` & `junifer-0.0.3.dev36/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/junifer.egg-info/PKG-INFO` & `junifer-0.0.3.dev36/junifer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.2.dev86
+Version: 0.0.3.dev36
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -34,14 +34,15 @@
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is curently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.2.dev86/junifer.egg-info/SOURCES.txt` & `junifer-0.0.3.dev36/junifer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.gitmodules
 AUTHORS.rst
 LICENSE.md
 README.md
 codecov.yml
 conda-env.yml
 ignore_words.txt
 pyproject.toml
@@ -22,57 +23,62 @@
 .github/workflows/lint.yml
 .github/workflows/pypi.yml
 docs/Makefile
 docs/builtin.rst
 docs/conf.py
 docs/contribution.rst
 docs/faq.rst
+docs/help.rst
 docs/index.rst
 docs/installation.rst
 docs/links.inc
 docs/maintaining.rst
 docs/redirect.html
+docs/starting.rst
 docs/whats_new.rst
 docs/_static/css/custom.css
 docs/_static/js/custom.js
 docs/_templates/versions.html
 docs/api/api.rst
 docs/api/configs.rst
 docs/api/data.rst
 docs/api/datagrabbers.rst
 docs/api/datareaders.rst
 docs/api/index.rst
 docs/api/markers.rst
+docs/api/nilearn.rst
 docs/api/pipeline.rst
 docs/api/preprocessing.rst
 docs/api/stats.rst
 docs/api/storage.rst
 docs/api/testing.rst
 docs/api/utils.rst
-docs/changes/0.0.1.inc
 docs/changes/contributors.inc
-docs/changes/latest.inc
+docs/changes/newsfragments/.gitignore
+docs/changes/newsfragments/220.doc
+docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
+docs/extending/masks.rst
+docs/extending/parcellations.rst
 docs/images/junifer_logo.png
-docs/images/pipeline/pipeline.001.png
-docs/images/pipeline/pipeline.002.png
 docs/sphinxext/gh_substitutions.py
 docs/understanding/data.rst
 docs/understanding/datagrabber.rst
 docs/understanding/datareader.rst
 docs/understanding/index.rst
 docs/understanding/marker.rst
 docs/understanding/pipeline.rst
 docs/understanding/preprocess.rst
 docs/understanding/storage.rst
 docs/using/codeless.rst
 docs/using/index.rst
+docs/using/masks.rst
 docs/using/queueing.rst
 docs/using/running.rst
 examples/README.rst
 examples/norun_hcpfc_pearson.py
 examples/norun_ukbvm_gmd.py
 examples/run_compute_parcel_mean.py
 examples/run_datagrabber_bids_datalad.py
@@ -174,14 +180,19 @@
 junifer/datagrabber/tests/test_multiple.py
 junifer/datagrabber/tests/test_pattern.py
 junifer/datagrabber/tests/test_pattern_datalad.py
 junifer/datareader/__init__.py
 junifer/datareader/default.py
 junifer/datareader/tests/test_default_reader.py
 junifer/external/__init__.py
+junifer/external/h5io/h5io/__init__.py
+junifer/external/h5io/h5io/_h5io.py
+junifer/external/h5io/h5io/_version.py
+junifer/external/h5io/h5io/chunked_array.py
+junifer/external/h5io/h5io/chunked_list.py
 junifer/external/nilearn/__init__.py
 junifer/external/nilearn/junifer_nifti_spheres_masker.py
 junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
 junifer/markers/__init__.py
 junifer/markers/base.py
 junifer/markers/collection.py
 junifer/markers/ets_rss.py
@@ -213,14 +224,21 @@
 junifer/markers/reho/reho_base.py
 junifer/markers/reho/reho_estimator.py
 junifer/markers/reho/reho_parcels.py
 junifer/markers/reho/reho_spheres.py
 junifer/markers/reho/tests/test_reho_estimator.py
 junifer/markers/reho/tests/test_reho_parcels.py
 junifer/markers/reho/tests/test_reho_spheres.py
+junifer/markers/temporal_snr/__init__.py
+junifer/markers/temporal_snr/temporal_snr_base.py
+junifer/markers/temporal_snr/temporal_snr_parcels.py
+junifer/markers/temporal_snr/temporal_snr_spheres.py
+junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
 junifer/markers/tests/test_collection.py
 junifer/markers/tests/test_ets_rss.py
 junifer/markers/tests/test_marker_utils.py
 junifer/markers/tests/test_markers_base.py
 junifer/markers/tests/test_parcel_aggregation.py
 junifer/markers/tests/test_sphere_aggregation.py
 junifer/pipeline/__init__.py
@@ -235,17 +253,19 @@
 junifer/preprocess/base.py
 junifer/preprocess/confounds/__init__.py
 junifer/preprocess/confounds/fmriprep_confound_remover.py
 junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
 junifer/preprocess/tests/test_preprocess_base.py
 junifer/storage/__init__.py
 junifer/storage/base.py
+junifer/storage/hdf5.py
 junifer/storage/pandas_base.py
 junifer/storage/sqlite.py
 junifer/storage/utils.py
+junifer/storage/tests/test_hdf5.py
 junifer/storage/tests/test_pandas_base.py
 junifer/storage/tests/test_sqlite.py
 junifer/storage/tests/test_storage_base.py
 junifer/storage/tests/test_utils.py
 junifer/testing/__init__.py
 junifer/testing/datagrabbers.py
 junifer/testing/registry.py
```

### Comparing `junifer-0.0.2.dev86/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.3.dev36/tools/create_aomic1000_example_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,101 @@
+"""Create a testing dataset for the DataladAOMICID1000 pattern datagrabber."""
+
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Xuan Li <xu.li@fz-juelich.de>
 # License: AGPL
 from tempfile import TemporaryDirectory
 from pathlib import Path
 
 import datalad.api as dl
 
 # repo has to be created on gin manually beforehand if not owner
-dst = 'git@gin.g-node.org:/juaml/datalad-example-aomic1000.git'
+dst = "git@gin.g-node.org:/juaml/datalad-example-aomic1000.git"
 
 # Use this if you create repo directly when pushing (see below)
 # dst_api = 'git@gin.g-node.org'
 # org_name = PurePosixPath('juaml')
 # repo_basename = PurePosixPath('datalad-example-aomic1000.git')
 
 with TemporaryDirectory() as tmpdir_name:
     tmpdir = Path(tmpdir_name)
     ds = dl.create(tmpdir)  # type: ignore
 
-    base_dir = tmpdir / 'derivatives'
+    base_dir = tmpdir / "derivatives"
     base_dir.mkdir(exist_ok=True, parents=True)
 
-    for dtype in ['dwipreproc', 'fmriprep']:
+    for dtype in ["dwipreproc", "fmriprep"]:
         dtype_dir = base_dir / dtype
         dtype_dir.mkdir()
 
         for i_sub in range(1, 10):
-            t_sub = f'sub-{i_sub:04d}'
+            t_sub = f"sub-{i_sub:04d}"
             sub_dir = dtype_dir / t_sub
             sub_dir.mkdir()
 
-            if dtype == 'fmriprep':
-                for dname in ['func', 'anat']:
+            if dtype == "fmriprep":
+                for dname in ["func", "anat"]:
                     (sub_dir / dname).mkdir()
 
                 fnames = [
-                    (f'anat/{t_sub}_space-MNI152NLin2009cAsym_desc-preproc'
-                     '_T1w.nii.gz'),
-                    (f'anat/{t_sub}_space-MNI152NLin2009cAsym_label-'
-                     'CSF_probseg.nii.gz'),
-                    (f'anat/{t_sub}_space-MNI152NLin2009cAsym_label-'
-                     'GM_probseg.nii.gz'),
-                    (f'anat/{t_sub}_space-MNI152NLin2009cAsym_label-'
-                     'WM_probseg.nii.gz'),
-                    (f'func/{t_sub}_task-moviewatching_space-'
-                     'MNI152NLin2009cAsym_desc-preproc_bold.nii.gz'),
-                    (f'func/{t_sub}_task-moviewatching_space-'
-                     'MNI152NLin2009cAsym_desc-preproc_bold.json'),
-                    (f'func/{t_sub}_task-moviewatching_desc-confounds'
-                     '_regressors.tsv'),
-                    (f'func/{t_sub}_task-moviewatching_desc-confounds'
-                     '_regressors.json'),
+                    (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_desc-preproc"
+                        "_T1w.nii.gz"
+                    ),
+                    (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
+                        "CSF_probseg.nii.gz"
+                    ),
+                    (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
+                        "GM_probseg.nii.gz"
+                    ),
+                    (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
+                        "WM_probseg.nii.gz"
+                    ),
+                    (
+                        f"func/{t_sub}_task-moviewatching_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
+                    ),
+                    (
+                        f"func/{t_sub}_task-moviewatching_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.json"
+                    ),
+                    (
+                        f"func/{t_sub}_task-moviewatching_desc-confounds"
+                        "_regressors.tsv"
+                    ),
+                    (
+                        f"func/{t_sub}_task-moviewatching_desc-confounds"
+                        "_regressors.json"
+                    ),
+                    (
+                        f"func/{t_sub}_task-moviewatching_"
+                        "space-MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
+                    ),
+                    (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_"
+                        "desc-brain_mask.nii.gz"
+                    ),
                 ]
 
-            elif dtype == 'dwipreproc':
-                dname = 'dwi'
+            elif dtype == "dwipreproc":
+                dname = "dwi"
                 (sub_dir / dname).mkdir()
 
                 fnames = [
-                    (f'{dname}/{t_sub}_desc-preproc_dwi.nii.gz'),
+                    (f"{dname}/{t_sub}_desc-preproc_dwi.nii.gz"),
                 ]
 
             for fname in fnames:
-                with open(sub_dir / fname, 'w') as f:
-                    f.write('placeholder')
+                with open(sub_dir / fname, "w") as f:
+                    f.write("placeholder")
 
     ds.save(recursive=True)
     # use this to create the repo automatically, only possible for juaml owner
     # ds.create_sibling_gin(
     #   (org_name/repo_basename).as_posix(), name='gin', existing='reconfigure',
     #   api=dst_api, access_protocol='ssh')
-    ds.siblings('add', name='gin', url=dst)
-    ds.push(to='gin', force='all')
+    ds.siblings("add", name="gin", url=dst)
+    ds.push(to="gin", force="all")
```

### Comparing `junifer-0.0.2.dev86/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.3.dev36/tools/create_aomicpiop2_example_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Create an example/testing dataset for PIOP1 with mock data."""
+"""Create an example/testing dataset for PIOP2 with mock data."""
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Xuan Li <xu.li@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 # License: AGPL
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import datalad.api as dl
 
 
 # repo has to be created on gin manually beforehand if not owner
-dst = "git@gin.g-node.org:/juaml/datalad-example-aomicpiop1.git"
+dst = "git@gin.g-node.org:/juaml/datalad-example-aomicpiop2.git"
 
 with TemporaryDirectory() as tmpdir_name:
     tmpdir = Path(tmpdir_name)
     ds = dl.create(tmpdir)  # type: ignore
 
     base_dir = tmpdir / "derivatives"
     base_dir.mkdir(exist_ok=True, parents=True)
@@ -35,59 +35,57 @@
 
                 fnames = [
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_desc-preproc"
                         "_T1w.nii.gz"
                     ),
                     (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym"
+                        "_desc-brain_mask.nii.gz"
+                    ),
+                    (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "CSF_probseg.nii.gz"
                     ),
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "GM_probseg.nii.gz"
                     ),
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "WM_probseg.nii.gz"
                     ),
                 ]
 
                 tasks = [
-                    "anticipation_acq-seq",
+                    "stopsignal_acq-seq",
                     "emomatching_acq-seq",
-                    "faces_acq-mb3",
-                    "gstroop_acq-seq",
-                    "restingstate_acq-mb3",
+                    "restingstate_acq-seq",
                     "workingmemory_acq-seq",
                 ]
                 for t in tasks:
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_space-"
-                            "MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
-                        )
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
+                    )
+                    fnames.append(
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.json"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_space-"
-                            "MNI152NLin2009cAsym_desc-preproc_bold.json"
-                        )
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_desc-confounds"
-                            "_regressors.tsv"
-                        )
+                        f"func/{t_sub}_task-{t}_desc-confounds"
+                        "_regressors.tsv"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_desc-confounds"
-                            "_regressors.json"
-                        )
+                        f"func/{t_sub}_task-{t}_desc-confounds"
+                        "_regressors.json"
                     )
 
             elif dtype == "dwipreproc":
                 dname = "dwi"
                 (sub_dir / dname).mkdir()
 
                 fnames = [
```

### Comparing `junifer-0.0.2.dev86/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.3.dev36/tools/create_aomicpiop1_example_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Create an example/testing dataset for PIOP2 with mock data."""
+"""Create an example/testing dataset for PIOP1 with mock data."""
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Xuan Li <xu.li@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 # License: AGPL
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import datalad.api as dl
 
 
 # repo has to be created on gin manually beforehand if not owner
-dst = "git@gin.g-node.org:/juaml/datalad-example-aomicpiop2.git"
+dst = "git@gin.g-node.org:/juaml/datalad-example-aomicpiop1.git"
 
 with TemporaryDirectory() as tmpdir_name:
     tmpdir = Path(tmpdir_name)
     ds = dl.create(tmpdir)  # type: ignore
 
     base_dir = tmpdir / "derivatives"
     base_dir.mkdir(exist_ok=True, parents=True)
@@ -35,57 +35,59 @@
 
                 fnames = [
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_desc-preproc"
                         "_T1w.nii.gz"
                     ),
                     (
+                        f"anat/{t_sub}_space-MNI152NLin2009cAsym_"
+                        "desc-brain_mask.nii.gz"  
+                    ),
+                    (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "CSF_probseg.nii.gz"
                     ),
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "GM_probseg.nii.gz"
                     ),
                     (
                         f"anat/{t_sub}_space-MNI152NLin2009cAsym_label-"
                         "WM_probseg.nii.gz"
                     ),
                 ]
 
                 tasks = [
-                    "stopsignal_acq-seq",
+                    "anticipation_acq-seq",
                     "emomatching_acq-seq",
-                    "restingstate_acq-seq",
+                    "faces_acq-mb3",
+                    "gstroop_acq-seq",
+                    "restingstate_acq-mb3",
                     "workingmemory_acq-seq",
                 ]
                 for t in tasks:
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_space-"
-                            "MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
-                        )
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
+                    )
+                    fnames.append(
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-preproc_bold.json"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_space-"
-                            "MNI152NLin2009cAsym_desc-preproc_bold.json"
-                        )
+                        f"func/{t_sub}_task-{t}_space-"
+                        "MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_desc-confounds"
-                            "_regressors.tsv"
-                        )
+                        f"func/{t_sub}_task-{t}_desc-confounds"
+                        "_regressors.tsv"
                     )
                     fnames.append(
-                        (
-                            f"func/{t_sub}_task-{t}_desc-confounds"
-                            "_regressors.json"
-                        )
+                        f"func/{t_sub}_task-{t}_desc-confounds"
+                        "_regressors.json"
                     )
 
             elif dtype == "dwipreproc":
                 dname = "dwi"
                 (sub_dir / dname).mkdir()
 
                 fnames = [
```

### Comparing `junifer-0.0.2.dev86/tools/create_bids_example_dataset.py` & `junifer-0.0.3.dev36/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.3.dev36/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.2.dev86/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.3.dev36/tools/create_hcp1200_example_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     with TemporaryDirectory() as tmpdir:
         # Convert str to Path
         tmpdir_path = Path(tmpdir)
         # Set base directory
         basedir = tmpdir_path / "example_hcp1200"
         # Create new datalad dataset
-        dataset = dl.create(path=str(basedir.absolute()))
+        dataset = dl.create(path=str(basedir.absolute()))  # type: ignore
         # Generate subject directories
         for sub in range(1, 10):
             subdir = basedir / f"sub-{sub:02d}"
             # Create subject directory
             subdir.mkdir()
 
             for (task, phase_encoding) in product(
@@ -53,22 +53,33 @@
                     subdir
                     / "MNINonLinear"
                     / "Results"
                     / f"{new_task}_{phase_encoding}"
                 )
                 # Create subject data directory
                 sub_datadir.mkdir(parents=True)
+
                 # Set subject data file
                 sub_datafile = (
                     sub_datadir
-                    / f"{new_task}_{phase_encoding}_hp2000_clean.nii.gz"
+                    / f"{new_task}_{phase_encoding}.nii.gz"
                 )
                 # Create subject data file
                 with open(sub_datafile, "w") as f:
                     f.write("placeholder")
 
+                if "REST" in task:
+                    # Set subject data file with ICA+FIX
+                    sub_datafile = (
+                        sub_datadir
+                        / f"{new_task}_{phase_encoding}_hp2000_clean.nii.gz"
+                    )
+                    # Create subject data file with ICA+FIX
+                    with open(sub_datafile, "w") as f:
+                        f.write("placeholder")
+
         # Save datalad dataset
         dataset.save(recursive=True)
         # Add datalad sibling
         dataset.siblings(action="add", name="gin", url=DST)
         # Push dataset to sibling
         dataset.push(to="gin", force="all")
```

### Comparing `junifer-0.0.2.dev86/tox.ini` & `junifer-0.0.3.dev36/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 [testenv:test]
 skip_install = false
 passenv =
     HOME
 deps =
     pytest
 commands =
-    pytest -vv
+    pytest
 
 [testenv:coverage]
 skip_install = false
 deps =
     pytest
     pytest-cov
 commands =
-    pytest --cov={envsitepackagesdir}/junifer --cov-report=xml -vv --cov-report=term
+    pytest --cov={envsitepackagesdir}/junifer --cov-report=xml --cov-report=term
 
 [testenv:codespell]
 skip_install = true
 deps =
     codespell
 commands =
     codespell --config tox.ini examples/ junifer/ scratch/ tools/
@@ -69,14 +69,15 @@
 ################
 # Tool configs #
 ################
 
 [isort]
 skip =
     __init__.py
+    junifer/external/h5io
 profile = black
 line_length = 79
 lines_after_imports = 2
 known_first_party = junifer
 known_third_party =
     click
     numpy
@@ -87,14 +88,15 @@
     sqlalchemy
     yaml
     pytest
 
 [flake8]
 exclude =
     __init__.py
+    junifer/external/h5io
 max-line-length = 79
 extend-ignore =
     ; Use of `functools.lru_cache` or `functools.cache` on methods can lead to
     ; memory leaks. The cache may retain instance references, preventing garbage
     ; collection.
     B019
     ; abstract class with no abstract methods
@@ -133,26 +135,27 @@
 [coverage:run]
 branch = true
 omit =
     */setup.py
     */_version.py
     */tests/*
     */junifer/configs/*
+    */junifer/external/h5io/*
 parallel = false
 
 [coverage:report]
 exclude_lines =
     # Have to re-enable the standard pragma
     pragma: no cover
     # Type checking if statements should not be considered
     if TYPE_CHECKING:
     # Don't complain if non-runnable code isn't run:
     if __name__ == .__main__.:
 precision = 2
 
 [codespell]
-skip = docs/auto_*,*.html,.git/,*.pyc,docs/_build
+skip = docs/auto_*,*.html,.git/,*.pyc,docs/_build,junifer/external/h5io/
 count =
 quiet-level = 3
 ignore-words = ignore_words.txt
 interactive = 0
 builtin = clear,rare,informal,names,usage
```

