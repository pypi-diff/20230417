# Comparing `tmp/dandi-0.8.0.tar.gz` & `tmp/dandi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dandi-cli/dandi-cli/dist/tmp4muxg8ke/dandi-0.8.0.tar", last modified: Tue Dec  1 15:09:54 2020, max compression
+gzip compressed data, was "/home/runner/work/dandi-cli/dandi-cli/dist/tmpa9gn047w/dandi-0.9.0.tar", last modified: Fri Dec  4 15:26:40 2020, max compression
```

## Comparing `dandi-0.8.0.tar` & `dandi-0.9.0.tar`

### file list

```diff
@@ -1,86 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)      303 2020-12-01 15:09:43.000000 dandi-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1796 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5355 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3491 2020-12-01 15:09:43.000000 dandi-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      200 2020-12-01 15:09:43.000000 dandi-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2044 2020-12-01 15:09:54.000000 dandi-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)    69489 2020-12-01 15:09:43.000000 dandi-0.8.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/
--rw-r--r--   0 runner    (1001) docker     (116)    11301 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/pynwb_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1552 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2018 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/due.py
--rw-r--r--   0 runner    (1001) docker     (116)     2729 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)    17309 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/model_types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     3051 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_download.py
--rw-r--r--   0 runner    (1001) docker     (116)     2767 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (116)     1172 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_register.py
--rw-r--r--   0 runner    (1001) docker     (116)     3651 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     9382 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_ls.py
--rw-r--r--   0 runner    (1001) docker     (116)    13980 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_organize.py
--rw-r--r--   0 runner    (1001) docker     (116)      596 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3386 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)     2632 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/cmd_validate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1477 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2068 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/cli/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (116)     3979 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/consts.py
--rw-r--r--   0 runner    (1001) docker     (116)     1275 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/support/
--rw-r--r--   0 runner    (1001) docker     (116)     4008 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/iterators.py
--rw-r--r--   0 runner    (1001) docker     (116)     3954 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/generatorify.py
--rw-r--r--   0 runner    (1001) docker     (116)       76 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2244 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/digests.py
--rw-r--r--   0 runner    (1001) docker     (116)      514 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/ui.py
--rw-r--r--   0 runner    (1001) docker     (116)     4780 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     6311 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/pyout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/support/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     6422 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     1935 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/tests/test_digests.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2103 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/tests/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (116)     2376 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/support/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (116)    13066 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/dandiapi.py
--rw-r--r--   0 runner    (1001) docker     (116)    15107 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/dandiarchive.py
--rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/register.py
--rw-r--r--   0 runner    (1001) docker     (116)     2054 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/validate.py
--rw-r--r--   0 runner    (1001) docker     (116)    17848 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    20690 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/models.py
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)    21976 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/download.py
--rw-r--r--   0 runner    (1001) docker     (116)     3734 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/dandiset.py
--rw-r--r--   0 runner    (1001) docker     (116)    21320 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/organize.py
--rw-r--r--   0 runner    (1001) docker     (116)    35242 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/girder.py
--rw-r--r--   0 runner    (1001) docker     (116)    22436 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/upload.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     8777 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_organize.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:54.000000 dandi-0.8.0/dandi/tests/data/dandiarchive-docker/
--rw-r--r--   0 runner    (1001) docker     (116)     3819 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/data/dandiarchive-docker/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (116)     9853 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6370 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6877 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (116)     4457 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_dandiarchive.py
--rw-r--r--   0 runner    (1001) docker     (116)     6653 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/skip.py
--rw-r--r--   0 runner    (1001) docker     (116)     1101 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (116)    10095 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)     2226 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_pynwb_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4699 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (116)    11725 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_girder.py
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)      933 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (116)      250 2020-12-01 15:09:43.000000 dandi-0.8.0/dandi/tests/test_dandiset.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1611 2020-12-01 15:09:43.000000 dandi-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     5355 2020-12-01 15:09:54.000000 dandi-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/
+-rw-r--r--   0 runner    (1001) docker     (116)    35249 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/girder.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16457 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2018 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/due.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3734 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/dandiset.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17848 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1275 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22698 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)     3051 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_download.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3386 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_upload.py
+-rw-r--r--   0 runner    (1001) docker     (116)      596 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13980 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_organize.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1001 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2068 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1989 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3651 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9879 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2767 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1172 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_register.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2632 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/cmd_validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1513 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/cli/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_dandiset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1122 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2226 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_pynwb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8777 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_organize.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1101 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11695 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_girder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9853 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4457 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_dandiarchive.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/tests/data/dandiarchive-docker/
+-rw-r--r--   0 runner    (1001) docker     (116)     3819 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/data/dandiarchive-docker/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     6653 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/skip.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33960 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4744 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6370 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10095 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6877 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3979 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/support/
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/support/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6422 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1935 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/tests/test_digests.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2103 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/tests/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3954 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/generatorify.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4008 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2244 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/digests.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4780 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6311 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/support/pyout.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21976 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/download.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21320 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/organize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/register.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17309 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/model_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2560 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13066 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/dandiapi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1552 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11481 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/pynwb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15107 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/dandiarchive.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22899 2020-12-04 15:26:28.000000 dandi-0.9.0/dandi/upload.py
+-rw-r--r--   0 runner    (1001) docker     (116)    69489 2020-12-04 15:26:28.000000 dandi-0.9.0/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      303 2020-12-04 15:26:28.000000 dandi-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     2089 2020-12-04 15:26:40.000000 dandi-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      200 2020-12-04 15:26:28.000000 dandi-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     3491 2020-12-04 15:26:28.000000 dandi-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)     1774 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      577 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     5405 2020-12-04 15:26:40.000000 dandi-0.9.0/dandi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5405 2020-12-04 15:26:40.000000 dandi-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1611 2020-12-04 15:26:28.000000 dandi-0.9.0/setup.py
```

### Comparing `dandi-0.8.0/dandi.egg-info/requires.txt` & `dandi-0.9.0/dandi.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 click-didyoumean
 email-validator
 etelemetry>=0.2.0
 fasteners
 joblib
 pycryptodomex
 pydantic
-pyout!=0.6.0
+pyout!=0.6.0,>=0.5
 humanize
 requests~=2.20
 ruamel.yaml<1,>=0.15
 keyring
 keyrings.alt
 python-dateutil
 semantic-version
```

### Comparing `dandi-0.8.0/dandi.egg-info/SOURCES.txt` & `dandi-0.9.0/dandi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,28 +47,27 @@
 dandi/cli/tests/test_ls.py
 dandi/support/__init__.py
 dandi/support/cache.py
 dandi/support/digests.py
 dandi/support/generatorify.py
 dandi/support/iterators.py
 dandi/support/pyout.py
