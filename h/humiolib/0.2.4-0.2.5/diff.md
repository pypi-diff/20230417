# Comparing `tmp/humiolib-0.2.4.tar.gz` & `tmp/humiolib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humiolib-0.2.4.tar", last modified: Mon Aug 15 10:36:26 2022, max compression
+gzip compressed data, was "humiolib-0.2.5.tar", last modified: Mon Apr 17 09:13:11 2023, max compression
```

## Comparing `humiolib-0.2.4.tar` & `humiolib-0.2.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.822789 humiolib-0.2.4/
--rw-r--r--   0 abrandborg   (501) staff       (20)      156 2022-08-15 10:31:58.000000 humiolib-0.2.4/.bumpversion.cfg
--rw-r--r--   0 abrandborg   (501) staff       (20)      666 2021-08-13 07:31:27.000000 humiolib-0.2.4/AUTHORS.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)     1295 2022-08-15 10:33:37.000000 humiolib-0.2.4/CHANGELOG.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)     7475 2021-08-13 06:46:58.000000 humiolib-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)    11406 2021-08-13 06:46:58.000000 humiolib-0.2.4/LICENSE
--rw-r--r--   0 abrandborg   (501) staff       (20)      245 2021-08-13 06:46:58.000000 humiolib-0.2.4/MANIFEST.in
--rw-r--r--   0 abrandborg   (501) staff       (20)     6941 2022-08-15 10:36:26.822967 humiolib-0.2.4/PKG-INFO
--rw-r--r--   0 abrandborg   (501) staff       (20)     4786 2021-08-13 06:46:58.000000 humiolib-0.2.4/README.rst
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.801566 humiolib-0.2.4/docs/
--rw-r--r--   0 abrandborg   (501) staff       (20)       28 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/authors.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)       30 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/changelog.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)      825 2022-08-15 10:31:58.000000 humiolib-0.2.4/docs/conf.py
--rw-r--r--   0 abrandborg   (501) staff       (20)       33 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/contributing.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)      220 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/index.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)       27 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/readme.rst
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.804044 humiolib-0.2.4/docs/reference/
--rw-r--r--   0 abrandborg   (501) staff       (20)       91 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/reference/humioclient.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)      103 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/reference/humioexceptions.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)      113 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/reference/index.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)       75 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/reference/queryjob.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)       79 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/reference/webcaller.rst
--rw-r--r--   0 abrandborg   (501) staff       (20)       29 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/requirements.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)      109 2021-08-13 06:46:58.000000 humiolib-0.2.4/docs/spelling_wordlist.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)      504 2022-08-15 10:36:26.823594 humiolib-0.2.4/setup.cfg
--rw-r--r--   0 abrandborg   (501) staff       (20)     3026 2022-08-15 10:31:58.000000 humiolib-0.2.4/setup.py
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.791442 humiolib-0.2.4/src/
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.808009 humiolib-0.2.4/src/humiolib/
--rw-r--r--   0 abrandborg   (501) staff       (20)    21473 2022-08-15 10:30:31.000000 humiolib-0.2.4/src/humiolib/HumioClient.py
--rw-r--r--   0 abrandborg   (501) staff       (20)      500 2021-08-13 06:46:58.000000 humiolib-0.2.4/src/humiolib/HumioExceptions.py
--rw-r--r--   0 abrandborg   (501) staff       (20)     7523 2021-08-13 07:06:27.000000 humiolib-0.2.4/src/humiolib/QueryJob.py
--rw-r--r--   0 abrandborg   (501) staff       (20)     4749 2022-08-15 10:30:31.000000 humiolib-0.2.4/src/humiolib/WebCaller.py
--rw-r--r--   0 abrandborg   (501) staff       (20)       85 2022-08-15 10:31:58.000000 humiolib-0.2.4/src/humiolib/__init__.py
--rw-r--r--   0 abrandborg   (501) staff       (20)      364 2021-08-13 06:46:58.000000 humiolib-0.2.4/src/humiolib/__main__.py
--rw-r--r--   0 abrandborg   (501) staff       (20)     4100 2021-08-13 06:46:58.000000 humiolib-0.2.4/src/humiolib/cli.py
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.811428 humiolib-0.2.4/src/humiolib.egg-info/
--rw-r--r--   0 abrandborg   (501) staff       (20)     6941 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/PKG-INFO
--rw-r--r--   0 abrandborg   (501) staff       (20)     2139 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/SOURCES.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)        1 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/dependency_links.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)       48 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/entry_points.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)        1 2021-08-13 06:53:20.000000 humiolib-0.2.4/src/humiolib.egg-info/not-zip-safe
--rw-r--r--   0 abrandborg   (501) staff       (20)       22 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/requires.txt
--rw-r--r--   0 abrandborg   (501) staff       (20)        9 2022-08-15 10:36:26.000000 humiolib-0.2.4/src/humiolib.egg-info/top_level.txt
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.812345 humiolib-0.2.4/tests/
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.792179 humiolib-0.2.4/tests/cassettes/
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.817191 humiolib-0.2.4/tests/cassettes/humioclient/
--rw-r--r--   0 abrandborg   (501) staff       (20)      920 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_create_queryjob_incorrect_query_syntax
--rw-r--r--   0 abrandborg   (501) staff       (20)     1066 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_create_queryjob_success
--rw-r--r--   0 abrandborg   (501) staff       (20)      935 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_get_status
--rw-r--r--   0 abrandborg   (501) staff       (20)      824 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_get_users
--rw-r--r--   0 abrandborg   (501) staff       (20)     1119 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_json_on_humioclient_success
--rw-r--r--   0 abrandborg   (501) staff       (20)     1117 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_json_on_ingestclient_success
--rw-r--r--   0 abrandborg   (501) staff       (20)     1283 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_messages_on_humioclient_success
--rw-r--r--   0 abrandborg   (501) staff       (20)     1274 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_messages_on_ingestclient_ssuccess
--rw-r--r--   0 abrandborg   (501) staff       (20)     1625 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/humioclient/test_streaming_query_success
-drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2022-08-15 10:36:26.822383 humiolib-0.2.4/tests/cassettes/queryjob/
--rw-r--r--   0 abrandborg   (501) staff       (20)     3965 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob
--rw-r--r--   0 abrandborg   (501) staff       (20)     5286 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_after_fully_polled_fail
--rw-r--r--   0 abrandborg   (501) staff       (20)     3965 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_aggregate_query
--rw-r--r--   0 abrandborg   (501) staff       (20)     4909 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_non_aggregate_query
--rw-r--r--   0 abrandborg   (501) staff       (20)     7546 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_poll_after_done_success
--rw-r--r--   0 abrandborg   (501) staff       (20)     4664 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob
--rw-r--r--   0 abrandborg   (501) staff       (20)     3185 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_after_fully_polled_fail
--rw-r--r--   0 abrandborg   (501) staff       (20)     3185 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_aggregate_query
--rw-r--r--   0 abrandborg   (501) staff       (20)     4125 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_non_aggregate_query
--rw-r--r--   0 abrandborg   (501) staff       (20)     4248 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/test_humioclient.py
--rw-r--r--   0 abrandborg   (501) staff       (20)     3202 2021-08-13 06:46:58.000000 humiolib-0.2.4/tests/test_queryjob.py
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.674568 humiolib-0.2.5/
+-rw-r--r--   0 abrandborg   (501) staff       (20)      156 2023-04-17 08:45:21.000000 humiolib-0.2.5/.bumpversion.cfg
+-rw-r--r--   0 abrandborg   (501) staff       (20)      726 2023-04-17 08:43:17.000000 humiolib-0.2.5/AUTHORS.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1438 2023-04-17 09:13:03.000000 humiolib-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)     7475 2021-08-13 06:46:58.000000 humiolib-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)    11406 2021-08-13 06:46:58.000000 humiolib-0.2.5/LICENSE
+-rw-r--r--   0 abrandborg   (501) staff       (20)      245 2021-08-13 06:46:58.000000 humiolib-0.2.5/MANIFEST.in
+-rw-r--r--   0 abrandborg   (501) staff       (20)     7121 2023-04-17 09:13:11.674821 humiolib-0.2.5/PKG-INFO
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4842 2023-04-17 09:07:05.000000 humiolib-0.2.5/README.rst
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.640319 humiolib-0.2.5/docs/
+-rw-r--r--   0 abrandborg   (501) staff       (20)       28 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/authors.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)       30 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/changelog.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)      825 2023-04-17 08:45:21.000000 humiolib-0.2.5/docs/conf.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)       33 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/contributing.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)      220 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/index.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)       27 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/readme.rst
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.644472 humiolib-0.2.5/docs/reference/
+-rw-r--r--   0 abrandborg   (501) staff       (20)       91 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/reference/humioclient.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)      103 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/reference/humioexceptions.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)      113 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/reference/index.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)       75 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/reference/queryjob.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)       79 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/reference/webcaller.rst
+-rw-r--r--   0 abrandborg   (501) staff       (20)       29 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/requirements.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)      109 2021-08-13 06:46:58.000000 humiolib-0.2.5/docs/spelling_wordlist.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)      504 2023-04-17 09:13:11.676024 humiolib-0.2.5/setup.cfg
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3026 2023-04-17 08:45:21.000000 humiolib-0.2.5/setup.py
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.621644 humiolib-0.2.5/src/
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.650049 humiolib-0.2.5/src/humiolib/
+-rw-r--r--   0 abrandborg   (501) staff       (20)    29582 2023-04-17 08:41:13.000000 humiolib-0.2.5/src/humiolib/HumioClient.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)      500 2021-08-13 06:46:58.000000 humiolib-0.2.5/src/humiolib/HumioExceptions.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)     7523 2021-08-13 07:06:27.000000 humiolib-0.2.5/src/humiolib/QueryJob.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4749 2022-08-15 10:30:31.000000 humiolib-0.2.5/src/humiolib/WebCaller.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)       85 2023-04-17 08:45:21.000000 humiolib-0.2.5/src/humiolib/__init__.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)      364 2021-08-13 06:46:58.000000 humiolib-0.2.5/src/humiolib/__main__.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4100 2021-08-13 06:46:58.000000 humiolib-0.2.5/src/humiolib/cli.py
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.655899 humiolib-0.2.5/src/humiolib.egg-info/
+-rw-r--r--   0 abrandborg   (501) staff       (20)     7121 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/PKG-INFO
+-rw-r--r--   0 abrandborg   (501) staff       (20)     2139 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/SOURCES.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)        1 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/dependency_links.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)       47 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/entry_points.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)        1 2021-08-13 06:53:20.000000 humiolib-0.2.5/src/humiolib.egg-info/not-zip-safe
+-rw-r--r--   0 abrandborg   (501) staff       (20)       22 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/requires.txt
+-rw-r--r--   0 abrandborg   (501) staff       (20)        9 2023-04-17 09:13:11.000000 humiolib-0.2.5/src/humiolib.egg-info/top_level.txt
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.657217 humiolib-0.2.5/tests/
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.624203 humiolib-0.2.5/tests/cassettes/
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.664105 humiolib-0.2.5/tests/cassettes/humioclient/
+-rw-r--r--   0 abrandborg   (501) staff       (20)      920 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_create_queryjob_incorrect_query_syntax
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1066 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_create_queryjob_success
+-rw-r--r--   0 abrandborg   (501) staff       (20)      935 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_get_status
+-rw-r--r--   0 abrandborg   (501) staff       (20)      824 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_get_users
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1119 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_json_on_humioclient_success
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1117 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_json_on_ingestclient_success
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1283 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_messages_on_humioclient_success
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1274 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_messages_on_ingestclient_ssuccess
+-rw-r--r--   0 abrandborg   (501) staff       (20)     1625 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/humioclient/test_streaming_query_success
+drwxr-xr-x   0 abrandborg   (501) staff       (20)        0 2023-04-17 09:13:11.673752 humiolib-0.2.5/tests/cassettes/queryjob/
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3965 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob
+-rw-r--r--   0 abrandborg   (501) staff       (20)     5286 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_after_fully_polled_fail
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3965 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_aggregate_query
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4909 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_non_aggregate_query
+-rw-r--r--   0 abrandborg   (501) staff       (20)     7546 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_poll_after_done_success
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4664 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3185 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_after_fully_polled_fail
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3185 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_aggregate_query
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4125 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_non_aggregate_query
+-rw-r--r--   0 abrandborg   (501) staff       (20)     4248 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/test_humioclient.py
+-rw-r--r--   0 abrandborg   (501) staff       (20)     3202 2021-08-13 06:46:58.000000 humiolib-0.2.5/tests/test_queryjob.py
```

### Comparing `humiolib-0.2.4/CHANGELOG.rst` & `humiolib-0.2.5/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -49,8 +49,15 @@
 
 0.2.4 (2022-08-15)
 ******************
 Smaller file related bugfixes
 Changed:
 
     * upload_file function no longer attempts a cast to json 
