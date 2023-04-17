# Comparing `tmp/loganmatic-0.0.2.tar.gz` & `tmp/loganmatic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loganmatic-0.0.2.tar", last modified: Mon Apr 17 01:10:11 2023, max compression
+gzip compressed data, was "loganmatic-0.0.4.tar", last modified: Mon Apr 17 02:14:51 2023, max compression
```

## Comparing `loganmatic-0.0.2.tar` & `loganmatic-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 01:10:11.539640 loganmatic-0.0.2/
--rw-rw-rw-   0        0        0      451 2023-04-17 01:10:11.538642 loganmatic-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-17 00:29:43.000000 loganmatic-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 01:10:11.536649 loganmatic-0.0.2/loganmatic.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-17 01:10:11.000000 loganmatic-0.0.2/loganmatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-04-17 01:10:11.000000 loganmatic-0.0.2/loganmatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 01:10:11.000000 loganmatic-0.0.2/loganmatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 01:10:11.000000 loganmatic-0.0.2/loganmatic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 01:10:11.539640 loganmatic-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-04-17 01:09:05.000000 loganmatic-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.912364 loganmatic-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:14:51.910367 loganmatic-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.4/README.md
+-rw-rw-rw-   0        0        0      648 2023-04-17 02:12:16.000000 loganmatic-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:14:51.914388 loganmatic-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.880193 loganmatic-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.887376 loganmatic-0.0.4/src/loganmatic/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:04:58.000000 loganmatic-0.0.4/src/loganmatic/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.4/src/loganmatic/loganmatic.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.907463 loganmatic-0.0.4/src/loganmatic.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/top_level.txt
```

