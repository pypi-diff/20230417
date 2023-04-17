# Comparing `tmp/pyflyby-1.8.2.tar.gz` & `tmp/pyflyby-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyby-1.8.2.tar", last modified: Mon Feb 27 06:04:39 2023, max compression
+gzip compressed data, was "pyflyby-1.8.3.tar", last modified: Mon Apr 17 07:48:56 2023, max compression
```

## Comparing `pyflyby-1.8.2.tar` & `pyflyby-1.8.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.295077 pyflyby-1.8.2/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2965 2021-09-24 06:20:21.000000 pyflyby-1.8.2/.pyflyby
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1188 2021-09-24 06:20:21.000000 pyflyby-1.8.2/LICENSE.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      520 2022-05-19 08:06:52.000000 pyflyby-1.8.2/MANIFEST.in
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    14760 2023-02-27 06:04:39.294392 pyflyby-1.8.2/PKG-INFO
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    13790 2022-09-09 06:09:39.000000 pyflyby-1.8.2/README.rst
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.169603 pyflyby-1.8.2/bin/
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2441 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/autoipython
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      207 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/autopython
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2966 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/collect-exports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2206 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/collect-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      238 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/create-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1035 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/find-import
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1130 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/list-bad-xrefs
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      926 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/prune-broken-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1079 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/py
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.199732 pyflyby-1.8.2/bin/pyflyby/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2712 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/__init__.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      296 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/__main__.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    82494 2022-09-30 05:55:12.000000 pyflyby-1.8.2/bin/pyflyby/_autoimp.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    20614 2023-02-27 05:52:44.000000 pyflyby-1.8.2/bin/pyflyby/_cmdline.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     4536 2022-09-09 06:09:39.000000 pyflyby-1.8.2/bin/pyflyby/_comms.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    46185 2022-10-12 05:57:20.000000 pyflyby-1.8.2/bin/pyflyby/_dbg.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    14280 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_docxref.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    22927 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_file.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7455 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_flags.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     6733 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_format.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7829 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_idents.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    21860 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_importclns.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    23556 2022-05-19 08:06:52.000000 pyflyby-1.8.2/bin/pyflyby/_importdb.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    23605 2023-02-27 05:52:44.000000 pyflyby-1.8.2/bin/pyflyby/_imports2s.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    17624 2023-02-27 05:52:44.000000 pyflyby-1.8.2/bin/pyflyby/_importstmt.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)   104335 2023-02-27 05:52:44.000000 pyflyby-1.8.2/bin/pyflyby/_interactive.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    30111 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_livepatch.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7915 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_log.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    15434 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_modules.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    56300 2022-10-12 05:57:20.000000 pyflyby-1.8.2/bin/pyflyby/_parse.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    76032 2022-05-19 08:06:52.000000 pyflyby-1.8.2/bin/pyflyby/_py.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    15506 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/_util.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      266 2023-02-27 05:54:03.000000 pyflyby-1.8.2/bin/pyflyby/_version.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      591 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/autoimport.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      600 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/pyflyby/importdb.py
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      938 2022-05-19 08:06:52.000000 pyflyby-1.8.2/bin/pyflyby-diff
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      755 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/reformat-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      978 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/replace-star-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     7855 2022-09-09 06:09:39.000000 pyflyby-1.8.2/bin/tidy-imports
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1515 2021-09-24 06:20:21.000000 pyflyby-1.8.2/bin/transform-imports
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.207054 pyflyby-1.8.2/doc/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1188 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/LICENSE.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      855 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/Makefile
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     5686 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/TODO.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)        0 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/__init__.py
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.224852 pyflyby-1.8.2/doc/api/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      275 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/api.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       78 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/autoimp.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       78 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/cmdline.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       72 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/comms.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       66 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/dbg.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       69 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/file.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      123 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/flags.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       75 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/format.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      109 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/idents.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       86 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/importclns.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       80 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/importdb.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       83 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/imports2s.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       86 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/importstmt.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       89 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/interactive.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       83 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/livepatch.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       65 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/log.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       77 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/modules.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       71 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/parse.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       62 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/py.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       68 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/api/util.rst
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.237371 pyflyby-1.8.2/doc/cli/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      102 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/autoipython.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      273 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/cli.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       85 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/collect_exports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       85 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/collect_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       73 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/find_import.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      100 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/prune_broken_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       46 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/py.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       76 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/pyflyby_diff.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       84 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/reformat_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      100 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/replace_star_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       76 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/tidy_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       91 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/cli/transform_imports.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1057 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/conf.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      201 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/index.rst
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      760 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/make.bat
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      186 2021-09-24 06:20:21.000000 pyflyby-1.8.2/doc/testing.txt
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.148542 pyflyby-1.8.2/etc/
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.244672 pyflyby-1.8.2/etc/pyflyby/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      270 2021-09-24 06:20:21.000000 pyflyby-1.8.2/etc/pyflyby/canonical.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      569 2021-09-24 06:20:21.000000 pyflyby-1.8.2/etc/pyflyby/common.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      369 2021-09-24 06:20:21.000000 pyflyby-1.8.2/etc/pyflyby/forget.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      352 2021-09-24 06:20:21.000000 pyflyby-1.8.2/etc/pyflyby/mandatory.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    10418 2022-09-30 08:07:11.000000 pyflyby-1.8.2/etc/pyflyby/numpy.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    17409 2022-05-19 08:06:52.000000 pyflyby-1.8.2/etc/pyflyby/std.py
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.149524 pyflyby-1.8.2/lib/
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.246081 pyflyby-1.8.2/lib/emacs/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     4122 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/emacs/pyflyby.el
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.150128 pyflyby-1.8.2/lib/python/
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.265081 pyflyby-1.8.2/lib/python/pyflyby/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2712 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/__init__.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      296 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/__main__.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    82494 2022-09-30 05:55:12.000000 pyflyby-1.8.2/lib/python/pyflyby/_autoimp.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    20614 2023-02-27 05:52:44.000000 pyflyby-1.8.2/lib/python/pyflyby/_cmdline.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     4536 2022-09-09 06:09:39.000000 pyflyby-1.8.2/lib/python/pyflyby/_comms.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    46185 2022-10-12 05:57:20.000000 pyflyby-1.8.2/lib/python/pyflyby/_dbg.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    14280 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_docxref.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    22927 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_file.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7455 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_flags.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     6733 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_format.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7829 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_idents.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    21860 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_importclns.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    23556 2022-05-19 08:06:52.000000 pyflyby-1.8.2/lib/python/pyflyby/_importdb.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    23605 2023-02-27 05:52:44.000000 pyflyby-1.8.2/lib/python/pyflyby/_imports2s.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    17624 2023-02-27 05:52:44.000000 pyflyby-1.8.2/lib/python/pyflyby/_importstmt.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)   104335 2023-02-27 05:52:44.000000 pyflyby-1.8.2/lib/python/pyflyby/_interactive.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    30111 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_livepatch.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7915 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_log.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    15434 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_modules.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    56300 2022-10-12 05:57:20.000000 pyflyby-1.8.2/lib/python/pyflyby/_parse.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    76032 2022-05-19 08:06:52.000000 pyflyby-1.8.2/lib/python/pyflyby/_py.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    15506 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/_util.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      266 2023-02-27 05:54:03.000000 pyflyby-1.8.2/lib/python/pyflyby/_version.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      591 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/autoimport.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      600 2021-09-24 06:20:21.000000 pyflyby-1.8.2/lib/python/pyflyby/importdb.py
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.270109 pyflyby-1.8.2/lib/python/pyflyby.egg-info/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    14760 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/PKG-INFO
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     3410 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/SOURCES.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)        1 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/dependency_links.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       69 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/entry_points.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       42 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/requires.txt
--rw-rw-r--   0 ojha     (15539) ojha     (15539)        8 2023-02-27 06:04:38.000000 pyflyby-1.8.2/lib/python/pyflyby.egg-info/top_level.txt
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.150847 pyflyby-1.8.2/libexec/
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.271544 pyflyby-1.8.2/libexec/pyflyby/
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)      938 2022-05-19 08:06:52.000000 pyflyby-1.8.2/libexec/pyflyby/colordiff
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     5643 2021-09-24 06:20:21.000000 pyflyby-1.8.2/libexec/pyflyby/diff-colorize
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       38 2023-02-27 06:04:39.295327 pyflyby-1.8.2/setup.cfg
--rwxrwxr-x   0 ojha     (15539) ojha     (15539)     7941 2022-09-09 06:09:39.000000 pyflyby-1.8.2/setup.py
-drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-02-27 06:04:39.293342 pyflyby-1.8.2/tests/
--rw-rw-r--   0 ojha     (15539) ojha     (15539)       66 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/__init__.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2142 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_0testconfig.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    59623 2022-09-30 05:55:12.000000 pyflyby-1.8.2/tests/test_autoimp.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    20380 2022-05-19 08:06:52.000000 pyflyby-1.8.2/tests/test_cmdline.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2520 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_docxref.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    10550 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_file.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     5026 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_flags.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     4238 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_format.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2831 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_idents.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     8006 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_importclns.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7256 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_importdb.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    29623 2023-02-27 05:52:44.000000 pyflyby-1.8.2/tests/test_imports2s.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     7332 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_importstmt.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)   156373 2023-02-27 05:52:44.000000 pyflyby-1.8.2/tests/test_interactive.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1397 2022-05-19 08:06:52.000000 pyflyby-1.8.2/tests/test_jupyterlab_pyflyby.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    77476 2022-05-19 08:06:52.000000 pyflyby-1.8.2/tests/test_livepatch.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     2682 2022-05-19 08:06:52.000000 pyflyby-1.8.2/tests/test_modules.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    46716 2022-10-12 05:57:20.000000 pyflyby-1.8.2/tests/test_parse.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)    77998 2023-02-27 05:52:44.000000 pyflyby-1.8.2/tests/test_py.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)      857 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/test_util.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1851 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tests/xrefs.py
--rw-rw-r--   0 ojha     (15539) ojha     (15539)     1890 2021-09-24 06:20:21.000000 pyflyby-1.8.2/tox.ini
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.156559 pyflyby-1.8.3/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2965 2021-09-24 06:20:21.000000 pyflyby-1.8.3/.pyflyby
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1188 2021-09-24 06:20:21.000000 pyflyby-1.8.3/LICENSE.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      520 2022-05-19 08:06:52.000000 pyflyby-1.8.3/MANIFEST.in
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    14760 2023-04-17 07:48:56.156109 pyflyby-1.8.3/PKG-INFO
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    13790 2022-09-09 06:09:39.000000 pyflyby-1.8.3/README.rst
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.041353 pyflyby-1.8.3/bin/
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2441 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/autoipython
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      207 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/autopython
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2966 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/collect-exports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     2206 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/collect-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      238 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/create-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1035 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/find-import
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1130 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/list-bad-xrefs
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      926 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/prune-broken-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1079 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/py
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.072921 pyflyby-1.8.3/bin/pyflyby/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2712 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/__init__.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      296 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/__main__.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    82494 2022-09-30 05:55:12.000000 pyflyby-1.8.3/bin/pyflyby/_autoimp.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    20614 2023-02-27 05:52:44.000000 pyflyby-1.8.3/bin/pyflyby/_cmdline.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     4536 2022-09-09 06:09:39.000000 pyflyby-1.8.3/bin/pyflyby/_comms.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    46185 2022-10-12 05:57:20.000000 pyflyby-1.8.3/bin/pyflyby/_dbg.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    14280 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_docxref.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    22927 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_file.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7455 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_flags.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     6733 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_format.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7829 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_idents.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    21860 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_importclns.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    23556 2022-05-19 08:06:52.000000 pyflyby-1.8.3/bin/pyflyby/_importdb.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    23605 2023-02-27 05:52:44.000000 pyflyby-1.8.3/bin/pyflyby/_imports2s.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    17624 2023-02-27 05:52:44.000000 pyflyby-1.8.3/bin/pyflyby/_importstmt.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)   104335 2023-02-27 05:52:44.000000 pyflyby-1.8.3/bin/pyflyby/_interactive.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    30111 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_livepatch.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7915 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_log.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    15691 2023-04-17 07:36:28.000000 pyflyby-1.8.3/bin/pyflyby/_modules.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    56300 2022-10-12 05:57:20.000000 pyflyby-1.8.3/bin/pyflyby/_parse.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    78227 2023-04-17 07:36:28.000000 pyflyby-1.8.3/bin/pyflyby/_py.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    15506 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/_util.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      266 2023-04-17 07:46:14.000000 pyflyby-1.8.3/bin/pyflyby/_version.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      591 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/autoimport.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      600 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/pyflyby/importdb.py
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      938 2022-05-19 08:06:52.000000 pyflyby-1.8.3/bin/pyflyby-diff
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      755 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/reformat-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      978 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/replace-star-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     7855 2022-09-09 06:09:39.000000 pyflyby-1.8.3/bin/tidy-imports
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     1515 2021-09-24 06:20:21.000000 pyflyby-1.8.3/bin/transform-imports
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.080335 pyflyby-1.8.3/doc/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1188 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/LICENSE.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      855 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/Makefile
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     5686 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/TODO.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)        0 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/__init__.py
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.095446 pyflyby-1.8.3/doc/api/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      275 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/api.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       78 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/autoimp.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       78 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/cmdline.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       72 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/comms.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       66 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/dbg.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       69 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/file.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      123 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/flags.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       75 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/format.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      109 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/idents.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       86 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/importclns.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       80 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/importdb.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       83 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/imports2s.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       86 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/importstmt.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       89 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/interactive.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       83 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/livepatch.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       65 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/log.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       77 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/modules.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       71 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/parse.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       62 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/py.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       68 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/api/util.rst
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.104047 pyflyby-1.8.3/doc/cli/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      102 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/autoipython.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      273 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/cli.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       85 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/collect_exports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       85 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/collect_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       73 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/find_import.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      100 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/prune_broken_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       46 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/py.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       76 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/pyflyby_diff.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       84 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/reformat_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      100 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/replace_star_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       76 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/tidy_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       91 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/cli/transform_imports.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1057 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/conf.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      201 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/index.rst
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      760 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/make.bat
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      186 2021-09-24 06:20:21.000000 pyflyby-1.8.3/doc/testing.txt
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.020379 pyflyby-1.8.3/etc/
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.108559 pyflyby-1.8.3/etc/pyflyby/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      270 2021-09-24 06:20:21.000000 pyflyby-1.8.3/etc/pyflyby/canonical.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      569 2021-09-24 06:20:21.000000 pyflyby-1.8.3/etc/pyflyby/common.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      369 2021-09-24 06:20:21.000000 pyflyby-1.8.3/etc/pyflyby/forget.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      352 2021-09-24 06:20:21.000000 pyflyby-1.8.3/etc/pyflyby/mandatory.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    10469 2023-04-17 07:36:28.000000 pyflyby-1.8.3/etc/pyflyby/numpy.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    17409 2022-05-19 08:06:52.000000 pyflyby-1.8.3/etc/pyflyby/std.py
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.021817 pyflyby-1.8.3/lib/
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.109639 pyflyby-1.8.3/lib/emacs/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     4122 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/emacs/pyflyby.el
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.022491 pyflyby-1.8.3/lib/python/
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.126822 pyflyby-1.8.3/lib/python/pyflyby/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2712 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/__init__.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      296 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/__main__.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    82494 2022-09-30 05:55:12.000000 pyflyby-1.8.3/lib/python/pyflyby/_autoimp.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    20614 2023-02-27 05:52:44.000000 pyflyby-1.8.3/lib/python/pyflyby/_cmdline.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     4536 2022-09-09 06:09:39.000000 pyflyby-1.8.3/lib/python/pyflyby/_comms.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    46185 2022-10-12 05:57:20.000000 pyflyby-1.8.3/lib/python/pyflyby/_dbg.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    14280 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_docxref.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    22927 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_file.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7455 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_flags.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     6733 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_format.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7829 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_idents.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    21860 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_importclns.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    23556 2022-05-19 08:06:52.000000 pyflyby-1.8.3/lib/python/pyflyby/_importdb.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    23605 2023-02-27 05:52:44.000000 pyflyby-1.8.3/lib/python/pyflyby/_imports2s.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    17624 2023-02-27 05:52:44.000000 pyflyby-1.8.3/lib/python/pyflyby/_importstmt.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)   104335 2023-02-27 05:52:44.000000 pyflyby-1.8.3/lib/python/pyflyby/_interactive.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    30111 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_livepatch.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7915 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_log.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    15691 2023-04-17 07:36:28.000000 pyflyby-1.8.3/lib/python/pyflyby/_modules.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    56300 2022-10-12 05:57:20.000000 pyflyby-1.8.3/lib/python/pyflyby/_parse.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    78227 2023-04-17 07:36:28.000000 pyflyby-1.8.3/lib/python/pyflyby/_py.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    15506 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/_util.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      266 2023-04-17 07:46:14.000000 pyflyby-1.8.3/lib/python/pyflyby/_version.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      591 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/autoimport.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      600 2021-09-24 06:20:21.000000 pyflyby-1.8.3/lib/python/pyflyby/importdb.py
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.131569 pyflyby-1.8.3/lib/python/pyflyby.egg-info/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    14760 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/PKG-INFO
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     3410 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)        1 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       69 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/entry_points.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       42 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/requires.txt
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)        8 2023-04-17 07:48:55.000000 pyflyby-1.8.3/lib/python/pyflyby.egg-info/top_level.txt
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.023240 pyflyby-1.8.3/libexec/
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.132810 pyflyby-1.8.3/libexec/pyflyby/
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)      938 2022-05-19 08:06:52.000000 pyflyby-1.8.3/libexec/pyflyby/colordiff
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     5643 2021-09-24 06:20:21.000000 pyflyby-1.8.3/libexec/pyflyby/diff-colorize
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       38 2023-04-17 07:48:56.156836 pyflyby-1.8.3/setup.cfg
+-rwxrwxr-x   0 ojha     (15539) ojha     (15539)     7941 2022-09-09 06:09:39.000000 pyflyby-1.8.3/setup.py
+drwxrwsr-x   0 ojha     (15539) ojha     (15539)        0 2023-04-17 07:48:56.155219 pyflyby-1.8.3/tests/
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)       66 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/__init__.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2142 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_0testconfig.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    59984 2023-04-17 07:36:28.000000 pyflyby-1.8.3/tests/test_autoimp.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    20380 2022-05-19 08:06:52.000000 pyflyby-1.8.3/tests/test_cmdline.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2520 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_docxref.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    10550 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_file.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     5026 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_flags.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     4238 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_format.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2831 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_idents.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     8006 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_importclns.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7256 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_importdb.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    29623 2023-02-27 05:52:44.000000 pyflyby-1.8.3/tests/test_imports2s.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     7332 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_importstmt.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)   156373 2023-02-27 05:52:44.000000 pyflyby-1.8.3/tests/test_interactive.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1397 2022-05-19 08:06:52.000000 pyflyby-1.8.3/tests/test_jupyterlab_pyflyby.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    77476 2022-05-19 08:06:52.000000 pyflyby-1.8.3/tests/test_livepatch.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     2682 2022-05-19 08:06:52.000000 pyflyby-1.8.3/tests/test_modules.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    46716 2022-10-12 05:57:20.000000 pyflyby-1.8.3/tests/test_parse.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)    81076 2023-04-17 07:36:28.000000 pyflyby-1.8.3/tests/test_py.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)      857 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/test_util.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1851 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tests/xrefs.py
+-rw-rw-r--   0 ojha     (15539) ojha     (15539)     1890 2021-09-24 06:20:21.000000 pyflyby-1.8.3/tox.ini
```

### Comparing `pyflyby-1.8.2/.pyflyby` & `pyflyby-1.8.3/.pyflyby`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/LICENSE.txt` & `pyflyby-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/MANIFEST.in` & `pyflyby-1.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/PKG-INFO` & `pyflyby-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyby
-Version: 1.8.2
+Version: 1.8.3
 Summary: pyflyby - Python development productivity tools, in particular automatic import management
 Home-page: https://pypi.org/project/pyflyby/
 Author: Karl Chen
 Author-email: quarl@8166.clguba.z.quarl.org
 License: MIT
 Project-URL: Documentation, https://deshaw.github.io/pyflyby/
 Project-URL: Source, https://github.com/deshaw/pyflyby
```