-    * list_files function now works on newer versions of humio
+    * list_files function now works on newer versions of humio
+
+0.2.5 (2023-04-17)
+******************
+Expand file functionality
+Changed:
+
+    * Added additional endpoints for manipulating files via GraphQL
```

### Comparing `humiolib-0.2.4/CONTRIBUTING.rst` & `humiolib-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/LICENSE` & `humiolib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/PKG-INFO` & `humiolib-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: humiolib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python SDK for connecting to Humio
 Home-page: https://github.com/humio/python-humio
 Author: Humio ApS
 Author-email: integrations@humio.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-humio.readthedocs.io/
 Project-URL: Changelog, https://python-humio.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/humio/python-humio/issues
 Keywords: humio,log management
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -115,43 +114,43 @@
 HumioIngestClient
 *****************
 The HumioIngestClient class is used for ingesting data into Humio.
 While the HumioClient can also be used for ingesting data, this is mainly meant for debugging.
  
 .. code-block:: python
 
-  from humiolib.HumioClient import HumioIngestClient
+   from humiolib.HumioClient import HumioIngestClient
  
- # Creating the client
- client = HumioIngestClient(
-    base_url= "https://cloud.humio.com",
-    ingest_token="*****")
- 
- # Ingesting Unstructured Data
- messages = [
-       "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
-       "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
-   ]
- 
- client.ingest_messages(messages) 
- 
- # Ingesting Structured Data
- structured_data = [
-       {
-           "tags": {"host": "server1" },
-           "events": [
-               {
-                   "timestamp": "2020-03-23T00:00:00+00:00",
-                   "attributes": {"key1": "value1", "key2": "value2"}      
-               }
-           ]
-       }
-   ]
- 
- client.ingest_json_data(structured_data)
+   # Creating the client
+   client = HumioIngestClient(
+      base_url= "https://cloud.humio.com",
+      ingest_token="*****")
+   
+   # Ingesting Unstructured Data
+   messages = [
+         "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
+         "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
+      ]
+   
+   client.ingest_messages(messages) 
+   
+   # Ingesting Structured Data
+   structured_data = [
+         {
+            "tags": {"host": "server1" },
+            "events": [
+                  {
+                     "timestamp": "2020-03-23T00:00:00+00:00",
+                     "attributes": {"key1": "value1", "key2": "value2"}      
+                  }
+            ]
+         }
+      ]
+   
+   client.ingest_json_data(structured_data)
  
 
 
 Changelog
 =========
 
 0.2.0 (2020-03-30)
