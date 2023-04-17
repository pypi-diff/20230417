# Comparing `tmp/linesieve-1.0b1.tar.gz` & `tmp/linesieve-1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linesieve-1.0b1.tar", last modified: Mon Apr 10 15:49:57 2023, max compression
+gzip compressed data, was "linesieve-1.0b2.tar", last modified: Mon Apr 17 16:49:21 2023, max compression
```

## Comparing `linesieve-1.0b1.tar` & `linesieve-1.0b2.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.894449 linesieve-1.0b1/
--rw-r--r--   0 lemon      (501) staff       (20)     1475 2023-04-10 15:23:48.000000 linesieve-1.0b1/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)      172 2023-04-10 15:23:48.000000 linesieve-1.0b1/MANIFEST.in
--rw-r--r--   0 lemon      (501) staff       (20)    14355 2023-04-10 15:49:57.894786 linesieve-1.0b1/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)    13050 2023-04-10 15:45:50.000000 linesieve-1.0b1/README.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.748155 linesieve-1.0b1/docs/
--rw-r--r--   0 lemon      (501) staff       (20)      634 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/Makefile
--rw-r--r--   0 lemon      (501) staff       (20)      115 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/cli.rst
--rw-r--r--   0 lemon      (501) staff       (20)     1552 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/conf.py
--rw-r--r--   0 lemon      (501) staff       (20)      133 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/examples.rst
--rw-r--r--   0 lemon      (501) staff       (20)      358 2023-04-10 15:44:42.000000 linesieve-1.0b1/docs/index.rst
--rw-r--r--   0 lemon      (501) staff       (20)      800 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/make.bat
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.757811 linesieve-1.0b1/examples/
--rw-r--r--   0 lemon      (501) staff       (20)      580 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-compile-error.diff
--rw-r--r--   0 lemon      (501) staff       (20)      855 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-compile-error.txt
--rw-r--r--   0 lemon      (501) staff       (20)      633 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-failure.diff
--rw-r--r--   0 lemon      (501) staff       (20)     8340 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-failure.txt
--rw-r--r--   0 lemon      (501) staff       (20)     4878 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-success.txt
--rwxr-xr-x   0 lemon      (501) staff       (20)     1140 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-wrapper.sh
--rw-r--r--   0 lemon      (501) staff       (20)      376 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/git-options.sh
--rw-r--r--   0 lemon      (501) staff       (20)      607 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/java-traceback.sh
--rw-r--r--   0 lemon      (501) staff       (20)    10527 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/java-traceback.txt
--rw-r--r--   0 lemon      (501) staff       (20)      163 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/simple.sh
--rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/simple.txt
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.734660 linesieve-1.0b1/examples/src/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.734976 linesieve-1.0b1/examples/src/com/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.735240 linesieve-1.0b1/examples/src/com/example/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.735599 linesieve-1.0b1/examples/src/com/example/someproject/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.758578 linesieve-1.0b1/examples/src/com/example/someproject/somepackage/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/src/com/example/someproject/somepackage/ThingDoer.java
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736292 linesieve-1.0b1/examples/tst/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736468 linesieve-1.0b1/examples/tst/com/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736636 linesieve-1.0b1/examples/tst/com/example/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736829 linesieve-1.0b1/examples/tst/com/example/someproject/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.759350 linesieve-1.0b1/examples/tst/com/example/someproject/somepackage/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/tst/com/example/someproject/somepackage/ThingDoerTest.java
--rw-r--r--   0 lemon      (501) staff       (20)       90 2023-04-10 15:23:48.000000 linesieve-1.0b1/pyproject.toml
--rwxr-xr-x   0 lemon      (501) staff       (20)      544 2023-04-10 15:23:48.000000 linesieve-1.0b1/run.sh
--rw-r--r--   0 lemon      (501) staff       (20)     1713 2023-04-10 15:49:57.896685 linesieve-1.0b1/setup.cfg
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.737577 linesieve-1.0b1/src/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.763480 linesieve-1.0b1/src/linesieve/
--rw-r--r--   0 lemon      (501) staff       (20)      735 2023-04-10 15:48:55.000000 linesieve-1.0b1/src/linesieve/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)       28 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/__main__.py
--rw-r--r--   0 lemon      (501) staff       (20)    28501 2023-04-10 15:43:13.000000 linesieve-1.0b1/src/linesieve/cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     7116 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/parsing.py
--rw-r--r--   0 lemon      (501) staff       (20)     2820 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/paths.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.775789 linesieve-1.0b1/src/linesieve.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)    14355 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     2791 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/entry_points.txt
--rw-r--r--   0 lemon      (501) staff       (20)      128 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/top_level.txt
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.778272 linesieve-1.0b1/tests/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.893871 linesieve-1.0b1/tests/data/
--rw-r--r--   0 lemon      (501) staff       (20)       20 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/exec.in
--rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/exec.out
--rw-r--r--   0 lemon      (501) staff       (20)      180 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/full.in
--rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/full.out
--rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/head.in
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/head.out
--rw-r--r--   0 lemon      (501) staff       (20)       58 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/iter-line-filter.in
--rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/iter-line-filter.out
--rw-r--r--   0 lemon      (501) staff       (20)       23 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only-not-found.in
--rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only-not-found.out
--rw-r--r--   0 lemon      (501) staff       (20)       74 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       85 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure.out
--rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-none.in
--rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-none.out
--rw-r--r--   0 lemon      (501) staff       (20)       21 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only-not-found.in
--rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only-not-found.out
--rw-r--r--   0 lemon      (501) staff       (20)       20 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only.in
--rw-r--r--   0 lemon      (501) staff       (20)        3 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success.in
--rw-r--r--   0 lemon      (501) staff       (20)        7 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success.out
--rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end-no-section.in
--rw-r--r--   0 lemon      (501) staff       (20)       52 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end-no-section.out
--rw-r--r--   0 lemon      (501) staff       (20)       80 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end.in
--rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end.out
--rw-r--r--   0 lemon      (501) staff       (20)       31 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-invert.in
--rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-invert.out
--rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-only.in
--rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match.in
--rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match.out
--rw-r--r--   0 lemon      (501) staff       (20)      102 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/per-section.in
--rw-r--r--   0 lemon      (501) staff       (20)       29 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/per-section.out
--rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all-empty.in
--rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all-empty.out
--rw-r--r--   0 lemon      (501) staff       (20)      143 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all.in
--rw-r--r--   0 lemon      (501) staff       (20)       53 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all.out
--rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-empty.in
--rw-r--r--   0 lemon      (501) staff       (20)       91 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-empty.out
--rw-r--r--   0 lemon      (501) staff       (20)      117 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop.in
--rw-r--r--   0 lemon      (501) staff       (20)       36 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop.out
--rw-r--r--   0 lemon      (501) staff       (20)      103 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/push.in
--rw-r--r--   0 lemon      (501) staff       (20)       30 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/push.out
--rw-r--r--   0 lemon      (501) staff       (20)       49 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-data.in
--rw-r--r--   0 lemon      (501) staff       (20)       22 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-data.out
--rw-r--r--   0 lemon      (501) staff       (20)       41 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-empty.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-empty.out
--rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-first-section-only.in
--rw-r--r--   0 lemon      (501) staff       (20)        5 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-first-section-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       65 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-nothing.in
--rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-nothing.out
--rw-r--r--   0 lemon      (501) staff       (20)       51 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/single.in
--rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/single.out
--rw-r--r--   0 lemon      (501) staff       (20)     1125 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/span.in
--rw-r--r--   0 lemon      (501) staff       (20)      352 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/span.out
--rw-r--r--   0 lemon      (501) staff       (20)      147 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split-max.in
--rw-r--r--   0 lemon      (501) staff       (20)       39 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split-max.out
--rw-r--r--   0 lemon      (501) staff       (20)      209 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split.in
--rw-r--r--   0 lemon      (501) staff       (20)       68 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split.out
--rw-r--r--   0 lemon      (501) staff       (20)       37 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/sub-to-empty-line.in
--rw-r--r--   0 lemon      (501) staff       (20)        9 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/sub-to-empty-line.out
--rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/tail.in
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/tail.out
--rw-r--r--   0 lemon      (501) staff       (20)     5982 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/test_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     1495 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/test_paths.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.540746 linesieve-1.0b2/
+-rw-r--r--   0 lemon      (501) staff       (20)     1475 2023-04-12 15:05:06.000000 linesieve-1.0b2/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)      172 2023-04-12 15:05:06.000000 linesieve-1.0b2/MANIFEST.in
+-rw-r--r--   0 lemon      (501) staff       (20)    15009 2023-04-17 16:49:21.541131 linesieve-1.0b2/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)    13704 2023-04-17 16:47:46.000000 linesieve-1.0b2/README.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.204566 linesieve-1.0b2/docs/
+-rw-r--r--   0 lemon      (501) staff       (20)      634 2023-04-12 15:05:06.000000 linesieve-1.0b2/docs/Makefile
+-rw-r--r--   0 lemon      (501) staff       (20)      115 2023-04-12 15:05:06.000000 linesieve-1.0b2/docs/cli.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     1552 2023-04-12 15:05:06.000000 linesieve-1.0b2/docs/conf.py
+-rw-r--r--   0 lemon      (501) staff       (20)      271 2023-04-17 16:43:08.000000 linesieve-1.0b2/docs/examples.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      355 2023-04-17 09:09:17.000000 linesieve-1.0b2/docs/index.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      800 2023-04-12 15:05:06.000000 linesieve-1.0b2/docs/make.bat
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.220435 linesieve-1.0b2/examples/
+-rw-r--r--   0 lemon      (501) staff       (20)      580 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/ant-test-single-compile-error.diff
+-rw-r--r--   0 lemon      (501) staff       (20)      855 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/ant-test-single-compile-error.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      633 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/ant-test-single-failure.diff
+-rw-r--r--   0 lemon      (501) staff       (20)     8340 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/ant-test-single-failure.txt
+-rw-r--r--   0 lemon      (501) staff       (20)     4878 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/ant-test-single-success.txt
+-rwxr-xr-x   0 lemon      (501) staff       (20)     1144 2023-04-17 16:36:10.000000 linesieve-1.0b2/examples/ant-wrapper.sh
+-rw-r--r--   0 lemon      (501) staff       (20)      376 2023-04-14 07:31:27.000000 linesieve-1.0b2/examples/git-options.sh
+-rw-r--r--   0 lemon      (501) staff       (20)      607 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/java-traceback.sh
+-rw-r--r--   0 lemon      (501) staff       (20)    10527 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/java-traceback.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      163 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/simple.sh
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/simple.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.166227 linesieve-1.0b2/examples/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.166731 linesieve-1.0b2/examples/src/com/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.167062 linesieve-1.0b2/examples/src/com/example/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.167359 linesieve-1.0b2/examples/src/com/example/someproject/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.221440 linesieve-1.0b2/examples/src/com/example/someproject/somepackage/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/src/com/example/someproject/somepackage/ThingDoer.java
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.168246 linesieve-1.0b2/examples/tst/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.168615 linesieve-1.0b2/examples/tst/com/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.168930 linesieve-1.0b2/examples/tst/com/example/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.169446 linesieve-1.0b2/examples/tst/com/example/someproject/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.222097 linesieve-1.0b2/examples/tst/com/example/someproject/somepackage/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-12 15:05:06.000000 linesieve-1.0b2/examples/tst/com/example/someproject/somepackage/ThingDoerTest.java
+-rw-r--r--   0 lemon      (501) staff       (20)       90 2023-04-12 15:05:06.000000 linesieve-1.0b2/pyproject.toml
+-rwxr-xr-x   0 lemon      (501) staff       (20)      544 2023-04-12 15:05:06.000000 linesieve-1.0b2/run.sh
+-rw-r--r--   0 lemon      (501) staff       (20)     1713 2023-04-17 16:49:21.543485 linesieve-1.0b2/setup.cfg
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.170982 linesieve-1.0b2/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.232252 linesieve-1.0b2/src/linesieve/
+-rw-r--r--   0 lemon      (501) staff       (20)     1679 2023-04-17 16:48:44.000000 linesieve-1.0b2/src/linesieve/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)       28 2023-04-12 15:05:06.000000 linesieve-1.0b2/src/linesieve/__main__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    26779 2023-04-17 16:28:28.000000 linesieve-1.0b2/src/linesieve/cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4468 2023-04-15 17:17:03.000000 linesieve-1.0b2/src/linesieve/click_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7116 2023-04-12 15:05:06.000000 linesieve-1.0b2/src/linesieve/parsing.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2820 2023-04-12 15:05:06.000000 linesieve-1.0b2/src/linesieve/paths.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.237990 linesieve-1.0b2/src/linesieve.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)    15009 2023-04-17 16:49:20.000000 linesieve-1.0b2/src/linesieve.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     2828 2023-04-17 16:49:21.000000 linesieve-1.0b2/src/linesieve.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2023-04-17 16:49:20.000000 linesieve-1.0b2/src/linesieve.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-17 16:49:21.000000 linesieve-1.0b2/src/linesieve.egg-info/entry_points.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      128 2023-04-17 16:49:21.000000 linesieve-1.0b2/src/linesieve.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-17 16:49:21.000000 linesieve-1.0b2/src/linesieve.egg-info/top_level.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.242219 linesieve-1.0b2/tests/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-17 16:49:21.539698 linesieve-1.0b2/tests/data/
+-rw-r--r--   0 lemon      (501) staff       (20)      180 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/full.in
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/full.out
+-rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/head.in
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/head.out
+-rw-r--r--   0 lemon      (501) staff       (20)       58 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/iter-line-filter.in
+-rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/iter-line-filter.out
+-rw-r--r--   0 lemon      (501) staff       (20)       23 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure-only-not-found.in
+-rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure-only-not-found.out
+-rw-r--r--   0 lemon      (501) staff       (20)       74 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       85 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-failure.out
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-none.in
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-none.out
+-rw-r--r--   0 lemon      (501) staff       (20)       21 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success-only-not-found.in
+-rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success-only-not-found.out
+-rw-r--r--   0 lemon      (501) staff       (20)       20 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)        3 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success.in
+-rw-r--r--   0 lemon      (501) staff       (20)        7 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-success.out
+-rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-unexpected-end-no-section.in
+-rw-r--r--   0 lemon      (501) staff       (20)       52 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-unexpected-end-no-section.out
+-rw-r--r--   0 lemon      (501) staff       (20)       80 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-unexpected-end.in
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/marker-unexpected-end.out
+-rw-r--r--   0 lemon      (501) staff       (20)       31 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match-invert.in
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match-invert.out
+-rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match.in
+-rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/match.out
+-rw-r--r--   0 lemon      (501) staff       (20)      102 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/per-section.in
+-rw-r--r--   0 lemon      (501) staff       (20)       29 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/per-section.out
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-all-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-all-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)      143 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-all.in
+-rw-r--r--   0 lemon      (501) staff       (20)       53 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-all.out
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)       91 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)      117 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop.in
+-rw-r--r--   0 lemon      (501) staff       (20)       36 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/pop.out
+-rw-r--r--   0 lemon      (501) staff       (20)      103 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/push.in
+-rw-r--r--   0 lemon      (501) staff       (20)       30 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/push.out
+-rw-r--r--   0 lemon      (501) staff       (20)       24 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/read-cmd.in
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/read-cmd.out
+-rw-r--r--   0 lemon      (501) staff       (20)       49 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-all-data.in
+-rw-r--r--   0 lemon      (501) staff       (20)       22 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-all-data.out
+-rw-r--r--   0 lemon      (501) staff       (20)       41 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-all-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-all-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-first-section-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)        5 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-first-section-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       65 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-nothing.in
+-rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/show-nothing.out
+-rw-r--r--   0 lemon      (501) staff       (20)       51 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/single.in
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/single.out
+-rw-r--r--   0 lemon      (501) staff       (20)     1125 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/span.in
+-rw-r--r--   0 lemon      (501) staff       (20)      352 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/span.out
+-rw-r--r--   0 lemon      (501) staff       (20)      147 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/split-max.in
+-rw-r--r--   0 lemon      (501) staff       (20)       39 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/split-max.out
+-rw-r--r--   0 lemon      (501) staff       (20)      209 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/split.in
+-rw-r--r--   0 lemon      (501) staff       (20)       68 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/split.out
+-rw-r--r--   0 lemon      (501) staff       (20)       37 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/sub-to-empty-line.in
+-rw-r--r--   0 lemon      (501) staff       (20)        9 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/sub-to-empty-line.out
+-rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/tail.in
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/data/tail.out
+-rw-r--r--   0 lemon      (501) staff       (20)     5982 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/test_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1495 2023-04-12 15:05:06.000000 linesieve-1.0b2/tests/test_paths.py
```

### Comparing `linesieve-1.0b1/LICENSE` & `linesieve-1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/PKG-INFO` & `linesieve-1.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linesieve
-Version: 1.0b1
+Version: 1.0b2
 Summary: An unholy blend of grep, sed, awk, and Python.
 Home-page: https://github.com/lemon24/linesieve
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Documentation, https://linesieve.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/lemon24/linesieve/issues
 Project-URL: Source Code, https://github.com/lemon24/linesieve