### Comparing `pyflyby-1.8.2/README.rst` & `pyflyby-1.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/autoipython` & `pyflyby-1.8.3/bin/autoipython`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/collect-exports` & `pyflyby-1.8.3/bin/collect-exports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/collect-imports` & `pyflyby-1.8.3/bin/collect-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/find-import` & `pyflyby-1.8.3/bin/find-import`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/list-bad-xrefs` & `pyflyby-1.8.3/bin/list-bad-xrefs`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/prune-broken-imports` & `pyflyby-1.8.3/bin/prune-broken-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/py` & `pyflyby-1.8.3/bin/py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/__init__.py` & `pyflyby-1.8.3/bin/pyflyby/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_autoimp.py` & `pyflyby-1.8.3/bin/pyflyby/_autoimp.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_cmdline.py` & `pyflyby-1.8.3/bin/pyflyby/_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_comms.py` & `pyflyby-1.8.3/bin/pyflyby/_comms.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_dbg.py` & `pyflyby-1.8.3/bin/pyflyby/_dbg.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_docxref.py` & `pyflyby-1.8.3/bin/pyflyby/_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_file.py` & `pyflyby-1.8.3/bin/pyflyby/_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_flags.py` & `pyflyby-1.8.3/bin/pyflyby/_flags.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_format.py` & `pyflyby-1.8.3/bin/pyflyby/_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_idents.py` & `pyflyby-1.8.3/bin/pyflyby/_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_importclns.py` & `pyflyby-1.8.3/bin/pyflyby/_importclns.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_importdb.py` & `pyflyby-1.8.3/bin/pyflyby/_importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_imports2s.py` & `pyflyby-1.8.3/bin/pyflyby/_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_importstmt.py` & `pyflyby-1.8.3/bin/pyflyby/_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_interactive.py` & `pyflyby-1.8.3/bin/pyflyby/_interactive.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_livepatch.py` & `pyflyby-1.8.3/bin/pyflyby/_livepatch.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_log.py` & `pyflyby-1.8.3/bin/pyflyby/_log.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_modules.py` & `pyflyby-1.8.3/bin/pyflyby/_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,23 +200,32 @@
         sys.meta_path.
         """
         name = str(self.name)
         if name in sys.modules:
             return True
         if self.parent and not self.parent.exists:
             return False
-        import pkgutil
+
+        # pkgutil.find_loader returns None for unimported Python 3
+        # namespace packages, so prefer importlib
+        try:
+            import importlib.util
+            find = importlib.util.find_spec
+        except ImportError:
+            import pkgutil
+            find = pkgutil.find_loader
+
         try:
-            loader = pkgutil.find_loader(name)
+            pkg = find(name)
         except Exception:
             # Catch all exceptions, not just ImportError.  If the __init__.py
             # for the parent package of the module raises an exception, it'll
             # propagate to here.
-            loader = None
-        return loader is not None
+            pkg = None
+        return pkg is not None
 
     @cached_attribute
     def filename(self):
         """
         Return the filename, if appropriate.
 
         The module itself will not be imported, but if the module is not a
