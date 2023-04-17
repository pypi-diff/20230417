# Comparing `tmp/netin-1.0.5.tar.gz` & `tmp/netin-1.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.tar", last modified: Sun Apr 16 07:54:19 2023, max compression
+gzip compressed data, was "netin-1.0.5.1.tar", last modified: Mon Apr 17 10:13:08 2023, max compression
```

## Comparing `netin-1.0.5.tar` & `netin-1.0.5.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3703 2023-04-16 07:54:19.249805 netin-1.0.5/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.245805 netin-1.0.5/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.245805 netin-1.0.5/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.245805 netin-1.0.5/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.245805 netin-1.0.5/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      351 2023-04-16 07:51:41.000000 netin-1.0.5/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.5/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-15 19:20:18.000000 netin-1.0.5/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14275 2023-04-15 22:08:18.000000 netin-1.0.5/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3703 2023-04-16 07:54:19.000000 netin-1.0.5/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-16 07:54:19.000000 netin-1.0.5/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:54:19.000000 netin-1.0.5/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-16 07:54:19.000000 netin-1.0.5/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-16 07:54:19.000000 netin-1.0.5/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:54:19.249805 netin-1.0.5/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-16 07:54:19.249805 netin-1.0.5/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.1/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.1/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 10:13:08.793910 netin-1.0.5.1/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.1/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.1/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.1/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.1/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.1/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.1/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.1/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.1/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-17 10:09:56.000000 netin-1.0.5.1/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.1/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.1/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.1/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.1/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.1/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.1/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.1/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.1/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.1/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.1/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.1/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.1/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.1/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.1/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.1/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.1/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.1/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.1/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.1/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.1/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.1/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.1/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.5.1/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.1/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    15383 2023-04-17 10:09:00.000000 netin-1.0.5.1/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.1/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.1/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.1/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-17 10:13:08.793910 netin-1.0.5.1/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.1/setup.py
```

### Comparing `netin-1.0.5/LICENSE` & `netin-1.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/PKG-INFO` & `netin-1.0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5/README.rst` & `netin-1.0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/dh.py` & `netin-1.0.5.1/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/directed.py` & `netin-1.0.5.1/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/dpa.py` & `netin-1.0.5.1/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/dpah.py` & `netin-1.0.5.1/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/graph.py` & `netin-1.0.5.1/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/h.py` & `netin-1.0.5.1/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/pa.py` & `netin-1.0.5.1/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/pah.py` & `netin-1.0.5.1/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/patc.py` & `netin-1.0.5.1/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/patch.py` & `netin-1.0.5.1/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/tc.py` & `netin-1.0.5.1/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/tests/test_directed.py` & `netin-1.0.5.1/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/tests/test_dpah.py` & `netin-1.0.5.1/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/tests/test_patch.py` & `netin-1.0.5.1/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/tests/test_undirected.py` & `netin-1.0.5.1/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/generators/undirected.py` & `netin-1.0.5.1/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/stats/distributions.py` & `netin-1.0.5.1/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/stats/ranking.py` & `netin-1.0.5.1/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/utils/constants.py` & `netin-1.0.5.1/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/utils/validator.py` & `netin-1.0.5.1/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/netin/viz/handlers.py` & `netin-1.0.5.1/netin/viz/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,21 +118,21 @@
         ax.set_title(g.graph['model'])
 
     # legend
     _add_class_legend(fig, **kwargs)
     _save_plot(fig, fn, **kwargs)
 
 
-def plot_distribution(data: Union[pd.DataFrame, List[pd.DataFrame]], x: Union[str, List],
+def plot_distribution(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List],
                       get_x_y_from_df_fnc: callable, fn=None, **kwargs):
     iter_data = [data] if type(data) == pd.DataFrame else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_data), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
-    iter_column = [x] * (nc * nr) if type(x) == str else x
+    iter_column = [col_name] * (nc * nr) if type(col_name) == str else col_name
 
     scatter = kwargs.pop('scatter', False)
     hue = kwargs.pop('hue', None)
     sharex = kwargs.pop('sharex', False)
     sharey = kwargs.pop('sharey', False)
     xy_fnc_name = get_x_y_from_df_fnc.__name__
     ylabel = xy_fnc_name.replace("get_", '').upper()
@@ -155,59 +155,59 @@
 
     w, h = cell_size if type(cell_size) == tuple else (cell_size, cell_size)
     fig, axes = plt.subplots(nr, nc, figsize=(nc * w, nr * h), sharex=sharex, sharey=sharey)
 
     for cell, df in enumerate(iter_data):
         row = cell // nc
         col = cell % nc
-        x = iter_column[cell]
+        _col_name = iter_column[cell]
 
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
         class_label: str