@@ -203,7 +202,13 @@
 ******************
 Smaller file related bugfixes
 Changed:
 
     * upload_file function no longer attempts a cast to json 
     * list_files function now works on newer versions of humio
 
+0.2.5 (2023-04-17)
+******************
+Expand file functionality
+Changed:
+
+    * Added additional endpoints for manipulating files via GraphQL
```

### Comparing `humiolib-0.2.4/README.rst` & `humiolib-0.2.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,37 +98,37 @@
 HumioIngestClient
 *****************
 The HumioIngestClient class is used for ingesting data into Humio.
 While the HumioClient can also be used for ingesting data, this is mainly meant for debugging.
  
 .. code-block:: python
 
-  from humiolib.HumioClient import HumioIngestClient
+   from humiolib.HumioClient import HumioIngestClient
  
- # Creating the client
- client = HumioIngestClient(
-    base_url= "https://cloud.humio.com",
-    ingest_token="*****")
- 
- # Ingesting Unstructured Data
- messages = [
-       "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
-       "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
-   ]
- 
- client.ingest_messages(messages) 
- 
- # Ingesting Structured Data
- structured_data = [
-       {
-           "tags": {"host": "server1" },
-           "events": [
-               {
-                   "timestamp": "2020-03-23T00:00:00+00:00",
-                   "attributes": {"key1": "value1", "key2": "value2"}      
-               }
-           ]
-       }
-   ]
- 
- client.ingest_json_data(structured_data)
+   # Creating the client
+   client = HumioIngestClient(
+      base_url= "https://cloud.humio.com",
+      ingest_token="*****")
+   
+   # Ingesting Unstructured Data
+   messages = [
+         "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
+         "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
+      ]
+   
+   client.ingest_messages(messages) 
+   
+   # Ingesting Structured Data
+   structured_data = [
+         {
+            "tags": {"host": "server1" },
+            "events": [
+                  {
+                     "timestamp": "2020-03-23T00:00:00+00:00",
+                     "attributes": {"key1": "value1", "key2": "value2"}      
+                  }
+            ]
+         }
+      ]
+   
+   client.ingest_json_data(structured_data)
```

### Comparing `humiolib-0.2.4/docs/conf.py` & `humiolib-0.2.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "humiolib"
 year = "2020"
 author = "Humio ApS"
 copyright = "{0}, {1}".format(year, author)