```

### Comparing `pyflyby-1.8.2/bin/pyflyby/_parse.py` & `pyflyby-1.8.3/bin/pyflyby/_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/_py.py` & `pyflyby-1.8.3/bin/pyflyby/_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,18 @@
 # "print_function" here, but we also use auto_flags=True, which means
 # print_function may be flipped off if the code contains print statements.
 FLAGS = CompilerFlags(["absolute_import", "with_statement", "division",
                        "print_function"])
 
 
 def _get_argspec(arg, _recurse=False):
-    from inspect import getargspec, ArgSpec
+    if sys.version_info[0] == 3:
+        from inspect import getfullargspec as getargspec, FullArgSpec as ArgSpec
+    else:
+        from inspect import getargspec, ArgSpec
     if isinstance(arg, FunctionType):
         return getargspec(arg)
     elif isinstance(arg, MethodType):
         argspec = getargspec(arg)
         if arg.__self__ is not None:
             # For bound methods, ignore the "self" argument.
             return ArgSpec(argspec.args[1:], *argspec[1:])
@@ -401,15 +404,18 @@
     elif isinstance(arg, getattr(types, 'ClassType', type)):
         argspec = _get_argspec(arg.__init__)
         return ArgSpec(argspec.args[1:], *argspec[1:])
     elif _recurse and hasattr(arg, '__call__'):
         return _get_argspec(arg.__call__, _recurse=False)
     elif callable(arg):
         # Unknown, probably a built-in method.
