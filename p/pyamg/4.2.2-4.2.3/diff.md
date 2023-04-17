# Comparing `tmp/pyamg-4.2.2.tar.gz` & `tmp/pyamg-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyamg-4.2.2.tar", last modified: Sun Feb  6 22:53:38 2022, max compression
+gzip compressed data, was "pyamg-4.2.3.tar", last modified: Fri Apr 15 16:47:24 2022, max compression
```

## Comparing `pyamg-4.2.2.tar` & `pyamg-4.2.3.tar`

### file list

```diff
@@ -1,203 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.508840 pyamg-4.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.508840 pyamg-4.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-02-06 22:53:31.000000 pyamg-4.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-02-06 22:53:31.000000 pyamg-4.2.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-02-06 22:53:31.000000 pyamg-4.2.2/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-02-06 22:53:31.000000 pyamg-4.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-06 22:53:31.000000 pyamg-4.2.2/DEVELOPERS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-02-06 22:53:31.000000 pyamg-4.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-02-06 22:53:31.000000 pyamg-4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-02-06 22:53:38.524840 pyamg-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-06 22:53:31.000000 pyamg-4.2.2/README-DEV.md
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-02-06 22:53:31.000000 pyamg-4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.508840 pyamg-4.2.2/bench/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-02-06 22:53:31.000000 pyamg-4.2.2/bench/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-02-06 22:53:31.000000 pyamg-4.2.2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.508840 pyamg-4.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.512841 pyamg-4.2.2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/dev/common_docstring.md
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/dev/todo.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.512841 pyamg-4.2.2/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)   116340 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg.mat
--rw-r--r--   0 runner    (1001) docker     (121)   119706 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo.pdf
--rw-r--r--   0 runner    (1001) docker     (121)  1352508 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo.py
--rw-r--r--   0 runner    (1001) docker     (121)   139020 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo_legacy.png
--rw-r--r--   0 runner    (1001) docker     (121)    66612 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo_legacy_withtext.png
--rw-r--r--   0 runner    (1001) docker     (121)   128585 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo_withtext.pdf
--rw-r--r--   0 runner    (1001) docker     (121)  1394824 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/logo/pyamg_logo_withtext.png
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/source/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     9832 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/source/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-02-06 22:53:31.000000 pyamg-4.2.2/docs/source/ref.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/pyamg/
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/pyamg/aggregation/
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32212 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (121)    10316 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)    18076 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    20086 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/rootnode.py
--rw-r--r--   0 runner    (1001) docker     (121)    43826 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/smooth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tentative.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/pyamg/aggregation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7241 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)    25370 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    22546 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_rootnode.py
--rw-r--r--   0 runner    (1001) docker     (121)    31886 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (121)     8820 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/aggregation/tests/test_tentative.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/amg_core/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10873 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/bindthem.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1241 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)    23657 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/evolution_strength.h
--rw-r--r--   0 runner    (1001) docker     (121)    18576 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/evolution_strength_bind.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)      195 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/generate.sh
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/graph-todo.md
--rw-r--r--   0 runner    (1001) docker     (121)    35474 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/graph.h
--rw-r--r--   0 runner    (1001) docker     (121)    27049 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/graph_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/instantiate.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/krylov.h
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/krylov_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    28784 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/linalg.h
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/linalg_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    32789 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/relaxation.h
--rw-r--r--   0 runner    (1001) docker     (121)    42887 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/relaxation_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    41514 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/ruge_stuben.h
--rw-r--r--   0 runner    (1001) docker     (121)    18962 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/ruge_stuben_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    31262 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/smoothed_aggregation.h
--rw-r--r--   0 runner    (1001) docker     (121)    23482 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/smoothed_aggregation_bind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/amg_core/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/tests/bind_examples.h
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/tests/bind_examples_bind.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/tests/instantiate-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/amg_core/tests/test_bind_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/citation.bib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/classical/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6670 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/classical.py
--rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/cr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)    13027 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/split.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/classical/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7685 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/tests/test_classical.py
--rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/classical/tests/test_cr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/gallery/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     9794 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/elasticity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/gallery/example_data/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19027 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/airfoil.mat
--rw-r--r--   0 runner    (1001) docker     (121)    42144 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/bar.mat
--rw-r--r--   0 runner    (1001) docker     (121)   164770 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/helmholtz_2D.mat
--rw-r--r--   0 runner    (1001) docker     (121)     8446 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/knot.mat
--rw-r--r--   0 runner    (1001) docker     (121)   446800 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat
--rw-r--r--   0 runner    (1001) docker     (121)    30384 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/recirc_flow.mat
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/unit_cube.mat
--rw-r--r--   0 runner    (1001) docker     (121)    14035 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/example_data/unit_square.mat
--rw-r--r--   0 runner    (1001) docker     (121)    27584 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/fem.py
--rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.520841 pyamg-4.2.2/pyamg/gallery/mesh_data/
--rw-r--r--   0 runner    (1001) docker     (121)    22998 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/mesh_data/square_mesh.npz
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/random_sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/stencil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/gallery/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     7759 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_fem.py
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/gallery/tests/test_stencil.py
--rw-r--r--   0 runner    (1001) docker     (121)    10552 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/graph_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/krylov/
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_bicgstab.py
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_cg.py
--rw-r--r--   0 runner    (1001) docker     (121)     6562 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_cgne.py
--rw-r--r--   0 runner    (1001) docker     (121)     6615 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_cgnr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_cr.py
--rw-r--r--   0 runner    (1001) docker     (121)    12564 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_fgmres.py
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_gmres.py
--rw-r--r--   0 runner    (1001) docker     (121)    13004 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_gmres_householder.py
--rw-r--r--   0 runner    (1001) docker     (121)    11072 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_gmres_mgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_minimal_residual.py
--rw-r--r--   0 runner    (1001) docker     (121)     5954 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/_steepest_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/krylov/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11672 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/tests/test_krylov.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7480 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/krylov/tests/test_simple_iterations.py
--rw-r--r--   0 runner    (1001) docker     (121)    27490 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/multilevel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/relaxation/
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (121)    37505 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (121)    24568 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/relaxation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    64489 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/tests/test_relaxation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/relaxation/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    34522 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/strength.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/test_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (121)    14855 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)    15177 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/test_multilevel.py
--rw-r--r--   0 runner    (1001) docker     (121)    32602 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/tests/test_strength.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/util/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/bsr_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    18547 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/linalg.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/params.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/util/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/tests/test_bsr_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13136 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (121)    61192 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/tests/test_warn.py
--rw-r--r--   0 runner    (1001) docker     (121)    69511 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/vis/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.524840 pyamg-4.2.2/pyamg/vis/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3279 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/tests/test_vtu.py
--rw-r--r--   0 runner    (1001) docker     (121)     9747 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/vis_coarse.py
--rw-r--r--   0 runner    (1001) docker     (121)    16162 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyamg/vis/vtk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 22:53:38.516841 pyamg-4.2.2/pyamg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-06 22:53:38.000000 pyamg-4.2.2/pyamg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-06 22:53:31.000000 pyamg-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-06 22:53:31.000000 pyamg-4.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-06 22:53:31.000000 pyamg-4.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-02-06 22:53:38.528840 pyamg-4.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1299 2022-02-06 22:53:31.000000 pyamg-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.665343 pyamg-4.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.665343 pyamg-4.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-04-15 16:47:15.000000 pyamg-4.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-04-15 16:47:15.000000 pyamg-4.2.3/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-04-15 16:47:15.000000 pyamg-4.2.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-04-15 16:47:15.000000 pyamg-4.2.3/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-04-15 16:47:15.000000 pyamg-4.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-04-15 16:47:15.000000 pyamg-4.2.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-04-15 16:47:15.000000 pyamg-4.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-15 16:47:15.000000 pyamg-4.2.3/DEVELOPERS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-04-15 16:47:15.000000 pyamg-4.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-15 16:47:15.000000 pyamg-4.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-04-15 16:47:24.685344 pyamg-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-04-15 16:47:15.000000 pyamg-4.2.3/README-DEV.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-04-15 16:47:15.000000 pyamg-4.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.665343 pyamg-4.2.3/bench/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-04-15 16:47:15.000000 pyamg-4.2.3/bench/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-04-15 16:47:15.000000 pyamg-4.2.3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.665343 pyamg-4.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.669344 pyamg-4.2.3/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/dev/common_docstring.md
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/dev/todo.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.669344 pyamg-4.2.3/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   116340 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg.mat
+-rw-r--r--   0 runner    (1001) docker     (121)   119706 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)  1352508 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo.py
+-rw-r--r--   0 runner    (1001) docker     (121)   139020 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo_legacy.png
+-rw-r--r--   0 runner    (1001) docker     (121)    66612 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo_legacy_withtext.png
+-rw-r--r--   0 runner    (1001) docker     (121)   128585 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo_withtext.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)  1394824 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/logo/pyamg_logo_withtext.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)   193617 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/example.res.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/example_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/source/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     9832 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/source/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-04-15 16:47:15.000000 pyamg-4.2.3/docs/source/ref.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/pyamg/
+-rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/pyamg/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32212 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10316 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18076 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20086 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/rootnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43826 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tentative.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/pyamg/aggregation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7241 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25370 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22546 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_rootnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31886 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8820 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/aggregation/tests/test_tentative.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.677343 pyamg-4.2.3/pyamg/amg_core/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10873 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/bindthem.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1241 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/build.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    23654 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/evolution_strength.h
+-rw-r--r--   0 runner    (1001) docker     (121)    18573 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/evolution_strength_bind.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)      195 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/graph-todo.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35419 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/graph.h
+-rw-r--r--   0 runner    (1001) docker     (121)    26682 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/graph_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/instantiate.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/krylov.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7424 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/krylov_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    28660 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/linalg.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/linalg_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    32808 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/relaxation.h
+-rw-r--r--   0 runner    (1001) docker     (121)    42621 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/relaxation_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    41871 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/ruge_stuben.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19164 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/ruge_stuben_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    31256 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/smoothed_aggregation.h
+-rw-r--r--   0 runner    (1001) docker     (121)    25249 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/smoothed_aggregation_bind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.677343 pyamg-4.2.3/pyamg/amg_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/tests/bind_examples.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/tests/bind_examples_bind.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/tests/instantiate-test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/amg_core/tests/test_bind_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/citation.bib
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.677343 pyamg-4.2.3/pyamg/classical/
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6695 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/classical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/cr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13027 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/split.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.677343 pyamg-4.2.3/pyamg/classical/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7685 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/tests/test_classical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/classical/tests/test_cr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.677343 pyamg-4.2.3/pyamg/gallery/
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11023 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9794 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/gallery/example_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19027 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/airfoil.mat
+-rw-r--r--   0 runner    (1001) docker     (121)    42144 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/bar.mat
+-rw-r--r--   0 runner    (1001) docker     (121)   164770 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/helmholtz_2D.mat
+-rw-r--r--   0 runner    (1001) docker     (121)     8446 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/knot.mat
+-rw-r--r--   0 runner    (1001) docker     (121)   446800 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat
+-rw-r--r--   0 runner    (1001) docker     (121)    30384 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/recirc_flow.mat
+-rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/unit_cube.mat
+-rw-r--r--   0 runner    (1001) docker     (121)    14035 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/example_data/unit_square.mat
+-rw-r--r--   0 runner    (1001) docker     (121)    28444 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/fem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5420 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/gallery/mesh_data/
+-rw-r--r--   0 runner    (1001) docker     (121)    22998 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/mesh_data/square_mesh.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/random_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/stencil.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/gallery/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_fem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/gallery/tests/test_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11050 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/graph_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/krylov/
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_bicgstab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_cg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6562 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_cgne.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6615 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_cgnr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_cr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12557 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_fgmres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_gmres.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12997 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_gmres_householder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11065 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_gmres_mgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_minimal_residual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5954 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/_steepest_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/krylov/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12075 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/tests/test_krylov.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7480 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/krylov/tests/test_simple_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27490 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/multilevel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.681343 pyamg-4.2.3/pyamg/relaxation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37505 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24568 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/relaxation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    64489 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/relaxation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34522 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/strength.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/test_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14855 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15572 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/test_multilevel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32602 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/tests/test_strength.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/bsr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18547 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/params.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/tests/test_bsr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13136 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61192 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/tests/test_warn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69511 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-15 16:47:23.000000 pyamg-4.2.3/pyamg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/vis/
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.685344 pyamg-4.2.3/pyamg/vis/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3279 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/tests/test_vtu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9705 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/vis_coarse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16247 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyamg/vis/vtk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 16:47:24.673344 pyamg-4.2.3/pyamg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-04-15 16:47:24.000000 pyamg-4.2.3/pyamg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-04-15 16:47:24.000000 pyamg-4.2.3/pyamg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 16:47:24.000000 pyamg-4.2.3/pyamg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 16:47:23.000000 pyamg-4.2.3/pyamg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-15 16:47:24.000000 pyamg-4.2.3/pyamg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-15 16:47:24.000000 pyamg-4.2.3/pyamg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-04-15 16:47:15.000000 pyamg-4.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-15 16:47:15.000000 pyamg-4.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-15 16:47:15.000000 pyamg-4.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-04-15 16:47:24.685344 pyamg-4.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1299 2022-04-15 16:47:15.000000 pyamg-4.2.3/setup.py
```

### Comparing `pyamg-4.2.2/.github/workflows/ci.yml` & `pyamg-4.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/.github/workflows/lint.yml` & `pyamg-4.2.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/.github/workflows/wheels.yml` & `pyamg-4.2.3/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/CONTRIBUTING.md` & `pyamg-4.2.3/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 Copyright (c) 2008-2015 PyAMG Developers
 License: MIT, http://opensource.org/licenses/MIT
 
 Contributing
 ---
 
 Contributing code to this project assumes that
-    - your contributions are not significant enough to claim copyright or
-      that you implicitly transfer the copyright of your contribution to
-      the PyAMG Developers
-    - you agree to the Developer Certificate of Origin for
-      your contributing portion as described here (and below):
-      http://developercertificate.org/
+
+- your contributions are not significant enough to claim copyright or
+  that you implicitly transfer the copyright of your contribution to
+  the PyAMG Developers
+- you agree to the Developer Certificate of Origin for
+  your contributing portion as described here (and below):
+  http://developercertificate.org/
 
 Certificate of Origin
 ---
 
 """
 Developer Certificate of Origin
 Version 1.1
```

### Comparing `pyamg-4.2.2/LICENSE.txt` & `pyamg-4.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/PKG-INFO` & `pyamg-4.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamg
-Version: 4.2.2
+Version: 4.2.3
 Summary: PyAMG: Algebraic Multigrid Solvers in Python
 Home-page: https://github.com/pyamg/pyamg
 Download-URL: https://github.com/pyamg/pyamg/releases
 Author: Nathan Bell, Luke Olson, and Jacob Schroder
 Author-email: luke.olson@gmail.com
 Maintainer: Luke Olson
 Maintainer-email: luke.olson@gmail.com
@@ -60,15 +60,15 @@
 conda install pyamg
 ```
 
 # Introduction
 
 PyAMG is a library of **Algebraic Multigrid (AMG)** solvers with a convenient Python interface.
 
-![](./Docs/logo/pyamg_logo_withtext.png)
+![](https://raw.githubusercontent.com/pyamg/pyamg/main/docs/logo/pyamg_logo_withtext.png)
 
 PyAMG is currently developed by [Luke Olson](http://lukeo.cs.illinois.edu), and [Jacob Schroder](http://people.llnl.gov/schroder2).
 
 # Citing
 
 <pre>
 @MISC{OlSc2018,
@@ -78,19 +78,30 @@
       url = "https://github.com/pyamg/pyamg",
       note = "Release 4.0"
       }
 </pre>
 
 # Getting Help
 
-For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
+- For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
 
-Create an [issue](https://github.com/pyamg/pyamg/issues).
+- Create an [issue](https://github.com/pyamg/pyamg/issues).
 
-Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [Examples](https://github.com/pyamg/pyamg/wiki/Examples) (for instance  the [0STARTHERE](https://github.com/pyamg/pyamg-examples/blob/master/0STARTHERE/demo.py) example).
+- Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [examples](https://github.com/pyamg/pyamg-examples) (for instance  the [0_start_here](https://github.com/pyamg/pyamg-examples/blob/main/0_start_here/demo.py) example).
+
+- Run the unit tests (`pip install pytest`):
+  - With PyAMG installed and from a non-source directory:
+  ```python
+  import pyamg
+  pyamg.test()
+  ```
+  - From the PyAMG source directory and installed (e.g. with `pip install -e .`):
+  ```python
+  pytest .
+  ```
 
 # What is AMG?
 
  AMG is a multilevel technique for solving large-scale linear systems with optimal or near-optimal efficiency.  Unlike geometric multigrid, AMG requires little or no geometric information about the underlying problem and develops a sequence of coarser grids directly from the input matrix.  This feature is especially important for problems discretized on unstructured meshes and irregular grids.
 
 # PyAMG Features
```

### Comparing `pyamg-4.2.2/README-DEV.md` & `pyamg-4.2.3/README-DEV.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Release Steps:
+- suppose the current tag is 4.2.2 and the next is 4.2.3
 - with no staged commits and a clean status...
-- meld a summary of `git log 7a74ef7..HEAD --oneline` with whatever hash with `[unreleased]` in changelog
+- meld a summary of `git log $(git tag --sort version:refname | tail -n 1)..HEAD --oneline` (all commits since last tag) with whatever hash with `[4.2.3]` in changelog
 - commit, push
 - `mkvirtualenv releasetest`
 - check that `pip install .` and `python -c "import pyamg; pyamg.test()"` pass (outside source directory)
 - remove untracked files `git clean -xdf`
-- the following can be done with a pre-release, `v4.2.1-alpha.6`, for testing.  It will not become the default on pypi and `gh release create` can be marked with `--prerelease`
+- the following can be done with a pre-release, `v4.2.3-alpha.6`, for testing.  It will not become the default on pypi and `gh release create` can be marked with `--prerelease` (below)
 - mark `fallback_version` in `pyproject.toml`
-- `git tag -a v3.2.0 -m "version 3.2.0"`
+- commit, push
+- `git tag -a v4.2.3 -m "version 4.2.3"`
 - `git push`
 - `git push --tags`
-- then release the version on Github: `gh release create v1.2.3 --notes "see changelog.md"`
+- then release the version on Github: `gh release create v4.2.3 --notes "see changelog.md"`
   - This will trigger the GHA `.github/workflows/wheels.yml` which builds wheels and a source distribution, and publishes to pypi
 
 Testing notes:
 - do not use seeds such as 0, 1, 42, 100
 - for each needed seed, generate a "random" int
 - `python3 -c "import numpy as np; np.random.seed(); seeds = np.random.randint(0, 2**32 - 1, 5); print(seeds)"`
```

### Comparing `pyamg-4.2.2/README.md` & `pyamg-4.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 conda install pyamg
 ```
 
 # Introduction
 
 PyAMG is a library of **Algebraic Multigrid (AMG)** solvers with a convenient Python interface.
 
-![](./Docs/logo/pyamg_logo_withtext.png)
+![](https://raw.githubusercontent.com/pyamg/pyamg/main/docs/logo/pyamg_logo_withtext.png)
 
 PyAMG is currently developed by [Luke Olson](http://lukeo.cs.illinois.edu), and [Jacob Schroder](http://people.llnl.gov/schroder2).
 
 # Citing
 
 <pre>
 @MISC{OlSc2018,
@@ -42,19 +42,30 @@
       url = "https://github.com/pyamg/pyamg",
       note = "Release 4.0"
       }
 </pre>
 
 # Getting Help
 
-For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
+- For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
 
-Create an [issue](https://github.com/pyamg/pyamg/issues).
+- Create an [issue](https://github.com/pyamg/pyamg/issues).
 
-Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [Examples](https://github.com/pyamg/pyamg/wiki/Examples) (for instance  the [0STARTHERE](https://github.com/pyamg/pyamg-examples/blob/master/0STARTHERE/demo.py) example).
+- Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [examples](https://github.com/pyamg/pyamg-examples) (for instance  the [0_start_here](https://github.com/pyamg/pyamg-examples/blob/main/0_start_here/demo.py) example).
+
+- Run the unit tests (`pip install pytest`):
+  - With PyAMG installed and from a non-source directory:
+  ```python
+  import pyamg
+  pyamg.test()
+  ```
+  - From the PyAMG source directory and installed (e.g. with `pip install -e .`):
+  ```python
+  pytest .
+  ```
 
 # What is AMG?
 
  AMG is a multilevel technique for solving large-scale linear systems with optimal or near-optimal efficiency.  Unlike geometric multigrid, AMG requires little or no geometric information about the underlying problem and develops a sequence of coarser grids directly from the input matrix.  This feature is especially important for problems discretized on unstructured meshes and irregular grids.
 
 # PyAMG Features
```

### Comparing `pyamg-4.2.2/docs/Makefile` & `pyamg-4.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/dev/common_docstring.md` & `pyamg-4.2.3/docs/dev/common_docstring.md`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/dev/todo.md` & `pyamg-4.2.3/docs/dev/todo.md`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg.mat` & `pyamg-4.2.3/docs/logo/pyamg.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo.pdf` & `pyamg-4.2.3/docs/logo/pyamg_logo.pdf`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo.png` & `pyamg-4.2.3/docs/logo/pyamg_logo.png`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo.py` & `pyamg-4.2.3/docs/logo/pyamg_logo.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo_legacy.png` & `pyamg-4.2.3/docs/logo/pyamg_logo_legacy.png`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo_legacy_withtext.png` & `pyamg-4.2.3/docs/logo/pyamg_logo_legacy_withtext.png`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo_withtext.pdf` & `pyamg-4.2.3/docs/logo/pyamg_logo_withtext.pdf`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/logo/pyamg_logo_withtext.png` & `pyamg-4.2.3/docs/logo/pyamg_logo_withtext.png`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/source/README.md` & `pyamg-4.2.3/docs/source/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 conda install pyamg
 ```
 
 # Introduction
 
 PyAMG is a library of **Algebraic Multigrid (AMG)** solvers with a convenient Python interface.
 
-![](./Docs/logo/pyamg_logo_withtext.png)
+![](https://raw.githubusercontent.com/pyamg/pyamg/main/docs/logo/pyamg_logo_withtext.png)
 
 PyAMG is currently developed by [Luke Olson](http://lukeo.cs.illinois.edu), and [Jacob Schroder](http://people.llnl.gov/schroder2).
 
 # Citing
 
 <pre>
 @MISC{OlSc2018,
@@ -42,19 +42,30 @@
       url = "https://github.com/pyamg/pyamg",
       note = "Release 4.0"
       }
 </pre>
 
 # Getting Help
 
-For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
+- For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
 
-Create an [issue](https://github.com/pyamg/pyamg/issues).
+- Create an [issue](https://github.com/pyamg/pyamg/issues).
 
-Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [Examples](https://github.com/pyamg/pyamg/wiki/Examples) (for instance  the [0STARTHERE](https://github.com/pyamg/pyamg-examples/blob/master/0STARTHERE/demo.py) example).
+- Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [examples](https://github.com/pyamg/pyamg-examples) (for instance  the [0_start_here](https://github.com/pyamg/pyamg-examples/blob/main/0_start_here/demo.py) example).
+
+- Run the unit tests (`pip install pytest`):
+  - With PyAMG installed and from a non-source directory:
+  ```python
+  import pyamg
+  pyamg.test()
+  ```
+  - From the PyAMG source directory and installed (e.g. with `pip install -e .`):
+  ```python
+  pytest .
+  ```
 
 # What is AMG?
 
  AMG is a multilevel technique for solving large-scale linear systems with optimal or near-optimal efficiency.  Unlike geometric multigrid, AMG requires little or no geometric information about the underlying problem and develops a sequence of coarser grids directly from the input matrix.  This feature is especially important for problems discretized on unstructured meshes and irregular grids.
 
 # PyAMG Features
```

### Comparing `pyamg-4.2.2/docs/source/_static/default.css` & `pyamg-4.2.3/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/docs/source/conf.py` & `pyamg-4.2.3/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 #!/usr/bin/env python3
-#
+"""Sphinx configuration."""
 import os
 import sys
+import pyamg
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.insert(0, os.path.abspath('.'))
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.viewcode',
               'sphinx.ext.autosummary',
               'sphinx.ext.mathjax',
-              'm2r',
+              'sphinx_automodapi.automodapi',
+              'm2r2',
               'numpydoc']
 
-autodoc_default_flags = ['members', 'undoc-members', 'special-members', 'private-members']
+autodoc_default_options = {
+    'members': True,
+    'undoc-members': True,
+    'special-members': True,
+    'private-members': True,
+}
 autosummary_generate = True
 
 templates_path = ['_templates']
 source_suffix = ['.rst', '.md']
 master_doc = 'index'
 
 project = 'PyAMG'
-copyright = '2018, Luke Olson'
-author = '2018, Luke Olson and Jacob Schroder'
+copyright = '2022, Luke Olson'  # pylint: disable=redefined-builtin
+author = '2022, Luke Olson and Jacob Schroder'
 
-import pyamg
 version = pyamg.__version__
 release = version
 
 language = None
 exclude_patterns = ['README.md']
 
 pygments_style = 'sphinx'
 
 todo_include_todos = False
 
 # for debugging
 # keep_warnings=True
 
-#html_theme = 'alabaster'
-html_theme = 'sphinx_rtd_theme'
-html_logo = '../logo/versions/logo_dropshadow_small.png'
+html_theme = 'pydata_sphinx_theme'
+html_logo = '../logo/pyamg_logo.png'
 html_static_path = ['_static']
 
 htmlhelp_basename = 'PyAMGdoc'
 
 latex_elements = {
     # 'papersize': 'letterpaper',
     # 'pointsize': '10pt',
     # 'preamble': '',
     # 'figure_align': 'htbp',
 }
 
 latex_documents = [
-    (master_doc, 'PyAMG.tex', 'PyAMG Documentation',
+    (master_doc, 'pyamg.tex', 'PyAMG Documentation',
      'Luke Olson', 'manual'),
 ]
 
 man_pages = [
     (master_doc, 'pyamg', 'PyAMG Documentation',
      [author], 1)
 ]
 
 texinfo_documents = [
     (master_doc, 'PyAMG', 'PyAMG Documentation',
      author, 'PyAMG', 'Algebraic Multigrid Solvers in Python.',
      'Miscellaneous'),
 ]
 
-def autodoc_skip_member(app, what, name, obj, skip, options):
+
+def autodoc_skip_member(_app, _what, name, _obj, skip, _options):
+    """Set skip member."""
     exclusions = ('__weakref__',  # special-members
                   '__doc__', '__module__', '__dict__',  # undoc-members
                   )
     exclude = name in exclusions
     return skip or exclude
 
+
 def setup(app):
+    """Define setup."""
     app.connect('autodoc-skip-member', autodoc_skip_member)
```

### Comparing `pyamg-4.2.2/docs/source/ref.rst` & `pyamg-4.2.3/docs/source/ref.rst`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,17 @@
 
 .. currentmodule:: pyamg
 
 .. autosummary::
     :toctree: generated/
 
     gallery
+
+amg\_core
+----------------
+
+.. currentmodule:: pyamg
+
+.. autosummary::
+    :toctree: generated/
+
+    amg_core
```

### Comparing `pyamg-4.2.2/pyamg/__init__.py` & `pyamg-4.2.3/pyamg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,16 @@
 
 __all__ += ['test']
 
 __doc__ += """
 
 Utility tools
 -------------
-
-  test        --- Run pyamg unittests (requires pytest)
-  __version__ --- pyamg version string
-
+test         Run pyamg unittests (requires pytest)
+__version__  pyamg version string
 """
 
 # Warn on old numpy or scipy.  Two digits.
 npreq = '1.6'
 npmin = [int(j) for j in npreq.split('.')]
 m = re.match(r'(\d+)\.(\d+).*', np.__version__)
 npver = [int(m.group(1)), int(m.group(2))]
@@ -61,15 +59,18 @@
     Parameters
     ----------
     verbose : bool
         Turn on verbose output.
 
     """
     import sys     # pylint: disable=import-outside-toplevel
-    import pytest  # pylint: disable=import-outside-toplevel
+    try:
+        import pytest  # pylint: disable=import-outside-toplevel
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError('pytest is not installed and is needed for test()') from e
 
     sysversion = sys.version.replace('\n', '')
     print(f'Python version: {sysversion}')
     print(f'pytest version: {pytest.__version__}')
     print(f'scipy  version: {sp.__version__}')
     print(f'numpy  version: {np.__version__}')
     print(f'pyamg  version: {__version__}')
