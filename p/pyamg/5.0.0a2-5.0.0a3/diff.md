# Comparing `tmp/pyamg-5.0.0a2.tar.gz` & `tmp/pyamg-5.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyamg-5.0.0a2.tar", last modified: Mon Apr 17 17:33:49 2023, max compression
+gzip compressed data, was "pyamg-5.0.0a3.tar", last modified: Mon Apr 17 18:05:15 2023, max compression
```

## Comparing `pyamg-5.0.0a2.tar` & `pyamg-5.0.0a3.tar`

### file list

```diff
@@ -1,226 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.605206 pyamg-5.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.513204 pyamg-5.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.533204 pyamg-5.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/.github/workflows/draft-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/DEVELOPERS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-17 17:33:49.605206 pyamg-5.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/README-DEV.md
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.533204 pyamg-5.0.0a2/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/bench/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.533204 pyamg-5.0.0a2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.533204 pyamg-5.0.0a2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/dev/common_docstring.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/dev/todo.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.541204 pyamg-5.0.0a2/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   116340 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg.mat
--rw-r--r--   0 runner    (1001) docker     (123)   119706 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)  1352508 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)   139020 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo_legacy.png
--rw-r--r--   0 runner    (1001) docker     (123)    66612 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo_legacy_withtext.png
--rw-r--r--   0 runner    (1001) docker     (123)   128585 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo_withtext.pdf
--rw-r--r--   0 runner    (1001) docker     (123)  1394824 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/logo/pyamg_logo_withtext.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.545204 pyamg-5.0.0a2/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)   193617 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/example.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/example.res.txt
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/example_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.545204 pyamg-5.0.0a2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/source/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.545204 pyamg-5.0.0a2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/source/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/docs/source/ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/organization.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.549204 pyamg-5.0.0a2/pyamg/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.553204 pyamg-5.0.0a2/pyamg/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32213 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/rootnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    43814 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tentative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.557205 pyamg-5.0.0a2/pyamg/aggregation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    25350 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_rootnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/aggregation/tests/test_tentative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.565205 pyamg-5.0.0a2/pyamg/amg_core/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/air.h
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/air_bind.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    10873 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/bindthem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/evolution_strength.h
--rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/evolution_strength_bind.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/generate.sh
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/graph-todo.md
--rw-r--r--   0 runner    (1001) docker     (123)    35419 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    26682 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/graph_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/instantiate.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/krylov.h
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/krylov_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    40809 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/linalg.h
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/linalg_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    42003 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/relaxation.h
--rw-r--r--   0 runner    (1001) docker     (123)    52289 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/relaxation_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41358 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/ruge_stuben.h
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/ruge_stuben_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35214 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/smoothed_aggregation.h
--rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/smoothed_aggregation_bind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.569205 pyamg-5.0.0a2/pyamg/amg_core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/tests/bind_examples.h
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/tests/bind_examples_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/tests/instantiate-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/amg_core/tests/test_bind_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/citation.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.569205 pyamg-5.0.0a2/pyamg/classical/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/air.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/classical.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/cr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.573205 pyamg-5.0.0a2/pyamg/classical/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/tests/test_air.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/tests/test_classical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/classical/tests/test_cr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.577205 pyamg-5.0.0a2/pyamg/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/advection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.581205 pyamg-5.0.0a2/pyamg/gallery/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/airfoil.mat
--rw-r--r--   0 runner    (1001) docker     (123)    42144 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/bar.mat
--rw-r--r--   0 runner    (1001) docker     (123)   164770 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/helmholtz_2D.mat
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/knot.mat
--rw-r--r--   0 runner    (1001) docker     (123)   446800 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat
--rw-r--r--   0 runner    (1001) docker     (123)    30384 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/recirc_flow.mat
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/unit_cube.mat
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/example_data/unit_square.mat
--rw-r--r--   0 runner    (1001) docker     (123)    28444 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.581205 pyamg-5.0.0a2/pyamg/gallery/mesh_data/
--rw-r--r--   0 runner    (1001) docker     (123)    22998 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/mesh_data/square_mesh.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/random_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/stencil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.581205 pyamg-5.0.0a2/pyamg/gallery/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_advection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/gallery/tests/test_stencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/graph_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/krylov/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_bicgstab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_cgne.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_cgnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_cr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_fgmres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_gmres.py
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_gmres_householder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_gmres_mgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_minimal_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/_steepest_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/krylov/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/tests/test_krylov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/krylov/tests/test_simple_iterations.py
--rw-r--r--   0 runner    (1001) docker     (123)    28777 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/multilevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/relaxation/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (123)    49080 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33487 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/relaxation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71883 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/tests/test_relaxation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/relaxation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/strength.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_amg_core_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_multilevel.py
--rw-r--r--   0 runner    (1001) docker     (123)    35201 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/tests/test_strength.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/util/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/bsr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/tests/test_bsr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    63523 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/tests/test_warn.py
--rw-r--r--   0 runner    (1001) docker     (123)    71144 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.601205 pyamg-5.0.0a2/pyamg/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.605206 pyamg-5.0.0a2/pyamg/vis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/tests/test_vtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/vis_coarse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyamg/vis/vtk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:49.549204 pyamg-5.0.0a2/pyamg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 17:33:49.000000 pyamg-5.0.0a2/pyamg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-17 17:33:49.605206 pyamg-5.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-04-17 17:33:43.000000 pyamg-5.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.625928 pyamg-5.0.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.649928 pyamg-5.0.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/DEVELOPERS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/README-DEV.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.649928 pyamg-5.0.0a3/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/bench/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.649928 pyamg-5.0.0a3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.649928 pyamg-5.0.0a3/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/dev/common_docstring.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/dev/todo.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.657929 pyamg-5.0.0a3/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   116340 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   119706 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1352508 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139020 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo_legacy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66612 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo_legacy_withtext.png
+-rw-r--r--   0 runner    (1001) docker     (123)   128585 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo_withtext.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1394824 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/logo/pyamg_logo_withtext.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.661929 pyamg-5.0.0a3/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193617 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/example.res.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/example_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.665929 pyamg-5.0.0a3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/source/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.665929 pyamg-5.0.0a3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/source/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/docs/source/ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/organization.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.669929 pyamg-5.0.0a3/pyamg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.677929 pyamg-5.0.0a3/pyamg/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32213 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/rootnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43814 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tentative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.681930 pyamg-5.0.0a3/pyamg/aggregation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25350 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_rootnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/aggregation/tests/test_tentative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.693930 pyamg-5.0.0a3/pyamg/amg_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/air.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/air_bind.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10873 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/bindthem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/evolution_strength.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/evolution_strength_bind.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/graph-todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35419 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26682 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/graph_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/instantiate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/krylov.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/krylov_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    40809 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/linalg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/linalg_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42003 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/relaxation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52289 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/relaxation_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    41358 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/ruge_stuben.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/ruge_stuben_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35214 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/smoothed_aggregation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/smoothed_aggregation_bind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.693930 pyamg-5.0.0a3/pyamg/amg_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/tests/bind_examples.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/tests/bind_examples_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/tests/instantiate-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/amg_core/tests/test_bind_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/citation.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.697930 pyamg-5.0.0a3/pyamg/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/air.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/classical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/cr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.697930 pyamg-5.0.0a3/pyamg/classical/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/tests/test_air.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/tests/test_classical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/classical/tests/test_cr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.705931 pyamg-5.0.0a3/pyamg/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/advection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.709931 pyamg-5.0.0a3/pyamg/gallery/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/airfoil.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    42144 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/bar.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   164770 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/helmholtz_2D.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/knot.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   446800 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    30384 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/recirc_flow.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/unit_cube.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/example_data/unit_square.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    28444 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.709931 pyamg-5.0.0a3/pyamg/gallery/mesh_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22998 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/mesh_data/square_mesh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/random_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/stencil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.713931 pyamg-5.0.0a3/pyamg/gallery/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_advection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/gallery/tests/test_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/graph_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.721931 pyamg-5.0.0a3/pyamg/krylov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_bicgstab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_cgne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_cgnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_cr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_fgmres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_gmres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_gmres_householder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_gmres_mgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_minimal_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/_steepest_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.721931 pyamg-5.0.0a3/pyamg/krylov/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/tests/test_krylov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/krylov/tests/test_simple_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28777 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/multilevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.725931 pyamg-5.0.0a3/pyamg/relaxation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49080 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33487 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.725931 pyamg-5.0.0a3/pyamg/relaxation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71883 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/relaxation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/strength.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/pyamg/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_amg_core_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_multilevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35201 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/tests/test_strength.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/pyamg/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/bsr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/pyamg/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/tests/test_bsr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63523 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/tests/test_warn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71144 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/pyamg/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/pyamg/vis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/tests/test_vtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/vis_coarse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyamg/vis/vtk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:05:15.673929 pyamg-5.0.0a3/pyamg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 18:05:15.000000 pyamg-5.0.0a3/pyamg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-17 18:05:15.729931 pyamg-5.0.0a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-04-17 18:05:09.000000 pyamg-5.0.0a3/setup.py
```

### Comparing `pyamg-5.0.0a2/.github/workflows/ci.yml` & `pyamg-5.0.0a3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/.github/workflows/draft-pdf.yml` & `pyamg-5.0.0a3/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/.github/workflows/lint.yml` & `pyamg-5.0.0a3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/.github/workflows/wheels.yml` & `pyamg-5.0.0a3/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/.readthedocs.yml` & `pyamg-5.0.0a3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/CONTRIBUTING.md` & `pyamg-5.0.0a3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/LICENSE.txt` & `pyamg-5.0.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/PKG-INFO` & `pyamg-5.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamg
-Version: 5.0.0a2
+Version: 5.0.0a3
 Summary: PyAMG: Algebraic Multigrid Solvers in Python
 Home-page: https://github.com/pyamg/pyamg
 Download-URL: https://github.com/pyamg/pyamg/releases
 Author: Nathan Bell, Luke Olson, and Jacob Schroder
 Author-email: luke.olson@gmail.com
 Maintainer: Luke Olson
 Maintainer-email: luke.olson@gmail.com