-dandi/support/ui.py
 dandi/support/tests/__init__.py
 dandi/support/tests/test_cache.py
 dandi/support/tests/test_digests.py
 dandi/support/tests/test_iterators.py
-dandi/support/tests/test_ui.py
 dandi/tests/__init__.py
 dandi/tests/fixtures.py
 dandi/tests/skip.py
 dandi/tests/test_dandiarchive.py
 dandi/tests/test_dandiset.py
 dandi/tests/test_download.py
 dandi/tests/test_fixtures.py
 dandi/tests/test_girder.py
+dandi/tests/test_metadata.py
 dandi/tests/test_models.py
 dandi/tests/test_organize.py
 dandi/tests/test_pynwb_utils.py
 dandi/tests/test_register.py
 dandi/tests/test_upload.py
 dandi/tests/test_utils.py
 dandi/tests/test_validate.py
```

### Comparing `dandi-0.8.0/dandi.egg-info/PKG-INFO` & `dandi-0.9.0/dandi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandi
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line client for interaction with DANDI archive elements
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
@@ -109,14 +109,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Provides: dandi
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: extensions
 Provides-Extra: extras
 Provides-Extra: style
```

### Comparing `dandi-0.8.0/README.md` & `dandi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/setup.cfg` & `dandi-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Topic :: Scientific/Engineering
 license = Apache 2.0
 description = Command line client for interaction with DANDI archive elements
 long_description = file:README.md
 long_description_content_type = text/markdown; charset=UTF-8
 platforms = OS Independent
 provides = 
@@ -36,15 +37,15 @@
 	click-didyoumean
 	email-validator
 	etelemetry >= 0.2.0
 	fasteners
 	joblib
 	pycryptodomex  # for EncryptedKeyring backend in keyrings.alt
 	pydantic
-	pyout != 0.6.0
+	pyout >=0.5, !=0.6.0
 	humanize
 	requests ~= 2.20
 	ruamel.yaml >=0.15, <1
 	keyring
 	keyrings.alt
 	python-dateutil
 	semantic-version
```

### Comparing `dandi-0.8.0/versioneer.py` & `dandi-0.9.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/pynwb_utils.py` & `dandi-0.9.0/dandi/pynwb_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     if isinstance(v, str) and not semantic_version.validate(v):
         msgtype = "error" if LooseVersion(v) >= "2.1.0" else "warning"
         log(f"{msgtype}: {msg} is not a proper semantic version. See http://semver.org")
 
     return v
 
 