```

### Comparing `pyamg-4.2.2/pyamg/aggregation/__init__.py` & `pyamg-4.2.3/pyamg/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/adaptive.py` & `pyamg-4.2.3/pyamg/aggregation/adaptive.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/aggregate.py` & `pyamg-4.2.3/pyamg/aggregation/aggregate.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/aggregation.py` & `pyamg-4.2.3/pyamg/aggregation/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/rootnode.py` & `pyamg-4.2.3/pyamg/aggregation/rootnode.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/smooth.py` & `pyamg-4.2.3/pyamg/aggregation/smooth.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tentative.py` & `pyamg-4.2.3/pyamg/aggregation/tentative.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_adaptive.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_aggregate.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_aggregation.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_rootnode.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_rootnode.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_smooth.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/aggregation/tests/test_tentative.py` & `pyamg-4.2.3/pyamg/aggregation/tests/test_tentative.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/__init__.py` & `pyamg-4.2.3/pyamg/amg_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/bindthem.py` & `pyamg-4.2.3/pyamg/amg_core/bindthem.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/build.sh` & `pyamg-4.2.3/pyamg/amg_core/build.sh`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/evolution_strength.h` & `pyamg-4.2.3/pyamg/amg_core/evolution_strength.h`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
  * Sx : {float|complex array}
  *      Block data structure of BSR matrix, S
  *      Sx is (n_blocks x blocksize) in length
  * Tx : {float|complex array}
  *      modified in place for output
  *
  * Returns
- * ------
+ * -------
  * Tx[i] modified in place, it holds
  * the minimum nonzero value of block i of S
  *
  * Notes
  * -----
  * Principle calling routine is evolution_strength_of_connection(...) in strength.py.
  * In that routine, it is used to assign a strength of connection value between
@@ -289,16 +289,16 @@
  * NullDim : {int}
  *      Number of nullspace vectors
  * tol : {float}
  *      Used to determine when values are numerically zero
  *
  * Returns
  * -------
- *   Sx is written in place and holds strength
- *   values reflecting the above minimization problem
+ * Sx is written in place and holds strength
+ * values reflecting the above minimization problem
  *
  * Notes
  * -----
  * Upon entry to the routine, S = (I - (t/k) Dinv A)^k.  However,
  * we only need the values of S at the sparsity pattern of A.  Hence,
  * there is no need to completely calculate all of S.
  *
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/evolution_strength_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/evolution_strength_bind.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 Sx : {float|complex array}
      Block data structure of BSR matrix, S
      Sx is (n_blocks x blocksize) in length
 Tx : {float|complex array}
      modified in place for output
 
 Returns
-------
+-------
 Tx[i] modified in place, it holds
 the minimum nonzero value of block i of S
 
 Notes
 -----
 Principle calling routine is evolution_strength_of_connection(...) in strength.py.
 In that routine, it is used to assign a strength of connection value between
@@ -396,16 +396,16 @@
 NullDim : {int}
      Number of nullspace vectors
 tol : {float}
      Used to determine when values are numerically zero
 
 Returns
 -------
-  Sx is written in place and holds strength
-  values reflecting the above minimization problem
+Sx is written in place and holds strength
+values reflecting the above minimization problem
 
 Notes
 -----
 Upon entry to the routine, S = (I - (t/k) Dinv A)^k.  However,
 we only need the values of S at the sparsity pattern of A.  Hence,
 there is no need to completely calculate all of S.
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/graph.h` & `pyamg-4.2.3/pyamg/amg_core/graph.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,45 @@
 inline void coreassert(const bool istrue, const std::string &errormsg){
     if (!istrue){
         throw std::runtime_error("pyamg-error (amg_core) -- " + errormsg);
     }
 }
 
 /*
- *  Compute a maximal independent set for a graph stored in CSR format
- *  using a greedy serial algorithm
- *
- *  Parameters
- *      num_rows   - number of rows in A (number of vertices)
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      active     - value used for active vertices        (input)
- *       C         - value used to mark non-MIS vertices   (output)
- *       F         - value used to mark MIS vertices       (output)
- *      x[]        - state of each vertex
- *
+ * Compute a maximal independent set for a graph stored in CSR format
+ * using a greedy serial algorithm
  *
- *  Returns:
- *      The number of nodes in the MIS.
- *
- *  Notes:
- *      Only the vertices with values with x[i] == active are considered
- *      when determining the MIS.  Upon return, all active vertices will
- *      be assigned the value C or F depending on whether they are in the
- *      MIS or not.
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     Number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * active : float-like
+ *     Value used for active vertices
+ * C : float-like
+ *     Value used to mark non-MIS vertices
+ * F : float-like
+ *     Value used to mark MIS vertices
+ * x : array, inplace output
+ *     State of each vertex
+ *
+ * Returns
+ * -------
+ * N : int
+ *     The number of nodes in the MIS.
+ *
+ * Notes
+ * -----
+ * Only the vertices with values with x[i] == active are considered
+ * when determining the MIS.  Upon return, all active vertices will
+ * be assigned the value C or F depending on whether they are in the
+ * MIS or not.
  *
  */
 template<class I, class T>
 I maximal_independent_set_serial(const I num_rows,
                                  const I Ap[], const int Ap_size,
                                  const I Aj[], const int Aj_size,
                                  const T active,
@@ -68,34 +78,45 @@
 }
 
 /*
  *  Compute a maximal independent set for a graph stored in CSR format
  *  using a variant of Luby's parallel MIS algorithm
  *
  *  Parameters
- *      num_rows   - number of rows in A (number of vertices)
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      active     - value used for active vertices        (input)
- *       C         - value used to mark non-MIS vertices   (output)
- *       F         - value used to mark MIS vertices       (output)
- *      x[]        - state of each vertex
- *      y[]        - random values for each vertex
- *      max_iters  - maximum number of iterations
- *                   by default max_iters=-1 and no limit
- *                   is imposed
+ *  ----------
+ *  num_rows : int
+ *      number of rows in A (number of vertices)
+ *  Ap : array
+ *      CSR row pointer
+ *  Aj : array
+ *      CSR index array
+ *  active : float
+ *      value used for active vertices
+ *  C : float
+ *      value used to mark non-MIS vertices
+ *  F : float
+ *      value used to mark MIS vertices
+ *  x : array, output
+ *      state of each vertex
+ *  y : array
+ *      random values for each vertex
+ *  max_iters : int
+ *      maximum number of iterations By default max_iters=-1 and no limit is imposed
  *
- *  Returns:
+ *  Returns
+ *  -------
+ *  N : int
  *      The number of nodes in the MIS.
  *
- *  Notes:
- *      Only the vertices with values with x[i] == active are considered
- *      when determining the MIS.  Upon return, all active vertices will
- *      be assigned the value C or F depending on whether they are in the
- *      MIS or not.
+ *  Notes
+ *  -----
+ *  Only the vertices with values with x[i] == active are considered
+ *  when determining the MIS.  Upon return, all active vertices will
+ *  be assigned the value C or F depending on whether they are in the
+ *  MIS or not.
  *
  */
 template<class I, class T, class R>
 I maximal_independent_set_parallel(const I num_rows,
                                    const I Ap[], const int Ap_size,
                                    const I Aj[], const int Aj_size,
                                    const T active,
@@ -223,30 +244,37 @@
 }
 
 
 
 /*
  * Compute a vertex coloring of a graph using the Jones-Plassmann algorithm
  *
- *  Parameters
- *      num_rows   - number of rows in A (number of vertices)
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      x[]        - color of each vertex
- *      y[]        - initial random values for each vertex
- *
- *  Notes:
- *      Arrays x and y will be overwritten
- *
- *  References:
- *      Mark T. Jones and Paul E. Plassmann
- *      A Parallel Graph Coloring Heuristic
- *      SIAM Journal on Scientific Computing 14:3 (1993) 654--669
- *      http://citeseer.ist.psu.edu/jones92parallel.html
- *
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * x : array, inplace
+ *     color of each vertex
+ * y : array
+ *     initial random values for each vertex
+ *
+ * Notes
+ * -----
+ *     Arrays x and y will be overwritten
+ *
+ * References
+ * ----------
+ * .. [Jones92] Mark T. Jones and Paul E. Plassmann
+ *    A Parallel Graph Coloring Heuristic
+ *    SIAM Journal on Scientific Computing 14:3 (1993) 654--669
+ *    http://citeseer.ist.psu.edu/jones92parallel.html
  */
 template<class I, class T, class R>
 T vertex_coloring_jones_plassmann(const I num_rows,
                                   const I Ap[], const int Ap_size,
                                   const I Aj[], const int Aj_size,
                                         T  x[], const int  x_size,
                                         R  z[], const int  z_size)
@@ -274,26 +302,33 @@
 }
 
 
 /*
  * Compute a vertex coloring of a graph using the parallel
  * Largest-Degree-First (LDF) algorithm
  *
- *  Parameters
- *      num_rows   - number of rows in A (number of vertices)
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      x[]        - color of each vertex
- *      y[]        - initial random values for each vertex
- *
- *   References:
- *     J. R. Allwright and R. Bordawekar and P. D. Coddington and K. Dincer and C. L. Martin
- *     A Comparison of Parallel Graph Coloring Algorithms
- *     DRAFT SCCS-666
- *     http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.45.4650
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * x : array
+ *     color of each vertex
+ * y : array
+ *     initial random values for each vertex
+ *
+ * References
+ * ----------
+ * .. [LDF] J. R. Allwright and R. Bordawekar and P. D. Coddington and K. Dincer and C. L. Martin
+ *    A Comparison of Parallel Graph Coloring Algorithms
+ *    DRAFT SCCS-666
+ *    http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.45.4650
  *
  */
 template<class I, class T, class R>
 T vertex_coloring_LDF(const I num_rows,
                       const I Ap[], const int Ap_size,
                       const I Aj[], const int Aj_size,
                             T  x[], const int  x_size,
@@ -331,47 +366,52 @@
     return *std::max_element(x, x + num_rows);
 }
 
 
 /*
  * Compute the incidence matrix for a clustering
  *
- *      I = Incidence matrix between nodes and clusters (num_nodes x num_clusters)
+ * Parameters
+ * ----------
+ * num_nodes : int
+ *     number of nodes
+ * num_clusters : int
+ *     number of clusters
+ * cm : array, num_nodes
+ *     cluster index for each node
+ * ICp : arrayt, num_clusters+1, inplace
+ *     CSC column pointer array for I
+ * ICi : array, num_nodes, inplace
+ *     CSC column indexes for I
+ * L : array, num_nodes, inplace
+ *     Local index mapping
+ *
+ * Notes
+ * -----
+ * I = Incidence matrix between nodes and clusters (num_nodes x num_clusters)
  * I[i,a] = 1 if node i is in cluster a, otherwise 0
  *
- *     Cluster indexes: a,b,c in 1..num_clusters
+ * Cluster indexes: a,b,c in 1..num_clusters
  * Global node indexes: i,j,k in 1..num_rows
- *  Local node indexes: pair (a,m) where a is cluster and m in 1..num_nodes_in_cluster
+ * Local node indexes: pair (a,m) where a is cluster and m in 1..num_nodes_in_cluster
  *
  * We store I in both CSC and CSR formats because we want to be able
  * to map global <-> local node indexes. However, I in CSR format is
  * simply the cm array, so we only need to compute CSC format.
  *
- * IC = (ICp,ICi)    = I in CSC format (don't store ICx because it's
- *                     always 1).
+ * IC = (ICp,ICi)    = I in CSC format (don't store ICx because it's always 1).
  *
  * IR = (IRa) = (cm) = I in CSR format (don't store IRp because we
- *                     have exactly one nonzero entry per row, and
- *                     don't store IRx because it's always 1). This is
- *                     just the cm array.
+ * have exactly one nonzero entry per row, and don't store IRx because it's always 1). This is
+ * just the cm array.
  *
  * Converting local (a,m) -> global i:   i = ICi[ICp[a] + m]
- *
- * Converting global i -> local (a,m):   a = cm[i]
- *                                       m = L[i]
+ * Converting global i -> local (a,m):   a = cm[i], m = L[i]
  *
  * L is an additional vector (length num_rows) to store local indexes.
- *
- *  Parameters
- *      num_nodes         - (IN)  number of nodes
- *      num_clusters      - (IN)  number of clusters
- *     cm[num_nodes]      - (IN)  cluster index for each node
- *    ICp[num_clusters+1] - (OUT) CSC column pointer array for I
- *    ICi[num_nodes]      - (OUT) CSC column indexes for I
- *      L[num_nodes]      - (OUT) Local index mapping
  */
 template<class I>
 void cluster_node_incidence(const I num_nodes,
                             const I num_clusters,
                             const I  cm[], const int  cm_size,
                                   I ICp[], const int ICp_size,
                                   I ICi[], const int ICi_size,
@@ -446,33 +486,47 @@
 }
 
 
 /*
  * Apply Floyd–Warshall to cluster "a" and use the result to find the
  * cluster center
  *
- *  Parameters
- *      a                  - (IN) cluster index to find the center of
- *      num_nodes          - (IN) number of nodes
- *      num_clusters       - (IN) number of clusters
- *      Ap[]               - (IN) CSR row pointer
- *      Aj[]               - (IN) CSR index array
- *      Ax[]               - (IN) CSR data array (edge lengths)
- *      cm[num_nodes]      - (IN) cluster index for each node
- *     ICp[num_clusters+1] - (IN) CSC column pointer array for I
- *     ICi[num_nodes]      - (IN) CSC column indexes for I
- *       L[num_nodes]      - (IN) Local index mapping
- *
- *  Returns
- *      i                  - global node index of center of cluster a
- *
- *  References:
- *      https://en.wikipedia.org/wiki/Graph_center
- *      https://en.wikipedia.org/wiki/Floyd–Warshall_algorithm
- *      https://en.wikipedia.org/wiki/Distance_(graph_theory)
+ * Parameters
+ * ----------
+ * a : int
+ *     cluster index to find the center of
+ * num_nodes : int
+ *     number of nodes
+ * num_clusters : int
+ *     number of clusters
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array (edge lengths)
+ * cm : array, num_nodes
+ *     cluster index for each node
+ * ICp : array, num_clusters+1
+ *     CSC column pointer array for I
+ * ICi : array, num_nodes
+ *     CSC column indexes for I
+ * L : array, num_nodes
+ *     Local index mapping
+ *
+ * Returns
+ * -------
+ * i : int
+ *     global node index of center of cluster a
+ *
+ * References
+ * ----------
+ * .. [1] Graph Center:   https://en.wikipedia.org/wiki/Graph_center
+ * .. [2] Floyd-Warshall: https://en.wikipedia.org/wiki/Floyd–Warshall_algorithm
+ * .. [3] Graph Distance: https://en.wikipedia.org/wiki/Distance_(graph_theory)
  */
 template<class I, class T>
 I cluster_center(const I a,
                  const I num_nodes,
                  const I num_clusters,
                  const I  Ap[], const int  Ap_size,
                  const I  Aj[], const int  Aj_size,
@@ -545,24 +599,32 @@
     return i;
 }
 
 /*
  * Apply one iteration of Bellman-Ford iteration on a distance
  * graph stored in CSR format.
  *
- *  Parameters
- *      num_nodes - (IN)    number of nodes (number of rows in A)
- *      Ap[]      - (IN)    CSR row pointer
- *      Aj[]      - (IN)    CSR index array
- *      Ax[]      - (IN)    CSR data array (edge lengths)
- *      d[]       - (INOUT) distance to nearest center
- *     cm[]       - (INOUT) cluster index for each node
- *
- *  References:
- *      http://en.wikipedia.org/wiki/Bellman-Ford_algorithm
+ * Parameters
+ * ----------
+ * num_nodes : int
+ *     number of nodes (number of rows in A)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array (edge lengths)
+ * d : array, inplace
+ *     distance to nearest center
+ * cm : array, inplace
+ *     cluster index for each node
+ *
+ * References
+ * ----------
+ * .. [1] Bellman-Ford Wikipedia: http://en.wikipedia.org/wiki/Bellman-Ford_algorithm
  */
 template<class I, class T>
 void bellman_ford(const I num_nodes,
                   const I Ap[], const int Ap_size,
                   const I Aj[], const int Aj_size,
                   const T Ax[], const int Ax_size,
                         T  d[], const int  d_size,
@@ -590,25 +652,34 @@
  * Apply Bellman-Ford with a heuristic to balance cluster sizes
  *
  * This version is modified to break distance ties by assigning nodes
  * to the cluster with the fewest points, while preserving cluster
  * connectivity. This will hopefully result in more balanced cluster
  * sizes.
  *
- *  Parameters
- *     num_nodes    - (IN)    number of nodes (vertices)
- *     num_clusters - (IN)    number of clusters
- *     Ap[]         - (IN)    CSR row pointer for adjacency matrix A
- *     Aj[]         - (IN)    CSR index array
- *     Ax[]         - (IN)    CSR data array (edge lengths)
- *      d[]         - (INOUT) distance to nearest center
- *     cm[]         - (INOUT) cluster index for each node
- *
- *  References:
- *      http://en.wikipedia.org/wiki/Bellman-Ford_algorithm
+ * Parameters
+ * ----------
+ * num_nodes : int
+ *     number of nodes (vertices)
+ * num_clusters : int
+ *     number of clusters
+ * Ap : array
+ *     CSR row pointer for adjacency matrix A
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array (edge lengths)
+ * d : array, inplace
+ *     distance to nearest center
+ * cm : array, inplace
+ *     cluster index for each node
+ *
+ * References
+ * ----------
+ * .. [1] Bellman-Ford: http://en.wikipedia.org/wiki/Bellman-Ford_algorithm
  */
 template<class I, class T>
 void bellman_ford_balanced(const I num_nodes,
                            const I num_clusters,
                            const I Ap[], const int Ap_size,
                            const I Aj[], const int Aj_size,
                            const T Ax[], const int Ax_size,
@@ -676,28 +747,37 @@
     } while(change);
 }
 
 
 /*
  * Perform one iteration of Lloyd clustering on a distance graph
  *
- *  Parameters
- *      num_nodes       - (IN)  number of nodes (number of rows in A)
- *      Ap[]            - (IN)  CSR row pointer for adjacency matrix A
- *      Aj[]            - (IN)  CSR index array
- *      Ax[]            - (IN)  CSR data array (edge lengths)
- *      num_clusters    - (IN)  number of clusters (seeds)
- *      d[num_nodes]    - (OUT) distance to nearest seed
- *     cm[num_nodes]    - (OUT) cluster index for each node
- *      c[num_clusters] - (INOUT)  cluster centers
- *
- *  References
- *      Nathan Bell
- *      Algebraic Multigrid for Discrete Differential Forms
- *      PhD thesis (UIUC), August 2008
+ * Parameters
+ * ----------
+ * num_nodes : int
+ *     number of nodes (number of rows in A)
+ * Ap : array
+ *     CSR row pointer for adjacency matrix A
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array (edge lengths)
+ * num_clusters : int
+ *     number of clusters (seeds)
+ * d : array, num_nodes
+ *     distance to nearest seed
+ * cm : array, num_nodes
+ *     cluster index for each node
+ * c : array, num_clusters
+ *     cluster centers
+ *
+ * References
+ * ----------
+ * .. [Bell2008] Nathan Bell, Algebraic Multigrid for Discrete Differential Forms
+ *    PhD thesis (UIUC), August 2008
  *
  */
 template<class I, class T>
 void lloyd_cluster(const I num_nodes,
                    const I Ap[], const int Ap_size,
                    const I Aj[], const int Aj_size,
                    const T Ax[], const int Ax_size,
@@ -761,32 +841,39 @@
 }
 
 
 /*
  * Perform one iteration of Lloyd clustering on a distance graph using
  * exact centers
  *
+ * Parameters
+ * ----------
+ * num_nodes : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array (edge lengths)
+ * num_clusters : int
+ *     number of clusters = number of seeds
+ * d : array, num_nodes
+ *     distance to nearest seed
+ * cm : array, num_nodes
+ *     cluster index for each node
+ * c : array, num_clusters
+ *     cluster centers
+ *
+ * Notes
+ * -----
  * This version computes exact cluster centers with Floyd-Warshall and
  * also uses a balanced version of Bellman-Ford to try and find
  * nearly-equal-sized clusters.
  *
- *  Parameters
- *      num_nodes       - (IN)  number of rows in A (number of vertices)
- *      Ap[]            - (IN)  CSR row pointer
- *      Aj[]            - (IN)  CSR index array
- *      Ax[]            - (IN)  CSR data array (edge lengths)
- *      num_clusters    - (IN)  number of clusters = number of seeds
- *      d[num_nodes]    - (OUT) distance to nearest seed
- *     cm[num_nodes]    - (OUT) cluster index for each node
- *      c[num_clusters] - (IN)  cluster centers
- *
- *  References
- *      Nathan Bell
- *      Algebraic Multigrid for Discrete Differential Forms
- *      PhD thesis (UIUC), August 2008
  */
 template<class I, class T>
 void lloyd_cluster_exact(const I num_nodes,
                          const I Ap[], const int Ap_size,
                          const I Aj[], const int Aj_size,
                          const T Ax[], const int Ax_size,
                          const I num_clusters,
@@ -878,30 +965,41 @@
 
         o_keys[i] = k_max;
         o_vals[i] = v_max;
     }
 }
 
 /*
- *  Compute a distance-k maximal independent set for a graph stored
- *  in CSR format using a parallel algorithm.  An MIS-k is a set of
- *  vertices such that all vertices in the MIS-k are separated by a
- *  path of at least K+1 edges and no additional vertex can be added
- *  to the set without destroying this property.  A standard MIS
- *  is therefore a MIS-1.
- *
- *  Parameters
- *      num_rows   - number of rows in A (number of vertices)
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      k          - minimum separation between MIS vertices
- *      x[]        - state of each vertex (1 if in the MIS, 0 otherwise)
- *      y[]        - random values used during parallel MIS algorithm
- *      max_iters  - maximum number of iterations to use (default, no limit)
+ * Compute MIS-k.
  *
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * k : int
+ *     minimum separation between MIS vertices
+ * x : array, inplace
+ *     state of each vertex (1 if in the MIS, 0 otherwise)
+ * y : array
+ *     random values used during parallel MIS algorithm
+ * max_iters : int
+ *     maximum number of iterations to use (default, no limit)
+ *
+ * Notes
+ * -----
+ * Compute a distance-k maximal independent set for a graph stored
+ * in CSR format using a parallel algorithm.  An MIS-k is a set of
+ * vertices such that all vertices in the MIS-k are separated by a
+ * path of at least K+1 edges and no additional vertex can be added
+ * to the set without destroying this property.  A standard MIS
+ * is therefore a MIS-1.
  */
 template<class I, class T, class R>
 void maximal_independent_set_k_parallel(const I num_rows,
                                         const I Ap[], const int Ap_size,
                                         const I Aj[], const int Aj_size,
                                         const I  k,
                                               T  x[], const int  x_size,
@@ -968,26 +1066,33 @@
         if( !work_left )
             return;
     }
 
 }
 
 /*
- *  Compute a breadth first search of a graph in CSR format
- *  beginning at a given seed vertex.
- *
- *  Parameters
- *      num_rows         - number of rows in A (number of vertices)
- *      Ap[]             - CSR row pointer
- *      Aj[]             - CSR index array
- *      order[num_rows]  - records the order in which vertices were searched
- *      level[num_rows]  - records the level set of the searched vertices (i.e. the minimum distance to the seed)
+ * Compute a breadth first search of a graph in CSR format
+ * beginning at a given seed vertex.
  *
- *  Notes:
- *      The values of the level must be initialized to -1
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * order : array, num_rows, inplace
+ *     records the order in which vertices were searched
+ * level : array, num_rows, inplace
+ *     records the level set of the searched vertices (i.e. the minimum distance to the seed)
+ *
+ * Notes
+ * -----
+ * The values of the level must be initialized to -1
  *
  */
 template <class I>
 void breadth_first_search(const I Ap[], const int Ap_size,
                           const I Aj[], const int Aj_size,
                           const I seed,
                                 I order[], const int order_size,
@@ -1024,25 +1129,31 @@
         current_level++;
     }
 
 }
 
 
 /*
- *  Compute the connected components of a graph stored in CSR format.
- *
- *  Vertices belonging to each component are marked with a unique integer
- *  in the range [0,K), where K is the number of components.
- *
- *  Parameters
- *      num_rows             - number of rows in A (number of vertices)
- *      Ap[]                 - CSR row pointer
- *      Aj[]                 - CSR index array
- *      components[num_rows] - component labels
+ * Compute the connected components of a graph stored in CSR format.
  *
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A (number of vertices)
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * components : array, num_rows
+ *     component labels
+ *
+ * Notes
+ * -----
+ * Vertices belonging to each component are marked with a unique integer
+ * in the range [0,K), where K is the number of components.
  */
 template <class I>
 I connected_components(const I num_nodes,
                        const I Ap[], const int Ap_size,
                        const I Aj[], const int Aj_size,
                              I components[], const int components_size)
 {
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/graph_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/graph_bind.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -432,62 +432,83 @@
     py::options options;
     options.disable_function_signatures();
 
     m.def("maximal_independent_set_serial", &_maximal_independent_set_serial<int, int>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("active"), py::arg("C"), py::arg("F"), py::arg("x").noconvert(),
 R"pbdoc(
 Compute a maximal independent set for a graph stored in CSR format
- using a greedy serial algorithm
+using a greedy serial algorithm
 
- Parameters
-     num_rows   - number of rows in A (number of vertices)
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     active     - value used for active vertices        (input)
-      C         - value used to mark non-MIS vertices   (output)
-      F         - value used to mark MIS vertices       (output)
-     x[]        - state of each vertex
-
-
- Returns:
-     The number of nodes in the MIS.
-
- Notes:
-     Only the vertices with values with x[i] == active are considered
-     when determining the MIS.  Upon return, all active vertices will
-     be assigned the value C or F depending on whether they are in the
-     MIS or not.)pbdoc");
+Parameters
+----------
+num_rows : int
+    Number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+active : float-like
+    Value used for active vertices
+C : float-like
+    Value used to mark non-MIS vertices
+F : float-like
+    Value used to mark MIS vertices
+x : array, inplace output
+    State of each vertex
+
+Returns
+-------
+N : int
+    The number of nodes in the MIS.
+
+Notes
+-----
+Only the vertices with values with x[i] == active are considered
+when determining the MIS.  Upon return, all active vertices will
+be assigned the value C or F depending on whether they are in the
+MIS or not.)pbdoc");
 
     m.def("maximal_independent_set_parallel", &_maximal_independent_set_parallel<int, int, double>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("active"), py::arg("C"), py::arg("F"), py::arg("x").noconvert(), py::arg("y").noconvert(), py::arg("max_iters"),
 R"pbdoc(
 Compute a maximal independent set for a graph stored in CSR format
  using a variant of Luby's parallel MIS algorithm
 
  Parameters
-     num_rows   - number of rows in A (number of vertices)
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     active     - value used for active vertices        (input)
-      C         - value used to mark non-MIS vertices   (output)
-      F         - value used to mark MIS vertices       (output)
-     x[]        - state of each vertex
-     y[]        - random values for each vertex
-     max_iters  - maximum number of iterations
-                  by default max_iters=-1 and no limit
-                  is imposed
+ ----------
+ num_rows : int
+     number of rows in A (number of vertices)
+ Ap : array
+     CSR row pointer
+ Aj : array
+     CSR index array
+ active : float
+     value used for active vertices
+ C : float
+     value used to mark non-MIS vertices
+ F : float
+     value used to mark MIS vertices
+ x : array, output
+     state of each vertex
+ y : array
+     random values for each vertex
+ max_iters : int
+     maximum number of iterations By default max_iters=-1 and no limit is imposed
 
- Returns:
+ Returns
+ -------
+ N : int
      The number of nodes in the MIS.
 
- Notes:
-     Only the vertices with values with x[i] == active are considered
-     when determining the MIS.  Upon return, all active vertices will
-     be assigned the value C or F depending on whether they are in the
-     MIS or not.)pbdoc");
+ Notes
+ -----
+ Only the vertices with values with x[i] == active are considered
+ when determining the MIS.  Upon return, all active vertices will
+ be assigned the value C or F depending on whether they are in the
+ MIS or not.)pbdoc");
 
     m.def("vertex_coloring_mis", &_vertex_coloring_mis<int, int>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("x").noconvert(),
 R"pbdoc(
 Compute a vertex coloring for a graph stored in CSR format.
 
  The coloring is computed by removing maximal independent sets
@@ -500,236 +521,319 @@
  of the i-th vertex.)pbdoc");
 
     m.def("vertex_coloring_jones_plassmann", &_vertex_coloring_jones_plassmann<int, int, double>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("x").noconvert(), py::arg("z").noconvert(),
 R"pbdoc(
 Compute a vertex coloring of a graph using the Jones-Plassmann algorithm
 
- Parameters
-     num_rows   - number of rows in A (number of vertices)
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     x[]        - color of each vertex
-     y[]        - initial random values for each vertex
-
- Notes:
-     Arrays x and y will be overwritten
-
- References:
-     Mark T. Jones and Paul E. Plassmann
-     A Parallel Graph Coloring Heuristic
-     SIAM Journal on Scientific Computing 14:3 (1993) 654--669
-     http://citeseer.ist.psu.edu/jones92parallel.html)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+x : array, inplace
+    color of each vertex
+y : array
+    initial random values for each vertex
+
+Notes
+-----
+    Arrays x and y will be overwritten
+
+References
+----------
+.. [Jones92] Mark T. Jones and Paul E. Plassmann
+   A Parallel Graph Coloring Heuristic
+   SIAM Journal on Scientific Computing 14:3 (1993) 654--669
+   http://citeseer.ist.psu.edu/jones92parallel.html)pbdoc");
 
     m.def("vertex_coloring_LDF", &_vertex_coloring_LDF<int, int, double>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("x").noconvert(), py::arg("y").noconvert(),
 R"pbdoc(
 Compute a vertex coloring of a graph using the parallel
 Largest-Degree-First (LDF) algorithm
 
- Parameters
-     num_rows   - number of rows in A (number of vertices)
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     x[]        - color of each vertex
-     y[]        - initial random values for each vertex
-
-  References:
-    J. R. Allwright and R. Bordawekar and P. D. Coddington and K. Dincer and C. L. Martin
-    A Comparison of Parallel Graph Coloring Algorithms
-    DRAFT SCCS-666
-    http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.45.4650)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+x : array
+    color of each vertex
+y : array
+    initial random values for each vertex
+
+References
+----------
+.. [LDF] J. R. Allwright and R. Bordawekar and P. D. Coddington and K. Dincer and C. L. Martin
+   A Comparison of Parallel Graph Coloring Algorithms
+   DRAFT SCCS-666
+   http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.45.4650)pbdoc");
 
     m.def("cluster_node_incidence", &_cluster_node_incidence<int>,
         py::arg("num_nodes"), py::arg("num_clusters"), py::arg("cm").noconvert(), py::arg("ICp").noconvert(), py::arg("ICi").noconvert(), py::arg("L").noconvert(),
 R"pbdoc(
 Compute the incidence matrix for a clustering
 
-     I = Incidence matrix between nodes and clusters (num_nodes x num_clusters)
+Parameters
+----------
+num_nodes : int
+    number of nodes
+num_clusters : int
+    number of clusters
+cm : array, num_nodes
+    cluster index for each node
+ICp : arrayt, num_clusters+1, inplace
+    CSC column pointer array for I
+ICi : array, num_nodes, inplace
+    CSC column indexes for I
+L : array, num_nodes, inplace
+    Local index mapping
+
+Notes
+-----
+I = Incidence matrix between nodes and clusters (num_nodes x num_clusters)
 I[i,a] = 1 if node i is in cluster a, otherwise 0
 
-    Cluster indexes: a,b,c in 1..num_clusters
+Cluster indexes: a,b,c in 1..num_clusters
 Global node indexes: i,j,k in 1..num_rows
- Local node indexes: pair (a,m) where a is cluster and m in 1..num_nodes_in_cluster
+Local node indexes: pair (a,m) where a is cluster and m in 1..num_nodes_in_cluster
 
 We store I in both CSC and CSR formats because we want to be able
 to map global <-> local node indexes. However, I in CSR format is
 simply the cm array, so we only need to compute CSC format.
 
-IC = (ICp,ICi)    = I in CSC format (don't store ICx because it's
-                    always 1).
+IC = (ICp,ICi)    = I in CSC format (don't store ICx because it's always 1).
 
 IR = (IRa) = (cm) = I in CSR format (don't store IRp because we
-                    have exactly one nonzero entry per row, and
-                    don't store IRx because it's always 1). This is
-                    just the cm array.
+have exactly one nonzero entry per row, and don't store IRx because it's always 1). This is
+just the cm array.
 
 Converting local (a,m) -> global i:   i = ICi[ICp[a] + m]
