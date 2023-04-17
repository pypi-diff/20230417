# Comparing `tmp/scalene-1.5.8.tar.gz` & `tmp/scalene-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scalene-1.5.8.tar", last modified: Fri Apr 29 20:48:53 2022, max compression
+gzip compressed data, was "dist/scalene-1.5.9.tar", last modified: Sun Jul 24 23:30:01 2022, max compression
```

## Comparing `scalene-1.5.8.tar` & `scalene-1.5.9.tar`

### file list

```diff
@@ -1,343 +1,344 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/.github/
--rw-r--r--   0 runner     (501) staff       (20)       83 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner     (501) staff       (20)      665 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner     (501) staff       (20)      595 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     4044 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/workflows/build-and-upload.yml
--rw-r--r--   0 runner     (501) staff       (20)      233 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/workflows/test-homebrew-install.yml
--rw-r--r--   0 runner     (501) staff       (20)     1312 2022-04-29 20:48:11.000000 scalene-1.5.8/.github/workflows/test-smoketests.yml
--rw-r--r--   0 runner     (501) staff       (20)     2387 2022-04-29 20:48:11.000000 scalene-1.5.8/.gitignore
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/.vscode/
--rw-r--r--   0 runner     (501) staff       (20)      735 2022-04-29 20:48:11.000000 scalene-1.5.8/.vscode/c_cpp_properties.json
--rw-r--r--   0 runner     (501) staff       (20)     3354 2022-04-29 20:48:11.000000 scalene-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner     (501) staff       (20)     3134 2022-04-29 20:48:11.000000 scalene-1.5.8/GNUmakefile
--rw-r--r--   0 runner     (501) staff       (20)    11358 2022-04-29 20:48:11.000000 scalene-1.5.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      100 2022-04-29 20:48:11.000000 scalene-1.5.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1326 2022-04-29 20:48:11.000000 scalene-1.5.8/Makefile
--rw-r--r--   0 runner     (501) staff       (20)    17435 2022-04-29 20:48:53.000000 scalene-1.5.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      201 2022-04-29 20:48:11.000000 scalene-1.5.8/Pipfile
--rw-r--r--   0 runner     (501) staff       (20)     8244 2022-04-29 20:48:11.000000 scalene-1.5.8/Pipfile.lock
--rwxr-xr-x   0 runner     (501) staff       (20)    16179 2022-04-29 20:48:11.000000 scalene-1.5.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/benchmarks/
--rw-r--r--   0 runner     (501) staff       (20)     8083 2022-04-29 20:48:11.000000 scalene-1.5.8/benchmarks/benchmark.py
--rw-r--r--   0 runner     (501) staff       (20)     2797 2022-04-29 20:48:11.000000 scalene-1.5.8/benchmarks/julia1_nopil.py
--rw-r--r--   0 runner     (501) staff       (20)     7444 2022-04-29 20:48:11.000000 scalene-1.5.8/benchmarks/pystone.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/docs/
--rw-r--r--   0 runner     (501) staff       (20)   307193 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/Ozsvald-tweet.png
--rwxr-xr-x   0 runner     (501) staff       (20)     9898 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/README_CN.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/docs/images/
--rw-r--r--   0 runner     (501) staff       (20)   244350 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/images/profiler-comparison.png
--rw-r--r--   0 runner     (501) staff       (20)   300776 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/images/sample-profile-pystone.png
--rw-r--r--   0 runner     (501) staff       (20)   196143 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/images/scalene-video-img.png
--rw-r--r--   0 runner     (501) staff       (20)    27943 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-demo.ipynb
--rw-r--r--   0 runner     (501) staff       (20)  1086911 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-gui-example-full.png
--rw-r--r--   0 runner     (501) staff       (20)    93644 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-gui-example.png
--rw-r--r--   0 runner     (501) staff       (20)   119139 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-image-large.png
--rw-r--r--   0 runner     (501) staff       (20)   107546 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-image-old.png
--rw-r--r--   0 runner     (501) staff       (20)   119139 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-image.png
--rw-r--r--   0 runner     (501) staff       (20)  1354390 2022-04-29 20:48:11.000000 scalene-1.5.8/docs/scalene-paper.pdf
--rw-r--r--   0 runner     (501) staff       (20)     1069 2022-04-29 20:48:11.000000 scalene-1.5.8/mypy.ini
--rw-r--r--   0 runner     (501) staff       (20)      149 2022-04-29 20:48:11.000000 scalene-1.5.8/pyrightconfig.json
--rw-r--r--   0 runner     (501) staff       (20)       29 2022-04-29 20:48:11.000000 scalene-1.5.8/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)      164 2022-04-29 20:48:11.000000 scalene-1.5.8/requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene/
--rw-r--r--   0 runner     (501) staff       (20)     1631 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/README.md
--rw-r--r--   0 runner     (501) staff       (20)       57 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      523 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     1565 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/adaptive.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene/old/
--rw-r--r--   0 runner     (501) staff       (20)     5533 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/old/leak_analysis.py
--rw-r--r--   0 runner     (501) staff       (20)     1130 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/profile.py
--rw-r--r--   0 runner     (501) staff       (20)      434 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_exit.py
--rw-r--r--   0 runner     (501) staff       (20)      629 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_fork.py
--rw-r--r--   0 runner     (501) staff       (20)      375 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_get_context.py
--rw-r--r--   0 runner     (501) staff       (20)     2126 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_lock.py
--rw-r--r--   0 runner     (501) staff       (20)     1101 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_mp_lock.py
--rw-r--r--   0 runner     (501) staff       (20)     1906 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_pjoin.py
--rw-r--r--   0 runner     (501) staff       (20)     1299 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_poll_selector.py
--rw-r--r--   0 runner     (501) staff       (20)     3805 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_signal_fns.py
--rw-r--r--   0 runner     (501) staff       (20)     1054 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/replacement_thread_join.py
--rw-r--r--   0 runner     (501) staff       (20)     2060 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/runningstats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene/scalene-gui/
--rw-r--r--   0 runner     (501) staff       (20)     1008 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/README.md
--rw-r--r--   0 runner     (501) staff       (20)   346688 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/example-profile.js
--rw-r--r--   0 runner     (501) staff       (20)    15086 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/favicon.ico
--rw-r--r--   0 runner     (501) staff       (20)     3671 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/index.html
--rw-r--r--   0 runner     (501) staff       (20)     2478 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/prism.css
--rw-r--r--   0 runner     (501) staff       (20)    64658 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/prism.js
--rw-r--r--   0 runner     (501) staff       (20)    16012 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/profile.json
--rw-r--r--   0 runner     (501) staff       (20)     2300 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/profiler.html
--rw-r--r--   0 runner     (501) staff       (20)      112 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/scalene-demo.js
--rw-r--r--   0 runner     (501) staff       (20)       13 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/scalene-fetch.js
--rw-r--r--   0 runner     (501) staff       (20)    23080 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/scalene-gui.js
--rw-r--r--   0 runner     (501) staff       (20)   119139 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/scalene-image.png
--rw-r--r--   0 runner     (501) staff       (20)     7784 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/tablesort.js
--rw-r--r--   0 runner     (501) staff       (20)      755 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-gui/tablesort.number.js
--rw-r--r--   0 runner     (501) staff       (20)     3547 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene-usage.txt
--rw-r--r--   0 runner     (501) staff       (20)     1969 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_apple_gpu.py
--rw-r--r--   0 runner     (501) staff       (20)     1695 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_arguments.py
--rw-r--r--   0 runner     (501) staff       (20)     1909 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_client_timer.py
--rw-r--r--   0 runner     (501) staff       (20)     1174 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_funcutils.py
--rw-r--r--   0 runner     (501) staff       (20)     1708 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_gpu.py
--rw-r--r--   0 runner     (501) staff       (20)    15171 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_json.py
--rw-r--r--   0 runner     (501) staff       (20)     1398 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_leak_analysis.py
--rw-r--r--   0 runner     (501) staff       (20)     3403 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_magics.py
--rw-r--r--   0 runner     (501) staff       (20)     2457 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_mapfile.py
--rw-r--r--   0 runner     (501) staff       (20)    27000 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_output.py
--rw-r--r--   0 runner     (501) staff       (20)    10968 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_parseargs.py
--rw-r--r--   0 runner     (501) staff       (20)     4311 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_preload.py
--rw-r--r--   0 runner     (501) staff       (20)    70596 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_profiler.py
--rw-r--r--   0 runner     (501) staff       (20)     1951 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_signals.py
--rw-r--r--   0 runner     (501) staff       (20)     1301 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_sigqueue.py
--rw-r--r--   0 runner     (501) staff       (20)    16816 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_statistics.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/scalene_version.py
--rw-r--r--   0 runner     (501) staff       (20)     2268 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/sparkline.py
--rw-r--r--   0 runner     (501) staff       (20)      342 2022-04-29 20:48:11.000000 scalene-1.5.8/scalene/syntaxline.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    17435 2022-04-29 20:48:52.000000 scalene-1.5.8/scalene.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    10081 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-04-29 20:48:52.000000 scalene-1.5.8/scalene.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       50 2022-04-29 20:48:52.000000 scalene-1.5.8/scalene.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       52 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2022-04-29 20:48:53.000000 scalene-1.5.8/scalene.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-04-29 20:48:53.000000 scalene-1.5.8/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     6564 2022-04-29 20:48:11.000000 scalene-1.5.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/src/include/
--rw-r--r--   0 runner     (501) staff       (20)      676 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/common.hpp
--rw-r--r--   0 runner     (501) staff       (20)    77989 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/libdivide.h
--rw-r--r--   0 runner     (501) staff       (20)     1241 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/lowdiscrepancy.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2104 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/mallocrecursionguard.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7652 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/memcpysampler.hpp
--rw-r--r--   0 runner     (501) staff       (20)      737 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/pywhere.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5181 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/samplefile.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8810 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/sampleheap.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1741 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/sampleinterval.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1794 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/sampler.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2192 2022-04-29 20:48:11.000000 scalene-1.5.8/src/include/scaleneheader.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/src/source/
--rw-r--r--   0 runner     (501) staff       (20)     2610 2022-04-29 20:48:11.000000 scalene-1.5.8/src/source/get_line_atomic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7378 2022-04-29 20:48:11.000000 scalene-1.5.8/src/source/libscalene.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7792 2022-04-29 20:48:11.000000 scalene-1.5.8/src/source/pywhere.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/test/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/test/issues/
--rw-r--r--   0 runner     (501) staff       (20)      111 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue124.py
--rw-r--r--   0 runner     (501) staff       (20)       67 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue130.py
--rw-r--r--   0 runner     (501) staff       (20)      188 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue156.py
--rw-r--r--   0 runner     (501) staff       (20)     1804 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue167.py
--rw-r--r--   0 runner     (501) staff       (20)      151 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue193.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue256.py
--rw-r--r--   0 runner     (501) staff       (20)      239 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue266.py
--rw-r--r--   0 runner     (501) staff       (20)      311 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue31.py
--rw-r--r--   0 runner     (501) staff       (20)      277 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue379.py
--rw-r--r--   0 runner     (501) staff       (20)      247 2022-04-29 20:48:11.000000 scalene-1.5.8/test/issues/test-issue74.py
--rw-r--r--   0 runner     (501) staff       (20)     1539 2022-04-29 20:48:11.000000 scalene-1.5.8/test/multiprocessing_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1181 2022-04-29 20:48:11.000000 scalene-1.5.8/test/new_mp_test.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/test/optimized/
--rwxr-xr-x   0 runner     (501) staff       (20)    20545 2022-04-29 20:48:11.000000 scalene-1.5.8/test/optimized/bm_pyflate.py
--rw-r--r--   0 runner     (501) staff       (20)    12330 2022-04-29 20:48:11.000000 scalene-1.5.8/test/optimized/bm_raytrace.py
--rw-r--r--   0 runner     (501) staff       (20)     9721 2022-04-29 20:48:11.000000 scalene-1.5.8/test/optimized/bm_richards.py
--rw-r--r--   0 runner     (501) staff       (20)    10363 2022-04-29 20:48:11.000000 scalene-1.5.8/test/optimized/bm_scimark.py
--rw-r--r--   0 runner     (501) staff       (20)     1997 2022-04-29 20:48:11.000000 scalene-1.5.8/test/optimized/bm_spectral_norm.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/test/original/
--rw-r--r--   0 runner     (501) staff       (20)     9396 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_mdp.py
--rwxr-xr-x   0 runner     (501) staff       (20)    20272 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_pyflate.py
--rw-r--r--   0 runner     (501) staff       (20)    12142 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_raytrace.py
--rw-r--r--   0 runner     (501) staff       (20)     9629 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_richards.py
--rw-r--r--   0 runner     (501) staff       (20)    10284 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_scimark.py
--rw-r--r--   0 runner     (501) staff       (20)     1773 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_spectral_norm.py
--rw-r--r--   0 runner     (501) staff       (20)     1512 2022-04-29 20:48:11.000000 scalene-1.5.8/test/original/bm_sympy.py
--rw-r--r--   0 runner     (501) staff       (20)      357 2022-04-29 20:48:11.000000 scalene-1.5.8/test/pool-test.py
--rw-r--r--   0 runner     (501) staff       (20)      400 2022-04-29 20:48:11.000000 scalene-1.5.8/test/small_mp_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1355 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test-martinheinz.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test-memory.py
--rw-r--r--   0 runner     (501) staff       (20)     1418 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test-pprofile.py
--rw-r--r--   0 runner     (501) staff       (20)     2145 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test-size.py
--rw-r--r--   0 runner     (501) staff       (20)     1942 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test_sparkline.py
--rw-r--r--   0 runner     (501) staff       (20)      354 2022-04-29 20:48:11.000000 scalene-1.5.8/test/test_timers.py
--rw-r--r--   0 runner     (501) staff       (20)      171 2022-04-29 20:48:11.000000 scalene-1.5.8/test/testflask-driver.py
--rw-r--r--   0 runner     (501) staff       (20)      248 2022-04-29 20:48:11.000000 scalene-1.5.8/test/testflask.py
--rw-r--r--   0 runner     (501) staff       (20)     1207 2022-04-29 20:48:11.000000 scalene-1.5.8/test/testme.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2022-04-29 20:48:11.000000 scalene-1.5.8/test/testpyt.py
--rw-r--r--   0 runner     (501) staff       (20)     1116 2022-04-29 20:48:11.000000 scalene-1.5.8/test/testtf.py
--rw-r--r--   0 runner     (501) staff       (20)      972 2022-04-29 20:48:11.000000 scalene-1.5.8/test/threads-test.py
--rw-r--r--   0 runner     (501) staff       (20)     2736 2022-04-29 20:48:11.000000 scalene-1.5.8/test/torchtest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/
--rw-r--r--   0 runner     (501) staff       (20)       12 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)   265736 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/Alexandrescu-memory-allocation.screen.pdf
--rw-r--r--   0 runner     (501) staff       (20)      155 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/BUILD
--rw-r--r--   0 runner     (501) staff       (20)    11358 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/COPYING
--rw-r--r--   0 runner     (501) staff       (20)     3268 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/NOTICE
--rw-r--r--   0 runner     (501) staff       (20)     3457 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/README.md
--rw-r--r--   0 runner     (501) staff       (20)       26 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/TODO
--rw-r--r--   0 runner     (501) staff       (20)       33 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/WORKSPACE
--rw-r--r--   0 runner     (501) staff       (20)   124113 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/cuj-2005-12.pdf
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/examples/kingsley/
--rwxr-xr-x   0 runner     (501) staff       (20)     1311 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/examples/kingsley/compile
--rw-r--r--   0 runner     (501) staff       (20)     1601 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/examples/kingsley/libkingsley.cpp
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaplayers
--rw-r--r--   0 runner     (501) staff       (20)     2350 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaplayers.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/
--rw-r--r--   0 runner     (501) staff       (20)      664 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/README
--rw-r--r--   0 runner     (501) staff       (20)      247 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/all.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/
--rw-r--r--   0 runner     (501) staff       (20)     1832 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/adaptheap.h
--rw-r--r--   0 runner     (501) staff       (20)      132 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1293 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/boundedfreelistheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2049 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/chunkheap.h
--rw-r--r--   0 runner     (501) staff       (20)     3499 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/coalesceheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1416 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/freelistheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/
--rw-r--r--   0 runner     (501) staff       (20)       94 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1702 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/hybridheap.h
--rw-r--r--   0 runner     (501) staff       (20)     5639 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/segheap.h
--rw-r--r--   0 runner     (501) staff       (20)     3368 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/strictsegheap.h
--rw-r--r--   0 runner     (501) staff       (20)      803 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/combining/tryheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/
--rw-r--r--   0 runner     (501) staff       (20)      123 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1432 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/checkheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1267 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/debugheap.h
--rw-r--r--   0 runner     (501) staff       (20)     5250 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/logheap.h
--rw-r--r--   0 runner     (501) staff       (20)     3368 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/sanitycheckheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2119 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/debug/statsheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/
--rw-r--r--   0 runner     (501) staff       (20)       77 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/all.h
--rw-r--r--   0 runner     (501) staff       (20)     9993 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/dlheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1441 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/kingsleyheap.h
--rwxr-xr-x   0 runner     (501) staff       (20)     1035 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/leamallocheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2448 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/general/oldkingsleyheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/
--rw-r--r--   0 runner     (501) staff       (20)     1328 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/addheap.h
--rw-r--r--   0 runner     (501) staff       (20)      102 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/all.h
--rw-r--r--   0 runner     (501) staff       (20)    10245 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/coalesceableheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1984 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/sizeheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1538 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/sizeownerheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/
--rw-r--r--   0 runner     (501) staff       (20)      186 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/all.h
--rw-r--r--   0 runner     (501) staff       (20)     2543 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/bumpalloc.h
--rw-r--r--   0 runner     (501) staff       (20)     2608 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/nestedheap.h
--rw-r--r--   0 runner     (501) staff       (20)     7993 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstack.h
--rw-r--r--   0 runner     (501) staff       (20)     7826 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstackheap.h
--rwxr-xr-x   0 runner     (501) staff       (20)     7112 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstackreap.h
--rw-r--r--   0 runner     (501) staff       (20)     2893 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/sbrk.c
--rw-r--r--   0 runner     (501) staff       (20)     2720 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/xallocheap.h
--rw-r--r--   0 runner     (501) staff       (20)     3566 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/special/zoneheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/
--rw-r--r--   0 runner     (501) staff       (20)      136 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1605 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/lockedheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2198 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/phothreadheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1099 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/sizethreadheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2041 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/threadheap.h
--rw-r--r--   0 runner     (501) staff       (20)     5054 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/threads/threadspecificheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/
--rw-r--r--   0 runner     (501) staff       (20)      100 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1367 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/mallocheap.h
--rw-r--r--   0 runner     (501) staff       (20)     4808 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/mmapheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2782 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/staticbufferheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1238 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/top/staticheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/
--rw-r--r--   0 runner     (501) staff       (20)      247 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1176 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/exactlyoneheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1203 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/exceptionheap.h
--rw-r--r--   0 runner     (501) staff       (20)      919 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/nullheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/old/
--rw-r--r--   0 runner     (501) staff       (20)     1173 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/old/oneheap.h
--rw-r--r--   0 runner     (501) staff       (20)      807 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/oneheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1691 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/perclassheap.h
--rw-r--r--   0 runner     (501) staff       (20)     1590 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/profileheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2063 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/slopheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2519 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/sysmallocheap.h
--rw-r--r--   0 runner     (501) staff       (20)     4207 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/traceheap.h
--rw-r--r--   0 runner     (501) staff       (20)     2637 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/heaps/utility/uniqueheap.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/
--rw-r--r--   0 runner     (501) staff       (20)      109 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/
--rw-r--r--   0 runner     (501) staff       (20)      759 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/README
--rw-r--r--   0 runner     (501) staff       (20)      984 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/addheader.h
--rw-r--r--   0 runner     (501) staff       (20)     1628 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/clearoptimizeheap.h
--rwxr-xr-x   0 runner     (501) staff       (20)     1315 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/compile
--rw-r--r--   0 runner     (501) staff       (20)     2993 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/libreap.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1059 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/reap.h
--rw-r--r--   0 runner     (501) staff       (20)     3138 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionheap.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5223 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionheap.h
--rw-r--r--   0 runner     (501) staff       (20)      478 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionheapapi.h
--rw-r--r--   0 runner     (501) staff       (20)     4736 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionsimulator.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15487 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionsimulator.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/locks/
--rw-r--r--   0 runner     (501) staff       (20)      115 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/all.h
--rw-r--r--   0 runner     (501) staff       (20)     1413 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/maclock.h
--rw-r--r--   0 runner     (501) staff       (20)     5278 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/oldspinlock.h
--rw-r--r--   0 runner     (501) staff       (20)     1093 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/posixlock.h
--rw-r--r--   0 runner     (501) staff       (20)     1521 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/recursivelock.h
--rw-r--r--   0 runner     (501) staff       (20)     5284 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/spinlock-old.h
--rw-r--r--   0 runner     (501) staff       (20)     2975 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/spinlock.h
--rw-r--r--   0 runner     (501) staff       (20)     1354 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/locks/winlock.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/threads/
--rw-r--r--   0 runner     (501) staff       (20)       39 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/threads/all.h
--rw-r--r--   0 runner     (501) staff       (20)      887 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/threads/cpuinfo.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3824 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/threads/cpuinfo.h
--rw-r--r--   0 runner     (501) staff       (20)     1500 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/threads/fred.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/utility/
--rw-r--r--   0 runner     (501) staff       (20)      614 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/align.h
--rw-r--r--   0 runner     (501) staff       (20)      465 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/all.h
--rw-r--r--   0 runner     (501) staff       (20)     2513 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/bins.h
--rw-r--r--   0 runner     (501) staff       (20)     9253 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/bins16k.h
--rw-r--r--   0 runner     (501) staff       (20)     1422 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/bins4k.h
--rwxr-xr-x   0 runner     (501) staff       (20)     2038 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/bins64k.h
--rw-r--r--   0 runner     (501) staff       (20)     5207 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/bins8k.h
--rw-r--r--   0 runner     (501) staff       (20)     2230 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/binspow2.h
--rw-r--r--   0 runner     (501) staff       (20)      959 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/checkpoweroftwo.h
--rw-r--r--   0 runner     (501) staff       (20)     1920 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/dllist.h
--rw-r--r--   0 runner     (501) staff       (20)     3239 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/dynarray.h
--rw-r--r--   0 runner     (501) staff       (20)      989 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/exactlyone.h
--rw-r--r--   0 runner     (501) staff       (20)     1067 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/freesllist.h
--rw-r--r--   0 runner     (501) staff       (20)      385 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/gcd.h
--rw-r--r--   0 runner     (501) staff       (20)      597 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/hash.h
--rw-r--r--   0 runner     (501) staff       (20)      388 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/ilog2.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1235 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/ilog2.h
--rw-r--r--   0 runner     (501) staff       (20)      614 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/istrue.h
--rw-r--r--   0 runner     (501) staff       (20)      303 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/lcm.h
--rw-r--r--   0 runner     (501) staff       (20)      517 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/modulo.h
--rw-r--r--   0 runner     (501) staff       (20)     2736 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/myhashmap.h
--rw-r--r--   0 runner     (501) staff       (20)      757 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/singleton.h
--rw-r--r--   0 runner     (501) staff       (20)     1675 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/sllist.h
--rw-r--r--   0 runner     (501) staff       (20)      201 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/testalign.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6581 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/timer-old.h
--rw-r--r--   0 runner     (501) staff       (20)     1447 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/timer.h
--rw-r--r--   0 runner     (501) staff       (20)     3026 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/utility/tprintf.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/
--rw-r--r--   0 runner     (501) staff       (20)      102 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/all.h
--rw-r--r--   0 runner     (501) staff       (20)     2664 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/ansiwrapper.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/arch-specific/
--rw-r--r--   0 runner     (501) staff       (20)       80 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/arch-specific/sparc-interchange.il
--rw-r--r--   0 runner     (501) staff       (20)       99 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/arch-specific/x86-interchange.il
--rw-r--r--   0 runner     (501) staff       (20)       78 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/arch-specific/x86_64-interchange.il
--rw-r--r--   0 runner     (501) staff       (20)     1264 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/generic-memalign.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3498 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/gnuwrapper-hooks.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2498 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/gnuwrapper.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8280 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/heapredirect.h
--rw-r--r--   0 runner     (501) staff       (20)      488 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/macinterpose.h
--rw-r--r--   0 runner     (501) staff       (20)    15534 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/macwrapper.cpp
--rw-r--r--   0 runner     (501) staff       (20)      856 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/mallocinfo.h
--rw-r--r--   0 runner     (501) staff       (20)     4658 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/mmapwrapper.h
--rw-r--r--   0 runner     (501) staff       (20)     3397 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/stlallocator.h
--rwxr-xr-x   0 runner     (501) staff       (20)    17068 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/winwrapper.cpp
--rw-r--r--   0 runner     (501) staff       (20)    13729 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/wrapper.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1865 2022-04-29 20:48:43.000000 scalene-1.5.8/vendor/Heap-Layers/wrappers/x86jump.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/printf/
--rw-r--r--   0 runner     (501) staff       (20)       46 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/.gitattributes
--rw-r--r--   0 runner     (501) staff       (20)     1543 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/.travis.yml
--rw-r--r--   0 runner     (501) staff       (20)     1080 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    11003 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/Makefile
--rw-r--r--   0 runner     (501) staff       (20)    11680 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/README.md
--rw-r--r--   0 runner     (501) staff       (20)       47 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/codecov.yml
--rw-r--r--   0 runner     (501) staff       (20)    28047 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/printf.c
--rw-r--r--   0 runner     (501) staff       (20)    28047 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/printf.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4984 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/printf.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-04-29 20:48:53.000000 scalene-1.5.8/vendor/printf/test/
--rw-r--r--   0 runner     (501) staff       (20)   517035 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/test/catch.hpp
--rw-r--r--   0 runner     (501) staff       (20)    43044 2022-04-29 20:48:44.000000 scalene-1.5.8/vendor/printf/test/test_suite.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/.github/
+-rw-r--r--   0 runner     (501) staff       (20)       83 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner     (501) staff       (20)      665 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner     (501) staff       (20)      595 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     4044 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/workflows/build-and-upload.yml
+-rw-r--r--   0 runner     (501) staff       (20)      233 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/workflows/test-homebrew-install.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1348 2022-07-24 23:29:23.000000 scalene-1.5.9/.github/workflows/test-smoketests.yml
+-rw-r--r--   0 runner     (501) staff       (20)     2387 2022-07-24 23:29:23.000000 scalene-1.5.9/.gitignore
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/.vscode/
+-rw-r--r--   0 runner     (501) staff       (20)      735 2022-07-24 23:29:23.000000 scalene-1.5.9/.vscode/c_cpp_properties.json
+-rw-r--r--   0 runner     (501) staff       (20)     3354 2022-07-24 23:29:23.000000 scalene-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner     (501) staff       (20)     3134 2022-07-24 23:29:23.000000 scalene-1.5.9/GNUmakefile
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2022-07-24 23:29:23.000000 scalene-1.5.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      100 2022-07-24 23:29:23.000000 scalene-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1326 2022-07-24 23:29:23.000000 scalene-1.5.9/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)    17781 2022-07-24 23:30:01.000000 scalene-1.5.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      201 2022-07-24 23:29:23.000000 scalene-1.5.9/Pipfile
+-rw-r--r--   0 runner     (501) staff       (20)    10474 2022-07-24 23:29:23.000000 scalene-1.5.9/Pipfile.lock
+-rwxr-xr-x   0 runner     (501) staff       (20)    16494 2022-07-24 23:29:23.000000 scalene-1.5.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/benchmarks/
+-rw-r--r--   0 runner     (501) staff       (20)     8083 2022-07-24 23:29:23.000000 scalene-1.5.9/benchmarks/benchmark.py
+-rw-r--r--   0 runner     (501) staff       (20)     2797 2022-07-24 23:29:23.000000 scalene-1.5.9/benchmarks/julia1_nopil.py
+-rw-r--r--   0 runner     (501) staff       (20)     7444 2022-07-24 23:29:23.000000 scalene-1.5.9/benchmarks/pystone.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/docs/
+-rw-r--r--   0 runner     (501) staff       (20)   307193 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/Ozsvald-tweet.png
+-rwxr-xr-x   0 runner     (501) staff       (20)     9898 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/README_CN.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/docs/images/
+-rw-r--r--   0 runner     (501) staff       (20)   244350 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/images/profiler-comparison.png
+-rw-r--r--   0 runner     (501) staff       (20)   300776 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/images/sample-profile-pystone.png
+-rw-r--r--   0 runner     (501) staff       (20)   196143 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/images/scalene-video-img.png
+-rw-r--r--   0 runner     (501) staff       (20)     5441 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/images/slack-logo.png
+-rw-r--r--   0 runner     (501) staff       (20)    27943 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-demo.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)  1086911 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-gui-example-full.png
+-rw-r--r--   0 runner     (501) staff       (20)    93644 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-gui-example.png
+-rw-r--r--   0 runner     (501) staff       (20)   119139 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-image-large.png
+-rw-r--r--   0 runner     (501) staff       (20)   107546 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-image-old.png
+-rw-r--r--   0 runner     (501) staff       (20)   119139 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-image.png
+-rw-r--r--   0 runner     (501) staff       (20)  1354390 2022-07-24 23:29:23.000000 scalene-1.5.9/docs/scalene-paper.pdf
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2022-07-24 23:29:23.000000 scalene-1.5.9/mypy.ini
+-rw-r--r--   0 runner     (501) staff       (20)      149 2022-07-24 23:29:23.000000 scalene-1.5.9/pyrightconfig.json
+-rw-r--r--   0 runner     (501) staff       (20)       29 2022-07-24 23:29:23.000000 scalene-1.5.9/pytest.ini
+-rw-r--r--   0 runner     (501) staff       (20)      150 2022-07-24 23:29:23.000000 scalene-1.5.9/requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene/
+-rw-r--r--   0 runner     (501) staff       (20)     1631 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       56 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      525 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1565 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/adaptive.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene/old/
+-rw-r--r--   0 runner     (501) staff       (20)     5533 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/old/leak_analysis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1130 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/profile.py
+-rw-r--r--   0 runner     (501) staff       (20)      434 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_exit.py
+-rw-r--r--   0 runner     (501) staff       (20)      629 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_fork.py
+-rw-r--r--   0 runner     (501) staff       (20)      375 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_get_context.py
+-rw-r--r--   0 runner     (501) staff       (20)     2126 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_lock.py
+-rw-r--r--   0 runner     (501) staff       (20)     1101 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_mp_lock.py
+-rw-r--r--   0 runner     (501) staff       (20)     1906 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_pjoin.py
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_poll_selector.py
+-rw-r--r--   0 runner     (501) staff       (20)     3805 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_signal_fns.py
+-rw-r--r--   0 runner     (501) staff       (20)     1054 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/replacement_thread_join.py
+-rw-r--r--   0 runner     (501) staff       (20)     2060 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/runningstats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene/scalene-gui/
+-rw-r--r--   0 runner     (501) staff       (20)     1008 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/README.md
+-rw-r--r--   0 runner     (501) staff       (20)   346688 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/example-profile.js
+-rw-r--r--   0 runner     (501) staff       (20)    15086 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/favicon.ico
+-rw-r--r--   0 runner     (501) staff       (20)     3671 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/index.html
+-rw-r--r--   0 runner     (501) staff       (20)     2478 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/prism.css
+-rw-r--r--   0 runner     (501) staff       (20)    64658 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/prism.js
+-rw-r--r--   0 runner     (501) staff       (20)    16012 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/profile.json
+-rw-r--r--   0 runner     (501) staff       (20)     2300 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/profiler.html
+-rw-r--r--   0 runner     (501) staff       (20)      112 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/scalene-demo.js
+-rw-r--r--   0 runner     (501) staff       (20)       13 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/scalene-fetch.js
+-rw-r--r--   0 runner     (501) staff       (20)    23782 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/scalene-gui.js
+-rw-r--r--   0 runner     (501) staff       (20)   119139 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/scalene-image.png
+-rw-r--r--   0 runner     (501) staff       (20)     7784 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/tablesort.js
+-rw-r--r--   0 runner     (501) staff       (20)      755 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-gui/tablesort.number.js
+-rw-r--r--   0 runner     (501) staff       (20)     3547 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene-usage.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2525 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_apple_gpu.py
+-rw-r--r--   0 runner     (501) staff       (20)     1695 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_arguments.py
+-rw-r--r--   0 runner     (501) staff       (20)     1909 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_client_timer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1223 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_funcutils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4328 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_gpu.py
+-rw-r--r--   0 runner     (501) staff       (20)    15420 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_json.py
+-rw-r--r--   0 runner     (501) staff       (20)     1398 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_leak_analysis.py
+-rw-r--r--   0 runner     (501) staff       (20)     3341 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_magics.py
+-rw-r--r--   0 runner     (501) staff       (20)     2457 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_mapfile.py
+-rw-r--r--   0 runner     (501) staff       (20)    26630 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_output.py
+-rw-r--r--   0 runner     (501) staff       (20)    10968 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_parseargs.py
+-rw-r--r--   0 runner     (501) staff       (20)     4087 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_preload.py
+-rw-r--r--   0 runner     (501) staff       (20)    71398 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_profiler.py
+-rw-r--r--   0 runner     (501) staff       (20)     2099 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_signals.py
+-rw-r--r--   0 runner     (501) staff       (20)     1557 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_sigqueue.py
+-rw-r--r--   0 runner     (501) staff       (20)    17419 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_statistics.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/scalene_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/sparkline.py
+-rw-r--r--   0 runner     (501) staff       (20)      342 2022-07-24 23:29:23.000000 scalene-1.5.9/scalene/syntaxline.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    17781 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    10104 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       50 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2022-07-24 23:30:01.000000 scalene-1.5.9/scalene.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-24 23:30:01.000000 scalene-1.5.9/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     6597 2022-07-24 23:29:23.000000 scalene-1.5.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/src/include/
+-rw-r--r--   0 runner     (501) staff       (20)      676 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/common.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1241 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/lowdiscrepancy.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2331 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/mallocrecursionguard.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7652 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/memcpysampler.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      793 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/pyptr.h
+-rw-r--r--   0 runner     (501) staff       (20)      737 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/pywhere.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5181 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/samplefile.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8779 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/sampleheap.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1741 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/sampleinterval.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1794 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/sampler.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2201 2022-07-24 23:29:23.000000 scalene-1.5.9/src/include/scaleneheader.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/src/source/
+-rw-r--r--   0 runner     (501) staff       (20)     2610 2022-07-24 23:29:23.000000 scalene-1.5.9/src/source/get_line_atomic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7332 2022-07-24 23:29:23.000000 scalene-1.5.9/src/source/libscalene.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     8115 2022-07-24 23:29:23.000000 scalene-1.5.9/src/source/pywhere.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/test/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/test/issues/
+-rw-r--r--   0 runner     (501) staff       (20)      111 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue124.py
+-rw-r--r--   0 runner     (501) staff       (20)       67 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue130.py
+-rw-r--r--   0 runner     (501) staff       (20)      188 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue156.py
+-rw-r--r--   0 runner     (501) staff       (20)     1804 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue167.py
+-rw-r--r--   0 runner     (501) staff       (20)      151 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue193.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue256.py
+-rw-r--r--   0 runner     (501) staff       (20)      239 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue266.py
+-rw-r--r--   0 runner     (501) staff       (20)      311 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue31.py
+-rw-r--r--   0 runner     (501) staff       (20)      277 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue379.py
+-rw-r--r--   0 runner     (501) staff       (20)      247 2022-07-24 23:29:23.000000 scalene-1.5.9/test/issues/test-issue74.py
+-rw-r--r--   0 runner     (501) staff       (20)     1539 2022-07-24 23:29:23.000000 scalene-1.5.9/test/multiprocessing_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1181 2022-07-24 23:29:23.000000 scalene-1.5.9/test/new_mp_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/test/optimized/
+-rwxr-xr-x   0 runner     (501) staff       (20)    20545 2022-07-24 23:29:23.000000 scalene-1.5.9/test/optimized/bm_pyflate.py
+-rw-r--r--   0 runner     (501) staff       (20)    12330 2022-07-24 23:29:23.000000 scalene-1.5.9/test/optimized/bm_raytrace.py
+-rw-r--r--   0 runner     (501) staff       (20)     9721 2022-07-24 23:29:23.000000 scalene-1.5.9/test/optimized/bm_richards.py
+-rw-r--r--   0 runner     (501) staff       (20)    10363 2022-07-24 23:29:23.000000 scalene-1.5.9/test/optimized/bm_scimark.py
+-rw-r--r--   0 runner     (501) staff       (20)     1997 2022-07-24 23:29:23.000000 scalene-1.5.9/test/optimized/bm_spectral_norm.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/test/original/
+-rw-r--r--   0 runner     (501) staff       (20)     9396 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_mdp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    20272 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_pyflate.py
+-rw-r--r--   0 runner     (501) staff       (20)    12142 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_raytrace.py
+-rw-r--r--   0 runner     (501) staff       (20)     9629 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_richards.py
+-rw-r--r--   0 runner     (501) staff       (20)    10284 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_scimark.py
+-rw-r--r--   0 runner     (501) staff       (20)     1773 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_spectral_norm.py
+-rw-r--r--   0 runner     (501) staff       (20)     1512 2022-07-24 23:29:23.000000 scalene-1.5.9/test/original/bm_sympy.py
+-rw-r--r--   0 runner     (501) staff       (20)      357 2022-07-24 23:29:23.000000 scalene-1.5.9/test/pool-test.py
+-rw-r--r--   0 runner     (501) staff       (20)      400 2022-07-24 23:29:23.000000 scalene-1.5.9/test/small_mp_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test-martinheinz.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test-memory.py
+-rw-r--r--   0 runner     (501) staff       (20)     1418 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test-pprofile.py
+-rw-r--r--   0 runner     (501) staff       (20)     2145 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test-size.py
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test_sparkline.py
+-rw-r--r--   0 runner     (501) staff       (20)      354 2022-07-24 23:29:23.000000 scalene-1.5.9/test/test_timers.py
+-rw-r--r--   0 runner     (501) staff       (20)      171 2022-07-24 23:29:23.000000 scalene-1.5.9/test/testflask-driver.py
+-rw-r--r--   0 runner     (501) staff       (20)      248 2022-07-24 23:29:23.000000 scalene-1.5.9/test/testflask.py
+-rw-r--r--   0 runner     (501) staff       (20)     1207 2022-07-24 23:29:23.000000 scalene-1.5.9/test/testme.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2022-07-24 23:29:23.000000 scalene-1.5.9/test/testpyt.py
+-rw-r--r--   0 runner     (501) staff       (20)     1116 2022-07-24 23:29:23.000000 scalene-1.5.9/test/testtf.py
+-rw-r--r--   0 runner     (501) staff       (20)      972 2022-07-24 23:29:23.000000 scalene-1.5.9/test/threads-test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2736 2022-07-24 23:29:23.000000 scalene-1.5.9/test/torchtest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/
+-rw-r--r--   0 runner     (501) staff       (20)       12 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)   265736 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/Alexandrescu-memory-allocation.screen.pdf
+-rw-r--r--   0 runner     (501) staff       (20)      155 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/BUILD
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/COPYING
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/NOTICE
+-rw-r--r--   0 runner     (501) staff       (20)     3457 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       26 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/TODO
+-rw-r--r--   0 runner     (501) staff       (20)       33 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/WORKSPACE
+-rw-r--r--   0 runner     (501) staff       (20)   124113 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/cuj-2005-12.pdf
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/examples/kingsley/
+-rwxr-xr-x   0 runner     (501) staff       (20)     1311 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/examples/kingsley/compile
+-rw-r--r--   0 runner     (501) staff       (20)     1601 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/examples/kingsley/libkingsley.cpp
+-rw-r--r--   0 runner     (501) staff       (20)       24 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaplayers
+-rw-r--r--   0 runner     (501) staff       (20)     2350 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaplayers.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/
+-rw-r--r--   0 runner     (501) staff       (20)      664 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/README
+-rw-r--r--   0 runner     (501) staff       (20)      247 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/all.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/
+-rw-r--r--   0 runner     (501) staff       (20)     1832 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/adaptheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      132 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1293 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/boundedfreelistheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/chunkheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     3499 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/coalesceheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1416 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/freelistheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/
+-rw-r--r--   0 runner     (501) staff       (20)       94 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1702 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/hybridheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     5639 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/segheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     3368 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/strictsegheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      803 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/combining/tryheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/
+-rw-r--r--   0 runner     (501) staff       (20)      123 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1432 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/checkheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1267 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/debugheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     5250 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/logheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     3368 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/sanitycheckheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2119 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/debug/statsheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/
+-rw-r--r--   0 runner     (501) staff       (20)       77 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     9993 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/dlheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1441 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/kingsleyheap.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     1035 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/leamallocheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2448 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/general/oldkingsleyheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/
+-rw-r--r--   0 runner     (501) staff       (20)     1328 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/addheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      102 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/all.h
+-rw-r--r--   0 runner     (501) staff       (20)    10245 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/coalesceableheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/sizeheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1538 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/sizeownerheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/
+-rw-r--r--   0 runner     (501) staff       (20)      186 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     2543 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/bumpalloc.h
+-rw-r--r--   0 runner     (501) staff       (20)     2608 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/nestedheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     7993 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstack.h
+-rw-r--r--   0 runner     (501) staff       (20)     7826 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstackheap.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     7112 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstackreap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2893 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/sbrk.c
+-rw-r--r--   0 runner     (501) staff       (20)     2720 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/xallocheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     3566 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/special/zoneheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/
+-rw-r--r--   0 runner     (501) staff       (20)      136 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1605 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/lockedheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/phothreadheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1099 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/sizethreadheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2041 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/threadheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     5054 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/threads/threadspecificheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/
+-rw-r--r--   0 runner     (501) staff       (20)      100 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1367 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/mallocheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     4808 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/mmapheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2782 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/staticbufferheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1238 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/top/staticheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/
+-rw-r--r--   0 runner     (501) staff       (20)      247 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1176 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/exactlyoneheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1203 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/exceptionheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      919 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/nullheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/old/
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/old/oneheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      807 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/oneheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1691 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/perclassheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/profileheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2063 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/slopheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2519 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/sysmallocheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     4207 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/traceheap.h
+-rw-r--r--   0 runner     (501) staff       (20)     2637 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/heaps/utility/uniqueheap.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/
+-rw-r--r--   0 runner     (501) staff       (20)      109 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/
+-rw-r--r--   0 runner     (501) staff       (20)      759 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/README
+-rw-r--r--   0 runner     (501) staff       (20)      984 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/addheader.h
+-rw-r--r--   0 runner     (501) staff       (20)     1628 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/clearoptimizeheap.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     1315 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/compile
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/libreap.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1059 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/reap.h
+-rw-r--r--   0 runner     (501) staff       (20)     3138 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionheap.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5223 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionheap.h
+-rw-r--r--   0 runner     (501) staff       (20)      478 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionheapapi.h
+-rw-r--r--   0 runner     (501) staff       (20)     4736 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionsimulator.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15487 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionsimulator.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/locks/
+-rw-r--r--   0 runner     (501) staff       (20)      115 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     1413 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/maclock.h
+-rw-r--r--   0 runner     (501) staff       (20)     5278 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/oldspinlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     1093 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/posixlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     1521 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/recursivelock.h
+-rw-r--r--   0 runner     (501) staff       (20)     5284 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/spinlock-old.h
+-rw-r--r--   0 runner     (501) staff       (20)     2975 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/spinlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     1354 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/locks/winlock.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/threads/
+-rw-r--r--   0 runner     (501) staff       (20)       39 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/threads/all.h
+-rw-r--r--   0 runner     (501) staff       (20)      887 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/threads/cpuinfo.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3824 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/threads/cpuinfo.h
+-rw-r--r--   0 runner     (501) staff       (20)     1500 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/threads/fred.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/utility/
+-rw-r--r--   0 runner     (501) staff       (20)      614 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/align.h
+-rw-r--r--   0 runner     (501) staff       (20)      465 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     2513 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/bins.h
+-rw-r--r--   0 runner     (501) staff       (20)     9253 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/bins16k.h
+-rw-r--r--   0 runner     (501) staff       (20)     1422 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/bins4k.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     2038 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/bins64k.h
+-rw-r--r--   0 runner     (501) staff       (20)     5207 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/bins8k.h
+-rw-r--r--   0 runner     (501) staff       (20)     2230 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/binspow2.h
+-rw-r--r--   0 runner     (501) staff       (20)      959 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/checkpoweroftwo.h
+-rw-r--r--   0 runner     (501) staff       (20)     1920 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/dllist.h
+-rw-r--r--   0 runner     (501) staff       (20)     3239 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/dynarray.h
+-rw-r--r--   0 runner     (501) staff       (20)      989 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/exactlyone.h
+-rw-r--r--   0 runner     (501) staff       (20)     1067 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/freesllist.h
+-rw-r--r--   0 runner     (501) staff       (20)      385 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/gcd.h
+-rw-r--r--   0 runner     (501) staff       (20)      597 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/hash.h
+-rw-r--r--   0 runner     (501) staff       (20)      388 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/ilog2.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1235 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/ilog2.h
+-rw-r--r--   0 runner     (501) staff       (20)      614 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/istrue.h
+-rw-r--r--   0 runner     (501) staff       (20)      303 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/lcm.h
+-rw-r--r--   0 runner     (501) staff       (20)      517 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/modulo.h
+-rw-r--r--   0 runner     (501) staff       (20)     2736 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/myhashmap.h
+-rw-r--r--   0 runner     (501) staff       (20)      757 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/singleton.h
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/sllist.h
+-rw-r--r--   0 runner     (501) staff       (20)      201 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/testalign.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/timer-old.h
+-rw-r--r--   0 runner     (501) staff       (20)     1447 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/timer.h
+-rw-r--r--   0 runner     (501) staff       (20)     3026 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/utility/tprintf.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/
+-rw-r--r--   0 runner     (501) staff       (20)      102 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/all.h
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/ansiwrapper.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/arch-specific/
+-rw-r--r--   0 runner     (501) staff       (20)       80 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/arch-specific/sparc-interchange.il
+-rw-r--r--   0 runner     (501) staff       (20)       99 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/arch-specific/x86-interchange.il
+-rw-r--r--   0 runner     (501) staff       (20)       78 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/arch-specific/x86_64-interchange.il
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/generic-memalign.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3498 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/gnuwrapper-hooks.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2498 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/gnuwrapper.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     8280 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/heapredirect.h
+-rw-r--r--   0 runner     (501) staff       (20)      488 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/macinterpose.h
+-rw-r--r--   0 runner     (501) staff       (20)    15534 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/macwrapper.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      856 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/mallocinfo.h
+-rw-r--r--   0 runner     (501) staff       (20)     4658 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/mmapwrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     3397 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/stlallocator.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    17068 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/winwrapper.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    13729 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/wrapper.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1865 2022-07-24 23:29:55.000000 scalene-1.5.9/vendor/Heap-Layers/wrappers/x86jump.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/printf/
+-rw-r--r--   0 runner     (501) staff       (20)       46 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/.gitattributes
+-rw-r--r--   0 runner     (501) staff       (20)     1543 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/.travis.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    11003 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)    11680 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       47 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/codecov.yml
+-rw-r--r--   0 runner     (501) staff       (20)    28047 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/printf.c
+-rw-r--r--   0 runner     (501) staff       (20)    28047 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/printf.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4984 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/printf.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-24 23:30:01.000000 scalene-1.5.9/vendor/printf/test/
+-rw-r--r--   0 runner     (501) staff       (20)   517035 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/test/catch.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    43044 2022-07-24 23:29:56.000000 scalene-1.5.9/vendor/printf/test/test_suite.cpp
```

### Comparing `scalene-1.5.8/.github/ISSUE_TEMPLATE/bug_report.md` & `scalene-1.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/.github/ISSUE_TEMPLATE/feature_request.md` & `scalene-1.5.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/.github/workflows/build-and-upload.yml` & `scalene-1.5.9/.github/workflows/build-and-upload.yml`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/.github/workflows/test-smoketests.yml` & `scalene-1.5.9/.github/workflows/test-smoketests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
       if: matrix.os == 'macos-latest'
       run: sudo rm -Rf /Library/Developer/CommandLineTools/SDKs/*
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r requirements.txt
+        python -m pip install numpy
 
     - name: Build scalene
       run: pip install -e .
 
     - name: cpu-only smoke test
       run: python -m scalene --cli --cpu-only test/testme.py
```