@@ -27,14 +27,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
+
+.. default-role:: literal
+
+
 .. begin-intro
 
 *This is my text munging tool. There are many like it, but this one is mine.*
 
 **linesieve** is an unholy blend of grep, sed, awk, and Python,
 born out of spite.
 
@@ -68,134 +72,88 @@
   :alt: code style: black
 
 
 
 .. begin-main
 
 
-
 Features
 --------
 
-* line-oriented
-* section-oriented
+`linesieve` allows you to:
 
-  * show only matching sections
-  * show the failing section
-  * apply filters only to specific sections
-
-* match/sub with the full power of `re`_
+* split text input into sections
+* apply filters to specific sections
+* search and highlight success/failure markers
+* match/sub/split with the full power of Python's `re`_
+* shorten paths, links and module names
 * chain filters into pipelines
-* colors!
-* TODO: specific filters
+* color output!
 
 .. _re: https://docs.python.org/3/library/re.html
 
 
-
-Quickstart
+Installing
 ----------
 
+Install and update using `pip`_:
+
 .. code-block:: console
 
-    $ pip install linesieve
+    $ pip install --upgrade linesieve
 
+.. _pip: https://pip.pypa.io/en/stable/getting-started/
 
-.. code-block:: console
 
-    $ cat simple.txt
-    0
-    one:
-    1...
-    two:
-    2 (two)
-    three:
-    3, three
-    fail
+A simple example
+----------------
 
 .. code-block:: console
 