-version = "0.2.4"
+version = "0.2.5"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/humio/python-humio/issues/%s", "#"),
     "pr": ("https://github.com/humio/python-humio/pulls/%s", "PR #"),
 }
```

### Comparing `humiolib-0.2.4/setup.py` & `humiolib-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     with io.open(
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 setup(
     name="humiolib",
-    version="0.2.4",
+    version="0.2.5",
     license="Apache-2.0",
     description="Python SDK for connecting to Humio",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
```

### Comparing `humiolib-0.2.4/src/humiolib/HumioClient.py` & `humiolib-0.2.5/src/humiolib/HumioClient.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import json
 from humiolib.WebCaller import WebCaller, WebStreamer
 from humiolib.QueryJob import StaticQueryJob, LiveQueryJob
 from humiolib.HumioExceptions import HumioConnectionException
 
+
 class BaseHumioClient():
     """
     Base class for other client types, is not meant to be instantiated
     """
 
     def __init__(self, base_url):
         self.base_url = base_url
@@ -52,15 +53,15 @@
                 ("type", parser),
                 ("fields", fields),
                 ("tags", tags),
             ]
             if v is not None
         )
 
-    
+
 class HumioClient(BaseHumioClient):
     """
     A Humio client that gives full access to the underlying API.
     While this client can be used for ingesting data,
     we recommend using the HumioIngestClient made exclusivly for ingestion.
     """
 
@@ -77,19 +78,18 @@
         :type user_token: str
         :param base_url: Url of Humio instance
         :type repository: str
         """
         super().__init__(base_url)
         self.repository = repository
         self.user_token = user_token
-        
 
     @property
     def _default_user_headers(self):
-        """ 
+        """
         :return: Default headers used for web requests
         :rtype: dict
         """
         return {
             "Content-Type": "application/json",
             "Authorization": "Bearer {}".format(self.user_token),
         }
@@ -104,15 +104,14 @@
             {
                 "user_token": self.user_token,
                 "repository": self.repository,
                 "base_url": self.base_url,
             }
         )
 
-
     def _streaming_query(
         self,
         query_string,
         start=None,
         end=None,
         is_live=None,
         timezone_offset_minutes=None,
@@ -148,21 +147,20 @@
                 ("arguments", arguments),
             ]
             if v is not None
         )
 
         data.update(raw_data)
 