-def get_nwb_version(filepath, sanitize=True):
+def get_nwb_version(filepath, sanitize=False):
     """Return a version of the NWB standard used by a file
 
     Parameters
     ----------
     sanitize: bool, optional
       Either to sanitize version and return it non-raw where we detect version
       which does not follow semantic but we possibly can handle
@@ -269,21 +269,28 @@
 
 # Many commands might be using load_namespaces but it causes HDMF to whine if there
 # is no cached name spaces in the file.  It is benign but not really useful
 # at this point, so we ignore it although ideally there should be a formal
 # way to get relevant warnings (not errors) from PyNWB.  It is a bad manner
 # to have this as a side effect of the importing this module, we should add/remove
 # that filter in our top level commands
+_ignored_benign_pynwb_warnings = False
+
+
 def ignore_benign_pynwb_warnings():
+    global _ignored_benign_pynwb_warnings
+    if _ignored_benign_pynwb_warnings:
+        return
     #   See https://github.com/dandi/dandi-cli/issues/14 for more info
     for s in (
         "No cached namespaces found .*",
         "ignoring namespace '.*' because it already exists",
     ):
         warnings.filterwarnings("ignore", s, UserWarning)
+    _ignored_benign_pynwb_warnings = True
 
 
 def get_object_id(path):
     """Read, if present an object_id
 
     if not available -- would simply raise a corresponding exception
     """
```

### Comparing `dandi-0.8.0/dandi/exceptions.py` & `dandi-0.9.0/dandi/exceptions.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/due.py` & `dandi-0.9.0/dandi/due.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/model_types.py` & `dandi-0.9.0/dandi/model_types.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/cmd_download.py` & `dandi-0.9.0/dandi/cli/cmd_download.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/command.py` & `dandi-0.9.0/dandi/cli/command.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/cmd_register.py` & `dandi-0.9.0/dandi/cli/cmd_register.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/base.py` & `dandi-0.9.0/dandi/cli/base.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/cmd_ls.py` & `dandi-0.9.0/dandi/cli/cmd_ls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import os.path as op
-import time
 
 import click
 
 from collections import defaultdict
 
 from .base import lgr, map_to_click_exceptions
 
-from ..utils import safe_call
 
 # TODO: all the recursion options etc
 
 
 @click.command()
 @click.option(
     "-F",
@@ -32,17 +30,24 @@
 @click.option(
     "-r",
     "--recursive",
     help="Recurse into content of dandisets/directories. Only .nwb files will "
     "be considered.",
     is_flag=True,
 )
+@click.option(
+    "-J",
+    "--jobs",
+    help="Number of parallel download jobs.",
+    default=6,  # TODO: come up with smart auto-scaling etc
+    show_default=True,
+)
 @click.argument("paths", nargs=-1, type=click.Path(exists=False, dir_okay=True))
 @map_to_click_exceptions
-def ls(paths, fields=None, format="auto", recursive=False):
+def ls(paths, fields=None, format="auto", recursive=False, jobs=6):
     """List .nwb files and dandisets metadata.
     """
     from ..consts import metadata_all_fields
 
     # TODO: more logical ordering in case of fields = None
     from .formatter import JSONFormatter, YAMLFormatter, PYOUTFormatter
 
@@ -100,77 +105,83 @@
     if format == "auto":
         format = "yaml" if any(urls) or (len(paths) == 1 and not recursive) else "pyout"
 
     if format == "pyout":
         if fields and fields[0] != "path":
             # we must always have path - our "id"
             fields = ["path"] + fields
-        out = PYOUTFormatter(fields=fields)
+        out = PYOUTFormatter(fields=fields, wait_for_top=3, max_workers=jobs)
     elif format == "json":
         out = JSONFormatter()
     elif format == "json_pp":
         out = JSONFormatter(indent=2)
     elif format == "yaml":
         out = YAMLFormatter()
     else:
         raise NotImplementedError("Unknown format %s" % format)
 
     async_keys = set(all_fields)
     if fields is not None:
         async_keys = async_keys.intersection(fields)
     async_keys = tuple(async_keys.difference(common_fields))
 
-    process_assets = set()
     errors = defaultdict(list)  # problem: [] paths
     with out:
         for asset in assets_gen():
-            while len(process_assets) >= 10:
-                lgr.log(2, "Sleep waiting for some paths to finish processing")
-                time.sleep(0.5)
-
             if isinstance(asset, str):  # path
-                process_assets.add(asset)
                 rec = {}
                 rec["path"] = asset
 
                 try:
                     if (not fields or "size" in fields) and not op.isdir(asset):
                         rec["size"] = os.stat(asset).st_size
 
                     if async_keys:
-                        cb = get_metadata_pyout(
-                            asset, async_keys, process_assets, flatten=format == "pyout"
+                        cb = get_metadata_ls(
+                            asset, async_keys, errors=errors, flatten=format == "pyout"
                         )
                         if format == "pyout":
                             rec[async_keys] = cb
                         else:
                             # TODO: parallel execution
                             # For now just call callback and get all the fields
-                            for k, v in cb().items():
+                            cb_res = cb()
+                            # TODO: we should stop masking exceptions in get_metadata_ls,
+                            # and centralize logic regardless either it is for pyout or not
+                            # and do parallelizaion on our end, so at large it is
+                            if cb_res is None:
+                                raise
+                            for k, v in cb_res.items():
                                 rec[k] = v
                 except Exception as exc:
-                    lgr.debug("Problem obtaining metadata for %s: %s", asset, exc)
-                    errors[str(type(exc).__name__)].append(asset)
+                    _add_exc_error(asset, rec, errors, exc)
             elif isinstance(asset, dict):
                 # ready record
                 # TODO: harmonization for pyout
                 rec = asset
             else:
                 raise TypeError(asset)
 
             if not rec:
                 errors["Empty record"].append(asset)
                 lgr.debug("Skipping a record for %s since empty", asset)
                 continue
             out(rec)
-        if errors:
-            lgr.warning(
-                "Failed to operate on some paths (empty records were listed):\n %s",
-                "\n ".join("%s: %d paths" % (k, len(v)) for k, v in errors.items()),
-            )
+    if errors:
+        lgr.warning(
+            "Failed to operate on some paths (empty records were listed):\n %s",
+            "\n ".join("%s: %d paths" % (k, len(v)) for k, v in errors.items()),
+        )
+
+
+def _add_exc_error(asset, rec, errors, exc):
+    """A helper to centralize collection of errors for pyout and non-pyout reporting"""
+    lgr.debug("Problem obtaining metadata for %s: %s", asset, exc)
+    errors[str(type(exc).__name__)].append(asset)
+    rec["errors"] = rec.get("errors", 0) + 1
 
 
 def display_known_fields(all_fields):
     from ..support.pyout import PYOUT_SHORT_NAMES
 
     # Display all known fields
     click.secho("Known fields:")
@@ -244,43 +255,46 @@
     for f, v in (meta or dict()).items():
         if not v:
             continue
         out[f] = flatten_v(v)
     return out
 
 
-def get_metadata_pyout(path, keys=None, process_paths=None, flatten=False):
+def get_metadata_ls(path, keys, errors, flatten=False):
     from ..pynwb_utils import get_nwb_version, ignore_benign_pynwb_warnings
     from ..metadata import get_metadata
 
     ignore_benign_pynwb_warnings()
 
     def fn():
         try:
             rec = {}
             # No need for calling get_metadata if no keys are needed from it
             if keys is None or list(keys) != ["nwb_version"]:
-                rec = safe_call(get_metadata, path)
+                try:
+                    rec = get_metadata(path)
+                except Exception as exc:
+                    _add_exc_error(path, rec, errors, exc)
                 if flatten:
                     rec = flatten_meta_to_pyout(rec)
             if keys is not None:
                 rec = {k: v for k, v in rec.items() if k in keys}
             if (
                 not op.isdir(path)
                 and "nwb_version" not in rec
                 and (keys and "nwb_version" in keys)
             ):
                 # Let's at least get that one
-                rec["nwb_version"] = safe_call(get_nwb_version, path, "ERROR") or ""
+                try:
+                    rec["nwb_version"] = get_nwb_version(path)
+                except Exception as exc:
+                    _add_exc_error(path, rec, errors, exc)
             return rec
         finally:
-            # TODO: this is a workaround, remove after
-            # https://github.com/pyout/pyout/issues/87 is resolved
-            if process_paths is not None and path in process_paths:
-                process_paths.remove(path)
+            pass
 
     return fn
 
 
 def is_url(s):
     """Very primitive url detection for now
```

### Comparing `dandi-0.8.0/dandi/cli/cmd_organize.py` & `dandi-0.9.0/dandi/cli/cmd_organize.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/__init__.py` & `dandi-0.9.0/dandi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/cmd_upload.py` & `dandi-0.9.0/dandi/cli/cmd_upload.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/cmd_validate.py` & `dandi-0.9.0/dandi/cli/cmd_validate.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/formatter.py` & `dandi-0.9.0/dandi/cli/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         yaml.dump(self.records, self.out)
 
     def __call__(self, rec):
         self.records.append(rec)
 
 
 class PYOUTFormatter(pyout.Tabular):
-    def __init__(self, fields):
+    def __init__(self, fields, **kwargs):
         PYOUT_STYLE = pyouts.get_style(hide_if_missing=not fields)
 
         kw = dict(style=PYOUT_STYLE)
+        kw.update(kwargs)
         if fields:
             kw["columns"] = fields
         super().__init__(**kw)
```

### Comparing `dandi-0.8.0/dandi/cli/tests/test_command.py` & `dandi-0.9.0/dandi/cli/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/tests/test_download.py` & `dandi-0.9.0/dandi/cli/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/cli/tests/test_ls.py` & `dandi-0.9.0/dandi/cli/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/consts.py` & `dandi-0.9.0/dandi/consts.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/__init__.py` & `dandi-0.9.0/dandi/__init__.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/iterators.py` & `dandi-0.9.0/dandi/support/iterators.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/generatorify.py` & `dandi-0.9.0/dandi/support/generatorify.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/digests.py` & `dandi-0.9.0/dandi/support/digests.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/cache.py` & `dandi-0.9.0/dandi/support/cache.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/pyout.py` & `dandi-0.9.0/dandi/support/pyout.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/tests/test_cache.py` & `dandi-0.9.0/dandi/support/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/tests/test_digests.py` & `dandi-0.9.0/dandi/support/tests/test_digests.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/support/tests/test_iterators.py` & `dandi-0.9.0/dandi/support/tests/test_iterators.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/dandiapi.py` & `dandi-0.9.0/dandi/dandiapi.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/dandiarchive.py` & `dandi-0.9.0/dandi/dandiarchive.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/register.py` & `dandi-0.9.0/dandi/register.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/validate.py` & `dandi-0.9.0/dandi/validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import os
 import os.path as op
 from .consts import dandiset_metadata_file
