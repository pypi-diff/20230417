# Comparing `tmp/bump-my-version-0.2.0.tar.gz` & `tmp/bump-my-version-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.2.0.tar", last modified: Fri Apr 14 17:08:51 2023, max compression
+gzip compressed data, was "bump-my-version-0.3.0.tar", last modified: Mon Apr 17 13:59:51 2023, max compression
```

## Comparing `bump-my-version-0.2.0.tar` & `bump-my-version-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.299748 bump-my-version-0.2.0/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5686 2023-04-14 17:05:38.000000 bump-my-version-0.2.0/CHANGELOG.md
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4900 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 OORDCOR    (502) staff       (20)    10135 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1075 2023-04-09 17:40:05.000000 bump-my-version-0.2.0/LICENSE
--rw-r--r--   0 OORDCOR    (502) staff       (20)      259 2023-03-24 16:56:31.000000 bump-my-version-0.2.0/MANIFEST.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)     8064 2023-04-14 17:08:51.299831 bump-my-version-0.2.0/PKG-INFO
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7542 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/README.md
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.275437 bump-my-version-0.2.0/bump_my_version.egg-info/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     8064 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1475 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        1 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       90 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        1 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/not-zip-safe
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1441 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       12 2023-04-14 17:08:51.000000 bump-my-version-0.2.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.283985 bump-my-version-0.2.0/bumpversion/
--rw-r--r--   0 OORDCOR    (502) staff       (20)       73 2023-04-14 17:05:38.000000 bump-my-version-0.2.0/bumpversion/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)       73 2023-04-08 15:15:04.000000 bump-my-version-0.2.0/bumpversion/__main__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1289 2023-03-24 14:53:33.000000 bump-my-version-0.2.0/bumpversion/aliases.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2245 2023-03-28 13:05:48.000000 bump-my-version-0.2.0/bumpversion/autocast.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3793 2023-04-09 14:04:00.000000 bump-my-version-0.2.0/bumpversion/bump.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     6723 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/bumpversion/cli.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    13071 2023-04-12 14:13:39.000000 bump-my-version-0.2.0/bumpversion/config.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1162 2023-04-10 13:57:20.000000 bump-my-version-0.2.0/bumpversion/exceptions.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7826 2023-04-09 14:29:57.000000 bump-my-version-0.2.0/bumpversion/files.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3373 2023-04-03 18:27:56.000000 bump-my-version-0.2.0/bumpversion/functions.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      747 2023-04-10 13:57:30.000000 bump-my-version-0.2.0/bumpversion/logging.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    10726 2023-04-10 13:58:30.000000 bump-my-version-0.2.0/bumpversion/scm.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1769 2023-04-10 13:51:01.000000 bump-my-version-0.2.0/bumpversion/utils.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    10319 2023-04-10 13:54:18.000000 bump-my-version-0.2.0/bumpversion/version_part.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3616 2023-04-14 17:05:38.000000 bump-my-version-0.2.0/pyproject.toml
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.287261 bump-my-version-0.2.0/requirements/
--rw-r--r--   0 OORDCOR    (502) staff       (20)       78 2023-03-28 12:31:10.000000 bump-my-version-0.2.0/requirements/dev.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4919 2023-04-07 18:56:11.000000 bump-my-version-0.2.0/requirements/dev.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)      113 2023-03-24 16:56:32.000000 bump-my-version-0.2.0/requirements/docs.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1962 2023-03-31 16:52:58.000000 bump-my-version-0.2.0/requirements/docs.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       39 2023-03-28 15:44:30.000000 bump-my-version-0.2.0/requirements/prod.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)      530 2023-03-31 16:52:52.000000 bump-my-version-0.2.0/requirements/prod.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       63 2023-04-07 18:56:01.000000 bump-my-version-0.2.0/requirements/test.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1434 2023-04-07 18:56:10.000000 bump-my-version-0.2.0/requirements/test.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       25 2023-03-24 16:56:31.000000 bump-my-version-0.2.0/requirements.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)      811 2023-04-14 17:08:51.301992 bump-my-version-0.2.0/setup.cfg
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2380 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/setup.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.294395 bump-my-version-0.2.0/tests/
--rw-r--r--   0 OORDCOR    (502) staff       (20)       41 2023-03-28 16:29:57.000000 bump-my-version-0.2.0/tests/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1694 2023-04-10 13:52:31.000000 bump-my-version-0.2.0/tests/conftest.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.296028 bump-my-version-0.2.0/tests/fixtures/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      556 2023-04-07 13:33:05.000000 bump-my-version-0.2.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 OORDCOR    (502) staff       (20)      865 2023-04-09 14:31:10.000000 bump-my-version-0.2.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 OORDCOR    (502) staff       (20)      632 2023-03-28 12:30:17.000000 bump-my-version-0.2.0/tests/fixtures/basic_cfg_expected.json
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.297364 bump-my-version-0.2.0/tests/fixtures/glob/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.297767 bump-my-version-0.2.0/tests/fixtures/glob/directory/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2023-04-05 14:35:18.000000 bump-my-version-0.2.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2023-04-05 14:34:47.000000 bump-my-version-0.2.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2023-04-05 14:34:58.000000 bump-my-version-0.2.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2023-04-05 14:35:34.000000 bump-my-version-0.2.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2023-04-14 17:08:51.299186 bump-my-version-0.2.0/tests/fixtures/interpolation/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      136 2023-04-05 05:50:31.000000 bump-my-version-0.2.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 OORDCOR    (502) staff       (20)      168 2023-04-05 06:12:10.000000 bump-my-version-0.2.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 OORDCOR    (502) staff       (20)      139 2023-04-05 05:50:07.000000 bump-my-version-0.2.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 OORDCOR    (502) staff       (20)    82487 2023-04-10 13:45:32.000000 bump-my-version-0.2.0/tests/old_tests.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2418 2023-03-28 16:29:57.000000 bump-my-version-0.2.0/tests/test_autocast.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5957 2023-04-08 15:09:29.000000 bump-my-version-0.2.0/tests/test_bump.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7353 2023-04-10 13:50:56.000000 bump-my-version-0.2.0/tests/test_cli.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     6705 2023-04-09 14:31:10.000000 bump-my-version-0.2.0/tests/test_config.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    10195 2023-04-13 18:31:03.000000 bump-my-version-0.2.0/tests/test_files.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2044 2023-04-03 18:10:42.000000 bump-my-version-0.2.0/tests/test_functions.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4265 2023-04-10 13:53:15.000000 bump-my-version-0.2.0/tests/test_scm.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    10825 2023-04-10 13:54:40.000000 bump-my-version-0.2.0/tests/test_version_part.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.689983 bump-my-version-0.3.0/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.689983 bump-my-version-0.3.0/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg_expected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_version_part.py
```

### Comparing `bump-my-version-0.2.0/CHANGELOG.md` & `bump-my-version-0.3.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,45 @@
 # Changelog
 