-        return ArgSpec((), "args", "kwargs", None)
+        if sys.version_info[0] == 3:
+            return ArgSpec((), "args", "kwargs", None, [], None, {})
+        else:
+            return ArgSpec((), "args", "kwargs", None)
     raise TypeError(
         "_get_argspec: unexpected %s" % (type(arg).__name__,))
 
 
 def _requires_parens_as_function(function_name):
     """
     Returns whether the given string of a callable would require parentheses
@@ -493,15 +499,16 @@
 def _build_function_usage_string(function_name, argspec, prefix):
     usage = []
     # TODO: colorize
     usage.append("Python signature:")
     usage.append("  >"+">> " + _format_call_spec(function_name, argspec))
     usage.append("")
     usage.append("Command-line signature:")
-    if not argspec.args and argspec.varargs and argspec.keywords:
+    keywords = argspec.keywords if sys.version_info[0] == 2 else argspec.varkw
+    if not argspec.args and argspec.varargs and keywords:
         # We have no information about the arguments.  It's probably a
         # built-in where getargspec failed.
         usage.append("  $ %s%s ...\n" % (prefix, function_name))
         return "\n".join(usage)
     defaults = argspec.defaults or ()
     first_with_default = len(argspec.args) - len(defaults)
     # Show first alternative of command-line syntax.
@@ -510,27 +517,39 @@
         if i >= first_with_default:
             syntax1 += " [%s" % (arg,)
         else:
             syntax1 += " %s" % (arg,)
     if argspec.varargs:
         syntax1 += " %s..." % argspec.varargs
     syntax1 += "]" * len(defaults)
-    if argspec.keywords:
+    if sys.version_info[0] == 3:
+        for arg in argspec.kwonlyargs:
+            if argspec.kwonlydefaults and arg in argspec.kwonlydefaults:
+                syntax1 += " [--%s=...]" % (arg,)
+            else:
+                syntax1 += " --%s=..." % (arg,)
+    if keywords:
         syntax1 += " [--...]"
     usage.append(syntax1)
     # usage.append("or:")
     syntax2 = "  $ %s%s" % (prefix, shquote(function_name),)
     for i, arg in enumerate(argspec.args):
         if i >= first_with_default:
             syntax2 += " [--%s=...]" % (arg,)
         else:
             syntax2 += " --%s=..." % (arg,)
+    if sys.version_info[0] == 3:
+        for arg in argspec.kwonlyargs:
+            if argspec.kwonlydefaults and arg in argspec.kwonlydefaults:
+                syntax2 += " [--%s=...]" % (arg,)
+            else:
+                syntax2 += " --%s=..." % (arg,)
     if argspec.varargs:
         syntax2 += " %s..." % argspec.varargs
-    if argspec.keywords:
+    if keywords:
         syntax2 += " [--...]"
     usage.append(syntax2)
     usage.append("")
     return "\n".join(usage)
 
 
 class ParseError(Exception):
@@ -700,20 +719,28 @@
 
     # Create a map from argname to default value.
     defaults = argspec.defaults or ()
     argname2default = {}
     for argname, default in zip(argspec.args[len(argspec.args)-len(defaults):],
                                 defaults):
         argname2default[argname] = make_expr(default, "raw_value")
+    if sys.version_info[0] == 3:
+        if argspec.kwonlydefaults:
+            for argname, default in argspec.kwonlydefaults.items():
+                argname2default[argname] = make_expr(default, "raw_value")
     # Create a map from prefix to arguments with that prefix.  E.g. {"foo":
     # ["foobar", "foobaz"]}
     prefix2argname = {}
     for argname in argspec.args:
         for prefix in prefixes(argname):
             prefix2argname.setdefault(prefix, []).append(argname)
+    if sys.version_info[0] == 3:
+        for argname in argspec.kwonlyargs:
+            for prefix in prefixes(argname):
+                prefix2argname.setdefault(prefix, []).append(argname)
     # Enumerate over input arguments.
     got_pos_args = []
     got_keyword_args = {}
     args = list(commandline_args)
     while args:
         arg = args.pop(0)
         if arg in ["--?", "-?", "?"]:
@@ -744,16 +771,23 @@
                 argname, = matched_argnames
             elif len(matched_argnames) == 0:
                 if equalsign == "":
                     if argname in ["help", "h"]:
                         raise _ParseInterruptedWantHelp
                     if argname in ["source"]:
                         raise _ParseInterruptedWantSource
-                if not argspec.keywords:
-                    raise ParseError("Unknown option name %s" % (argname,))
+                if sys.version_info[0] == 3:
+                    if not argspec.varkw:
+                        raise ParseError("Unknown option name %s" %
+                                         (argname,))
+                else:
+                    if not argspec.keywords:
+                        raise ParseError("Unknown option name %s" %
+                                         (argname,))
+
             elif len(matched_argnames) > 1:
                 raise ParseError(
                     "Ambiguous %s: could mean one of: %s"
                     % (argname,
                        ", ".join("--%s"%s for s in matched_argnames)))
             else:
                 raise AssertionError
@@ -795,14 +829,33 @@
             value = expr.value
         except Exception as e:
             raise ParseError(
                 "Error parsing value for --%s=%s: %s: %s"
                 % (argname, expr, type(e).__name__, e))
         parsed_args.append(value)
 
+    if sys.version_info[0] == 3:
+        for argname in argspec.kwonlyargs:
+            try:
+                expr = got_keyword_args.pop(argname)
+            except KeyError:
+                try:
+                    expr = argname2default[argname]
+                except KeyError:
+                    raise ParseError(
+                        "missing required keyword argument %s" % (argname,))
+
+            try:
+                value = expr.value
+            except Exception as e:
+                raise ParseError(
+                    "Error parsing value for --%s=%s: %s: %s"
+                    % (argname, expr, type(e).__name__, e))
+            parsed_kwargs[argname] = value
+
     if len(got_pos_args) > len(argspec.args):
         if argspec.varargs:
             for expr in got_pos_args[len(argspec.args):]:
                 try:
                     value = expr.value
                 except Exception as e:
                     raise ParseError(
```

### Comparing `pyflyby-1.8.2/bin/pyflyby/_util.py` & `pyflyby-1.8.3/bin/pyflyby/_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/autoimport.py` & `pyflyby-1.8.3/bin/pyflyby/autoimport.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby/importdb.py` & `pyflyby-1.8.3/bin/pyflyby/importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/pyflyby-diff` & `pyflyby-1.8.3/bin/pyflyby-diff`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/reformat-imports` & `pyflyby-1.8.3/bin/reformat-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/replace-star-imports` & `pyflyby-1.8.3/bin/replace-star-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/tidy-imports` & `pyflyby-1.8.3/bin/tidy-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/bin/transform-imports` & `pyflyby-1.8.3/bin/transform-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/doc/LICENSE.txt` & `pyflyby-1.8.3/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/doc/Makefile` & `pyflyby-1.8.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/doc/TODO.txt` & `pyflyby-1.8.3/doc/TODO.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/doc/conf.py` & `pyflyby-1.8.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/doc/make.bat` & `pyflyby-1.8.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/etc/pyflyby/common.py` & `pyflyby-1.8.3/etc/pyflyby/common.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/etc/pyflyby/numpy.py` & `pyflyby-1.8.3/etc/pyflyby/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,49 +52,50 @@
                                         flatnonzero, fliplr, flipud, float32,
                                         float64, float_, floating, floor,
                                         floor_divide, fmax, fmin, fmod, frexp,
                                         frombuffer, fromfile, fromfunction,
                                         fromiter, frompyfunc, fromregex,
                                         fromstring, gradient, greater,
                                         greater_equal, hamming, hanning,
-                                        histogram, histogram2d, histogramdd,
-                                        hsplit, hstack, hypot, i0, identity,
-                                        iinfo, imag, in1d, index_exp, indices,
-                                        inexact, inf, inner, int0, int16,
-                                        int32, int64, int8, int_, intc,
-                                        integer, interp, intersect1d, intp,
-                                        invert, ipmt, irr, iscomplex,
-                                        iscomplexobj, isfinite, isfortran,
-                                        isinf, isnan, isneginf, isposinf,
-                                        isreal, isrealobj, isscalar, issctype,
-                                        issubclass_, issubdtype, issubsctype,
-                                        iterable, ix_, kaiser, kron, ldexp,
-                                        left_shift, less, less_equal, lexsort,
-                                        linalg, linspace, little_endian,
-                                        loadtxt, log, log as logarithm, log10,
-                                        log1p, log2, logaddexp, logaddexp2,
-                                        logical_and, logical_not, logical_or,
-                                        logical_xor, logspace, longcomplex,
-                                        longdouble, longfloat, longlong,
-                                        mafromtxt, mask_indices, mat, matrix,
-                                        maximum, mean, median, memmap,
-                                        meshgrid, mgrid, minimum, mintypecode,
-                                        mirr, mod, modf, msort, multiply, nan,
-                                        nan_to_num, nanargmax, nanargmin,
-                                        nanmax, nanmin, nansum, nbytes,
-                                        ndarray, ndenumerate, ndim, ndindex,
-                                        negative, newaxis, newbuffer,
-                                        nextafter, nonzero, not_equal, nper,
-                                        npv, number, object0, object_, ogrid,
-                                        ones, ones_like, outer, packbits, pi,
-                                        piecewise, pkgload, place, pmt, poly,
-                                        poly1d, polyadd, polyder, polydiv,
-                                        polyfit, polyint, polymul, polynomial,
-                                        polysub, polyval, power, ppmt, prod,
-                                        product, ptp, putmask, pv, r_, rad2deg,
+                                        heaviside, histogram, histogram2d,
+                                        histogramdd, hsplit, hstack, hypot,
+                                        i0, identity, iinfo, imag, in1d,
+                                        index_exp, indices, inexact, inf,
+                                        inner, int0, int16, int32, int64,
+                                        int8, int_, intc, integer, interp,
+                                        intersect1d, intp, invert, ipmt, irr,
+                                        iscomplex, iscomplexobj, isfinite,
+                                        isfortran, isinf, isnan, isneginf,
+                                        isposinf, isreal, isrealobj, isscalar,
+                                        issctype, issubclass_, issubdtype,
+                                        issubsctype, iterable, ix_, kaiser,
+                                        kron, ldexp, left_shift, less,
+                                        less_equal, lexsort, linalg, linspace,
+                                        little_endian, loadtxt, log,
+                                        log as logarithm, log10, log1p, log2,
+                                        logaddexp, logaddexp2, logical_and,
+                                        logical_not, logical_or, logical_xor,
+                                        logspace, longcomplex, longdouble,
+                                        longfloat, longlong, mafromtxt,
+                                        mask_indices, mat, matrix, maximum,
+                                        mean, median, memmap, meshgrid, mgrid,
+                                        minimum, mintypecode, mirr, mod, modf,
+                                        msort, multiply, nan, nan_to_num,
+                                        nanargmax, nanargmin, nanmax, nanmin,
+                                        nansum, nbytes, ndarray, ndenumerate,
+                                        ndim, ndindex, negative, newaxis,
+                                        newbuffer, nextafter, nonzero,
+                                        not_equal, nper, npv, number, object0,
+                                        object_, ogrid, ones, ones_like,
+                                        outer, packbits, pi, piecewise,
+                                        pkgload, place, pmt, poly, poly1d,
+                                        polyadd, polyder, polydiv, polyfit,
+                                        polyint, polymul, polynomial, polysub,
+                                        polyval, power, ppmt, prod, product,
+                                        ptp, putmask, pv, r_, rad2deg,
                                         radians, rank, rate, ravel, real,
                                         real_if_close, recarray, recfromcsv,
                                         recfromtxt, reciprocal, record,
                                         remainder, repeat, reshape, resize,
                                         restoredot, right_shift, rint, roll,
                                         rollaxis, roots, rot90, round, round_,
                                         row_stack, s_, searchsorted,
```

### Comparing `pyflyby-1.8.2/etc/pyflyby/std.py` & `pyflyby-1.8.3/etc/pyflyby/std.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/emacs/pyflyby.el` & `pyflyby-1.8.3/lib/emacs/pyflyby.el`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/__init__.py` & `pyflyby-1.8.3/lib/python/pyflyby/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_autoimp.py` & `pyflyby-1.8.3/lib/python/pyflyby/_autoimp.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_cmdline.py` & `pyflyby-1.8.3/lib/python/pyflyby/_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_comms.py` & `pyflyby-1.8.3/lib/python/pyflyby/_comms.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_dbg.py` & `pyflyby-1.8.3/lib/python/pyflyby/_dbg.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_docxref.py` & `pyflyby-1.8.3/lib/python/pyflyby/_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_file.py` & `pyflyby-1.8.3/lib/python/pyflyby/_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_flags.py` & `pyflyby-1.8.3/lib/python/pyflyby/_flags.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_format.py` & `pyflyby-1.8.3/lib/python/pyflyby/_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_idents.py` & `pyflyby-1.8.3/lib/python/pyflyby/_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_importclns.py` & `pyflyby-1.8.3/lib/python/pyflyby/_importclns.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_importdb.py` & `pyflyby-1.8.3/lib/python/pyflyby/_importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_imports2s.py` & `pyflyby-1.8.3/lib/python/pyflyby/_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_importstmt.py` & `pyflyby-1.8.3/lib/python/pyflyby/_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_interactive.py` & `pyflyby-1.8.3/lib/python/pyflyby/_interactive.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_livepatch.py` & `pyflyby-1.8.3/lib/python/pyflyby/_livepatch.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_log.py` & `pyflyby-1.8.3/lib/python/pyflyby/_log.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_modules.py` & `pyflyby-1.8.3/lib/python/pyflyby/_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,23 +200,32 @@
         sys.meta_path.
         """
         name = str(self.name)
         if name in sys.modules:
             return True
         if self.parent and not self.parent.exists:
             return False