-
         connection = self.webcaller.call_rest(
             "post", endpoint, data=json.dumps(data), headers=headers, stream=True, **kwargs
         )
 
         return WebStreamer(connection)
-    
+
     # Wrap method to be pythonic
     def streaming_query(
         self,
         query_string,
         start=None,
         end=None,
         is_live=None,
@@ -209,15 +207,14 @@
             media_type=media_type,
             raw_data=raw_data,
             **kwargs
         )
 
         for event in res:
             yield json.loads(event.decode(encoding))
-                
 
     def create_queryjob(
         self,
         query_string,
         start=None,
         end=None,
         is_live=None,
@@ -226,15 +223,15 @@
         raw_data=None,
         **kwargs
     ):
         """
         Creates a queryjob on Humio, which executes asynchronously of the calling code.
         The returned QueryJob instance can be used to get the query results at a later time.
         Queryjobs are good to use for live queries, or static queries that return smaller
-        amounts of data. 
+        amounts of data.
 
         :param query_string: Humio query
         :type query_string: str
         :param start: Starting time of query
         :type start: Union[int, str], optional
         :param end: Ending time of query
         :type end: Union[int, str], optional
@@ -242,15 +239,15 @@
         :type is_live: bool, optional
         :param is_live: Timezone offset in minutes
         :type is_live: int, optional
         :param argument: Arguments specified in query
         :type argument: dict(string->string), optional
         :param raw_data: Additional arguments to add to POST body under other keys
         :type raw_data: dict(string->string), optional
-        
+
         :return:  An instance that grants access to the created queryjob and associated results
         :rtype: QueryJob
         """
 
         endpoint = "dataspaces/{}/queryjobs".format(self.repository)
 
         headers = self._default_user_headers
@@ -269,23 +266,22 @@
             if v is not None
         )
 
         if raw_data is not None:
             data.update(raw_data)
 
         query_id = self.webcaller.call_rest(
-            "post", endpoint,  data=json.dumps(data), headers=headers, **kwargs
-            ).json()['id']
-        
+            "post", endpoint, data=json.dumps(data), headers=headers, **kwargs
+        ).json()['id']
+
         if is_live:
             return LiveQueryJob(query_id, self.base_url, self.repository, self.user_token)
         else:
             return StaticQueryJob(query_id, self.base_url, self.repository, self.user_token)
 
-
     def _ingest_json_data(self, json_elements=None, **kwargs):
         """
         Ingest structured json data to repository.
         Structure of ingested data is discussed in: https://docs.humio.com/reference/api/ingest/#structured-data
 
         :param messages: A list of event strings.
         :type messages: list(string), optional
@@ -295,15 +291,15 @@
         :type fields: dict(string->string), optional
         :param tags:  Tags to associate with the messages.
         :type tags: dict(string->string), optional
 
         :return: Response to web request as json string
         :rtype: str
         """
-        
+
         if json_elements is None:
             json_elements = []
 
         headers = self._default_user_headers
         headers.update(kwargs.pop("headers", {}))
 
         endpoint = "dataspaces/{}/ingest".format(self.repository)
@@ -339,16 +335,16 @@
 
         headers = self._default_user_headers
         headers.update(kwargs.pop("headers", {}))
 
         endpoint = "dataspaces/{}/ingest-messages".format(self.repository)
 
         obj = self._create_unstructured_data_object(
-                messages, parser=parser, fields=fields, tags=tags
-            )
+            messages, parser=parser, fields=fields, tags=tags
+        )
 
         return self.webcaller.call_rest(
             "post", endpoint, data=json.dumps([obj]), headers=headers, **kwargs
         )
 
     # Wrap method to be pythonic
     ingest_messages = WebCaller.response_as_json(_ingest_messages)
@@ -464,15 +460,15 @@
         """
 
         headers = self._default_user_headers
         request = {
             "query": "query {organizations{id, name, description}}",
             "variables": None,
         }
-        
+
         return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
 
     # Wrap method to be pythonic
     def list_organizations(self):
         resp = self._list_organizations()
         return resp.json()["data"]["organizations"]
 
@@ -506,75 +502,306 @@
         """
         Upload file to repository
 
         :param filepath: Path to file.
         :type filepath: string
 
         :return: Response to web request
-        :rtype: Response
+        :rtype: Response Object
         """
 
         endpoint = "dataspaces/{}/files".format(self.repository)
-        headers = {"Authorization": "Bearer {}".format(self.user_token)} # Not using default headers as files are sent
+        headers = {"Authorization": "Bearer {}".format(self.user_token)}  # Not using default headers as files are sent
         with open(filepath, "rb") as f:
             return self.webcaller.call_rest("post", endpoint, files={"file": f}, headers=headers)
 
     # Wrap method to be pythonic
     # The uploaded files endpoint currently doesn't return JSON, thus this function doesn't attempt to cast to json.
     def upload_file(self, filepath):
         return self._upload_file(filepath)
 
+    def _create_file(self, file_name):
+        """
+        Create new file.
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :return: Response to web request
+        :rtype: Response Object
+        """
+
+        headers = self._default_user_headers
+        request = {
+            "query": "mutation($fileName : String!, $repo : String!){newFile(fileName: $fileName, name: $repo){nameAndPath { name, path}}}",
+            "variables": {"fileName": file_name, "repo": self.repository},
+        }
+        return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
+
+    def create_file(self, file_name):
+        """
+        Create new file.
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :return: Response data to web request as json string
+        :rtype: str
+        """
+
+        resp = self._create_file(file_name)
+        return resp.json()["data"]
+
     def _list_files(self):
         """
         List uploaded files on repository
 