+## 0.3.0 (2023-04-17)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.2.0...0.3.0)
+
+### Fixes
+
+- Fixed bug in SCMInfo setup. [e8fddc9](https://github.com/callowayproject/bump-my-version/commit/e8fddc99ec5f4632f097790ca6b851d8854e09bd)
+    
+- Fixed missing xml coverage report. [696503f](https://github.com/callowayproject/bump-my-version/commit/696503fff800ea1f3ffb559108cde726296f2d98)
+    
+- Fixed assertion in failing test. [7afe58c](https://github.com/callowayproject/bump-my-version/commit/7afe58c4a15e0b48f223c3f2c80c48679e44aebc)
+    
+- Fixes issue when new version equals current version. [64b0de3](https://github.com/callowayproject/bump-my-version/commit/64b0de39828367c6c6f3e7103497256ce3f44f41)
+    
+  - Now it reports they are the same and exits.
+- Fixes issue of duplicate tags. [c025650](https://github.com/callowayproject/bump-my-version/commit/c0256509cb39c3e78c09d35205007191fbf3732e)
+    
+  - Now it checks if the tag exists and reports a warning
+- Fixed automation tooling. [19f13b7](https://github.com/callowayproject/bump-my-version/commit/19f13b7c0c388f15af45cf3fa04424a2946b4a04)
+    
+  - changed name to bump-my-version in setup.cfg
+  - added PAT in release pipeline to (hopefully) allow committing and tagging to master without issue.
+### New
+
+- Added codecov to workflow. [a5009e0](https://github.com/callowayproject/bump-my-version/commit/a5009e04068787bb98363c3e6803f84a338ee798)
+    
+### Other
+
+- Migrated setuptools metadata to pyproject.toml. [0bd54dc](https://github.com/callowayproject/bump-my-version/commit/0bd54dca1230021de266042014164fada25e0837)
+    
+### Updates
+
+- Updated the readme. [1b1d910](https://github.com/callowayproject/bump-my-version/commit/1b1d910756be07638e6cb113ee05a6f5261f6393)
+    
+- Updated documentation. [6c3b4fe](https://github.com/callowayproject/bump-my-version/commit/6c3b4fe4995ea67b1cc13ca265d16506bde4dd02)
+    
+
 ## 0.2.0 (2023-04-14)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.1.0...0.2.0)
 
 ### Fixes
 
 - Fixed configuration to allow_dirty in bumpversion. [b042e31](https://github.com/callowayproject/bump-my-version/commit/b042e31c47fe03978847552e1efea6a1acb8729e)
```

### Comparing `bump-my-version-0.2.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/CONTRIBUTING.md` & `bump-my-version-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/LICENSE` & `bump-my-version-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/PKG-INFO` & `bump-my-version-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,48 @@
-Metadata-Version: 2.1
-Name: bump-my-version
-Version: 0.2.0
-Summary: Version bump your Python project
-Home-page: https://github.com/callowayproject/bump-my-version
-Author: Corey Oordt
-Author-email: coreyoordt@gmail.com
-Keywords: bumpversion
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Bump My Version
 
 [![image](https://img.shields.io/pypi/v/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/l/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/pyversions/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
+[![codecov](https://codecov.io/gh/callowayproject/bump-my-version/branch/master/graph/badge.svg?token=D1GSOtWEPU)](https://codecov.io/gh/callowayproject/bump-my-version)
 [![GitHub Actions](https://github.com/callowayproject/bump-my-version/workflows/CI/badge.svg)](https://github.com/callowayproject/bump-my-version/actions)
 
 > **NOTE**
 >
-> This is a maintained refactor of the [bump2version fork of](https://github.com/c4urself/bump2version) the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
+> This is a maintained refactor of the [bump2version fork](https://github.com/c4urself/bump2version) of the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
 >
 > - Add support for `pyproject.toml` configuration files.
 > - Convert to [click](https://click.palletsprojects.com/en/8.1.x/) for and [rich](https://rich.readthedocs.io/en/stable/index.html) for the CLI interface
 > - Add better configuration validation using [Pydantic](https://docs.pydantic.dev)
 > - Make the code and tests easier to read and maintain
 
 
 ## Overview
 
 Version-bump your software with a single command!
 
-A small command line tool to simplify releasing software by updating all
-version strings in your source code by the correct increment. Also creates
-commits and tags:
+A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an always increment configuration
+- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-
-**Potential bugs to verify**
-
 - https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/260 Incorrect behavior when new version == current version
-- https://github.com/c4urself/bump2version/issues/248 Potential bug/test case
-- https://github.com/c4urself/bump2version/issues/246 Release inconsistency
 - https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
 - https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-- https://github.com/c4urself/bump2version/issues/224 Verify tag doesn't exist
 
 **Documentation opportunities**
 
 - https://github.com/c4urself/bump2version/issues/252 
 - https://github.com/c4urself/bump2version/issues/247
 - https://github.com/c4urself/bump2version/issues/243
 - https://github.com/c4urself/bump2version/issues/240
@@ -182,15 +157,13 @@
 
 ## Development & Contributing
 
 Thank you, contributors! You can find a full list here: https://github.com/callowayproject/bump-my-version/graphs/contributors
 
 See also our [CONTRIBUTING.md](CONTRIBUTING.md)
 
-Development of this happens on GitHub, patches including tests, and documentation
-are very welcome, as well as bug reports! Also please open an issue if this
-tool does not support every aspect of bumping versions in your development
+Development of this happens on GitHub, patches including tests, and documentation are very welcome, as well as bug reports! Please open an issue if this tool does not support every aspect of bumping versions in your development
 workflow, as it is intended to be very versatile.
 
 ## License
 
 bump-my-version is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `bump-my-version-0.2.0/README.md` & `bump-my-version-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,102 @@
+Metadata-Version: 2.1
+Name: bump-my-version
+Version: 0.3.0
+Summary: Version bump your Python project
+Author-email: Corey Oordt <coreyoordt@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2013-2014 Filip Noetzel
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/callowayproject/bump-my-version
+Project-URL: repository, https://github.com/callowayproject/bump-my-version.git
+Project-URL: documentation, https://callowayproject.github.io/bump-my-version/
+Keywords: bumpversion,version,release
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: System :: Software Distribution
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
 # Bump My Version
 
 [![image](https://img.shields.io/pypi/v/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/l/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/pyversions/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
+[![codecov](https://codecov.io/gh/callowayproject/bump-my-version/branch/master/graph/badge.svg?token=D1GSOtWEPU)](https://codecov.io/gh/callowayproject/bump-my-version)
 [![GitHub Actions](https://github.com/callowayproject/bump-my-version/workflows/CI/badge.svg)](https://github.com/callowayproject/bump-my-version/actions)
 
 > **NOTE**
 >
-> This is a maintained refactor of the [bump2version fork of](https://github.com/c4urself/bump2version) the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
+> This is a maintained refactor of the [bump2version fork](https://github.com/c4urself/bump2version) of the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
 >
 > - Add support for `pyproject.toml` configuration files.
 > - Convert to [click](https://click.palletsprojects.com/en/8.1.x/) for and [rich](https://rich.readthedocs.io/en/stable/index.html) for the CLI interface
 > - Add better configuration validation using [Pydantic](https://docs.pydantic.dev)
 > - Make the code and tests easier to read and maintain
 
 
 ## Overview
 
 Version-bump your software with a single command!
 
-A small command line tool to simplify releasing software by updating all
-version strings in your source code by the correct increment. Also creates
-commits and tags:
+A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an always increment configuration
+- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-
-**Potential bugs to verify**
-
 - https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/260 Incorrect behavior when new version == current version
-- https://github.com/c4urself/bump2version/issues/248 Potential bug/test case
-- https://github.com/c4urself/bump2version/issues/246 Release inconsistency
 - https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
 - https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-- https://github.com/c4urself/bump2version/issues/224 Verify tag doesn't exist
 
 **Documentation opportunities**
 
 - https://github.com/c4urself/bump2version/issues/252 
 - https://github.com/c4urself/bump2version/issues/247
 - https://github.com/c4urself/bump2version/issues/243
 - https://github.com/c4urself/bump2version/issues/240
@@ -165,15 +211,13 @@
 
 ## Development & Contributing
 
 Thank you, contributors! You can find a full list here: https://github.com/callowayproject/bump-my-version/graphs/contributors
 
 See also our [CONTRIBUTING.md](CONTRIBUTING.md)
 
-Development of this happens on GitHub, patches including tests, and documentation
-are very welcome, as well as bug reports! Also please open an issue if this
-tool does not support every aspect of bumping versions in your development
+Development of this happens on GitHub, patches including tests, and documentation are very welcome, as well as bug reports! Please open an issue if this tool does not support every aspect of bumping versions in your development
 workflow, as it is intended to be very versatile.
 
 ## License
 
 bump-my-version is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `bump-my-version-0.2.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.3.0/bump_my_version.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,102 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.2.0
+Version: 0.3.0
 Summary: Version bump your Python project
-Home-page: https://github.com/callowayproject/bump-my-version
-Author: Corey Oordt
-Author-email: coreyoordt@gmail.com
-Keywords: bumpversion
-Classifier: Development Status :: 3 - Alpha
+Author-email: Corey Oordt <coreyoordt@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2013-2014 Filip Noetzel
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/callowayproject/bump-my-version
+Project-URL: repository, https://github.com/callowayproject/bump-my-version.git
+Project-URL: documentation, https://callowayproject.github.io/bump-my-version/
+Keywords: bumpversion,version,release
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: System :: Software Distribution
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Bump My Version
 
 [![image](https://img.shields.io/pypi/v/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/l/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/pyversions/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
+[![codecov](https://codecov.io/gh/callowayproject/bump-my-version/branch/master/graph/badge.svg?token=D1GSOtWEPU)](https://codecov.io/gh/callowayproject/bump-my-version)
 [![GitHub Actions](https://github.com/callowayproject/bump-my-version/workflows/CI/badge.svg)](https://github.com/callowayproject/bump-my-version/actions)
 
 > **NOTE**
 >
-> This is a maintained refactor of the [bump2version fork of](https://github.com/c4urself/bump2version) the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
+> This is a maintained refactor of the [bump2version fork](https://github.com/c4urself/bump2version) of the excellent [bumpversion project](https://github.com/peritus/bumpversion). The main goals of this refactor were:
 >
 > - Add support for `pyproject.toml` configuration files.
 > - Convert to [click](https://click.palletsprojects.com/en/8.1.x/) for and [rich](https://rich.readthedocs.io/en/stable/index.html) for the CLI interface
 > - Add better configuration validation using [Pydantic](https://docs.pydantic.dev)
 > - Make the code and tests easier to read and maintain
 
 
 ## Overview
 
 Version-bump your software with a single command!
 
-A small command line tool to simplify releasing software by updating all
-version strings in your source code by the correct increment. Also creates
-commits and tags:
+A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an always increment configuration
+- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-
-**Potential bugs to verify**
-
 - https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/260 Incorrect behavior when new version == current version
-- https://github.com/c4urself/bump2version/issues/248 Potential bug/test case
-- https://github.com/c4urself/bump2version/issues/246 Release inconsistency
 - https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
 - https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-- https://github.com/c4urself/bump2version/issues/224 Verify tag doesn't exist
 
 **Documentation opportunities**
 
 - https://github.com/c4urself/bump2version/issues/252 
 - https://github.com/c4urself/bump2version/issues/247
 - https://github.com/c4urself/bump2version/issues/243
 - https://github.com/c4urself/bump2version/issues/240
@@ -182,15 +211,13 @@
 
 ## Development & Contributing
 
 Thank you, contributors! You can find a full list here: https://github.com/callowayproject/bump-my-version/graphs/contributors
 
 See also our [CONTRIBUTING.md](CONTRIBUTING.md)
 
-Development of this happens on GitHub, patches including tests, and documentation
-are very welcome, as well as bug reports! Also please open an issue if this
-tool does not support every aspect of bumping versions in your development
+Development of this happens on GitHub, patches including tests, and documentation are very welcome, as well as bug reports! Please open an issue if this tool does not support every aspect of bumping versions in your development
 workflow, as it is intended to be very versatile.
 
 ## License
 
 bump-my-version is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `bump-my-version-0.2.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.3.0/bump_my_version.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 requirements/docs.txt
 requirements/prod.in
 requirements/prod.txt
 requirements/test.in
 requirements/test.txt
 tests/__init__.py
 tests/conftest.py
-tests/old_tests.py
 tests/test_autocast.py
 tests/test_bump.py
 tests/test_cli.py
 tests/test_config.py
 tests/test_files.py
 tests/test_functions.py
 tests/test_scm.py
```

### Comparing `bump-my-version-0.2.0/bump_my_version.egg-info/requires.txt` & `bump-my-version-0.3.0/bump_my_version.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/aliases.py` & `bump-my-version-0.3.0/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/autocast.py` & `bump-my-version-0.3.0/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/bump.py` & `bump-my-version-0.3.0/bumpversion/bump.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
 
     ctx = get_context(config)
     version = config.version_config.parse(config.current_version)
     next_version = get_next_version(version, config, version_part, new_version)
     next_version_str = config.version_config.serialize(next_version, ctx)
     logger.info("New version will be '%s'", next_version_str)
 
+    if config.current_version == next_version_str:
+        logger.info("Version is already '%s'", next_version_str)
+        return
+
     if dry_run:
         logger.info("Dry run active, won't touch any files.")
 
     ctx = get_context(config, version, next_version)
 
     configured_files = resolve_file_config(config.files, config.version_config)
     modify_files(configured_files, version, next_version, ctx, dry_run)
```

### Comparing `bump-my-version-0.2.0/bumpversion/cli.py` & `bump-my-version-0.3.0/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/config.py` & `bump-my-version-0.3.0/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/exceptions.py` & `bump-my-version-0.3.0/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/files.py` & `bump-my-version-0.3.0/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/functions.py` & `bump-my-version-0.3.0/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/logging.py` & `bump-my-version-0.3.0/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/scm.py` & `bump-my-version-0.3.0/bumpversion/scm.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 class SourceCodeManager:
     """Base class for version control systems."""
 
     _TEST_USABLE_COMMAND: List[str] = []
     _COMMIT_COMMAND: List[str] = []
+    _ALL_TAGS_COMMAND: List[str] = []
 
     @classmethod
     def commit(cls, message: str, current_version: str, new_version: str, extra_args: Optional[list] = None) -> None:
         """Commit the changes."""
         extra_args = extra_args or []
 
         with NamedTemporaryFile("wb", delete=False) as f:
@@ -81,14 +82,23 @@
 
     @classmethod
     def tag(cls, name: str, sign: bool = False, message: Optional[str] = None) -> None:
         """Create a tag of the new_version in VCS."""
         raise NotImplementedError
 
     @classmethod
+    def get_all_tags(cls) -> List[str]:
+        """Return all tags in VCS."""
+        try:
+            result = subprocess.run(cls._ALL_TAGS_COMMAND, text=True, check=True, capture_output=True)
+            return result.stdout.splitlines()
+        except (FileNotFoundError, PermissionError, NotADirectoryError, subprocess.CalledProcessError):
+            return []
+
+    @classmethod
     def commit_to_scm(
         cls,
         files: List[Union[str, Path]],
         config: "Config",
         context: MutableMapping,
         extra_args: Optional[List[str]] = None,
         dry_run: bool = False,
@@ -131,15 +141,21 @@
 
     @classmethod
     def tag_in_scm(cls, config: "Config", context: MutableMapping, dry_run: bool = False) -> None:
         """Tag the current commit in the source code management system."""
         sign_tags = config.sign_tags
         tag_name = config.tag_name.format(**context)
         tag_message = config.tag_message.format(**context)
+        existing_tags = cls.get_all_tags()
         do_tag = config.tag and not dry_run
+
+        if tag_name in existing_tags and config.tag:
+            logger.warning("Tag '%s' already exists. Will not tag.", tag_name)
+            return
+
         logger.info(
             "%s '%s' %s in %s and %s",
             "Tagging" if do_tag else "Would tag",
             tag_name,
             f"with message '{tag_message}'" if tag_message else "without message",
             cls.__name__,
             "signing" if sign_tags else "not signing",
@@ -149,14 +165,15 @@
 
 
 class Git(SourceCodeManager):
     """Git implementation."""
 
     _TEST_USABLE_COMMAND = ["git", "rev-parse", "--git-dir"]
     _COMMIT_COMMAND = ["git", "commit", "-F"]
+    _ALL_TAGS_COMMAND = ["git", "tag", "--list"]
 
     @classmethod
     def assert_nondirty(cls) -> None:
         """Assert that the working directory is not dirty."""
         lines = [
             line.strip()
             for line in subprocess.check_output(["git", "status", "--porcelain"]).splitlines()
@@ -192,15 +209,15 @@
             ]
             result = subprocess.run(git_cmd, text=True, check=True, capture_output=True)
             describe_out = result.stdout.strip().split("-")
         except subprocess.CalledProcessError as e:
             logger.debug("Error when running git describe: %s", e.stderr)
             return SCMInfo(tool=cls)
 
-        info = SCMInfo()
+        info = SCMInfo(tool=cls)
 
         if describe_out[-1].strip() == "dirty":
             info.dirty = True
             describe_out.pop()
         else:
             info.dirty = False
 
@@ -237,14 +254,15 @@
 
 
 class Mercurial(SourceCodeManager):
     """Mercurial implementation."""
 
     _TEST_USABLE_COMMAND = ["hg", "root"]
     _COMMIT_COMMAND = ["hg", "commit", "--logfile"]
+    _ALL_TAGS_COMMAND = ["hg", "log", '--rev="tag()"', '--template="{tags}\n"']
 
     @classmethod
     def latest_tag_info(cls, tag_pattern: str) -> SCMInfo:
         """Return information about the latest tag."""
         current_version = None
         re_pattern = tag_pattern.replace("*", ".*")
         result = subprocess.run(
```

### Comparing `bump-my-version-0.2.0/bumpversion/utils.py` & `bump-my-version-0.3.0/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/bumpversion/version_part.py` & `bump-my-version-0.3.0/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/requirements/dev.txt` & `bump-my-version-0.3.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/requirements/docs.txt` & `bump-my-version-0.3.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/requirements/prod.txt` & `bump-my-version-0.3.0/requirements/prod.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/requirements/test.txt` & `bump-my-version-0.3.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/setup.py` & `bump-my-version-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/conftest.py` & `bump-my-version-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.3.0/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.3.0/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.3.0/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_autocast.py` & `bump-my-version-0.3.0/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_bump.py` & `bump-my-version-0.3.0/tests/test_bump.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 
 from bumpversion import bump
 from bumpversion.exceptions import ConfigurationError
 from bumpversion.files import ConfiguredFile
 from bumpversion.scm import Git, SCMInfo
-from tests.conftest import get_config_data
+from tests.conftest import get_config_data, inside_dir
 
 
 @pytest.fixture
 def mock_context():
     return {"current_version": "1.2.3", "new_version": "1.2.4"}
 
 
@@ -112,23 +112,38 @@
     mock_update_config_file.assert_called_once()
     assert mock_update_config_file.call_args[0][0] is None
     assert mock_update_config_file.call_args[0][1] is config.current_version
     assert mock_update_config_file.call_args[0][2] == "2.0.0"
     assert mock_update_config_file.call_args[0][3] is True
 
 
+@patch("bumpversion.files.modify_files")
+@patch("bumpversion.bump.update_config_file")
+def test_do_bump_when_new_equals_current(mock_update_config_file, mock_modify_files, tmp_path: Path):
+    """When the new version is the same as the current version, nothing should happen."""
+
+    # Arrange
+    version_part = None
+    new_version = "1.2.3"
+
+    with inside_dir(tmp_path):
+        config, version_config, current_version = get_config_data({"current_version": "1.2.3"})
+        # Act
+        bump.do_bump(version_part, new_version, config)
+
+    # Assert
+    mock_modify_files.assert_not_called()
+    mock_update_config_file.assert_not_called()
+
+
 def test_do_bump_with_no_arguments():
     # Arrange
     version_part = None
     new_version = None
-    config, version_config, current_version = get_config_data(
-        {
-            "current_version": "1.2.3",
-        }
-    )
+    config, version_config, current_version = get_config_data({"current_version": "1.2.3"})
     config.scm_info = SCMInfo()
     dry_run = False
 
     # Act/Assert
     with pytest.raises(ConfigurationError):
         bump.do_bump(version_part, new_version, config, dry_run=dry_run)
```

### Comparing `bump-my-version-0.2.0/tests/test_cli.py` & `bump-my-version-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_config.py` & `bump-my-version-0.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_files.py` & `bump-my-version-0.3.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_functions.py` & `bump-my-version-0.3.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.2.0/tests/test_version_part.py` & `bump-my-version-0.3.0/tests/test_version_part.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,8 +293,40 @@
 
 def test_parse_doesnt_parse_current_version(tmp_path: Path, caplog: LogCaptureFixture) -> None:
     """A warning should be output when the parse regex doesn't parse the version."""
     overrides = {"current_version": "12", "parse": "xxx"}
     with inside_dir(tmp_path):
         get_config_data(overrides)
 
-    assert caplog.messages == ["Evaluating 'parse' option: 'xxx' does not parse current version '12'"]
+    assert "Evaluating 'parse' option: 'xxx' does not parse current version '12'" in caplog.messages
+
+
+def test_part_does_not_revert_to_zero_if_optional(tmp_path: Path) -> None:
+    """A non-numeric part with the optional value should not revert to zero."""
+    # From https://github.com/c4urself/bump2version/issues/248
+    # Arrange
+    overrides = {
+        "current_version": "0.3.1",
+        "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)((?P<release>\D+)(?P<build>\d*))?",
+        "serialize": [
+            "{major}.{minor}.{patch}{release}{build}",
+            "{major}.{minor}.{patch}{release}",
+            "{major}.{minor}.{patch}",
+        ],
+        "parts": {
+            "release": {
+                "optional_value": "g",
+                "first_value": "g",
+                "values": [
+                    "dev",
+                    "a",
+                    "b",
+                    "g",
+                ],
+            },
+        },
+    }
+    with inside_dir(tmp_path):
+        conf, version_config, current_version = get_config_data(overrides)
+
+    new_version = current_version.bump("build", version_config.order)
+    assert version_config.serialize(new_version, get_context(conf)) == "0.3.1g1"
```