-
+from .metadata import get_metadata
 from .pynwb_utils import validate as pynwb_validate, validate_cache
 from .utils import find_dandi_files, yaml_load
-from .metadata import get_metadata
 
 
 # TODO -- should come from schema.  This is just a simplistic example for now
 _required_dandiset_metadata_fields = ["identifier", "name", "description"]
 _required_nwb_metadata_fields = ["subject_id"]
 
 
@@ -44,20 +44,34 @@
         meta = yaml_load(f, typ="safe")
     return _check_required_fields(meta, _required_dandiset_metadata_fields)
 
 
 def validate_dandi_nwb(filepath):
     """Provide validation of .nwb file regarding requirements we impose
     """
-    # make sure that we have some basic metadata fields we require
-    try:
-        meta = get_metadata(filepath)
-    except BaseException as e:
-        return [f"Failed to read metadata: {e}"]
-    return _check_required_fields(meta, _required_nwb_metadata_fields)
+    if os.environ.get("DANDI_SCHEMA"):
+        from pydantic import ValidationError
+        from .metadata import nwb2asset
+        from .models import AssetMeta
+
+        try:
+            asset = nwb2asset(filepath, digest="dummy_value", digest_type="sha1")
+            AssetMeta(**asset.dict())
+        except ValidationError as e:
+            return [str(e)]
+        except Exception as e:
+            return [f"Failed to read metadata: {e}"]
+        return []
+    else:
+        # make sure that we have some basic metadata fields we require
+        try:
+            meta = get_metadata(filepath)
+        except BaseException as e:
+            return [f"Failed to read metadata: {e}"]
+        return _check_required_fields(meta, _required_nwb_metadata_fields)
 
 
 def _check_required_fields(d, required):
     errors = []
     for f in required:
         v = d.get(f, None)
         if not v or (isinstance(v, str) and not (v.strip())):
```

### Comparing `dandi-0.8.0/dandi/utils.py` & `dandi-0.9.0/dandi/utils.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/models.py` & `dandi-0.9.0/dandi/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         fp.write("# AUTOGENERATED - DO NOT EDIT\n")
         yaml.safe_dump(jsonld_doc, fp, indent=2)
     return jsonld_doc
 
 
 AccessType = create_enum(AccessTypeDict)
 RoleType = create_enum(RoleTypeDict)
-Relation = create_enum(RelationTypeDict)
-License = create_enum(LicenseTypeDict)
+RelationType = create_enum(RelationTypeDict)
+LicenseType = create_enum(LicenseTypeDict)
 IdentifierType = create_enum(IdentifierTypeDict)
 DigestType = create_enum(DigestTypeDict)
 
 
 class DandiBaseModel(BaseModel):
     @classmethod
     def unvalidated(__pydantic_cls__: Type[BaseModel], **data: Any) -> BaseModel:
@@ -121,38 +121,44 @@
             __pydantic_cls__.unvalidated()
             .__repr__()
             .replace(__pydantic_cls__.__name__, "dict")
         )
 
 
 class PropertyValue(DandiBaseModel):