-        import pkgutil
+
+        # pkgutil.find_loader returns None for unimported Python 3
+        # namespace packages, so prefer importlib
+        try:
+            import importlib.util
+            find = importlib.util.find_spec
+        except ImportError:
+            import pkgutil
+            find = pkgutil.find_loader
+
         try:
-            loader = pkgutil.find_loader(name)
+            pkg = find(name)
         except Exception:
             # Catch all exceptions, not just ImportError.  If the __init__.py
             # for the parent package of the module raises an exception, it'll
             # propagate to here.
-            loader = None
-        return loader is not None
+            pkg = None
+        return pkg is not None
 
     @cached_attribute
     def filename(self):
         """
         Return the filename, if appropriate.
 
         The module itself will not be imported, but if the module is not a
```

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_parse.py` & `pyflyby-1.8.3/lib/python/pyflyby/_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_py.py` & `pyflyby-1.8.3/lib/python/pyflyby/_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,18 @@
 # "print_function" here, but we also use auto_flags=True, which means
 # print_function may be flipped off if the code contains print statements.
 FLAGS = CompilerFlags(["absolute_import", "with_statement", "division",
                        "print_function"])
 
 
 def _get_argspec(arg, _recurse=False):
-    from inspect import getargspec, ArgSpec
+    if sys.version_info[0] == 3:
+        from inspect import getfullargspec as getargspec, FullArgSpec as ArgSpec
+    else:
+        from inspect import getargspec, ArgSpec
     if isinstance(arg, FunctionType):
         return getargspec(arg)
     elif isinstance(arg, MethodType):
         argspec = getargspec(arg)
         if arg.__self__ is not None:
             # For bound methods, ignore the "self" argument.
             return ArgSpec(argspec.args[1:], *argspec[1:])
@@ -401,15 +404,18 @@
     elif isinstance(arg, getattr(types, 'ClassType', type)):
         argspec = _get_argspec(arg.__init__)
         return ArgSpec(argspec.args[1:], *argspec[1:])
     elif _recurse and hasattr(arg, '__call__'):
         return _get_argspec(arg.__call__, _recurse=False)
     elif callable(arg):
         # Unknown, probably a built-in method.
-        return ArgSpec((), "args", "kwargs", None)
+        if sys.version_info[0] == 3:
+            return ArgSpec((), "args", "kwargs", None, [], None, {})
+        else:
+            return ArgSpec((), "args", "kwargs", None)
     raise TypeError(
         "_get_argspec: unexpected %s" % (type(arg).__name__,))
 
 
 def _requires_parens_as_function(function_name):
     """
     Returns whether the given string of a callable would require parentheses