+Converting global i -> local (a,m):   a = cm[i], m = L[i]
 
-Converting global i -> local (a,m):   a = cm[i]
-                                      m = L[i]
-
-L is an additional vector (length num_rows) to store local indexes.
-
- Parameters
-     num_nodes         - (IN)  number of nodes
-     num_clusters      - (IN)  number of clusters
-    cm[num_nodes]      - (IN)  cluster index for each node
-   ICp[num_clusters+1] - (OUT) CSC column pointer array for I
-   ICi[num_nodes]      - (OUT) CSC column indexes for I
-     L[num_nodes]      - (OUT) Local index mapping)pbdoc");
+L is an additional vector (length num_rows) to store local indexes.)pbdoc");
 
     m.def("cluster_center", &_cluster_center<int, int>,
         py::arg("a"), py::arg("num_nodes"), py::arg("num_clusters"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("cm").noconvert(), py::arg("ICp").noconvert(), py::arg("ICi").noconvert(), py::arg("L").noconvert());
     m.def("cluster_center", &_cluster_center<int, float>,
         py::arg("a"), py::arg("num_nodes"), py::arg("num_clusters"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("cm").noconvert(), py::arg("ICp").noconvert(), py::arg("ICi").noconvert(), py::arg("L").noconvert());
     m.def("cluster_center", &_cluster_center<int, double>,
         py::arg("a"), py::arg("num_nodes"), py::arg("num_clusters"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("cm").noconvert(), py::arg("ICp").noconvert(), py::arg("ICi").noconvert(), py::arg("L").noconvert(),
 R"pbdoc(
 Apply Floyd–Warshall to cluster "a" and use the result to find the
 cluster center
 
- Parameters
-     a                  - (IN) cluster index to find the center of
-     num_nodes          - (IN) number of nodes
-     num_clusters       - (IN) number of clusters
-     Ap[]               - (IN) CSR row pointer
-     Aj[]               - (IN) CSR index array
-     Ax[]               - (IN) CSR data array (edge lengths)
-     cm[num_nodes]      - (IN) cluster index for each node
-    ICp[num_clusters+1] - (IN) CSC column pointer array for I
-    ICi[num_nodes]      - (IN) CSC column indexes for I
-      L[num_nodes]      - (IN) Local index mapping
-
- Returns
-     i                  - global node index of center of cluster a
-
- References:
-     https://en.wikipedia.org/wiki/Graph_center
-     https://en.wikipedia.org/wiki/Floyd–Warshall_algorithm
-     https://en.wikipedia.org/wiki/Distance_(graph_theory))pbdoc");
+Parameters
+----------
+a : int
+    cluster index to find the center of
+num_nodes : int
+    number of nodes
+num_clusters : int
+    number of clusters
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array (edge lengths)
+cm : array, num_nodes
+    cluster index for each node
+ICp : array, num_clusters+1
+    CSC column pointer array for I
+ICi : array, num_nodes
+    CSC column indexes for I
+L : array, num_nodes
+    Local index mapping
+
+Returns
+-------
+i : int
+    global node index of center of cluster a
+
+References
+----------
+.. [1] Graph Center:   https://en.wikipedia.org/wiki/Graph_center
+.. [2] Floyd-Warshall: https://en.wikipedia.org/wiki/Floyd–Warshall_algorithm
+.. [3] Graph Distance: https://en.wikipedia.org/wiki/Distance_(graph_theory))pbdoc");
 
     m.def("bellman_ford", &_bellman_ford<int, int>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("d").noconvert(), py::arg("cm").noconvert());
     m.def("bellman_ford", &_bellman_ford<int, float>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("d").noconvert(), py::arg("cm").noconvert());
     m.def("bellman_ford", &_bellman_ford<int, double>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("d").noconvert(), py::arg("cm").noconvert(),
 R"pbdoc(
 Apply one iteration of Bellman-Ford iteration on a distance
 graph stored in CSR format.
 
- Parameters
-     num_nodes - (IN)    number of nodes (number of rows in A)
-     Ap[]      - (IN)    CSR row pointer
-     Aj[]      - (IN)    CSR index array
-     Ax[]      - (IN)    CSR data array (edge lengths)
-     d[]       - (INOUT) distance to nearest center
-    cm[]       - (INOUT) cluster index for each node
-
- References:
-     http://en.wikipedia.org/wiki/Bellman-Ford_algorithm)pbdoc");
+Parameters
+----------
+num_nodes : int
+    number of nodes (number of rows in A)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array (edge lengths)
+d : array, inplace
+    distance to nearest center
+cm : array, inplace
+    cluster index for each node
+
+References
+----------
+.. [1] Bellman-Ford Wikipedia: http://en.wikipedia.org/wiki/Bellman-Ford_algorithm)pbdoc");
 
     m.def("lloyd_cluster", &_lloyd_cluster<int, int>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert());
     m.def("lloyd_cluster", &_lloyd_cluster<int, float>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert());
     m.def("lloyd_cluster", &_lloyd_cluster<int, double>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert(),
 R"pbdoc(
 Perform one iteration of Lloyd clustering on a distance graph
 
- Parameters
-     num_nodes       - (IN)  number of nodes (number of rows in A)
-     Ap[]            - (IN)  CSR row pointer for adjacency matrix A
-     Aj[]            - (IN)  CSR index array
-     Ax[]            - (IN)  CSR data array (edge lengths)
-     num_clusters    - (IN)  number of clusters (seeds)
-     d[num_nodes]    - (OUT) distance to nearest seed
-    cm[num_nodes]    - (OUT) cluster index for each node
-     c[num_clusters] - (INOUT)  cluster centers
-
- References
-     Nathan Bell
-     Algebraic Multigrid for Discrete Differential Forms
-     PhD thesis (UIUC), August 2008)pbdoc");
+Parameters
+----------
+num_nodes : int
+    number of nodes (number of rows in A)
+Ap : array
+    CSR row pointer for adjacency matrix A
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array (edge lengths)
+num_clusters : int
+    number of clusters (seeds)
+d : array, num_nodes
+    distance to nearest seed
+cm : array, num_nodes
+    cluster index for each node
+c : array, num_clusters
+    cluster centers
+
+References
+----------
+.. [Bell2008] Nathan Bell, Algebraic Multigrid for Discrete Differential Forms
+   PhD thesis (UIUC), August 2008)pbdoc");
 
     m.def("lloyd_cluster_exact", &_lloyd_cluster_exact<int, int>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert());
     m.def("lloyd_cluster_exact", &_lloyd_cluster_exact<int, float>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert());
     m.def("lloyd_cluster_exact", &_lloyd_cluster_exact<int, double>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("num_clusters"), py::arg("d").noconvert(), py::arg("cm").noconvert(), py::arg("c").noconvert(),
 R"pbdoc(
 Perform one iteration of Lloyd clustering on a distance graph using
 exact centers
 
+Parameters
+----------
+num_nodes : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array (edge lengths)
+num_clusters : int
+    number of clusters = number of seeds
+d : array, num_nodes
+    distance to nearest seed
+cm : array, num_nodes
+    cluster index for each node
+c : array, num_clusters
+    cluster centers
+
+Notes
+-----
 This version computes exact cluster centers with Floyd-Warshall and
 also uses a balanced version of Bellman-Ford to try and find
-nearly-equal-sized clusters.
-
- Parameters
-     num_nodes       - (IN)  number of rows in A (number of vertices)
-     Ap[]            - (IN)  CSR row pointer
-     Aj[]            - (IN)  CSR index array
-     Ax[]            - (IN)  CSR data array (edge lengths)
-     num_clusters    - (IN)  number of clusters = number of seeds
-     d[num_nodes]    - (OUT) distance to nearest seed
-    cm[num_nodes]    - (OUT) cluster index for each node
-     c[num_clusters] - (IN)  cluster centers
-
- References
-     Nathan Bell
-     Algebraic Multigrid for Discrete Differential Forms
-     PhD thesis (UIUC), August 2008)pbdoc");
+nearly-equal-sized clusters.)pbdoc");
 
     m.def("maximal_independent_set_k_parallel", &_maximal_independent_set_k_parallel<int, int, double>,
         py::arg("num_rows"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("k"), py::arg("x").noconvert(), py::arg("y").noconvert(), py::arg("max_iters"),
 R"pbdoc(
-Compute a distance-k maximal independent set for a graph stored
- in CSR format using a parallel algorithm.  An MIS-k is a set of
- vertices such that all vertices in the MIS-k are separated by a
- path of at least K+1 edges and no additional vertex can be added
- to the set without destroying this property.  A standard MIS
- is therefore a MIS-1.
+Compute MIS-k.
 
- Parameters
-     num_rows   - number of rows in A (number of vertices)
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     k          - minimum separation between MIS vertices
-     x[]        - state of each vertex (1 if in the MIS, 0 otherwise)
-     y[]        - random values used during parallel MIS algorithm
-     max_iters  - maximum number of iterations to use (default, no limit))pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+k : int
+    minimum separation between MIS vertices
+x : array, inplace
+    state of each vertex (1 if in the MIS, 0 otherwise)
+y : array
+    random values used during parallel MIS algorithm
+max_iters : int
+    maximum number of iterations to use (default, no limit)
+
+Notes
+-----
+Compute a distance-k maximal independent set for a graph stored
+in CSR format using a parallel algorithm.  An MIS-k is a set of
+vertices such that all vertices in the MIS-k are separated by a
+path of at least K+1 edges and no additional vertex can be added
+to the set without destroying this property.  A standard MIS
+is therefore a MIS-1.)pbdoc");
 
     m.def("breadth_first_search", &_breadth_first_search<int>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("seed"), py::arg("order").noconvert(), py::arg("level").noconvert(),
 R"pbdoc(
 Compute a breadth first search of a graph in CSR format
- beginning at a given seed vertex.
+beginning at a given seed vertex.
 
- Parameters
-     num_rows         - number of rows in A (number of vertices)
-     Ap[]             - CSR row pointer
-     Aj[]             - CSR index array
-     order[num_rows]  - records the order in which vertices were searched
-     level[num_rows]  - records the level set of the searched vertices (i.e. the minimum distance to the seed)
-
- Notes:
-     The values of the level must be initialized to -1)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+order : array, num_rows, inplace
+    records the order in which vertices were searched
+level : array, num_rows, inplace
+    records the level set of the searched vertices (i.e. the minimum distance to the seed)
+
+Notes
+-----
+The values of the level must be initialized to -1)pbdoc");
 
     m.def("connected_components", &_connected_components<int>,
         py::arg("num_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("components").noconvert(),
 R"pbdoc(
 Compute the connected components of a graph stored in CSR format.
 
- Vertices belonging to each component are marked with a unique integer
- in the range [0,K), where K is the number of components.
-
- Parameters
-     num_rows             - number of rows in A (number of vertices)
-     Ap[]                 - CSR row pointer
-     Aj[]                 - CSR index array
-     components[num_rows] - component labels)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A (number of vertices)
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+components : array, num_rows
+    component labels
+
+Notes
+-----
+Vertices belonging to each component are marked with a unique integer
+in the range [0,K), where K is the number of components.)pbdoc");
 
 }
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/instantiate.yml` & `pyamg-4.2.3/pyamg/amg_core/instantiate.yml`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/krylov.h` & `pyamg-4.2.3/pyamg/amg_core/krylov.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #ifndef KRYLOV_H
 #define KRYLOV_H
 
 #include "linalg.h"
 
-/* Apply |start-stop| Householder reflectors in B to z
+/* Apply Householder reflectors in B to z
  *
  * Implements the below python
  *
- * for j in range(start,stop,step):
- *   z = z - 2.0*dot(conjugate(B[j,:]), v)*B[j,:]
+ * .. code-block:: python
+ *
+ *     for j in range(start,stop,step):
+ *       z = z - 2.0*dot(conjugate(B[j,:]), v)*B[j,:]
  *
  * Parameters
  * ----------
- * z : {float array}
- *  length n vector to be operated on
- * B : {float array}
- *  n x m matrix of householder reflectors
- *  must be in row major form
- * n : {int}
- *  dimensionality of z
- * start, stop, step : {int}
- *  control the choice of vectors in B to use
+ * z : array
+ *     length n vector to be operated on
+ * B : array
+ *     n x m matrix of householder reflectors
+ *     must be in row major form
+ * n : int
+ *     dimensionality of z
+ * start, stop, step : int
+ *     control the choice of vectors in B to use
  *
  * Returns
  * -------
  * z is modified in place to reflect the application of
  * the Householder reflectors, B[:,range(start,stop,step)]
  *
  * Notes
@@ -52,50 +54,54 @@
     }
 }
 
 /* For use after gmres is finished iterating and the least squares
  * solution has been found.  This routine maps the solution back to
  * the original space via the Householder reflectors.
  *
- * Apply |start-stop| Householder reflectors in B to z
+ * Apply Householder reflectors in B to z
  * while also adding in the appropriate value from y, so
  * that we follow the Horner-like scheme to map our least squares
  * solution in y back to the original space
  *
  * Implements the below python
  *
- * for j in range(inner,-1,-1):
- *  z[j] += y[j]
- *  # Apply j-th reflector, (I - 2.0*w_j*w_j.T)*update
- *  z = z - 2.0*dot(conjugate(B[j,:]), update)*B[j,:]
+ * .. code-block:: python
+ *
+ *     for j in range(inner,-1,-1):
+ *       z[j] += y[j]
+ *       # Apply j-th reflector, (I - 2.0*w_j*w_j.T)*update
+ *       z = z - 2.0*dot(conjugate(B[j,:]), update)*B[j,:]
  *
  * Parameters
  * ----------
- * z : {float array}
- *  length n vector to be operated on
- * B : {float array}
- *  n x m matrix of householder reflectors
- *  must be in row major form
- * y : {float array}
- *  solution to the reduced system at the end of GMRES
- * n : {int}
- *  dimensionality of z
- * start, stop, step : {int}
- *  control the choice of vectors in B to use
+ * z : array
+ *     length n vector to be operated on
+ * B : array
+ *     n x m matrix of householder reflectors
+ *     must be in row major form
+ * y : array
+ *     solution to the reduced system at the end of GMRES
+ * n : int
+ *     dimensionality of z
+ * start, stop, step : int
+ *     control the choice of vectors in B to use
  *
  * Returns
  * -------
  * z is modified in place to reflect the application of
  * the Householder reflectors, B[:,range(start,stop,step)],
  * and the inclusion of values in y.
  *
  * Notes
  * -----
  * Principle calling routine is gmres(...) and fgmres(...) in krylov.py
  *
+ * References
+ * ----------
  * See pages 164-167 in Saad, "Iterative Methods for Sparse Linear Systems"
  */
 template<class I, class T, class F>
 void householder_hornerscheme(      T z[], const int z_size,
                                const T B[], const int B_size,
                                const T y[], const int y_size,
                                const I n,
@@ -120,23 +126,23 @@
 }
 
 
 /* Apply the first nrot Givens rotations in B to x
  *
  * Parameters
  * ----------
- * x : {float array}
- *  n-vector to be operated on
- * B : {float array}
- *  Each 4 entries represent a Givens rotation
- *  length nrot*4
- * n : {int}
- *  dimensionality of x
- * nrot : {int}
- *  number of rotations in B
+ * x : array
+ *     n-vector to be operated on
+ * B : array
+ *     Each 4 entries represent a Givens rotation
+ *     length nrot*4
+ * n : int
+ *     dimensionality of x
+ * nrot : int
+ *     number of rotations in B
  *
  * Returns
  * -------
  * x is modified in place to reflect the application of the nrot
  * rotations in B.  It is assumed that the first rotation operates on
  * degrees of freedom 0 and 1.  The second rotation operates on dof's 1 and 2,
  * and so on
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/krylov_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/krylov_bind.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -102,32 +102,34 @@
     m.def("apply_householders", &_apply_householders<int, double, double>,
         py::arg("z").noconvert(), py::arg("B").noconvert(), py::arg("n"), py::arg("start"), py::arg("stop"), py::arg("step"));
     m.def("apply_householders", &_apply_householders<int, std::complex<float>, float>,
         py::arg("z").noconvert(), py::arg("B").noconvert(), py::arg("n"), py::arg("start"), py::arg("stop"), py::arg("step"));
     m.def("apply_householders", &_apply_householders<int, std::complex<double>, double>,
         py::arg("z").noconvert(), py::arg("B").noconvert(), py::arg("n"), py::arg("start"), py::arg("stop"), py::arg("step"),
 R"pbdoc(
-Apply |start-stop| Householder reflectors in B to z
+Apply Householder reflectors in B to z
 
 Implements the below python
 
-for j in range(start,stop,step):
-  z = z - 2.0*dot(conjugate(B[j,:]), v)*B[j,:]
+.. code-block:: python
+
+    for j in range(start,stop,step):
+      z = z - 2.0*dot(conjugate(B[j,:]), v)*B[j,:]
 
 Parameters
 ----------
-z : {float array}
- length n vector to be operated on
-B : {float array}
- n x m matrix of householder reflectors
- must be in row major form
-n : {int}
- dimensionality of z
-start, stop, step : {int}
- control the choice of vectors in B to use
+z : array
+    length n vector to be operated on
+B : array
+    n x m matrix of householder reflectors
+    must be in row major form
+n : int
+    dimensionality of z
+start, stop, step : int
+    control the choice of vectors in B to use
 
 Returns
 -------
 z is modified in place to reflect the application of
 the Householder reflectors, B[:,range(start,stop,step)]
 
 Notes
@@ -143,50 +145,54 @@
     m.def("householder_hornerscheme", &_householder_hornerscheme<int, std::complex<double>, double>,
         py::arg("z").noconvert(), py::arg("B").noconvert(), py::arg("y").noconvert(), py::arg("n"), py::arg("start"), py::arg("stop"), py::arg("step"),
 R"pbdoc(
 For use after gmres is finished iterating and the least squares
 solution has been found.  This routine maps the solution back to
 the original space via the Householder reflectors.
 
-Apply |start-stop| Householder reflectors in B to z
+Apply Householder reflectors in B to z
 while also adding in the appropriate value from y, so
 that we follow the Horner-like scheme to map our least squares
 solution in y back to the original space
 
 Implements the below python
 
-for j in range(inner,-1,-1):
- z[j] += y[j]
- # Apply j-th reflector, (I - 2.0*w_j*w_j.T)*update
- z = z - 2.0*dot(conjugate(B[j,:]), update)*B[j,:]
+.. code-block:: python
+
+    for j in range(inner,-1,-1):
+      z[j] += y[j]
+      # Apply j-th reflector, (I - 2.0*w_j*w_j.T)*update
+      z = z - 2.0*dot(conjugate(B[j,:]), update)*B[j,:]
 
 Parameters
 ----------
-z : {float array}
- length n vector to be operated on
-B : {float array}
- n x m matrix of householder reflectors
- must be in row major form
-y : {float array}
- solution to the reduced system at the end of GMRES
-n : {int}
- dimensionality of z
-start, stop, step : {int}
- control the choice of vectors in B to use
+z : array
+    length n vector to be operated on
+B : array
+    n x m matrix of householder reflectors
+    must be in row major form
+y : array
+    solution to the reduced system at the end of GMRES
+n : int
+    dimensionality of z
+start, stop, step : int
+    control the choice of vectors in B to use
 
 Returns
 -------
 z is modified in place to reflect the application of
 the Householder reflectors, B[:,range(start,stop,step)],
 and the inclusion of values in y.
 
 Notes
 -----
 Principle calling routine is gmres(...) and fgmres(...) in krylov.py
 
+References
+----------
 See pages 164-167 in Saad, "Iterative Methods for Sparse Linear Systems")pbdoc");
 
     m.def("apply_givens", &_apply_givens<int, float, float>,
         py::arg("B").noconvert(), py::arg("x").noconvert(), py::arg("n"), py::arg("nrot"));
     m.def("apply_givens", &_apply_givens<int, double, double>,
         py::arg("B").noconvert(), py::arg("x").noconvert(), py::arg("n"), py::arg("nrot"));
     m.def("apply_givens", &_apply_givens<int, std::complex<float>, float>,
@@ -194,23 +200,23 @@
     m.def("apply_givens", &_apply_givens<int, std::complex<double>, double>,
         py::arg("B").noconvert(), py::arg("x").noconvert(), py::arg("n"), py::arg("nrot"),
 R"pbdoc(
 Apply the first nrot Givens rotations in B to x
 
 Parameters
 ----------
-x : {float array}
- n-vector to be operated on
-B : {float array}
- Each 4 entries represent a Givens rotation
- length nrot*4
-n : {int}
- dimensionality of x
-nrot : {int}
- number of rotations in B
+x : array
+    n-vector to be operated on
+B : array
+    Each 4 entries represent a Givens rotation
+    length nrot*4
+n : int
+    dimensionality of x
+nrot : int
+    number of rotations in B
 
 Returns
 -------
 x is modified in place to reflect the application of the nrot
 rotations in B.  It is assumed that the first rotation operates on
 degrees of freedom 0 and 1.  The second rotation operates on dof's 1 and 2,
 and so on
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/linalg.h` & `pyamg-4.2.3/pyamg/amg_core/linalg.h`

 * *Files 4% similar despite different names*

```diff
@@ -128,24 +128,25 @@
  *      templated for pyamg's complex class, float and double
  *******************************************************************/
 
 /* dot(x, y, n)
  *
  * Parameters
  * ----------
- * x : {float|complex array}
- *      n-vector
- * y : {float|complex array}
- *      n-vector
- * n : {int}
- *      size of x and y
- *
- * Return
- * ------
- * conjugate(x).T y
+ * x : array
+ *     n-vector
+ * y : array
+ *     n-vector
+ * n : int
+ *     size of x and y
+ *
+ * Returns
+ * -------
+ * float
+ *     conjugate(x).T y
  *
  */
 template<class I, class T>
 inline T dot_prod(const T x[], const T y[], const I n)
 {
     T sum = 0.0;
     for( I i = 0; i < n; i++)
@@ -154,71 +155,75 @@
 }
 
 
 /* norm(x, n)
  *
  * Parameters
  * ----------
- * x : {float|complex array}
- *      n-vector
- * n : {int}
- *      size of x and y
- * normx : {scalar}
- *      output value
- *
- * Return
- * ------
- * normx = sqrt( <x, x> )
+ * x : array
+ *     n-vector
+ * n : int
+ *     size of x and y
+ * normx : float
+ *     output value
+ *
+ * Returns
+ * -------
+ * float
+ *     normx = sqrt( <x, x> )
  *
  */
 template<class I, class T, class F>
 inline void norm(const T x[], const I n, F &normx)
 {
     normx = sqrt(real(dot_prod(x,x,n)));
 }
 
 
 /* axpy(x, y, alpha, n)
  *
  * Parameters
  * ----------
- * x : {float|complex array}
- *      n-vector
- * y : {float|complex array}
- *      n-vector
- * n : {int}
- *      size of x and y
- * alpha : {scalar}
- *
- * Return
- * ------
- * x = x + alpha*y
- *
+ * x : array
+ *     n-vector
+ * y : array
+ *     n-vector
+ * n : int
+ *     size of x and y
+ * alpha : float
+ *     value to scale with
+ *
+ * Returns
+ * -------
+ * x : float
+ *     x = x + alpha*y
  */
 template<class I, class T>
 inline void axpy(T x[], const T y[], const T alpha, const I n)
 {
     for( I i = 0; i < n; i++)
     {   x[i] += alpha*y[i]; }
 }
 
 
 /* Transpose Ax by overwriting Bx
  *
  * Parameters
  * ----------
- * Ax : {float|complex array}
+ * Ax : array
  *      m x n dense array
- * Bx : {float|complex array}
+ * Bx :array
  *      m x n dense array
- * m,n : {int}
- *      Dimensions of Ax and Bx
+ * m : int
+ *      Dimensions of Ax
+ * n : int
+ *      Dimensions of Bx
  *
- * Return
- * ------
+ * Returns
+ * -------
  * Bx is overwritten with the transpose of Ax
  *
  * Notes
  * -----
  * There is a fair amount of hard-coding to make this routine very
  * fast for small (<10) square matrices, although it works for general
  * m x n matrices.
@@ -305,60 +310,57 @@
 }
 
 
 /* Calculate Ax*Bx = S
  *
  * Parameters
  * ----------
- * Ax : {float|complex array}
+ * Ax : array
  *      Stored in row major
- * Arows : {int}
+ * Arows : int
  *      Number of rows of A
- * Acols : {int}
+ * Acols : int
  *      Number of columns of A
- * Atrans : {char}
+ * Atrans : char
  *      Not Used
- * Bx : {float|complex array}
+ * Bx : array
  *      Stored in col major
- * Brows : {int}
+ * Brows : int
  *      Number of rows of B
- * Bcols : {int}
+ * Bcols : int
  *      Number of columns of B
- * Btrans : {char}
+ * Btrans : char
  *      Supported, essentially Btrans='F' assumes
  *      B is in column major, and Brans='T' assumes
  *      B is in row major
- * Sx : {float|complex array}
+ * Sx : array
  *      Output array, Contents are overwritten
- * Srows : {int}
+ * Srows : int
  *      Number of rows of S
- * Scols : {int}
+ * Scols : int
  *      Number of columns of S
- * Strans : {char}
+ * Strans : char
  *      'T' gives S in col major (only works with Btrans='F')
  *      'F' gives S in row major
  * overwrite : {char}
  *      'T' overwrite S
  *      'F' accumulate to S
  *
- *
- * Return
- * ------
- * Sx = Ax*Bx in column or row major, depending on Strans.
+ * Returns
+ * -------
+ * Modified inplace: Sx = Ax*Bx in column or row major, depending on Strans.
  *
  * Notes
  * -----
- *  Supported matrix format combinations,
- *  Btrans = 'F' and Strans = 'T'
- *  Btrans = 'F' and Strans = 'F'
- *  Btrans = 'T' and Strans = 'F'
- *
- *  All other combinations are not yet supported
- *
+ * Supported matrix format combinations,
+ * - Btrans = 'F' and Strans = 'T'
+ * - Btrans = 'F' and Strans = 'F'
+ * - Btrans = 'T' and Strans = 'F'
  *
+ * All other combinations are not yet supported
  */
 template<class I, class T>
 inline void gemm(const T Ax[], const I Arows, const I Acols, const char Atrans,
           const T Bx[], const I Brows, const I Bcols, const char Btrans,
           T Sx[], const I Srows, const I Scols, const char Strans,
           const char overwrite)
 {
@@ -451,44 +453,46 @@
 
 /*
  * Compute the SVD of a matrix, Ax, using the Jacobi method.
  * Compute Ax = U S V.H
  *
  * Parameters
  * ----------
- * Ax : {float|complex array}
- *      m x n dense matrix, stored in col major form
- * U : {float|complex array}
- *      m x n dense matrix initialized to 0.0
- *      Passed in as Tx
- * V : {float|complex array}
- *      n x n dense matrix initialized to 0.0
- *      Passed in as Bx
- * S : {float|complex array}
- *      n x 1 dense matrix initialized to 0.0
- *      Passed in as Sx
- * m,n : {int}
+ * Ax : array
+ *     m x n dense matrix, stored in col major form
+ * U : array
+ *     m x n dense matrix initialized to 0.0
+ *     Passed in as Tx
+ * V : array
+ *     n x n dense matrix initialized to 0.0
+ *     Passed in as Bx
+ * S : array
+ *     n x 1 dense matrix initialized to 0.0
+ *     Passed in as Sx
+ * m,n : int
  *      Dimensions of Ax, m > n.
  *
- * Return
- * ------
+ * Returns
+ * -------
  * Returns Ax = U S V.H
  * U, V, S are modified in place
  *
- * V : {array}
+ * V : array
  *      Orthogonal n x n matrix, V, stored in col major
- * U : {array}
+ * U : array
  *      Orthogonal m x n matrix, U, stored in col major
- * S : {array}
+ * S : array
  *      Singular values
- * int : {int}
+ * int : int
  *      Function return value,
- *      -1:  error
- *      0:  successful
- *      1:  did not converge
+        ==  =====================
+ *      -1  error
+ *       0  successful
+ *       1  did not converge
+        ==  =====================
  *
  * Notes
  * -----
  * The Jacobi method is used to compute the SVD.  Conceptually,
  * the Jacobi method applies successive Jacobi rotations, Q_i to
  * the system, Q_i^H Ax.H Ax Q_i.  Despite the normal equations
  * appearing here, the actual method can be quite accurate.
@@ -501,15 +505,15 @@
  * De Rijk, "A One-Sided Jacobi Algorithm for computing the singular value
  * decomposition on a vector computer", SIAM J Sci and Statistical Comp,
  * Vol 10, No 2, p 359-371, March 1989.
  *
  */
 
 template<class I, class T, class F>
-I svd_jacobi (const T Ax[], T Tx[], T Bx[], F Sx[], const I m, const I n)
+I svd_jacobi(const T Ax[], T Tx[], T Bx[], F Sx[], const I m, const I n)
 {
     // Not implemented for m < n matrices
     if( m < n)
     {   return -1; }
 
     // Rename
     const T * A = Ax;
@@ -766,29 +770,29 @@
 
 /*
  * Solve a system with the SVD, i.e. use a robust Moore-Penrose
  * Pseudoinverse to multiply the RHS
  *
  * Parameters
  * ----------
- * A : {float|complex array}
- *      m x n dense column major array, m>n
- * m,n : {int}
- *      Dimensions of A, m > n
- * b : {float|complex array}
- *      RHS, m-vector
+ * A : array
+ *     m x n dense column major array, m>n
+ * m,n : int
+ *     Dimensions of A, m > n
+ * b : array
+ *     RHS, m-vector
  * sing_vals : {float array}
- *      Holds the singular values upon return
- * work : {float|complex array}
- *      worksize array for temporary space for routine
- * worksize : {int}
- *      must be > m*n + n
+ *     Holds the singular values upon return
+ * work : array
+ *     worksize array for temporary space for routine
+ * worksize : int
+ *     must be > m*n + n
  *
- * Return
- * ------
+ * Returns
+ * -------
  * A^{-1} b replaces b
  * sing_vals holds the singular values
  *
  * Notes
  * -----
  * forcing preallocation of sing_vals and work, allows for
  * efficient multiple calls to this routine
@@ -839,29 +843,30 @@
          &(b[0]), n, 1, trans, 'T');
 
     return;
 }
 
 /* Replace each block of A with a Moore-Penrose pseudoinverse of that block.
  * Routine is designed to invert many small matrices at once.
+ *
  * Parameters
  * ----------
- * AA : {float|complex array}
- *      (m, n, n) array, assumed to be "raveled" and in row major form
+ * AA : array
+ *     (m, n, n) array, assumed to be "raveled" and in row major form
  * m,n : int
- *      dimensions of AA
+ *     dimensions of AA
  * TransA : char
- *      'T' or 'F'.  Decides whether to transpose each nxn block
- *      of A before inverting.  If using Python array, should be 'T'.
+ *     'T' or 'F'.  Decides whether to transpose each nxn block
+ *     of A before inverting.  If using Python array, should be 'T'.
  *
- * Return
- * ------
- * AA : {array}
- *      AA is modified in place with the pseduoinverse replacing each
- *      block of AA.  AA is returned in row-major form for Python
+ * Returns
+ * -------
+ * AA : array
+ *     AA is modified in place with the pseduoinverse replacing each
+ *     block of AA.  AA is returned in row-major form for Python
  *
  * Notes
  * -----
  * This routine is designed to be called once for a large m.
  * Calling this routine repeatably would not be efficient.
  *
  * This function offers substantial speedup over native Python
@@ -952,17 +957,19 @@
 
     return;
 }
 
 /*
  * Scale the columns of a CSC matrix *in place*
  *
+ * ..
  *   A[:,i] *= X[i]
  *
- * See:
+ * References
+ * ----------
  * https://github.com/scipy/scipy/blob/master/scipy/sparse/sparsetools/csr.h
  *
  */
 template <class I, class T>
 void csc_scale_columns(const I n_row,
                        const I n_col,
                        const I Ap[], const int Ap_size,
@@ -976,17 +983,19 @@
         }
     }
 }
 
 /*
  * Scale the rows of a CSC matrix *in place*
  *
+ * ..
  *   A[i,:] *= X[i]
  *
- * See:
+ * References
+ * ----------
  * https://github.com/scipy/scipy/blob/master/scipy/sparse/sparsetools/csr.h
  *
  */
 template <class I, class T>
 void csc_scale_rows(const I n_row,
                     const I n_col,
                     const I Ap[], const int Ap_size,
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/linalg_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/linalg_bind.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -137,29 +137,30 @@
     m.def("pinv_array", &_pinv_array<int, std::complex<float>, float>,
         py::arg("AA").noconvert(), py::arg("m"), py::arg("n"), py::arg("TransA"));
     m.def("pinv_array", &_pinv_array<int, std::complex<double>, double>,
         py::arg("AA").noconvert(), py::arg("m"), py::arg("n"), py::arg("TransA"),
 R"pbdoc(
 Replace each block of A with a Moore-Penrose pseudoinverse of that block.
 Routine is designed to invert many small matrices at once.
+
 Parameters
 ----------
-AA : {float|complex array}
-     (m, n, n) array, assumed to be "raveled" and in row major form
+AA : array
+    (m, n, n) array, assumed to be "raveled" and in row major form
 m,n : int
-     dimensions of AA
+    dimensions of AA
 TransA : char
-     'T' or 'F'.  Decides whether to transpose each nxn block
-     of A before inverting.  If using Python array, should be 'T'.
+    'T' or 'F'.  Decides whether to transpose each nxn block
+    of A before inverting.  If using Python array, should be 'T'.
 
-Return
-------
-AA : {array}
-     AA is modified in place with the pseduoinverse replacing each
-     block of AA.  AA is returned in row-major form for Python
+Returns
+-------
+AA : array
+    AA is modified in place with the pseduoinverse replacing each
+    block of AA.  AA is returned in row-major form for Python
 
 Notes
 -----
 This routine is designed to be called once for a large m.
 Calling this routine repeatably would not be efficient.
 
 This function offers substantial speedup over native Python
@@ -187,28 +188,32 @@
     m.def("csc_scale_columns", &_csc_scale_columns<int, float>,
         py::arg("n_row"), py::arg("n_col"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Xx").noconvert());
     m.def("csc_scale_columns", &_csc_scale_columns<int, double>,
         py::arg("n_row"), py::arg("n_col"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Xx").noconvert(),
 R"pbdoc(
 Scale the columns of a CSC matrix *in place*
 
+..
   A[:,i] *= X[i]
 
-See:
+References
+----------
 https://github.com/scipy/scipy/blob/master/scipy/sparse/sparsetools/csr.h)pbdoc");
 
     m.def("csc_scale_rows", &_csc_scale_rows<int, int>,
         py::arg("n_row"), py::arg("n_col"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Xx").noconvert());
     m.def("csc_scale_rows", &_csc_scale_rows<int, float>,
         py::arg("n_row"), py::arg("n_col"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Xx").noconvert());
     m.def("csc_scale_rows", &_csc_scale_rows<int, double>,
         py::arg("n_row"), py::arg("n_col"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Xx").noconvert(),
 R"pbdoc(
 Scale the rows of a CSC matrix *in place*
 
+..
   A[i,:] *= X[i]
 
-See:
+References
+----------
 https://github.com/scipy/scipy/blob/master/scipy/sparse/sparsetools/csr.h)pbdoc");
 
 }
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/relaxation.h` & `pyamg-4.2.3/pyamg/amg_core/relaxation.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 #ifndef RELAXATION_H
 #define RELAXATION_H
 
 #include "linalg.h"
 
 /*
- *  Perform one iteration of Gauss-Seidel relaxation on the linear
- *  system Ax = b, where A is stored in CSR format and x and b
- *  are column vectors.
- *
- *  The unknowns are swept through according to the slice defined
- *  by row_start, row_end, and row_step.  These options are used
- *  to implement standard forward and backward sweeps, or sweeping
- *  only a subset of the unknowns.  A forward sweep is implemented
- *  with gauss_seidel(Ap, Aj, Ax, x, b, 0, N, 1) where N is the
- *  number of rows in matrix A.  Similarly, a backward sweep is
- *  implemented with gauss_seidel(Ap, Aj, Ax, x, b, N, -1, -1).
- *
- *  Parameters
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      row_start  - beginning of the sweep
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
+ * Perform one iteration of Gauss-Seidel relaxation on the linear
+ * system Ax = b, where A is stored in CSR format and x and b
+ * are column vectors.
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Parameters
+ * ----------
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * row_start : int
+ *     beginning of the sweep
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ *
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
+ * Notes
+ * -----
+ * The unknowns are swept through according to the slice defined
+ * by row_start, row_end, and row_step.  These options are used
+ * to implement standard forward and backward sweeps, or sweeping
+ * only a subset of the unknowns.  A forward sweep is implemented
+ * with gauss_seidel(Ap, Aj, Ax, x, b, 0, N, 1) where N is the
+ * number of rows in matrix A.  Similarly, a backward sweep is
+ * implemented with gauss_seidel(Ap, Aj, Ax, x, b, N, -1, -1).
  */
 template<class I, class T, class F>
 void gauss_seidel(const I Ap[], const int Ap_size,
                   const I Aj[], const int Aj_size,
                   const T Ax[], const int Ax_size,
                         T  x[], const int  x_size,
                   const T  b[], const int  b_size,
@@ -58,35 +69,46 @@
             x[i] = (b[i] - rsum)/diag;
         }
     }
 }
 
 
 /*
- *  Perform one iteration of Gauss-Seidel relaxation on the linear
- *  system Ax = b, where A is stored in Block CSR format and x and b
- *  are column vectors.  This method applies point-wise relaxation
- *  to the BSR as opposed to \"block relaxation\".
- *
- *  Refer to gauss_seidel for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]       - BSR row pointer
- *      Aj[]       - BSR index array
- *      Ax[]       - BSR data array
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      row_start  - beginning of the sweep (block row index)
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
- *      blocksize  - BSR blocksize (blocks must be square)
+ * Perform one iteration of Gauss-Seidel relaxation on the linear
+ * system Ax = b, where A is stored in Block CSR format and x and b
+ * are column vectors.  This method applies point-wise relaxation
+ * to the BSR as opposed to \"block relaxation\".
+ *
+ * Refer to gauss_seidel for additional information regarding
+ * row_start, row_stop, and row_step.
+ *
+ * Parameters
+ * ----------
+ * Ap : array
+ *     BSR row pointer
+ * Aj : array
+ *     BSR index array
+ * Ax : array
+ *     BSR data array
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * row_start : int
+ *     beginning of the sweep (block row index)
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ * blocksize : int
+ *     BSR blocksize (blocks must be square)
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
  */
 template<class I, class T, class F>
 void bsr_gauss_seidel(const I Ap[], const int Ap_size,
                       const I Aj[], const int Aj_size,
                       const T Ax[], const int Ax_size,
                             T  x[], const int  x_size,
@@ -166,36 +188,48 @@
 
     delete[] rsum;
     delete[] Axloc;
 }// end function
 
 
 /*
- *  Perform one iteration of Jacobi relaxation on the linear
- *  system Ax = b, where A is stored in CSR format and x and b
- *  are column vectors.  Damping is controlled by the omega
- *  parameter.
- *
- *  Refer to gauss_seidel for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      temp[]     - temporary vector the same size as x
- *      row_start  - beginning of the sweep
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
- *      omega      - damping parameter
+ * Perform one iteration of Jacobi relaxation on the linear
+ * system Ax = b, where A is stored in CSR format and x and b
+ * are column vectors.  Damping is controlled by the omega
+ * parameter.
+ *
+ * Refer to gauss_seidel for additional information regarding
+ * row_start, row_stop, and row_step.
+ *
+ * Parameters
+ * ----------
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * temp, array
+ *     temporary vector the same size as x
+ * row_start : int
+ *     beginning of the sweep
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ * omega : float
+ *     damping parameter
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
  */
 template<class I, class T, class F>
 void jacobi(const I Ap[], const int Ap_size,
             const I Aj[], const int Aj_size,
             const T Ax[], const int Ax_size,
                   T  x[], const int  x_size,
@@ -230,37 +264,50 @@
         if (diag != (F) 0.0){
             x[i] = (one - omega2) * temp[i] + omega2 * ((b[i] - rsum)/diag);
         }
     }
 }
 
 /*
- *  Perform one iteration of Jacobi relaxation on the linear
- *  system Ax = b, where A is stored in Block CSR format and x and b
- *  are column vectors.  This method applies point-wise relaxation
- *  to the BSR as opposed to \"block relaxation\".
- *
- *  Refer to jacobi for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]       - BSR row pointer
- *      Aj[]       - BSR index array
- *      Ax[]       - BSR data array
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      temp[]     - temporary vector the same size as x
- *      row_start  - beginning of the sweep (block row index)
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
- *      blocksize  - BSR blocksize (blocks must be square)
- *      omega      - damping parameter
+ * Perform one iteration of Jacobi relaxation on the linear
+ * system Ax = b, where A is stored in Block CSR format and x and b
+ * are column vectors.  This method applies point-wise relaxation
+ * to the BSR as opposed to \"block relaxation\".
+ *
+ * Refer to jacobi for additional information regarding
+ * row_start, row_stop, and row_step.
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Parameters
+ * ----------
+ * Ap : array
+ *     BSR row pointer
+ * Aj : array
+ *     BSR index array
+ * Ax : array
+ *     BSR data array
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * temp : array, inplace
+ *     temporary vector the same size as x
+ * row_start : int
+ *     beginning of the sweep (block row index)
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ * blocksize : int
+ *     BSR blocksize (blocks must be square)
+ * omega : float
+ *     damping parameter
+ *
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
  */
 template<class I, class T, class F>
 void bsr_jacobi(const I Ap[], const int Ap_size,
                 const I Aj[], const int Aj_size,
                 const T Ax[], const int Ax_size,
                       T  x[], const int  x_size,
@@ -350,42 +397,54 @@
     delete[] rsum;
     delete[] Axloc;
 }// end function
 
 
 
 /*
- *  Perform one iteration of Gauss-Seidel relaxation on the linear
- *  system Ax = b, where A is stored in CSR format and x and b
- *  are column vectors.
- *
- *  Unlike gauss_seidel, which is restricted to updating a slice
- *  of the unknowns (defined by row_start, row_start, and row_step),
- *  this method updates unknowns according to the rows listed in
- *  an index array.  This allows and arbitrary set of the unknowns
- *  to be updated in an arbitrary order, as is necessary for the
- *  relaxation steps in the Compatible Relaxation method.
- *
- *  In this method the slice arguments are used to define the subset
- *  of the index array Id which is to be considered.
- *
- *  Parameters
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      Id[]       - index array representing the
- *      row_start  - beginning of the sweep (in array Id)
- *      row_stop   - end of the sweep (in array Id)
- *      row_step   - stride used during the sweep (may be negative)
+ * Perform one iteration of Gauss-Seidel relaxation on the linear
+ * system Ax = b, where A is stored in CSR format and x and b
+ * are column vectors.
+ *
+ * Parameters
+ * ----------
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * Id : array
+ *     index array representing the
+ * row_start : int
+ *     beginning of the sweep (in array Id)
+ * row_stop : int
+ *     end of the sweep (in array Id)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ *
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Notes
+ * -----
+ * Unlike gauss_seidel, which is restricted to updating a slice
+ * of the unknowns (defined by row_start, row_start, and row_step),
+ * this method updates unknowns according to the rows listed in
+ * an index array.  This allows and arbitrary set of the unknowns
+ * to be updated in an arbitrary order, as is necessary for the
+ * relaxation steps in the Compatible Relaxation method.
  *
+ * In this method the slice arguments are used to define the subset
+ * of the index array Id which is to be considered.
  */
 template<class I, class T, class F>
 void gauss_seidel_indexed(const I Ap[], const int Ap_size,
                           const I Aj[], const int Aj_size,
                           const T Ax[], const int Ax_size,
                                 T  x[], const int  x_size,
                           const T  b[], const int  b_size,
@@ -420,39 +479,42 @@
 /*
  * Perform NE Jacobi on the linear system A x = b
  * This effectively carries out weighted-Jacobi on A A^T x = A^T b
  * (also known as Cimmino's relaxation)
  *
  * Parameters
  * ----------
- * Ap : {int array}
- *  index pointer for CSR matrix A
- * Aj : {int array}
- *  column indices for CSR matrix A
- * Ax : {array}
- *  value array for CSR matrix A
- * x : {array}
- *  current guess to the linear system
- * b : {array}
- *  right hand side
- * Tx : {array}
- *  scaled residual
- *  D_A^{-1} (b - Ax)
- * temp : {array}
- *  work space
- * row_start,stop,step : {int}
- *  controls which rows to iterate over
- * omega : {array}
- *  size one array that contains the weighted-jacobi
- *  parameter.  An array must be used to pass in omega to
- *  account for the case where omega may be complex
+ * Ap : array
+ *     index pointer for CSR matrix A
+ * Aj : array
+ *     column indices for CSR matrix A
+ * Ax : array
+ *     value array for CSR matrix A
+ * x : array, inplace
+ *     current guess to the linear system
+ * b : array
+ *     right hand side
+ * Tx : array
+ *     scaled residual D_A^{-1} (b - Ax)
+ * temp : array
+ *     work space
+ * row_start : int
+ *     controls which rows to start on
+ * row_stop : int
+ *     controls which rows to stop on
+ * row_step : int
+ *     controls which rows to iterate over
+ * omega : array
+ *     size one array that contains the weighted-jacobi
+ *     parameter.  An array must be used to pass in omega to
+ *     account for the case where omega may be complex
  *
  * Returns
  * -------
- * x is modified in place in an additive, not overwriting fashion
+ * x is modified inplace in an additive, not overwriting fashion
  *
  * Notes
  * -----
  * Primary calling routine is jacobi_ne in relaxation.py
  */
 template<class I, class T, class F>
 void jacobi_ne(const I Ap[], const int Ap_size,
@@ -488,35 +550,34 @@
 
 /*
  * Perform NE Gauss-Seidel on the linear system A x = b
  * This effectively carries out Gauss-Seidel on A A.H x = b
  *
  * Parameters
  * ----------
- * Ap : {int array}
- *  index pointer for CSR matrix A
- * Aj : {int array}
- *  column indices for CSR matrix A
- * Ax : {array}
- *  value array for CSR matrix A
- * x : {array}
- *  current guess to the linear system
- * b : {array}
- *  right hand side
- * Tx : {array}
- *  inverse(diag(A A.H))
- * omega : {float}
- *  relaxation parameter
- *  (if not 1.0, then algorithm becomes SOR)
- * row_start,stop,step : {int}
- *  controls which rows to iterate over
+ * Ap : array
+ *     index pointer for CSR matrix A
+ * Aj : array
+ *     column indices for CSR matrix A
+ * Ax : array
+ *     value array for CSR matrix A
+ * x : array
+ *     current guess to the linear system
+ * b : array
+ *     right hand side
+ * Tx : array
+ *     inverse(diag(A A.H))
+ * omega : float
+ *     relaxation parameter (if not 1.0, then algorithm becomes SOR)
+ * row_start,stop,step : int
+ *     controls which rows to iterate over
  *
  * Returns
  * -------
- * x is modified in place in an additive, not overwriting fashion
+ * x is modified inplace in an additive, not overwriting fashion
  *
  * Notes
  * -----
  * Primary calling routine is gass_seidel_ne in relaxation.py
  */
 template<class I, class T, class F>
 void gauss_seidel_ne(const I Ap[], const int Ap_size,
@@ -553,35 +614,34 @@
 
 /*
  * Perform NR Gauss-Seidel on the linear system A x = b
  * This effectively carries out Gauss-Seidel on A.H A x = A.H b
  *
  * Parameters
  * ----------
- * Ap : {int array}
- *  index pointer for CSC matrix A
- * Aj : {int array}
- *  row indices for CSC matrix A
- * Ax : {array}
- *  value array for CSC matrix A
- * x : {array}
- *  current guess to the linear system
- * z : {array}
- *  initial residual
- * Tx : {array}
- *  inverse(diag(A.H A))
- * omega : {float}
- *  relaxation parameter
- *  (if not 1.0, then algorithm becomes SOR)
- * col_start,stop,step : {int}
- *  controls which rows to iterate over
+ * Ap : array
+ *     index pointer for CSC matrix A
+ * Aj : array
+ *     row indices for CSC matrix A
+ * Ax : array
+ *     value array for CSC matrix A
+ * x : array
+ *     current guess to the linear system
+ * z : array
+ *     initial residual
+ * Tx : array
+ *     inverse(diag(A.H A))
+ * omega : float
+ *     relaxation parameter (if not 1.0, then algorithm becomes SOR)
+ * col_start,stop,step : int
+ *     controls which rows to iterate over
  *
  * Returns
  * -------
- * x is modified in place in an additive, not overwriting fashion
+ * x is modified inplace in an additive, not overwriting fashion
  *
  * Notes
  * -----
  * Primary calling routine is gauss_seidel_nr in relaxation.py
  */
 template<class I, class T, class F>
 void gauss_seidel_nr(const I Ap[], const int Ap_size,
@@ -619,40 +679,49 @@
         for(I j = start; j < end; j++)
         {   r[Aj[j]] -= delta*Ax[j]; }
     }
 
 }
 
 /*
- *  Perform one iteration of block Jacobi relaxation on the linear
- *  system Ax = b, where A is stored in BSR format and x and b
- *  are column vectors.  Damping is controlled by the omega
- *  parameter.
- *
- *  Refer to gauss_seidel for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]       - BSR row pointer
- *      Aj[]       - BSR index array
- *      Ax[]       - BSR data array, blocks assumed square
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      Tx[]       - Inverse of each diagonal block of A stored
- *                   as a (n/blocksize, blocksize, blocksize) array
- *      temp[]     - temporary vector the same size as x
- *      row_start  - beginning of the sweep
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
- *      omega      - damping parameter
- *      blocksize  - dimension of sqare blocks in BSR matrix A
+ * Perform one iteration of block Jacobi relaxation on the linear
+ * system Ax = b, where A is stored in BSR format and x and b
+ * are column vectors.  Damping is controlled by the omega
+ * parameter.
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Refer to gauss_seidel for additional information regarding
+ * row_start, row_stop, and row_step.
  *
+ * Parameters
+ * ----------
+ * Ap : array
+ *     BSR row pointer
+ * Aj : array
+ *     BSR index array
+ * Ax : array
+ *     BSR data array, blocks assumed square
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * Tx : array
+ *     Inverse of each diagonal block of A stored
+ *     as a (n/blocksize, blocksize, blocksize) array
+ * temp : array
+ *     temporary vector the same size as x
+ * row_start : int
+ *     beginning of the sweep
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ * omega : float
+ *     damping parameter
+ * blocksize int
+ *     dimension of sqare blocks in BSR matrix A
  */
 template<class I, class T, class F>
 void block_jacobi(const I Ap[], const int Ap_size,
                   const I Aj[], const int Aj_size,
                   const T Ax[], const int Ax_size,
                         T  x[], const int  x_size,
                   const T  b[], const int  b_size,
@@ -718,37 +787,44 @@
     }
 
     delete[] v;
     delete[] rsum;
 }
 
 /*
- *  Perform one iteration of block Gauss-Seidel relaxation on
- *  the linear system Ax = b, where A is stored in BSR format
- *  and x and b are column vectors.
- *
- *  Refer to gauss_seidel for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]       - BSR row pointer
- *      Aj[]       - BSR index array
- *      Ax[]       - BSR data array, blocks assumed square
- *      x[]        - approximate solution
- *      b[]        - right hand side
- *      Tx[]       - Inverse of each diagonal block of A stored
- *                   as a (n/blocksize, blocksize, blocksize) array
- *      row_start  - beginning of the sweep
- *      row_stop   - end of the sweep (i.e. one past the last unknown)
- *      row_step   - stride used during the sweep (may be negative)
- *      blocksize  - dimension of square blocks in BSR matrix A
+ * Perform one iteration of block Gauss-Seidel relaxation on
+ * the linear system Ax = b, where A is stored in BSR format
+ * and x and b are column vectors.
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Refer to gauss_seidel for additional information regarding
+ * row_start, row_stop, and row_step.
  *
+ * Parameters
+ * ----------
+ * Ap : array
+ *     BSR row pointer
+ * Aj : array
+ *     BSR index array
+ * Ax : array
+ *     BSR data array, blocks assumed square
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * Tx : array
+ *     Inverse of each diagonal block of A stored
+ *     as a (n/blocksize, blocksize, blocksize) array
+ * row_start : int
+ *     beginning of the sweep
+ * row_stop : int
+ *     end of the sweep (i.e. one past the last unknown)
+ * row_step : int
+ *     stride used during the sweep (may be negative)
+ * blocksize : int
+ *     dimension of square blocks in BSR matrix A
  */
 template<class I, class T, class F>
 void block_gauss_seidel(const I Ap[], const int Ap_size,
                         const I Aj[], const int Aj_size,
                         const T Ax[], const int Ax_size,
                               T  x[], const int  x_size,
                         const T  b[], const int  b_size,
@@ -801,36 +877,45 @@
     }
 
     delete[] v;
     delete[] rsum;
 }
 
 /*
- *  Extract diagonal blocks from A and insert into a linear array.
- *  This is a helper function for overlapping_schwarz_csr.
- *
- *  Parameters
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *                   __must be sorted for each row__
- *      Ax[]       - CSR data array, blocks assumed square
- *      Tx[]       - Inverse of each diagonal block of A, stored in
- *                   row major
- *      Tp[]       - Pointer array into Tx indicating where the
- *                   diagonal blocks start and stop
- *      Sj[]       - Indices of each subdomain
- *                   __must be sorted over each subdomain__
- *      Sp[]       - Pointer array indicating where each subdomain
- *                   starts and stops
- *      nsdomains  - Number of subdomains
- *      nrows      - Number of rows
+ * Extract diagonal blocks from A and insert into a linear array.
+ * This is a helper function for overlapping_schwarz_csr.
  *
- *  Returns:
- *      Nothing, Tx will be modified in place
+ * Parameters
+ * ----------
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ *     must be sorted for each row
+ * Ax : array
+ *     CSR data array, blocks assumed square
+ * Tx : array, inplace
+ *     Inverse of each diagonal block of A, stored in row major
+ * Tp : array
+ *     Pointer array into Tx indicating where the
+ *     diagonal blocks start and stop
+ * Sj : array
+ *     Indices of each subdomain
+ *     must be sorted over each subdomain
+ * Sp : array
+ *     Pointer array indicating where each subdomain
+ *     starts and stops
+ * nsdomains : int
+ *     Number of subdomains
+ * nrows : int
+ *     Number of rows
  *
+ * Returns
+ * -------
+ * Nothing, Tx will be modified inplace
  */
 template<class I, class T, class F>
 void extract_subblocks(const I Ap[], const int Ap_size,
                        const I Aj[], const int Aj_size,
                        const T Ax[], const int Ax_size,
                              T Tx[], const int Tx_size,
                        const I Tp[], const int Tp_size,
@@ -891,44 +976,56 @@
             Tx_offset += row_length;
         }
     }
 }
 
 
 /*
- *  Perform one iteration of an overlapping Schwarz relaxation on
- *  the linear system Ax = b, where A is stored in CSR format
- *  and x and b are column vectors.
- *
- *  Refer to gauss_seidel for additional information regarding
- *  row_start, row_stop, and row_step.
- *
- *  Parameters
- *      Ap[]           - CSR row pointer
- *      Aj[]           - CSR index array
- *      Ax[]           - CSR data array, blocks assumed square
- *      x[]            - approximate solution
- *      b[]            - right hand side
- *      Tx[]           - Inverse of each diagonal block of A, stored in
- *                       row major
- *      Tp[]           - Pointer array into Tx indicating where the
- *                       diagonal blocks start and stop
- *      Sj[]           - Indices of each subdomain
- *                       __must be sorted over each subdomain__
- *      Sp[]           - Pointer array indicating where each subdomain
- *                       starts and stops
- *      nsdomains      - Number of subdomains
- *      nrows          - Number of rows
- *      row_start      --- The subdomains are processed in this order,
- *      row_stop       --- for(i = row_start, i != row_stop, i+=row_step)
- *      row_step       --- {...computation...}
+ * Perform one iteration of an overlapping Schwarz relaxation on
+ * the linear system Ax = b, where A is stored in CSR format
+ * and x and b are column vectors.
  *
+ * Refer to gauss_seidel for additional information regarding
+ * row_start, row_stop, and row_step.
  *
- *  Returns:
- *      Nothing, x will be modified in place
+ * Parameters
+ * ----------
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array, blocks assumed square
+ * x : array, inplace
+ *     approximate solution
+ * b : array
+ *     right hand side
+ * Tx : array
+ *     Inverse of each diagonal block of A, stored in row major
+ * Tp : array
+ *     Pointer array into Tx indicating where the diagonal blocks start and stop
+ * Sj : array
+ *     Indices of each subdomain
+ *     must be sorted over each subdomain
+ * Sp : array
+ *     Pointer array indicating where each subdomain starts and stops
+ * nsdomains
+ *     Number of subdomains
+ * nrows
+ *     Number of rows
+ * row_start : int
+ *     The subdomains are processed in this order,
+ * row_stop : int
+ *     for(i = row_start, i != row_stop, i+=row_step)
+ * row_step : int
+ *     {...computation...}
+ *
+ * Returns
+ * -------
+ * Nothing, x will be modified inplace
  *
  */
 template<class I, class T, class F>
 void overlapping_schwarz_csr(const I Ap[], const int Ap_size,
                              const I Aj[], const int Aj_size,
                              const T Ax[], const int Ax_size,
                                    T  x[], const int  x_size,
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/relaxation_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/relaxation_bind.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -551,170 +551,231 @@
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("gauss_seidel", &_gauss_seidel<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("gauss_seidel", &_gauss_seidel<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"),
 R"pbdoc(
 Perform one iteration of Gauss-Seidel relaxation on the linear
- system Ax = b, where A is stored in CSR format and x and b
- are column vectors.
+system Ax = b, where A is stored in CSR format and x and b
+are column vectors.
 
- The unknowns are swept through according to the slice defined
- by row_start, row_end, and row_step.  These options are used
- to implement standard forward and backward sweeps, or sweeping
- only a subset of the unknowns.  A forward sweep is implemented
- with gauss_seidel(Ap, Aj, Ax, x, b, 0, N, 1) where N is the
- number of rows in matrix A.  Similarly, a backward sweep is
- implemented with gauss_seidel(Ap, Aj, Ax, x, b, N, -1, -1).
-
- Parameters
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-     x[]        - approximate solution
-     b[]        - right hand side
-     row_start  - beginning of the sweep
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
+Parameters
+----------
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+row_start : int
+    beginning of the sweep
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+
+Returns
+-------
+Nothing, x will be modified inplace
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Notes
+-----
+The unknowns are swept through according to the slice defined
+by row_start, row_end, and row_step.  These options are used
+to implement standard forward and backward sweeps, or sweeping
+only a subset of the unknowns.  A forward sweep is implemented
+with gauss_seidel(Ap, Aj, Ax, x, b, 0, N, 1) where N is the
+number of rows in matrix A.  Similarly, a backward sweep is
+implemented with gauss_seidel(Ap, Aj, Ax, x, b, N, -1, -1).)pbdoc");
 
     m.def("bsr_gauss_seidel", &_bsr_gauss_seidel<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("bsr_gauss_seidel", &_bsr_gauss_seidel<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("bsr_gauss_seidel", &_bsr_gauss_seidel<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("bsr_gauss_seidel", &_bsr_gauss_seidel<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"),
 R"pbdoc(
 Perform one iteration of Gauss-Seidel relaxation on the linear
- system Ax = b, where A is stored in Block CSR format and x and b
- are column vectors.  This method applies point-wise relaxation
- to the BSR as opposed to \"block relaxation\".
-
- Refer to gauss_seidel for additional information regarding
- row_start, row_stop, and row_step.
-
- Parameters
-     Ap[]       - BSR row pointer
-     Aj[]       - BSR index array
-     Ax[]       - BSR data array
-     x[]        - approximate solution
-     b[]        - right hand side
-     row_start  - beginning of the sweep (block row index)
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
-     blocksize  - BSR blocksize (blocks must be square)
+system Ax = b, where A is stored in Block CSR format and x and b
+are column vectors.  This method applies point-wise relaxation
+to the BSR as opposed to \"block relaxation\".
+
+Refer to gauss_seidel for additional information regarding
+row_start, row_stop, and row_step.
+
+Parameters
+----------
+Ap : array
+    BSR row pointer
+Aj : array
+    BSR index array
+Ax : array
+    BSR data array
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+row_start : int
+    beginning of the sweep (block row index)
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+blocksize : int
+    BSR blocksize (blocks must be square)
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Returns
+-------
+Nothing, x will be modified inplace)pbdoc");
 
     m.def("jacobi", &_jacobi<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
     m.def("jacobi", &_jacobi<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
     m.def("jacobi", &_jacobi<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
     m.def("jacobi", &_jacobi<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert(),
 R"pbdoc(
 Perform one iteration of Jacobi relaxation on the linear
- system Ax = b, where A is stored in CSR format and x and b
- are column vectors.  Damping is controlled by the omega
- parameter.
-
- Refer to gauss_seidel for additional information regarding
- row_start, row_stop, and row_step.
-
- Parameters
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-     x[]        - approximate solution
-     b[]        - right hand side
-     temp[]     - temporary vector the same size as x
-     row_start  - beginning of the sweep
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
-     omega      - damping parameter
+system Ax = b, where A is stored in CSR format and x and b
+are column vectors.  Damping is controlled by the omega
+parameter.
+
+Refer to gauss_seidel for additional information regarding
+row_start, row_stop, and row_step.
+
+Parameters
+----------
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+temp, array
+    temporary vector the same size as x
+row_start : int
+    beginning of the sweep
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+omega : float
+    damping parameter
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Returns
+-------
+Nothing, x will be modified inplace)pbdoc");
 
     m.def("bsr_jacobi", &_bsr_jacobi<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"), py::arg("omega").noconvert());
     m.def("bsr_jacobi", &_bsr_jacobi<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"), py::arg("omega").noconvert());
     m.def("bsr_jacobi", &_bsr_jacobi<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"), py::arg("omega").noconvert());
     m.def("bsr_jacobi", &_bsr_jacobi<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"), py::arg("omega").noconvert(),
 R"pbdoc(
 Perform one iteration of Jacobi relaxation on the linear
- system Ax = b, where A is stored in Block CSR format and x and b
- are column vectors.  This method applies point-wise relaxation
- to the BSR as opposed to \"block relaxation\".
-
- Refer to jacobi for additional information regarding
- row_start, row_stop, and row_step.
-
- Parameters
-     Ap[]       - BSR row pointer
-     Aj[]       - BSR index array
-     Ax[]       - BSR data array
-     x[]        - approximate solution
-     b[]        - right hand side
-     temp[]     - temporary vector the same size as x
-     row_start  - beginning of the sweep (block row index)
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
-     blocksize  - BSR blocksize (blocks must be square)
-     omega      - damping parameter
+system Ax = b, where A is stored in Block CSR format and x and b
+are column vectors.  This method applies point-wise relaxation
+to the BSR as opposed to \"block relaxation\".
+
+Refer to jacobi for additional information regarding
+row_start, row_stop, and row_step.
+
+Parameters
+----------
+Ap : array
+    BSR row pointer
+Aj : array
+    BSR index array
+Ax : array
+    BSR data array
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+temp : array, inplace
+    temporary vector the same size as x
+row_start : int
+    beginning of the sweep (block row index)
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+blocksize : int
+    BSR blocksize (blocks must be square)
+omega : float
+    damping parameter
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Returns
+-------
+Nothing, x will be modified inplace)pbdoc");
 
     m.def("gauss_seidel_indexed", &_gauss_seidel_indexed<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Id").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("gauss_seidel_indexed", &_gauss_seidel_indexed<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Id").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("gauss_seidel_indexed", &_gauss_seidel_indexed<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Id").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("gauss_seidel_indexed", &_gauss_seidel_indexed<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Id").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"),
 R"pbdoc(
 Perform one iteration of Gauss-Seidel relaxation on the linear
- system Ax = b, where A is stored in CSR format and x and b
- are column vectors.
+system Ax = b, where A is stored in CSR format and x and b
+are column vectors.
+
+Parameters
+----------
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+Id : array
+    index array representing the
+row_start : int
+    beginning of the sweep (in array Id)
+row_stop : int
+    end of the sweep (in array Id)
+row_step : int
+    stride used during the sweep (may be negative)
+
+Returns
+-------
+Nothing, x will be modified inplace
 
- Unlike gauss_seidel, which is restricted to updating a slice
- of the unknowns (defined by row_start, row_start, and row_step),
- this method updates unknowns according to the rows listed in
- an index array.  This allows and arbitrary set of the unknowns
- to be updated in an arbitrary order, as is necessary for the
- relaxation steps in the Compatible Relaxation method.
-
- In this method the slice arguments are used to define the subset
- of the index array Id which is to be considered.
-
- Parameters
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-     x[]        - approximate solution
-     b[]        - right hand side
-     Id[]       - index array representing the
-     row_start  - beginning of the sweep (in array Id)
-     row_stop   - end of the sweep (in array Id)
-     row_step   - stride used during the sweep (may be negative)
+Notes
+-----
+Unlike gauss_seidel, which is restricted to updating a slice
+of the unknowns (defined by row_start, row_start, and row_step),
+this method updates unknowns according to the rows listed in
+an index array.  This allows and arbitrary set of the unknowns
+to be updated in an arbitrary order, as is necessary for the
+relaxation steps in the Compatible Relaxation method.
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+In this method the slice arguments are used to define the subset
+of the index array Id which is to be considered.)pbdoc");
 
     m.def("jacobi_ne", &_jacobi_ne<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
     m.def("jacobi_ne", &_jacobi_ne<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
     m.def("jacobi_ne", &_jacobi_ne<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert());
@@ -723,39 +784,42 @@
 R"pbdoc(
 Perform NE Jacobi on the linear system A x = b
 This effectively carries out weighted-Jacobi on A A^T x = A^T b
 (also known as Cimmino's relaxation)
 
 Parameters
 ----------
-Ap : {int array}
- index pointer for CSR matrix A
-Aj : {int array}
- column indices for CSR matrix A
-Ax : {array}
- value array for CSR matrix A
-x : {array}
- current guess to the linear system
-b : {array}
- right hand side
-Tx : {array}
- scaled residual
- D_A^{-1} (b - Ax)
-temp : {array}
- work space
-row_start,stop,step : {int}
- controls which rows to iterate over
-omega : {array}
- size one array that contains the weighted-jacobi
- parameter.  An array must be used to pass in omega to
- account for the case where omega may be complex
+Ap : array
+    index pointer for CSR matrix A
+Aj : array
+    column indices for CSR matrix A
+Ax : array
+    value array for CSR matrix A
+x : array, inplace
+    current guess to the linear system
+b : array
+    right hand side
+Tx : array
+    scaled residual D_A^{-1} (b - Ax)
+temp : array
+    work space
+row_start : int
+    controls which rows to start on
+row_stop : int
+    controls which rows to stop on
+row_step : int
+    controls which rows to iterate over
+omega : array
+    size one array that contains the weighted-jacobi
+    parameter.  An array must be used to pass in omega to
+    account for the case where omega may be complex
 
 Returns
 -------
-x is modified in place in an additive, not overwriting fashion
+x is modified inplace in an additive, not overwriting fashion
 
 Notes
 -----
 Primary calling routine is jacobi_ne in relaxation.py)pbdoc");
 
     m.def("gauss_seidel_ne", &_gauss_seidel_ne<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("Tx").noconvert(), py::arg("omega"));
@@ -767,35 +831,34 @@
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("Tx").noconvert(), py::arg("omega"),
 R"pbdoc(
 Perform NE Gauss-Seidel on the linear system A x = b
 This effectively carries out Gauss-Seidel on A A.H x = b
 
 Parameters
 ----------
-Ap : {int array}
- index pointer for CSR matrix A
-Aj : {int array}
- column indices for CSR matrix A
-Ax : {array}
- value array for CSR matrix A
-x : {array}
- current guess to the linear system
-b : {array}
- right hand side
-Tx : {array}
- inverse(diag(A A.H))
-omega : {float}
- relaxation parameter
- (if not 1.0, then algorithm becomes SOR)
-row_start,stop,step : {int}
- controls which rows to iterate over
+Ap : array
+    index pointer for CSR matrix A
+Aj : array
+    column indices for CSR matrix A
+Ax : array
+    value array for CSR matrix A
+x : array
+    current guess to the linear system
+b : array
+    right hand side
+Tx : array
+    inverse(diag(A A.H))
+omega : float
+    relaxation parameter (if not 1.0, then algorithm becomes SOR)
+row_start,stop,step : int
+    controls which rows to iterate over
 
 Returns
 -------
-x is modified in place in an additive, not overwriting fashion
+x is modified inplace in an additive, not overwriting fashion
 
 Notes
 -----
 Primary calling routine is gass_seidel_ne in relaxation.py)pbdoc");
 
     m.def("gauss_seidel_nr", &_gauss_seidel_nr<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("z").noconvert(), py::arg("col_start"), py::arg("col_stop"), py::arg("col_step"), py::arg("Tx").noconvert(), py::arg("omega"));
@@ -807,35 +870,34 @@
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("z").noconvert(), py::arg("col_start"), py::arg("col_stop"), py::arg("col_step"), py::arg("Tx").noconvert(), py::arg("omega"),
 R"pbdoc(
 Perform NR Gauss-Seidel on the linear system A x = b
 This effectively carries out Gauss-Seidel on A.H A x = A.H b
 
 Parameters
 ----------
-Ap : {int array}
- index pointer for CSC matrix A
-Aj : {int array}
- row indices for CSC matrix A
-Ax : {array}
- value array for CSC matrix A
-x : {array}
- current guess to the linear system
-z : {array}
- initial residual
-Tx : {array}
- inverse(diag(A.H A))
-omega : {float}
- relaxation parameter
- (if not 1.0, then algorithm becomes SOR)
-col_start,stop,step : {int}
- controls which rows to iterate over
+Ap : array
+    index pointer for CSC matrix A
+Aj : array
+    row indices for CSC matrix A
+Ax : array
+    value array for CSC matrix A
+x : array
+    current guess to the linear system
+z : array
+    initial residual
+Tx : array
+    inverse(diag(A.H A))
+omega : float
+    relaxation parameter (if not 1.0, then algorithm becomes SOR)
+col_start,stop,step : int
+    controls which rows to iterate over
 
 Returns
 -------
-x is modified in place in an additive, not overwriting fashion
+x is modified inplace in an additive, not overwriting fashion
 
 Notes
 -----
 Primary calling routine is gauss_seidel_nr in relaxation.py)pbdoc");
 
     m.def("block_jacobi", &_block_jacobi<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert(), py::arg("blocksize"));
@@ -843,137 +905,177 @@
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert(), py::arg("blocksize"));
     m.def("block_jacobi", &_block_jacobi<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert(), py::arg("blocksize"));
     m.def("block_jacobi", &_block_jacobi<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("temp").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("omega").noconvert(), py::arg("blocksize"),
 R"pbdoc(
 Perform one iteration of block Jacobi relaxation on the linear
- system Ax = b, where A is stored in BSR format and x and b
- are column vectors.  Damping is controlled by the omega
- parameter.
-
- Refer to gauss_seidel for additional information regarding
- row_start, row_stop, and row_step.
-
- Parameters
-     Ap[]       - BSR row pointer
-     Aj[]       - BSR index array
-     Ax[]       - BSR data array, blocks assumed square
-     x[]        - approximate solution
-     b[]        - right hand side
-     Tx[]       - Inverse of each diagonal block of A stored
-                  as a (n/blocksize, blocksize, blocksize) array
-     temp[]     - temporary vector the same size as x
-     row_start  - beginning of the sweep
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
-     omega      - damping parameter
-     blocksize  - dimension of sqare blocks in BSR matrix A
+system Ax = b, where A is stored in BSR format and x and b
+are column vectors.  Damping is controlled by the omega
+parameter.
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Refer to gauss_seidel for additional information regarding
+row_start, row_stop, and row_step.
+
+Parameters
+----------
+Ap : array
+    BSR row pointer
+Aj : array
+    BSR index array
+Ax : array
+    BSR data array, blocks assumed square
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+Tx : array
+    Inverse of each diagonal block of A stored
+    as a (n/blocksize, blocksize, blocksize) array
+temp : array
+    temporary vector the same size as x
+row_start : int
+    beginning of the sweep
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+omega : float
+    damping parameter
+blocksize int
+    dimension of sqare blocks in BSR matrix A)pbdoc");
 
     m.def("block_gauss_seidel", &_block_gauss_seidel<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("block_gauss_seidel", &_block_gauss_seidel<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("block_gauss_seidel", &_block_gauss_seidel<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"));
     m.def("block_gauss_seidel", &_block_gauss_seidel<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"), py::arg("blocksize"),
 R"pbdoc(
 Perform one iteration of block Gauss-Seidel relaxation on
- the linear system Ax = b, where A is stored in BSR format
- and x and b are column vectors.
+the linear system Ax = b, where A is stored in BSR format
+and x and b are column vectors.
 
- Refer to gauss_seidel for additional information regarding
- row_start, row_stop, and row_step.
+Refer to gauss_seidel for additional information regarding
+row_start, row_stop, and row_step.
 
- Parameters
-     Ap[]       - BSR row pointer
-     Aj[]       - BSR index array
-     Ax[]       - BSR data array, blocks assumed square
-     x[]        - approximate solution
-     b[]        - right hand side
-     Tx[]       - Inverse of each diagonal block of A stored
-                  as a (n/blocksize, blocksize, blocksize) array
-     row_start  - beginning of the sweep
-     row_stop   - end of the sweep (i.e. one past the last unknown)
-     row_step   - stride used during the sweep (may be negative)
-     blocksize  - dimension of square blocks in BSR matrix A
-
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Parameters
+----------
+Ap : array
+    BSR row pointer
+Aj : array
+    BSR index array
+Ax : array
+    BSR data array, blocks assumed square
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+Tx : array
+    Inverse of each diagonal block of A stored
+    as a (n/blocksize, blocksize, blocksize) array
+row_start : int
+    beginning of the sweep
+row_stop : int
+    end of the sweep (i.e. one past the last unknown)
+row_step : int
+    stride used during the sweep (may be negative)
+blocksize : int
+    dimension of square blocks in BSR matrix A)pbdoc");
 
     m.def("extract_subblocks", &_extract_subblocks<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"));
     m.def("extract_subblocks", &_extract_subblocks<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"));
     m.def("extract_subblocks", &_extract_subblocks<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"));
     m.def("extract_subblocks", &_extract_subblocks<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"),
 R"pbdoc(
 Extract diagonal blocks from A and insert into a linear array.
- This is a helper function for overlapping_schwarz_csr.
+This is a helper function for overlapping_schwarz_csr.
 
- Parameters
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-                  __must be sorted for each row__
-     Ax[]       - CSR data array, blocks assumed square
-     Tx[]       - Inverse of each diagonal block of A, stored in
-                  row major
-     Tp[]       - Pointer array into Tx indicating where the
-                  diagonal blocks start and stop
-     Sj[]       - Indices of each subdomain
-                  __must be sorted over each subdomain__
-     Sp[]       - Pointer array indicating where each subdomain
-                  starts and stops
-     nsdomains  - Number of subdomains
-     nrows      - Number of rows
+Parameters
+----------
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+    must be sorted for each row
+Ax : array
+    CSR data array, blocks assumed square
+Tx : array, inplace
+    Inverse of each diagonal block of A, stored in row major
+Tp : array
+    Pointer array into Tx indicating where the
+    diagonal blocks start and stop
+Sj : array
+    Indices of each subdomain
+    must be sorted over each subdomain
+Sp : array
+    Pointer array indicating where each subdomain
+    starts and stops
+nsdomains : int
+    Number of subdomains
+nrows : int
+    Number of rows
 
- Returns:
-     Nothing, Tx will be modified in place)pbdoc");
+Returns
+-------
+Nothing, Tx will be modified inplace)pbdoc");
 
     m.def("overlapping_schwarz_csr", &_overlapping_schwarz_csr<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("overlapping_schwarz_csr", &_overlapping_schwarz_csr<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("overlapping_schwarz_csr", &_overlapping_schwarz_csr<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"));
     m.def("overlapping_schwarz_csr", &_overlapping_schwarz_csr<int, std::complex<double>, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("x").noconvert(), py::arg("b").noconvert(), py::arg("Tx").noconvert(), py::arg("Tp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sp").noconvert(), py::arg("nsdomains"), py::arg("nrows"), py::arg("row_start"), py::arg("row_stop"), py::arg("row_step"),
 R"pbdoc(
 Perform one iteration of an overlapping Schwarz relaxation on
- the linear system Ax = b, where A is stored in CSR format
- and x and b are column vectors.
-
- Refer to gauss_seidel for additional information regarding
- row_start, row_stop, and row_step.
+the linear system Ax = b, where A is stored in CSR format
+and x and b are column vectors.
 
- Parameters
-     Ap[]           - CSR row pointer
-     Aj[]           - CSR index array
-     Ax[]           - CSR data array, blocks assumed square
-     x[]            - approximate solution
-     b[]            - right hand side
-     Tx[]           - Inverse of each diagonal block of A, stored in
-                      row major
-     Tp[]           - Pointer array into Tx indicating where the
-                      diagonal blocks start and stop
-     Sj[]           - Indices of each subdomain
-                      __must be sorted over each subdomain__
-     Sp[]           - Pointer array indicating where each subdomain
-                      starts and stops
-     nsdomains      - Number of subdomains
-     nrows          - Number of rows
-     row_start      --- The subdomains are processed in this order,
-     row_stop       --- for(i = row_start, i != row_stop, i+=row_step)
-     row_step       --- {...computation...}
+Refer to gauss_seidel for additional information regarding
+row_start, row_stop, and row_step.
 
+Parameters
+----------
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array, blocks assumed square
+x : array, inplace
+    approximate solution
+b : array
+    right hand side
+Tx : array
+    Inverse of each diagonal block of A, stored in row major
+Tp : array
+    Pointer array into Tx indicating where the diagonal blocks start and stop
+Sj : array
+    Indices of each subdomain
+    must be sorted over each subdomain
+Sp : array
+    Pointer array indicating where each subdomain starts and stops
+nsdomains
+    Number of subdomains
+nrows
+    Number of rows
+row_start : int
+    The subdomains are processed in this order,
+row_stop : int
+    for(i = row_start, i != row_stop, i+=row_step)
+row_step : int
+    {...computation...}
 
- Returns:
-     Nothing, x will be modified in place)pbdoc");
+Returns
+-------
+Nothing, x will be modified inplace)pbdoc");
 
 }
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/ruge_stuben.h` & `pyamg-4.2.3/pyamg/amg_core/ruge_stuben.h`

 * *Files 12% similar despite different names*

```diff
@@ -19,37 +19,47 @@
 
 /*
  *  Compute a strength of connection matrix using the classical strength
  *  of connection measure by Ruge and Stuben. Both the input and output
  *  matrices are stored in CSR format.  An off-diagonal nonzero entry
  *  A[i,j] is considered strong if:
  *
+ *  ..
  *      |A[i,j]| >= theta * max( |A[i,k]| )   where k != i
  *
  * Otherwise, the connection is weak.
  *
- *  Parameters
- *      num_rows   - number of rows in A
- *      theta      - stength of connection tolerance
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *      Sp[]       - (output) CSR row pointer
- *      Sj[]       - (output) CSR index array
- *      Sx[]       - (output) CSR data array
- *
- *
- *  Returns:
- *      Nothing, S will be stored in Sp, Sj, Sx
- *
- *  Notes:
- *      Storage for S must be preallocated.  Since S will consist of a subset
- *      of A's nonzero values, a conservative bound is to allocate the same
- *      storage for S as is used by A.
- *
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A
+ * theta : float
+ *     stength of connection tolerance
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ * Sp : array
+ *     CSR row pointer
+ * Sj : array
+ *     CSR index array
+ * Sx : array
+ *     CSR data array
+ *
+ * Returns
+ * -------
+ * Nothing, S will be stored in Sp, Sj, Sx
+ *
+ * Notes
+ * -----
+ * Storage for S must be preallocated.  Since S will consist of a subset
+ * of A's nonzero values, a conservative bound is to allocate the same
+ * storage for S as is used by A.
  */
 template<class I, class T, class F>
 void classical_strength_of_connection_abs(const I n_row,
                                           const F theta,
                                           const I Ap[], const int Ap_size,
                                           const I Aj[], const int Aj_size,
                                           const T Ax[], const int Ax_size,
@@ -144,25 +154,32 @@
         }
 
         Sp[i+1] = nnz;
     }
 }
 
 /*
- *  Compute the maximum in magnitude row value for a CSR matrix
- *
- *  Parameters
- *      num_rows   - number of rows in A
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *       x[]       - num_rows array
+ * Compute the maximum in magnitude row value for a CSR matrix
  *
- *  Returns:
- *      Nothing, x[i] will hold row i's maximum magnitude entry
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A
+ * x : array, inplace
+ *      num_rows array
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ *
+ * Returns
+ * -------
+ * Nothing, x[i] will hold row i's maximum magnitude entry
  *
  */
 template<class I, class T, class F>
 void maximum_row_value(const I n_row,
                               T x[], const int  x_size,
                        const I Ap[], const int Ap_size,
                        const I Aj[], const int Aj_size,
@@ -187,27 +204,35 @@
 
 /* Compute a C/F (coarse-fine( splitting using the classical coarse grid
  * selection method of Ruge and Stuben.  The strength of connection matrix S,
  * and its transpose T, are stored in CSR format.  Upon return, the  splitting
  * array will consist of zeros and ones, where C-nodes (coarse nodes) are
  * marked with the value 1 and F-nodes (fine nodes) with the value 0.
  *
- * Parameters:
- *   n_nodes   - number of rows in A
- *   C_rowptr[]      - CSR row pointer array for SOC matrix
- *   C_colinds[]      - CSR column index array for SOC matrix
- *   Tp[]      - CSR row pointer array for transpose of SOC matrix
- *   Tj[]      - CSR column index array for transpose of SOC matrix
- *   influence - array that influences splitting (values stored here are
- *               added to lambda for each point)
- *   splitting - array to store the C/F splitting
- *
- * Notes:
- *   The splitting array must be preallocated
- *
+ * Parameters
+ * ----------
+ * n_nodes : int
+ *     number of rows in A
+ * C_rowptr : array
+ *     CSR row pointer array for SOC matrix
+ * C_colinds : array
+ *     CSR column index array for SOC matrix
+ * Tp : array
+ *     CSR row pointer array for transpose of SOC matrix
+ * Tj : array
+ *     CSR column index array for transpose of SOC matrix
+ * influence : array
+ *     array that influences splitting (values stored here are
+ *     added to lambda for each point)
+ * splitting : array, inplace
+ *     array to store the C/F splitting
+ *
+ * Notes
+ * -----
+ * The splitting array must be preallocated
  */
 template<class I>
 void rs_cf_splitting(const I n_nodes,
                      const I C_rowptr[], const int C_rowptr_size,
                      const I C_colinds[], const int C_colinds_size,
                      const I Tp[], const int Tp_size,
                      const I Tj[], const int Tj_size,
@@ -263,15 +288,15 @@
     for (I i = 0; i < n_nodes; i++) {
         if (lambda[i] == 0 || (lambda[i] == 1 && Tj[Tp[i]] == i))
             splitting[i] = F_NODE;
     }
 
     // Add elements to C and F, in descending order of lambda
     for (I top_index=(n_nodes - 1); top_index>-1; top_index--) {
-        
+
         I i        = index_to_node[top_index];
         I lambda_i = lambda[i];
 
         // Remove i from its interval
         interval_count[lambda_i]--;
 
         // ----------------- Sorting every iteration = O(n^2) complexity ----------------- //
@@ -311,15 +336,15 @@
             // values for neighborhood of j
             for (I jj = Tp[i]; jj < Tp[i+1]; jj++)
             {
                 I j = Tj[jj];
                 if(splitting[j] == PRE_F_NODE)
                 {
                     splitting[j] = F_NODE;
-                    
+
                     // For each k in S_j /\ U, modify lambda value, lambda_k += 1
                     for (I kk = C_rowptr[j]; kk < C_rowptr[j+1]; kk++){
                         I k = C_colinds[kk];
 
                         if(splitting[k] == U_NODE){
 
                             // Move k to the end of its current interval
@@ -422,15 +447,15 @@
                         if (dependence) {
                             break;
                         }
                     }
 
                     // Node j passed dependence test
                     if (dependence) {
-                        continue;   
+                        continue;
                     }
                     // Node j did not pass dependence test
                     else {
                         // If no tentative C-point, mark j as tentative C-point
                         if (Cpt0 < 0) {
                             Cpt0 = j;
                             splitting[j] = C_NODE;
@@ -447,28 +472,37 @@
             }
         }
     }
 }
 
 
 /*
- *  Compute a CLJP splitting
+ * Compute a CLJP splitting
  *
- *  Parameters
- *      n          - number of rows in A (number of vertices)
- *      Sp[]       - CSR row pointer (strength matrix)
- *      Sj[]       - CSR index array
- *      Tp[]       - CSR row pointer (transpose of the strength matrix)
- *      Tj[]       - CSR index array
- *      splitting  - array to store the C/F splitting
- *      colorflag  - flag to indicate coloring
- *
- *  Notes:
- *      The splitting array must be preallocated.
- *      CLJP naive since it requires the transpose.
+ * Parameters
+ * ----------
+ * n : int
+ *     number of rows in A (number of vertices)
+ * Sp : array
+ *     CSR row pointer (strength matrix)
+ * Sj : array
+ *     CSR index array
+ * Tp : array
+ *     CSR row pointer (transpose of the strength matrix)
+ * Tj : array
+ *     CSR index array
+ * splitting : array, inplace
+ *     array to store the C/F splitting
+ * colorflag : int
+ *     flag to indicate coloring
+ *
+ * Notes
+ * -----
+ * The splitting array must be preallocated.
+ * CLJP naive since it requires the transpose.
  */
 
 template<class I>
 void cljp_naive_splitting(const I n,
                           const I Sp[], const int Sp_size,
                           const I Sj[], const int Sj_size,
                           const I Tp[], const int Tp_size,
@@ -631,24 +665,38 @@
     }
   }
   delete[] c_dep_cache;
 }
 
 
 /*
- *   Produce the Ruge-Stuben prolongator using "Direct Interpolation"
+ * Produce the Ruge-Stuben prolongator using "Direct Interpolation"
  *
  *
- *   The first pass uses the strength of connection matrix 'S'
- *   and C/F splitting to compute the row pointer for the prolongator.
+ * The first pass uses the strength of connection matrix 'S'
+ * and C/F splitting to compute the row pointer for the prolongator.
  *
- *   The second pass fills in the nonzero entries of the prolongator
+ * The second pass fills in the nonzero entries of the prolongator
  *
- *   Reference:
- *      Page 479 of "Multigrid"
+ * Parameters
+ * ----------
+ * n_nodes : int
+ *     Number of nodes
+ * Sp : array
+ *     Strength matrix row pointer array
+ * Sj : array
+ *     Strength matrix column index array
+ * splitting : array
+ *     C/F splitting
+ * Bp : array, inplace
+ *     Row pointer array
+ *
+ * References
+ * ----------
+ * Page 479 of Multigrid
  *
  */
 template<class I>
 void rs_direct_interpolation_pass1(const I n_nodes,
                                    const I Sp[], const int Sp_size,
                                    const I Sj[], const int Sj_size,
                                    const I splitting[], const int splitting_size,
@@ -761,48 +809,48 @@
     // Not implemented
 }
 
 
 /* Helper function for compatible relaxation to perform steps 3.1d - 3.1f
  * in Falgout / Brannick (2010).
  *
- * Input:
- * ------
- * A_rowptr : const {int array}
+ * Parameters
+ * ----------
+ * A_rowptr : array
  *      Row pointer for sparse matrix in CSR format.
- * A_colinds : const {int array}
+ * A_colinds : array
  *      Column indices for sparse matrix in CSR format.
- * B : const {float array}
+ * B : array
  *      Target near null space vector for computing candidate set measure.
- * e : {float array}
+ * e : array, inplace
  *      Relaxed vector for computing candidate set measure.
- * indices : {int array}
+ * indices : array, inplace
  *      Array of indices, where indices[0] = the number of F indices, nf,
  *      followed by F indices in elements 1:nf, and C indices in (nf+1):n.
- * splitting : {int array}
+ * splitting : array, inplace
  *      Integer array with current C/F splitting of nodes, 0 = C-point,
  *      1 = F-point.
- * gamma : {float array}
+ * gamma : array, inplace
  *      Preallocated vector to store candidate set measure.
- * thetacs : const {float}
+ * thetacs : float
  *      Threshold for coarse grid candidates from set measure.
  *
- * Returns:
- * --------
+ * Returns
+ * -------
  * Nothing, updated C/F-splitting and corresponding indices modified in place.
  */
 template<class I, class T>
-void cr_helper(const I A_rowptr[], const int A_rowptr_size,
+void cr_helper(const I A_rowptr[],  const int A_rowptr_size,
                const I A_colinds[], const int A_colinds_size,
-               const T B[], const int B_size,
-               T e[], const int e_size,
-               I indices[], const int indices_size,
-               I splitting[], const int splitting_size,
-               T gamma[], const int gamma_size,
-               const T thetacs  )
+               const T B[],         const int B_size,
+               T e[],               const int e_size,
+               I indices[],         const int indices_size,
+               I splitting[],       const int splitting_size,
+               T gamma[],           const int gamma_size,
+               const T thetacs)
 {
     I n = splitting_size;
     I &num_Fpts = indices[0];
 
     // Steps 3.1d, 3.1e in Falgout / Brannick (2010)
     // Divide each element in e by corresponding index in initial target vector.
     // Get inf norm of new e.
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/ruge_stuben_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/ruge_stuben_bind.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -347,36 +347,47 @@
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(),
 R"pbdoc(
 Compute a strength of connection matrix using the classical strength
  of connection measure by Ruge and Stuben. Both the input and output
  matrices are stored in CSR format.  An off-diagonal nonzero entry
  A[i,j] is considered strong if:
 
+ ..
      |A[i,j]| >= theta * max( |A[i,k]| )   where k != i
 
 Otherwise, the connection is weak.
 
- Parameters
-     num_rows   - number of rows in A
-     theta      - stength of connection tolerance
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-     Sp[]       - (output) CSR row pointer
-     Sj[]       - (output) CSR index array
-     Sx[]       - (output) CSR data array
-
-
- Returns:
-     Nothing, S will be stored in Sp, Sj, Sx
-
- Notes:
-     Storage for S must be preallocated.  Since S will consist of a subset
-     of A's nonzero values, a conservative bound is to allocate the same
-     storage for S as is used by A.)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A
+theta : float
+    stength of connection tolerance
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+Sp : array
+    CSR row pointer
+Sj : array
+    CSR index array
+Sx : array
+    CSR data array
+
+Returns
+-------
+Nothing, S will be stored in Sp, Sj, Sx
+
+Notes
+-----
+Storage for S must be preallocated.  Since S will consist of a subset
+of A's nonzero values, a conservative bound is to allocate the same
+storage for S as is used by A.)pbdoc");
 
     m.def("classical_strength_of_connection_min", &_classical_strength_of_connection_min<int, float>,
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert());
     m.def("classical_strength_of_connection_min", &_classical_strength_of_connection_min<int, double>,
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(),
 R"pbdoc(
 )pbdoc");
@@ -388,45 +399,61 @@
     m.def("maximum_row_value", &_maximum_row_value<int, std::complex<float>, float>,
         py::arg("n_row"), py::arg("x").noconvert(), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert());
     m.def("maximum_row_value", &_maximum_row_value<int, std::complex<double>, double>,
         py::arg("n_row"), py::arg("x").noconvert(), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(),
 R"pbdoc(
 Compute the maximum in magnitude row value for a CSR matrix
 
- Parameters
-     num_rows   - number of rows in A
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-      x[]       - num_rows array
-
- Returns:
-     Nothing, x[i] will hold row i's maximum magnitude entry)pbdoc");
+Parameters
+----------
+num_rows : int
+    number of rows in A
+x : array, inplace
+     num_rows array
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+
+Returns
+-------
+Nothing, x[i] will hold row i's maximum magnitude entry)pbdoc");
 
     m.def("rs_cf_splitting", &_rs_cf_splitting<int>,
         py::arg("n_nodes"), py::arg("C_rowptr").noconvert(), py::arg("C_colinds").noconvert(), py::arg("Tp").noconvert(), py::arg("Tj").noconvert(), py::arg("influence").noconvert(), py::arg("splitting").noconvert(),
 R"pbdoc(
 Compute a C/F (coarse-fine( splitting using the classical coarse grid
 selection method of Ruge and Stuben.  The strength of connection matrix S,
 and its transpose T, are stored in CSR format.  Upon return, the  splitting
 array will consist of zeros and ones, where C-nodes (coarse nodes) are
 marked with the value 1 and F-nodes (fine nodes) with the value 0.
 
-Parameters:
-  n_nodes   - number of rows in A
-  C_rowptr[]      - CSR row pointer array for SOC matrix
-  C_colinds[]      - CSR column index array for SOC matrix
-  Tp[]      - CSR row pointer array for transpose of SOC matrix
-  Tj[]      - CSR column index array for transpose of SOC matrix
-  influence - array that influences splitting (values stored here are
-              added to lambda for each point)
-  splitting - array to store the C/F splitting
-
-Notes:
-  The splitting array must be preallocated)pbdoc");
+Parameters
+----------
+n_nodes : int
+    number of rows in A
+C_rowptr : array
+    CSR row pointer array for SOC matrix
+C_colinds : array
+    CSR column index array for SOC matrix
+Tp : array
+    CSR row pointer array for transpose of SOC matrix
+Tj : array
+    CSR column index array for transpose of SOC matrix
+influence : array
+    array that influences splitting (values stored here are
+    added to lambda for each point)
+splitting : array, inplace
+    array to store the C/F splitting
+
+Notes
+-----
+The splitting array must be preallocated)pbdoc");
 
     m.def("rs_cf_splitting_pass2", &_rs_cf_splitting_pass2<int>,
         py::arg("n_nodes"), py::arg("C_rowptr").noconvert(), py::arg("C_colinds").noconvert(), py::arg("splitting").noconvert(),
 R"pbdoc(
 )pbdoc");
 
     m.def("cljp_naive_splitting", &_cljp_naive_splitting<int>,
@@ -436,21 +463,35 @@
 
     m.def("rs_direct_interpolation_pass1", &_rs_direct_interpolation_pass1<int>,
         py::arg("n_nodes"), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("splitting").noconvert(), py::arg("Bp").noconvert(),
 R"pbdoc(
 Produce the Ruge-Stuben prolongator using "Direct Interpolation"
 
 
-  The first pass uses the strength of connection matrix 'S'
-  and C/F splitting to compute the row pointer for the prolongator.
+The first pass uses the strength of connection matrix 'S'
+and C/F splitting to compute the row pointer for the prolongator.
 
-  The second pass fills in the nonzero entries of the prolongator
+The second pass fills in the nonzero entries of the prolongator
 
-  Reference:
-     Page 479 of "Multigrid")pbdoc");
+Parameters
+----------
+n_nodes : int
+    Number of nodes
+Sp : array
+    Strength matrix row pointer array
+Sj : array
+    Strength matrix column index array
+splitting : array
+    C/F splitting
+Bp : array, inplace
+    Row pointer array
+
+References
+----------
+Page 479 of Multigrid)pbdoc");
 
     m.def("rs_direct_interpolation_pass2", &_rs_direct_interpolation_pass2<int, float>,
         py::arg("n_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("splitting").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert());
     m.def("rs_direct_interpolation_pass2", &_rs_direct_interpolation_pass2<int, double>,
         py::arg("n_nodes"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("splitting").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert(),
 R"pbdoc(
 )pbdoc");
@@ -459,34 +500,34 @@
         py::arg("A_rowptr").noconvert(), py::arg("A_colinds").noconvert(), py::arg("B").noconvert(), py::arg("e").noconvert(), py::arg("indices").noconvert(), py::arg("splitting").noconvert(), py::arg("gamma").noconvert(), py::arg("thetacs"));
     m.def("cr_helper", &_cr_helper<int, double>,
         py::arg("A_rowptr").noconvert(), py::arg("A_colinds").noconvert(), py::arg("B").noconvert(), py::arg("e").noconvert(), py::arg("indices").noconvert(), py::arg("splitting").noconvert(), py::arg("gamma").noconvert(), py::arg("thetacs"),
 R"pbdoc(
 Helper function for compatible relaxation to perform steps 3.1d - 3.1f
 in Falgout / Brannick (2010).
 
-Input:
-------
-A_rowptr : const {int array}
+Parameters
+----------
+A_rowptr : array
      Row pointer for sparse matrix in CSR format.
-A_colinds : const {int array}
+A_colinds : array
      Column indices for sparse matrix in CSR format.
-B : const {float array}
+B : array
      Target near null space vector for computing candidate set measure.
-e : {float array}
+e : array, inplace
      Relaxed vector for computing candidate set measure.
-indices : {int array}
+indices : array, inplace
      Array of indices, where indices[0] = the number of F indices, nf,
      followed by F indices in elements 1:nf, and C indices in (nf+1):n.
-splitting : {int array}
+splitting : array, inplace
      Integer array with current C/F splitting of nodes, 0 = C-point,
      1 = F-point.
-gamma : {float array}
+gamma : array, inplace
      Preallocated vector to store candidate set measure.
-thetacs : const {float}
+thetacs : float
      Threshold for coarse grid candidates from set measure.
 
-Returns:
---------
+Returns
+-------
 Nothing, updated C/F-splitting and corresponding indices modified in place.)pbdoc");
 
 }
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/smoothed_aggregation.h` & `pyamg-4.2.3/pyamg/amg_core/smoothed_aggregation.h`

 * *Files 9% similar despite different names*

```diff
@@ -9,42 +9,49 @@
 #include <assert.h>
 #include <cmath>
 
 #include "linalg.h"
 
 
 /*
- *  Compute a strength of connection matrix using the standard symmetric
- *  Smoothed Aggregation heuristic.  Both the input and output matrices
- *  are stored in CSR format.  A nonzero connection A[i,j] is considered
- *  strong if:
+ * Compute a strength of connection matrix using the standard symmetric
+ * Smoothed Aggregation heuristic.  Both the input and output matrices
+ * are stored in CSR format.  A nonzero connection A[i,j] is considered
+ * strong if:
  *
- *      abs(A[i,j]) >= theta * sqrt( abs(A[i,i]) * abs(A[j,j]) )
+ * ..
+ *     abs(A[i,j]) >= theta * sqrt( abs(A[i,i]) * abs(A[j,j]) )
  *
- *  The strength of connection matrix S is simply the set of nonzero entries
- *  of A that qualify as strong connections.
+ * The strength of connection matrix S is simply the set of nonzero entries
+ * of A that qualify as strong connections.
  *
- *  Parameters
- *      num_rows   - number of rows in A
- *      theta      - stength of connection tolerance
- *      Ap[]       - CSR row pointer
- *      Aj[]       - CSR index array
- *      Ax[]       - CSR data array
- *      Sp[]       - (output) CSR row pointer
- *      Sj[]       - (output) CSR index array
- *      Sx[]       - (output) CSR data array
- *
- *
- *  Returns:
- *      Nothing, S will be stored in Sp, Sj, Sx
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A
+ * theta : float
+ *     stength of connection tolerance
+ * Ap : array
+ *     CSR row pointer
+ * Aj : array
+ *     CSR index array
+ * Ax : array
+ *     CSR data array
+ * Sp : array, inplace
+ *     CSR row pointer
+ * Sj : array, inplace
+ *     CSR index array
+ * Sx : array, inplace
+ *     CSR data array
  *
- *  Notes:
- *      Storage for S must be preallocated.  Since S will consist of a subset
- *      of A's nonzero values, a conservative bound is to allocate the same
- *      storage for S as is used by A.
+ * Notes
+ * -----
+ * Storage for S must be preallocated.  Since S will consist of a subset
+ * of A's nonzero values, a conservative bound is to allocate the same
+ * storage for S as is used by A.
  *
  */
 template<class I, class T, class F>
 void symmetric_strength_of_connection(const I n_row,
                                       const F theta,
                                       const I Ap[], const int Ap_size,
                                       const I Aj[], const int Aj_size,
@@ -96,28 +103,37 @@
     }
 }
 
 
 /*
  * Compute aggregates for a matrix A stored in CSR format
  *
- * Parameters:
- *   n_row         - number of rows in A
- *   Ap[n_row + 1] - CSR row pointer
- *   Aj[nnz]       - CSR column indices
- *    x[n_row]     - aggregate numbers for each node
- *    y[n_row]     - will hold Cpts upon return
- *
- * Returns:
- *  The number of aggregates (== max(x[:]) + 1 )
- *
- * Notes:
- *    It is assumed that A is symmetric.
- *    A may contain diagonal entries (self loops)
- *    Unaggregated nodes are marked with a -1
+ * Parameters
+ * ----------
+ * n_row : int
+ *     number of rows in A
+ * Ap : array, n_row + 1
+ *     CSR row pointer
+ * Aj : array, nnz
+ *     CSR column indices
+ * x : array, n_row, inplace
+ *     aggregate numbers for each node
+ * y : array, n_row, inplace
+ *     will hold Cpts upon return
+ *
+ * Returns
+ * -------
+ * int
+ *     The number of aggregates (``== max(x[:]) + 1``)
+ *
+ * Notes
+ * -----
+ * - It is assumed that A is symmetric.
+ * - A may contain diagonal entries (self loops)
+ * - Unaggregated nodes are marked with a -1
  *
  */
 template <class I>
 I standard_aggregation(const I n_row,
                        const I Ap[], const int Ap_size,
                        const I Aj[], const int Aj_size,
                              I  x[], const int  x_size,
@@ -210,34 +226,42 @@
             if(x[j] == 0){ //unmarked neighbors
                 x[j] = next_aggregate;
             }
         }
         next_aggregate++;
     }
 
-
     return next_aggregate; //number of aggregates
 }
 
 
 
 /*
  * Compute aggregates for a matrix A stored in CSR format
  *
- * Parameters:
- *   n_row         - number of rows in A
- *   Ap[n_row + 1] - CSR row pointer
- *   Aj[nnz]       - CSR column indices
- *    x[n_row]     - aggregate numbers for each node
- *    y[n_row]     - will hold Cpts upon return
+ * Parameters
+ * ----------
+ * n_row : int
+ *     number of rows in A
+ * Ap : array, n_row + 1
+ *     CSR row pointer
+ * Aj : array, nnz
+ *     CSR column indices
+ * x : array, n_row, inplace
+ *     aggregate numbers for each node
+ * y : array, n_row, inplace
+ *     will hold Cpts upon return
  *
- * Returns:
- *  The number of aggregates (== max(x[:]) + 1 )
+ * Returns
+ * -------
+ * int
+ *     The number of aggregates (``== max(x[:]) + 1``)
  *
- * Notes:
+ * Notes
+ * -----
  * Differs from standard aggregation.  Each dof is considered.
  * If it has been aggregated, skip over.  Otherwise, put dof
  * and any unaggregated neighbors in an aggregate.  Results
  * in possibly much higher complexities.
  */
 template <class I>
 I naive_aggregation(const I n_row,
@@ -272,53 +296,60 @@
     }
 
     return (next_aggregate-1); //number of aggregates
 }
 
 
 /*
- *  Given a set of near-nullspace candidates stored in the columns of B, and
- *  an aggregation operator stored in A using BSR format, this method computes
- *      Ax : the data array of the tentative prolongator in BSR format
- *      R : the coarse level near-nullspace candidates
- *
- *  The tentative prolongator A and coarse near-nullspaces candidates satisfy
- *  the following relationships:
- *      B = A * R        and      transpose(A) * A = identity
- *
- *  Parameters
- *      num_rows   - number of rows in A
- *      num_cols   - number of columns in A
- *      K1         - BSR row blocksize
- *      K2         - BSR column blocksize
- *      Ap[]       - BSR row pointer
- *      Aj[]       - BSR index array
- *      Ax[]       - BSR data array
- *      B[]        - fine-level near-nullspace candidates (n_row x K2)
- *      R[]        - coarse-level near-nullspace candidates (n_coarse x K2)
- *      tol        - tolerance used to drop numerically linearly dependent vectors
+ * Given a set of near-nullspace candidates stored in the columns of B, and
+ * an aggregation operator stored in A using BSR format, this method computes
+ * Ax, the data array of the tentative prolongator in BSR format, and
+ * R, the coarse level near-nullspace candidates.
+ *
+ * The tentative prolongator A and coarse near-nullspaces candidates satisfy
+ * the following relationships:
+ * - ``B = A @ R``
+ * - ``transpose(A) @ A = identity``
  *
+ * Parameters
+ * ----------
+ * num_rows : int
+ *     number of rows in A
+ * num_cols : int
+ *     number of columns in A
+ * K1 : int
+ *     BSR row blocksize
+ * K2 : int
+ *     BSR column blocksize
+ * Ap : array
+ *     BSR row pointer
+ * Aj : array
+ *     BSR index array
+ * Ax : array, inplace
+ *     BSR data array
+ * B : array
+ *     fine-level near-nullspace candidates (n_row x K2)
+ * R : array, inplace
+ *     coarse-level near-nullspace candidates (n_coarse x K2)
+ * tol :float
+ *     tolerance used to drop numerically linearly dependent vectors
  *
- *  Returns:
- *      Nothing, Ax and R will be modified in places.
- *
- *  Notes:
- *      - Storage for Ax and R must be preallocated.
- *      - The tol parameter is applied to the candidates restricted to each
- *      aggregate to discard (redundant) numerically linear dependencies.
- *      For instance, if the restriction of two different fine-level candidates
- *      to a single aggregate are equal, then the second candidate will not
- *      contribute to the range of A.
- *      - When the aggregation operator does not aggregate all fine-level
- *      nodes, the corresponding rows of A will simply be zero.  In this case,
- *      the two relationships mentioned above do not hold.  Instead the following
- *      relationships are maintained:
- *             B[i,:] = A[i,:] * R     where  A[i,:] is nonzero
- *         and
- *             transpose(A[i,:]) * A[i,:] = 1   where A[i,:] is nonzero
+ * Notes
+ * -----
+ * - Storage for Ax and R must be preallocated.
+ * - The tol parameter is applied to the candidates restricted to each
+ * aggregate to discard (redundant) numerically linear dependencies.
+ * For instance, if the restriction of two different fine-level candidates
+ * to a single aggregate are equal, then the second candidate will not
+ * contribute to the range of A.
+ * - When the aggregation operator does not aggregate all fine-level
+ * nodes, the corresponding rows of A will simply be zero.  In this case,
+ * the two relationships mentioned above do not hold.  Instead the following
+ * relationships are maintained: ``B[i,:] = A[i,:] @ R`` where ``A[i,:]`` is nonzero
+ * and ``transpose(A[i,:]) * A[i,:] = 1`` where ``A[i,:]``is nonzero
  *
  */
 template <class I, class S, class T, class DOT, class NORM>
 void fit_candidates_common(const I n_row,
                            const I n_col,
                            const I   K1,
                            const I   K2,
@@ -494,66 +525,66 @@
                                   T  R[], const int  R_size,
                             const S  tol)
 { fit_candidates_common(n_row, n_col, K1, K2, Ap, Ai, Ax, B, R, tol, complex_dot<T>(), complex_norm<S,T>()); }
 
 
 /*
  * Helper routine for satisfy_constraints routine called
- *     by energy_prolongation_smoother(...) in smooth.py
- * This implements the python code:
- *
- *   # U is a BSR matrix, B is num_block_rows x cols_per_block x cols_per_block
- *   # UB is num_block_rows x rows_per_block x cols_per_block,  BtBinv is
- *        num_block_rows x cols_per_block x cols_per_block
- *   B  = asarray(B).reshape(-1,cols_per_block,B.shape[1])
- *   UB = asarray(UB).reshape(-1,rows_per_block,UB.shape[1])
- *
- *   rows = csr_matrix((U.indices,U.indices,U.indptr), \
- *           shape=(U.shape[0]/rows_per_block,U.shape[1]/cols_per_block)).tocoo(copy=False).row
- *   for n,j in enumerate(U.indices):
- *      i = rows[n]
- *      Bi  = mat(B[j])
- *      UBi = UB[i]
- *      U.data[n] -= dot(UBi,dot(BtBinv[i],Bi.H))
+ * by energy_prolongation_smoother(...) in smooth.py
  *
  * Parameters
  * ----------
- * rows_per_block : {int}
+ * rows_per_block : int
  *      rows per block in the BSR matrix, S
- * cols_per_block : {int}
+ * cols_per_block : int
  *      cols per block in the BSR matrix, S
- * num_block_rows : {int}
+ * num_block_rows : int
  *      Number of block rows, S.shape[0]/rows_per_block
- * NullDim : {int}
+ * NullDim : int
  *      Null-space dimension, i.e., the number of columns in B
- * x : {float|complex array}
+ * x : array
  *      Conjugate of near-nullspace vectors, B, in row major
- * y : {float|complex array}
+ * y : array
  *      S*B, in row major
- * z : {float|complex array}
+ * z : array
  *      BtBinv, in row major, i.e. z[i] = pinv(B_i.H Bi), where
  *      B_i is B restricted to the neighborhood of dof of i.
- * Sp : {int array}
+ * Sp : array
  *      Row pointer array for BSR matrix S
- * Sj : {int array}
+ * Sj : array
  *      Col index array for BSR matrix S
- * Sx : {float|complex array}
+ * Sx : array
  *      Value array for BSR matrix S
  *
  * Return
  * ------
  * Sx is modified such that S*B = 0.  S ends up being the
  * update to the prolongator in the energy_minimization algorithm.
  *
  * Notes
  * -----
  * Principle calling routine is energy_prolongation_smoother(...) in smooth.py.
  *
+ * This implements the python code:
+ *
+ * .. code-block:: python
+ *
+ *   # U is a BSR matrix, B is num_block_rows x cols_per_block x cols_per_block
+ *   # UB is num_block_rows x rows_per_block x cols_per_block,  BtBinv is
+ *        num_block_rows x cols_per_block x cols_per_block
+ *   B  = asarray(B).reshape(-1,cols_per_block,B.shape[1])
+ *   UB = asarray(UB).reshape(-1,rows_per_block,UB.shape[1])
+ *   rows = csr_matrix((U.indices,U.indices,U.indptr), \
+ *           shape=(U.shape[0]/rows_per_block,U.shape[1]/cols_per_block)).tocoo(copy=False).row
+ *   for n,j in enumerate(U.indices):
+ *      i = rows[n]
+ *      Bi  = mat(B[j])
+ *      UBi = UB[i]
+ *      U.data[n] -= dot(UBi,dot(BtBinv[i],Bi.H))
  */
-
 template<class I, class T, class F>
 void satisfy_constraints_helper(const I rows_per_block,
                                 const I cols_per_block,
                                  const I num_block_rows,
                                  const I NullDim,
                                  const T x[], const int x_size,
                                  const T y[], const int y_size,
@@ -601,58 +632,65 @@
         }
     }
 }
 
 
 /*
  * Helper routine for energy_prolongation_smoother
- * Calculates the following python code:
- *
- *   rows_per_block = Sparsity_Pattern.blocksize[0]
- *   BtB = zeros((Nnodes,NullDim,NullDim), dtype=B.dtype)
- *   S2 = Sparsity_Pattern.tocsr()
- *   for i in range(Nnodes):
- *       Bi = mat( B[S2.indices[S2.indptr[i*rows_per_block]:S2.indptr[i*rows_per_block + 1]],:] )
- *       BtB[i,:,:] = Bi.H*Bi
  *
  * Parameters
  * ----------
- * NullDim : {int}
+ * NullDim : int
  *      Number of near nullspace vectors
- * Nnodes : {int}
+ * Nnodes : int
  *      Number of nodes, i.e. number of block rows in BSR matrix, S
- * cols_per_block : {int}
+ * cols_per_block : int
  *      Columns per block in S
- * b : {float|complex array}
+ * b : array
  *      Nnodes x BsqCols array, in row-major form.
  *      This is B-squared, i.e. it is each column of B
  *      multiplied against each other column of B.  For a Nx3 B,
- *      b[:,0] = conjugate(B[:,0])*B[:,0]
- *      b[:,1] = conjugate(B[:,0])*B[:,1]
- *      b[:,2] = conjugate(B[:,0])*B[:,2]
- *      b[:,3] = conjugate(B[:,1])*B[:,1]
- *      b[:,4] = conjugate(B[:,1])*B[:,2]
- *      b[:,5] = conjugate(B[:,2])*B[:,2]
- * BsqCols : {int}
+ *
+ *      .. code-block:: python
+ *
+ *          b[:,0] = conjugate(B[:,0])*B[:,0]
+ *          b[:,1] = conjugate(B[:,0])*B[:,1]
+ *          b[:,2] = conjugate(B[:,0])*B[:,2]
+ *          b[:,3] = conjugate(B[:,1])*B[:,1]
+ *          b[:,4] = conjugate(B[:,1])*B[:,2]
+ *          b[:,5] = conjugate(B[:,2])*B[:,2]
+ *
+ * BsqCols : int
  *      sum(range(NullDim+1)), i.e. number of columns in b
  * x  : {float|complex array}
  *      Modified inplace for output.  Should be zeros upon entry
- * Sp,Sj : {int array}
+ * Sp,Sj : int array
  *      BSR indptr and indices members for matrix, S
  *
- * Return
- * ------
- * BtB[i] = B_i.H*B_i in __column__ major format
+ * Returns
+ * -------
+ * ``BtB[i] = B_i.H*B_i`` in column major format
  * where B_i is B[colindices,:], colindices = all the nonzero
  * column indices for block row i in S
  *
  * Notes
  * -----
  * Principle calling routine is energy_prolongation_smoother(...) in smooth.py.
  *
+ * Calculates the following python code:
+ *
+ * .. code-block:: python
+ *
+ *     rows_per_block = Sparsity_Pattern.blocksize[0]
+ *     BtB = zeros((Nnodes,NullDim,NullDim), dtype=B.dtype)
+ *     S2 = Sparsity_Pattern.tocsr()
+ *     for i in range(Nnodes):
+ *         Bi = mat( B[S2.indices[S2.indptr[i*rows_per_block]:S2.indptr[i*rows_per_block + 1]],:] )
+ *         BtB[i,:,:] = Bi.H*Bi
+ *
  */
 template<class I, class T, class F>
 void calc_BtB(const I NullDim,
               const I Nnodes,
               const I cols_per_block,
               const T  b[], const int  b_size,
               const I BsqCols,
@@ -733,17 +771,17 @@
 
 /*
  * Calculate A*B = S, but only at the pre-existing sparsity
  * pattern of S, i.e. do an exact, but incomplete mat-mat mult.
  *
  * A, B and S must all be in BSR, may be rectangular, but the
  * indices need not be sorted.
- * Also, A.blocksize[0] must equal S.blocksize[0]
- *       A.blocksize[1] must equal B.blocksize[0]
- *       B.blocksize[1] must equal S.blocksize[1]
+ * Also, A.blocksize[0] must equal S.blocksize[0],
+ * A.blocksize[1] must equal B.blocksize[0], and
+ * B.blocksize[1] must equal S.blocksize[1]
  *
  * Parameters
  * ----------
  * Ap : {int array}
  *      BSR row pointer array
  * Aj : {int array}
  *      BSR col index array
@@ -880,17 +918,17 @@
    x[i]   = x[j];
    x[j]   = temp_t;
    temp_i = y[i];
    y[i]   = y[j];
    y[j]   = temp_i;
 }
 
-/* Apply quicksort to the array x, while simultaneously shuffling 
- * the array y to mirror the swapping of entries done in x.   Then 
- * aftwards x[i] and y[i] correspond to some x[k] and y[k] 
+/* Apply quicksort to the array x, while simultaneously shuffling
+ * the array y to mirror the swapping of entries done in x.   Then
+ * aftwards x[i] and y[i] correspond to some x[k] and y[k]
  * before the sort.
  *
  * This function is particularly useful for sorting the rows (or columns)
  * of a sparse matrix according to the values
  * */
 template<class I, class T>
 void qsort_twoarrays( T x[], I y[], I left, I right )
@@ -903,39 +941,39 @@
     last = left;
     for (i = left+1; i <= right; i++)
     {
        if (mynorm(x[i]) < mynorm(x[left]))
        {    swap(x, y, ++last, i); }
     }
     swap(x, y, left, last);
-    
+
     /* Recursive calls */
     qsort_twoarrays(x, y, left, last-1);
     qsort_twoarrays(x, y, last+1, right);
 }
 
 /*
- *  Truncate the entries in A, such that only the largest (in magnitude) 
- *  k entries per row are left.   Smaller entries are zeroed out. 
+ *  Truncate the entries in A, such that only the largest (in magnitude)
+ *  k entries per row are left.   Smaller entries are zeroed out.
  *
  *  Parameters
- *      n_row      - number of rows in A 
+ *      n_row      - number of rows in A
  *      k          - number of entries per row to keep
  *      Sp[]       - CSR row pointer
  *      Sj[]       - CSR index array
  *      Sx[]       - CSR data array
  *
- *  
+ *
  *  Returns:
  *      Nothing, A will be stored in Sp, Sj, Sx with some entries zeroed out
  *
  */
 template<class I, class T, class F>
-void truncate_rows_csr(const I n_row, 
-                       const I k, 
+void truncate_rows_csr(const I n_row,
+                       const I k,
                        const I Sp[],  const int Sp_size,
                              I Sj[],  const int Sj_size,
                              T Sx[],  const int Sx_size)
 {
 
     // Loop over each row of A, sort based on the entries in Sx,
     // and then truncate all but the largest k entries
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/smoothed_aggregation_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/smoothed_aggregation_bind.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -357,78 +357,103 @@
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert());
     m.def("symmetric_strength_of_connection", &_symmetric_strength_of_connection<int, std::complex<float>, float>,
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert());
     m.def("symmetric_strength_of_connection", &_symmetric_strength_of_connection<int, std::complex<double>, double>,
         py::arg("n_row"), py::arg("theta"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(),
 R"pbdoc(
 Compute a strength of connection matrix using the standard symmetric
- Smoothed Aggregation heuristic.  Both the input and output matrices
- are stored in CSR format.  A nonzero connection A[i,j] is considered
- strong if:
-
-     abs(A[i,j]) >= theta * sqrt( abs(A[i,i]) * abs(A[j,j]) )
-
- The strength of connection matrix S is simply the set of nonzero entries
- of A that qualify as strong connections.
-
- Parameters
-     num_rows   - number of rows in A
-     theta      - stength of connection tolerance
-     Ap[]       - CSR row pointer
-     Aj[]       - CSR index array
-     Ax[]       - CSR data array
-     Sp[]       - (output) CSR row pointer
-     Sj[]       - (output) CSR index array
-     Sx[]       - (output) CSR data array
-
-
- Returns:
-     Nothing, S will be stored in Sp, Sj, Sx
-
- Notes:
-     Storage for S must be preallocated.  Since S will consist of a subset
-     of A's nonzero values, a conservative bound is to allocate the same
-     storage for S as is used by A.)pbdoc");
+Smoothed Aggregation heuristic.  Both the input and output matrices
+are stored in CSR format.  A nonzero connection A[i,j] is considered
+strong if:
+
+..
+    abs(A[i,j]) >= theta * sqrt( abs(A[i,i]) * abs(A[j,j]) )
+
+The strength of connection matrix S is simply the set of nonzero entries
+of A that qualify as strong connections.
+
+Parameters
+----------
+num_rows : int
+    number of rows in A
+theta : float
+    stength of connection tolerance
+Ap : array
+    CSR row pointer
+Aj : array
+    CSR index array
+Ax : array
+    CSR data array
+Sp : array, inplace
+    CSR row pointer
+Sj : array, inplace
+    CSR index array
+Sx : array, inplace
+    CSR data array
+
+Notes
+-----
+Storage for S must be preallocated.  Since S will consist of a subset
+of A's nonzero values, a conservative bound is to allocate the same
+storage for S as is used by A.)pbdoc");
 
     m.def("standard_aggregation", &_standard_aggregation<int>,
         py::arg("n_row"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("x").noconvert(), py::arg("y").noconvert(),
 R"pbdoc(
 Compute aggregates for a matrix A stored in CSR format
 
-Parameters:
-  n_row         - number of rows in A
-  Ap[n_row + 1] - CSR row pointer
-  Aj[nnz]       - CSR column indices
-   x[n_row]     - aggregate numbers for each node
-   y[n_row]     - will hold Cpts upon return
-
-Returns:
- The number of aggregates (== max(x[:]) + 1 )
-
-Notes:
-   It is assumed that A is symmetric.
-   A may contain diagonal entries (self loops)
-   Unaggregated nodes are marked with a -1)pbdoc");
+Parameters
+----------
+n_row : int
+    number of rows in A
+Ap : array, n_row + 1
+    CSR row pointer
+Aj : array, nnz
+    CSR column indices
+x : array, n_row, inplace
+    aggregate numbers for each node
+y : array, n_row, inplace
+    will hold Cpts upon return
+
+Returns
+-------
+int
+    The number of aggregates (``== max(x[:]) + 1``)
+
+Notes
+-----
+- It is assumed that A is symmetric.
+- A may contain diagonal entries (self loops)
+- Unaggregated nodes are marked with a -1)pbdoc");
 
     m.def("naive_aggregation", &_naive_aggregation<int>,
         py::arg("n_row"), py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("x").noconvert(), py::arg("y").noconvert(),
 R"pbdoc(
 Compute aggregates for a matrix A stored in CSR format
 
-Parameters:
-  n_row         - number of rows in A
-  Ap[n_row + 1] - CSR row pointer
-  Aj[nnz]       - CSR column indices
-   x[n_row]     - aggregate numbers for each node
-   y[n_row]     - will hold Cpts upon return
-
-Returns:
- The number of aggregates (== max(x[:]) + 1 )
+Parameters
+----------
+n_row : int
+    number of rows in A
+Ap : array, n_row + 1
+    CSR row pointer
+Aj : array, nnz
+    CSR column indices
+x : array, n_row, inplace
+    aggregate numbers for each node
+y : array, n_row, inplace
+    will hold Cpts upon return
+
+Returns
+-------
+int
+    The number of aggregates (``== max(x[:]) + 1``)
 
-Notes:
+Notes
+-----
 Differs from standard aggregation.  Each dof is considered.
 If it has been aggregated, skip over.  Otherwise, put dof
 and any unaggregated neighbors in an aggregate.  Results
 in possibly much higher complexities.)pbdoc");
 
     m.def("fit_candidates", &_fit_candidates_real<int, float>,
         py::arg("n_row"), py::arg("n_col"), py::arg("K1"), py::arg("K2"), py::arg("Ap").noconvert(), py::arg("Ai").noconvert(), py::arg("Ax").noconvert(), py::arg("B").noconvert(), py::arg("R").noconvert(), py::arg("tol"));
@@ -449,69 +474,127 @@
     m.def("satisfy_constraints_helper", &_satisfy_constraints_helper<int, double, double>,
         py::arg("rows_per_block"), py::arg("cols_per_block"), py::arg("num_block_rows"), py::arg("NullDim"), py::arg("x").noconvert(), py::arg("y").noconvert(), py::arg("z").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert());
     m.def("satisfy_constraints_helper", &_satisfy_constraints_helper<int, std::complex<float>, float>,
         py::arg("rows_per_block"), py::arg("cols_per_block"), py::arg("num_block_rows"), py::arg("NullDim"), py::arg("x").noconvert(), py::arg("y").noconvert(), py::arg("z").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert());
     m.def("satisfy_constraints_helper", &_satisfy_constraints_helper<int, std::complex<double>, double>,
         py::arg("rows_per_block"), py::arg("cols_per_block"), py::arg("num_block_rows"), py::arg("NullDim"), py::arg("x").noconvert(), py::arg("y").noconvert(), py::arg("z").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(),
 R"pbdoc(
-)pbdoc");
+Helper routine for satisfy_constraints routine called
+by energy_prolongation_smoother(...) in smooth.py
+
+Parameters
+----------
+rows_per_block : int
+     rows per block in the BSR matrix, S
+cols_per_block : int
+     cols per block in the BSR matrix, S
+num_block_rows : int
+     Number of block rows, S.shape[0]/rows_per_block
+NullDim : int
+     Null-space dimension, i.e., the number of columns in B
+x : array
+     Conjugate of near-nullspace vectors, B, in row major
+y : array
+     S*B, in row major
+z : array
+     BtBinv, in row major, i.e. z[i] = pinv(B_i.H Bi), where
+     B_i is B restricted to the neighborhood of dof of i.
+Sp : array
+     Row pointer array for BSR matrix S
+Sj : array
+     Col index array for BSR matrix S
+Sx : array
+     Value array for BSR matrix S
+
+Return
+------
+Sx is modified such that S*B = 0.  S ends up being the
+update to the prolongator in the energy_minimization algorithm.
+
+Notes
+-----
+Principle calling routine is energy_prolongation_smoother(...) in smooth.py.
+
+This implements the python code:
+
+.. code-block:: python
+
+  # U is a BSR matrix, B is num_block_rows x cols_per_block x cols_per_block
+  # UB is num_block_rows x rows_per_block x cols_per_block,  BtBinv is
+       num_block_rows x cols_per_block x cols_per_block
+  B  = asarray(B).reshape(-1,cols_per_block,B.shape[1])
+  UB = asarray(UB).reshape(-1,rows_per_block,UB.shape[1])
+  rows = csr_matrix((U.indices,U.indices,U.indptr), \
+          shape=(U.shape[0]/rows_per_block,U.shape[1]/cols_per_block)).tocoo(copy=False).row
+  for n,j in enumerate(U.indices):
+     i = rows[n]
+     Bi  = mat(B[j])
+     UBi = UB[i]
+     U.data[n] -= dot(UBi,dot(BtBinv[i],Bi.H)))pbdoc");
 
     m.def("calc_BtB", &_calc_BtB<int, float, float>,
         py::arg("NullDim"), py::arg("Nnodes"), py::arg("cols_per_block"), py::arg("b").noconvert(), py::arg("BsqCols"), py::arg("x").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert());
     m.def("calc_BtB", &_calc_BtB<int, double, double>,
         py::arg("NullDim"), py::arg("Nnodes"), py::arg("cols_per_block"), py::arg("b").noconvert(), py::arg("BsqCols"), py::arg("x").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert());
     m.def("calc_BtB", &_calc_BtB<int, std::complex<float>, float>,
         py::arg("NullDim"), py::arg("Nnodes"), py::arg("cols_per_block"), py::arg("b").noconvert(), py::arg("BsqCols"), py::arg("x").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert());
     m.def("calc_BtB", &_calc_BtB<int, std::complex<double>, double>,
         py::arg("NullDim"), py::arg("Nnodes"), py::arg("cols_per_block"), py::arg("b").noconvert(), py::arg("BsqCols"), py::arg("x").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(),
 R"pbdoc(
 Helper routine for energy_prolongation_smoother
-Calculates the following python code:
-
-  rows_per_block = Sparsity_Pattern.blocksize[0]
-  BtB = zeros((Nnodes,NullDim,NullDim), dtype=B.dtype)
-  S2 = Sparsity_Pattern.tocsr()
-  for i in range(Nnodes):
-      Bi = mat( B[S2.indices[S2.indptr[i*rows_per_block]:S2.indptr[i*rows_per_block + 1]],:] )
-      BtB[i,:,:] = Bi.H*Bi
 
 Parameters
 ----------
-NullDim : {int}
+NullDim : int
      Number of near nullspace vectors
-Nnodes : {int}
+Nnodes : int
      Number of nodes, i.e. number of block rows in BSR matrix, S
-cols_per_block : {int}
+cols_per_block : int
      Columns per block in S
-b : {float|complex array}
+b : array
      Nnodes x BsqCols array, in row-major form.
      This is B-squared, i.e. it is each column of B
      multiplied against each other column of B.  For a Nx3 B,
-     b[:,0] = conjugate(B[:,0])*B[:,0]
-     b[:,1] = conjugate(B[:,0])*B[:,1]
-     b[:,2] = conjugate(B[:,0])*B[:,2]
-     b[:,3] = conjugate(B[:,1])*B[:,1]
-     b[:,4] = conjugate(B[:,1])*B[:,2]
-     b[:,5] = conjugate(B[:,2])*B[:,2]
-BsqCols : {int}
+
+     .. code-block:: python
+
+         b[:,0] = conjugate(B[:,0])*B[:,0]
+         b[:,1] = conjugate(B[:,0])*B[:,1]
+         b[:,2] = conjugate(B[:,0])*B[:,2]
+         b[:,3] = conjugate(B[:,1])*B[:,1]
+         b[:,4] = conjugate(B[:,1])*B[:,2]
+         b[:,5] = conjugate(B[:,2])*B[:,2]
+
+BsqCols : int
      sum(range(NullDim+1)), i.e. number of columns in b
 x  : {float|complex array}
      Modified inplace for output.  Should be zeros upon entry
-Sp,Sj : {int array}
+Sp,Sj : int array
      BSR indptr and indices members for matrix, S
 
-Return
-------
-BtB[i] = B_i.H*B_i in __column__ major format
+Returns
+-------
+``BtB[i] = B_i.H*B_i`` in column major format
 where B_i is B[colindices,:], colindices = all the nonzero
 column indices for block row i in S
 
 Notes
 -----
-Principle calling routine is energy_prolongation_smoother(...) in smooth.py.)pbdoc");
+Principle calling routine is energy_prolongation_smoother(...) in smooth.py.
+
+Calculates the following python code:
+
+.. code-block:: python
+
+    rows_per_block = Sparsity_Pattern.blocksize[0]
+    BtB = zeros((Nnodes,NullDim,NullDim), dtype=B.dtype)
+    S2 = Sparsity_Pattern.tocsr()
+    for i in range(Nnodes):
+        Bi = mat( B[S2.indices[S2.indptr[i*rows_per_block]:S2.indptr[i*rows_per_block + 1]],:] )
+        BtB[i,:,:] = Bi.H*Bi)pbdoc");
 
     m.def("incomplete_mat_mult_bsr", &_incomplete_mat_mult_bsr<int, float, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("n_brow"), py::arg("n_bcol"), py::arg("brow_A"), py::arg("bcol_A"), py::arg("bcol_B"));
     m.def("incomplete_mat_mult_bsr", &_incomplete_mat_mult_bsr<int, double, double>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("n_brow"), py::arg("n_bcol"), py::arg("brow_A"), py::arg("bcol_A"), py::arg("bcol_B"));
     m.def("incomplete_mat_mult_bsr", &_incomplete_mat_mult_bsr<int, std::complex<float>, float>,
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("n_brow"), py::arg("n_bcol"), py::arg("brow_A"), py::arg("bcol_A"), py::arg("bcol_B"));
@@ -519,17 +602,17 @@
         py::arg("Ap").noconvert(), py::arg("Aj").noconvert(), py::arg("Ax").noconvert(), py::arg("Bp").noconvert(), py::arg("Bj").noconvert(), py::arg("Bx").noconvert(), py::arg("Sp").noconvert(), py::arg("Sj").noconvert(), py::arg("Sx").noconvert(), py::arg("n_brow"), py::arg("n_bcol"), py::arg("brow_A"), py::arg("bcol_A"), py::arg("bcol_B"),
 R"pbdoc(
 Calculate A*B = S, but only at the pre-existing sparsity
 pattern of S, i.e. do an exact, but incomplete mat-mat mult.
 
 A, B and S must all be in BSR, may be rectangular, but the
 indices need not be sorted.
-Also, A.blocksize[0] must equal S.blocksize[0]
-      A.blocksize[1] must equal B.blocksize[0]
-      B.blocksize[1] must equal S.blocksize[1]
+Also, A.blocksize[0] must equal S.blocksize[0],
+A.blocksize[1] must equal B.blocksize[0], and
+B.blocksize[1] must equal S.blocksize[1]
 
 Parameters
 ----------
 Ap : {int array}
      BSR row pointer array
 Aj : {int array}
      BSR col index array
```

### Comparing `pyamg-4.2.2/pyamg/amg_core/tests/bind_examples.h` & `pyamg-4.2.3/pyamg/amg_core/tests/bind_examples.h`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/tests/bind_examples_bind.cpp` & `pyamg-4.2.3/pyamg/amg_core/tests/bind_examples_bind.cpp`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/amg_core/tests/test_bind_examples.py` & `pyamg-4.2.3/pyamg/amg_core/tests/test_bind_examples.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/blackbox.py` & `pyamg-4.2.3/pyamg/blackbox.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/classical/classical.py` & `pyamg-4.2.3/pyamg/classical/classical.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
                        max_levels=10, max_coarse=10, keep=False, **kwargs):
     """Create a multilevel solver using Classical AMG (Ruge-Stuben AMG).
 
     Parameters
     ----------
     A : csr_matrix
         Square matrix in CSR format
-    strength : ['symmetric', 'classical', 'evolution', 'distance',
-                'algebraic_distance','affinity', 'energy_based', None]
+    strength : string
+        Valid strings are ['symmetric', 'classical', 'evolution', 'distance',
+        'algebraic_distance','affinity', 'energy_based', None].
         Method used to determine the strength of connection between unknowns
         of the linear system.  Method-specific parameters may be passed in
         using a tuple, e.g. strength=('symmetric',{'theta' : 0.25 }). If
         strength=None, all nonzero entries of the matrix are considered strong.
     CF : string
         Method used for coarse grid selection (C/F splitting)
         Supported methods are RS, PMIS, PMISc, CLJP, CLJPc, and CR.
@@ -80,15 +81,14 @@
     .. [2001TrOoSc] Trottenberg, U., Oosterlee, C. W., and Schuller, A.,
        "Multigrid" San Diego: Academic Press, 2001.  Appendix A
 
     See Also
     --------
     aggregation.smoothed_aggregation_solver, MultilevelSolver,
     aggregation.rootnode_solver
-
     """
     levels = [MultilevelSolver.Level()]
 
     # convert A to csr
     if not isspmatrix_csr(A):
         try:
             A = csr_matrix(A)