-    maxValue: float = Field(None, nskey="schema")
-    minValue: float = Field(None, nskey="schema")
-    unitCode: Union[str, AnyUrl] = Field(None, nskey="schema")
-    unitText: str = Field(None, nskey="schema")
-    value: Union[bool, float, str, int, List[Union[bool, float, str, int]]] = Field(
+    maxValue: float = Field(None, title="Max Value", nskey="schema")
+    minValue: float = Field(None, title="Min Value", nskey="schema")
+    unitCode: Union[str, AnyUrl] = Field(None, title="Unit Code", nskey="schema")
+    unitText: str = Field(None, title="Unit Text", nskey="schema")
+    value: Union[str, bool, int, float, List[Union[str, bool, int, float]]] = Field(
         None, nskey="schema"
     )
     valueReference: "PropertyValue" = Field(
-        None, nskey="schema"
+        None, title="Value Reference", nskey="schema"
     )  # Note: recursive (circular or not)
-    propertyID: Union[IdentifierType, AnyUrl, str] = Field(None, nskey="schema")
+    propertyID: Union[IdentifierType, AnyUrl, str] = Field(
+        None,
+        title="Property ID",
+        description="A commonly used identifier for"
+        "the characteristic represented by the property.",
+        nskey="schema",
+    )
 
     _ldmeta = {"nskey": "schema"}
 
 
 PropertyValue.update_forward_refs()
 Identifier = Union[AnyUrl, PropertyValue, str]
 
 
 class TypeModel(DandiBaseModel):
     """Base class for enumerated types"""
 
-    identifier: Identifier = Field(nskey="schema")
-    name: str = Field(
+    identifier: Optional[Identifier] = Field(nskey="schema")
+    name: Optional[str] = Field(
         title="Title",
         description="The name of the item.",
         max_length=150,
         nskey="schema",
     )
 
     _ldmeta = {"rdfs:subClassOf": ["prov:Entity", "schema:Thing"], "nskey": "dandi"}
@@ -207,37 +213,46 @@
     email: Optional[EmailStr] = Field(None, nskey="schema")
     url: Optional[AnyUrl] = Field(None, nskey="schema")
 
     _ldmeta = {"nskey": "schema"}
 
 
 class Contributor(DandiBaseModel):
-    identifier: Identifier = Field(None, nskey="schema")
+    identifier: Identifier = Field(
+        None,
+        title="A Common Identifier",
+        description="Use a common identifier such as ORCID for people or ROR for institutions",
+        nskey="schema",
+    )
     name: str = Field(None, nskey="schema")
     email: EmailStr = Field(None, nskey="schema")
     url: AnyUrl = Field(None, nskey="schema")
-    roleName: List[RoleType] = Field(nskey="schema")
+    roleName: List[RoleType] = Field(
+        title="Role", description="Role of the contributor", nskey="schema"
+    )
     includeInCitation: bool = Field(
         True,
-        title="Include contributor in citation",
+        title="Include Contributor in Citation",
         description="A flag to indicate whether a contributor should be included "
         "when generating a citation for the item",
         nskey="dandi",
     )
     awardNumber: Identifier = Field(
         None,
         title="Identifier for an award",
         description="Identifier associated with a sponsored or gidt award",
         nskey="dandi",
     )
 
 
 class Organization(Contributor):
     contactPoint: List[ContactPoint] = Field(
-        description="Contact for the organization", nskey="schema"
+        title="Contact Point",
+        description="Contact for the organization",
+        nskey="schema",
     )
     _ldmeta = {
         "rdfs:subClassOf": ["schema:Organization", "prov:Organization"],
         "nskey": "dandi",
     }
 
 
@@ -260,32 +275,37 @@
     name: str = Field(nskey="schema")
     version: str = Field(nskey="schema")
 
 
 class EthicsApproval(DandiBaseModel):
     """Information about ethics committee approval for project"""
 
-    identifier: Identifier = Field(nskey="schema")
+    identifier: Identifier = Field(
+        nskey="schema", title="Identifier String for Approved Protocol"
+    )
     contactPoint: ContactPoint = Field(
-        description="Information about the ethics approval committee.", nskey="schema"
+        title="Contact Point",
+        description="Information about the ethics approval committee.",
+        nskey="schema",
     )
 
     _ldmeta = {"rdfs:subClassOf": ["schema:Thing", "prov:Entity"], "nskey": "dandi"}
 
 
 class Resource(DandiBaseModel):
     identifier: Identifier = Field(None, nskey="schema")
     name: str = Field(None, nskey="schema")
     url: str = Field(None, nskey="schema")
     repository: Union[str, AnyUrl] = Field(
         None,
         description="An identifier of a repository in which the resource is housed",
         nskey="dandi",
     )
-    relation: Relation = Field(
+    relation: RelationType = Field(
+        title="Relation",
         description="Indicates how the resource is related to the dataset",
         nskey="dandi",
     )
 
     _ldmeta = {
         "rdfs:subClassOf": ["schema:CreativeWork", "prov:Entity"],
         "rdfs:comment": "A resource related to the project (e.g., another "
@@ -299,15 +319,17 @@
 
     status: AccessType = Field(
         title="Access status",
         description="The access status of the item",
         nskey="dandi",
     )
     email: Optional[EmailStr] = Field(None, nskey="schema")
-    contactPoint: Optional[ContactPoint] = Field(None, nskey="schema")
+    contactPoint: Optional[ContactPoint] = Field(
+        None, title="Contact Point", nskey="schema"
+    )
     description: Optional[str] = Field(
         None,
         title="Description",
         description="A description of the item.",
         nskey="schema",
     )
     embargoedUntil: Optional[date] = Field(
@@ -322,46 +344,56 @@
     _ldmeta = {"rdfs:subClassOf": ["schema:Thing", "prov:Entity"], "nskey": "dandi"}
 
 
 class AssetsSummary(DandiBaseModel):
     """Summary over assets contained in a dandiset (published or not)"""
 
     # stats which are not stats
-    numberOfBytes: int = Field(readOnly=True, sameas="schema:contentSize")
-    numberOfFiles: int = Field(readOnly=True)  # universe
-    numberOfSubjects: int = Field(readOnly=True)  # NWB + BIDS
-    numberOfSamples: Optional[int] = Field(None, readOnly=True)  # more of NWB
-    numberOfCells: Optional[int] = Field(None, readOnly=True)
+    numberOfBytes: int = Field(
+        title="Number of Bytes", readOnly=True, sameas="schema:contentSize"
+    )
+    numberOfFiles: int = Field(title="Number of Files", readOnly=True)  # universe
+    numberOfSubjects: int = Field(
+        title="Number of Subjects", readOnly=True
+    )  # NWB + BIDS
+    numberOfSamples: Optional[int] = Field(
+        None, title="Number of Samples", readOnly=True
+    )  # more of NWB
+    numberOfCells: Optional[int] = Field(None, title="Number of Cells", readOnly=True)
 
     dataStandard: List[StandardsType] = Field(
-        readOnly=True
+        title="Data Standard", readOnly=True
     )  # TODO: types of things NWB, BIDS
     # Web UI: icons per each modality?
     modality: List[ModalityType] = Field(
         readOnly=True
     )  # TODO: types of things, BIDS etc...
     # Web UI: could be an icon with number, which if hovered on  show a list?
-    measurementTechnique: List[MeasurementTechniqueType] = Field(readOnly=True)
-    variableMeasured: Optional[List[PropertyValue]] = Field(None, readOnly=True)
+    measurementTechnique: List[MeasurementTechniqueType] = Field(
+        title="Measurement Technique", readOnly=True
+    )
+    variableMeasured: Optional[List[PropertyValue]] = Field(
+        None, title="Variable Measured", readOnly=True
+    )
 
     species: List[SpeciesType] = Field(readOnly=True)
 
     _ldmeta = {
         "rdfs:subClassOf": ["schema:CreativeWork", "prov:Entity"],
         "nskey": "dandi",
     }
 
 
 class Digest(DandiBaseModel):
     """Information about the crytographic checksum of the item."""
 
     value: str = Field(nskey="schema")
     cryptoType: DigestType = Field(
-        description="Which cryptographic checksum is used",
         title="Cryptographic method used",
+        description="Which cryptographic checksum is used",
         nskey="dandi",
     )
 
     _ldmeta = {
         "rdfs:subClassOf": ["schema:Thing", "prov:Entity"],
         "rdfs:label": "Cryptographic checksum information",
         "nskey": "dandi",
@@ -369,26 +401,32 @@
 
 
 class BioSample(DandiBaseModel):
     """Description about the sample that was studied"""
 
     identifier: Identifier = Field(nskey="schema")
     assayType: Optional[List[AssayType]] = Field(
-        None, description="OBI based identifier for the assay(s) used", nskey="dandi"
+        None,
+        title="Assay Type",
+        description="OBI based identifier for the assay(s) used",
+        nskey="dandi",
     )
     anatomy: Optional[List[Anatomy]] = Field(
         None,
         description="UBERON based identifier for the location of the sample",
         nskey="dandi",
     )
     strain: Optional[StrainType] = Field(
         None, description="Identifier for the strain of the sample", nskey="dandi"
     )
     cellLine: Optional[Identifier] = Field(
-        None, description="Cell line associated with the sample", nskey="dandi"
+        None,
+        title="Cell Line",
+        description="Cell line associated with the sample",
+        nskey="dandi",
     )
     vendor: Optional[Organization] = Field(None, nskey="dandi")
     age: Optional[PropertyValue] = Field(
         None,
         description="A representation of age using ISO 8601 duration. This "
         "should include a valueReference if anything other than "
         "date of birth is used.",
@@ -433,35 +471,37 @@
     )
     description: Optional[str] = Field(
         None,
         title="Description",
         description="A description of the item.",
         nskey="schema",
     )
-    startDate: Optional[date] = Field(None, nskey="schema")
-    endDate: Optional[date] = Field(None, nskey="schema")
+    startDate: Optional[date] = Field(None, title="Start Date", nskey="schema")
+    endDate: Optional[date] = Field(None, title="End Date", nskey="schema")
 
-    isPartOf: Optional["Activity"] = Field(None, nskey="schema")
-    hasPart: Optional["Activity"] = Field(None, nskey="schema")
+    isPartOf: Optional["Activity"] = Field(None, title="Is Part Of", nskey="schema")
+    hasPart: Optional["Activity"] = Field(None, title="Has Part", nskey="schema")
     wasAssociatedWith: Optional[Union[Person, Organization, Software]] = Field(
-        None, nskey="prov"
+        None, title="Was Associated With", nskey="prov"
     )
 
     _ldmeta = {"rdfs:subClassOf": ["prov:Activity", "schema:Thing"], "nskey": "dandi"}
 
 
 Activity.update_forward_refs()
 
 
 class Project(Activity):
     pass
 
 
 class CommonModel(DandiBaseModel):
-    schemaVersion: str = Field(default="1.0.0-rc1", readOnly=True, nskey="schema")
+    schemaVersion: str = Field(
+        default="1.0.0-rc1", title="Schema Version", readOnly=True, nskey="schema"
+    )
     identifier: Identifier = Field(readOnly=True, nskey="schema")
     name: Optional[str] = Field(
         None,
         title="Title",
         description="The name of the item.",
         max_length=150,
         nskey="schema",
@@ -476,53 +516,63 @@
         None,
         title="Contributors",
         description="Contributors to this item.",
         nskey="schema",
     )
     about: Optional[List[Union[Disorder, Anatomy, Identifier]]] = Field(
         None,
-        title="Subject matter",
+        title="Subject Matter",
         description="The subject matter of the content, such as disorders, brain anatomy.",
         nskey="schema",
     )
     studyTarget: Optional[List[Union[str, AnyUrl]]] = Field(
-        None, title="What the study is related to", nskey="dandi"
+        None,
+        title="Study Target",
+        description="What the study is related to",
+        nskey="dandi",
+    )
+    license: List[LicenseType] = Field(
+        title="License", description="License of item.", nskey="schema"
     )
     protocol: Optional[List[str]] = Field(None, nskey="dandi")
-    ethicsApproval: Optional[List[EthicsApproval]] = Field(None, nskey="dandi")
-    license: List[License] = Field(nskey="schema")
+    ethicsApproval: Optional[List[EthicsApproval]] = Field(
+        None, title="Ethics Approval", nskey="dandi"
+    )
     keywords: Optional[List[str]] = Field(
         None,
         title="Keywords",
         description="Keywords or tags used to describe "
         "this content. Multiple entries in a "
         "keywords list are typically delimited "
         "by commas.",
         nskey="schema",
     )
     acknowledgement: Optional[str] = Field(None, title="Acknowledgement", nskey="dandi")
 
     # Linking to this dandiset or the larger thing
     access: List[AccessRequirements] = Field(
+        title="Access Type",
         default_factory=lambda: [AccessRequirements(status=AccessType.Open)],
         nskey="dandi",
     )
     url: Optional[AnyUrl] = Field(
         None, readOnly=True, description="permalink to the item", nskey="schema"
     )
     repository: AnyUrl = Field(
         "https://dandiarchive.org/",
         readOnly=True,
         description="location of the item",
         nskey="dandi",
     )
-    relatedResource: Optional[List[Resource]] = Field(None, nskey="dandi")
+    relatedResource: Optional[List[Resource]] = Field(
+        None, title="Related Resource", nskey="dandi"
+    )
 
     wasGeneratedBy: Optional[Union[Activity, AnyUrl]] = Field(
-        None, readOnly=True, nskey="prov"
+        None, title="Was Generated By", readOnly=True, nskey="prov"
     )
 
 
 class DandiMeta(CommonModel):
     """A body of structured information describing a DANDI dataset."""
 
     @validator("contributor")
@@ -554,83 +604,99 @@
         nskey="schema",
         min_items=1,
     )
 
     citation: str = Field(readOnly=True, nskey="schema")
 
     # From assets
-    assetsSummary: AssetsSummary = Field(readOnly=True, nskey="dandi")
+    assetsSummary: AssetsSummary = Field(
+        title="Assets Summary", readOnly=True, nskey="dandi"
+    )
 
     # From server (requested by users even for drafts)
-    manifestLocation: List[AnyUrl] = Field(readOnly=True, nskey="dandi")
+    manifestLocation: List[AnyUrl] = Field(
+        title="Manifest Location", readOnly=True, nskey="dandi"
+    )
 
     # On publish
     version: str = Field(readOnly=True, nskey="schema")
-    doi: Optional[Union[str, AnyUrl]] = Field(None, readOnly=True, nskey="dandi")
+    doi: Optional[Union[str, AnyUrl]] = Field(
+        None, title="DOI", readOnly=True, nskey="dandi"
+    )
 
     _ldmeta = {
         "rdfs:subClassOf": ["schema:Dataset", "prov:Entity"],
         "rdfs:label": "Information about the dataset",
         "nskey": "dandi",
     }
 
 
 class PublishedDandiMeta(DandiMeta):
     publishedBy: AnyUrl = Field(
+        title="Published By",
         description="The URL should contain the provenance of the publishing process.",
         readOnly=True,
         nskey="dandi",
     )  # TODO: formalize "publish" activity to at least the Actor
-    datePublished: date = Field(readOnly=True, nskey="schema")
+    datePublished: date = Field(title="Date Published", readOnly=True, nskey="schema")
 
 
 class AssetMeta(CommonModel):
     """Metadata used to describe an asset.
 
     Derived from C2M2 (Level 0 and 1) and schema.org
     """
 
     # Overrides CommonModel.license
     # TODO: https://github.com/NeurodataWithoutBorders/nwb-schema/issues/320
-    license: Optional[List[License]] = Field(None, nskey="schema")
+    license: Optional[List[LicenseType]] = Field(
+        None, title="License", description="License of item", nskey="schema"
+    )
 
-    contentSize: str = Field(nskey="schema")
-    encodingFormat: Union[str, AnyUrl] = Field(nskey="schema")
+    contentSize: str = Field(title="Content Size", nskey="schema")
+    encodingFormat: Union[str, AnyUrl] = Field(
+        title="File Encoding Format", nskey="schema"
+    )
     digest: Digest = Field(nskey="dandi")
 
     path: str = Field(None, nskey="dandi")
 
     # this is from C2M2 level 1 - using EDAM vocabularies - in our case we would
     # need to come up with things for neurophys
     # TODO: waiting on input <https://github.com/dandi/dandi-cli/pull/226>
-    dataType: Optional[AnyUrl] = Field(None, nskey="dandi")
+    dataType: Optional[AnyUrl] = Field(None, title="Data Type", nskey="dandi")
 
-    sameAs: Optional[List[AnyUrl]] = Field(None, nskey="schema")
+    sameAs: Optional[List[AnyUrl]] = Field(None, title="Same As", nskey="schema")
 
     # TODO
     modality: Optional[List[ModalityType]] = Field(None, readOnly=True, nskey="dandi")
     measurementTechnique: Optional[List[MeasurementTechniqueType]] = Field(
-        None, readOnly=True, nskey="schema"
+        None, title="Measurement Technique", readOnly=True, nskey="schema"
     )
     variableMeasured: Optional[List[PropertyValue]] = Field(
-        None, readOnly=True, nskey="schema"
+        None, title="Variable Measured", readOnly=True, nskey="schema"
     )
 
-    wasDerivedFrom: Optional[List[BioSample]] = Field(None, nskey="prov")
+    wasDerivedFrom: Optional[List[BioSample]] = Field(
+        None, title="Was Derived From", nskey="prov"
+    )
 
     # on publish or set by server
-    contentUrl: Optional[List[AnyUrl]] = Field(None, readOnly=True, nskey="schema")
+    contentUrl: Optional[List[AnyUrl]] = Field(
+        None, title="Content URL", readOnly=True, nskey="schema"
+    )
 
     _ldmeta = {
         "rdfs:subClassOf": ["schema:CreativeWork", "prov:Entity"],
         "rdfs:label": "Information about the asset",
         "nskey": "dandi",
     }
 
 
 class PublishedAssetMeta(AssetMeta):
     publishedBy: AnyUrl = Field(
+        title="Published By",
         description="The URL should contain the provenance of the publishing process.",
         readOnly=True,
         nskey="dandi",
     )  # TODO: formalize "publish" activity to at least the Actor
-    datePublished: date = Field(readOnly=True, nskey="schema")
+    datePublished: date = Field(title="Date Published", readOnly=True, nskey="schema")
```

### Comparing `dandi-0.8.0/dandi/download.py` & `dandi-0.9.0/dandi/download.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/dandiset.py` & `dandi-0.9.0/dandi/dandiset.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/organize.py` & `dandi-0.9.0/dandi/organize.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/girder.py` & `dandi-0.9.0/dandi/girder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import random
 import sys
 import time
 
 from functools import lru_cache
 from pathlib import Path
 
+import click
 from keyring.core import get_keyring, load_config, load_env
 from keyring.backend import get_all_keyring
 from keyring.errors import KeyringError
 from keyring.util.platform_ import config_root
 from keyrings.alt.file import EncryptedKeyring
 
 import girder_client as gcl
 
 from . import get_logger
 from .exceptions import LockingError
-from .support.ui import askyesno
 from .utils import ensure_datetime, flattened, flatten, remap_dict
 from .consts import known_instances_rev, MAX_CHUNK_SIZE
 
 lgr = get_logger()
 
 
 # TODO: more flexible
@@ -908,15 +908,17 @@
             len(kbs) == 1
         ), "EncryptedKeyring not available; is pycryptodomex installed?"
         kb = kbs[0]
         if op.exists(kb.file_path):
             lgr.info("EncryptedKeyring file exists; using as keyring backend")
             return (kb, kb.get_password(service_name, username))
         lgr.info("EncryptedKeyring file does not exist")
-        if askyesno("Would you like to establish an encrypted keyring?", default=True):
+        if click.confirm(
+            "Would you like to establish an encrypted keyring?", default=True
+        ):
             keyring_cfg = Path(keyringrc_file())
             if keyring_cfg.exists():
                 lgr.info("%s exists; refusing to overwrite", keyring_cfg)
             else:
                 lgr.info(
                     "Configuring %s to use EncryptedKeyring as default backend",
                     keyring_cfg,
```

### Comparing `dandi-0.8.0/dandi/upload.py` & `dandi-0.9.0/dandi/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,22 @@
         # Ensure consistent types
         path = Path(path)
         relpath = PurePosixPath(relpath)
         try:
             try:
                 path_stat = path.stat()
                 yield {"size": path_stat.st_size}
+                size_cut_off = 67108864000
+                if path_stat.st_size > size_cut_off:
+                    raise RuntimeError(
+                        "Too large! We are experiencing problems uploading files larger than %s. "
+                        "See https://github.com/dandi/dandiarchive/issues/517 and update "
+                        "client when the issue is resolved."
+                        % (naturalsize(size_cut_off))
+                    )
             except FileNotFoundError:
                 yield skip_file("ERROR: File not found")
                 return
             except Exception as exc:
                 # without limiting [:50] it might cause some pyout indigestion
                 yield skip_file("ERROR: %s" % str(exc)[:50])
                 return
```

### Comparing `dandi-0.8.0/dandi/tests/test_organize.py` & `dandi-0.9.0/dandi/tests/test_organize.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/data/dandiarchive-docker/docker-compose.yml` & `dandi-0.9.0/dandi/tests/data/dandiarchive-docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_utils.py` & `dandi-0.9.0/dandi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_upload.py` & `dandi-0.9.0/dandi/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_download.py` & `dandi-0.9.0/dandi/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_dandiarchive.py` & `dandi-0.9.0/dandi/tests/test_dandiarchive.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/skip.py` & `dandi-0.9.0/dandi/tests/skip.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_register.py` & `dandi-0.9.0/dandi/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/fixtures.py` & `dandi-0.9.0/dandi/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 @pytest.fixture(scope="session")
 def simple2_nwb(simple1_nwb_metadata, tmpdir_factory):
     """With a subject"""
     return make_nwb_file(
         str(tmpdir_factory.mktemp("data").join("simple2.nwb")),
         subject=pynwb.file.Subject(
             subject_id="mouse001",
-            date_of_birth=datetime(2019, 12, 1, tzinfo=tzutc()),
+            date_of_birth=datetime(2016, 12, 1, tzinfo=tzutc()),
             sex="M",
             species="mouse",
         ),
         **simple1_nwb_metadata,
     )
 
 
@@ -83,15 +83,15 @@
     # need to copy first and then use -f move since we will create one more
     # file to be "organized"
     shutil.copy(str(simple2_nwb), str(tmp_path))
     make_nwb_file(
         str(tmp_path / "simple3.nwb"),
         subject=pynwb.file.Subject(
             subject_id="lizard001",
-            date_of_birth=datetime(2019, 12, 1, tzinfo=tzutc()),
+            date_of_birth=datetime(2016, 12, 1, tzinfo=tzutc()),
             sex="F",
             species="Gekko gecko",
         ),
         **simple1_nwb_metadata,
     )
     (tmp_path / dandiset_metadata_file).write_text("{}\n")
     r = clirunner.invoke(organize, ["-f", "move", "--dandiset-path", str(tmp_path)])
```

### Comparing `dandi-0.8.0/dandi/tests/test_pynwb_utils.py` & `dandi-0.9.0/dandi/tests/test_pynwb_utils.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/dandi/tests/test_models.py` & `dandi-0.9.0/dandi/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import pytest
 
 from ..models import DandiMeta, AssetMeta
-from ..models import AccessType, RoleType, Relation, License, IdentifierType, DigestType
+from ..models import (
+    AccessType,
+    RoleType,
+    RelationType,
+    LicenseType,
+    IdentifierType,
+    DigestType,
+)
 
 
 def test_dandiset():
     assert DandiMeta.unvalidated()
 
 
 def test_asset():
@@ -53,15 +60,15 @@
                 "StudyParticipant": "dandi:StudyParticipant",
                 "Affiliation": "dandi:Affiliation",
                 "EthicsApproval": "dandi:EthicsApproval",
                 "Other": "dandi:Other",
             },
         ),
         (
-            Relation,
+            RelationType,
             {
                 "IsCitedBy": "dandi:IsCitedBy",
                 "Cites": "dandi:Cites",
                 "IsSupplementTo": "dandi:IsSupplementTo",
                 "IsSupplementedBy": "dandi:IsSupplementedBy",
                 "IsContinuedBy": "dandi:IsContinuedBy",
                 "Continues": "dandi:Continues",
@@ -91,15 +98,15 @@
                 "IsRequiredBy": "dandi:IsRequiredBy",
                 "Requires": "dandi:Requires",
                 "Obsoletes": "dandi:Obsoletes",
                 "IsObsoletedBy": "dandi:IsObsoletedBy",
             },
         ),
         (
-            License,
+            LicenseType,
             {
                 "CC0": "dandi:CC0",
                 "CCBY40": "dandi:CCBY40",
                 "CCBYNC40": "dandi:CCBYNC40",
             },
         ),
         (
```

### Comparing `dandi-0.8.0/dandi/tests/test_girder.py` & `dandi-0.9.0/dandi/tests/test_girder.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,54 +235,54 @@
 def test_keyring_lookup_encrypted_fallback_not_exists_no_create(
     fs, mocker, monkeypatch
 ):
     # Requesting the `fs` fixture (even if it's not directly used) should
     # guarantee that an encrypted keyring on the real filesystem isn't found.
     monkeypatch.delenv("PYTHON_KEYRING_BACKEND", raising=False)
     get_keyring = mocker.patch("dandi.girder.get_keyring", return_value=fail.Keyring())
-    askyesno = mocker.patch("dandi.girder.askyesno", return_value=False)
+    confirm = mocker.patch("click.confirm", return_value=False)
     with pytest.raises(KeyringError):
         girder.keyring_lookup("testservice", "testusername")
     get_keyring.assert_called_once_with()
-    askyesno.assert_called_once_with(
+    confirm.assert_called_once_with(
         "Would you like to establish an encrypted keyring?", default=True
     )
 
 
 def test_keyring_lookup_encrypted_fallback_not_exists_create_rcconf(
     fs, mocker, monkeypatch
 ):
     # Requesting the `fs` fixture (even if it's not directly used) should
     # guarantee that a fake filesystem is used.
     monkeypatch.delenv("PYTHON_KEYRING_BACKEND", raising=False)
     get_keyring = mocker.patch("dandi.girder.get_keyring", return_value=fail.Keyring())
-    askyesno = mocker.patch("dandi.girder.askyesno", return_value=True)
+    confirm = mocker.patch("click.confirm", return_value=True)
     kb, password = girder.keyring_lookup("testservice", "testusername")
     assert isinstance(kb, keyfile.EncryptedKeyring)
     assert password is None
     get_keyring.assert_called_once_with()
-    askyesno.assert_called_once_with(
+    confirm.assert_called_once_with(
         "Would you like to establish an encrypted keyring?", default=True
     )
     assert os.path.exists(girder.keyringrc_file())
     with open(girder.keyringrc_file()) as fp:
         assert fp.read() == (
             "[backend]\ndefault-keyring = keyrings.alt.file.EncryptedKeyring\n"
         )
 
 
 def test_keyring_lookup_encrypted_fallback_not_exists_create_rcconf_exists(
     fs, mocker, monkeypatch
 ):
     monkeypatch.delenv("PYTHON_KEYRING_BACKEND", raising=False)
     get_keyring = mocker.patch("dandi.girder.get_keyring", return_value=fail.Keyring())
-    askyesno = mocker.patch("dandi.girder.askyesno", return_value=True)
+    confirm = mocker.patch("click.confirm", return_value=True)
     fs.create_file(girder.keyringrc_file(), contents="# placeholder\n")
     kb, password = girder.keyring_lookup("testservice", "testusername")
     assert isinstance(kb, keyfile.EncryptedKeyring)
     assert password is None
     get_keyring.assert_called_once_with()
-    askyesno.assert_called_once_with(
+    confirm.assert_called_once_with(
         "Would you like to establish an encrypted keyring?", default=True
     )
     with open(girder.keyringrc_file()) as fp:
         assert fp.read() == "# placeholder\n"
```

### Comparing `dandi-0.8.0/dandi/tests/test_validate.py` & `dandi-0.9.0/dandi/tests/test_validate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from ..validate import validate_file
 
 
-def test_validate_simple1(simple1_nwb):
+def test_validate_simple1(monkeypatch, simple1_nwb):
+    monkeypatch.setenv("DANDI_SCHEMA", "1")
     # this file lacks subject_id
     errors = validate_file(simple1_nwb)
     assert len(errors) == 1
-    assert errors[0] == "Required field 'subject_id' has no value"
+    assert errors[0] == (
+        "1 validation error for AssetMeta\n"
+        "wasDerivedFrom -> 0 -> identifier\n"
+        "  none is not an allowed value (type=type_error.none.not_allowed)"
+    )
 
 
 def test_validate_simple2(simple2_nwb):
     # this file should be ok
     errors = validate_file(simple2_nwb)
     assert not errors
```

### Comparing `dandi-0.8.0/setup.py` & `dandi-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `dandi-0.8.0/PKG-INFO` & `dandi-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandi
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line client for interaction with DANDI archive elements
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
@@ -109,14 +109,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Provides: dandi
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: extensions
 Provides-Extra: extras
 Provides-Extra: style
```