@@ -493,15 +499,16 @@
 def _build_function_usage_string(function_name, argspec, prefix):
     usage = []
     # TODO: colorize
     usage.append("Python signature:")
     usage.append("  >"+">> " + _format_call_spec(function_name, argspec))
     usage.append("")
     usage.append("Command-line signature:")
-    if not argspec.args and argspec.varargs and argspec.keywords:
+    keywords = argspec.keywords if sys.version_info[0] == 2 else argspec.varkw
+    if not argspec.args and argspec.varargs and keywords:
         # We have no information about the arguments.  It's probably a
         # built-in where getargspec failed.
         usage.append("  $ %s%s ...\n" % (prefix, function_name))
         return "\n".join(usage)
     defaults = argspec.defaults or ()
     first_with_default = len(argspec.args) - len(defaults)
     # Show first alternative of command-line syntax.
@@ -510,27 +517,39 @@
         if i >= first_with_default:
             syntax1 += " [%s" % (arg,)
         else:
             syntax1 += " %s" % (arg,)
     if argspec.varargs:
         syntax1 += " %s..." % argspec.varargs
     syntax1 += "]" * len(defaults)
-    if argspec.keywords:
+    if sys.version_info[0] == 3:
+        for arg in argspec.kwonlyargs:
+            if argspec.kwonlydefaults and arg in argspec.kwonlydefaults:
+                syntax1 += " [--%s=...]" % (arg,)
+            else:
+                syntax1 += " --%s=..." % (arg,)
+    if keywords:
         syntax1 += " [--...]"
     usage.append(syntax1)
     # usage.append("or:")
     syntax2 = "  $ %s%s" % (prefix, shquote(function_name),)
     for i, arg in enumerate(argspec.args):
         if i >= first_with_default:
             syntax2 += " [--%s=...]" % (arg,)
         else:
             syntax2 += " --%s=..." % (arg,)