-    $ cat simple.txt \
-    | linesieve --section '(\S+):$' --failure fail \
-      show --ignore-case ^O \
-      match --section one --only-matching '\d+' \
-      sub '([a-z])' '\1\1\1'
-    one
-    1
-    ..
-    three
-    3, ttthhhrrreeeeee
-    fail
+    $ ls -1 /* | linesieve -s '.*:' show bin match ^d head -n2
+    .....
+    /bin:
+    dash
+    date
+    ......
+    /sbin:
+    disklabel
+    dmesg
+    ...
 
+This example uses `linesieve`
+to print the first two files starting with `d`
+from each directory whose name contains `bin`
+(skipped sections are marked with a dot on stderr).
 
 
 Links
 -----
 
 * PyPI Releases: https://pypi.org/project/linesieve/
 * Documentation: https://linesieve.readthedocs.io/
 * Issue Tracker: https://github.com/lemon24/linesieve/issues
 * Source Code: https://github.com/lemon24/linesieve
 
 
-
 .. end-main
 
 
 
 Examples
 --------
 
 .. begin-examples
 
-Get all options used by any git command
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Note that some of the man pages contain multiple OPTIONS sections (e.g. ADVANCED OPTIONS).
-
-.. code-block:: bash
-
-    export MANWIDTH=9999
-
-    function man-section {
-        col -b | linesieve -s '^[A-Z ()-]+$' show "$@"
-    }
-
-    man git \
-    | man-section COMMANDS match -o '^ +(git-\w+)' \
-    | cat - <( echo git ) \
-    | sort | uniq \
-    | xargs -n1 man \
-    | man-section OPTIONS match -o '^ +(-.*)' \
-        sub -F -- '--[no-]' '--' \
-        sub -F -- '--no-' '--' \
-    | sort -dfu
-
-
-.. code-block:: text
-
-    -/ <path>
-    -, --stdin
-    -0
-    ...
-    -a, --all
-    -A, --all, --ignore-removal
-    -a, --annotate
-    ...
-    --autosquash, --autosquash
-    --autostash, --autostash
-    -b
-    -b, --branch
-    ...
-
 
 Make Java tracebacks more readable
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Assume you're writing some Java tests with JUnit, on a project that looks like this:
+Assume you're writing some Java tests with JUnit,
+on a project that looks like this:
 
 .. code-block:: text
 
     .
     ├── src
     │   └── com
     │       └── example
@@ -227,15 +185,15 @@
         (?P<cls> \w+ )
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>'
 
-... shortens this traceback:
+... shortens this 76 line traceback:
 
 .. code-block:: text
 
     12:34:56.789 [main] ERROR com.example.someproject.somepackage.ThingDoer - exception while notifying done listener
     java.lang.RuntimeException: listener failed
     	at com.example.someproject.somepackage.ThingDoerTest$DummyListener.onThingDone(ThingDoerTest.java:420) ~[tests/:?]
     	at com.example.someproject.somepackage.ThingDoer.doThing(ThingDoer.java:69) ~[library/:?]
@@ -257,47 +215,48 @@
     	at ..ThingDoerTest$DummyListener.onThingDone(:420) ~[tests/:?]
     	at ..ThingDoer.doThing(:69) ~[library/:?]
     	at com.example.otherproject.Framework.doAllTheThings(:1066)
     	at ..ThingDoerTest.listenerException(:666) ~[tests/:?]
     	...
     12:34:56.999 [main] INFO done
 
-Let's break that linesieve command down a bit:
+Let's break that `linesieve` command down a bit:
 
 * The `span` gets rid of all the traceback lines coming from JUnit.
+* The `match -v` skips some usually useless lines from stack traces.
 * The `sub-paths` shortens and highlights the names of classes in the current project;
   `com.example.someproject.somepackage.ThingDoer` becomes `..ThingDoer`
   (presumably that's enough info to open the file).
 * The first `sub` gets rid of line numbers and JAR names for everything
   that is not either in the current project or in another `com.example.` package.
 * The second `sub` gets rid of JAR names for things in other `com.example.` packages.
 * The third `sub` gets rid of the source file name;
   `..ThingDoer.doThing(ThingDoer.java:69)` becomes `..ThingDoer.doThing(:69)`
   (the file name matches the class name).
 
 
 Apache Ant output
 ~~~~~~~~~~~~~~~~~
 
-Finally, let's look at why linesieve was born in the first place
+Let's look at why `linesieve` was born in the first place
 – cleaning up Apache Ant output.
 
 We'll use Ant's own test output as an example,
 since it `builds itself`_.
 
 .. _builds itself: https://github.com/apache/ant/tree/ff62ff7151bbc84a7706f40988258fabbcc324f5
 
 
 Running a single test with:
 
 .. code-block:: bash
 
     ant junit-single-test -Djunit.testcase=org.apache.tools.ant.ProjectTest
 
-... produces 77 lines of output, which looks like this:
+... produces 77 lines of output:
 
 .. code-block:: text
 
     Buildfile: /Users/lemon/code/ant/build.xml
 
     check-optional-packages:
 
@@ -322,31 +281,38 @@
             ... more lines
 
     junit-single-test:
 
     BUILD SUCCESSFUL
     Total time: 12 seconds
 
-(If you don't think it's all that bad,
-try to imagine how it would look for a serious Enterprise Project™.)
+If this doesn't look all that bad,
+try imagining what it looks like
+for a Serious Enterprise Project™.
 
-This is indeed very helpful
+
+Lots of output is indeed very helpful
 – if you're waiting tens of minutes for the entire test suite to run,
-you want all the details in the output,
+and/or it runs on some remote server,
+you want all the details in there,
 so you can debug failures without having to run it another time.
 
-However, it's not very helpful when you're developing,
-and only care about the thing you're working on right now.
+However, it's not very helpful during development,
+whey you only care about the thing you're working on *right now*.
+And it's doubly not helpful if you want to re-run the test suite
+on each file update with something like `entr`_.
+
+.. _entr: http://eradman.com/entrproject/
 
-This is where a script consisting of a single linesieve command comes in:
+
+This is where a `linesieve` wrapper script can help:
 
 .. code-block:: bash
 
     #!/bin/sh
-
     linesieve \
         --section '^(\S+):$' \
         --success 'BUILD SUCCESSFUL' \
         --failure 'BUILD FAILED' \
     show junit-batch \
     show junit-single-test-only \
     sub-cwd \
@@ -375,20 +341,20 @@
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>' \
     sub --color -X '^( \w+ (\.\w+)+ (?= :\s ))' '\1' \
     sub --color -X '(FAILED)' '\1' \
-    exec ant "$@"
+    read-cmd ant "$@"
 
-You can then call it instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
+You can then call this instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
 
 
-TODO: describe this output
+Successful output looks like this (28 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 0, Errors: 0, Skipped: 1, Time elapsed: 5.635 sec
@@ -413,14 +379,15 @@
     Testcase: testNullThrowableMessageLog took 0.002 sec
     Testcase: testTaskDefinitionContainsValue took 0.002 sec
     Testcase: testResolveFile took 0.001 sec
 
     .
     BUILD SUCCESSFUL
 
+... "failure" output looks like this (34 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 1, Errors: 0, Skipped: 1, Time elapsed: 5.638 sec
@@ -451,14 +418,15 @@
     Testcase: testTaskDefinitionContainsValue took 0.001 sec
     Testcase: testResolveFile took 0.001 sec
     Test ..ProjectTest FAILED
 
     .
     BUILD SUCCESSFUL
 
+... and true failure due to a compile error looks like this (12 lines):
 
 .. code-block:: text
 
     ...
     compile
     .../Project.java:65: error: cannot find symbol
     public class Project implements xResourceFactory {
@@ -468,10 +436,29 @@
         @Override
         ^
     2 errors
 
     BUILD FAILED
 
 
-TODO: linesieve command breakdown
+Breaking down the `linesieve` command
+(skipping the parts discussed in the previous example):
+
+* `--section '^(\S+):$'` tells `linesieve`
+  sections start with a word followed by a colon.
+* The `show`\s hide all sections except specific ones.
+* `--success` and `--failure` tell `linesieve`
+  to exit when encountering one of these patterns.
+  Note that the failing section above is shown
+  despite not being selected with `show`.
+* `sub-cwd` makes absolute paths in the working directory relative.
+* The `-s compile` option passed to `sub` applies that filter
+  only to sections matching `compile`.
+* `push compile` applies all the following filters, until `pop`,
+  only to sections matching `compile`.
+* The last two `sub --color ... '\1'` color
+  dotted words followed by a colon at the beginning of the line
+  (e.g. `junit.framework.AssertionFailedError:`),
+  and `FAILED` anywhere in the input.
+* Finally, `read-cmd` executes a command and uses its output as input.
 
 .. end-examples
```

### Comparing `linesieve-1.0b1/README.rst` & `linesieve-1.0b2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+
+.. default-role:: literal
+
+
 .. begin-intro
 
 *This is my text munging tool. There are many like it, but this one is mine.*
 
 **linesieve** is an unholy blend of grep, sed, awk, and Python,
 born out of spite.
 
@@ -35,134 +39,88 @@
   :alt: code style: black
 
 
 
 .. begin-main
 
 
-
 Features
 --------
 
-* line-oriented
-* section-oriented
+`linesieve` allows you to:
 
-  * show only matching sections
-  * show the failing section
-  * apply filters only to specific sections
-
-* match/sub with the full power of `re`_
+* split text input into sections
+* apply filters to specific sections
+* search and highlight success/failure markers
+* match/sub/split with the full power of Python's `re`_
+* shorten paths, links and module names
 * chain filters into pipelines
-* colors!
-* TODO: specific filters
+* color output!
 
 .. _re: https://docs.python.org/3/library/re.html
 
 
-
-Quickstart
+Installing
 ----------
 
+Install and update using `pip`_:
+
 .. code-block:: console
 
-    $ pip install linesieve
+    $ pip install --upgrade linesieve
 
+.. _pip: https://pip.pypa.io/en/stable/getting-started/
 
-.. code-block:: console
 
-    $ cat simple.txt
-    0
-    one:
-    1...
-    two:
-    2 (two)
-    three:
-    3, three
-    fail
+A simple example
+----------------
 
 .. code-block:: console
 
-    $ cat simple.txt \
-    | linesieve --section '(\S+):$' --failure fail \
-      show --ignore-case ^O \
-      match --section one --only-matching '\d+' \
-      sub '([a-z])' '\1\1\1'
-    one
-    1
-    ..
-    three
-    3, ttthhhrrreeeeee
-    fail
+    $ ls -1 /* | linesieve -s '.*:' show bin match ^d head -n2
+    .....
+    /bin:
+    dash
+    date
+    ......
+    /sbin:
+    disklabel
+    dmesg
+    ...
 
+This example uses `linesieve`
+to print the first two files starting with `d`
+from each directory whose name contains `bin`
+(skipped sections are marked with a dot on stderr).
 
 
 Links
 -----
 
 * PyPI Releases: https://pypi.org/project/linesieve/
 * Documentation: https://linesieve.readthedocs.io/
 * Issue Tracker: https://github.com/lemon24/linesieve/issues
 * Source Code: https://github.com/lemon24/linesieve
 
 
-
 .. end-main
 
 
 
 Examples
 --------
 
 .. begin-examples
 
-Get all options used by any git command
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Note that some of the man pages contain multiple OPTIONS sections (e.g. ADVANCED OPTIONS).
-
-.. code-block:: bash
-
-    export MANWIDTH=9999
-
-    function man-section {
-        col -b | linesieve -s '^[A-Z ()-]+$' show "$@"
-    }
-
-    man git \
-    | man-section COMMANDS match -o '^ +(git-\w+)' \
-    | cat - <( echo git ) \
-    | sort | uniq \
-    | xargs -n1 man \
-    | man-section OPTIONS match -o '^ +(-.*)' \
-        sub -F -- '--[no-]' '--' \
-        sub -F -- '--no-' '--' \
-    | sort -dfu
-
-
-.. code-block:: text
-
-    -/ <path>
-    -, --stdin
-    -0
-    ...
-    -a, --all
-    -A, --all, --ignore-removal
-    -a, --annotate
-    ...
-    --autosquash, --autosquash
-    --autostash, --autostash
-    -b
-    -b, --branch
-    ...
-
 
 Make Java tracebacks more readable
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Assume you're writing some Java tests with JUnit, on a project that looks like this:
+Assume you're writing some Java tests with JUnit,
+on a project that looks like this:
 
 .. code-block:: text
 
     .
     ├── src
     │   └── com
     │       └── example
@@ -194,15 +152,15 @@
         (?P<cls> \w+ )
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>'
 
-... shortens this traceback:
+... shortens this 76 line traceback:
 
 .. code-block:: text
 
     12:34:56.789 [main] ERROR com.example.someproject.somepackage.ThingDoer - exception while notifying done listener
     java.lang.RuntimeException: listener failed
     	at com.example.someproject.somepackage.ThingDoerTest$DummyListener.onThingDone(ThingDoerTest.java:420) ~[tests/:?]
     	at com.example.someproject.somepackage.ThingDoer.doThing(ThingDoer.java:69) ~[library/:?]
@@ -224,47 +182,48 @@
     	at ..ThingDoerTest$DummyListener.onThingDone(:420) ~[tests/:?]
     	at ..ThingDoer.doThing(:69) ~[library/:?]
     	at com.example.otherproject.Framework.doAllTheThings(:1066)
     	at ..ThingDoerTest.listenerException(:666) ~[tests/:?]
     	...
     12:34:56.999 [main] INFO done
 
-Let's break that linesieve command down a bit:
+Let's break that `linesieve` command down a bit:
 
 * The `span` gets rid of all the traceback lines coming from JUnit.
+* The `match -v` skips some usually useless lines from stack traces.
 * The `sub-paths` shortens and highlights the names of classes in the current project;
   `com.example.someproject.somepackage.ThingDoer` becomes `..ThingDoer`
   (presumably that's enough info to open the file).
 * The first `sub` gets rid of line numbers and JAR names for everything
   that is not either in the current project or in another `com.example.` package.
 * The second `sub` gets rid of JAR names for things in other `com.example.` packages.
 * The third `sub` gets rid of the source file name;
   `..ThingDoer.doThing(ThingDoer.java:69)` becomes `..ThingDoer.doThing(:69)`
   (the file name matches the class name).
 
 
 Apache Ant output
 ~~~~~~~~~~~~~~~~~
 
-Finally, let's look at why linesieve was born in the first place
+Let's look at why `linesieve` was born in the first place
 – cleaning up Apache Ant output.
 
 We'll use Ant's own test output as an example,
 since it `builds itself`_.
 
 .. _builds itself: https://github.com/apache/ant/tree/ff62ff7151bbc84a7706f40988258fabbcc324f5
 
 
 Running a single test with:
 
 .. code-block:: bash
 
     ant junit-single-test -Djunit.testcase=org.apache.tools.ant.ProjectTest
 
-... produces 77 lines of output, which looks like this:
+... produces 77 lines of output:
 
 .. code-block:: text
 
     Buildfile: /Users/lemon/code/ant/build.xml
 
     check-optional-packages:
 
@@ -289,31 +248,38 @@
             ... more lines
 
     junit-single-test:
 
     BUILD SUCCESSFUL
     Total time: 12 seconds
 
-(If you don't think it's all that bad,
-try to imagine how it would look for a serious Enterprise Project™.)
+If this doesn't look all that bad,
+try imagining what it looks like
+for a Serious Enterprise Project™.
 
-This is indeed very helpful
+
+Lots of output is indeed very helpful
 – if you're waiting tens of minutes for the entire test suite to run,
-you want all the details in the output,
+and/or it runs on some remote server,
+you want all the details in there,
 so you can debug failures without having to run it another time.
 
-However, it's not very helpful when you're developing,
-and only care about the thing you're working on right now.
+However, it's not very helpful during development,
+whey you only care about the thing you're working on *right now*.
+And it's doubly not helpful if you want to re-run the test suite
+on each file update with something like `entr`_.
+
+.. _entr: http://eradman.com/entrproject/
 
-This is where a script consisting of a single linesieve command comes in:
+
+This is where a `linesieve` wrapper script can help:
 
 .. code-block:: bash
 
     #!/bin/sh
-
     linesieve \
         --section '^(\S+):$' \
         --success 'BUILD SUCCESSFUL' \
         --failure 'BUILD FAILED' \
     show junit-batch \
     show junit-single-test-only \
     sub-cwd \
@@ -342,20 +308,20 @@
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>' \
     sub --color -X '^( \w+ (\.\w+)+ (?= :\s ))' '\1' \
     sub --color -X '(FAILED)' '\1' \
-    exec ant "$@"
+    read-cmd ant "$@"
 
-You can then call it instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
+You can then call this instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
 
 
-TODO: describe this output
+Successful output looks like this (28 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 0, Errors: 0, Skipped: 1, Time elapsed: 5.635 sec
@@ -380,14 +346,15 @@
     Testcase: testNullThrowableMessageLog took 0.002 sec
     Testcase: testTaskDefinitionContainsValue took 0.002 sec
     Testcase: testResolveFile took 0.001 sec
 
     .
     BUILD SUCCESSFUL
 
+... "failure" output looks like this (34 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 1, Errors: 0, Skipped: 1, Time elapsed: 5.638 sec
@@ -418,14 +385,15 @@
     Testcase: testTaskDefinitionContainsValue took 0.001 sec
     Testcase: testResolveFile took 0.001 sec
     Test ..ProjectTest FAILED
 
     .
     BUILD SUCCESSFUL
 
+... and true failure due to a compile error looks like this (12 lines):
 
 .. code-block:: text
 
     ...
     compile
     .../Project.java:65: error: cannot find symbol
     public class Project implements xResourceFactory {
@@ -435,10 +403,29 @@
         @Override
         ^
     2 errors
 
     BUILD FAILED
 
 
-TODO: linesieve command breakdown
+Breaking down the `linesieve` command
+(skipping the parts discussed in the previous example):
+
+* `--section '^(\S+):$'` tells `linesieve`
+  sections start with a word followed by a colon.
+* The `show`\s hide all sections except specific ones.
+* `--success` and `--failure` tell `linesieve`
+  to exit when encountering one of these patterns.
+  Note that the failing section above is shown
+  despite not being selected with `show`.
+* `sub-cwd` makes absolute paths in the working directory relative.
+* The `-s compile` option passed to `sub` applies that filter
+  only to sections matching `compile`.
+* `push compile` applies all the following filters, until `pop`,
+  only to sections matching `compile`.
+* The last two `sub --color ... '\1'` color
+  dotted words followed by a colon at the beginning of the line
+  (e.g. `junit.framework.AssertionFailedError:`),
+  and `FAILED` anywhere in the input.
+* Finally, `read-cmd` executes a command and uses its output as input.
 
 .. end-examples
```

### Comparing `linesieve-1.0b1/docs/Makefile` & `linesieve-1.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/docs/conf.py` & `linesieve-1.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/docs/make.bat` & `linesieve-1.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-test-single-compile-error.diff` & `linesieve-1.0b2/examples/ant-test-single-compile-error.diff`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-test-single-compile-error.txt` & `linesieve-1.0b2/examples/ant-test-single-compile-error.txt`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-test-single-failure.diff` & `linesieve-1.0b2/examples/ant-test-single-failure.diff`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-test-single-failure.txt` & `linesieve-1.0b2/examples/ant-test-single-failure.txt`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-test-single-success.txt` & `linesieve-1.0b2/examples/ant-test-single-success.txt`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/ant-wrapper.sh` & `linesieve-1.0b2/examples/ant-wrapper.sh`

 * *Files 11% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     (?P<mid> .* \( )
     (?P=cls) \.java
     (?P<suf> : .* )
     ' \
     '\g<pre>\g<cls>\g<mid>\g<suf>' \
 sub --color -X '^( \w+ (\.\w+)+ (?= :\s ))' '\1' \
 sub --color -X '(FAILED)' '\1' \
-exec ant "$@"
+read-cmd ant "$@"
```

### Comparing `linesieve-1.0b1/examples/java-traceback.sh` & `linesieve-1.0b2/examples/java-traceback.sh`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/examples/java-traceback.txt` & `linesieve-1.0b2/examples/java-traceback.txt`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/run.sh` & `linesieve-1.0b2/run.sh`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/setup.cfg` & `linesieve-1.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/src/linesieve/cli.py` & `linesieve-1.0b2/src/linesieve/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import click
 from click import BadParameter
 from click import echo
 from click import style
 from click import UsageError
 
 import linesieve
+from .click_utils import Group
 from .parsing import make_pipeline
 
 
 # references for common command-line option names:
 # https://www.gnu.org/prep/standards/html_node/Option-Table.html
 # http://www.catb.org/~esr/writings/taoup/html/ch10s05.html
 # all the git options, generated with the script in the README
@@ -24,31 +25,23 @@
 \b
 linesieve help --all
 linesieve COMMAND --help
 https://github.com/lemon24/linesieve
 """
 
 
-class CLIGroup(click.Group):
-    def format_options(self, ctx, formatter):
-        super().format_options(ctx, formatter)
-        with formatter.section('Further help'):
-            formatter.write_text(FURTHER_HELP)
-
-    def list_commands(self, ctx):
-        return self.commands
-
-
 @click.group(
     name='linesieve',
     chain=True,
-    cls=CLIGroup,
+    cls=Group,
     invoke_without_command=True,
-    no_args_is_help=True,
     subcommand_metavar='[COMMAND [ARGS]...]... ',
+    epilog_sections={'Further help': FURTHER_HELP},
+    help=linesieve.__doc__,
+    short_help="An unholy blend of grep, sed, awk, and Python.",
 )
 @click.option(
     '-s',
     '--section',
     metavar='PATTERN',
     help="""
     Consider matching lines the start of a new section.
@@ -68,15 +61,14 @@
     If matched, exit with a status code indicating failure.
     Before exiting, output the last section if it wasn't already.
     """,
 )
 @click.version_option(linesieve.__version__, message='%(prog)s %(version)s')
 @click.pass_context
 def cli(ctx, **kwargs):
-    """An unholy blend of grep, sed, awk, and Python."""
     # options reserved for future expansion:
     # -s --section --section-start
     # -e --section-end
     # -n --section-name # same as annotate_lines() marker
     ctx.obj = {}
 
 
@@ -94,14 +86,22 @@
             failure = re.compile(failure)
 
     file = ctx.obj.get('file')
     if not file:
         file = click.get_text_stream('stdin')
 
     if file.isatty():
+        # we are not using no_args_is_help=True, because as of click 8.1.3,
+        # "linesieve show p --not-an-option" shows help instead of
+        # "Error: No such command '--not-an-option'." (click bug?)
+        if not ctx.initial_args:
+            # TODO: show short help here instead
+            echo(ctx.get_help(), color=ctx.color)
+            ctx.exit()
+
         echo(style("linesieve: reading from terminal", dim=True), err=True)
 
     process = ctx.obj.get('process')
     show = ctx.obj.get('show')
 
     processors = [p for p in processors if p]
 
@@ -225,38 +225,47 @@
 
 # INPUT
 
 
 @cli.command(short_help="Read input from file.")
 @click.argument('file', type=click.File('r', lazy=True))
 @click.pass_obj
-def open(obj, file):
+def read(obj, file):
     """Read input from FILE instead of standard input.
 
-    Roughly equivalent to: cat FILE | linesieve
+    Roughly equivalent to: `linesieve < FILE`
+
+    \b
+        $ linesieve read file.txt
+        hello
 
     """
-    assert not obj.get('file'), "should not be possible for open to follow exec"
+    assert not obj.get('file'), "should not be possible for read to follow read-cmd"
     obj['file'] = file
 
 
 @cli.command(short_help="Read input from command.")
 @click.argument('command')
 @click.argument('argument', nargs=-1)
 @click.pass_obj
-def exec(obj, command, argument):
+def read_cmd(obj, command, argument):
     """Execute COMMAND and use its output as input.
 
-    Roughly equivalent to: COMMAND | linesieve
+    Roughly equivalent to: `COMMAND | linesieve`
 
     If the command finishes, exit with its status code.
 
+    \b
+        $ linesieve read-cmd echo bonjour
+        bonjour
+        linesieve: echo exited with status code 0  # green
+
     """
     if obj.get('file'):
-        raise UsageError("exec and open are mutually exclusive")
+        raise UsageError("read-cmd and read are mutually exclusive")
     try:
         process = subprocess.Popen(
             (command,) + argument,
             text=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
@@ -324,14 +333,22 @@
 @click.pass_obj
 def show(obj, pattern, fixed_strings):
     """Output only sections matching PATTERN.
 
     `^$` matches the lines before the first section.
     `$none` matches no section.
 
+    \b
+        $ ls -1 /* | linesieve -s '.*:' show /bin match ash
+        .....  # dim
+        /bin:  # dim bold
+        bash
+        dash
+        ..........  # dim
+
     """
     obj.setdefault('show', []).append(pattern)
 
 
 @cli.command(short_help="Push patterns onto the section stack.")
 @pattern_argument
 @click.pass_obj
@@ -341,14 +358,30 @@
     When there are patterns on the section stack,
     filters apply only to the sections that match
     any of the patterns in the stack.
 
     `filter --section PATTERN` is equivalent to
     `push PATTERN filter pop`.
 
+    \b
+        $ ls -1 /* | linesieve -s '.*:' \\
+        > show bin \\
+        > push /bin \\
+        >   head -n1 \\
+        > pop \\
+        > head -n2
+        .....  # dim
+        /bin:  # dim bold
+        [
+        ......  # dim
+        /sbin:  # dim bold
+        apfs_hfs_convert
+        disklabel
+        ...  # dim
+
     """
     stack = obj.setdefault('section_stack', [])
     stack.append(pattern)
 
 
 @cli.command(short_help="Pop patterns off the section stack.")
 @click.option(
@@ -412,15 +445,20 @@
     help="Print the first COUNT lines. "
     "With a leading `-`, print all but the last COUNT lines.",
 )
 @section_option
 def head(count):
     """Print the first COUNT lines.
 
-    Roughly equivalent to: head -n COUNT
+    Roughly equivalent to: `head -n COUNT`
+
+    \b
+        $ echo -e 'a\\nb\\nc' | linesieve head -n2
+        a
+        b
 
     """
     from itertools import islice
 
     def head(lines):
         if count >= 0:
             return islice(lines, count)
@@ -454,15 +492,20 @@
     help="Print the last COUNT lines. "
     "With a leading `+`, print lines starting with line COUNT.",
 )
 @section_option
 def tail(count):
     """Print the last COUNT lines.
 
-    Roughly equivalent to: tail -n COUNT
+    Roughly equivalent to: `tail -n COUNT`
+
+    \b
+        $ echo -e 'a\\nb\\nc' | linesieve tail -n2
+        b
+        c
 
     """
     from itertools import islice
     from collections import deque
 
     def tail(lines):
         if count <= 0:
@@ -496,15 +539,23 @@
     without `--invert-match`, only escapes are expanded.
     """,
 )
 @section_option
 def span(start, end, fixed_strings, ignore_case, verbose, invert_match, repl):
     """Output only lines between those matching `--start` and `--end`.
 
-    Roughly equivalent to: grep START -A9999 | grep END -B9999 | head -n-1
+    Roughly equivalent to: `grep START -A9999 | grep END -B9999 | head -n-1`
+
+    \b
+        $ seq 20 | linesieve span --start ^2$ --end ^5$ --repl ...
+        ...
+        2
+        3
+        4
+        ...
 
     """
 
     # options reserved for future expansion:
     # --start-after (mutually exclusive with --start-with)
     # --end-with (mutually exclusive with --end-before)
 
@@ -576,18 +627,28 @@
 )
 @click.option('--color', is_flag=True, help="Color matches.")
 @section_option
 @click.pass_context
 def match(ctx, pattern, fixed_strings, only_matching, invert_match, color):
     """Output only lines matching PATTERN.
 
-    Roughly equivalent to: grep PATTERN
+    Roughly equivalent to: `grep PATTERN`
 
     Works like re.search() in Python.
 
+    \b
+        $ seq 10 | linesieve match 1
+        1
+        10
+    \b
+        $ echo a1b2c3 | linesieve match -o '\\d+'
+        1
+        2
+        3
+
     """
 
     if color and not invert_match and not only_matching:
         return ctx.invoke(
             sub,
             pattern=pattern,
             repl=r'\g<0>',
@@ -707,14 +768,19 @@
         N-M   from Nth to Mth (included) field
          -M   from first to Mth (included) field
 
     This is the same as the cut command. Unlike cut,
     selected fields are printed in the order from the list,
     and more than once, if repeated.
 
+    \b
+        $ echo -e 'a-b\\nc-d' | linesieve split -d- -f2
+        b
+        d
+
     """
     if delimiter is None or (fixed_strings and not ignore_case):
         max_split = max_split or -1
 
         def split(line):
             return line.split(delimiter, max_split)
 
@@ -758,18 +824,22 @@
 @click.argument('repl')
 @click.option('-o', '--only-matching', is_flag=True, help="Output only matching lines.")
 @click.option('--color', is_flag=True, help="Color replacements.")
 @section_option
 def sub(pattern, repl, fixed_strings, only_matching, color):
     """Replace PATTERN matches with REPL.
 
-    Roughly equivalent to: sed 's/PATTERN/REPL/g'
+    Roughly equivalent to: `sed 's/PATTERN/REPL/g'`
 
     Works like re.sub() in Python.
 
+    \b
+        $ echo a1b2c3 | linesieve sub '\\d+' x
+        axbxcx
+
     """
     if fixed_strings:
         repl = repl.replace('\\', r'\\')
     if color:
         repl = style(repl, fg='red')
 
     def sub(line):
@@ -791,15 +861,15 @@
     metavar='GLOB',
     help="""
     Replace the paths of existing files matching this pattern.
     Both recursive globs and brace expansion are supported, e.g.
     `{src,tests}/**/*.py`.
     """,
 )
-@click.option('--modules', is_flag=True, help="Also replaced dotted module names.")
+@click.option('--modules', is_flag=True, help="Also replace dotted module names.")
 @click.option(
     '--modules-skip',
     type=click.IntRange(0),
     metavar='INTEGER',
     help="Path levels to skip to obtain module names from paths. Implies `--modules`.",
 )
 @click.option(
@@ -843,23 +913,23 @@
     \b
         ..mod1
         ..mod2
         ..two
 
     """
     from glob import glob
-    from braceexpand import braceexpand, UnbalancedBracesError
+    from braceexpand import braceexpand
     from .paths import shorten_paths, paths_to_modules, make_file_paths_re
 
     paths = []
     try:
         for unexpanded_pattern in include:
             for pattern in braceexpand(unexpanded_pattern):
                 paths.extend(glob(pattern, recursive=True))
-    except UnbalancedBracesError as e:
+    except ValueError as e:
         raise BadParameter(e, param_hint=['--include'])
 
     replacements = shorten_paths(paths, os.sep, '...')
 
     if modules or modules_recursive or modules_skip is not None:
         modules = paths_to_modules(
             paths, skip=modules_skip or 0, recursive=modules_recursive
@@ -882,17 +952,21 @@
 
     return sub_paths
 
 
 @cli.command(short_help="Make working directory paths relative.")
 @section_option
 def sub_cwd():
-    """Make paths in the working directory relative.
+    """Make absolute paths in the working directory relative.
 
-    Roughly equivalent to: sub $( pwd ) ''
+    Roughly equivalent to: `sub $( pwd ) ''`
+
+    \b
+        $ echo "hello from $( pwd )/src" | linesieve sub-cwd
+        hello from src
 
     """
     min_length = 2
 
     path = os.getcwd()
     if len(path.split(os.sep)) < min_length:
         return None
@@ -912,15 +986,15 @@
 
 @cli.command(short_help="Replace symlink targets.")
 @click.argument('link')
 @section_option
 def sub_link(link):
     """Replace the target of symlink LINK with LINK.
 
-    Roughly equivalent to: sub $( realpath LINK ) LINK
+    Roughly equivalent to: `sub $( realpath LINK ) LINK`
 
     """
     min_length = 2
 
     try:
         path = os.path.abspath(os.readlink(link))
     except FileNotFoundError:
@@ -950,127 +1024,17 @@
 
 @cli.command()
 @click.option('--all', is_flag=True, help="Show help for all commands, man-style.")
 @click.pass_context
 def help(ctx, all):
     """Show detailed help."""
 
+    from .click_utils import format_help_all
+
     ctx = ctx.find_root()
-    original_help = ctx.command.help
-    ctx.command.help = color_help(linesieve.__doc__)
 
-    try:
-        if not all:
-            click.echo(ctx.get_help(), color=ctx.color)
-        else:
-            click.echo_via_pager(format_help_all(ctx))
-    finally:
-        ctx.command.help = original_help
+    if not all:
+        click.echo(ctx.get_help(), color=ctx.color)
+    else:
+        click.echo_via_pager(format_help_all(ctx))
 
     ctx.exit()
-
-
-def color_help(text):
-    KWARGS = {
-        'dim': dict(dim=True),
-        'red': dict(fg='red'),
-        'green': dict(fg='green'),
-        'yellow': dict(fg='yellow'),
-    }
-
-    def repl(match):
-        line, options = match.groups()
-        kwargs = {}
-        for option in options.split():
-            kwargs.update(KWARGS[option])
-        return style(line, **kwargs)
-
-    options_re = '|'.join(map(re.escape, KWARGS))
-    line_re = f"(.*)#((?: +(?:{options_re}))+ *)$"
-
-    return re.sub(line_re, repl, text, flags=re.M)
-
-
-class ManFormatter(click.HelpFormatter):
-    def __init__(self):
-        super().__init__(4, max_width=999999)
-        # print(self.width)
-
-    def write_dl(self, rows, col_max=30, col_spacing=2):
-        """Write the options definition after the term, indented.
-
-        col_max and col_spacing are ignored.
-
-        """
-        # for reasons (click bug?), the original write_dl() will spill over
-        # if indenting more than once (worsened by indent_increment > 2);
-        # this does not happen with our implementation
-
-        for i, (first, second) in enumerate(rows, 1):
-            self.write_text(first)
-            with self.indentation():
-                self.write_text(second)
-            if i != len(rows):
-                self.write_paragraph()
-
-    def write_usage(self, prog, args='', prefix='Usage: '):
-        if prefix is not None:
-            prefix = style(prefix, bold=True)
-
-        self.write(f"{'':>{self.current_indent}}")
-        super().write_usage(prog, args, prefix)
-
-    def write_heading(self, heading):
-        heading = style(heading, bold=True)
-        self.write(f"{'':>{self.current_indent}}{heading}\n")
-
-    @contextmanager
-    def supersection(self, name, short=None):
-        title = style(name.upper(), bold=True)
-        if short:
-            title += style(' - ' + short, dim=True)
-
-        self.write(title)
-        self.write_paragraph()
-        self.write_paragraph()
-
-        with self.indentation():
-            yield
-
-        self.write_paragraph()
-
-
-def format_help_all(ctx):
-    formatter = ManFormatter()
-    commands = list_commands_recursive(ctx.command, ctx)
-
-    for path, command in commands:
-        short = command.get_short_help_str(limit=55)
-        if short:
-            first = short.partition(' ')[0]
-            if first.istitle():
-                short = first.lower() + short[len(first) :]
-            short = short.rstrip('.')
-
-        if command is ctx.command:
-            format_ctx = ctx
-        else:
-            format_ctx = type(ctx)(command, ctx, command.name)
-
-        with formatter.supersection(' '.join(path), short):
-            command.format_help(format_ctx, formatter)
-
-    return formatter.getvalue()
-
-
-def list_commands_recursive(self, ctx, path=()):
-    path = path + (self.name,)
-    yield path, self
-    if not hasattr(self, 'list_commands'):
-        return
-    for subcommand in self.list_commands(ctx):
-        cmd = self.get_command(ctx, subcommand)
-        if cmd is None:
-            continue
-        if cmd.hidden:
-            continue
-        yield from list_commands_recursive(cmd, ctx, path)
```