### Comparing `scalene-1.5.8/.gitignore` & `scalene-1.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/.vscode/c_cpp_properties.json` & `scalene-1.5.9/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/CODE_OF_CONDUCT.md` & `scalene-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/GNUmakefile` & `scalene-1.5.9/GNUmakefile`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/LICENSE` & `scalene-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/Makefile` & `scalene-1.5.9/Makefile`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/PKG-INFO` & `scalene-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: scalene
-Version: 1.5.8
+Version: 1.5.9
 Summary: Scalene: A high-resolution, low-overhead CPU, GPU, and memory profiler for Python
 Home-page: https://github.com/plasma-umass/scalene
 Author: Emery Berger
 Author-email: emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: performance memory profiler
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![scalene](https://github.com/plasma-umass/scalene/raw/master/docs/scalene-image.png)
 
 # Scalene: a high-performance CPU, GPU and memory profiler for Python
 
 by [Emery Berger](https://emeryberger.com), [Sam Stern](https://samstern.me/), and [Juan Altmayer Pizzorno](https://github.com/jaltmayerpizzorno).
 
-[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
+[![Scalene community Slack](https://github.com/plasma-umass/scalene/raw/master/docs/images/slack-logo.png)](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/scalene.svg)](https://pypi.org/project/scalene/)[![Downloads](https://pepy.tech/badge/scalene)](https://pepy.tech/project/scalene) [![Downloads](https://pepy.tech/badge/scalene/month)](https://pepy.tech/project/scalene) ![Python versions](https://img.shields.io/pypi/pyversions/scalene.svg?style=flat-square) ![License](https://img.shields.io/github/license/plasma-umass/scalene) [![Twitter Follow](https://img.shields.io/twitter/follow/emeryberger.svg?style=social)](https://twitter.com/emeryberger)
 
 ![Ozsvald tweet](https://github.com/plasma-umass/scalene/raw/master/docs/Ozsvald-tweet.png)
 
 (tweet from Ian Ozsvald, author of [_High Performance Python_](https://smile.amazon.com/High-Performance-Python-Performant-Programming/dp/1492055026/ref=sr_1_1?crid=texbooks))
 
@@ -69,15 +69,16 @@
 
 ```console
 scalene your_prog.py                             # full profile (outputs to web interface)
 python3 -m scalene your_prog.py                  # equivalent alternative
 scalene --cli your_prog.py                       # use the command-line only (no web interface)
 scalene --cpu-only your_prog.py                  # only CPU/GPU
 scalene --reduced-profile your_prog.py           # only profile lines with significant usage
-scalene --profile-interval 5.0 your_prog.py.     # output a new profile every five seconds
+scalene --profile-interval 5.0 your_prog.py      # output a new profile every five seconds
+scalene (Scalene options) --- your_prog.py (...) # use --- to tell Scalene to ignore options after that point
 scalene --help                                   # lists all options
 ```
 
 To use Scalene programmatically in your code, invoke using `scalene` as above and then:
 
 ```Python
 from scalene import scalene_profiler
@@ -364,9 +365,7 @@
 Logo created by [Sophia Berger](https://www.linkedin.com/in/sophia-berger/).
 
 This material is based upon work supported by the National Science
 Foundation under Grant No. 1955610. Any opinions, findings, and
 conclusions or recommendations expressed in this material are those of
 the author(s) and do not necessarily reflect the views of the National
 Science Foundation.
-
-
```

### Comparing `scalene-1.5.8/Pipfile.lock` & `scalene-1.5.9/Pipfile.lock`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9225063131313131%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9f757d0137b9d6c220f7ef249204dfc801fcacf88760f96946131e434817f9ab'}}",*

 * * "'default'": "{'colorama': {'hashes': "*

 * *              "['sha256:854bf444933e37f5824ae7bfc1e98d5bce2ebe4160d46b5edf346a89358e99da', "*

 * *              "'sha256:e6c6b4334fc50988a639d9b98aa429a0b57da6e17b9a44f0451f930b6967b7a4'], "*

 * *              "'version': '==0.4.5'}, 'numpy': {'hashes': "*

 * *              "['sha256:0cfe07133fd00b27edee5e6385e333e9eeb010607e8a46e1cd673f05f8596595', "*

 * *              […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "facb292603f47d58ce68162d9019e5d311bc8431890bf4c3734c8438379bdfb0"
+            "sha256": "9f757d0137b9d6c220f7ef249204dfc801fcacf88760f96946131e434817f9ab"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -20,68 +20,70 @@
                 "sha256:9bc994f9e9447593bd0a45371f0e7ac7333710fcf64a4eb9834bf149f4ef2f32"
             ],
             "index": "pypi",
             "version": "==1.6.0"
         },
         "colorama": {
             "hashes": [
-                "sha256:5941b2b48a20143d2267e95b1c2a7603ce057ee39fd88e7329b0c292aa16869b",
-                "sha256:9f47eda37229f68eee03b24b9748937c7dc3868f906e8ba69fbcbdd3bc5dc3e2"
+                "sha256:854bf444933e37f5824ae7bfc1e98d5bce2ebe4160d46b5edf346a89358e99da",
+                "sha256:e6c6b4334fc50988a639d9b98aa429a0b57da6e17b9a44f0451f930b6967b7a4"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==0.4.4"
+            "version": "==0.4.5"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "numpy": {
             "hashes": [
-                "sha256:1a784e8ff7ea2a32e393cc53eb0003eca1597c7ca628227e34ce34eb11645a0e",
-                "sha256:2ba579dde0563f47021dcd652253103d6fd66165b18011dce1a0609215b2791e",
-                "sha256:3537b967b350ad17633b35c2f4b1a1bbd258c018910b518c30b48c8e41272717",
-                "sha256:3c40e6b860220ed862e8097b8f81c9af6d7405b723f4a7af24a267b46f90e461",
-                "sha256:598fe100b2948465cf3ed64b1a326424b5e4be2670552066e17dfaa67246011d",
-                "sha256:620732f42259eb2c4642761bd324462a01cdd13dd111740ce3d344992dd8492f",
-                "sha256:709884863def34d72b183d074d8ba5cfe042bc3ff8898f1ffad0209161caaa99",
-                "sha256:75579acbadbf74e3afd1153da6177f846212ea2a0cc77de53523ae02c9256513",
-                "sha256:7c55407f739f0bfcec67d0df49103f9333edc870061358ac8a8c9e37ea02fcd2",
-                "sha256:a1f2fb2da242568af0271455b89aee0f71e4e032086ee2b4c5098945d0e11cf6",
-                "sha256:a290989cd671cd0605e9c91a70e6df660f73ae87484218e8285c6522d29f6e38",
-                "sha256:ac4fd578322842dbda8d968e3962e9f22e862b6ec6e3378e7415625915e2da4d",
-                "sha256:ad09f55cc95ed8d80d8ab2052f78cc21cb231764de73e229140d81ff49d8145e",
-                "sha256:b9205711e5440954f861ceeea8f1b415d7dd15214add2e878b4d1cf2bcb1a914",
-                "sha256:bba474a87496d96e61461f7306fba2ebba127bed7836212c360f144d1e72ac54",
-                "sha256:bebab3eaf0641bba26039fb0b2c5bf9b99407924b53b1ea86e03c32c64ef5aef",
-                "sha256:cc367c86eb87e5b7c9592935620f22d13b090c609f1b27e49600cd033b529f54",
-                "sha256:ccc6c650f8700ce1e3a77668bb7c43e45c20ac06ae00d22bdf6760b38958c883",
-                "sha256:cf680682ad0a3bef56dae200dbcbac2d57294a73e5b0f9864955e7dd7c2c2491",
-                "sha256:d2910d0a075caed95de1a605df00ee03b599de5419d0b95d55342e9a33ad1fb3",
-                "sha256:d5caa946a9f55511e76446e170bdad1d12d6b54e17a2afe7b189112ed4412bb8",
-                "sha256:d89b0dc7f005090e32bb4f9bf796e1dcca6b52243caf1803fdd2b748d8561f63",
-                "sha256:d95d16204cd51ff1a1c8d5f9958ce90ae190be81d348b514f9be39f878b8044a",
-                "sha256:e4d5a86a5257843a18fb1220c5f1c199532bc5d24e849ed4b0289fb59fbd4d8f",
-                "sha256:e58ddb53a7b4959932f5582ac455ff90dcb05fac3f8dcc8079498d43afbbde6c",
-                "sha256:e80fe25cba41c124d04c662f33f6364909b985f2eb5998aaa5ae4b9587242cce",
-                "sha256:eda2829af498946c59d8585a9fd74da3f810866e05f8df03a86f70079c7531dd",
-                "sha256:fd0a359c1c17f00cb37de2969984a74320970e0ceef4808c32e00773b06649d9"
+                "sha256:0cfe07133fd00b27edee5e6385e333e9eeb010607e8a46e1cd673f05f8596595",
+                "sha256:11a1f3816ea82eed4178102c56281782690ab5993251fdfd75039aad4d20385f",
+                "sha256:2762331de395739c91f1abb88041f94a080cb1143aeec791b3b223976228af3f",
+                "sha256:283d9de87c0133ef98f93dfc09fad3fb382f2a15580de75c02b5bb36a5a159a5",
+                "sha256:3d22662b4b10112c545c91a0741f2436f8ca979ab3d69d03d19322aa970f9695",
+                "sha256:41388e32e40b41dd56eb37fcaa7488b2b47b0adf77c66154d6b89622c110dfe9",
+                "sha256:42c16cec1c8cf2728f1d539bd55aaa9d6bb48a7de2f41eb944697293ef65a559",
+                "sha256:47ee7a839f5885bc0c63a74aabb91f6f40d7d7b639253768c4199b37aede7982",
+                "sha256:5a311ee4d983c487a0ab546708edbdd759393a3dc9cd30305170149fedd23c88",
+                "sha256:5dc65644f75a4c2970f21394ad8bea1a844104f0fe01f278631be1c7eae27226",
+                "sha256:6ed0d073a9c54ac40c41a9c2d53fcc3d4d4ed607670b9e7b0de1ba13b4cbfe6f",
+                "sha256:76ba7c40e80f9dc815c5e896330700fd6e20814e69da9c1267d65a4d051080f1",
+                "sha256:818b9be7900e8dc23e013a92779135623476f44a0de58b40c32a15368c01d471",
+                "sha256:a024181d7aef0004d76fb3bce2a4c9f2e67a609a9e2a6ff2571d30e9976aa383",
+                "sha256:a955e4128ac36797aaffd49ab44ec74a71c11d6938df83b1285492d277db5397",
+                "sha256:a97a954a8c2f046d3817c2bce16e3c7e9a9c2afffaf0400f5c16df5172a67c9c",
+                "sha256:a97e82c39d9856fe7d4f9b86d8a1e66eff99cf3a8b7ba48202f659703d27c46f",
+                "sha256:b55b953a1bdb465f4dc181758570d321db4ac23005f90ffd2b434cc6609a63dd",
+                "sha256:bb02929b0d6bfab4c48a79bd805bd7419114606947ec8284476167415171f55b",
+                "sha256:bece0a4a49e60e472a6d1f70ac6cdea00f9ab80ff01132f96bd970cdd8a9e5a9",
+                "sha256:e41e8951749c4b5c9a2dc5fdbc1a4eec6ab2a140fdae9b460b0f557eed870f4d",
+                "sha256:f71d57cc8645f14816ae249407d309be250ad8de93ef61d9709b45a0ddf4050c"
             ],
             "index": "pypi",
-            "version": "==1.21.0"
+            "version": "==1.22.0"
+        },
+        "nvidia-ml-py": {
+            "hashes": [
+                "sha256:88d2d0bbd73c43707e15730e6d14edc6a13707fb222489489421fa4f4ad7fac6",
+                "sha256:d4784ab4de877dc93627ea6c07c649dddd8600ac8dcb28fd379e4dcde89c7fb1"
+            ],
+            "index": "pypi",
+            "version": "==11.515.48"
         },
         "pygments": {
             "hashes": [
-                "sha256:44238f1b60a76d78fc8ca0528ee429702aae011c265fe6a8dd8b63049ae41c65",
-                "sha256:4e426f72023d88d03b2fa258de560726ce890ff3b630f88c21cbb8b2503b8c6a"
+                "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb",
+                "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.11.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.12.0"
         },
         "rich": {
             "hashes": [
                 "sha256:3070d53e3a93864de351c1091af1deb25f41e6051b33e485d4626b591c0cfdb3",
                 "sha256:e0f2db62a52536ee32f6f584a47536465872cae2b94887cf1f080fb9eaa13eb2"
             ],
             "index": "pypi",
@@ -108,14 +110,42 @@
         "iniconfig": {
             "hashes": [
                 "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3",
                 "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"
             ],
             "version": "==1.1.1"
         },
+        "numpy": {
+            "hashes": [
+                "sha256:0cfe07133fd00b27edee5e6385e333e9eeb010607e8a46e1cd673f05f8596595",
+                "sha256:11a1f3816ea82eed4178102c56281782690ab5993251fdfd75039aad4d20385f",
+                "sha256:2762331de395739c91f1abb88041f94a080cb1143aeec791b3b223976228af3f",
+                "sha256:283d9de87c0133ef98f93dfc09fad3fb382f2a15580de75c02b5bb36a5a159a5",
+                "sha256:3d22662b4b10112c545c91a0741f2436f8ca979ab3d69d03d19322aa970f9695",
+                "sha256:41388e32e40b41dd56eb37fcaa7488b2b47b0adf77c66154d6b89622c110dfe9",
+                "sha256:42c16cec1c8cf2728f1d539bd55aaa9d6bb48a7de2f41eb944697293ef65a559",
+                "sha256:47ee7a839f5885bc0c63a74aabb91f6f40d7d7b639253768c4199b37aede7982",
+                "sha256:5a311ee4d983c487a0ab546708edbdd759393a3dc9cd30305170149fedd23c88",
+                "sha256:5dc65644f75a4c2970f21394ad8bea1a844104f0fe01f278631be1c7eae27226",
+                "sha256:6ed0d073a9c54ac40c41a9c2d53fcc3d4d4ed607670b9e7b0de1ba13b4cbfe6f",
+                "sha256:76ba7c40e80f9dc815c5e896330700fd6e20814e69da9c1267d65a4d051080f1",
+                "sha256:818b9be7900e8dc23e013a92779135623476f44a0de58b40c32a15368c01d471",
+                "sha256:a024181d7aef0004d76fb3bce2a4c9f2e67a609a9e2a6ff2571d30e9976aa383",
+                "sha256:a955e4128ac36797aaffd49ab44ec74a71c11d6938df83b1285492d277db5397",
+                "sha256:a97a954a8c2f046d3817c2bce16e3c7e9a9c2afffaf0400f5c16df5172a67c9c",
+                "sha256:a97e82c39d9856fe7d4f9b86d8a1e66eff99cf3a8b7ba48202f659703d27c46f",
+                "sha256:b55b953a1bdb465f4dc181758570d321db4ac23005f90ffd2b434cc6609a63dd",
+                "sha256:bb02929b0d6bfab4c48a79bd805bd7419114606947ec8284476167415171f55b",
+                "sha256:bece0a4a49e60e472a6d1f70ac6cdea00f9ab80ff01132f96bd970cdd8a9e5a9",
+                "sha256:e41e8951749c4b5c9a2dc5fdbc1a4eec6ab2a140fdae9b460b0f557eed870f4d",
+                "sha256:f71d57cc8645f14816ae249407d309be250ad8de93ef61d9709b45a0ddf4050c"
+            ],
+            "index": "pypi",
+            "version": "==1.22.0"
+        },
         "packaging": {
             "hashes": [
                 "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
                 "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.3"
@@ -134,19 +164,19 @@
                 "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==1.11.0"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:04ff808a5b90911829c55c4e26f75fa5ca8a2f5f36aa3a51f68e27033341d3e4",
-                "sha256:d9bdec0013ef1eb5a84ab39a3b3868911598afa494f5faa038647101504e2b81"
+                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
+                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.6"
+            "markers": "python_full_version >= '3.6.8'",
+            "version": "==3.0.9"
         },
         "pyperf": {
             "hashes": [
                 "sha256:1257d673d89fdcdbaec8077afeb365e7a94739c1b263572b09403cac25708ad3",
                 "sha256:ca7f13c922e6a16ce2d69ac86b243c8faf5183da5b346eb064385e0de4d8c18d"
             ],
             "index": "pypi",
@@ -163,10 +193,18 @@
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==0.10.2"
+        },
+        "wheel": {
+            "hashes": [
+                "sha256:4bdcd7d840138086126cd09254dc6195fb4fc6f01c050a1d7236f2630db1d22a",
+                "sha256:e9a504e793efbca1b8e0e9cb979a249cf4a0a7b5b8c9e8b65a5e39d49529c1c4"
+            ],
+            "index": "pypi",
+            "version": "==0.37.1"
         }
     }
 }
```

### Comparing `scalene-1.5.8/README.md` & `scalene-1.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![scalene](https://github.com/plasma-umass/scalene/raw/master/docs/scalene-image.png)
 
 # Scalene: a high-performance CPU, GPU and memory profiler for Python
 
 by [Emery Berger](https://emeryberger.com), [Sam Stern](https://samstern.me/), and [Juan Altmayer Pizzorno](https://github.com/jaltmayerpizzorno).
 
-[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
+[![Scalene community Slack](https://github.com/plasma-umass/scalene/raw/master/docs/images/slack-logo.png)](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/scalene.svg)](https://pypi.org/project/scalene/)[![Downloads](https://pepy.tech/badge/scalene)](https://pepy.tech/project/scalene) [![Downloads](https://pepy.tech/badge/scalene/month)](https://pepy.tech/project/scalene) ![Python versions](https://img.shields.io/pypi/pyversions/scalene.svg?style=flat-square) ![License](https://img.shields.io/github/license/plasma-umass/scalene) [![Twitter Follow](https://img.shields.io/twitter/follow/emeryberger.svg?style=social)](https://twitter.com/emeryberger)
 
 ![Ozsvald tweet](https://github.com/plasma-umass/scalene/raw/master/docs/Ozsvald-tweet.png)
 
 (tweet from Ian Ozsvald, author of [_High Performance Python_](https://smile.amazon.com/High-Performance-Python-Performant-Programming/dp/1492055026/ref=sr_1_1?crid=texbooks))
 
@@ -38,15 +38,16 @@
 
 ```console
 scalene your_prog.py                             # full profile (outputs to web interface)
 python3 -m scalene your_prog.py                  # equivalent alternative
 scalene --cli your_prog.py                       # use the command-line only (no web interface)
 scalene --cpu-only your_prog.py                  # only CPU/GPU
 scalene --reduced-profile your_prog.py           # only profile lines with significant usage
-scalene --profile-interval 5.0 your_prog.py.     # output a new profile every five seconds
+scalene --profile-interval 5.0 your_prog.py      # output a new profile every five seconds
+scalene (Scalene options) --- your_prog.py (...) # use --- to tell Scalene to ignore options after that point
 scalene --help                                   # lists all options
 ```
 
 To use Scalene programmatically in your code, invoke using `scalene` as above and then:
 
 ```Python
 from scalene import scalene_profiler
```

### Comparing `scalene-1.5.8/benchmarks/benchmark.py` & `scalene-1.5.9/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/benchmarks/julia1_nopil.py` & `scalene-1.5.9/benchmarks/julia1_nopil.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/benchmarks/pystone.py` & `scalene-1.5.9/benchmarks/pystone.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/Ozsvald-tweet.png` & `scalene-1.5.9/docs/Ozsvald-tweet.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/README_CN.md` & `scalene-1.5.9/docs/README_CN.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/images/profiler-comparison.png` & `scalene-1.5.9/docs/images/profiler-comparison.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/images/sample-profile-pystone.png` & `scalene-1.5.9/docs/images/sample-profile-pystone.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/images/scalene-video-img.png` & `scalene-1.5.9/docs/images/scalene-video-img.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-demo.ipynb` & `scalene-1.5.9/docs/scalene-demo.ipynb`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-gui-example-full.png` & `scalene-1.5.9/docs/scalene-gui-example-full.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-gui-example.png` & `scalene-1.5.9/docs/scalene-gui-example.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-image-large.png` & `scalene-1.5.9/docs/scalene-image-large.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-image-old.png` & `scalene-1.5.9/docs/scalene-image-old.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-image.png` & `scalene-1.5.9/docs/scalene-image.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/docs/scalene-paper.pdf` & `scalene-1.5.9/docs/scalene-paper.pdf`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/mypy.ini` & `scalene-1.5.9/mypy.ini`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/README.md` & `scalene-1.5.9/scalene/README.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/__main__.py` & `scalene-1.5.9/scalene/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 
 def should_trace(s) -> bool:
     if scalene_profiler.Scalene.is_done():
         return False
     return scalene_profiler.Scalene.should_trace(s)
 
+
 def main():
     try:
         from scalene import scalene_profiler
+
         scalene_profiler.Scalene.main()
     except Exception as exc:
         sys.stderr.write("ERROR: Calling scalene main function failed: %s\n" % exc)
         traceback.print_exc()
         sys.exit(1)
```

### Comparing `scalene-1.5.8/scalene/adaptive.py` & `scalene-1.5.9/scalene/adaptive.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/old/leak_analysis.py` & `scalene-1.5.9/scalene/old/leak_analysis.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/profile.py` & `scalene-1.5.9/scalene/profile.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_fork.py` & `scalene-1.5.9/scalene/replacement_fork.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_lock.py` & `scalene-1.5.9/scalene/replacement_lock.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_mp_lock.py` & `scalene-1.5.9/scalene/replacement_mp_lock.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_pjoin.py` & `scalene-1.5.9/scalene/replacement_pjoin.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_poll_selector.py` & `scalene-1.5.9/scalene/replacement_poll_selector.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_signal_fns.py` & `scalene-1.5.9/scalene/replacement_signal_fns.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/replacement_thread_join.py` & `scalene-1.5.9/scalene/replacement_thread_join.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/runningstats.py` & `scalene-1.5.9/scalene/runningstats.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/README.md` & `scalene-1.5.9/scalene/scalene-gui/README.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/example-profile.js` & `scalene-1.5.9/scalene/scalene-gui/example-profile.js`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/favicon.ico` & `scalene-1.5.9/scalene/scalene-gui/favicon.ico`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/index.html` & `scalene-1.5.9/scalene/scalene-gui/index.html`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/prism.css` & `scalene-1.5.9/scalene/scalene-gui/prism.css`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/prism.js` & `scalene-1.5.9/scalene/scalene-gui/prism.js`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/profile.json` & `scalene-1.5.9/scalene/scalene-gui/profile.json`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/profiler.html` & `scalene-1.5.9/scalene/scalene-gui/profiler.html`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/scalene-gui.js` & `scalene-1.5.9/scalene/scalene-gui/scalene-gui.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,50 +13,75 @@
         height: "container",
         padding: 0,
         data: {
             values: [{
                 x: 0,
                 y: python.toFixed(1),
                 c: "(Python) " + python.toFixed(1) + "%",
+                d: python.toFixed(0) + "%",
             }, {
                 x: 0,
                 y: native.toFixed(1),
                 c: "(native) " + native.toFixed(1) + "%",
+                d: native.toFixed(0) + "%",
             }, {
                 x: 0,
                 y: system.toFixed(1),
                 c: "(system) " + system.toFixed(1) + "%",
+                d: system.toFixed(0) + "%",
             }, ],
         },
-        mark: {
-            type: "bar"
-        },
-        encoding: {
-            x: {
-                aggregate: "sum",
-                field: "y",
-                axis: false,
-                scale: {
-                    domain: [0, 100]
+        layer: [{
+                mark: {
+                    type: "bar"
                 },
-            },
-            color: {
-                field: "c",
-                type: "nominal",
-                legend: false,
-                scale: {
-                    range: ["darkblue", "#6495ED", "blue"]
+                encoding: {
+                    x: {
+                        aggregate: "sum",
+                        field: "y",
+                        axis: false,
+                        scale: {
+                            domain: [0, 100]
+                        },
+                    },
+                    color: {
+                        field: "c",
+                        type: "nominal",
+                        legend: false,
+                        scale: {
+                            range: ["darkblue", "#6495ED", "blue"]
+                        },
+                    },
+                    tooltip: [{
+                        field: "c",
+                        type: "nominal",
+                        title: "time"
+                    }],
                 },
             },
-            tooltip: [{
-                field: "c",
-                type: "nominal",
-                title: "time"
-            }],
-        },
+            /*	  ,
+      {
+          mark: {
+              type: "text",
+              opacity: 1.0,
+              color: "white",
+              align: "right",
+              limit: 50,
+          },
+          encoding: {
+              x: { type: "quantitative", field: "y" },
+              text: {
+		  field: "d",
+		  bandPosition: 0.5,
+		  condition: { test: `datum['y'] < 20`, value: "" },
+              },
+          },
+	  },
+	  */
+        ],
     };
 }
 
 function makeGPUPie(util) {
     return {
         $schema: "https://vega.github.io/schema/vega-lite/v5.json",
         config: {
@@ -467,16 +492,18 @@
             )
         );
         s += "</td>";
         s += `<td style='vertical-align: middle; width: 100'><span style="height:25; width: 100; vertical-align: middle" id="memory_sparkline${memory_sparklines.length}"></span>`;
         s += "</td>";
         if (line.memory_samples.length > 0) {
             let leak_velocity = 0;
-            if (line.lineno in prof.files[filename].leaks) {
-                leak_velocity = prof.files[filename].leaks[line.lineno].velocity_mb_s;
+            if ("leaks" in prof.files[filename]) {
+                if (line.lineno in prof.files[filename].leaks) {
+                    leak_velocity = prof.files[filename].leaks[line.lineno].velocity_mb_s;
+                }
             }
             memory_sparklines.push(
                 makeSparkline(
                     line.memory_samples,
                     prof.elapsed_time_sec * 1e9,
                     prof.max_footprint_mb,
                     leak_velocity
```

### Comparing `scalene-1.5.8/scalene/scalene-gui/scalene-image.png` & `scalene-1.5.9/scalene/scalene-gui/scalene-image.png`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/tablesort.js` & `scalene-1.5.9/scalene/scalene-gui/tablesort.js`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-gui/tablesort.number.js` & `scalene-1.5.9/scalene/scalene-gui/tablesort.number.js`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene-usage.txt` & `scalene-1.5.9/scalene/scalene-usage.txt`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_apple_gpu.py` & `scalene-1.5.9/scalene/scalene_apple_gpu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 import platform
+import random
 import re
 import subprocess
 from typing import Tuple
 
 
 class ScaleneAppleGPU:
     """Wrapper class for Apple integrated GPU statistics."""
 
-    def __init__(self) -> None:
+    def __init__(self, sampling_frequency=100) -> None:
         assert platform.system() == "Darwin"
         self.cmd = (
             'DYLD_INSERT_LIBRARIES="" ioreg -r -d 1 -w 0 -c "IOAccelerator"'
         )
         self.regex_util = re.compile(r'"Device Utilization %"=(\d+)')
         self.regex_inuse = re.compile(r'"In use system memory"=(\d+)')
+        # Only actually get stats some fraction of the time, since it is costly.
+        # Used in get_stats().
+        self.gpu_sampling_frequency = sampling_frequency
 
     def has_gpu(self) -> bool:
         """Returns true: as far as I am aware, all Macs have had integrated GPUs for some time."""
         return True
 
     def nvml_reinit(self) -> None:
         """A NOP, here for compatibility with the nvidia wrapper."""
         return
 
     def get_stats(self) -> Tuple[float, float]:
         """Returns a tuple of (utilization%, memory in use)"""
         if not self.has_gpu():
             return (0.0, 0.0)
         try:
+            # Only periodically query the statistics for real (at a
+            # rate of 1/self.gpu_sampling_frequency).  We do this to
+            # amortize its cost, as it is shockingly expensive.
+            if random.randint(0, self.gpu_sampling_frequency - 1) != 0:
+                return (0.0, 0.0)
             in_use = 0.0
             util = 0.0
             read_process = subprocess.Popen(
                 self.cmd, shell=True, stdout=subprocess.PIPE
             )
             if read_process.stdout is not None:
                 read_process_return = read_process.stdout.readlines()
                 for line in read_process_return:
                     decoded_line = line.decode("utf-8")
+                    # print(decoded_line)
                     if "In use system memory" in decoded_line:
                         in_use_re = self.regex_inuse.search(decoded_line)
                         if in_use_re:
                             in_use = float(in_use_re.group(1))
                     if "Device Utilization %" in decoded_line:
                         util_re = self.regex_util.search(decoded_line)
                         if util_re:
```

### Comparing `scalene-1.5.8/scalene/scalene_arguments.py` & `scalene-1.5.9/scalene/scalene_arguments.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_client_timer.py` & `scalene-1.5.9/scalene/scalene_client_timer.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_funcutils.py` & `scalene-1.5.9/scalene/scalene_funcutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     # distinguish between Python and native code execution when
     # running in threads.
     __call_opcodes: FrozenSet[int] = frozenset(
         {
             dis.opmap[op_name]
             for op_name in dis.opmap
             if op_name.startswith("CALL_FUNCTION")
+            or op_name.startswith("CALL_METHOD")
             or (sys.version_info >= (3, 11) and op_name.startswith("CALL"))
         }
     )
 
     @staticmethod
     @lru_cache(maxsize=None)
     def is_call_function(code: CodeType, bytei: ByteCodeIndex) -> bool:
```

### Comparing `scalene-1.5.8/scalene/scalene_json.py` & `scalene-1.5.9/scalene/scalene_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,20 @@
             samples = []
 
         output: Dict[str, Any] = {
             "program": program,
             "elapsed_time_sec": stats.elapsed_time,
             "growth_rate": growth_rate,
             "max_footprint_mb": stats.max_footprint,
+            "max_footprint_fname": stats.max_footprint_loc[0]
+            if stats.max_footprint_loc
+            else None,
+            "max_footprint_lineno": stats.max_footprint_loc[1]
+            if stats.max_footprint_loc
+            else None,
             "files": {},
             "gpu": self.gpu,
             "memory": profile_memory,
             "samples": samples,
         }
 
         # Build a list of files we will actually report on.
```

### Comparing `scalene-1.5.8/scalene/scalene_leak_analysis.py` & `scalene-1.5.9/scalene/scalene_leak_analysis.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_magics.py` & `scalene-1.5.9/scalene/scalene_magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,27 @@
                 args, [filename], is_jupyter=True
             )
 
         @line_cell_magic
         def scalene(self, line: str, cell: str = "") -> None:
             """%%scalene magic: see https://github.com/plasma-umass/scalene for usage info."""
             if line:
-                sys.argv = ["scalene"]
-                sys.argv.extend(line.split(" "))
+                sys.argv = ["scalene", *line.split(" ")]
                 (args, _left) = ScaleneParseArgs.parse_args()
             else:
                 args = ScaleneArguments()
             if cell:
                 self.run_code(args, cell)  # type: ignore
 
         @line_magic
         def scrun(self, line: str = "") -> None:
             """%scrun magic: see https://github.com/plasma-umass/scalene for usage info."""
 
             if line:
-                sys.argv = ["scalene"]
-                sys.argv.extend(line.split(" "))
+                sys.argv = ["scalene", *line.split(" ")]
                 (args, left) = ScaleneParseArgs.parse_args()
                 self.run_code(args, " ".join(left))  # type: ignore
 
     def load_ipython_extension(ip: Any) -> None:
         ip.register_magics(ScaleneMagics)
         with contextlib.suppress(Exception):
             # For some reason, this isn't loading correctly on the web.
```

### Comparing `scalene-1.5.8/scalene/scalene_mapfile.py` & `scalene-1.5.9/scalene/scalene_mapfile.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_output.py` & `scalene-1.5.9/scalene/scalene_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,24 +45,24 @@
         self.gpu = False
 
     # Profile output methods
 
     def output_top_memory(
         self, title: str, console: Console, mallocs: Dict[LineNumber, float]
     ) -> None:
-        # Print the top N lines by memory consumption, as long
-        # as they are above some threshold MB in size.
-        print_top_mallocs_count = 5
-        print_top_mallocs_threshold_mb = 1
-        if len(mallocs) > 0:
+        if mallocs:
             printed_header = False
             number = 1
-            for malloc_lineno in mallocs:
+            # Print the top N lines by memory consumption, as long
+            # as they are above some threshold MB in size.
+            print_top_mallocs_count = 5
+            print_top_mallocs_threshold_mb = 1
+            for malloc_lineno, value in mallocs.items():
                 # Don't print lines with less than the threshold MB allocated.
-                if mallocs[malloc_lineno] <= print_top_mallocs_threshold_mb:
+                if value <= print_top_mallocs_threshold_mb:
                     break
                 # Only print the top N.
                 if number > print_top_mallocs_count:
                     break
                 # Print the header only if we are printing something (and only once).
                 if not printed_header:
                     console.print(title)
@@ -406,35 +406,34 @@
 
         # Don't actually output the profile if we are a child process.
         # Instead, write info to disk for the main process to collect.
         if pid:
             stats.output_stats(pid, python_alias_dir)
             return True
 
-        if len(report_files) == 0:
+        if not report_files:
             return False
 
         for fname in report_files:
 
             # If the file was actually a Jupyter (IPython) cell,
             # restore its name, as in "[12]".
             fname_print = fname
             import re
 
-            result = re.match("<ipython-input-([0-9]+)-.*>", fname_print)
-            if result:
-                fname_print = Filename("[" + result.group(1) + "]")
+            if result := re.match("<ipython-input-([0-9]+)-.*>", fname_print):
+                fname_print = Filename(f"[{result.group(1)}]")
 
             # Print header.
-            if not stats.total_cpu_samples:
-                percent_cpu_time = 0
-            else:
-                percent_cpu_time = (
-                    100 * stats.cpu_samples[fname] / stats.total_cpu_samples
-                )
+            percent_cpu_time = (
+                (100 * stats.cpu_samples[fname] / stats.total_cpu_samples)
+                if stats.total_cpu_samples
+                else 0
+            )
+
             new_title = mem_usage_line + (
                 f"{fname_print}: % of time = {percent_cpu_time:6.2f} out of {stats.elapsed_time:6.2f}."
             )
             # Only display total memory usage once.
             mem_usage_line = ""
 
             tbl = Table(
@@ -503,27 +502,21 @@
                 tbl.add_column(
                     Markdown("Copy  \n_(MB/s)_", style="yellow4"),
                     style="yellow4",
                     no_wrap=True,
                     width=6,
                 )
                 other_columns_width = 75 + (6 if self.gpu else 0)
-                tbl.add_column(
-                    "\n" + fname_print,
-                    width=column_width - other_columns_width,
-                    no_wrap=True,
-                )
             else:
                 other_columns_width = 37 + (5 if self.gpu else 0)
-                tbl.add_column(
-                    "\n" + fname_print,
-                    width=column_width - other_columns_width,
-                    no_wrap=True,
-                )
-
+            tbl.add_column(
+                "\n" + fname_print,
+                width=column_width - other_columns_width,
+                no_wrap=True,
+            )
             # Print out the the profile for the source, line by line.
             if fname == "<BOGUS>":
                 continue
             if not fname:
                 continue
             # Print out the profile for the source, line by line.
             with open(fname, "r", encoding="utf-8") as source_file:
@@ -597,19 +590,18 @@
                     f"function summary for {fname}", style="bold italic"
                 )
                 if profile_memory:
                     if self.gpu:
                         tbl.add_row("", "", "", "", "", "", "", "", "", txt)
                     else:
                         tbl.add_row("", "", "", "", "", "", "", "", txt)
+                elif self.gpu:
+                    tbl.add_row("", "", "", "", "", txt)
                 else:
-                    if self.gpu:
-                        tbl.add_row("", "", "", "", "", txt)
-                    else:
-                        tbl.add_row("", "", "", "", txt)
+                    tbl.add_row("", "", "", "", txt)
 
                 for fn_name in sorted(
                     fn_stats.cpu_samples_python,
                     key=lambda k: stats.firstline_map[k],
                 ):
                     if fn_name == fname:
                         continue
@@ -639,16 +631,15 @@
 
             console.print(tbl)
 
             # Compute AVERAGE memory consumption.
             avg_mallocs: Dict[LineNumber, float] = defaultdict(float)
             for line_no in stats.bytei_map[fname]:
                 n_malloc_mb = stats.memory_aggregate_footprint[fname][line_no]
-                count = stats.memory_malloc_count[fname][line_no]
-                if count:
+                if count := stats.memory_malloc_count[fname][line_no]:
                     avg_mallocs[line_no] = n_malloc_mb / count
                 else:
                     # Setting to n_malloc_mb addresses the edge case where this allocation is the last line executed.
                     avg_mallocs[line_no] = n_malloc_mb
 
             avg_mallocs = OrderedDict(
                 sorted(avg_mallocs.items(), key=itemgetter(1), reverse=True)
@@ -695,15 +686,14 @@
             md = Markdown(
                 "generated by the [scalene](https://github.com/plasma-umass/scalene) profiler"
             )
             console.print(md)
             if not self.output_file:
                 self.output_file = "/dev/stdout"
             console.save_html(self.output_file, clear=False)
+        elif self.output_file:
+            # Don't output styles to text file.
+            console.save_text(self.output_file, styles=False, clear=False)
         else:
-            if not self.output_file:
-                # No output file specified: write to stdout.
-                sys.stdout.write(console.export_text(styles=True))
-            else:
-                # Don't output styles to text file.
-                console.save_text(self.output_file, styles=False, clear=False)
+            # No output file specified: write to stdout.
+            sys.stdout.write(console.export_text(styles=True))
         return True
```

### Comparing `scalene-1.5.8/scalene/scalene_parseargs.py` & `scalene-1.5.9/scalene/scalene_parseargs.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/scalene/scalene_preload.py` & `scalene-1.5.9/scalene/scalene_preload.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,43 +10,41 @@
 
 import scalene
 
 
 class ScalenePreload:
     @staticmethod
     def get_preload_environ(args: argparse.Namespace) -> Dict[str, str]:
-        env = dict()
-
-        # Set allocation sampling window (sync environment variable
-        # name with src/include/sampleheap.hpp).
-        env["SCALENE_ALLOCATION_SAMPLING_WINDOW"] = str(
-            args.allocation_sampling_window
-        )
+        env = {
+            "SCALENE_ALLOCATION_SAMPLING_WINDOW": str(
+                args.allocation_sampling_window
+            )
+        }
 
         # Set environment variables for loading the Scalene dynamic library,
         # which interposes on allocation and copying functions.
-        if sys.platform == "linux":
+        if sys.platform == "darwin":
             if not args.cpu_only:
-                env["LD_PRELOAD"] = os.path.join(
-                    scalene.__path__[0], "libscalene.so"
+                env["DYLD_INSERT_LIBRARIES"] = os.path.join(
+                    scalene.__path__[0].replace(" ", "\ "), "libscalene.dylib"
                 )
                 # Disable command-line specified PYTHONMALLOC.
                 if "PYTHONMALLOC" in env:
                     del env["PYTHONMALLOC"]
+            # required for multiprocessing support, even without libscalene
+            env["OBJC_DISABLE_INITIALIZE_FORK_SAFETY"] = "YES"
 
-        elif sys.platform == "darwin":
+        elif sys.platform == "linux":
             if not args.cpu_only:
-                env["DYLD_INSERT_LIBRARIES"] = os.path.join(
-                    scalene.__path__[0], "libscalene.dylib"
+                env["LD_PRELOAD"] = os.path.join(
+                    scalene.__path__[0].replace(" ", "\ "), "libscalene.so"
                 )
                 # Disable command-line specified PYTHONMALLOC.
                 if "PYTHONMALLOC" in env:
                     del env["PYTHONMALLOC"]
-            # required for multiprocessing support, even without libscalene
-            env["OBJC_DISABLE_INITIALIZE_FORK_SAFETY"] = "YES"
 
         elif sys.platform == "win32":
             # Force CPU only on Windows for now.
             args.cpu_only = True
 
         return env
 
@@ -57,21 +55,16 @@
         as well as any other required environment variables.
         Returns true iff we had to run another process.
         """
 
         # First, check that we are on a supported platform.
         # (x86-64 and ARM only for now.)
         if not args.cpu_only and (
-            (
-                platform.machine() != "x86_64"
-                and platform.machine() != "AMD64"
-                and platform.machine() != "arm64"
-                and platform.machine() != "aarch64"
-            )
-            or struct.calcsize("P") * 8 != 64
+            platform.machine() not in ["x86_64", "AMD64", "arm64", "aarch64"]
+            or struct.calcsize("P") != 8
         ):
             args.cpu_only = True
             print(
                 "Scalene warning: currently only 64-bit x86-64 and ARM platforms are supported for memory and copy profiling."
             )
 
         with contextlib.suppress(Exception):
@@ -80,17 +73,16 @@
             if get_ipython():
                 sys.exit = Scalene.clean_exit  # type: ignore
                 sys._exit = Scalene.clean_exit  # type: ignore
 
         # Start a subprocess with the required environment variables,
         # which may include preloading libscalene
         req_env = ScalenePreload.get_preload_environ(args)
-        if not all(k_v in os.environ.items() for k_v in req_env.items()):
+        if any(k_v not in os.environ.items() for k_v in req_env.items()):
             os.environ.update(req_env)
-
             new_args = [
                 sys.executable,
                 "-m",
                 "scalene",
             ] + sys.argv[1:]
             result = subprocess.Popen(new_args, close_fds=True, shell=False)
             with contextlib.suppress(Exception):
```

### Comparing `scalene-1.5.8/scalene/scalene_profiler.py` & `scalene-1.5.9/scalene/scalene_profiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Scalene: a scripting-language aware profiler for Python.
+"""Scalene: a CPU+memory+GPU (and more) profiler for Python.
 
     https://github.com/plasma-umass/scalene
 
     See the paper "docs/scalene-paper.pdf" in this repository for technical
     details on an earlier version of Scalene's design; note that a
     number of these details have changed.
 
@@ -86,28 +86,36 @@
 # particular, Linux, Mac OS X, and WSL 2 (Windows Subsystem for Linux 2 = Ubuntu).
 # It also has partial support for Windows.
 
 # Install our profile decorator.
 
 
 def scalene_redirect_profile(func: Any) -> Any:
+    """Handle @profile decorators.
+
+    If Scalene encounters any functions decorated by @profile, it will
+    only report stats for those functions.
+
+    """
     return Scalene.profile(func)
 
 
 builtins.profile = scalene_redirect_profile  # type: ignore
 
 # Must equal src/include/sampleheap.hpp NEWLINE *minus 1*
 NEWLINE_TRIGGER_LENGTH = 98820  # SampleHeap<...>::NEWLINE-1
 
 
 def start() -> None:
+    """Start profiling."""
     Scalene.start()
 
 
 def stop() -> None:
+    """Stop profiling."""
     Scalene.stop()
 
 
 class Scalene:
     """The Scalene profiler itself."""
 
     __in_jupyter = False  # are we running inside a Jupyter notebook
@@ -119,18 +127,18 @@
     __parent_pid = -1
     __initialized: bool = False
     __last_profiled = (Filename("NADA"), LineNumber(0), ByteCodeIndex(0))
     __last_profiled_invalidated = False
 
     # Support for @profile
     # decorated files
-    __files_to_profile: Dict[Filename, bool] = defaultdict(bool)
+    __files_to_profile: Set[Filename] = set()
     # decorated functions
-    __functions_to_profile: Dict[Filename, Dict[Any, bool]] = defaultdict(
-        lambda: {}
+    __functions_to_profile: Dict[Filename, Set[Any]] = defaultdict(
+        lambda: set()
     )
 
     # Cache the original thread join function, which we replace with our own version.
     __original_thread_join = threading.Thread.join
 
     # As above; we'll cache the original thread and replace it.
     __original_lock = threading.Lock
@@ -143,14 +151,15 @@
     __gpu = ScaleneGPU()
 
     __output.gpu = __gpu.has_gpu()
     __json.gpu = __gpu.has_gpu()
 
     @staticmethod
     def get_original_lock() -> threading.Lock:
+        """Return the true lock, which we shim in replacement_lock.py."""
         return Scalene.__original_lock()
 
     # Likely names for the Python interpreter.
     __all_python_names = [
         os.path.basename(sys.executable),
         os.path.basename(sys.executable) + str(sys.version_info.major),
         os.path.basename(sys.executable)
@@ -190,16 +199,15 @@
         bool
     )  # False by default
 
     child_pids: Set[
         int
     ] = set()  # Needs to be unmangled to be accessed by shims
 
-    # Signal queues for CPU timers, allocations, and memcpy
-    __cpu_sigq: ScaleneSigQueue[Any]
+    # Signal queues for allocations and memcpy
     __alloc_sigq: ScaleneSigQueue[Any]
     __memcpy_sigq: ScaleneSigQueue[Any]
     __sigqueues: List[ScaleneSigQueue[Any]]
 
     client_timer: ScaleneClientTimer = ScaleneClientTimer()
 
     __orig_signal = signal.signal
@@ -212,54 +220,69 @@
     __orig_kill = os.kill
     if sys.platform != "win32":
         __orig_setitimer = signal.setitimer
         __orig_siginterrupt = signal.siginterrupt
 
     @staticmethod
     def get_all_signals_set() -> Set[int]:
+        """Return the set of all signals currently set.
+
+        Used by replacement_signal_fns.py to shim signals used by the client program.
+        """
         return set(Scalene.__signals.get_all_signals())
 
     @staticmethod
     def get_timer_signals() -> Tuple[int, signal.Signals]:
+        """Return the set of all TIMER signals currently set.
+
+        Used by replacement_signal_fns.py to shim timers used by the client program.
+        """
         return Scalene.__signals.get_timer_signals()
 
     @staticmethod
     def set_in_jupyter() -> None:
+        """Tell Scalene that it is running inside a Jupyter notebook."""
         Scalene.__in_jupyter = True
 
     @staticmethod
     def in_jupyter() -> bool:
+        """Return whether Scalene is running inside a Jupyter notebook."""
         return Scalene.__in_jupyter
 
     @staticmethod
     def interruption_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
+        """Handle keyboard interrupts (e.g., Ctrl-C)."""
         raise KeyboardInterrupt
 
     @staticmethod
     def on_stack(
         frame: FrameType, fname: Filename, lineno: LineNumber
     ) -> Optional[FrameType]:
-        """Returns true iff the given filename and line number are anywhere on the stack starting at frame."""
-        found_frame = None
+        """Find a frame matching the given filename and line number, if any.
+
+        Used for checking whether we are still executing the same line
+        of code or not in invalidate_lines (for per-line memory
+        accounting).
+        """
         f = frame
+        current_file_and_line = (fname, lineno)
         while f:
-            if (f.f_code.co_filename, f.f_lineno) == (fname, lineno):
-                found_frame = f
-                break
+            if (f.f_code.co_filename, f.f_lineno) == current_file_and_line:
+                return f
             f = cast(FrameType, f.f_back)
-        return found_frame
+        return None
 
     @staticmethod
     def update_line() -> None:
-        # Mark a new line by allocating the trigger number of bytes.
+        """Mark a new line by allocating the trigger number of bytes."""
         bytearray(NEWLINE_TRIGGER_LENGTH)
 
     @staticmethod
     def invalidate_lines(frame: FrameType, _event: str, _arg: str) -> Any:
         """Mark the last_profiled information as invalid as soon as we execute a different line of code."""
         try:
             # If we are still on the same line, return.
@@ -270,19 +293,16 @@
                 return None
             # Different line: stop tracing this frame.
             frame.f_trace = None
             frame.f_trace_lines = False
             # If we are not in a file we should be tracing, return.
             if not Scalene.should_trace(ff):
                 return None
-            # Check if we are still executing the same line of code or
-            # not (whether in this frame or one above it).
-            f = Scalene.on_stack(frame, fname, lineno)
-            if f:
-                # Still the same line, but somewhere up the stack
+            if f := Scalene.on_stack(frame, fname, lineno):
+                # We are still on the same line, but somewhere up the stack
                 # (since we returned when it was the same line in this
                 # frame). Stop tracing in this frame.
                 return None
             # We are on a different line; stop tracing and increment the count.
             sys.settrace(None)
             Scalene.update_line()
             Scalene.__last_profiled_invalidated = False
@@ -298,126 +318,131 @@
         except Exception as e:
             print("Error in program being profiled:\n", e)
             traceback.print_exc()
             return None
 
     @classmethod
     def clear_metrics(cls) -> None:
-        """
-        Clears the various states so that each forked process
-        can start with a clean slate
-        """
+        """Clear the various states for forked processes."""
         cls.__stats.clear()
         cls.child_pids.clear()
 
     @classmethod
     def add_child_pid(cls, pid: int) -> None:
+        """Add this pid to the set of children. Used when forking."""
         cls.child_pids.add(pid)
 
     @classmethod
     def remove_child_pid(cls, pid: int) -> None:
-        try:
+        """Remove a child once we have joined with it (used by replacement_pjoin.py)."""
+        with contextlib.suppress(KeyError):
             cls.child_pids.remove(pid)
-        except KeyError:
-            # Defensive programming: this should never happen.
-            pass
 
-    # Replacement @profile decorator function.
-    # We track which functions - in which files - have been decorated,
-    # and only report stats for those.
     @staticmethod
     def profile(func: Any) -> Any:
-        # Record the file and function name
-        Scalene.__files_to_profile[func.__code__.co_filename] = True
-        Scalene.__functions_to_profile[func.__code__.co_filename][func] = True
+        """Record the file and function name.
+
+        Replacement @profile decorator function.  Scalene tracks which
+        functions - in which files - have been decorated; if any have,
+        it and only reports stats for those.
+
+        """
+        Scalene.__files_to_profile.add(func.__code__.co_filename)
+        Scalene.__functions_to_profile[func.__code__.co_filename].add(func)
 
         @functools.wraps(func)
         def wrapper_profile(*args: Any, **kwargs: Any) -> Any:
-            value = func(*args, **kwargs)
-            return value
+            return func(*args, **kwargs)
 
         return wrapper_profile
 
     @staticmethod
     def shim(func: Callable[[Any], Any]) -> Any:
-        """
-        Provides a decorator that, when used, calls the wrapped function with the Scalene type
+        """Provide a decorator that calls the wrapped function with the
+        Scalene variant.
+
+                Wrapped function must be of type (s: Scalene) -> Any.
 
-        Wrapped function must be of type (s: Scalene) -> Any
+                This decorator allows for marking a function in a separate
+                file as a drop-in replacement for an existing library
+                function. The intention is for these functions to replace a
+                function that indefinitely blocks (which interferes with
+                Scalene) with a function that awakens periodically to allow
+                for signals to be delivered.
 
-        This decorator allows for marking a function in a separate file as a drop-in replacement for an existing
-        library function. The intention is for these functions to replace a function that indefinitely blocks (which
-        interferes with Scalene) with a function that awakens periodically to allow for signals to be delivered
         """
         func(Scalene)
         # Returns the function itself to the calling file for the sake
         # of not displaying unusual errors if someone attempts to call
         # it
 
         @functools.wraps(func)
         def wrapped(*args: Any, **kwargs: Any) -> Any:
             return func(*args, **kwargs)
 
         return wrapped
 
     @staticmethod
-    def cleanup_files() -> None:
-        Scalene.__malloc_mapfile.cleanup()
-        Scalene.__memcpy_mapfile.cleanup()
-
-    @staticmethod
     def set_thread_sleeping(tid: int) -> None:
+        """Indicate the given thread is sleeping.
+
+        Used to attribute CPU time by cpu_sigqueue_processor.
+        """
         Scalene.__is_thread_sleeping[tid] = True
 
     @staticmethod
     def reset_thread_sleeping(tid: int) -> None:
+        """Indicate the given thread is not sleeping.
+
+        Used to attribute CPU time by cpu_sigqueue_processor."""
         Scalene.__is_thread_sleeping[tid] = False
 
     timer_signals = True
 
     @staticmethod
     def windows_timer_loop() -> None:
         """For Windows, send periodic timer signals; launch as a background thread."""
         Scalene.timer_signals = True
         while Scalene.timer_signals:
             time.sleep(Scalene.__args.cpu_sampling_rate)
             Scalene.__orig_raise_signal(Scalene.__signals.cpu_signal)
 
     @staticmethod
     def start_signal_queues() -> None:
-        """Starts the signal processing queues (i.e., their threads)"""
+        """Start the signal processing queues (i.e., their threads)."""
         for sigq in Scalene.__sigqueues:
             sigq.start()
 
     @staticmethod
     def stop_signal_queues() -> None:
-        """Stops the signal processing queues (i.e., their threads)"""
+        """Stop the signal processing queues (i.e., their threads)."""
         for sigq in Scalene.__sigqueues:
             sigq.stop()
 
     @staticmethod
     def term_signal_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
-
+        """Handle terminate signals."""
         Scalene.stop()
         Scalene.output_profile()
 
         Scalene.__orig_exit(Scalene.__sigterm_exit_code)
 
     @staticmethod
     def malloc_signal_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
+        """Handle allocation signals."""
         invalidated = Scalene.__last_profiled_invalidated
         (fname, lineno, lasti) = Scalene.__last_profiled
         if this_frame:
             Scalene.enter_function_meta(this_frame, Scalene.__stats)
         # Walk the stack till we find a line of code in a file we are tracing.
         found_frame = False
         f = this_frame
@@ -454,26 +479,28 @@
     @staticmethod
     def free_signal_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
+        """Handle free signals."""
         if this_frame:
             Scalene.enter_function_meta(this_frame, Scalene.__stats)
         Scalene.__alloc_sigq.put([0])
         del this_frame
 
     @staticmethod
     def memcpy_signal_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
+        """Handle memcpy signals."""
         Scalene.__memcpy_sigq.put((signum, this_frame))
         del this_frame
 
     @staticmethod
     def enable_signals() -> None:
         """Set up the signal handlers to handle interrupts for profiling and start the
         timer interrupts."""
@@ -500,15 +527,15 @@
         Scalene.__orig_signal(
             Scalene.__signals.memcpy_signal, Scalene.memcpy_signal_handler
         )
         Scalene.__orig_signal(signal.SIGTERM, Scalene.term_signal_handler)
         # Set every signal to restart interrupted system calls.
         for s in Scalene.__signals.get_all_signals():
             Scalene.__orig_siginterrupt(s, False)
-        # Turn on the CPU profiling timer to run at the sampling rate (exactly once).
+        # Turn on the CPU profiling timer to run at the sampling rate, exactly once.
         Scalene.__orig_signal(
             Scalene.__signals.cpu_signal,
             Scalene.cpu_signal_handler,
         )
         if sys.platform != "win32":
             Scalene.__orig_setitimer(
                 Scalene.__signals.cpu_timer_signal,
@@ -531,34 +558,32 @@
         import scalene.replacement_thread_join
 
         if sys.platform != "win32":
             import scalene.replacement_fork
             import scalene.replacement_poll_selector
 
         Scalene.__args = cast(ScaleneArguments, arguments)
-        Scalene.__cpu_sigq = ScaleneSigQueue(Scalene.cpu_sigqueue_processor)
         Scalene.__alloc_sigq = ScaleneSigQueue(
             Scalene.alloc_sigqueue_processor
         )
         Scalene.__memcpy_sigq = ScaleneSigQueue(
             Scalene.memcpy_sigqueue_processor
         )
         Scalene.__sigqueues = [
-            Scalene.__cpu_sigq,
             Scalene.__alloc_sigq,
             Scalene.__memcpy_sigq,
         ]
 
         # Initialize the malloc related files; if for whatever reason
         # the files don't exist and we are supposed to be profiling
         # memory, exit.
         try:
             Scalene.__malloc_mapfile = ScaleneMapFile("malloc")
             Scalene.__memcpy_mapfile = ScaleneMapFile("memcpy")
-        except:
+        except Exception:
             # Ignore if we aren't profiling memory; otherwise, exit.
             if not arguments.cpu_only:
                 sys.exit(1)
 
         Scalene.__signals.set_timer_signals(arguments.use_virtual_time)
         if arguments.pid:
             # Child process.
@@ -631,16 +656,18 @@
     @staticmethod
     def cpu_signal_handler(
         signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         this_frame: Optional[FrameType],
     ) -> None:
-        """Wrapper for CPU signal handlers."""
+        """Handle CPU signals."""
         # Get current time stats.
+        now_sys: float = 0
+        now_user: float = 0
         if sys.platform != "win32":
             # On Linux/Mac, use getrusage, which provides higher
             # resolution values than os.times() for some reason.
             ru = resource.getrusage(resource.RUSAGE_SELF)
             now_sys = ru.ru_stime
             now_user = ru.ru_utime
         else:
@@ -661,55 +688,53 @@
             if sys.platform != "win32":
                 Scalene.__orig_setitimer(
                     Scalene.__signals.cpu_timer_signal,
                     Scalene.__args.cpu_sampling_rate,
                 )
             return
 
-        # Periodically sample GPU load as well.
-        if random.randint(0, 9) == 0:
-            (gpu_load, gpu_mem_used) = Scalene.__gpu.get_stats()
-        else:
-            (gpu_load, gpu_mem_used) = (0.0, 0.0)
+        (gpu_load, gpu_mem_used) = Scalene.__gpu.get_stats()
 
-        # Pass on to the signal queue.
-        Scalene.__cpu_sigq.put(
-            (
-                signum,
-                this_frame,
-                now_virtual,
-                now_wallclock,
-                now_sys,
-                now_user,
-                gpu_load,
-                gpu_mem_used,
-                Scalene.__last_signal_time_virtual,
-                Scalene.__last_signal_time_wallclock,
-                Scalene.__last_signal_time_sys,
-                Scalene.__last_signal_time_user,
-                copy(Scalene.__is_thread_sleeping),
-            )
+        # Process these frames immediately (we no longer use sigqueues
+        # because they led to frame "drag", holding down memory until
+        # processed).
+        Scalene.cpu_sigqueue_processor(
+            signum,
+            Scalene.compute_frames_to_record(),
+            now_virtual,
+            now_wallclock,
+            now_sys,
+            now_user,
+            gpu_load,
+            gpu_mem_used,
+            Scalene.__last_signal_time_virtual,
+            Scalene.__last_signal_time_wallclock,
+            Scalene.__last_signal_time_sys,
+            Scalene.__last_signal_time_user,
+            Scalene.__is_thread_sleeping,
         )
         elapsed = now_wallclock - Scalene.__last_signal_time_wallclock
         # Store the latest values as the previously recorded values.
         Scalene.__last_signal_time_virtual = now_virtual
         Scalene.__last_signal_time_wallclock = now_wallclock
         Scalene.__last_signal_time_sys = now_sys
         Scalene.__last_signal_time_user = now_user
+        # Restart the timer while handling any timers set by the client.
         if sys.platform != "win32":
             if Scalene.client_timer.is_set:
 
                 (
                     should_raise,
                     remaining_time,
                 ) = Scalene.client_timer.yield_next_delay(elapsed)
                 if should_raise:
                     Scalene.__orig_raise_signal(signal.SIGUSR1)
                 # NOTE-- 0 will only be returned if the 'seconds' have elapsed
                 # and there is no interval
+                to_wait = 0
                 if remaining_time > 0:
                     to_wait = min(
                         remaining_time, Scalene.__args.cpu_sampling_rate
                     )
                 else:
                     to_wait = Scalene.__args.cpu_sampling_rate
                     Scalene.client_timer.reset()
@@ -721,63 +746,60 @@
                 Scalene.__orig_setitimer(
                     Scalene.__signals.cpu_timer_signal,
                     Scalene.__args.cpu_sampling_rate,
                 )
 
     @staticmethod
     def output_profile() -> bool:
+        # sourcery skip: inline-immediately-returned-variable
+        """Output the profile. Returns true iff there was any info reported the profile."""
         if Scalene.__args.json:
             json_output = Scalene.__json.output_profiles(
                 Scalene.__program_being_profiled,
                 Scalene.__stats,
                 Scalene.__pid,
                 Scalene.profile_this_code,
                 Scalene.__python_alias_dir,
                 profile_memory=not Scalene.__args.cpu_only,
             )
-            if json_output:
-                if not Scalene.__output.output_file:
-                    Scalene.__output.output_file = "/dev/stdout"
-                with open(Scalene.__output.output_file, "w") as f:
-                    f.write(
-                        json.dumps(json_output, sort_keys=True, indent=4)
-                        + "\n"
-                    )
-                return True
-            else:
-                return False
+            if not Scalene.__output.output_file:
+                Scalene.__output.output_file = "/dev/stdout"
+            with open(Scalene.__output.output_file, "w") as f:
+                f.write(
+                    json.dumps(json_output, sort_keys=True, indent=4) + "\n"
+                )
+            return json_output != {}
+
         else:
             output = Scalene.__output
             column_width = Scalene.__args.column_width
             if not Scalene.__args.html:
                 # Get column width of the terminal and adjust to fit.
-                try:
+                with contextlib.suppress(Exception):
                     # If we are in a Jupyter notebook, stick with 132
                     if "ipykernel" in sys.modules:
                         column_width = 132
                     else:
                         import shutil
 
                         column_width = shutil.get_terminal_size().columns
-                except:
-                    pass
-
             did_output: bool = output.output_profiles(
                 column_width,
                 Scalene.__stats,
                 Scalene.__pid,
                 Scalene.profile_this_code,
                 Scalene.__python_alias_dir,
                 profile_memory=not Scalene.__args.cpu_only,
                 reduced_profile=Scalene.__args.reduced_profile,
             )
             return did_output
 
     @staticmethod
     def profile_this_code(fname: Filename, lineno: LineNumber) -> bool:
+        # sourcery skip: inline-immediately-returned-variable
         """When using @profile, only profile files & lines that have been decorated."""
         if not Scalene.__files_to_profile:
             return True
         if fname not in Scalene.__files_to_profile:
             return False
         # Now check to see if it's the right line range.
         line_info = (
@@ -791,15 +813,15 @@
         return found_function
 
     @staticmethod
     def cpu_sigqueue_processor(
         _signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
-        this_frame: FrameType,
+        new_frames: List[Tuple[FrameType, int, FrameType]],
         now_virtual: float,
         now_wallclock: float,
         now_sys: float,
         now_user: float,
         gpu_load: float,
         gpu_mem_used: float,
         prev_virtual: float,
@@ -824,14 +846,18 @@
                 locks = [
                     stack.enter_context(s.lock) for s in Scalene.__sigqueues
                 ]
                 stats.stop_clock()
                 Scalene.output_profile()
                 stats.start_clock()
 
+        if not new_frames:
+            # No new frames, so nothing to update.
+            return
+
         # Here we take advantage of an ostensible limitation of Python:
         # it only delivers signals after the interpreter has given up
         # control. This seems to mean that sampling is limited to code
         # running purely in the interpreter, and in fact, that was a limitation
         # of the first version of Scalene, meaning that native code was entirely ignored.
         #
         # (cf. https://docs.python.org/3.9/library/signal.html#execution-of-python-signal-handlers)
@@ -847,18 +873,17 @@
         # and compare it to the interval, and add any computed delay
         # (as if it were sampled) to the C counter.
         elapsed_virtual = now_virtual - prev_virtual
         elapsed_wallclock = now_wallclock - prev_wallclock
         # CPU utilization is the fraction of time spent on the CPU
         # over the total time.
         elapsed_user = now_user - prev_user
-        try:
+        cpu_utilization = 0.0
+        if elapsed_wallclock != 0:
             cpu_utilization = elapsed_user / elapsed_wallclock
-        except ZeroDivisionError:
-            cpu_utilization = 0.0
         # On multicore systems running multi-threaded native code, CPU
         # utilization can exceed 1; that is, elapsed user time is
         # longer than elapsed wallclock time. If this occurs, set
         # wall clock time to user time and set CPU utilization to 100%.
         if cpu_utilization > 1.0:
             cpu_utilization = 1.0
             elapsed_wallclock = elapsed_user
@@ -867,106 +892,101 @@
         # We don't want to report 'nan', so turn the load into 0.
         if math.isnan(gpu_load):
             gpu_load = 0.0
         gpu_time = gpu_load * Scalene.__args.cpu_sampling_rate
         Scalene.__stats.total_gpu_samples += gpu_time
         python_time = Scalene.__args.cpu_sampling_rate
         c_time = elapsed_virtual - python_time
-        if c_time < 0:
-            c_time = 0
-
-        # Update counters for every running thread.
-
-        new_frames = Scalene.compute_frames_to_record(this_frame)
-
+        c_time = max(c_time, 0)
         # Now update counters (weighted) for every frame we are tracking.
         total_time = python_time + c_time
 
         # First, find out how many frames are not sleeping.  We need
         # to know this number so we can parcel out time appropriately
         # (equally to each running thread).
         total_frames = sum(
-            1
-            for (frame, tident, orig_frame) in new_frames
-            if not is_thread_sleeping[tident]
+            not is_thread_sleeping[tident]
+            for frame, tident, orig_frame in new_frames
         )
 
-        if total_frames == 0:
-            normalized_time = total_time
-        else:
-            normalized_time = total_time / total_frames
+        normalized_time = total_time
+        if total_frames != 0:
+            normalized_time /= total_frames
 
         # Now attribute execution time.
+
+        main_thread_frame = new_frames[0][0]
+        if total_frames:
+            average_python_time = python_time / total_frames
+            average_c_time = c_time / total_frames
+            average_gpu_time = gpu_time / total_frames
+            average_cpu_time = (python_time + c_time) / total_frames
+
+        # First, handle the main thread.
+        Scalene.enter_function_meta(main_thread_frame, Scalene.__stats)
+        fname = Filename(main_thread_frame.f_code.co_filename)
+        lineno = LineNumber(main_thread_frame.f_lineno)
+        if not is_thread_sleeping[threading.main_thread().ident]:
+            Scalene.__stats.cpu_samples_python[fname][
+                lineno
+            ] += average_python_time
+            Scalene.__stats.cpu_samples_c[fname][lineno] += average_c_time
+            Scalene.__stats.cpu_samples[fname] += average_cpu_time
+            Scalene.__stats.cpu_utilization[fname][lineno].push(
+                cpu_utilization
+            )
+            Scalene.__stats.gpu_samples[fname][lineno] += average_gpu_time
+            Scalene.__stats.gpu_mem_samples[fname][lineno].push(
+                gpu_mem_used
+            )
+
+        # Now handle the rest of the threads.
         for (frame, tident, orig_frame) in new_frames:
+            if frame == main_thread_frame:
+                continue
+            # In a thread.
             fname = Filename(frame.f_code.co_filename)
             lineno = LineNumber(frame.f_lineno)
             Scalene.enter_function_meta(frame, Scalene.__stats)
-            if frame == new_frames[0][0]:
-                # Main thread.
-                if not is_thread_sleeping[tident]:
-
-                    Scalene.__stats.cpu_samples_python[fname][lineno] += (
-                        python_time / total_frames
-                    )
-                    Scalene.__stats.cpu_samples_c[fname][lineno] += (
-                        c_time / total_frames
-                    )
-                    Scalene.__stats.cpu_samples[fname] += (
-                        python_time + c_time
-                    ) / total_frames
-                    Scalene.__stats.cpu_utilization[fname][lineno].push(
-                        cpu_utilization
-                    )
-                    Scalene.__stats.gpu_samples[fname][lineno] += (
-                        gpu_time / total_frames
-                    )
-                    Scalene.__stats.gpu_mem_samples[fname][lineno].push(
-                        gpu_mem_used
-                    )
-
-            else:
-                # We can't play the same game here of attributing
-                # time, because we are in a thread, and threads don't
-                # get signals in Python. Instead, we check if the
-                # bytecode instruction being executed is a function
-                # call.  If so, we attribute all the time to native.
-                # NOTE: for now, we don't try to attribute GPU time to threads.
-                if not is_thread_sleeping[tident]:
-                    # Check if the original caller is stuck inside a call.
-                    if ScaleneFuncUtils.is_call_function(
-                        orig_frame.f_code,
-                        ByteCodeIndex(orig_frame.f_lasti),
-                    ):
-                        # It is. Attribute time to native.
-                        Scalene.__stats.cpu_samples_c[fname][
-                            lineno
-                        ] += normalized_time
-                    else:
-                        # Not in a call function so we attribute the time to Python.
-                        Scalene.__stats.cpu_samples_python[fname][
-                            lineno
-                        ] += normalized_time
-                    Scalene.__stats.cpu_samples[fname] += normalized_time
-                    Scalene.__stats.cpu_utilization[fname][lineno].push(
-                        cpu_utilization
-                    )
+            # We can't play the same game here of attributing
+            # time, because we are in a thread, and threads don't
+            # get signals in Python. Instead, we check if the
+            # bytecode instruction being executed is a function
+            # call.  If so, we attribute all the time to native.
+            # NOTE: for now, we don't try to attribute GPU time to threads.
+            if not is_thread_sleeping[tident]:
+                # Check if the original caller is stuck inside a call.
+                if ScaleneFuncUtils.is_call_function(
+                    orig_frame.f_code,
+                    ByteCodeIndex(orig_frame.f_lasti),
+                ):
+                    # It is. Attribute time to native.
+                    Scalene.__stats.cpu_samples_c[fname][
+                        lineno
+                    ] += normalized_time
+                else:
+                    # Not in a call function so we attribute the time to Python.
+                    Scalene.__stats.cpu_samples_python[fname][
+                        lineno
+                    ] += normalized_time
+                Scalene.__stats.cpu_samples[fname] += normalized_time
+                Scalene.__stats.cpu_utilization[fname][lineno].push(
+                    cpu_utilization
+                )
 
         # Clean up all the frames
         del new_frames[:]
         del new_frames
-        del this_frame
         del is_thread_sleeping
         Scalene.__stats.total_cpu_samples += total_time
 
     # Returns final frame (up to a line in a file we are profiling), the thread identifier, and the original frame.
     @staticmethod
-    def compute_frames_to_record(
-        _this_frame: FrameType,
-    ) -> List[Tuple[FrameType, int, FrameType]]:
-        """Collects all stack frames that Scalene actually processes."""
+    def compute_frames_to_record() -> List[Tuple[FrameType, int, FrameType]]:
+        """Collect all stack frames that Scalene actually processes."""
         frames: List[Tuple[FrameType, int]] = [
             (
                 cast(
                     FrameType,
                     sys._current_frames().get(cast(int, t.ident), None),
                 ),
                 cast(int, t.ident),
@@ -1002,18 +1022,18 @@
             while not Scalene.should_trace(fname):
                 # Walk the stack backwards until we hit a frame that
                 # IS one we should trace (if there is one).  i.e., if
                 # it's in the code being profiled, and it is just
                 # calling stuff deep in libraries.
                 if frame:
                     frame = cast(FrameType, frame.f_back)
-                    if frame:
-                        fname = frame.f_code.co_filename
                 else:
                     break
+                if frame:
+                    fname = frame.f_code.co_filename
             if frame:
                 new_frames.append((frame, tident, orig_frame))
         del frames[:]
         return new_frames
 
     @staticmethod
     def enter_function_meta(
@@ -1026,15 +1046,15 @@
         f = frame
         try:
             while "<" in Filename(f.f_code.co_name):
                 f = cast(FrameType, f.f_back)
                 # Handle case where the function with the name wrapped in triangle brackets is at the bottom of the stack
                 if f is None:
                     return
-        except:
+        except Exception:
             return
         if not Scalene.should_trace(f.f_code.co_filename):
             return
 
         fn_name = Filename(f.f_code.co_name)
         firstline = f.f_code.co_firstlineno
         # Prepend the class, if any
@@ -1044,21 +1064,21 @@
             and f.f_back.f_code
             # NOTE: next line disabled as it is interfering with name resolution for thread run methods
             # and Scalene.should_trace(f.f_back.f_code.co_filename)
         ):
             if "self" in f.f_locals:
                 prepend_name = f.f_locals["self"].__class__.__name__
                 if "Scalene" not in prepend_name:
-                    fn_name = prepend_name + "." + fn_name
+                    fn_name = f"{prepend_name}.{fn_name}"
                 break
             if "cls" in f.f_locals:
                 prepend_name = getattr(f.f_locals["cls"], "__name__", None)
                 if not prepend_name or "Scalene" in prepend_name:
                     break
-                fn_name = prepend_name + "." + fn_name
+                fn_name = f"{prepend_name}.{fn_name}"
                 break
             f = f.f_back
 
         stats.function_map[fname][lineno] = fn_name
         stats.firstline_map[fn_name] = LineNumber(firstline)
 
     @staticmethod
@@ -1091,76 +1111,76 @@
                     python_fraction_str,
                     pid,
                     pointer,
                     reported_fname,
                     reported_lineno,
                     bytei_str,
                 ) = count_str.split(",")
-                if int(curr_pid) == int(pid):
-                    arr.append(
-                        (
-                            int(alloc_time_str),
-                            action,
-                            float(count_str),
-                            float(python_fraction_str),
-                            pointer,
-                            Filename(reported_fname),
-                            LineNumber(int(reported_lineno)),
-                            ByteCodeIndex(int(bytei_str)),
-                        )
+                if int(curr_pid) != int(pid):
+                    continue
+                arr.append(
+                    (
+                        int(alloc_time_str),
+                        action,
+                        float(count_str),
+                        float(python_fraction_str),
+                        pointer,
+                        Filename(reported_fname),
+                        LineNumber(int(reported_lineno)),
+                        ByteCodeIndex(int(bytei_str)),
                     )
+                )
 
         # Iterate through the array to compute the new current footprint
         # and update the global __memory_footprint_samples. Since on some systems,
         # we get free events before mallocs, force `before` to always be at least 0.
         before = max(stats.current_footprint, 0)
         prevmax = stats.max_footprint
         freed_last_trigger = 0
-        for (index, item) in enumerate(arr):
+        for item in arr:
             (
                 _alloc_time,
                 action,
                 count,
                 _python_fraction,
                 pointer,
                 fname,
                 lineno,
                 bytei,
             ) = item
             is_malloc = action == "M"
             count /= 1024 * 1024
             if is_malloc:
                 stats.current_footprint += count
-                stats.max_footprint = max(
-                    stats.current_footprint, stats.max_footprint
-                )
+                # stats.max_footprint = max(
+                #     stats.current_footprint, stats.max_footprint
+                # )
+                if stats.current_footprint > stats.max_footprint:
+                    stats.max_footprint = stats.current_footprint
+                    stats.max_footprint_loc = (fname, lineno)
             else:
-                assert action == "f" or action == "F"
+                assert action in ["f", "F"]
                 stats.current_footprint -= count
                 # Force current footprint to be non-negative; this
                 # code is needed because Scalene can miss some initial
                 # allocations at startup.
                 stats.current_footprint = max(0, stats.current_footprint)
-                if action == "f":
-                    # Check if pointer actually matches
-                    if stats.last_malloc_triggered[2] == pointer:
-                        freed_last_trigger += 1
+                if action == "f" and stats.last_malloc_triggered[2] == pointer:
+                    freed_last_trigger += 1
             timestamp = time.monotonic_ns() - Scalene.__start_time
             if len(stats.memory_footprint_samples) > 2:
                 # Compress the footprints by discarding intermediate
                 # points along increases and decreases. For example:
                 # if the new point is an increase over the previous
                 # point, and that point was also an increase,
                 # eliminate the previous (intermediate) point.
                 (t1, prior_y) = stats.memory_footprint_samples[-2]
                 (t2, last_y) = stats.memory_footprint_samples[-1]
                 y = stats.current_footprint
-                if (prior_y < last_y and last_y < y) or (
-                    prior_y > last_y and last_y > y
-                ):
+                if prior_y < last_y < y or prior_y > last_y > y:
                     # Same direction.
                     # Replace the previous (intermediate) point.
                     stats.memory_footprint_samples[-1] = [timestamp, y]
                 else:
                     stats.memory_footprint_samples.append([timestamp, y])
             else:
                 stats.memory_footprint_samples.append(
@@ -1168,19 +1188,15 @@
                         timestamp,
                         stats.current_footprint,
                     ]
                 )
         after = stats.current_footprint
 
         if freed_last_trigger:
-            if freed_last_trigger > 1:
-                # Ignore the case where we have multiple last triggers in the sample file,
-                # since this can lead to false positives.
-                pass
-            else:
+            if freed_last_trigger <= 1:
                 # We freed the last allocation trigger. Adjust scores.
                 this_fn, this_ln, _this_ptr = stats.last_malloc_triggered
                 if this_ln != 0:
                     mallocs, frees = stats.leak_score[this_fn][this_ln]
                     stats.leak_score[this_fn][this_ln] = (
                         mallocs,
                         frees + 1,
@@ -1246,15 +1262,15 @@
                     stats.memory_current_footprint[fname][lineno],
                 )
                 stats.memory_max_footprint[fname][lineno] = max(
                     stats.memory_current_footprint[fname][lineno],
                     stats.memory_max_footprint[fname][lineno],
                 )
             else:
-                assert action == "f" or action == "F"
+                assert action in ["f", "F"]
                 curr -= count
                 stats.memory_free_samples[fname][lineno] += count
                 stats.memory_free_count[fname][lineno] += 1
                 stats.total_memory_free_samples += count
                 stats.memory_current_footprint[fname][lineno] -= count
                 # Ensure that we never drop the current footprint below 0.
                 stats.memory_current_footprint[fname][lineno] = max(
@@ -1271,80 +1287,92 @@
                     LineNumber(lineno),
                     Address(malloc_pointer),
                 )
         stats.allocation_velocity = (
             stats.allocation_velocity[0] + (after - before),
             stats.allocation_velocity[1] + allocs,
         )
-        if Scalene.__args.memory_leak_detector:
-            # Update leak score if we just increased the max footprint (starting at a fixed threshold, currently 100MB
-            if prevmax < stats.max_footprint and stats.max_footprint > 100:
-                stats.last_malloc_triggered = last_malloc
-                fname, lineno, _ = last_malloc
-                mallocs, frees = stats.leak_score[fname][lineno]
-                stats.leak_score[fname][lineno] = (mallocs + 1, frees)
+        if (
+            Scalene.__args.memory_leak_detector
+            and prevmax < stats.max_footprint
+            and stats.max_footprint > 100
+        ):
+            stats.last_malloc_triggered = last_malloc
+            fname, lineno, _ = last_malloc
+            mallocs, frees = stats.leak_score[fname][lineno]
+            stats.leak_score[fname][lineno] = (mallocs + 1, frees)
 
     @staticmethod
     def before_fork() -> None:
-        """Executed just before a fork."""
+        """The parent process should invoke this function just before a fork.
+
+        Invoked by replacement_fork.py.
+        """
         Scalene.stop_signal_queues()
 
     @staticmethod
     def after_fork_in_parent(child_pid: int) -> None:
-        """Executed by the parent process after a fork."""
+        """The parent process should invoke this function after a fork.
+
+        Invoked by replacement_fork.py.
+        """
         Scalene.add_child_pid(child_pid)
         Scalene.start_signal_queues()
 
     @staticmethod
     def after_fork_in_child() -> None:
         """
-        Executed by a child process after a fork and mutates the
+        Executed by a child process after a fork; mutates the
         current profiler into a child.
+
+        Invoked by replacement_fork.py.
         """
         Scalene.__is_child = True
 
         Scalene.clear_metrics()
         if Scalene.__gpu.has_gpu():
             Scalene.__gpu.nvml_reinit()
-        # Note-- __parent_pid of the topmost process is its own pid
+        # Note: __parent_pid of the topmost process is its own pid.
         Scalene.__pid = Scalene.__parent_pid
-        if not "off" in Scalene.__args or not Scalene.__args.off:
+        if "off" not in Scalene.__args or not Scalene.__args.off:
             Scalene.enable_signals()
 
     @staticmethod
     def memcpy_sigqueue_processor(
         _signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         frame: FrameType,
     ) -> None:
+        """Process memcpy signals (used in a ScaleneSigQueue)."""
         curr_pid = os.getpid()
         arr: List[Tuple[str, int, int, int, int]] = []
         # Process the input array.
         with contextlib.suppress(ValueError):
             while Scalene.__memcpy_mapfile.read():
                 count_str = Scalene.__memcpy_mapfile.get_str()
                 (
                     memcpy_time_str,
                     count_str2,
                     pid,
                     filename,
                     lineno,
                     bytei,
                 ) = count_str.split(",")
-                if int(curr_pid) == int(pid):
-                    arr.append(
-                        (
-                            filename,
-                            int(lineno),
-                            int(bytei),
-                            int(memcpy_time_str),
-                            int(count_str2),
-                        )
+                if int(curr_pid) != int(pid):
+                    continue
+                arr.append(
+                    (
+                        filename,
+                        int(lineno),
+                        int(bytei),
+                        int(memcpy_time_str),
+                        int(count_str2),
                     )
+                )
         arr.sort()
 
         for item in arr:
             filename, linenum, byteindex, _memcpy_time, count = item
             fname = Filename(filename)
             line_no = LineNumber(linenum)
             byteidx = ByteCodeIndex(byteindex)
@@ -1357,78 +1385,64 @@
     def should_trace(filename: str) -> bool:
         """Return true if the filename is one we should trace."""
         if not filename:
             return False
         if "scalene/scalene" in filename:
             # Don't profile the profiler.
             return False
-        if "site-packages" in filename or "/lib/python" in filename:
-            # Don't profile Python internals by default.
-            if not Scalene.__args.profile_all:
-                return False
+        if (
+            "site-packages" in filename or "/lib/python" in filename
+        ) and not Scalene.__args.profile_all:
+            return False
         # Generic handling follows (when no @profile decorator has been used).
         profile_exclude_list = Scalene.__args.profile_exclude.split(",")
         if any(
             prof in filename for prof in profile_exclude_list if prof != ""
         ):
             return False
         if filename[0] == "<":
-            if "<ipython" in filename:
-                # Profiling code created in a Jupyter cell:
-                # create a file to hold the contents.
-                import re
-
-                import IPython
-
-                # Find the input where the function was defined;
-                # we need this to properly annotate the code.
-                result = re.match("<ipython-input-([0-9]+)-.*>", filename)
-                if result:
-                    # Write the cell's contents into the file.
-                    with open(filename, "w+") as f:
-                        f.write(
-                            IPython.get_ipython().history_manager.input_hist_raw[
-                                int(result.group(1))
-                            ]
-                        )
-                return True
-            else:
+            if "<ipython" not in filename:
                 # Not a real file and not a function created in Jupyter.
                 return False
+            # Profiling code created in a Jupyter cell:
+            # create a file to hold the contents.
+            import re
+
+            import IPython
+
+            if result := re.match("<ipython-input-([0-9]+)-.*>", filename):
+                # Write the cell's contents into the file.
+                with open(filename, "w+") as f:
+                    f.write(
+                        IPython.get_ipython().history_manager.input_hist_raw[
+                            int(result[1])
+                        ]
+                    )
+            return True
         # If (a) `profile-only` was used, and (b) the file matched
         # NONE of the provided patterns, don't profile it.
         profile_only_set = set(Scalene.__args.profile_only.split(","))
-        not_found_in_profile_only = profile_only_set and not any(
-            prof in filename for prof in profile_only_set
-        )
-        if not_found_in_profile_only:
+        if not_found_in_profile_only := profile_only_set and all(
+            prof not in filename for prof in profile_only_set
+        ):
             return False
         # Now we've filtered out any non matches to profile-only patterns.
         # If `profile-all` is specified, profile this file.
         if Scalene.__args.profile_all:
             return True
         # Profile anything in the program's directory or a child directory,
         # but nothing else, unless otherwise specified.
         filename = os.path.abspath(filename)
         return Scalene.__program_path in filename
 
-    @staticmethod
-    def clear_mmap_data() -> None:
-        if not Scalene.__args.cpu_only:
-            while Scalene.__malloc_mapfile.read():
-                pass
-            while Scalene.__memcpy_mapfile.read():
-                pass
-
     __done = False
 
     @staticmethod
     def start() -> None:
         """Initiate profiling."""
-        # Scalene.clear_mmap_data()
         if not Scalene.__initialized:
             print(
                 "ERROR: Do not try to invoke `start` when you have not called Scalene using one of the methods "
                 "in https://github.com/plasma-umass/scalene#using-scalene"
             )
             sys.exit(1)
         Scalene.__stats.start_clock()
@@ -1448,56 +1462,65 @@
             and not Scalene.__is_child
         ):
             if Scalene.in_jupyter():
                 # Force JSON output to profile.json.
                 Scalene.__args.json = True
                 Scalene.__output.html = False
                 Scalene.__output.output_file = "profile.json"
-            else:
-                # Check for a browser.
-                try:
-                    if (
-                        not webbrowser.get()
-                        or type(webbrowser.get()).__name__ == "GenericBrowser"
-                    ):
-                        # Could not open a graphical web browser tab;
-                        # act as if --web was not specified
-                        # (GenericBrowser means text-based browsers like Lynx.)
-                        Scalene.__args.web = False
-                    else:
-                        # Force JSON output to profile.json.
-                        Scalene.__args.json = True
-                        Scalene.__output.html = False
-                        Scalene.__output.output_file = "profile.json"
-                except:
-                    # Couldn't find a browser.
+                return
+            # Check for a browser.
+            try:
+                if (
+                    not webbrowser.get()
+                    or type(webbrowser.get()).__name__ == "GenericBrowser"
+                ):
+                    # Could not open a graphical web browser tab;
+                    # act as if --web was not specified
+                    # (GenericBrowser means text-based browsers like Lynx.)
                     Scalene.__args.web = False
+                else:
+                    # Force JSON output to profile.json.
+                    Scalene.__args.json = True
+                    Scalene.__output.html = False
+                    Scalene.__output.output_file = "profile.json"
+            except Exception:
+                # Couldn't find a browser.
+                Scalene.__args.web = False
 
     @staticmethod
     def is_done() -> bool:
+        """Return true if Scalene has stopped profiling."""
         return Scalene.__done
 
     @staticmethod
     def start_signal_handler(
         _signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         _this_frame: Optional[FrameType],
     ) -> None:
+        """Respond to a signal to start or resume profiling (--on).
+
+        See scalene_parseargs.py.
+        """
         for pid in Scalene.child_pids:
             Scalene.__orig_kill(pid, Scalene.__signals.start_profiling_signal)
         Scalene.start()
 
     @staticmethod
     def stop_signal_handler(
         _signum: Union[
             Callable[[Signals, FrameType], None], int, Handlers, None
         ],
         _this_frame: Optional[FrameType],
     ) -> None:
+        """Respond to a signal to suspend profiling (--off).
+
+        See scalene_parseargs.py.
+        """
         for pid in Scalene.child_pids:
             Scalene.__orig_kill(pid, Scalene.__signals.stop_profiling_signal)
         Scalene.stop()
 
     @staticmethod
     def disable_signals(retry: bool = True) -> None:
         """Turn off the profiling signals."""
@@ -1528,29 +1551,21 @@
         # Delete the temporary directory.
         with contextlib.suppress(Exception):
             if not Scalene.__pid:
                 Scalene.__python_alias_dir.cleanup()  # type: ignore
         with contextlib.suppress(Exception):
             os.remove(f"/tmp/scalene-malloc-lock{os.getpid()}")
 
-    @staticmethod
-    def termination_handler(
-        _signum: Union[
-            Callable[[Signals, FrameType], None], int, Handlers, None
-        ],
-        _this_frame: FrameType,
-    ) -> None:
-        sys.exit(1)
-
     def profile_code(
         self,
         code: str,
         the_globals: Dict[str, str],
         the_locals: Dict[str, str],
     ) -> int:
+        """Initiate execution and profiling."""
         # If --off is set, tell all children to not profile and stop profiling before we even start.
         if "off" not in Scalene.__args or not Scalene.__args.off:
             self.start()
         # Run the code being profiled.
         exit_status = 0
         try:
             exec(code, the_globals, the_locals)
@@ -1564,137 +1579,145 @@
             print("Error in program being profiled:\n", e)
             traceback.print_exc()
             exit_status = 1
         finally:
             self.stop()
             sys.settrace(None)
             # If we've collected any samples, dump them.
-            if not Scalene.output_profile():
+            did_output = Scalene.output_profile()
+            if not did_output:
                 print(
                     "Scalene: Program did not run for long enough to profile."
                 )
 
-            if (
-                Scalene.__args.web
+            if not (
+                did_output
+                and Scalene.__args.web
                 and not Scalene.__args.cli
                 and not Scalene.__is_child
             ):
-                # Start up a web server (in a background thread) to host the GUI,
-                # and open a browser tab to the server. If this fails, fail-over
-                # to using the CLI.
-
-                try:
-                    PORT = Scalene.__args.port
-
-                    # Silence web server output by overriding logging messages.
-                    class NoLogs(http.server.SimpleHTTPRequestHandler):
-                        def log_message(
-                            self, format: str, *args: List[Any]
-                        ) -> None:
-                            return
-
-                        def log_request(
-                            self,
-                            code: Union[int, str] = 0,
-                            size: Union[int, str] = 0,
-                        ) -> None:
-                            return
-
-                    Handler = NoLogs
-                    socketserver.TCPServer.allow_reuse_address = True
-                    with socketserver.TCPServer(("", PORT), Handler) as httpd:
-                        import threading
+                return exit_status
+            
+            # Start up a web server (in a background thread) to host the GUI,
+            # and open a browser tab to the server. If this fails, fail-over
+            # to using the CLI.
 
-                        t = threading.Thread(target=httpd.serve_forever)
-                        # Copy files into a new directory and then point the tab there.
-                        import shutil
+            try:
+                PORT = Scalene.__args.port
 
-                        webgui_dir = pathlib.Path(
-                            tempfile.mkdtemp(prefix="scalene-gui")
-                        )
-                        shutil.copytree(
-                            os.path.join(
-                                os.path.dirname(__file__), "scalene-gui"
-                            ),
-                            os.path.join(webgui_dir, "scalene-gui"),
-                        )
-                        shutil.copy(
-                            "profile.json",
-                            os.path.join(webgui_dir, "scalene-gui"),
-                        )
-                        os.chdir(os.path.join(webgui_dir, "scalene-gui"))
-                        t.start()
-                        if Scalene.in_jupyter():
-                            from IPython.core.display import HTML, display
-                            from IPython.display import IFrame
-
-                            display(
-                                IFrame(
-                                    src=f"http://localhost:{PORT}/profiler.html",
-                                    width=700,
-                                    height=600,
-                                )
-                            )
-                        else:
-                            # Disable the preload environment
-                            # variables which are no longer needed
-                            # anyway (for memory/copy volume tracking)
-                            # and which interfere with at least one
-                            # browser on one platform.
-                            os.environ["LD_PRELOAD"] = ""
-                            os.environ["DYLD_INSERT_LIBRARIES"] = ""
-                            # Now open a new tab with the profiler.
-                            result = webbrowser.open_new_tab(
-                                f"http://localhost:{PORT}/profiler.html"
-                            )
-                        # Wait long enough for the server to serve the page, and then shut down the server.
-                        time.sleep(5)
-                        httpd.shutdown()
-                except OSError:
-                    print(
-                        f"Scalene: unable to run the Scalene GUI on port {PORT}."
+                # Silence web server output by overriding logging messages.
+                class NoLogs(http.server.SimpleHTTPRequestHandler):
+                    def log_message(
+                        self, format: str, *args: List[Any]
+                    ) -> None:
+                        return
+
+                    def log_request(
+                        self,
+                        code: Union[int, str] = 0,
+                        size: Union[int, str] = 0,
+                    ) -> None:
+                        return
+
+                Handler = NoLogs
+                socketserver.TCPServer.allow_reuse_address = True
+                with socketserver.TCPServer(("", PORT), Handler) as httpd:
+                    import threading
+
+                    t = threading.Thread(target=httpd.serve_forever)
+                    # Copy files into a new directory and then point the tab there.
+                    import shutil
+
+                    webgui_dir = pathlib.Path(
+                        tempfile.mkdtemp(prefix="scalene-gui")
                     )
-                    print("Possible solutions:")
-                    print("(1) Use a different port (with --port)")
-                    print("(2) Use the text version (with --cli)")
-                    print(
-                        "(3) Upload a generated profile.json file to the web GUI: https://plasma-umass.org/scalene-gui/."
+                    shutil.copytree(
+                        os.path.join(
+                            os.path.dirname(__file__), "scalene-gui"
+                        ),
+                        os.path.join(webgui_dir, "scalene-gui"),
+                    )
+                    shutil.copy(
+                        "profile.json",
+                        os.path.join(webgui_dir, "scalene-gui"),
                     )
+                    os.chdir(os.path.join(webgui_dir, "scalene-gui"))
+                    t.start()
+                    if Scalene.in_jupyter():
+                        from IPython.core.display import HTML, display
+                        from IPython.display import IFrame
+
+                        display(
+                            IFrame(
+                                src=f"http://localhost:{PORT}/profiler.html",
+                                width=700,
+                                height=600,
+                            )
+                        )
+                    else:
+                        # Disable the preload environment
+                        # variables which are no longer needed
+                        # anyway (for memory/copy volume tracking)
+                        # and which interfere with at least one
+                        # browser on one platform.
+                        os.environ["LD_PRELOAD"] = ""
+                        os.environ["DYLD_INSERT_LIBRARIES"] = ""
+                        # Now open a new tab with the profiler.
+                        result = webbrowser.open_new_tab(
+                            f"http://localhost:{PORT}/profiler.html"
+                        )
+                    # Wait long enough for the server to serve the page, and then shut down the server.
+                    time.sleep(5)
+                    httpd.shutdown()
+            except OSError:
+                print(
+                    f"Scalene: unable to run the Scalene GUI on port {PORT}."
+                )
+                print("Possible solutions:")
+                print("(1) Use a different port (with --port)")
+                print("(2) Use the text version (with --cli)")
+                print(
+                    "(3) Upload a generated profile.json file to the web GUI: https://plasma-umass.org/scalene-gui/."
+                )
 
         return exit_status
 
     @staticmethod
     def process_args(args: argparse.Namespace) -> None:
+        """Process all arguments."""
         Scalene.__args = cast(ScaleneArguments, args)
         Scalene.__next_output_time = (
             time.perf_counter() + Scalene.__args.profile_interval
         )
         Scalene.__output.html = args.html
         Scalene.__output.output_file = args.outfile
         Scalene.__is_child = args.pid != 0
         # the pid of the primary profiler
         Scalene.__parent_pid = args.pid if Scalene.__is_child else os.getpid()
 
     @staticmethod
     def set_initialized() -> None:
+        """Indicate that Scalene has been initialized and is ready to begin profiling."""
         Scalene.__initialized = True
 
     @staticmethod
     def main() -> None:
+        """Initialize and profile."""
         (
             args,
             left,
         ) = ScaleneParseArgs.parse_args()
         Scalene.set_initialized()
         Scalene.run_profiler(args, left)
 
     @staticmethod
     def run_profiler(
         args: argparse.Namespace, left: List[str], is_jupyter: bool = False
     ) -> None:
+        """Set up and initiate profiling."""
         # Set up signal handlers for starting and stopping profiling.
         if is_jupyter:
             Scalene.set_in_jupyter()
         if not Scalene.__initialized:
             print(
                 "ERROR: Do not try to manually invoke `run_profiler`.\n"
                 "To invoke Scalene programmatically, see the usage noted in https://github.com/plasma-umass/scalene#using-scalene"
@@ -1713,18 +1736,17 @@
                 Scalene.__signals.start_profiling_signal, False
             )
             Scalene.__orig_siginterrupt(
                 Scalene.__signals.stop_profiling_signal, False
             )
 
         Scalene.__orig_signal(signal.SIGINT, Scalene.interruption_handler)
-        if not is_jupyter:
-            did_preload = ScalenePreload.setup_preload(args)
-        else:
-            did_preload = False
+        did_preload = (
+            False if is_jupyter else ScalenePreload.setup_preload(args)
+        )
         if not did_preload:
             with contextlib.suppress(Exception):
                 # If running in the background, print the PID.
                 if os.getpgrp() != os.tcgetpgrp(sys.stdout.fileno()):
                     # In the background.
                     print(f"Scalene now profiling process {os.getpid()}")
                     print(
@@ -1743,20 +1765,20 @@
             progs = None
             exit_status = 0
             try:
                 # Look for something ending in '.py'. Treat the first one as our executable.
                 progs = [x for x in sys.argv if re.match(".*\.py$", x)]
                 # Just in case that didn't work, try sys.argv[0] and __file__.
                 with contextlib.suppress(Exception):
-                    progs.append(sys.argv[0])
-                    progs.append(__file__)
+                    progs.extend((sys.argv[0], __file__))
                 if not progs:
                     raise FileNotFoundError
                 with open(progs[0], "rb") as prog_being_profiled:
                     # Read in the code and compile it.
+                    code: Any
                     try:
                         code = compile(
                             prog_being_profiled.read(),
                             progs[0],
                             "exec",
                         )
                     except SyntaxError:
@@ -1772,15 +1794,15 @@
                     else:
                         Scalene.__program_path = program_path
                     # Grab local and global variables.
                     if not Scalene.__args.cpu_only:
                         from scalene import pywhere  # type: ignore
 
                         pywhere.register_files_to_profile(
-                            list(Scalene.__files_to_profile.keys()),
+                            list(Scalene.__files_to_profile),
                             Scalene.__program_path,
                             Scalene.__args.profile_all,
                         )
 
                     import __main__
 
                     the_locals = __main__.__dict__
@@ -1808,15 +1830,15 @@
                     except Exception as ex:
                         template = "Scalene: An exception of type {0} occurred. Arguments:\n{1!r}"
                         message = template.format(type(ex).__name__, ex.args)
                         print(message)
                         print(traceback.format_exc())
             except (FileNotFoundError, IOError):
                 if progs:
-                    print("Scalene: could not find input file " + progs[0])
+                    print(f"Scalene: could not find input file {progs[0]}")
                 else:
                     print("Scalene: no input file specified.")
                 sys.exit(1)
         except SystemExit:
             pass
         except StopJupyterExecution:
             pass
@@ -1824,13 +1846,15 @@
             print("Scalene failed to initialize.\n" + traceback.format_exc())
             sys.exit(1)
         finally:
             with contextlib.suppress(Exception):
                 Scalene.__malloc_mapfile.close()
                 Scalene.__memcpy_mapfile.close()
                 if not Scalene.__is_child:
-                    Scalene.cleanup_files()
+                    # We are done with these files, so remove them.
+                    Scalene.__malloc_mapfile.cleanup()
+                    Scalene.__memcpy_mapfile.cleanup()
             sys.exit(exit_status)
 
 
 if __name__ == "__main__":
     Scalene.main()
```

### Comparing `scalene-1.5.8/scalene/scalene_signals.py` & `scalene-1.5.9/scalene/scalene_signals.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,17 +35,19 @@
                 self.cpu_timer_signal = signal.ITIMER_VIRTUAL
                 self.cpu_signal = signal.SIGVTALRM
             else:
                 self.cpu_timer_signal = signal.ITIMER_REAL
                 self.cpu_signal = signal.SIGALRM
 
     def get_timer_signals(self) -> Tuple[int, signal.Signals]:
+        """Return the signals used for CPU profiling."""
         return self.cpu_timer_signal, self.cpu_signal
 
     def get_all_signals(self) -> List[int]:
+        """Return all the signals used for controlling profiling, except the CPU timer."""
         return [
             self.start_profiling_signal,
             self.stop_profiling_signal,
             self.memcpy_signal,
             self.malloc_signal,
             self.free_signal,
             self.cpu_signal,
```

### Comparing `scalene-1.5.8/scalene/scalene_sigqueue.py` & `scalene-1.5.9/scalene/scalene_sigqueue.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,33 +9,40 @@
     def __init__(self, process: Any) -> None:
         self.queue: queue.SimpleQueue[Optional[T]] = queue.SimpleQueue()
         self.process = process
         self.thread: Optional[threading.Thread] = None
         self.lock = threading.RLock()  # held while processing an item
 
     def put(self, item: Optional[T]) -> None:
+        """Add an item to the queue."""
         self.queue.put(item)
 
     def get(self) -> Optional[T]:
+        """Get one item from the queue."""
         return self.queue.get()
 
     def start(self) -> None:
+        """Start processing."""
         # We use a daemon thread to defensively avoid hanging if we never join with it
         if not self.thread:
             self.thread = threading.Thread(target=self.run, daemon=True)
             self.thread.start()
 
     def stop(self) -> None:
+        """Stop processing."""
         if self.thread:
             self.queue.put(None)
             # We need to join all threads before a fork() to avoid an inconsistent
             # state, locked mutexes, etc.
             self.thread.join()
             self.thread = None
 
     def run(self) -> None:
+        """Run the function processing items until stop is called.
+
+        Executed in a separate thread."""
         while True:
             item = self.queue.get()
             if item is None:  # None => stop request
                 break
             with self.lock:
                 self.process(*item)
```

### Comparing `scalene-1.5.8/scalene/scalene_statistics.py` & `scalene-1.5.9/scalene/scalene_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import os
 import pathlib
 import pickle
 import time
 from collections import defaultdict
-from typing import Any, DefaultDict, Dict, List, NewType, Set, Tuple, TypeVar
+from typing import (
+    Any,
+    DefaultDict,
+    Dict,
+    List,
+    NewType,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+)
 
 import cloudpickle
 
 # from scalene.adaptive import Adaptive
 from scalene.runningstats import RunningStats
 
 Address = NewType("Address", str)
@@ -137,15 +147,15 @@
         self.total_memory_free_samples: float = 0.0
 
         # the current memory footprint
         self.current_footprint: float = 0.0
 
         # the peak memory footprint
         self.max_footprint: float = 0.0
-
+        self.max_footprint_loc: Optional[Tuple[Filename, LineNumber]] = None
         # memory footprint samples (time, footprint)
         self.memory_footprint_samples: List[List[float]] = []
 
         # same, but per line
         self.per_line_footprint_samples: Dict[
             Filename, Dict[LineNumber, List[Any]]
         ] = defaultdict(lambda: defaultdict(list))
@@ -162,14 +172,15 @@
             Filename, Dict[LineNumber, Filename]
         ] = defaultdict(lambda: defaultdict(lambda: Filename("")))
         self.firstline_map: Dict[Filename, LineNumber] = defaultdict(
             lambda: LineNumber(1)
         )
 
     def clear(self) -> None:
+        """Reset all statistics except for memory footprint."""
         self.start_time = 0
         self.elapsed_time = 0
         self.cpu_samples_python.clear()
         self.cpu_samples_c.clear()
         self.cpu_utilization.clear()
         self.cpu_samples.clear()
         self.gpu_samples.clear()
@@ -199,28 +210,33 @@
         self.per_line_footprint_samples.clear()
         self.bytei_map.clear()
         # Not clearing current footprint
         # Not clearing max footprint
         # FIXME: leak score, leak velocity
 
     def clear_all(self) -> None:
+        """Clear all statistics."""
         self.clear()
         self.current_footprint = 0
         self.max_footprint = 0
+        self.max_footprint_loc = None
         self.per_line_footprint_samples.clear()
 
     def start_clock(self) -> None:
+        """Start the timer."""
         self.start_time = time.time()
 
     def stop_clock(self) -> None:
+        """Stop the timer."""
         if self.start_time > 0:
             self.elapsed_time += time.time() - self.start_time
         self.start_time = 0
 
     def build_function_stats(self, filename: Filename):  # type: ignore
+        """Produce aggregated statistics for each function."""
         fn_stats = ScaleneStatistics()
         fn_stats.elapsed_time = self.elapsed_time
         fn_stats.total_cpu_samples = self.total_cpu_samples
         fn_stats.total_gpu_samples = self.total_gpu_samples
         fn_stats.total_memory_malloc_samples = self.total_memory_malloc_samples
         first_line_no = LineNumber(1)
         fn_stats.function_map = self.function_map
@@ -282,14 +298,15 @@
             fn_stats.memory_aggregate_footprint[fn_name][
                 first_line_no
             ] += self.memory_aggregate_footprint[filename][line_no]
         return fn_stats
 
     payload_contents = [
         "max_footprint",
+        "max_footprint_loc",
         "current_footprint",
         "elapsed_time",
         "total_cpu_samples",
         "cpu_samples_c",
         "cpu_samples_python",
         "bytei_map",
         "cpu_samples",
@@ -310,22 +327,21 @@
         "memory_malloc_count",
         "memory_free_count",
     ]
     # To be added: __malloc_samples
 
     def output_stats(self, pid: int, dir_name: pathlib.Path) -> None:
         """Output statistics for a particular process to a given directory."""
-        payload: List[Any] = []
-        for n in ScaleneStatistics.payload_contents:
-            payload.append(getattr(self, n))
+        payload: List[Any] = [
+            getattr(self, n) for n in ScaleneStatistics.payload_contents
+        ]
 
         # Create a file in the Python alias directory with the relevant info.
         out_filename = os.path.join(
-            dir_name,
-            "scalene" + str(pid) + "-" + str(os.getpid()),
+            dir_name, f"scalene{pid}-{str(os.getpid())}"
         )
         with open(out_filename, "wb") as out_file:
             cloudpickle.dump(payload, out_file)
 
     @staticmethod
     def increment_per_line_samples(
         dest: Dict[Filename, Dict[LineNumber, T]],
@@ -338,14 +354,15 @@
                 dest[filename][lineno] += v  # type: ignore
 
     @staticmethod
     def increment_cpu_utilization(
         dest: Dict[Filename, Dict[LineNumber, RunningStats]],
         src: Dict[Filename, Dict[LineNumber, RunningStats]],
     ) -> None:
+        """Increment CPU utilization."""
         for filename in src:
             for lineno in src[filename]:
                 dest[filename][lineno] += src[filename][lineno]
 
     def merge_stats(self, the_dir_name: pathlib.Path) -> None:
         """Merge all statistics in a given directory."""
         the_dir = pathlib.Path(the_dir_name)
@@ -355,15 +372,18 @@
                 continue
             with open(f, "rb") as file:
                 unpickler = pickle.Unpickler(file)
                 value = unpickler.load()
                 x = ScaleneStatistics()
                 for i, n in enumerate(ScaleneStatistics.payload_contents):
                     setattr(x, n, value[i])
-                self.max_footprint = max(self.max_footprint, x.max_footprint)
+                # self.max_footprint = max(self.max_footprint, x.max_footprint)
+                if x.max_footprint > self.max_footprint:
+                    self.max_footprint = self.max_footprint
+                    self.max_footprint_loc = x.max_footprint_loc
                 self.current_footprint = max(
                     self.current_footprint, x.current_footprint
                 )
                 self.increment_cpu_utilization(
                     self.cpu_utilization, x.cpu_utilization
                 )
                 self.elapsed_time = max(self.elapsed_time, x.elapsed_time)
```

### Comparing `scalene-1.5.8/scalene/sparkline.py` & `scalene-1.5.9/scalene/sparkline.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ) -> Tuple[float, float, str]:
     all_zeros = all(i == 0 for i in arr)
     if all_zeros:
         return 0, 0, ""
 
     # Prevent negative memory output due to sampling error.
     samples = [i if i > 0 else 0.0 for i in arr]
-    return _create(samples[0 : len(arr)], minimum, maximum)
+    return _create(samples[: len(arr)], minimum, maximum)
 
 
 def _create(
     numbers: List[float],
     fixed_min: Optional[float] = None,
     fixed_max: Optional[float] = None,
 ) -> Tuple[float, float, str]:
```

### Comparing `scalene-1.5.8/scalene.egg-info/PKG-INFO` & `scalene-1.5.9/scalene.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: scalene
-Version: 1.5.8
+Version: 1.5.9
 Summary: Scalene: A high-resolution, low-overhead CPU, GPU, and memory profiler for Python
 Home-page: https://github.com/plasma-umass/scalene
 Author: Emery Berger
 Author-email: emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: performance memory profiler
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![scalene](https://github.com/plasma-umass/scalene/raw/master/docs/scalene-image.png)
 
 # Scalene: a high-performance CPU, GPU and memory profiler for Python
 
 by [Emery Berger](https://emeryberger.com), [Sam Stern](https://samstern.me/), and [Juan Altmayer Pizzorno](https://github.com/jaltmayerpizzorno).
 
-[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
+[![Scalene community Slack](https://github.com/plasma-umass/scalene/raw/master/docs/images/slack-logo.png)](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)[Scalene community Slack](https://join.slack.com/t/scaleneprofil-jge3234/shared_invite/zt-110vzrdck-xJh5d4gHnp5vKXIjYD3Uwg)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/scalene.svg)](https://pypi.org/project/scalene/)[![Downloads](https://pepy.tech/badge/scalene)](https://pepy.tech/project/scalene) [![Downloads](https://pepy.tech/badge/scalene/month)](https://pepy.tech/project/scalene) ![Python versions](https://img.shields.io/pypi/pyversions/scalene.svg?style=flat-square) ![License](https://img.shields.io/github/license/plasma-umass/scalene) [![Twitter Follow](https://img.shields.io/twitter/follow/emeryberger.svg?style=social)](https://twitter.com/emeryberger)
 
 ![Ozsvald tweet](https://github.com/plasma-umass/scalene/raw/master/docs/Ozsvald-tweet.png)
 
 (tweet from Ian Ozsvald, author of [_High Performance Python_](https://smile.amazon.com/High-Performance-Python-Performant-Programming/dp/1492055026/ref=sr_1_1?crid=texbooks))
 
@@ -69,15 +69,16 @@
 
 ```console
 scalene your_prog.py                             # full profile (outputs to web interface)
 python3 -m scalene your_prog.py                  # equivalent alternative
 scalene --cli your_prog.py                       # use the command-line only (no web interface)
 scalene --cpu-only your_prog.py                  # only CPU/GPU
 scalene --reduced-profile your_prog.py           # only profile lines with significant usage
-scalene --profile-interval 5.0 your_prog.py.     # output a new profile every five seconds
+scalene --profile-interval 5.0 your_prog.py      # output a new profile every five seconds
+scalene (Scalene options) --- your_prog.py (...) # use --- to tell Scalene to ignore options after that point
 scalene --help                                   # lists all options
 ```
 
 To use Scalene programmatically in your code, invoke using `scalene` as above and then:
 
 ```Python
 from scalene import scalene_profiler
@@ -364,9 +365,7 @@
 Logo created by [Sophia Berger](https://www.linkedin.com/in/sophia-berger/).
 
 This material is based upon work supported by the National Science
 Foundation under Grant No. 1955610. Any opinions, findings, and
 conclusions or recommendations expressed in this material are those of
 the author(s) and do not necessarily reflect the views of the National
 Science Foundation.
-
-
```

### Comparing `scalene-1.5.8/scalene.egg-info/SOURCES.txt` & `scalene-1.5.9/scalene.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 docs/scalene-image-large.png
 docs/scalene-image-old.png
 docs/scalene-image.png
 docs/scalene-paper.pdf
 docs/images/profiler-comparison.png
 docs/images/sample-profile-pystone.png
 docs/images/scalene-video-img.png
+docs/images/slack-logo.png
 scalene/README.md
 scalene/__init__.py
 scalene/__main__.py
 scalene/adaptive.py
 scalene/profile.py
 scalene/replacement_exit.py
 scalene/replacement_fork.py
@@ -87,18 +88,18 @@
 scalene/scalene-gui/scalene-demo.js
 scalene/scalene-gui/scalene-fetch.js
 scalene/scalene-gui/scalene-gui.js
 scalene/scalene-gui/scalene-image.png
 scalene/scalene-gui/tablesort.js
 scalene/scalene-gui/tablesort.number.js
 src/include/common.hpp
-src/include/libdivide.h
 src/include/lowdiscrepancy.hpp
 src/include/mallocrecursionguard.hpp
 src/include/memcpysampler.hpp
+src/include/pyptr.h
 src/include/pywhere.hpp
 src/include/samplefile.hpp
 src/include/sampleheap.hpp
 src/include/sampleinterval.hpp
 src/include/sampler.hpp
 src/include/scaleneheader.hpp
 src/source/get_line_atomic.cpp
```

### Comparing `scalene-1.5.8/setup.py` & `scalene-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,29 +141,29 @@
         "Topic :: Software Development :: Debuggers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows :: Windows 10"
     ],
     packages=find_packages(),
     cmdclass={
         'bdist_wheel': BdistWheelCommand,
         'egg_info': EggInfoCommand,
         'build_ext': BuildExtCommand,
     },
     install_requires=[
         "rich>=9.2.0",
         "cloudpickle>=1.5.0",
-        "numpy",
         "pynvml>=11.0.0"
     ],
     ext_modules=([get_line_atomic, pywhere] if sys.platform != 'win32' else []),
     setup_requires=['setuptools_scm'],
     include_package_data=True,
     entry_points={"console_scripts": ["scalene = scalene.__main__:main"]},
     python_requires=">=3.8",
```

### Comparing `scalene-1.5.8/src/include/common.hpp` & `scalene-1.5.9/src/include/common.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/lowdiscrepancy.hpp` & `scalene-1.5.9/src/include/lowdiscrepancy.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/mallocrecursionguard.hpp` & `scalene-1.5.9/src/include/mallocrecursionguard.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -5,76 +5,86 @@
 #include <pthread.h>
 
 #include <mutex>
 
 #include "common.hpp"
 
 /**
- * Implements a thread-specific flag to guard against inadventernt recursions
+ * Implements a thread-specific flag to guard against inadvertent recursions
  * when interposing heap functions.
  */
 class MallocRecursionGuard {
   static pthread_key_t* getKey() {
     static pthread_key_t _inMallocKey;
     return &_inMallocKey;
   }
 
-  static bool isInMalloc() {
-    // modified double-checked locking pattern
-    // (https://en.wikipedia.org/wiki/Double-checked_locking)
-    static enum {
+  enum {
       NEEDS_KEY = 0,
       CREATING_KEY = 1,
       DONE = 2
-    } inMallocKeyState{NEEDS_KEY};
+  };
+  
+  static inline bool isInMalloc() {
+    // modified double-checked locking pattern
+    // (https://en.wikipedia.org/wiki/Double-checked_locking)
     static std::recursive_mutex m;
+    static int inMallocKeyState{NEEDS_KEY};
 
     // We create the thread-specific data store the pthread way because the C++
-    // language based ones all seem to fail when interposing on malloc et al, as
+    // language based ones all seem to fail when interposing on malloc et al., as
     // they are invoked early from within library initialization.
 
     auto state = __atomic_load_n(&inMallocKeyState, __ATOMIC_ACQUIRE);
     if (state != DONE) {
-      std::lock_guard<decltype(m)> g{m};
-
-      state = __atomic_load_n(&inMallocKeyState, __ATOMIC_RELAXED);
-      if (unlikely(state == CREATING_KEY)) {
+      if (slowPathInMalloc(m, inMallocKeyState) == CREATING_KEY) {
+        // this happens IFF pthread_key_create allocates memory
         return true;
-      } else if (unlikely(state == NEEDS_KEY)) {
-        __atomic_store_n(&inMallocKeyState, CREATING_KEY, __ATOMIC_RELAXED);
-        if (pthread_key_create(getKey(), 0) !=
-            0) {  // may call malloc/calloc/...
-          abort();
-        }
-        __atomic_store_n(&inMallocKeyState, DONE, __ATOMIC_RELEASE);
       }
     }
 
     return pthread_getspecific(*getKey()) != 0;
   }
 
-  static void setInMalloc(bool state) {
+  static int slowPathInMalloc(std::recursive_mutex& m, int& inMallocKeyState) {
+    std::lock_guard<decltype(m)> g{m};
+    
+    auto state = __atomic_load_n(&inMallocKeyState, __ATOMIC_RELAXED);
+
+    if (unlikely(state == NEEDS_KEY)) {
+      __atomic_store_n(&inMallocKeyState, CREATING_KEY, __ATOMIC_RELAXED);
+      if (pthread_key_create(getKey(), 0) != 0) {  // may call [cm]alloc
+        abort();
+      }
+      __atomic_store_n(&inMallocKeyState, DONE, __ATOMIC_RELEASE);
+      return DONE;
+    }
+
+    return state;
+  }
+  
+  static inline void setInMalloc(bool state) {
     pthread_setspecific(*getKey(), state ? (void*)1 : (void*)0);
   }
 
   bool _wasInMalloc;
 
   MallocRecursionGuard(const MallocRecursionGuard&) = delete;
   MallocRecursionGuard& operator=(const MallocRecursionGuard&) = delete;
 
  public:
-  MallocRecursionGuard() {
+  inline MallocRecursionGuard() {
     if (!(_wasInMalloc = isInMalloc())) {
       setInMalloc(true);
     }
   }
 
-  ~MallocRecursionGuard() {
+  inline ~MallocRecursionGuard() {
     if (!_wasInMalloc) {
       setInMalloc(false);
     }
   }
 
-  bool wasInMalloc() const { return _wasInMalloc; }
+  inline bool wasInMalloc() const { return _wasInMalloc; }
 };
 
 #endif
```

### Comparing `scalene-1.5.8/src/include/memcpysampler.hpp` & `scalene-1.5.9/src/include/memcpysampler.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/pywhere.hpp` & `scalene-1.5.9/src/include/pywhere.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/samplefile.hpp` & `scalene-1.5.9/src/include/samplefile.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/sampleheap.hpp` & `scalene-1.5.9/src/include/sampleheap.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     if (where != nullptr && where(filename, lineno, bytei)) {
       ;
     }
 #endif
 
     writeCount(FreeSignal, sampleFree, nullptr, filename, lineno, bytei);
 #if !SCALENE_DISABLE_SIGNALS
-    raise(FreeSignal);  // was FreeSignal
+    raise(FreeSignal);
 #endif
     freeTriggered()++;
   }
 
  public:
   void* memalign(size_t alignment, size_t sz) {
     MallocRecursionGuard g;
@@ -277,15 +277,15 @@
   void writeCount(AllocSignal sig, uint64_t count, void* ptr,
                   const std::string& filename, int lineno, int bytei) {
     char buf[SampleFile::MAX_BUFSIZE];
     if (_pythonCount == 0) {
       _pythonCount = 1;  // prevent 0/0
     }
     snprintf_(
-        buf, SampleFile::MAX_BUFSIZE,
+        buf, sizeof(buf),
 #if defined(__APPLE__)
         "%c,%llu,%llu,%f,%d,%p,%s,%d,%d\n\n",
 #else
         "%c,%lu,%lu,%f,%d,%p,%s,%d,%d\n\n",
 #endif
         ((sig == MallocSignal) ? 'M' : ((_freedLastMallocTrigger) ? 'f' : 'F')),
         mallocTriggered() + freeTriggered(), count,
```

### Comparing `scalene-1.5.8/src/include/sampleinterval.hpp` & `scalene-1.5.9/src/include/sampleinterval.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/sampler.hpp` & `scalene-1.5.9/src/include/sampler.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/include/scaleneheader.hpp` & `scalene-1.5.9/src/include/scaleneheader.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #else
 extern "C" size_t malloc_usable_size(void *) throw();
 #endif
 #include <assert.h>
 
 #define USE_HEADERS 1
 #define DEBUG_HEADER 0
+
 #if DEBUG_HEADERS
 const int n_padding = 16 - 2 * sizeof(size_t);
 #else
 const int n_padding = 16 - sizeof(size_t);
 #endif
 // Maximum size allocated internally by pymalloc;
 // aka "SMALL_REQUEST_THRESHOLD" in cpython/Objects/obmalloc.c
@@ -50,15 +51,15 @@
 
 #endif
 
   static inline ScaleneHeader *getHeader(void *ptr) {
 #if USE_HEADERS
     return (ScaleneHeader *)ptr - 1;
 #else
-    return (Header *)ptr;
+    return (ScaleneHeader *)ptr;
 #endif
   }
 
   static inline size_t getSize(void *ptr) {
 #if USE_HEADERS
 #if DEBUG_HEADER
     assert(getHeader(ptr)->magic == MAGIC_NUMBER);
@@ -91,8 +92,8 @@
 #if USE_HEADERS
     return (void *)(header + 1);
 #else
     return (void *)header;
 #endif
   }
 };
-#endif
+#endif
```

### Comparing `scalene-1.5.8/src/source/get_line_atomic.cpp` & `scalene-1.5.9/src/source/get_line_atomic.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/src/source/libscalene.cpp` & `scalene-1.5.9/src/source/libscalene.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,14 @@
 // Intercept local allocation for tracking when using the (fast, built-in)
 // pymalloc allocator.
 
 #if !defined(_WIN32)
 
 #include <Python.h>
 
-#define USE_HEADERS 1
-#define DEBUG_HEADER 0
-
 #define DL_FUNCTION(name) \
   static decltype(name) *dl##name = (decltype(name) *)dlsym(RTLD_DEFAULT, #name)
 
 // Maximum size allocated internally by pymalloc;
 // aka "SMALL_REQUEST_THRESHOLD" in cpython/Objects/obmalloc.c
 #define PYMALLOC_MAX_SIZE 512
```

### Comparing `scalene-1.5.8/src/source/pywhere.cpp` & `scalene-1.5.9/src/source/pywhere.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -102,47 +102,43 @@
   GIL() { _gstate = PyGILState_Ensure(); }
   ~GIL() { PyGILState_Release(_gstate); }
 
  private:
   PyGILState_STATE _gstate;
 };
 
-// Implements a mini smart pointer to PyObject.
-// Manages a "strong" reference to the object... to use with a weak reference,
-// Py_IncRef it first. Unfortunately, not all PyObject subclasses (e.g.,
-// PyFrameObject) are declared as such, so we need to make this a template and
-// cast.
-template <class O = PyObject>
-class PyPtr {
- public:
-  PyPtr(O* o) : _obj(o) {}
+#include "pyptr.h"
 
-  O* operator->() { return _obj; }
-
-  operator O*() { return _obj; }
-
-  PyPtr& operator=(O* o) {
-    Py_DecRef((PyObject*)_obj);
-    _obj = o;
-    return *this;
+#if PY_VERSION_HEX < 0x03090000  // new in 3.9
+inline PyFrameObject* PyThreadState_GetFrame(PyThreadState* threadState) {
+  if (threadState != nullptr && threadState->frame != nullptr &&
+      // threadState->frame is a "borrowed" reference.  With Python 3.8.10,
+      // this sometimes refers to a zero-refcount frame that, if we were to
+      // attempt freeing again (when we decrement back to 0), glibc would
+      // abort due to a double free.
+      threadState->frame->ob_base.ob_base.ob_refcnt > 0) {
+    Py_XINCREF(threadState->frame);
+    return threadState->frame;
   }
+  return nullptr;
+}
+inline PyCodeObject* PyFrame_GetCode(PyFrameObject* frame) {
+  Py_XINCREF(frame->f_code);
+  return frame->f_code;
+}
+inline PyFrameObject* PyFrame_GetBack(PyFrameObject* frame) {
+  Py_XINCREF(frame->f_back);
+  return frame->f_back;
+}
+#endif
+#if PY_VERSION_HEX < 0x030B0000  // new in 3.11
+inline int PyFrame_GetLasti(PyFrameObject* frame) { return frame->f_lasti; }
+#endif
 
-  PyPtr& operator=(PyPtr& ptr) {
-    Py_IncRef((PyObject*)ptr._obj);
-    *this = ptr._obj;
-    return *this;
-  }
-
-  ~PyPtr() { Py_DecRef((PyObject*)_obj); }
-
- private:
-  O* _obj;
-};
-
-static PyThreadState* findMainPythonThread() {
+static PyPtr<PyFrameObject> findMainPythonThread_frame() {
   PyThreadState* main = nullptr;
 
   PyThreadState* t = PyInterpreterState_ThreadHead(PyInterpreterState_Main());
   for (; t != nullptr; t = PyThreadState_Next(t)) {
     // Recognize the main thread as the one with the smallest ID.
     // In Juan's experiments, it's the last thread on the list and has id 1.
     //
@@ -152,79 +148,78 @@
     // might go away or change, and thread_id is initialized with the
     // native thread ID of whichever thread creates that PyThreadState.
     if (main == nullptr || main->id > t->id) {
       main = t;
     }
   }
 
-  return main;
+  return PyPtr<PyFrameObject>(main ? PyThreadState_GetFrame(main) : nullptr);
 }
 
 int whereInPython(std::string& filename, int& lineno, int& bytei) {
   if (!Py_IsInitialized()) {  // No python, no python stack.
     return 0;
   }
-
   // This function walks the Python stack until it finds a frame
   // corresponding to a file we are actually profiling. On success,
   // it updates filename, lineno, and byte code index appropriately,
   // and returns 1.  If the stack walk encounters no such file, it
   // sets the filename to the pseudo-filename "<BOGUS>" for special
   // treatment within Scalene, and returns 0.
   filename = "<BOGUS>";
   lineno = 1;
   bytei = 0;
   GIL gil;
 
   PyThreadState* threadState = PyGILState_GetThisThreadState();
-  if (threadState == 0 || threadState->frame == 0) {
+  PyPtr<PyFrameObject> frame =
+      threadState ? PyThreadState_GetFrame(threadState) : nullptr;
+
+  if (frame == nullptr) {
     // Various packages may create native threads; attribute what they do
     // to what the main thread is doing, as it's likely to have requested it.
-    threadState = findMainPythonThread();
-    if (threadState == 0) {
-      return 0;  // No thread, no stack
-    }
+    frame = findMainPythonThread_frame();  // note this may be nullptr
   }
 
   auto traceConfig = TraceConfig::getInstance();
   if (!traceConfig) {
     return 0;
   }
 
-  for (auto frame = threadState->frame; frame != nullptr;
-       frame = frame->f_back) {
-    auto fname = frame->f_code->co_filename;
-    PyPtr<> encoded = PyUnicode_AsASCIIString(fname);
-    if (!encoded) {
+  while (frame != nullptr) {
+    PyPtr<PyCodeObject> code = PyFrame_GetCode(frame);
+    PyPtr<> co_filename = PyUnicode_AsASCIIString(code->co_filename);
+    if (!co_filename) {
       return 0;
     }
 
-    auto filenameStr = PyBytes_AsString(encoded);
+    auto filenameStr = PyBytes_AsString(co_filename);
     if (strlen(filenameStr) == 0) {
       continue;
     }
 
     if (!strstr(filenameStr, "<") && !strstr(filenameStr, "/python") &&
         !strstr(filenameStr, "scalene/scalene")) {
       if (traceConfig->should_trace(filenameStr)) {
 #if defined(PyPy_FatalError)
         // If this macro is defined, we are compiling PyPy, which
         // AFAICT does not have any way to access bytecode index, so
         // we punt and set it to 0.
         bytei = 0;
 #else
-        bytei = frame->f_lasti;
+        bytei = PyFrame_GetLasti(frame);
 #endif
-        lineno = PyCode_Addr2Line(frame->f_code, bytei);
+        lineno = PyFrame_GetLineNumber(frame);
 
         filename = filenameStr;
-        // printf_("FOUND IT: %s %d\n", filenameStr, lineno);
         return 1;
       }
     }
+
+    frame = PyFrame_GetBack(frame);
   }
   return 0;
 }
 
 static PyObject* register_files_to_profile(PyObject* self, PyObject* args) {
   PyObject* a_list;
   PyObject* base_path;
```

### Comparing `scalene-1.5.8/test/issues/test-issue167.py` & `scalene-1.5.9/test/issues/test-issue167.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/multiprocessing_test.py` & `scalene-1.5.9/test/multiprocessing_test.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/new_mp_test.py` & `scalene-1.5.9/test/new_mp_test.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/optimized/bm_pyflate.py` & `scalene-1.5.9/test/optimized/bm_pyflate.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/optimized/bm_raytrace.py` & `scalene-1.5.9/test/optimized/bm_raytrace.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/optimized/bm_richards.py` & `scalene-1.5.9/test/optimized/bm_richards.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/optimized/bm_scimark.py` & `scalene-1.5.9/test/optimized/bm_scimark.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/optimized/bm_spectral_norm.py` & `scalene-1.5.9/test/optimized/bm_spectral_norm.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_mdp.py` & `scalene-1.5.9/test/original/bm_mdp.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_pyflate.py` & `scalene-1.5.9/test/original/bm_pyflate.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_raytrace.py` & `scalene-1.5.9/test/original/bm_raytrace.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_richards.py` & `scalene-1.5.9/test/original/bm_richards.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_scimark.py` & `scalene-1.5.9/test/original/bm_scimark.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_spectral_norm.py` & `scalene-1.5.9/test/original/bm_spectral_norm.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/original/bm_sympy.py` & `scalene-1.5.9/test/original/bm_sympy.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/test-martinheinz.py` & `scalene-1.5.9/test/test-martinheinz.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/test-memory.py` & `scalene-1.5.9/test/test-memory.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/test-pprofile.py` & `scalene-1.5.9/test/test-pprofile.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/test-size.py` & `scalene-1.5.9/test/test-size.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/test_sparkline.py` & `scalene-1.5.9/test/test_sparkline.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/testme.py` & `scalene-1.5.9/test/testme.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/testpyt.py` & `scalene-1.5.9/test/testpyt.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/testtf.py` & `scalene-1.5.9/test/testtf.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/threads-test.py` & `scalene-1.5.9/test/threads-test.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/test/torchtest.py` & `scalene-1.5.9/test/torchtest.py`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/Alexandrescu-memory-allocation.screen.pdf` & `scalene-1.5.9/vendor/Heap-Layers/Alexandrescu-memory-allocation.screen.pdf`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/COPYING` & `scalene-1.5.9/vendor/Heap-Layers/COPYING`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/NOTICE` & `scalene-1.5.9/vendor/Heap-Layers/NOTICE`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/README.md` & `scalene-1.5.9/vendor/Heap-Layers/README.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/cuj-2005-12.pdf` & `scalene-1.5.9/vendor/Heap-Layers/cuj-2005-12.pdf`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/examples/kingsley/compile` & `scalene-1.5.9/vendor/Heap-Layers/examples/kingsley/compile`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/examples/kingsley/libkingsley.cpp` & `scalene-1.5.9/vendor/Heap-Layers/examples/kingsley/libkingsley.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaplayers.h` & `scalene-1.5.9/vendor/Heap-Layers/heaplayers.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/README` & `scalene-1.5.9/vendor/Heap-Layers/heaps/README`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/adaptheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/adaptheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/boundedfreelistheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/boundedfreelistheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/chunkheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/chunkheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/coalesceheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/coalesceheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/buildingblock/freelistheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/buildingblock/freelistheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/combining/hybridheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/combining/hybridheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/combining/segheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/combining/segheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/combining/strictsegheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/combining/strictsegheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/combining/tryheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/combining/tryheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/debug/checkheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/debug/checkheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/debug/debugheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/debug/debugheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/debug/logheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/debug/logheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/debug/sanitycheckheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/debug/sanitycheckheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/debug/statsheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/debug/statsheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/general/dlheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/general/dlheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/general/kingsleyheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/general/kingsleyheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/general/leamallocheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/general/leamallocheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/general/oldkingsleyheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/general/oldkingsleyheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/addheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/addheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/coalesceableheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/coalesceableheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/sizeheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/sizeheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/objectrep/sizeownerheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/objectrep/sizeownerheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/bumpalloc.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/bumpalloc.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/nestedheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/nestedheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstack.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstack.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstackheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstackheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/obstackreap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/obstackreap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/sbrk.c` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/sbrk.c`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/xallocheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/xallocheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/special/zoneheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/special/zoneheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/threads/lockedheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/threads/lockedheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/threads/phothreadheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/threads/phothreadheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/threads/sizethreadheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/threads/sizethreadheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/threads/threadheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/threads/threadheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/threads/threadspecificheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/threads/threadspecificheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/top/mallocheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/top/mallocheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/top/mmapheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/top/mmapheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/top/staticbufferheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/top/staticbufferheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/top/staticheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/top/staticheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/exactlyoneheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/exactlyoneheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/exceptionheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/exceptionheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/nullheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/nullheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/old/oneheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/old/oneheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/oneheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/oneheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/perclassheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/perclassheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/profileheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/profileheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/slopheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/slopheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/sysmallocheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/sysmallocheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/traceheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/traceheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/heaps/utility/uniqueheap.h` & `scalene-1.5.9/vendor/Heap-Layers/heaps/utility/uniqueheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/README` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/README`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/addheader.h` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/addheader.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/clearoptimizeheap.h` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/clearoptimizeheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/compile` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/compile`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/libreap.cpp` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/libreap.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/reap.h` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/reap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionheap.cpp` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionheap.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionheap.h` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionheap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionsimulator.cpp` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionsimulator.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/legacy/reap/regionsimulator.h` & `scalene-1.5.9/vendor/Heap-Layers/legacy/reap/regionsimulator.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/maclock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/maclock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/oldspinlock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/oldspinlock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/posixlock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/posixlock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/recursivelock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/recursivelock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/spinlock-old.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/spinlock-old.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/spinlock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/spinlock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/locks/winlock.h` & `scalene-1.5.9/vendor/Heap-Layers/locks/winlock.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/threads/cpuinfo.cpp` & `scalene-1.5.9/vendor/Heap-Layers/threads/cpuinfo.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/threads/cpuinfo.h` & `scalene-1.5.9/vendor/Heap-Layers/threads/cpuinfo.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/threads/fred.h` & `scalene-1.5.9/vendor/Heap-Layers/threads/fred.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/align.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/align.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/bins.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/bins.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/bins16k.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/bins16k.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/bins4k.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/bins4k.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/bins64k.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/bins64k.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/bins8k.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/bins8k.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/binspow2.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/binspow2.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/checkpoweroftwo.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/checkpoweroftwo.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/dllist.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/dllist.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/dynarray.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/dynarray.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/exactlyone.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/exactlyone.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/freesllist.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/freesllist.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/hash.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/hash.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/ilog2.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/ilog2.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/istrue.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/istrue.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/modulo.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/modulo.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/myhashmap.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/myhashmap.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/singleton.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/singleton.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/sllist.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/sllist.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/timer-old.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/timer-old.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/timer.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/timer.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/utility/tprintf.h` & `scalene-1.5.9/vendor/Heap-Layers/utility/tprintf.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/ansiwrapper.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/ansiwrapper.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/generic-memalign.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/generic-memalign.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/gnuwrapper-hooks.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/gnuwrapper-hooks.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/gnuwrapper.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/gnuwrapper.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/heapredirect.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/heapredirect.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/macwrapper.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/macwrapper.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/mallocinfo.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/mallocinfo.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/mmapwrapper.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/mmapwrapper.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/stlallocator.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/stlallocator.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/winwrapper.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/winwrapper.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/wrapper.cpp` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/Heap-Layers/wrappers/x86jump.h` & `scalene-1.5.9/vendor/Heap-Layers/wrappers/x86jump.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/.travis.yml` & `scalene-1.5.9/vendor/printf/.travis.yml`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/LICENSE` & `scalene-1.5.9/vendor/printf/LICENSE`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/Makefile` & `scalene-1.5.9/vendor/printf/Makefile`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/README.md` & `scalene-1.5.9/vendor/printf/README.md`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/printf.c` & `scalene-1.5.9/vendor/printf/printf.c`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/printf.cpp` & `scalene-1.5.9/vendor/printf/printf.cpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/printf.h` & `scalene-1.5.9/vendor/printf/printf.h`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/test/catch.hpp` & `scalene-1.5.9/vendor/printf/test/catch.hpp`

 * *Files identical despite different names*

### Comparing `scalene-1.5.8/vendor/printf/test/test_suite.cpp` & `scalene-1.5.9/vendor/printf/test/test_suite.cpp`

 * *Files identical despite different names*