+    if sys.version_info[0] == 3:
+        for arg in argspec.kwonlyargs:
+            if argspec.kwonlydefaults and arg in argspec.kwonlydefaults:
+                syntax2 += " [--%s=...]" % (arg,)
+            else:
+                syntax2 += " --%s=..." % (arg,)
     if argspec.varargs:
         syntax2 += " %s..." % argspec.varargs
-    if argspec.keywords:
+    if keywords:
         syntax2 += " [--...]"
     usage.append(syntax2)
     usage.append("")
     return "\n".join(usage)
 
 
 class ParseError(Exception):
@@ -700,20 +719,28 @@
 
     # Create a map from argname to default value.
     defaults = argspec.defaults or ()
     argname2default = {}
     for argname, default in zip(argspec.args[len(argspec.args)-len(defaults):],
                                 defaults):
         argname2default[argname] = make_expr(default, "raw_value")
+    if sys.version_info[0] == 3:
+        if argspec.kwonlydefaults:
+            for argname, default in argspec.kwonlydefaults.items():
+                argname2default[argname] = make_expr(default, "raw_value")
     # Create a map from prefix to arguments with that prefix.  E.g. {"foo":
     # ["foobar", "foobaz"]}
     prefix2argname = {}
     for argname in argspec.args:
         for prefix in prefixes(argname):
             prefix2argname.setdefault(prefix, []).append(argname)
+    if sys.version_info[0] == 3:
+        for argname in argspec.kwonlyargs:
+            for prefix in prefixes(argname):
+                prefix2argname.setdefault(prefix, []).append(argname)
     # Enumerate over input arguments.
     got_pos_args = []
     got_keyword_args = {}
     args = list(commandline_args)
     while args:
         arg = args.pop(0)
         if arg in ["--?", "-?", "?"]:
@@ -744,16 +771,23 @@
                 argname, = matched_argnames
             elif len(matched_argnames) == 0:
                 if equalsign == "":
                     if argname in ["help", "h"]:
                         raise _ParseInterruptedWantHelp
                     if argname in ["source"]:
                         raise _ParseInterruptedWantSource
-                if not argspec.keywords:
-                    raise ParseError("Unknown option name %s" % (argname,))
+                if sys.version_info[0] == 3:
+                    if not argspec.varkw:
+                        raise ParseError("Unknown option name %s" %
+                                         (argname,))
+                else:
+                    if not argspec.keywords:
+                        raise ParseError("Unknown option name %s" %
+                                         (argname,))
+
             elif len(matched_argnames) > 1:
                 raise ParseError(
                     "Ambiguous %s: could mean one of: %s"
                     % (argname,
                        ", ".join("--%s"%s for s in matched_argnames)))
             else:
                 raise AssertionError
@@ -795,14 +829,33 @@
             value = expr.value
         except Exception as e:
             raise ParseError(
                 "Error parsing value for --%s=%s: %s: %s"
                 % (argname, expr, type(e).__name__, e))
         parsed_args.append(value)
 