### Comparing `linesieve-1.0b1/src/linesieve/parsing.py` & `linesieve-1.0b2/src/linesieve/parsing.py`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/src/linesieve/paths.py` & `linesieve-1.0b2/src/linesieve/paths.py`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/src/linesieve.egg-info/PKG-INFO` & `linesieve-1.0b2/src/linesieve.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linesieve
-Version: 1.0b1
+Version: 1.0b2
 Summary: An unholy blend of grep, sed, awk, and Python.
 Home-page: https://github.com/lemon24/linesieve
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Documentation, https://linesieve.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/lemon24/linesieve/issues
 Project-URL: Source Code, https://github.com/lemon24/linesieve
@@ -27,14 +27,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
+
+.. default-role:: literal
+
+
 .. begin-intro
 
 *This is my text munging tool. There are many like it, but this one is mine.*
 
 **linesieve** is an unholy blend of grep, sed, awk, and Python,
 born out of spite.
 
@@ -68,134 +72,88 @@
   :alt: code style: black
 
 
 
 .. begin-main
 
 
-
 Features
 --------
 
-* line-oriented
-* section-oriented
+`linesieve` allows you to:
 
-  * show only matching sections
-  * show the failing section
-  * apply filters only to specific sections
-
-* match/sub with the full power of `re`_
+* split text input into sections
+* apply filters to specific sections
+* search and highlight success/failure markers
+* match/sub/split with the full power of Python's `re`_
+* shorten paths, links and module names
 * chain filters into pipelines