```

### Comparing `pyamg-4.2.2/pyamg/classical/cr.py` & `pyamg-4.2.3/pyamg/classical/cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/classical/interpolate.py` & `pyamg-4.2.3/pyamg/classical/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/classical/split.py` & `pyamg-4.2.3/pyamg/classical/split.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/classical/tests/test_classical.py` & `pyamg-4.2.3/pyamg/classical/tests/test_classical.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/classical/tests/test_cr.py` & `pyamg-4.2.3/pyamg/classical/tests/test_cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/__init__.py` & `pyamg-4.2.3/pyamg/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/demo.py` & `pyamg-4.2.3/pyamg/gallery/demo.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/diffusion.py` & `pyamg-4.2.3/pyamg/gallery/diffusion.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,40 @@
     >>> from pyamg.gallery.diffusion import diffusion_stencil_2d
     >>> sten = diffusion_stencil_2d(epsilon=0.0001,theta=sp.pi/6,type='FD')
     >>> print(sten)
     [[-0.2164847 -0.750025   0.2164847]
      [-0.250075   2.0002    -0.250075 ]
      [ 0.2164847 -0.750025  -0.2164847]]
 
+    Considered a 2 x 4 grid
+    x--x--x
+    |  |  |
+    x--x--x
+    |  |  |
+    x--x--x
+    |  |  |
+    x--x--x
+    The first dimension of the stencil defines
+    >>> nx, ny = (2, 4)
+    >>> sten = pyamg.gallery.diffusion_stencil_2d(epsilon=0.1, type='FD')
+    >>> A = pyamg.gallery.stencil_grid(sten, (nx, ny)).toarray()
+    >>> print(sten)
+        [[-0.  -1.   0. ]
+         [-0.1  2.2 -0.1]
+         [ 0.  -1.  -0. ]]
+    >>> print(A)
+        [[ 2.2 -0.1  0.   0.  -1.   0.   0.   0. ]
+         [-0.1  2.2 -0.1  0.   0.  -1.   0.   0. ]
+         [ 0.  -0.1  2.2 -0.1  0.   0.  -1.   0. ]
+         [ 0.   0.  -0.1  2.2  0.   0.   0.  -1. ]
+         [-1.   0.   0.   0.   2.2 -0.1  0.   0. ]
+         [ 0.  -1.   0.   0.  -0.1  2.2 -0.1  0. ]
+         [ 0.   0.  -1.   0.   0.  -0.1  2.2 -0.1]
+         [ 0.   0.   0.  -1.   0.   0.  -0.1  2.2]]
+
     """
     eps = float(epsilon)  # for brevity
     theta = float(theta)
 
     C = np.cos(theta)
     S = np.sin(theta)
     CS = C*S
```

### Comparing `pyamg-4.2.2/pyamg/gallery/elasticity.py` & `pyamg-4.2.3/pyamg/gallery/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example.py` & `pyamg-4.2.3/pyamg/gallery/example.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/README.txt` & `pyamg-4.2.3/pyamg/gallery/example_data/README.txt`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/airfoil.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/airfoil.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/bar.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/bar.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/helmholtz_2D.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/helmholtz_2D.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/knot.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/knot.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/local_disc_galerkin_diffusion.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/recirc_flow.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/recirc_flow.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/unit_cube.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/unit_cube.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/example_data/unit_square.mat` & `pyamg-4.2.3/pyamg/gallery/example_data/unit_square.mat`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/fem.py` & `pyamg-4.2.3/pyamg/gallery/fem.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,14 +518,33 @@
             if move < tol:
                 break
 
         self.V = Vnew
         return _it
 
 
+def _compute_diffusion_matrix(kappa_lmbda, x, y):
+    """Standardize diffusion tensor/scalar.
+
+    This will return an ndarray or a scalar, depending on input.
+    """
+    kappa = kappa_lmbda(x, y)
+
+    if isinstance(kappa, (int, float)):
+        return np.eye(2) * kappa
+
+    if isinstance(kappa, np.ndarray):
+        if kappa.shape == (2, 2):
+            return kappa
+        raise ValueError(f'kappa must return a scalar or ndarray of shape (2,2), '
+                         f'received ndarray of shape {kappa.shape}')
+    raise ValueError(f'kappa must return a scalar or ndarray of shape (2,2), '
+                     f'received type {type(kappa)}')
+
+
 def gradgradform(mesh, kappa=None, f=None, degree=1):
     """Finite element discretization of a Poisson problem.
 
     - div . kappa(x,y) grad u = f(x,y)
 
     Parameters
     ----------
