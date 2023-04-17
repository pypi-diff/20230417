# Comparing `tmp/WAZP-0.1.3.tar.gz` & `tmp/WAZP-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WAZP-0.1.3.tar", last modified: Mon Apr  3 11:47:57 2023, max compression
+gzip compressed data, was "WAZP-0.2.0.tar", last modified: Mon Apr 17 17:55:26 2023, max compression
```

## Comparing `WAZP-0.1.3.tar` & `WAZP-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.032089 WAZP-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-03 11:47:39.000000 WAZP-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.016089 WAZP-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.020089 WAZP-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-03 11:47:39.000000 WAZP-0.1.3/.github/workflows/docs_build_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-03 11:47:39.000000 WAZP-0.1.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-03 11:47:39.000000 WAZP-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-03 11:47:39.000000 WAZP-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-03 11:47:39.000000 WAZP-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-03 11:47:39.000000 WAZP-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-03 11:47:39.000000 WAZP-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-03 11:47:57.032089 WAZP-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-03 11:47:39.000000 WAZP-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.020089 WAZP-0.1.3/WAZP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-03 11:47:54.000000 WAZP-0.1.3/WAZP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-03 11:47:57.000000 WAZP-0.1.3/WAZP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:47:54.000000 WAZP-0.1.3/WAZP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-03 11:47:54.000000 WAZP-0.1.3/WAZP.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-03 11:47:54.000000 WAZP-0.1.3/WAZP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 11:47:54.000000 WAZP-0.1.3/WAZP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-03 11:47:39.000000 WAZP-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.020089 WAZP-0.1.3/sample_project/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-03 11:47:39.000000 WAZP-0.1.3/sample_project/input_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-03 11:47:39.000000 WAZP-0.1.3/sample_project/metadata_fields.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.028089 WAZP-0.1.3/sample_project/videos/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-03 11:47:42.000000 WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:47:57.032089 WAZP-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.028089 WAZP-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.028089 WAZP-0.1.3/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_integration/test_smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.028089 WAZP-0.1.3/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_unit/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-03 11:47:42.000000 WAZP-0.1.3/tests/test_unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-03 11:47:42.000000 WAZP-0.1.3/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.032089 WAZP-0.1.3/wazp/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.032089 WAZP-0.1.3/wazp/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/callbacks/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/callbacks/home.py
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/callbacks/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/callbacks/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:47:57.032089 WAZP-0.1.3/wazp/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/pages/01_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/pages/02_ROI.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/pages/03_pose_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/pages/04_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/pages/home.py
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-04-03 11:47:42.000000 WAZP-0.1.3/wazp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 17:55:09.000000 WAZP-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.824925 WAZP-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.824925 WAZP-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 17:55:09.000000 WAZP-0.2.0/.github/workflows/docs_build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-17 17:55:09.000000 WAZP-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-17 17:55:09.000000 WAZP-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 17:55:09.000000 WAZP-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-17 17:55:09.000000 WAZP-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-17 17:55:09.000000 WAZP-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 17:55:09.000000 WAZP-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-17 17:55:26.832925 WAZP-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-17 17:55:09.000000 WAZP-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.828925 WAZP-0.2.0/WAZP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-17 17:55:26.000000 WAZP-0.2.0/WAZP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-17 17:55:09.000000 WAZP-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.828925 WAZP-0.2.0/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 17:55:09.000000 WAZP-0.2.0/sample_project/input_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-17 17:55:09.000000 WAZP-0.2.0/sample_project/metadata_fields.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/sample_project/videos/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:55:26.832925 WAZP-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/test_smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-17 17:55:12.000000 WAZP-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25843 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/01_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/02_ROI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/03_pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/04_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/utils.py
```

### Comparing `WAZP-0.1.3/.github/workflows/docs_build_and_deploy.yml` & `WAZP-0.2.0/.github/workflows/docs_build_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/.github/workflows/test_and_deploy.yml` & `WAZP-0.2.0/.github/workflows/test_and_deploy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
       - '*'
   pull_request:
 
 jobs:
   linting:
     runs-on: ubuntu-latest
     steps:
-      - uses: neuroinformatics-unit/actions/lint@v2
+      - uses: neuroinformatics-unit/actions/lint@v2.0.0
 
   manifest:
     name: Check Manifest
     runs-on: ubuntu-latest
     steps:
-      - uses: neuroinformatics-unit/actions/check_manifest@v2
+      - uses: neuroinformatics-unit/actions/check_manifest@v2.0.0
 
   test:
     needs: [linting, manifest]
     name: ${{ matrix.os }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
@@ -40,25 +40,25 @@
       - name: Fix Chrome application path on Windows
         if: matrix.os == 'windows-latest'
         shell: bash
         run: |
           echo "C:\Program Files\Google\Chrome\Application" >> $GITHUB_PATH
 
       # Run tests
-      - uses: neuroinformatics-unit/actions/test@v2
+      - uses: neuroinformatics-unit/actions/test@v2.0.0
         with:
           python-version: ${{ matrix.python-version }}
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
-    - uses: neuroinformatics-unit/actions/build_sdist_wheels@v2
+    - uses: neuroinformatics-unit/actions/build_sdist_wheels@v2.0.0
 
 
   upload_all:
     name: Publish build distributions
     needs: [build_sdist_wheels]
     runs-on: ubuntu-latest
     steps:
```

### Comparing `WAZP-0.1.3/.gitignore` & `WAZP-0.2.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -82,11 +82,7 @@
 .python-version
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
-
-sample_project_2/pose_estimation_results/*.csv
-sample_project_2/pose_estimation_results/*.pickle
-*.pickle
```

### Comparing `WAZP-0.1.3/.pre-commit-config.yaml` & `WAZP-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/CONTRIBUTING.md` & `WAZP-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/LICENSE` & `WAZP-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/PKG-INFO` & `WAZP-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WAZP
-Version: 0.1.3
+Version: 0.2.0
 Summary: Wasp Animal-tracking Zoo project with Pose estimation
 Author-email: Sofia Miñano <s.minano@ucl.ac.uk>, Nikoloz Sirmpilatze <niko.sirbiladze@gmail.com>, Sam Cunliffe <s.cunliffe@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/SainsburyWellcomeCentre/WAZP
 Project-URL: Bug tracker, https://github.com/SainsburyWellcomeCentre/WAZP/issues
 Project-URL: Documentation, https://SainsburyWellcomeCentre.github.io/WAZP
 Project-URL: Source code, https://github.com/SainsburyWellcomeCentre/WAZP
```

### Comparing `WAZP-0.1.3/README.md` & `WAZP-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/WAZP.egg-info/PKG-INFO` & `WAZP-0.2.0/WAZP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WAZP
-Version: 0.1.3
+Version: 0.2.0
 Summary: Wasp Animal-tracking Zoo project with Pose estimation
 Author-email: Sofia Miñano <s.minano@ucl.ac.uk>, Nikoloz Sirmpilatze <niko.sirbiladze@gmail.com>, Sam Cunliffe <s.cunliffe@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/SainsburyWellcomeCentre/WAZP
 Project-URL: Bug tracker, https://github.com/SainsburyWellcomeCentre/WAZP/issues
 Project-URL: Documentation, https://SainsburyWellcomeCentre.github.io/WAZP
 Project-URL: Source code, https://github.com/SainsburyWellcomeCentre/WAZP
```

### Comparing `WAZP-0.1.3/WAZP.egg-info/SOURCES.txt` & `WAZP-0.2.0/WAZP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/pyproject.toml` & `WAZP-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
   "pillow",
   "pandas",
   "dash",
   "dash-bootstrap-components",
   "opencv-python",
   "PyYAML",
   "shapely",
+  "openpyxl",
+  "defusedxml"
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
```

### Comparing `WAZP-0.1.3/sample_project/input_config.yaml` & `WAZP-0.2.0/sample_project/input_config.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/metadata_fields.yaml` & `WAZP-0.2.0/sample_project/metadata_fields.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/tests/test_integration/test_smoke.py` & `WAZP-0.2.0/tests/test_integration/test_smoke.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/tests/test_unit/test_utils.py` & `WAZP-0.2.0/tests/test_unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/app.py` & `WAZP-0.2.0/wazp/app.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/callbacks/dashboard.py` & `WAZP-0.2.0/wazp/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/callbacks/home.py` & `WAZP-0.2.0/wazp/callbacks/home.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     """
 
     @app.callback(
         Output("session-storage", "data"),
         Output("upload-message", "is_open"),
         Output("upload-message", "children"),
         Output("upload-message", "color"),
-        Input("upload-data", "contents"),
-        State("upload-data", "filename"),
+        Input("upload-project-config", "contents"),
+        State("upload-project-config", "filename"),
         State("upload-message", "is_open"),
     )
     def save_input_config_to_storage(
         up_content: str, up_filename: str, up_message_state: bool
     ) -> tuple[dict[Any, Any], bool, str, str]:
         """Save project configuration file to temporary memory storage for the current session.
```

### Comparing `WAZP-0.1.3/wazp/callbacks/roi.py` & `WAZP-0.2.0/wazp/callbacks/roi.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/pages/02_ROI.py` & `WAZP-0.2.0/wazp/pages/02_ROI.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/pages/04_dashboard.py` & `WAZP-0.2.0/wazp/pages/04_dashboard.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.1.3/wazp/pages/home.py` & `WAZP-0.2.0/wazp/pages/home.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dash.register_page(__name__, path="/")
 
 ###############
 # Components
 ################
 # Upload component for project config
 upload_component = dcc.Upload(
-    id="upload-data",
+    id="upload-project-config",
     children=html.Div(
         ["Drag and Drop or ", html.A("Select project config file")]
     ),
     contents=None,
     style={
         "width": "100%",
         "height": "60px",
```

### Comparing `WAZP-0.1.3/wazp/utils.py` & `WAZP-0.2.0/wazp/utils.py`

 * *Files identical despite different names*