-        :return: Response to web request as json string
-        :rtype: str
+        :return: Response to web request
+        :rtype: Response Object
         """
 
         headers = self._default_user_headers
         request = {
             "query": "query {{searchDomain(name: {}){{files {{nameAndPath {{path, name}} }} }} }}".format(
                 json.dumps(self.repository)
             ),
             "variables": None,
         }
         return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
 
     def list_files(self):
+        """
+        List uploaded files on repository
+
+        :return: Response to web request as json string
+        :rtype: str
+        """
+
         resp = self._list_files()
         return resp.json()["data"]["searchDomain"]["files"]
 
+    def _get_file_content(self, file_name, offset, limit, filter_string=None):
+        """
+        Get the contents of a file
+
+        :param file_name: Name of file.
+        :type name: string
+
+        :param offset: Starting index to replace the old rows with the updated ones.
+        :type offset: int
+
+        :param limit: Used to find when to stop replacing rows, by adding the limit to the offset
+        :type limit: int
+
+        :param filter_string: Used to apply a filter string
+        :type filter_string: string, optional
+
+        :return: Response to web request
+        :rtype: Response Object
+        """
+
+        headers = self._default_user_headers
+
+        if filter_string is not None:
+            request = {
+                "query": "query {{"
+                            "getFileContent(name: {}, fileName: \"{}\", offset: {}, limit: {}, filterString: \"{}\") {{ "
+                                "totalLinesCount, limit, offset, headers, lines}} "
+                            "}}".format(json.dumps(self.repository), file_name, offset, limit, filter_string),
+                "variables": None,
+            }
+        else:
+            request = {
+                "query": "query {{"
+                            "getFileContent(name: {}, fileName: \"{}\", offset: {}, limit: {}) {{ "
+                                "totalLinesCount, limit, offset, headers, lines}} "
+                            "}}".format(json.dumps(self.repository), file_name, offset, limit),
+                "variables": None,
+            }
+
+        return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
+
+    def get_file_content(self, filename, offset=0, limit=200, filter_string=None):
+        """
+        Get the contents of a file
+
+        :param file_name: Name of file.
+        :type name: string
+
+        :param offset: Starting index to replace the old rows with the updated ones.
+        :type offset: int
+
+        :param limit: Used to find when to stop replacing rows, by adding the limit to the offset
+        :type limit: int
+
+        :param filter_string: Used to apply a filter string
+        :type filter_string: string, optional
+
+        :return: Response to web request as json string
+        :rtype: str
+        """
+
+        resp = self._get_file_content(filename, offset=offset, limit=limit, filter_string=filter_string)
+        return resp.json()["data"]
+
     def _get_file(self, file_name):
         """
         Get specific file on repository
 
         :param file_name: Name of file to get.
         :type file_name: string
 
         :return: Response to web request as json string