@@ -533,14 +552,15 @@
         nv x 2 list of coordinates
 
     E : ndarray
         ne x 3 or 6 list of vertices
 
     kappa : function
         diffusion coefficient, kappa(x,y) with vector input
+        can either return a scalar value or a 2x2 matrix that transforms <grad u>
 
     f : function
         right hand side, f(x,y) with vector input
 
     degree : 1 or 2
         polynomial degree of the bases (assumed to be Lagrange locally)
 
@@ -553,16 +573,16 @@
         finite element rhs where b_ij = <f, phi_j>
 
     Notes
     -----
         - modepy is used to generate the quadrature points
           q = modepy.XiaoGimbutasSimplexQuadrature(4,2)
 
-    Example
-    -------
+    Examples
+    --------
     >>> import numpy as np
     >>> from pyamg.gallery import fem
     >>> import scipy.sparse.linalg as sla
     >>> V = np.array(
     ... [[  0,  0],
     ...  [  1,  0],
     ...  [2*1,  0],
@@ -677,15 +697,16 @@
             dbasis = np.array([[-1, 1, 0],
                                [-1, 0, 1]])
 
             # Step 4
             dphi = invJ.dot(dbasis)
 
             # Step 5, 1-point gauss quadrature
-            Aelem = kappa(X[K].mean(), Y[K].mean()) * (detJ / 2.0) * (dphi.T).dot(dphi)
+            kappaelem = _compute_diffusion_matrix(kappa, X[K].mean(), Y[K].mean())
+            Aelem = (detJ / 2.0) * dphi.T @ kappaelem @ dphi
 
             # Step 6, 1-point gauss quadrature
             belem = f(X[K].mean(), Y[K].mean()) * (detJ / 6.0) * np.ones((3,))
 
         if degree == 2:
             ww = np.array([0.44676317935602256, 0.44676317935602256, 0.44676317935602256,
                            0.21990348731064327, 0.21990348731064327, 0.21990348731064327])
@@ -716,15 +737,16 @@
                 ])
 
                 # Step 4
                 dphi = invJ.dot(dbasis)
 
                 # Step 5
                 xt, yt = J.dot(np.array([x, y])) + np.array([x0, y0])