```

### Comparing `pyamg-5.0.0a2/README-DEV.md` & `pyamg-5.0.0a3/README-DEV.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/README.md` & `pyamg-5.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/changelog.md` & `pyamg-5.0.0a3/changelog.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/Makefile` & `pyamg-5.0.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/dev/common_docstring.md` & `pyamg-5.0.0a3/docs/dev/common_docstring.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/dev/todo.md` & `pyamg-5.0.0a3/docs/dev/todo.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg.mat` & `pyamg-5.0.0a3/docs/logo/pyamg.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo.pdf` & `pyamg-5.0.0a3/docs/logo/pyamg_logo.pdf`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo.png` & `pyamg-5.0.0a3/docs/logo/pyamg_logo.png`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo.py` & `pyamg-5.0.0a3/docs/logo/pyamg_logo.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo_legacy.png` & `pyamg-5.0.0a3/docs/logo/pyamg_logo_legacy.png`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo_legacy_withtext.png` & `pyamg-5.0.0a3/docs/logo/pyamg_logo_legacy_withtext.png`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo_withtext.pdf` & `pyamg-5.0.0a3/docs/logo/pyamg_logo_withtext.pdf`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/logo/pyamg_logo_withtext.png` & `pyamg-5.0.0a3/docs/logo/pyamg_logo_withtext.png`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/common.py` & `pyamg-5.0.0a3/docs/paper/common.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/example.pdf` & `pyamg-5.0.0a3/docs/paper/example.pdf`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/example.res.txt` & `pyamg-5.0.0a3/docs/paper/example.res.txt`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/example_plot.py` & `pyamg-5.0.0a3/docs/paper/example_plot.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/paper.bib` & `pyamg-5.0.0a3/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/paper/paper.md` & `pyamg-5.0.0a3/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/source/README.md` & `pyamg-5.0.0a3/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/source/_static/default.css` & `pyamg-5.0.0a3/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/source/conf.py` & `pyamg-5.0.0a3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/docs/source/ref.rst` & `pyamg-5.0.0a3/docs/source/ref.rst`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/organization.md` & `pyamg-5.0.0a3/organization.md`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/__init__.py` & `pyamg-5.0.0a3/pyamg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/__init__.py` & `pyamg-5.0.0a3/pyamg/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/adaptive.py` & `pyamg-5.0.0a3/pyamg/aggregation/adaptive.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/aggregate.py` & `pyamg-5.0.0a3/pyamg/aggregation/aggregate.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/aggregation.py` & `pyamg-5.0.0a3/pyamg/aggregation/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/pairwise.py` & `pyamg-5.0.0a3/pyamg/aggregation/pairwise.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/rootnode.py` & `pyamg-5.0.0a3/pyamg/aggregation/rootnode.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/smooth.py` & `pyamg-5.0.0a3/pyamg/aggregation/smooth.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tentative.py` & `pyamg-5.0.0a3/pyamg/aggregation/tentative.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_adaptive.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_aggregate.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_aggregation.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_pairwise.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_pairwise.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_rootnode.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_rootnode.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_smooth.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/aggregation/tests/test_tentative.py` & `pyamg-5.0.0a3/pyamg/aggregation/tests/test_tentative.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/__init__.py` & `pyamg-5.0.0a3/pyamg/amg_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/air.h` & `pyamg-5.0.0a3/pyamg/amg_core/air.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/air_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/air_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/bindthem.py` & `pyamg-5.0.0a3/pyamg/amg_core/bindthem.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/build.sh` & `pyamg-5.0.0a3/pyamg/amg_core/build.sh`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/evolution_strength.h` & `pyamg-5.0.0a3/pyamg/amg_core/evolution_strength.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/evolution_strength_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/evolution_strength_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/graph.h` & `pyamg-5.0.0a3/pyamg/amg_core/graph.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/graph_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/graph_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/instantiate.yml` & `pyamg-5.0.0a3/pyamg/amg_core/instantiate.yml`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/krylov.h` & `pyamg-5.0.0a3/pyamg/amg_core/krylov.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/krylov_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/krylov_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/linalg.h` & `pyamg-5.0.0a3/pyamg/amg_core/linalg.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/linalg_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/linalg_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/relaxation.h` & `pyamg-5.0.0a3/pyamg/amg_core/relaxation.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/relaxation_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/relaxation_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/ruge_stuben.h` & `pyamg-5.0.0a3/pyamg/amg_core/ruge_stuben.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/ruge_stuben_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/ruge_stuben_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/smoothed_aggregation.h` & `pyamg-5.0.0a3/pyamg/amg_core/smoothed_aggregation.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/smoothed_aggregation_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/smoothed_aggregation_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/tests/bind_examples.h` & `pyamg-5.0.0a3/pyamg/amg_core/tests/bind_examples.h`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/tests/bind_examples_bind.cpp` & `pyamg-5.0.0a3/pyamg/amg_core/tests/bind_examples_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/amg_core/tests/test_bind_examples.py` & `pyamg-5.0.0a3/pyamg/amg_core/tests/test_bind_examples.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/blackbox.py` & `pyamg-5.0.0a3/pyamg/blackbox.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/air.py` & `pyamg-5.0.0a3/pyamg/classical/air.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/classical.py` & `pyamg-5.0.0a3/pyamg/classical/classical.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/cr.py` & `pyamg-5.0.0a3/pyamg/classical/cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/interpolate.py` & `pyamg-5.0.0a3/pyamg/classical/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/split.py` & `pyamg-5.0.0a3/pyamg/classical/split.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/tests/test_air.py` & `pyamg-5.0.0a3/pyamg/classical/tests/test_air.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/tests/test_classical.py` & `pyamg-5.0.0a3/pyamg/classical/tests/test_classical.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/classical/tests/test_cr.py` & `pyamg-5.0.0a3/pyamg/classical/tests/test_cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/__init__.py` & `pyamg-5.0.0a3/pyamg/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/advection.py` & `pyamg-5.0.0a3/pyamg/gallery/advection.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/demo.py` & `pyamg-5.0.0a3/pyamg/gallery/demo.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/diffusion.py` & `pyamg-5.0.0a3/pyamg/gallery/diffusion.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/elasticity.py` & `pyamg-5.0.0a3/pyamg/gallery/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example.py` & `pyamg-5.0.0a3/pyamg/gallery/example.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/README.txt` & `pyamg-5.0.0a3/pyamg/gallery/example_data/README.txt`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/airfoil.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/airfoil.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/bar.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/bar.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/helmholtz_2D.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/helmholtz_2D.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/knot.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/knot.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/recirc_flow.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/recirc_flow.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/unit_cube.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/unit_cube.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/example_data/unit_square.mat` & `pyamg-5.0.0a3/pyamg/gallery/example_data/unit_square.mat`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/fem.py` & `pyamg-5.0.0a3/pyamg/gallery/fem.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/laplacian.py` & `pyamg-5.0.0a3/pyamg/gallery/laplacian.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/mesh.py` & `pyamg-5.0.0a3/pyamg/gallery/mesh.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/mesh_data/square_mesh.npz` & `pyamg-5.0.0a3/pyamg/gallery/mesh_data/square_mesh.npz`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/random_sparse.py` & `pyamg-5.0.0a3/pyamg/gallery/random_sparse.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/stencil.py` & `pyamg-5.0.0a3/pyamg/gallery/stencil.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_advection.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_advection.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_diffusion.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_elasticity.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_elasticity.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_example.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_fem.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_fem.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_laplacian.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_mesh.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/gallery/tests/test_stencil.py` & `pyamg-5.0.0a3/pyamg/gallery/tests/test_stencil.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/graph.py` & `pyamg-5.0.0a3/pyamg/graph.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/graph_ref.py` & `pyamg-5.0.0a3/pyamg/graph_ref.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/__init__.py` & `pyamg-5.0.0a3/pyamg/krylov/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_bicgstab.py` & `pyamg-5.0.0a3/pyamg/krylov/_bicgstab.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_cg.py` & `pyamg-5.0.0a3/pyamg/krylov/_cg.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_cgne.py` & `pyamg-5.0.0a3/pyamg/krylov/_cgne.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_cgnr.py` & `pyamg-5.0.0a3/pyamg/krylov/_cgnr.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_cr.py` & `pyamg-5.0.0a3/pyamg/krylov/_cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_fgmres.py` & `pyamg-5.0.0a3/pyamg/krylov/_fgmres.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_gmres.py` & `pyamg-5.0.0a3/pyamg/krylov/_gmres.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_gmres_householder.py` & `pyamg-5.0.0a3/pyamg/krylov/_gmres_householder.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_gmres_mgs.py` & `pyamg-5.0.0a3/pyamg/krylov/_gmres_mgs.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_minimal_residual.py` & `pyamg-5.0.0a3/pyamg/krylov/_minimal_residual.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/_steepest_descent.py` & `pyamg-5.0.0a3/pyamg/krylov/_steepest_descent.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/tests/test_krylov.py` & `pyamg-5.0.0a3/pyamg/krylov/tests/test_krylov.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/tests/test_scipy.py` & `pyamg-5.0.0a3/pyamg/krylov/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/krylov/tests/test_simple_iterations.py` & `pyamg-5.0.0a3/pyamg/krylov/tests/test_simple_iterations.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/multilevel.py` & `pyamg-5.0.0a3/pyamg/multilevel.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/__init__.py` & `pyamg-5.0.0a3/pyamg/relaxation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/chebyshev.py` & `pyamg-5.0.0a3/pyamg/relaxation/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/relaxation.py` & `pyamg-5.0.0a3/pyamg/relaxation/relaxation.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/smoothing.py` & `pyamg-5.0.0a3/pyamg/relaxation/smoothing.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/tests/test_relaxation.py` & `pyamg-5.0.0a3/pyamg/relaxation/tests/test_relaxation.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/tests/test_smoothing.py` & `pyamg-5.0.0a3/pyamg/relaxation/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/relaxation/utils.py` & `pyamg-5.0.0a3/pyamg/relaxation/utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/strength.py` & `pyamg-5.0.0a3/pyamg/strength.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_amg_core_linalg.py` & `pyamg-5.0.0a3/pyamg/tests/test_amg_core_linalg.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_blackbox.py` & `pyamg-5.0.0a3/pyamg/tests/test_blackbox.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_clustering.py` & `pyamg-5.0.0a3/pyamg/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_graph.py` & `pyamg-5.0.0a3/pyamg/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_multilevel.py` & `pyamg-5.0.0a3/pyamg/tests/test_multilevel.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/tests/test_strength.py` & `pyamg-5.0.0a3/pyamg/tests/test_strength.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/bsr_utils.py` & `pyamg-5.0.0a3/pyamg/util/bsr_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/linalg.py` & `pyamg-5.0.0a3/pyamg/util/linalg.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/params.py` & `pyamg-5.0.0a3/pyamg/util/params.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/tests/test_bsr_utils.py` & `pyamg-5.0.0a3/pyamg/util/tests/test_bsr_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/tests/test_linalg.py` & `pyamg-5.0.0a3/pyamg/util/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/tests/test_utils.py` & `pyamg-5.0.0a3/pyamg/util/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/util/utils.py` & `pyamg-5.0.0a3/pyamg/util/utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/vis/tests/test_vis.py` & `pyamg-5.0.0a3/pyamg/vis/tests/test_vis.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/vis/tests/test_vtu.py` & `pyamg-5.0.0a3/pyamg/vis/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/vis/vis_coarse.py` & `pyamg-5.0.0a3/pyamg/vis/vis_coarse.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg/vis/vtk_writer.py` & `pyamg-5.0.0a3/pyamg/vis/vtk_writer.py`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/pyamg.egg-info/PKG-INFO` & `pyamg-5.0.0a3/pyamg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamg
-Version: 5.0.0a2
+Version: 5.0.0a3
 Summary: PyAMG: Algebraic Multigrid Solvers in Python
 Home-page: https://github.com/pyamg/pyamg
 Download-URL: https://github.com/pyamg/pyamg/releases
 Author: Nathan Bell, Luke Olson, and Jacob Schroder
 Author-email: luke.olson@gmail.com
 Maintainer: Luke Olson
 Maintainer-email: luke.olson@gmail.com
```

### Comparing `pyamg-5.0.0a2/pyamg.egg-info/SOURCES.txt` & `pyamg-5.0.0a3/pyamg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.git_archival.txt
+.gitattributes
 .readthedocs.yml
 CITATION.bib
 CITATION.cff
 CONTRIBUTING.md
 DEVELOPERS.txt
 LICENSE.txt
 MANIFEST.in
```

### Comparing `pyamg-5.0.0a2/setup.cfg` & `pyamg-5.0.0a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyamg-5.0.0a2/setup.py` & `pyamg-5.0.0a3/setup.py`

 * *Files identical despite different names*