+    if sys.version_info[0] == 3:
+        for argname in argspec.kwonlyargs:
+            try:
+                expr = got_keyword_args.pop(argname)
+            except KeyError:
+                try:
+                    expr = argname2default[argname]
+                except KeyError:
+                    raise ParseError(
+                        "missing required keyword argument %s" % (argname,))
+
+            try:
+                value = expr.value
+            except Exception as e:
+                raise ParseError(
+                    "Error parsing value for --%s=%s: %s: %s"
+                    % (argname, expr, type(e).__name__, e))
+            parsed_kwargs[argname] = value
+
     if len(got_pos_args) > len(argspec.args):
         if argspec.varargs:
             for expr in got_pos_args[len(argspec.args):]:
                 try:
                     value = expr.value
                 except Exception as e:
                     raise ParseError(
```

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/_util.py` & `pyflyby-1.8.3/lib/python/pyflyby/_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/autoimport.py` & `pyflyby-1.8.3/lib/python/pyflyby/autoimport.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby/importdb.py` & `pyflyby-1.8.3/lib/python/pyflyby/importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/lib/python/pyflyby.egg-info/PKG-INFO` & `pyflyby-1.8.3/lib/python/pyflyby.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyby
-Version: 1.8.2
+Version: 1.8.3
 Summary: pyflyby - Python development productivity tools, in particular automatic import management
 Home-page: https://pypi.org/project/pyflyby/
 Author: Karl Chen
 Author-email: quarl@8166.clguba.z.quarl.org
 License: MIT
 Project-URL: Documentation, https://deshaw.github.io/pyflyby/
 Project-URL: Source, https://github.com/deshaw/pyflyby
```

### Comparing `pyflyby-1.8.2/lib/python/pyflyby.egg-info/SOURCES.txt` & `pyflyby-1.8.3/lib/python/pyflyby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/libexec/pyflyby/colordiff` & `pyflyby-1.8.3/libexec/pyflyby/colordiff`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/libexec/pyflyby/diff-colorize` & `pyflyby-1.8.3/libexec/pyflyby/diff-colorize`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/setup.py` & `pyflyby-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_0testconfig.py` & `pyflyby-1.8.3/tests/test_0testconfig.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_autoimp.py` & `pyflyby-1.8.3/tests/test_autoimp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2118,7 +2118,19 @@
 
 def test_post_import_hook_fullname():
     db = ImportDB('import numpy.compat')
     expected = Import('import numpy.compat')
     def test_hook(val):
         assert val == expected
     auto_import("numpy.compat", [{}], db=db, post_import_hook=test_hook)
+
+@pytest.mark.skipif(
+    PY2,
+    reason="Python 3-only namespace package.")
+def test_namespace_package(tpp, capsys):
+    os.mkdir(str(tpp/'namespace_package'))
+    auto_import("namespace_package", [{}])
+    out, _ = capsys.readouterr()
+    expected = dedent("""
+        [PYFLYBY] import namespace_package
+    """).lstrip()
+    assert out.startswith(expected)
```

### Comparing `pyflyby-1.8.2/tests/test_cmdline.py` & `pyflyby-1.8.3/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_docxref.py` & `pyflyby-1.8.3/tests/test_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_file.py` & `pyflyby-1.8.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_flags.py` & `pyflyby-1.8.3/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_format.py` & `pyflyby-1.8.3/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_idents.py` & `pyflyby-1.8.3/tests/test_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_importclns.py` & `pyflyby-1.8.3/tests/test_importclns.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_importdb.py` & `pyflyby-1.8.3/tests/test_importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_imports2s.py` & `pyflyby-1.8.3/tests/test_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_importstmt.py` & `pyflyby-1.8.3/tests/test_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_interactive.py` & `pyflyby-1.8.3/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_jupyterlab_pyflyby.py` & `pyflyby-1.8.3/tests/test_jupyterlab_pyflyby.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_livepatch.py` & `pyflyby-1.8.3/tests/test_livepatch.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_modules.py` & `pyflyby-1.8.3/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_parse.py` & `pyflyby-1.8.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/test_py.py` & `pyflyby-1.8.3/tests/test_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,14 +368,122 @@
     expected = dedent("""
         [PYFLYBY] round(2.984375, ndigits=3)
         2.984
     """).strip()
     assert expected == result
 
 
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_kwonlyargs_1():
+    result = py("--apply", "lambda x, *, y: x + y", "2", "--y=3")
+    expected = dedent("""
+        [PYFLYBY] (lambda x, *, y: x + y)(2, y=3)
+        5
+    """).strip()
+    assert expected == result
+
+
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_kwonlyargs_2():
+    result = py("--apply", "lambda x, *, y, z=1: x + y + z", "2", "--y=3")
+    expected = dedent("""
+        [PYFLYBY] (lambda x, *, y, z=1: x + y + z)(2, y=3, z=1)
+        6
+    """).strip()
+    assert expected == result
+
+
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_kwonlyargs_3():
+    result = py("--apply", "lambda x, *, y, z=1: x + y + z", "2", "--y=3", "--z=4")
+    expected = dedent("""
+        [PYFLYBY] (lambda x, *, y, z=1: x + y + z)(2, y=3, z=4)
+        9
+    """).strip()
+    assert expected == result
+
+
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_kwonlyargs_4():
+    result = py("--apply", "lambda x, *, y, z=1: x + y + z", "2", "3")
+    expected = dedent("""
+        [PYFLYBY] missing required keyword argument y
+
+        Python signature:
+          >>> (lambda x, *, y, z=1: x + y + z)(x, *, y, z=1)
+
+        Command-line signature:
+          $ py 'lambda x, *, y, z=1: x + y + z' x --y=... [--z=...]
+          $ py 'lambda x, *, y, z=1: x + y + z' --x=... --y=... [--z=...]
+
+        Filename:
+          <unknown>
+
+        Docstring:
+          (No docstring)
+    """).strip(), 1
+    assert expected == result
+
+
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_kwonlyargs_5():
+    result = py("--apply", "lambda x, *, y, z=1: x + y + z", "2", "--z=3")
+    expected = dedent("""
+        [PYFLYBY] missing required keyword argument y
+
+        Python signature:
+          >>> (lambda x, *, y, z=1: x + y + z)(x, *, y, z=1)
+
+        Command-line signature:
+          $ py 'lambda x, *, y, z=1: x + y + z' x --y=... [--z=...]
+          $ py 'lambda x, *, y, z=1: x + y + z' --x=... --y=... [--z=...]
+
+        Filename:
+          <unknown>
+
+        Docstring:
+          (No docstring)
+    """).strip(), 1
+    assert expected == result
+
+
+@pytest.mark.skipif(
+    sys.version_info[0] != 3, reason="keyword-only args require Python 3"
+)
+def test_apply_unknown_option():
+    result = py("--apply", "lambda a, *, b=10, c: a + b", "2", "--b=15", "-c=1", "-d=6")
+    expected = dedent("""
+        [PYFLYBY] Unknown option name d
+
+        Python signature:
+          >>> (lambda a, *, b=10, c: a + b)(a, *, b=10, c)
+
+        Command-line signature:
+          $ py 'lambda a, *, b=10, c: a + b' a [--b=...] --c=...
+          $ py 'lambda a, *, b=10, c: a + b' --a=... [--b=...] --c=...
+
+        Filename:
+          <unknown>
+
+        Docstring:
+          (No docstring)
+    """).strip(), 1
+    assert expected == result
+
+
 def test_apply_print_function_1():
     result = py("--apply", "print", "50810461")
     expected = dedent("""
         [PYFLYBY] print(50810461)
         50810461
     """).strip()
     assert expected == result
```

### Comparing `pyflyby-1.8.2/tests/test_util.py` & `pyflyby-1.8.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tests/xrefs.py` & `pyflyby-1.8.3/tests/xrefs.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.8.2/tox.ini` & `pyflyby-1.8.3/tox.ini`

 * *Files identical despite different names*