-                Aelem += (detJ / 2) * w * kappa(xt, yt) * dphi.T.dot(dphi)
+                kappaelem = _compute_diffusion_matrix(kappa, xt, yt)
+                Aelem += (detJ / 2) * w * dphi.T @ kappaelem @ dphi
 
                 # Step 6
                 belem += (detJ / 2) * w * f(xt, yt) * basis
 
         # Step 7
         AA[ei, :] = Aelem.ravel()
         IA[ei, :] = np.repeat(K[np.arange(m)], m)
@@ -938,16 +960,16 @@
     """Construct model elliptic problem.
 
     Parameters
     ----------
     num : int or string
         A tag for a particular problem.  See the notes below.
 
-    Return
-    ------
+    Returns
+    -------
     A
     b
     V
     E
     f
     kappa
     bc
```

### Comparing `pyamg-4.2.2/pyamg/gallery/laplacian.py` & `pyamg-4.2.3/pyamg/gallery/laplacian.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 def poisson(grid, dtype=float, format=None, type='FD'):
     """Return a sparse matrix for the N-dimensional Poisson problem.
 
     The matrix represents a finite Difference approximation to the
     Poisson problem on a regular n-dimensional grid with unit grid
     spacing and Dirichlet boundary conditions.
 
+    The last dimension is iterated over first: z, then y, then x.
+    This should be used with np.mgrid() or np.ndenumerate.
+
     Parameters
     ----------
     grid : tuple of integers
         grid dimensions e.g. (100,100)
 
     Notes
     -----