-        :rtype: str
+        :rtype: Response Object
         """
         endpoint = "dataspaces/{}/files/{}".format(self.repository, file_name)
-        headers = {"Authorization": "Bearer {}".format(self.user_token)} # Not using default headers as files are sent
+        headers = {"Authorization": "Bearer {}".format(self.user_token)}  # Not using default headers as files are sent
         return self.webcaller.call_rest("get", endpoint, headers=headers)
 
     def get_file(self, file_name, encoding=None):
+        """
+        Get specific file on repository
+
+        :param file_name: Name of file to get.
+        :type file_name: string
+
+        :return: Response to web request as json string
+        :rtype: str
+        """
         resp = self._get_file(file_name)
         raw_data = resp.content
         if encoding is None:
             return raw_data
         else:
             return raw_data.decode("utf-8")
 
+    def _delete_file(self, file_name):
+        """
+        Delete an existing file.
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :return: Response to web request
+        :rtype: Response Object
+        """
+
+        headers = self._default_user_headers
+        request = {
+            "query": "mutation($fileName : String!, $repo : String!){removeFile(fileName: $fileName, name: $repo){ __typename}}",
+            "variables": {"fileName": file_name, "repo": self.repository},
+        }
+        return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
+
+    def delete_file(self, file_name):
+        """
+        Delete an existing file.
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :return: Response to web request as json string
+        :rtype: str
+        """
+
+        resp = self._delete_file(file_name)
+        return resp.json()["data"]
+
+    def _update_file_contents(self, file_name, file_headers, changed_rows, column_changes=[], offset=0, limit=200):
+        """
+        Add contents to a file
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :param file_headers: Headers of the file
+        :type file_headers: list
+
+        :param changed_rows: Rows within the offset and limit to overwrite existing rows
+        :type changed_rows: list
+
+        :param column_changes: Column changes that will be applied to all rows in the file
+        :type column_changes: list, optional
+
+        :param offset: Starting index to replace the old rows with the updated ones.
+        :type offset: int, optional
+
+        :param limit: Used to find when to stop adding rows, by adding the limit to the offset
+        :type limit: int, optional
+
+        :return: Response data to web request
+        :rtype: Response Object
+        """
+
+        headers = self._default_user_headers
+        request = {
+            "query": "mutation ($fileName: String!, $name: String!, $changedRows: [[String!]!]!, $headers: [String!]!, $columnChanges: [ColumnChange!]!, $limit: Int, $offset: Int) {updateFile(limit: $limit, offset: $offset, fileName: $fileName, name: $name, changedRows: $changedRows, headers: $headers, columnChanges: $columnChanges) {offset, limit, totalLinesCount, headers, lines, nameAndPath {name, path } } }",
+            "variables": {"name": self.repository, "fileName": file_name, "changedRows": changed_rows,
+                          "headers": file_headers,
+                          "columnChanges": column_changes, "offset": offset, "limit": limit}
+        }
+
+        return self.webcaller.call_graphql(headers=headers, data=json.dumps(request))
+
+    def add_file_contents(self, file_name, file_headers, changed_rows, column_changes=[], offset=0, limit=200):
+        """
+        Add contents to a file
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :param file_headers: Headers of the file
+        :type file_headers: list
+
+        :param changed_rows: Rows within the offset and limit to overwrite existing rows
+        :type changed_rows: list
+
+        :param column_changes: Column changes that will be applied to all rows in the file
+        :type column_changes: list, optional
+
+        :param offset: Starting index to replace the old rows with the updated ones.
+        :type offset: int, optional
+
+        :param limit: Used to determine when to stop replacing rows, by adding the limit to the offset
+        :type limit: int, optional
+
+        :return: Response data to web request as json string
+        :rtype: str
+        """
+
+        resp = self._update_file_contents(file_name, file_headers, changed_rows, column_changes, offset, limit)
+        return resp.json()["data"]
+
+    def remove_file_contents(self, file_name, offset=0, limit=200):
+        """
+        Remove contents of a file
+
+        :param file_name: Name of file
+        :type file_name: string
+
+        :param offset: Starting index to replace the old rows with the updated ones.
+        :type offset: int, optional
+
+        :param limit: Used to find when to stop replacing rows, by adding the limit to the offset
+        :type limit: int, optional
+
+        :return: Response data to web request as json string
+        :rtype: str
+        """
+
+        resp = self._update_file_contents(file_name, file_headers=[], offset=offset, limit=limit, changed_rows=[],
+                                          column_changes=[])
+        return resp.json()["data"]
+
 
 class HumioIngestClient(BaseHumioClient):
     """
     A Humio client that is used exclusivly for ingesting data
     """
+
     def __init__(
         self,
         ingest_token,
         base_url="http://localhost:3000",
     ):
         """
         :param ingest_token: Ingest token to access ingest.