-        iter_groups = df.group(hue) if hue is not None else [(None, df)]
+        iter_groups = df.groupby(hue) if hue is not None else [(None, df)]
         f_m = df.query("class_label == @const.MINORITY_LABEL").shape[0] / df.shape[0]
-        for class_label, data in iter_groups:
-            total = df[x].sum() if common_norm else data[x].sum()
-            xs, ys = get_x_y_from_df_fnc(data, x, total)
+        for class_label, group in iter_groups:
+            total = df[_col_name].sum() if common_norm else group[_col_name].sum()
+            xs, ys = get_x_y_from_df_fnc(group, _col_name, total)
             plot = ax.scatter if scatter else ax.plot
             plot(xs, ys, label=class_label, color=_get_class_label_color(class_label, xy_fnc_name), **kwargs)
 
             if hline_fnc:
-                hline_fnc(ax.axhline, data)
+                hline_fnc(ax.axhline, group)
             if vline_fnc:
-                vline_fnc(ax.axvline, data)
+                vline_fnc(ax.axvline, group)
             if me_fnc:
                 me_fnc(ax, f_m, ys, beta)
             if gini_fnc:
                 gini_fnc(ax, ys, cuts)
 
         if log_scale[0]:
             ax.set_xscale('log')
         if log_scale[1]:
             ax.set_yscale('log')
         if xlim:
             ax.set_xlim(xlim)
         if ylim:
             ax.set_ylim(ylim)
-
-        if (sharey and col == 0) or (not sharey):
+        if ylabel and ((sharey and col == 0) or (not sharey)):
             ax.set_ylabel(ylabel)
-
-        if (sharex and row == nr - 1) or (not sharex):
+        if xlabel is None:
+            ax.set_xlabel(_col_name)
+        elif (sharex and row == nr - 1) or (not sharex):
             ax.set_xlabel(xlabel)
 
         ax.set_title(df.name)
 
     # suptitle
     if suptitle is not None:
         fig.suptitle(suptitle)
 
     # legend
-    if class_label_legend:
+    if hue is not None and class_label_legend:
         _add_class_legend(fig, **kwargs)
 
     # save figure
     _save_plot(fig, fn, wspace=wspace, hspace=hspace, **kwargs)
 
 
 def _show_cuts(axline, data):
@@ -228,15 +228,15 @@
     kwargs['ylim'] = (0.0 - gap, 1.0 + gap)
     kwargs['xlim'] = (-1.0 - gap, 1.0 + gap)
     kwargs['scatter'] = True
     kwargs['hline_fnc'] = _show_cuts
     kwargs['vline_fnc'] = _show_beta
 
     plot_distribution(iter_data,
-                      x=x,
+                      col_name=x,
                       get_x_y_from_df_fnc=get_disparity,
                       fn=fn, **kwargs)
 
 
 def plot_gini_coefficient(iter_data: Union[pd.DataFrame, List[pd.DataFrame]], x: Union[str, List], fn=None, **kwargs):
     def show_gini(ax, ys, cuts):
         gini, x, y, va, ha, color = get_gini_label(ys, cuts)
@@ -268,15 +268,15 @@
     kwargs['hline_fnc'] = _show_cuts
     kwargs['gini_fnc'] = show_gini
     kwargs['xlabel'] = RANKING_LABEL
     kwargs['ylabel'] = GINI_TOPK_AXIS_LABEL
     kwargs['ylim'] = (-0.01, 1.01)
 
     plot_distribution(iter_data,
-                      x=x,
+                      col_name=x,
                       get_x_y_from_df_fnc=get_gini_coefficient,
                       fn=fn, **kwargs)
 
 
 def plot_fraction_of_minority(iter_data: Union[pd.DataFrame, List[pd.DataFrame]], x: Union[str, List],
                               fn=None, **kwargs):
     gap = 0.02
@@ -327,71 +327,93 @@
     kwargs['hline_fnc'] = show_minority
     kwargs['me_fnc'] = show_me
     kwargs['xlabel'] = RANKING_LABEL
     kwargs['ylabel'] = FM_TOPK_AXIS_LABEL
     kwargs['ylim'] = (0. - gap, 1. + gap)
 
     plot_distribution(iter_data,
-                      x=x,
+                      col_name=x,
                       get_x_y_from_df_fnc=get_fraction_of_minority,
                       fn=fn, **kwargs)
 
 
-def plot_powerlaw_fit(iter_data: Set[pd.DataFrame], x: str, kind: str, fn=None, **kwargs):
+def plot_powerlaw_fit(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List], kind: str,
+                      fn=None, **kwargs):
+
+    if kind not in TYPE_OF_DISTRIBUTION:
+        raise ValueError(f"kind must be one of {TYPE_OF_DISTRIBUTION}")
+
+    iter_data = [data] if type(data) == pd.DataFrame else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_data), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
+    iter_column = [col_name] * (nc * nr) if type(col_name) == str else col_name
 