@@ -37,15 +40,14 @@
     >>> poisson((2,3)).toarray()
     array([[ 4., -1.,  0., -1.,  0.,  0.],
            [-1.,  4., -1.,  0., -1.,  0.],
            [ 0., -1.,  4.,  0.,  0., -1.],
            [-1.,  0.,  0.,  4., -1.,  0.],
            [ 0., -1.,  0., -1.,  4., -1.],
            [ 0.,  0., -1.,  0., -1.,  4.]])
-
     """
     grid = tuple(grid)
 
     N = len(grid)  # grid dimension
 
     if N < 1 or min(grid) < 1:
         raise ValueError(f'Invalid grid shape: {grid}')
```

### Comparing `pyamg-4.2.2/pyamg/gallery/mesh.py` & `pyamg-4.2.3/pyamg/gallery/mesh.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/mesh_data/square_mesh.npz` & `pyamg-4.2.3/pyamg/gallery/mesh_data/square_mesh.npz`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/random_sparse.py` & `pyamg-4.2.3/pyamg/gallery/random_sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     m, n : int
         shape of the result
     density : float
         target a matrix with nnz(A) = m*n*density, 0<=density<=1
     format : string
         sparse matrix format to return, e.g. 'csr', 'coo', etc.
 
-    Return
-    ------
+    Returns
+    -------
     A : sparse matrix
         m x n sparse matrix
 
     Examples
     --------
     >>> from pyamg.gallery import sprand
     >>> A = sprand(5,5,3/5.0)
```

### Comparing `pyamg-4.2.2/pyamg/gallery/stencil.py` & `pyamg-4.2.3/pyamg/gallery/stencil.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_diffusion.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_elasticity.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_elasticity.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_example.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_laplacian.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_mesh.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/gallery/tests/test_stencil.py` & `pyamg-4.2.3/pyamg/gallery/tests/test_stencil.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/graph.py` & `pyamg-4.2.3/pyamg/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,27 @@
 
     Returns
     -------
     distances : array
         Distance of each point to the nearest seed
     nearest_seed : array
         Index of the nearest seed
+
+    Notes
+    -----
+    This should be viewed as the transpose of Bellman-Ford in
+    scipy.sparse.csgraph. Here, bellman_ford is used to find the shortest path
+    from any point *to* the seeds. In csgraph, bellman_ford is used to find
+    "the shortest distance from point i to point j".  So csgraph.bellman_ford
+    could be run `for seed in seeds`.  Also note that `test_graph.py` tests
+    against `csgraph.bellman_ford(G.T)`.
+
+    See Also
+    --------
+    scipy.sparse.csgraph.bellman_ford
     """
     G = asgraph(G)
     N = G.shape[0]
 
     if G.nnz > 0:
         if G.data.min() < 0:
             raise ValueError('Bellman-Ford is defined only for positive weights.')