-* colors!
-* TODO: specific filters
+* color output!
 
 .. _re: https://docs.python.org/3/library/re.html
 
 
-
-Quickstart
+Installing
 ----------
 
+Install and update using `pip`_:
+
 .. code-block:: console
 
-    $ pip install linesieve
+    $ pip install --upgrade linesieve
 
+.. _pip: https://pip.pypa.io/en/stable/getting-started/
 
-.. code-block:: console
 
-    $ cat simple.txt
-    0
-    one:
-    1...
-    two:
-    2 (two)
-    three:
-    3, three
-    fail
+A simple example
+----------------
 
 .. code-block:: console
 
-    $ cat simple.txt \
-    | linesieve --section '(\S+):$' --failure fail \
-      show --ignore-case ^O \
-      match --section one --only-matching '\d+' \
-      sub '([a-z])' '\1\1\1'
-    one
-    1
-    ..
-    three
-    3, ttthhhrrreeeeee
-    fail
+    $ ls -1 /* | linesieve -s '.*:' show bin match ^d head -n2
+    .....
+    /bin:
+    dash
+    date
+    ......
+    /sbin:
+    disklabel
+    dmesg
+    ...
 
+This example uses `linesieve`
+to print the first two files starting with `d`
+from each directory whose name contains `bin`
+(skipped sections are marked with a dot on stderr).
 
 
 Links
 -----
 
 * PyPI Releases: https://pypi.org/project/linesieve/
 * Documentation: https://linesieve.readthedocs.io/
 * Issue Tracker: https://github.com/lemon24/linesieve/issues
 * Source Code: https://github.com/lemon24/linesieve
 
 
-
 .. end-main
 
 
 
 Examples
 --------
 
 .. begin-examples
 
-Get all options used by any git command
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Note that some of the man pages contain multiple OPTIONS sections (e.g. ADVANCED OPTIONS).
-
-.. code-block:: bash
-
-    export MANWIDTH=9999
-
-    function man-section {
-        col -b | linesieve -s '^[A-Z ()-]+$' show "$@"
-    }
-
-    man git \
-    | man-section COMMANDS match -o '^ +(git-\w+)' \
-    | cat - <( echo git ) \
-    | sort | uniq \
-    | xargs -n1 man \
-    | man-section OPTIONS match -o '^ +(-.*)' \
-        sub -F -- '--[no-]' '--' \
-        sub -F -- '--no-' '--' \
-    | sort -dfu
-
-
-.. code-block:: text
-
-    -/ <path>
-    -, --stdin
-    -0
-    ...
-    -a, --all
-    -A, --all, --ignore-removal
-    -a, --annotate
-    ...
-    --autosquash, --autosquash
-    --autostash, --autostash
-    -b
-    -b, --branch
-    ...
-
 
 Make Java tracebacks more readable
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Assume you're writing some Java tests with JUnit, on a project that looks like this:
+Assume you're writing some Java tests with JUnit,
+on a project that looks like this:
 
 .. code-block:: text
 
     .
     ├── src
     │   └── com
     │       └── example
@@ -227,15 +185,15 @@
         (?P<cls> \w+ )
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>'
 
-... shortens this traceback:
+... shortens this 76 line traceback:
 
 .. code-block:: text
 
     12:34:56.789 [main] ERROR com.example.someproject.somepackage.ThingDoer - exception while notifying done listener
     java.lang.RuntimeException: listener failed
     	at com.example.someproject.somepackage.ThingDoerTest$DummyListener.onThingDone(ThingDoerTest.java:420) ~[tests/:?]
     	at com.example.someproject.somepackage.ThingDoer.doThing(ThingDoer.java:69) ~[library/:?]
@@ -257,47 +215,48 @@
     	at ..ThingDoerTest$DummyListener.onThingDone(:420) ~[tests/:?]
     	at ..ThingDoer.doThing(:69) ~[library/:?]
     	at com.example.otherproject.Framework.doAllTheThings(:1066)
     	at ..ThingDoerTest.listenerException(:666) ~[tests/:?]
     	...
     12:34:56.999 [main] INFO done
 
-Let's break that linesieve command down a bit:
+Let's break that `linesieve` command down a bit:
 
 * The `span` gets rid of all the traceback lines coming from JUnit.
+* The `match -v` skips some usually useless lines from stack traces.
 * The `sub-paths` shortens and highlights the names of classes in the current project;
   `com.example.someproject.somepackage.ThingDoer` becomes `..ThingDoer`
   (presumably that's enough info to open the file).
 * The first `sub` gets rid of line numbers and JAR names for everything
   that is not either in the current project or in another `com.example.` package.
 * The second `sub` gets rid of JAR names for things in other `com.example.` packages.
 * The third `sub` gets rid of the source file name;
   `..ThingDoer.doThing(ThingDoer.java:69)` becomes `..ThingDoer.doThing(:69)`
   (the file name matches the class name).
 
 
 Apache Ant output
 ~~~~~~~~~~~~~~~~~
 
-Finally, let's look at why linesieve was born in the first place
+Let's look at why `linesieve` was born in the first place
 – cleaning up Apache Ant output.
 
 We'll use Ant's own test output as an example,
 since it `builds itself`_.
 
 .. _builds itself: https://github.com/apache/ant/tree/ff62ff7151bbc84a7706f40988258fabbcc324f5
 
 
 Running a single test with:
 
 .. code-block:: bash
 
     ant junit-single-test -Djunit.testcase=org.apache.tools.ant.ProjectTest
 
-... produces 77 lines of output, which looks like this:
+... produces 77 lines of output:
 
 .. code-block:: text
 
     Buildfile: /Users/lemon/code/ant/build.xml
 
     check-optional-packages:
 
@@ -322,31 +281,38 @@
             ... more lines
 
     junit-single-test:
 
     BUILD SUCCESSFUL
     Total time: 12 seconds
 
-(If you don't think it's all that bad,
-try to imagine how it would look for a serious Enterprise Project™.)
+If this doesn't look all that bad,
+try imagining what it looks like
+for a Serious Enterprise Project™.
 
-This is indeed very helpful
+
+Lots of output is indeed very helpful
 – if you're waiting tens of minutes for the entire test suite to run,
-you want all the details in the output,
+and/or it runs on some remote server,
+you want all the details in there,
 so you can debug failures without having to run it another time.
 
-However, it's not very helpful when you're developing,
-and only care about the thing you're working on right now.
+However, it's not very helpful during development,
+whey you only care about the thing you're working on *right now*.
+And it's doubly not helpful if you want to re-run the test suite
+on each file update with something like `entr`_.
+
+.. _entr: http://eradman.com/entrproject/
 
-This is where a script consisting of a single linesieve command comes in:
+
+This is where a `linesieve` wrapper script can help:
 
 .. code-block:: bash
 
     #!/bin/sh
-
     linesieve \
         --section '^(\S+):$' \
         --success 'BUILD SUCCESSFUL' \
         --failure 'BUILD FAILED' \
     show junit-batch \
     show junit-single-test-only \
     sub-cwd \
@@ -375,20 +341,20 @@
         (?P<mid> .* \( )
         (?P=cls) \.java
         (?P<suf> : .* )
         ' \
         '\g<pre>\g<cls>\g<mid>\g<suf>' \
     sub --color -X '^( \w+ (\.\w+)+ (?= :\s ))' '\1' \
     sub --color -X '(FAILED)' '\1' \
-    exec ant "$@"
+    read-cmd ant "$@"
 
-You can then call it instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
+You can then call this instead of `ant`: `ant-wrapper.sh junit-single-test ...`.
 
 
-TODO: describe this output
+Successful output looks like this (28 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 0, Errors: 0, Skipped: 1, Time elapsed: 5.635 sec
@@ -413,14 +379,15 @@
     Testcase: testNullThrowableMessageLog took 0.002 sec
     Testcase: testTaskDefinitionContainsValue took 0.002 sec
     Testcase: testResolveFile took 0.001 sec
 
     .
     BUILD SUCCESSFUL
 
+... "failure" output looks like this (34 lines):
 
 .. code-block:: text
 
     ............
     junit-single-test-only
     Testsuite: ..ProjectTest
     Tests run: 12, Failures: 1, Errors: 0, Skipped: 1, Time elapsed: 5.638 sec
@@ -451,14 +418,15 @@
     Testcase: testTaskDefinitionContainsValue took 0.001 sec
     Testcase: testResolveFile took 0.001 sec
     Test ..ProjectTest FAILED
 
     .
     BUILD SUCCESSFUL
 
+... and true failure due to a compile error looks like this (12 lines):
 
 .. code-block:: text
 
     ...
     compile
     .../Project.java:65: error: cannot find symbol
     public class Project implements xResourceFactory {
@@ -468,10 +436,29 @@
         @Override
         ^
     2 errors
 
     BUILD FAILED
 
 
-TODO: linesieve command breakdown
+Breaking down the `linesieve` command
+(skipping the parts discussed in the previous example):
+
+* `--section '^(\S+):$'` tells `linesieve`
+  sections start with a word followed by a colon.
+* The `show`\s hide all sections except specific ones.
+* `--success` and `--failure` tell `linesieve`
+  to exit when encountering one of these patterns.
+  Note that the failing section above is shown
+  despite not being selected with `show`.
+* `sub-cwd` makes absolute paths in the working directory relative.
+* The `-s compile` option passed to `sub` applies that filter
+  only to sections matching `compile`.
+* `push compile` applies all the following filters, until `pop`,
+  only to sections matching `compile`.
+* The last two `sub --color ... '\1'` color
+  dotted words followed by a colon at the beginning of the line
+  (e.g. `junit.framework.AssertionFailedError:`),
+  and `FAILED` anywhere in the input.
+* Finally, `read-cmd` executes a command and uses its output as input.
 
 .. end-examples
```

### Comparing `linesieve-1.0b1/src/linesieve.egg-info/SOURCES.txt` & `linesieve-1.0b2/src/linesieve.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,25 @@
 examples/simple.sh
 examples/simple.txt
 examples/src/com/example/someproject/somepackage/ThingDoer.java
 examples/tst/com/example/someproject/somepackage/ThingDoerTest.java
 src/linesieve/__init__.py
 src/linesieve/__main__.py
 src/linesieve/cli.py
+src/linesieve/click_utils.py
 src/linesieve/parsing.py
 src/linesieve/paths.py
 src/linesieve.egg-info/PKG-INFO
 src/linesieve.egg-info/SOURCES.txt
 src/linesieve.egg-info/dependency_links.txt
 src/linesieve.egg-info/entry_points.txt
 src/linesieve.egg-info/requires.txt
 src/linesieve.egg-info/top_level.txt
 tests/test_cli.py
 tests/test_paths.py
-tests/data/exec.in
-tests/data/exec.out
 tests/data/full.in
 tests/data/full.out
 tests/data/head.in
 tests/data/head.out
 tests/data/iter-line-filter.in
 tests/data/iter-line-filter.out
 tests/data/marker-failure-only-not-found.in
@@ -76,14 +75,16 @@
 tests/data/pop-all.out
 tests/data/pop-empty.in
 tests/data/pop-empty.out
 tests/data/pop.in
 tests/data/pop.out
 tests/data/push.in
 tests/data/push.out
+tests/data/read-cmd.in
+tests/data/read-cmd.out
 tests/data/show-all-data.in
 tests/data/show-all-data.out
 tests/data/show-all-empty.in
 tests/data/show-all-empty.out
 tests/data/show-first-section-only.in
 tests/data/show-first-section-only.out
 tests/data/show-nothing.in
```

### Comparing `linesieve-1.0b1/tests/data/span.in` & `linesieve-1.0b2/tests/data/span.in`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/tests/test_cli.py` & `linesieve-1.0b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `linesieve-1.0b1/tests/test_paths.py` & `linesieve-1.0b2/tests/test_paths.py`

 * *Files identical despite different names*