-    hue = kwargs.pop('hue', None)
+    # whole plot
     sharex = kwargs.pop('sharex', False)
     sharey = kwargs.pop('sharey', False)
     log_scale = kwargs.pop('log_scale', (False, False))
-    ylabel = kwargs.pop('ylabel', "p(X≥x)" if kind == "ccdf" else "p(X<x)" if kind == 'cdf' else "p(X=x)")
+    xlabel = kwargs.pop('xlabel', None)
+    ylabel = kwargs.pop('ylabel', "p(X≥x)" if kind == "ccdf" else "p(X<x)" if kind == 'cdf' else "p(X=x)" if kind == 'pdf' else None)
     verbose = kwargs.pop('verbose', False)
-    bbox = kwargs.pop('bbox', (1.0, 0.9))
-    fontsize = kwargs.pop('fontsize', None)
     wspace = kwargs.pop('wspace', None)
     hspace = kwargs.pop('hspace', None)
 
+    # outer legend
+    hue = kwargs.pop('hue', None)
+    bbox = kwargs.pop('bbox', (1.0, 0.9))
+
+    # inner legend
+    fontsize = kwargs.pop('fontsize', None)
+    loc = kwargs.pop('loc', None)
+
+    # plot
     w, h = cell_size if type(cell_size) == tuple else (cell_size, cell_size)
     fig, axes = plt.subplots(nr, nc, figsize=(nc * w, nr * h), sharex=sharex, sharey=sharey)
 
     for cell, df in enumerate(iter_data):
         row = cell // nc
         col = cell % nc
+        _col_name = iter_column[cell]
 
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
         class_label: str
-        for class_label, data in df.groupby(hue):
-            data = data.query(f"{x}>0")
-            discrete = data[x].dtype == np.int64
-            fit = fit_power_law(data.loc[:, x].values, discrete=discrete, verbose=verbose)
+        iter_groups = df.groupby(hue) if hue is not None else [(None, df)]
+        for class_label, group in iter_groups:
+            group_nonzero = group.query(f"{_col_name}>0")
+            discrete = group_nonzero[_col_name].dtype == np.int64
+            fit = fit_power_law(group_nonzero.loc[:, _col_name].values, discrete=discrete, verbose=verbose)
 
             color = _get_class_label_color(class_label)
 
             efnc = fit.plot_ccdf if kind == "ccdf" else fit.plot_cdf if kind == 'cdf' else fit.plot_pdf
             fnc = fit.power_law.plot_ccdf if kind == "ccdf" else fit.power_law.plot_cdf if kind == 'cdf' \
                 else fit.power_law.plot_pdf
 
             ax = efnc(label=r"Empirical", ax=ax, color=color, **kwargs)
             ax = fnc(label=f'Powerlaw $\gamma={fit.alpha:.2f}$', linestyle='--', ax=ax, color=color, **kwargs)
 
+            # legend inside: empirical vs powerlaw
             handles, labels = ax.get_legend_handles_labels()
-            leg = ax.legend(handles, labels, loc=4 if kind == 'cdf' else 3, fontsize=fontsize)
+            loc = loc if loc is not None else 4 if kind == 'cdf' else 1
+            leg = ax.legend(handles, labels, loc=loc, fontsize=fontsize)
             leg.draw_frame(False)
 
         if log_scale[0]:
             ax.set_xscale('log')
         if log_scale[1]:
             ax.set_yscale('log')
-
-        if (sharey and col == 0) or (not sharey):
+        if ylabel is not None and ((sharey and col == 0) or (not sharey)):
             ax.set_ylabel(ylabel)
+        if xlabel is None:
+            ax.set_xlabel(_col_name)
+        elif (sharex and row == nr - 1) or (not sharex):
+            ax.set_xlabel(xlabel)
 
-        ax.set_xlabel(x)
         ax.set_title(df.name)
 
     # legend
-    kwargs['bbox'] = bbox
-    _add_class_legend(fig, **kwargs)
+    if hue:
+        kwargs['bbox'] = bbox
+        _add_class_legend(fig, **kwargs)
     _save_plot(fig, fn, wspace=wspace, hspace=hspace, **kwargs)
```

### Comparing `netin-1.0.5/netin.egg-info/PKG-INFO` & `netin-1.0.5.1/netin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5/netin.egg-info/SOURCES.txt` & `netin-1.0.5.1/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5/setup.py` & `netin-1.0.5.1/setup.py`

 * *Files identical despite different names*