```

### Comparing `pyamg-4.2.2/pyamg/graph_ref.py` & `pyamg-4.2.3/pyamg/graph_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     ----------
     A : coo sparse matrix
         n x n directed graph with positive weights
 
     c : array_like
         list of cluster centers
 
-    Return
-    ------
+    Returns
+    -------
     m : ndarray
         cluster index
 
     d : ndarray
         distance to cluster center
 
     See Also
```

### Comparing `pyamg-4.2.2/pyamg/krylov/__init__.py` & `pyamg-4.2.3/pyamg/krylov/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - gmres
     - fgmres
     - cgne
     - cgnr
     - cg
     - bicgstab
     - steepest descent, (simple iteration)
-    - minimial residual (MR), (simple iteration)
+    - minimal residual (MR), (simple iteration)
 
 
 References
 ----------
 .. [1] Yousef Saad, "Iterative Methods for Sparse Linear Systems,
    Second Edition", SIAM, pp. 231-234, 2003
    http://www-users.cs.umn.edu/~saad/books.html
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_bicgstab.py` & `pyamg-4.2.3/pyamg/krylov/_bicgstab.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/_cg.py` & `pyamg-4.2.3/pyamg/krylov/_cg.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/_cgne.py` & `pyamg-4.2.3/pyamg/krylov/_cgne.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/_cgnr.py` & `pyamg-4.2.3/pyamg/krylov/_cgnr.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/_cr.py` & `pyamg-4.2.3/pyamg/krylov/_cr.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/_fgmres.py` & `pyamg-4.2.3/pyamg/krylov/_fgmres.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         n x n, linear system to solve
     b : array, matrix
         right hand side, shape is (n,) or (n,1)
     x0 : array, matrix
         initial guess, default is a vector of zeros
     tol : float
         Tolerance for stopping criteria, let r=r_k
-           ||r||     < tol ||b||
+        ||r|| < tol ||b||
         if ||b||=0, then set ||b||=1 for these tests.
     restrt : None, int
         - if int, restrt is max number of inner iterations
           and maxiter is the max number of outer iterations
         - if None, do not restart GMRES, and max number of inner iterations
           is maxiter
     maxiter : None, int
@@ -130,19 +130,19 @@
             max_outer = 1
         if restrt > n:
             warn('Setting restrt to maximum allowed, n.')
             restrt = n
         max_inner = restrt
     else:
         max_outer = 1
-        if maxiter > n:
+        if maxiter is None:
+            maxiter = min(n, 40)
+        elif maxiter > n:
             warn('Setting maxiter to maximum allowed, n.')
             maxiter = n
-        elif maxiter is None:
-            maxiter = min(n, 40)
         max_inner = maxiter
 
     # Is this a one dimensional matrix?
     if n == 1:
         entry = np.ravel(A @ np.array([1.0], dtype=x.dtype))
         return (postprocess(b/entry), 0)
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_gmres.py` & `pyamg-4.2.3/pyamg/krylov/_gmres.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         n x n, linear system to solve
     b : array, matrix
         right hand side, shape is (n,) or (n,1)
     x0 : array, matrix
         initial guess, default is a vector of zeros
     tol : float
         Tolerance for stopping criteria, let r=r_k
-           ||M r||     < tol ||M b||
+        ||M r|| < tol ||M b||
         if ||b||=0, then set ||M b||=1 for these tests.
     restrt : None, int
         - if int, restrt is max number of inner iterations
           and maxiter is the max number of outer iterations
         - if None, do not restart GMRES, and max number of inner iterations
           is maxiter
     maxiter : None, int
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_gmres_householder.py` & `pyamg-4.2.3/pyamg/krylov/_gmres_householder.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         n x n, linear system to solve
     b : array, matrix
         right hand side, shape is (n,) or (n,1)
     x0 : array, matrix
         initial guess, default is a vector of zeros
     tol : float
         Tolerance for stopping criteria, let r=r_k
-           ||M r||     < tol ||M b||
+        ||M r|| < tol ||M b||
         if ||b||=0, then set ||M b||=1 for these tests.
     restrt : None, int
         - if int, restrt is max number of inner iterations
           and maxiter is the max number of outer iterations
         - if None, do not restart GMRES, and max number of inner iterations
           is maxiter
     maxiter : None, int
@@ -128,19 +128,19 @@
             max_outer = 1
         if restrt > n:
             warn('Setting restrt to maximum allowed, n.')
             restrt = n
         max_inner = restrt
     else:
         max_outer = 1
-        if maxiter > n:
+        if maxiter is None:
+            maxiter = min(n, 40)
+        elif maxiter > n:
             warn('Setting maxiter to maximum allowed, n.')
             maxiter = n
-        elif maxiter is None:
-            maxiter = min(n, 40)
         max_inner = maxiter
 
     # Is this a one dimensional matrix?
     if n == 1:
         entry = np.ravel(A @ np.array([1.0], dtype=x.dtype))
         return (postprocess(b/entry), 0)
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_gmres_mgs.py` & `pyamg-4.2.3/pyamg/krylov/_gmres_mgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         n x n, linear system to solve
     b : array, matrix
         right hand side, shape is (n,) or (n,1)
     x0 : array, matrix
         initial guess, default is a vector of zeros
     tol : float
         Tolerance for stopping criteria, let r=r_k
-           ||M r||     < tol ||M b||
+        ||M r|| < tol ||M b||
         if ||b||=0, then set ||M b||=1 for these tests.
     restrt : None, int
         - if int, restrt is max number of inner iterations
           and maxiter is the max number of outer iterations
         - if None, do not restart GMRES, and max number of inner iterations
           is maxiter
     maxiter : None, int
@@ -158,19 +158,19 @@
             max_outer = 1
         if restrt > n:
             warn('Setting restrt to maximum allowed, n.')
             restrt = n
         max_inner = restrt
     else:
         max_outer = 1
-        if maxiter > n:
+        if maxiter is None:
+            maxiter = min(n, 40)
+        elif maxiter > n:
             warn('Setting maxiter to maximum allowed, n.')
             maxiter = n
-        elif maxiter is None:
-            maxiter = min(n, 40)
         max_inner = maxiter
 
     # Is this a one dimensional matrix?
     if n == 1:
         entry = np.ravel(A @ np.array([1.0], dtype=x.dtype))
         return (postprocess(b/entry), 0)
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_minimal_residual.py` & `pyamg-4.2.3/pyamg/krylov/_minimal_residual.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         n x n, linear system to solve
     b : array, matrix
         right hand side, shape is (n,) or (n,1)
     x0 : array, matrix
         initial guess, default is a vector of zeros
     tol : float
         Tolerance for stopping criteria, let r=r_k
-           ||M r||     < tol ||M b||
+        ||M r|| < tol ||M b||
         if ||b||=0, then set ||M b||=1 for these tests.
     maxiter : int
         maximum number of iterations allowed
     M : array, matrix, sparse matrix, LinearOperator
         n x n, inverted preconditioner, i.e. solve M A x = M b.
     callback : function
         User-supplied function is called after each iteration as
@@ -52,21 +52,22 @@
 
     Notes
     -----
     The LinearOperator class is in scipy.sparse.linalg.
     Use this class if you prefer to define A or M as a mat-vec routine
     as opposed to explicitly constructing the matrix.
 
-    minimal residual algorithm:      Preconditioned version:
-    r = b - A x                      r = b - A x, z = M r
-    while not converged:             while not converged:
-        p = A r                          p = M A z
-        alpha = (p,r) / (p,p)            alpha = (p, z) / (p, p)
-        x = x + alpha r                  x = x + alpha z
-        r = r - alpha p                  z = z - alpha p
+    ..
+        minimal residual algorithm:      Preconditioned version:
+        r = b - A x                      r = b - A x, z = M r
+        while not converged:             while not converged:
+            p = A r                          p = M A z
+            alpha = (p,r) / (p,p)            alpha = (p, z) / (p, p)
+            x = x + alpha r                  x = x + alpha z
+            r = r - alpha p                  z = z - alpha p
 
     See Also
     --------
     _steepest_descent
 
     Examples
     --------
```

### Comparing `pyamg-4.2.2/pyamg/krylov/_steepest_descent.py` & `pyamg-4.2.3/pyamg/krylov/_steepest_descent.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/tests/test_krylov.py` & `pyamg-4.2.3/pyamg/krylov/tests/test_krylov.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import pyamg
 from pyamg.util.linalg import norm
 from pyamg.krylov import bicgstab, cg, cgne, cgnr, cr, fgmres, gmres, steepest_descent
 from pyamg.krylov._gmres_householder import gmres_householder
 from pyamg.krylov._gmres_mgs import gmres_mgs
 
+import pytest
+
 
 class TestStoppingCriteria(TestCase):
     def setUp(self):
         self.cases = []
 
         np.random.seed(9062883)
         n = 10
@@ -244,7 +246,20 @@
                 b = case['b']
                 x0 = case['x0']
                 xNew, _ = method(A, b, x0=x0, tol=case['tol'],
                                  maxiter=A.shape[0])
                 xNew = xNew.reshape(-1, 1)
                 assert_equal((norm(b - A.dot(xNew)) / norm(b - A.dot(x0))) < 0.35,
                              True, err_msg='Inexact Krylov Method Failed Test')
+
+
+np.random.seed(751537155)
+A = pyamg.gallery.poisson((10,), format='csr')
+b = np.random.rand(A.shape[0])
+
+
+@pytest.mark.parametrize('method', [fgmres, gmres_mgs, gmres_householder, gmres,
+                                    bicgstab, cg, cgne, cgnr, cr])
+def test_defaults(method):
+    x, info = method(A, b)
+    assert info == 0
+    assert np.linalg.norm(b - A @ x) < np.linalg.norm(b)
```

### Comparing `pyamg-4.2.2/pyamg/krylov/tests/test_scipy.py` & `pyamg-4.2.3/pyamg/krylov/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/krylov/tests/test_simple_iterations.py` & `pyamg-4.2.3/pyamg/krylov/tests/test_simple_iterations.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/multilevel.py` & `pyamg-4.2.3/pyamg/multilevel.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/__init__.py` & `pyamg-4.2.3/pyamg/relaxation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/chebyshev.py` & `pyamg-4.2.3/pyamg/relaxation/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/relaxation.py` & `pyamg-4.2.3/pyamg/relaxation/relaxation.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/smoothing.py` & `pyamg-4.2.3/pyamg/relaxation/smoothing.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/tests/test_relaxation.py` & `pyamg-4.2.3/pyamg/relaxation/tests/test_relaxation.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/tests/test_smoothing.py` & `pyamg-4.2.3/pyamg/relaxation/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/relaxation/utils.py` & `pyamg-4.2.3/pyamg/relaxation/utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/strength.py` & `pyamg-4.2.3/pyamg/strength.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/tests/test_blackbox.py` & `pyamg-4.2.3/pyamg/tests/test_blackbox.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/tests/test_clustering.py` & `pyamg-4.2.3/pyamg/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/tests/test_graph.py` & `pyamg-4.2.3/pyamg/tests/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Test graph routings."""
 import numpy as np
 import scipy.sparse as sparse
 
-from numpy.testing import TestCase, assert_equal
+from numpy.testing import TestCase, assert_equal, assert_array_almost_equal
 
 from pyamg.gallery import poisson, load_example
 from pyamg.graph import (maximal_independent_set, vertex_coloring,
                          bellman_ford, lloyd_cluster, connected_components)
 from pyamg.graph_ref import bellman_ford_reference
+from scipy.sparse.csgraph import bellman_ford as bellman_ford_scipy
 from pyamg import amg_core
 
 
 def canonical_graph(G):
     # convert to expected format
     # - remove diagonal entries
     # - all nonzero values = 1
@@ -109,16 +110,22 @@
                     continue
 
                 seeds = np.random.permutation(N)[:n_seeds]
 
                 D_result, S_result = bellman_ford(G, seeds)
                 D_expected, S_expected = bellman_ford_reference(G, seeds)
 
-                assert_equal(D_result, D_expected)
-                assert_equal(S_result, S_expected)
+                assert_array_almost_equal(D_result, D_expected)
+                assert_array_almost_equal(S_result, S_expected)
+
+                # test only small matrices with scipy
+                if G.shape[0] < 15:
+                    D = bellman_ford_scipy(csgraph=G.T)
+                    D_scipy = D[:, seeds].min(axis=1).ravel()
+                    assert_array_almost_equal(D_result, D_scipy)
 
     def test_bellman_ford_reference(self):
         Edges = np.array([[1, 4],
                           [3, 1],
                           [1, 3],
                           [0, 1],
                           [0, 2],
```

### Comparing `pyamg-4.2.2/pyamg/tests/test_multilevel.py` & `pyamg-4.2.3/pyamg/tests/test_multilevel.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/tests/test_strength.py` & `pyamg-4.2.3/pyamg/tests/test_strength.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/bsr_utils.py` & `pyamg-4.2.3/pyamg/util/bsr_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/linalg.py` & `pyamg-4.2.3/pyamg/util/linalg.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/params.py` & `pyamg-4.2.3/pyamg/util/params.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/tests/test_bsr_utils.py` & `pyamg-4.2.3/pyamg/util/tests/test_bsr_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/tests/test_linalg.py` & `pyamg-4.2.3/pyamg/util/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/tests/test_utils.py` & `pyamg-4.2.3/pyamg/util/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/util/utils.py` & `pyamg-4.2.3/pyamg/util/utils.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/vis/tests/test_vis.py` & `pyamg-4.2.3/pyamg/vis/tests/test_vis.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/vis/tests/test_vtu.py` & `pyamg-4.2.3/pyamg/vis/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `pyamg-4.2.2/pyamg/vis/vis_coarse.py` & `pyamg-4.2.3/pyamg/vis/vis_coarse.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     mesh_type : {string}
         type of elements: vertex, tri, quad, tet, hex (all 3d)
     fname : {string, file object}
         file to be written, e.g. 'output.vtu'
 
     Returns
     -------
-        - Writes data to .vtu file for use in paraview (xml 0.1 format) or
-          displays to screen using matplotlib
+    Writes data to .vtu file for use in paraview (xml 0.1 format) or
+    displays to screen using matplotlib
 
     Notes
     -----
-        - Works for both 2d and 3d elements.  Element groupings are colored
-          with data equal to 2.0 and stringy edges in the aggregate are colored
-          with 3.0
+    Works for both 2d and 3d elements.  Element groupings are colored
+    with data equal to 2.0 and stringy edges in the aggregate are colored
+    with 3.0
 
     Examples
     --------
     >>> from pyamg.aggregation import standard_aggregation
     >>> from pyamg.vis.vis_coarse import vis_aggregate_groups
     >>> from pyamg.gallery import load_example
     >>> data = load_example('unit_square')
@@ -151,16 +151,16 @@
     fname : {string, file object}
         file to be written, e.g. 'output.vtu'
     output : {string}
         'vtk' or 'matplotlib'
 
     Returns
     -------
-        - Displays in screen or writes data to .vtu file for use in paraview
-          (xml 0.1 format)
+    Displays in screen or writes data to .vtu file for use in paraview
+    (xml 0.1 format)
 
     Notes
     -----
     D :
         dimension of coordinate space
     N :
         # of vertices in the mesh represented in V
```

### Comparing `pyamg-4.2.2/pyamg/vis/vtk_writer.py` & `pyamg-4.2.3/pyamg/vis/vtk_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     cdata : {dictionary}
         scalar valued cell data
     cvdata : {dictionary}
         vector valued cell data
 
     Returns
     -------
-     writes a .vtu file for use in Paraview
+    writes a .vtu file for use in Paraview
 
     Notes
     -----
     - Poly data not supported
     - Non-Poly data is stored in Numpy array: Ncell x vtk_cell_info
     - Each I1 must be >=3
     - pdata = Ndof x Nfields
@@ -199,17 +199,18 @@
                 cvdata[key] = cvdata[key].reshape((cvdata[key].size, 1))
             if cvdata[key].shape[0] != 3 * cells[key].shape[0]:
                 raise ValueError('size mismatch with cvdata and cells')
             if cvdata[key] is None:
                 raise ValueError(f'cvdata array cannot be empty for key {key}')
 
     Ncells = 0
-    cell_ind = []
-    cell_offset = []  # np.zeros((Ncells,1),dtype=uint8) # zero indexed
-    cell_type = []    # np.zeros((Ncells,1),dtype=uint8)
+    cell_ind = np.empty((0,), dtype=np.int32)
+    # zero indexed
+    cell_offset = np.empty((0,), dtype='uint8')  # np.zeros((Ncells,1),dtype=uint8)
+    cell_type = np.empty((0,), dtype='uint8')    # np.zeros((Ncells,1),dtype=uint8)
 
     cdata_all = None
     cvdata_all = None
     for key in cells:
         # non-Poly data
         sz = cells[key].shape[0]
         offset = cells[key].shape[1]
```

### Comparing `pyamg-4.2.2/pyamg.egg-info/PKG-INFO` & `pyamg-4.2.3/pyamg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamg
-Version: 4.2.2
+Version: 4.2.3
 Summary: PyAMG: Algebraic Multigrid Solvers in Python
 Home-page: https://github.com/pyamg/pyamg
 Download-URL: https://github.com/pyamg/pyamg/releases
 Author: Nathan Bell, Luke Olson, and Jacob Schroder
 Author-email: luke.olson@gmail.com
 Maintainer: Luke Olson
 Maintainer-email: luke.olson@gmail.com
@@ -60,15 +60,15 @@
 conda install pyamg
 ```
 
 # Introduction
 
 PyAMG is a library of **Algebraic Multigrid (AMG)** solvers with a convenient Python interface.
 
-![](./Docs/logo/pyamg_logo_withtext.png)
+![](https://raw.githubusercontent.com/pyamg/pyamg/main/docs/logo/pyamg_logo_withtext.png)
 
 PyAMG is currently developed by [Luke Olson](http://lukeo.cs.illinois.edu), and [Jacob Schroder](http://people.llnl.gov/schroder2).
 
 # Citing
 
 <pre>
 @MISC{OlSc2018,
@@ -78,19 +78,30 @@
       url = "https://github.com/pyamg/pyamg",
       note = "Release 4.0"
       }
 </pre>
 
 # Getting Help
 
-For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
+- For documentation see [http://pyamg.readthedocs.io/en/latest/](http://pyamg.readthedocs.io/en/latest/).
 
-Create an [issue](https://github.com/pyamg/pyamg/issues).
+- Create an [issue](https://github.com/pyamg/pyamg/issues).
 
-Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [Examples](https://github.com/pyamg/pyamg/wiki/Examples) (for instance  the [0STARTHERE](https://github.com/pyamg/pyamg-examples/blob/master/0STARTHERE/demo.py) example).
+- Look at the [Tutorial](https://github.com/pyamg/pyamg/wiki/Tutorial) or the [examples](https://github.com/pyamg/pyamg-examples) (for instance  the [0_start_here](https://github.com/pyamg/pyamg-examples/blob/main/0_start_here/demo.py) example).
+
+- Run the unit tests (`pip install pytest`):
+  - With PyAMG installed and from a non-source directory:
+  ```python
+  import pyamg
+  pyamg.test()
+  ```
+  - From the PyAMG source directory and installed (e.g. with `pip install -e .`):
+  ```python
+  pytest .
+  ```
 
 # What is AMG?
 
  AMG is a multilevel technique for solving large-scale linear systems with optimal or near-optimal efficiency.  Unlike geometric multigrid, AMG requires little or no geometric information about the underlying problem and develops a sequence of coarser grids directly from the input matrix.  This feature is especially important for problems discretized on unstructured meshes and irregular grids.
 
 # PyAMG Features
```

### Comparing `pyamg-4.2.2/pyamg.egg-info/SOURCES.txt` & `pyamg-4.2.3/pyamg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+.readthedocs.yml
+CITATION.cff
 CONTRIBUTING.md
 DEVELOPERS.txt
 LICENSE.txt
 MANIFEST.in
 README-DEV.md
 README.md
 changelog.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/ci.yml
+.github/workflows/draft-pdf.yml
 .github/workflows/lint.yml
 .github/workflows/wheels.yml
 bench/memory.py
 docs/Makefile
 docs/README.md
 docs/requirements.txt
 docs/dev/common_docstring.md
@@ -24,14 +27,21 @@
 docs/logo/pyamg_logo.pdf
 docs/logo/pyamg_logo.png
 docs/logo/pyamg_logo.py
 docs/logo/pyamg_logo_legacy.png
 docs/logo/pyamg_logo_legacy_withtext.png
 docs/logo/pyamg_logo_withtext.pdf
 docs/logo/pyamg_logo_withtext.png
+docs/paper/common.py
+docs/paper/example.pdf
+docs/paper/example.py
+docs/paper/example.res.txt
+docs/paper/example_plot.py
+docs/paper/paper.bib
+docs/paper/paper.md
 docs/source/README.md
 docs/source/conf.py
 docs/source/index.rst
 docs/source/ref.rst
 docs/source/_static/default.css
 pyamg/__init__.py
 pyamg/blackbox.py
```

### Comparing `pyamg-4.2.2/setup.cfg` & `pyamg-4.2.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 include_package_data = False
 packages = find:
 platforms = any
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.7.0
 	scipy>=0.12.0
+tests_require = 
 	pytest>=2
 
 [options.packages.find]
 exclude = 
 	docs
 	README-DEV.md
```

### Comparing `pyamg-4.2.2/setup.py` & `pyamg-4.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
-"""
-PyAMG: Algebraic Multigrid Solvers in Python
+"""PyAMG: Algebraic Multigrid Solvers in Python.
 
 PyAMG is a library of Algebraic Multigrid (AMG)
 solvers with a convenient Python interface.
 
 PyAMG features implementations of:
 
 - Ruge-Stuben (RS) or Classical AMG
```