@@ -584,15 +811,15 @@
         """
         super().__init__(base_url)
         self.ingest_token = ingest_token
         self.webcaller = WebCaller(self.base_url)
 
     @property
     def _default_ingest_headers(self):
-        """ 
+        """
         :return: Default headers used for web requests
         :rtype: dict
         """
 
         return {
             "Content-Type": "application/json",
             "Authorization": "Bearer {}".format(self.ingest_token),
@@ -615,15 +842,15 @@
     def _ingest_json_data(self, json_elements=None, **kwargs):
         """
         Ingest structured json data to repository.
         Structure of ingested data is discussed in: https://docs.humio.com/reference/api/ingest/#structured-data
 
         :param json_elements: Structured data that can be parsed to a json string.
         :type json_elements: str
-        
+
         :return: Response to web request as json string
         :rtype: str
         """
 
         if json_elements is None:
             json_elements = []
 
@@ -654,24 +881,24 @@
         :type fields: dict(string->string), optional
         :param tags:  Tags to associate with the messages.
         :type tags: dict(string->string), optional
 
         :return: Response to web request as json string
         :rtype: str
         """
-        
+
         if messages is None:
             messages = []
 
         headers = self._default_ingest_headers
         headers.update(kwargs.pop("headers", {}))
 
-        endpoint = "ingest/humio-unstructured" 
+        endpoint = "ingest/humio-unstructured"
 
         obj = self._create_unstructured_data_object(
-                messages, parser=parser, fields=fields, tags=tags
-            )
+            messages, parser=parser, fields=fields, tags=tags
+        )
 
-        return self.webcaller.call_rest("post", endpoint, data=json.dumps([obj]), headers=headers) 
+        return self.webcaller.call_rest("post", endpoint, data=json.dumps([obj]), headers=headers)
 
     # Wrap method to be pythonic
     ingest_messages = WebCaller.response_as_json(_ingest_messages)
```

### Comparing `humiolib-0.2.4/src/humiolib/QueryJob.py` & `humiolib-0.2.5/src/humiolib/QueryJob.py`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/src/humiolib/WebCaller.py` & `humiolib-0.2.5/src/humiolib/WebCaller.py`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/src/humiolib/cli.py` & `humiolib-0.2.5/src/humiolib/cli.py`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/src/humiolib.egg-info/PKG-INFO` & `humiolib-0.2.5/src/humiolib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: humiolib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python SDK for connecting to Humio
 Home-page: https://github.com/humio/python-humio
 Author: Humio ApS
 Author-email: integrations@humio.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-humio.readthedocs.io/
 Project-URL: Changelog, https://python-humio.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/humio/python-humio/issues
 Keywords: humio,log management
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -115,43 +114,43 @@
 HumioIngestClient
 *****************
 The HumioIngestClient class is used for ingesting data into Humio.
 While the HumioClient can also be used for ingesting data, this is mainly meant for debugging.
  
 .. code-block:: python
 
-  from humiolib.HumioClient import HumioIngestClient
+   from humiolib.HumioClient import HumioIngestClient
  
- # Creating the client
- client = HumioIngestClient(
-    base_url= "https://cloud.humio.com",
-    ingest_token="*****")
- 
- # Ingesting Unstructured Data
- messages = [
-       "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
-       "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
-   ]
- 
- client.ingest_messages(messages) 
- 
- # Ingesting Structured Data
- structured_data = [
-       {
-           "tags": {"host": "server1" },
-           "events": [
-               {
-                   "timestamp": "2020-03-23T00:00:00+00:00",
-                   "attributes": {"key1": "value1", "key2": "value2"}      
-               }
-           ]
-       }
-   ]
- 
- client.ingest_json_data(structured_data)
+   # Creating the client
+   client = HumioIngestClient(
+      base_url= "https://cloud.humio.com",
+      ingest_token="*****")
+   
+   # Ingesting Unstructured Data
+   messages = [
+         "192.168.1.21 - user1 [02/Nov/2017:13:48:26 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.015 664 0.015",
+         "192.168.1..21 - user2 [02/Nov/2017:13:49:09 +0000] \"POST /humio/api/v1/ingest/elastic-bulk HTTP/1.1\" 200 0 \"-\" \"useragent\" 0.013 565 0.013"
+      ]
+   
+   client.ingest_messages(messages) 
+   
+   # Ingesting Structured Data
+   structured_data = [
+         {
+            "tags": {"host": "server1" },
+            "events": [
+                  {
+                     "timestamp": "2020-03-23T00:00:00+00:00",
+                     "attributes": {"key1": "value1", "key2": "value2"}      
+                  }
+            ]
+         }
+      ]
+   
+   client.ingest_json_data(structured_data)
  
 
 
 Changelog
 =========
 
 0.2.0 (2020-03-30)
@@ -203,7 +202,13 @@
 ******************
 Smaller file related bugfixes
 Changed:
 
     * upload_file function no longer attempts a cast to json 
     * list_files function now works on newer versions of humio
 
+0.2.5 (2023-04-17)
+******************
+Expand file functionality
+Changed:
+
+    * Added additional endpoints for manipulating files via GraphQL
```

### Comparing `humiolib-0.2.4/src/humiolib.egg-info/SOURCES.txt` & `humiolib-0.2.5/src/humiolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_create_queryjob_incorrect_query_syntax` & `humiolib-0.2.5/tests/cassettes/humioclient/test_create_queryjob_incorrect_query_syntax`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_create_queryjob_success` & `humiolib-0.2.5/tests/cassettes/humioclient/test_create_queryjob_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_get_status` & `humiolib-0.2.5/tests/cassettes/humioclient/test_get_status`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_get_users` & `humiolib-0.2.5/tests/cassettes/humioclient/test_get_users`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_json_on_humioclient_success` & `humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_json_on_humioclient_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_json_on_ingestclient_success` & `humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_json_on_ingestclient_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_messages_on_humioclient_success` & `humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_messages_on_humioclient_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_ingest_messages_on_ingestclient_ssuccess` & `humiolib-0.2.5/tests/cassettes/humioclient/test_ingest_messages_on_ingestclient_ssuccess`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/humioclient/test_streaming_query_success` & `humiolib-0.2.5/tests/cassettes/humioclient/test_streaming_query_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_after_fully_polled_fail` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_after_fully_polled_fail`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_aggregate_query` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_aggregate_query`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_non_aggregate_query` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_non_aggregate_query`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_poll_after_done_success` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_live_queryjob_poll_after_done_success`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_after_fully_polled_fail` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_after_fully_polled_fail`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_aggregate_query` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_aggregate_query`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_non_aggregate_query` & `humiolib-0.2.5/tests/cassettes/queryjob/test_poll_until_done_static_queryjob_non_aggregate_query`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/test_humioclient.py` & `humiolib-0.2.5/tests/test_humioclient.py`

 * *Files identical despite different names*

### Comparing `humiolib-0.2.4/tests/test_queryjob.py` & `humiolib-0.2.5/tests/test_queryjob.py`

 * *Files identical despite different names*

