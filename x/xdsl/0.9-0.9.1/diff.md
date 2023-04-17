# Comparing `tmp/xdsl-0.9.tar.gz` & `tmp/xdsl-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdsl-0.9.tar", last modified: Wed Feb  1 11:18:24 2023, max compression
+gzip compressed data, was "xdsl-0.9.1.tar", last modified: Tue Feb  7 22:56:37 2023, max compression
```

## Comparing `xdsl-0.9.tar` & `xdsl-0.9.1.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-02-01 11:18:14.000000 xdsl-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-01 11:18:14.000000 xdsl-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-02-01 11:18:24.463516 xdsl-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-01 11:18:14.000000 xdsl-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-01 11:18:14.000000 xdsl-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-01 11:18:14.000000 xdsl-0.9/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-01 11:18:14.000000 xdsl-0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-01 11:18:24.463516 xdsl-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-01 11:18:14.000000 xdsl-0.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68933 2023-02-01 11:18:14.000000 xdsl-0.9/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.467516 xdsl-0.9/xdsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-01 11:18:24.467516 xdsl-0.9/xdsl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/xdsl/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/arith.py
--rw-r--r--   0 runner    (1001) docker     (123)    23415 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/cmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/irdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/llvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/memref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/dialects/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/xdsl/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/code_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/xdsl/frontend/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/dialects/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/op_inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/python_code_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/symref.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/frontend/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    39372 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    48950 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/irdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/irdl_mlir_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/mlir_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    70580 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/pattern_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/rewriter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/xdsl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/utils/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/utils/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-02-01 11:18:14.000000 xdsl-0.9/xdsl/xdsl_opt_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:18:24.463516 xdsl-0.9/xdsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-01 11:18:24.000000 xdsl-0.9/xdsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-02-07 22:56:27.000000 xdsl-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-07 22:56:27.000000 xdsl-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-07 22:56:37.580122 xdsl-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-07 22:56:27.000000 xdsl-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-07 22:56:27.000000 xdsl-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-07 22:56:27.000000 xdsl-0.9.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-07 22:56:27.000000 xdsl-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-07 22:56:37.580122 xdsl-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-07 22:56:27.000000 xdsl-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68933 2023-02-07 22:56:27.000000 xdsl-0.9.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/arith.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23961 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/cmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/irdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/llvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/memref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/dialects/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/frontend/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/dialects/arith.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/dialects/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/op_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/op_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/python_code_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/symref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/frontend/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39192 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51362 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/irdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/irdl_mlir_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/mlir_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72053 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/pattern_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23676 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/rewriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/tools/xdsl-opt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.580122 xdsl-0.9.1/xdsl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/utils/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/utils/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-02-07 22:56:27.000000 xdsl-0.9.1/xdsl/xdsl_opt_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:56:37.576122 xdsl-0.9.1/xdsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 22:56:37.000000 xdsl-0.9.1/xdsl.egg-info/top_level.txt
```

### Comparing `xdsl-0.9/LICENSE` & `xdsl-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/PKG-INFO` & `xdsl-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdsl
-Version: 0.9
+Version: 0.9.1
 Summary: xDSL
 Home-page: https://xdsl.dev/
 Author: Mathieu Fehr
 Author-email: mathieu.fehr@ed.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/xdslproject/xdsl
 Project-URL: Issue Tracker, https://github.com/xdslproject/xdsl/issues
```

### Comparing `xdsl-0.9/README.md` & `xdsl-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/setup.cfg` & `xdsl-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/setup.py` & `xdsl-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 setup(
     name="xdsl",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="xDSL",
     long_description=long_description,
     long_description_content_type='text/markdown',
+    scripts=['xdsl/tools/xdsl-opt'],
     project_urls={
         "Source Code": "https://github.com/xdslproject/xdsl",
         "Issue Tracker": "https://github.com/xdslproject/xdsl/issues",
     },
     url="https://xdsl.dev/",
     platforms=["Linux", "Mac OS-X", "Unix"],
     test_suite="pytest",
```

### Comparing `xdsl-0.9/versioneer.py` & `xdsl-0.9.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/__init__.py` & `xdsl-0.9.1/xdsl/__init__.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/affine.py` & `xdsl-0.9.1/xdsl/dialects/affine.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/arith.py` & `xdsl-0.9.1/xdsl/dialects/arith.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/builtin.py` & `xdsl-0.9.1/xdsl/dialects/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,14 +636,32 @@
                          shape: List[int] = []) -> DenseIntOrFPElementsAttr:
         t = AnyTensorType.from_type_and_list(
             typ, shape if len(shape) else [len(data)])
         return DenseIntOrFPElementsAttr.from_list(t, data)
 
 
 @irdl_attr_definition
+class DenseResourceAttr(ParametrizedAttribute):
+    name = "dense_resource"
+
+    resource_handle: ParameterDef[StringAttr]
+
+    # Should be a ShapedType, but this is not defined yet in xDSL
+    type: ParameterDef[Attribute]
+
+    @staticmethod
+    @builder
+    def from_params(handle: str | StringAttr,
+                    type: Attribute) -> DenseResourceAttr:
+        if isinstance(handle, str):
+            handle = StringAttr.from_str(handle)
+        return DenseResourceAttr([handle, type])
+
+
+@irdl_attr_definition
 class FunctionType(ParametrizedAttribute, MLIRType):
     name = "fun"
 
     inputs: ParameterDef[ArrayAttr[Attribute]]
     outputs: ParameterDef[ArrayAttr[Attribute]]
 
     @staticmethod
@@ -749,14 +767,15 @@
         FlatSymbolRefAttr,
         SymbolNameAttr,
         IntAttr,
         IntegerAttr,
         ArrayAttr,
         DictionaryAttr,
         DenseIntOrFPElementsAttr,
+        DenseResourceAttr,
         UnitAttr,
         FloatData,
         NoneAttr,
         OpaqueAttr,
 
         # Types
         FunctionType,
```

### Comparing `xdsl-0.9/xdsl/dialects/cf.py` & `xdsl-0.9.1/xdsl/dialects/cf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import Annotated, List, Union
 
 from xdsl.dialects.builtin import IntegerType
 from xdsl.ir import SSAValue, Operation, Block, Dialect
 from xdsl.irdl import (irdl_op_definition, VarOperand, AnyAttr, Operand,
                        AttrSizedOperandSegments)
```

### Comparing `xdsl-0.9/xdsl/dialects/cmath.py` & `xdsl-0.9.1/xdsl/dialects/cmath.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/func.py` & `xdsl-0.9.1/xdsl/dialects/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
     def verify_(self) -> None:
         # TODO: how to verify that there is a terminator?
         entry_block: Block = self.body.blocks[0]
         block_arg_types = [arg.typ for arg in entry_block.args]
         if self.function_type.inputs.data != block_arg_types:
             raise VerifyException(
-                "Expected entry block arguments to have the same types as the function input types"
-            )
+                "Expected entry block arguments to have the same types as the function "
+                "input types")
 
     @staticmethod
     def from_callable(name: str, input_types: List[Attribute],
                       return_types: List[Attribute],
                       func: Block.BlockCallback) -> FuncOp:
         type_attr = FunctionType.from_lists(input_types, return_types)
         attributes = {
```

### Comparing `xdsl-0.9/xdsl/dialects/irdl.py` & `xdsl-0.9.1/xdsl/dialects/irdl.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/llvm.py` & `xdsl-0.9.1/xdsl/dialects/llvm.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/memref.py` & `xdsl-0.9.1/xdsl/dialects/memref.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/scf.py` & `xdsl-0.9.1/xdsl/dialects/scf.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/dialects/vector.py` & `xdsl-0.9.1/xdsl/dialects/vector.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,8 +165,80 @@
                                 result_types=[
                                     VectorType.from_element_type_and_shape(
                                         SSAValue.get(memref).typ.element_type,
                                         [1])
                                 ])
 
 
-Vector = Dialect([Load, Store, Broadcast, FMA, Maskedload], [])
+@irdl_op_definition
+class Maskedstore(Operation):
+    name = "vector.maskedstore"
+    memref: Annotated[Operand, MemRefType]
+    indices: Annotated[VarOperand, IndexType]
+    mask: Annotated[Operand, VectorType]
+    value_to_store: Annotated[Operand, VectorType]
+
+    def verify_(self):
+        memref_element_type = self.memref.typ.element_type
+
+        if memref_element_type != self.value_to_store.typ.element_type:
+            raise VerifyException(
+                "MemRef element type should match the stored vector type. Obtained types were "
+                + str(memref_element_type) + " and " +
+                str(self.value_to_store.typ.element_type) + ".")
+
+        if len(self.value_to_store.typ.get_shape()) != 1:
+            raise VerifyException("Expected a rank 1 vector to be stored.")
+
+        if len(self.mask.typ.get_shape()) != 1:
+            raise VerifyException("Expected a rank 1 mask vector.")
+
+        if self.mask.typ.element_type != i1:
+            raise VerifyException("Expected mask element type to be i1.")
+
+        if self.memref.typ.get_num_dims() != len(self.indices):
+            raise VerifyException(
+                "Expected an index for each memref dimension.")
+
+    @staticmethod
+    def get(memref: SSAValue | Operation, indices: List[SSAValue | Operation],
+            mask: SSAValue | Operation,
+            value_to_store: SSAValue | Operation) -> Maskedstore:
+        return Maskedstore.build(
+            operands=[memref, indices, mask, value_to_store])
+
+
+@irdl_op_definition
+class Print(Operation):
+    name = "vector.print"
+    source: Annotated[Operand, AnyAttr()]
+
+    @staticmethod
+    def get(source: Operation | SSAValue) -> Print:
+        return Print.build(operands=[source])
+
+
+@irdl_op_definition
+class Createmask(Operation):
+    name = "vector.create_mask"
+    mask_operands: Annotated[VarOperand, IndexType]
+    mask_vector: Annotated[OpResult, VectorType]
+
+    def verify_(self):
+        if self.mask_vector.typ.element_type != i1:
+            raise VerifyException("Expected mask element type to be i1.")
+
+        if self.mask_vector.typ.get_num_dims() != len(self.mask_operands):
+            raise VerifyException(
+                "Expected an operand value for each dimension of resultant mask."
+            )
+
+    @staticmethod
+    def get(mask_operands: Operation | SSAValue) -> Createmask:
+        return Createmask.build(
+            operands=[mask_operands],
+            result_types=[VectorType.from_element_type_and_shape(i1, [1])])
+
+
+Vector = Dialect(
+    [Load, Store, Broadcast, FMA, Maskedload, Maskedstore, Print, Createmask],
+    [])
```

### Comparing `xdsl-0.9/xdsl/frontend/block.py` & `xdsl-0.9.1/xdsl/frontend/block.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/frontend/const.py` & `xdsl-0.9.1/xdsl/frontend/const.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/frontend/context.py` & `xdsl-0.9.1/xdsl/frontend/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Underlying frontend program which can be compiled and translated to
     xDSL/MLIR.
     """
 
     def __enter__(self) -> None:
         # First, get the Python AST from the code.
         frame = _getframe(1)
+        self.program.file = frame.f_code.co_filename
         src = getsource(frame)
         python_ast = ast.parse(src)
 
         # Get all the global information and record it as well. In particular,
         # this contains all the imports.
         self.program.globals = frame.f_globals
 
@@ -41,8 +42,8 @@
                 # execution.
                 self.program.stmts = node.body
 
     def __exit__(self, *args):
         # Having proccessed all the code in the context, check it is well-formed
         # and can be compiled/executed.
         assert self.program.stmts is not None
-        PythonCodeCheck.run(self.program.stmts)
+        PythonCodeCheck.run(self.program.stmts, self.program.file)
```

### Comparing `xdsl-0.9/xdsl/frontend/exception.py` & `xdsl-0.9.1/xdsl/frontend/exception.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,17 +20,29 @@
 @dataclass
 class CodeGenerationException(FrontendProgramException):
     """
     Exception type used when xDSL code generation fails. Should be used for
     user-facing errors, e.g. unsupported functionality or failed type checks.
     """
 
+    file: str
     line: int
     col: int
 
-    def __init__(self, line: int, col: int, msg: str):
+    def __init__(
+        self,
+        file: str,
+        line: int,
+        col: int,
+        msg: str,
+    ):
         super().__init__(msg)
+        self.file = file
         self.line = line
         self.col = col
 
     def __str__(self) -> str:
-        return f"Code generation exception at {self.line}:{self.col}. {self.msg}"
+        str = 'Code generation exception at '
+        if self.file:
+            return str + f'"{self.file}", line {self.line} column {self.col}: {self.msg}'
+        else:
+            return str + f'line {self.line} column {self.col}: {self.msg}'
```

### Comparing `xdsl-0.9/xdsl/frontend/op_inserter.py` & `xdsl-0.9.1/xdsl/frontend/op_inserter.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             raise FrontendProgramException(
                 f"Trying to set the insertion point for operation '{op.name}' with no regions."
             )
         if len(op.regions[-1].blocks) == 0:
             raise FrontendProgramException(
                 f"Trying to set the insertion point for operation '{op.name}' with no blocks in its last region."
             )
-        self.ip = op.regions[-1].blocks[-1]
+        self.insertion_point = op.regions[-1].blocks[-1]
 
     def set_insertion_point_from_region(self, region: Region) -> None:
         """Sets the insertion point to the last block in this region."""
         if len(region.blocks) == 0:
             raise FrontendProgramException(
                 "Trying to set the insertion point from the region without blocks."
             )
```

### Comparing `xdsl-0.9/xdsl/frontend/program.py` & `xdsl-0.9.1/xdsl/frontend/program.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
     globals: Dict[str, Any] | None = field(default=None)
     """Global information for this program, including all the imports."""
 
     xdsl_program: ModuleOp | None = field(default=None)
     """Generated xDSL program when AST is compiled."""
 
+    file: str | None = field(default=None)
+    """Path to the file that contains the program."""
+
     def _check_can_compile(self):
         if self.stmts is None or self.globals is None:
             msg = \
                 """
 Cannot compile program without the code context. Try to use:
     p = FrontendProgram()
     with CodeContext(p):
@@ -44,15 +47,15 @@
         # `CodeContext`.
         self._check_can_compile()
         assert self.globals is not None
         assert self.stmts is not None
 
         type_converter = TypeConverter(self.globals)
         self.xdsl_program = CodeGeneration.run_with_type_converter(
-            type_converter, self.stmts)
+            type_converter, self.stmts, self.file)
         self.xdsl_program.verify()
 
         # Optionally run desymrefication pass to produce actual SSA.
         if desymref:
             self.desymref()
 
     def desymref(self) -> None:
```

### Comparing `xdsl-0.9/xdsl/frontend/python_code_check.py` & `xdsl-0.9.1/xdsl/frontend/python_code_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from xdsl.frontend.exception import CodeGenerationException
 
 
 @dataclass
 class PythonCodeCheck:
 
     @staticmethod
-    def run(stmts: List[ast.stmt]) -> None:
+    def run(stmts: List[ast.stmt], file: str) -> None:
         """
         Checks if Python code within `CodeContext` is supported. On unsupported
         cases, an exception is raised. Particularly, the check is used for
         scoping because Python (as an interpreted language) does not have a
         notion of constants, global variables, etc. Hence, one can redefine
         functions, place variables in arbitrary locations and do many other
         weird things which xDSL/MLIR would not like.
@@ -41,111 +41,117 @@
         single_scope: bool = True
         for stmt in stmts:
             if isinstance(stmt, ast.FunctionDef) and not is_block(stmt):
                 single_scope = False
                 break
 
         # Check Python code is correctly structured.
-        CheckStructure.run_with_scope(single_scope, stmts)
+        CheckStructure.run_with_scope(single_scope, stmts, file)
 
         # Check constant/global variables are correctly defined. Should be
         # called only after the structure is checked.
-        CheckAndInlineConstants.run(stmts)
+        CheckAndInlineConstants.run(stmts, file)
 
 
 @dataclass
 class CheckStructure:
 
     @staticmethod
-    def run_with_scope(single_scope: bool, stmts: List[ast.stmt]) -> None:
+    def run_with_scope(single_scope: bool, stmts: List[ast.stmt],
+                       file: str) -> None:
         if single_scope:
-            visitor = SingleScopeVisitor()
+            visitor = SingleScopeVisitor(file)
         else:
-            visitor = MultipleScopeVisitor()
+            visitor = MultipleScopeVisitor(file)
         for stmt in stmts:
             visitor.visit(stmt)
 
 
 @dataclass
 class SingleScopeVisitor(ast.NodeVisitor):
 
+    file: str = field(default=None)
+    """File path for error reporting."""
+
     block_names: Set[str] = field(default_factory=set)
     """Tracks duplicate block labels."""
 
     def visit(self, node: ast.AST) -> None:
         super().visit(node)
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         assert is_block(node)
 
         if node.name in self.block_names:
             raise CodeGenerationException(
-                node.lineno, node.col_offset,
+                self.file, node.lineno, node.col_offset,
                 f"Block '{node.name}' is already defined.")
         self.block_names.add(node.name)
 
         for stmt in node.body:
             if isinstance(stmt, ast.FunctionDef):
                 if is_block(stmt):
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        self.file, stmt.lineno, stmt.col_offset,
                         f"Cannot have a nested block '{stmt.name}' inside the "
                         f"block '{node.name}'.")
                 else:
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        self.file, stmt.lineno, stmt.col_offset,
                         f"Cannot have an inner function '{stmt.name}' inside "
                         f"the block '{node.name}'.")
 
 
 @dataclass
 class MultipleScopeVisitor(ast.NodeVisitor):
 
+    file: str = field(default=None)
+
     function_and_block_names: Dict[str, Set[str]] = field(default_factory=dict)
     """Tracks duplicate function names and duplicate block labels."""
 
     def visit(self, node: ast.AST) -> None:
         super().visit(node)
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         assert not is_block(node)
 
         if node.name in self.function_and_block_names:
             raise CodeGenerationException(
-                node.lineno, node.col_offset,
+                self.file, node.lineno, node.col_offset,
                 f"Function '{node.name}' is already defined.")
         self.function_and_block_names[node.name] = set()
 
         # Functions cannot have inner functions but can have blocks inside
         # which we still have to check.
         for stmt in node.body:
             if isinstance(stmt, ast.FunctionDef):
                 if not is_block(stmt):
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        self.file, stmt.lineno, stmt.col_offset,
                         f"Cannot have an inner function '{stmt.name}' inside "
                         f"the function '{node.name}'.")
                 else:
                     if stmt.name in self.function_and_block_names[node.name]:
                         raise CodeGenerationException(
-                            stmt.lineno, stmt.col_offset,
+                            self.file, stmt.lineno, stmt.col_offset,
                             f"Block '{stmt.name}' is already defined in "
                             f"function '{node.name}'.")
                     self.function_and_block_names[node.name].add(stmt.name)
 
                     for inner in stmt.body:
                         if isinstance(inner, ast.FunctionDef):
                             if is_block(inner):
                                 raise CodeGenerationException(
-                                    inner.lineno, inner.col_offset,
+                                    self.file, inner.lineno, inner.col_offset,
                                     f"Cannot have a nested block '{inner.name}'"
                                     f" inside the block '{stmt.name}'.")
                             else:
                                 raise CodeGenerationException(
-                                    inner.lineno, inner.col_offset,
+                                    self.file, inner.lineno, inner.col_offset,
                                     f"Cannot have an inner function '{inner.name}'"
                                     f" inside the block '{stmt.name}'.")
 
 
 @dataclass
 class CheckAndInlineConstants:
     """
@@ -164,20 +170,20 @@
     ```
 
     Note that the algorithm does not remove constant definitions from the AST,
     but this functionality can be added later.
     """
 
     @staticmethod
-    def run(stmts: List[ast.stmt]) -> None:
-        CheckAndInlineConstants.run_with_variables(stmts, set())
+    def run(stmts: List[ast.stmt], file: str) -> None:
+        CheckAndInlineConstants.run_with_variables(stmts, set(), file)
 
     @staticmethod
-    def run_with_variables(stmts: List[ast.stmt],
-                           defined_variables: Set[str]) -> None:
+    def run_with_variables(stmts: List[ast.stmt], defined_variables: Set[str],
+                           file: str) -> None:
         for i, stmt in enumerate(stmts):
             # This variable (`a = ...`) can be redefined as a constant, and so
             # we have to keep track of these to raise an exception.
             if isinstance(stmt, ast.Assign) and len(
                     stmt.targets) == 1 and isinstance(stmt.targets[0],
                                                       ast.Name):
                 defined_variables.add(stmt.targets[0].id)
@@ -192,42 +198,42 @@
                 continue
 
             # This is a constant.
             if isinstance(stmt, ast.AnnAssign) and is_constant(
                     stmt.annotation):
                 if not isinstance(stmt.target, ast.Name):
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        file, stmt.lineno, stmt.col_offset,
                         f"All constant expressions have to be assigned to "
                         "'ast.Name' nodes.")
 
                 name = stmt.target.id
                 try:
                     value = eval(ast.unparse(stmt.value))
                 except Exception:
                     # TODO: This error message can be improved by matching exact
                     # exceptions returned by `eval` call.
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        file, stmt.lineno, stmt.col_offset,
                         f"Non-constant expression cannot be assigned to "
                         f"constant variable '{name}' or cannot be evaluated.")
 
                 # For now, support primitive types only and add a guard to abort
                 # in other cases.
                 if not isinstance(value, int) and not isinstance(value, float):
                     raise CodeGenerationException(
-                        stmt.lineno, stmt.col_offset,
+                        file, stmt.lineno, stmt.col_offset,
                         f"Constant '{name}' has evaluated type '{type(value)}' "
                         "which is not supported.")
 
                 # TODO: We should typecheck the value against the type. This can
                 # get tricky since ints can overflow, etc. For example, `a:
                 # Const[i16] = 100000000` should give an error.
                 new_node = ast.Constant(value)
-                inliner = ConstantInliner(name, new_node)
+                inliner = ConstantInliner(name, new_node, file)
                 for candidate in stmts[(i + 1):]:
                     inliner.visit(candidate)
 
                 # Ideally, we can prune this AST node now, but it is easier just
                 # to avoid it during code generation phase.
                 continue
 
@@ -235,15 +241,15 @@
             # the nested list of statements as well. Note that if we reached
             # this then all constants above `i` must have been already inlined.
             # Hence, it is sufficient to check the function body only.
             if isinstance(stmt, ast.FunctionDef):
                 new_defined_variables = set(
                     [arg.arg for arg in stmt.args.args])
                 CheckAndInlineConstants.run_with_variables(
-                    stmt.body, new_defined_variables)
+                    stmt.body, new_defined_variables, file)
 
 
 @dataclass
 class ConstantInliner(ast.NodeTransformer):
     """
     Given the name of a constant and a corresponding AST node, `ConstantInliner`
     traverses the AST and replaces the uses of the `name` with the node.
@@ -254,37 +260,40 @@
 
     name: str
     """The name of the constant to inline."""
 
     new_node: ast.Constant
     """New AST node to inline."""
 
+    file: str = field(default=None)
+    """Path to the file containing the program."""
+
     def visit_Assign(self, node: ast.Assign) -> ast.Assign:
         if len(node.targets) == 1 and isinstance(
                 node.targets[0], ast.Name) and node.targets[0].id == self.name:
             raise CodeGenerationException(
-                node.lineno, node.col_offset,
+                self.file, node.lineno, node.col_offset,
                 f"Constant '{self.name}' is already defined and cannot be "
                 "assigned to.")
         node.value = self.visit(node.value)
         return node
 
     def visit_AnnAssign(self, node: ast.AnnAssign) -> ast.AnnAssign:
         if isinstance(node.target, ast.Name) and node.target.id == self.name:
             raise CodeGenerationException(
-                node.lineno, node.col_offset,
+                self.file, node.lineno, node.col_offset,
                 f"Constant '{self.name}' is already defined.")
         node.value = self.visit(node.value)
         return node
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         for arg in node.args.args:
             if arg.arg == self.name:
                 raise CodeGenerationException(
-                    node.lineno, node.col_offset,
+                    self.file, node.lineno, node.col_offset,
                     f"Constant '{self.name}' is already defined and cannot be "
                     "used as a function/block argument name.")
         for stmt in node.body:
             self.visit(stmt)
         return node
 
     def visit_Name(self, node: ast.Name) -> ast.Name:
```

### Comparing `xdsl-0.9/xdsl/frontend/symref.py` & `xdsl-0.9.1/xdsl/frontend/symref.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/frontend/type_conversion.py` & `xdsl-0.9.1/xdsl/frontend/type_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
                                     Type[_FrontendType]] = field(
                                         default_factory=dict)
     """
     Map to lookup frontend types based on xDSL type. Useful if we want to see
     what overloaded Python operations does this xDSL type support.
     """
 
+    file: str = field(default=None)
+
     def __post_init__(self) -> None:
         # Cache index type because it is always used implicitly in loops and
         # many other IR constructs.
         self._cache_type(frontend_builtin._Index, xdsl_builtin.IndexType(),
                          "index")
 
     def _cache_type(self, frontend_type: Type[_FrontendType],
@@ -58,73 +60,73 @@
         type_name = type_hint.id
         if type_name in self.name_to_xdsl_type_map:
             return self.name_to_xdsl_type_map[type_name]
 
         # Otherwise, it must be some frontend type, and we can look up its class
         # using the imports.
         if type_name not in self.globals:
-            raise CodeGenerationException(type_hint.lineno,
+            raise CodeGenerationException(self.file, type_hint.lineno,
                                           type_hint.col_offset,
                                           f"Unknown type hint '{type_name}'.")
         type_class = self.globals[type_name]
 
         # First, type can be generic, e.g. `class _Integer(Generic[_W, _S])`.
         if isinstance(type_class, _GenericAlias):
             generic_type_arguments = type_class.__args__
             arguments_for_constructor = []
             for type_argument in generic_type_arguments:
 
                 # Convert Literal[...] to concrete values.
                 materialized_arguments = type_argument.__args__
                 if len(materialized_arguments) != 1:
                     raise CodeGenerationException(
-                        type_hint.lineno, type_hint.col_offset,
+                        self.file, type_hint.lineno, type_hint.col_offset,
                         f"Expected 1 type argument for generic type '{type_name}', got {len(materialized_arguments)} type arguments instead."
                     )
                 arguments_for_constructor.append(materialized_arguments[0])
                 continue
 
             # Finally, get the constructor of this type and build an xDSL type.
             if issubclass(type_class.__origin__, _FrontendType):
                 xdsl_type = type_class.to_xdsl()(*arguments_for_constructor)
                 self._cache_type(type_class.__origin__, xdsl_type, type_name)
                 return xdsl_type
 
             # If this is not a subclass of FrontendType, then abort.
             raise CodeGenerationException(
-                type_hint.lineno, type_hint.col_offset,
+                self.file, type_hint.lineno, type_hint.col_offset,
                 f"'{type_name}' is not a frontend type.")
 
         # Otherwise, type can be a simple non-generic frontend type, e.g. `class
         # _Index(FrontendType)`.
         if issubclass(type_class, _FrontendType):
             xdsl_type = type_class.to_xdsl()()
             self._cache_type(type_class, xdsl_type, type_name)
             return xdsl_type
 
         raise CodeGenerationException(
-            type_hint.lineno, type_hint.col_offset,
+            self.file, type_hint.lineno, type_hint.col_offset,
             f"Unknown type hint for type '{type_name}' inside 'ast.Name' expression."
         )
 
     def convert_type_hint(self, type_hint: ast.expr) -> Attribute:
         """Convertes a Python/frontend type given as AST expression into xDSL type."""
 
         # Type hint should always be provided if this function is called.
         assert type_hint is not None
 
         # TODO: Type hint can be a Subscript AST node, for example
         # `Foo[Literal[2]]``. Support this in the future patches.
         if isinstance(type_hint, ast.Subscript):
             raise CodeGenerationException(
-                type_hint.lineno, type_hint.col_offset,
+                self.file, type_hint.lineno, type_hint.col_offset,
                 f"Converting subscript type hints is not supported.")
 
         # Type hint can also be a TypeAlias. For example, one can define
         # `foo = Foo[Literal[2]]`. This case also handles standard Python types, like
         # int, float, etc.
         if isinstance(type_hint, ast.Name):
             return self._convert_name(type_hint)
 
         raise CodeGenerationException(
-            type_hint.lineno, type_hint.col_offset,
+            self.file, type_hint.lineno, type_hint.col_offset,
             f"Unknown type hint AST node '{type_hint}'.")
```

### Comparing `xdsl-0.9/xdsl/ir.py` & `xdsl-0.9.1/xdsl/ir.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
-
 import re
+import sys
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from frozenlist import FrozenList
 from io import StringIO
+from itertools import chain
 from typing import (TYPE_CHECKING, Any, Callable, Generic, Optional, Protocol,
                     Sequence, TypeVar, cast, Iterator, ClassVar)
-import sys
 
 # Used for cyclic dependencies in type hints
 if TYPE_CHECKING:
     from xdsl.parser import BaseParser
     from xdsl.printer import Printer
     from xdsl.irdl import OpDef, ParamAttrDef
 
@@ -109,16 +109,18 @@
 
     index: int
     """The index of the operand using the value in the operation."""
 
 
 @dataclass
 class SSAValue(ABC):
-    """A reference to an SSA variable.
-    An SSA variable is either an operation result, or a basic block argument."""
+    """
+    A reference to an SSA variable.
+    An SSA variable is either an operation result, or a basic block argument.
+    """
 
     typ: Attribute
     """Each SSA variable is associated to a type."""
 
     uses: set[Use] = field(init=False, default_factory=set, repr=False)
     """All uses of the value."""
 
@@ -360,15 +362,15 @@
 @dataclass
 class Operation(IRNode):
     """A generic operation. Operation definitions inherit this class."""
 
     name: str = field(default="", init=False)
     """The operation name. Should be a static member of the class"""
 
-    _operands: FrozenList[SSAValue] = field(default_factory=FrozenList)
+    _operands: tuple[SSAValue, ...] = field(default_factory=lambda: ())
     """The operation operands."""
 
     results: list[OpResult] = field(default_factory=list)
     """The results created by the operation."""
 
     successors: list[Block] = field(default_factory=list)
     """
@@ -395,27 +397,26 @@
             return p.parent
         return None
 
     def parent_block(self) -> Block | None:
         return self.parent
 
     @property
-    def operands(self) -> FrozenList[SSAValue]:
+    def operands(self) -> tuple[SSAValue, ...]:
         return self._operands
 
     @operands.setter
-    def operands(self, new: list[SSAValue] | FrozenList[SSAValue]):
+    def operands(self, new: list[SSAValue] | tuple[SSAValue, ...]):
         if isinstance(new, list):
-            new = FrozenList(new)
+            new = tuple(new)
         for idx, operand in enumerate(self._operands):
             operand.remove_use(Use(self, idx))
         for idx, operand in enumerate(new):
             operand.add_use(Use(self, idx))
         self._operands = new
-        self._operands.freeze()
 
     def __post_init__(self):
         assert (self.name != "")
         assert (isinstance(self.name, str))
 
     @staticmethod
     def with_result_types(
@@ -582,17 +583,17 @@
 
     def is_structurally_equivalent(
             self,
             other: IRNode,
             context: Optional[dict[IRNode, IRNode]] = None) -> bool:
         """
         Check if two operations are structurally equivalent.
-        The context is a mapping of IR nodes to IR nodes that are already known "
-        "to be equivalent. This enables checking whether the use dependencies and "
-        "successors are equivalent.
+        The context is a mapping of IR nodes to IR nodes that are already known
+        to be equivalent. This enables checking whether the use dependencies and
+        successors are equivalent.
         """
         if context is None:
             context = {}
         if not isinstance(other, Operation):
             return False
         if self.name != other.name:
             return False
@@ -638,15 +639,15 @@
 
 @dataclass()
 class Block(IRNode):
     """A sequence of operations"""
 
     declared_at: 'Span' | None = None
 
-    _args: FrozenList[BlockArgument] = field(default_factory=FrozenList,
+    _args: tuple[BlockArgument, ...] = field(default_factory=lambda: (),
                                              init=False)
     """The basic block arguments."""
 
     ops: list[Operation] = field(default_factory=list, init=False)
     """Ordered operations contained in the block."""
 
     parent: Region | None = field(default=None, init=False, repr=False)
@@ -661,37 +662,34 @@
     def parent_block(self) -> Block | None:
         return self.parent.parent.parent if self.parent and self.parent.parent else None
 
     def __repr__(self) -> str:
         return f"Block(_args={repr(self._args)}, num_ops={len(self.ops)})"
 
     @property
-    def args(self) -> FrozenList[BlockArgument]:
+    def args(self) -> tuple[BlockArgument, ...]:
         """Returns the block arguments."""
         return self._args
 
     @staticmethod
     def from_arg_types(arg_types: list[Attribute]) -> Block:
         b = Block()
-        b._args = FrozenList([
-            BlockArgument(typ, b, index) for index, typ in enumerate(arg_types)
-        ])
-        b._args.freeze()
+        b._args = tuple(
+            BlockArgument(typ, b, index)
+            for index, typ in enumerate(arg_types))
         return b
 
     @staticmethod
     def from_ops(ops: list[Operation],
                  arg_types: list[Attribute] | None = None):
         b = Block()
         if arg_types:
-            b._args = FrozenList([
+            b._args = tuple(
                 BlockArgument(typ, b, index)
-                for index, typ in enumerate(arg_types)
-            ])
-            b._args.freeze()
+                for index, typ in enumerate(arg_types))
         b.add_ops(ops)
         return b
 
     class BlockCallback(Protocol):
 
         def __call__(self, *args: BlockArgument) -> list[Operation]:
             ...
@@ -708,32 +706,31 @@
         Returns the new argument.
         """
         if index < 0 or index > len(self._args):
             raise Exception("Unexpected index")
         new_arg = BlockArgument(typ, self, index)
         for arg in self._args[index:]:
             arg.index += 1
-        self._args = FrozenList(
-            list(self._args[:index]) + [new_arg] + list(self._args[index:]))
-        self._args.freeze()
+        self._args = tuple(
+            chain(self._args[:index], [new_arg], self._args[index:]))
         return new_arg
 
     def erase_arg(self, arg: BlockArgument, safe_erase: bool = True) -> None:
         """
         Erase a block argument.
         If safe_erase is True, check that the block argument is not used.
         If safe_erase is False, replace the block argument uses with an ErasedSSAVAlue.
         """
         if arg.block is not self:
             raise Exception(
                 "Attempting to delete an argument of the wrong block")
         for block_arg in self._args[arg.index + 1:]:
             block_arg.index -= 1
-        self._args = FrozenList(
-            list(self._args[:arg.index]) + list(self._args[arg.index + 1:]))
+        self._args = tuple(
+            chain(self._args[:arg.index], self._args[arg.index + 1:]))
         arg.erase(safe_erase=safe_erase)
 
     def _attach_op(self, operation: Operation) -> None:
         """Attach an operation to the block, and check that it has no parents."""
         if operation.parent:
             raise ValueError(
                 "Can't add to a block an operation already attached to a block."
@@ -851,17 +848,17 @@
 
     def is_structurally_equivalent(
             self,
             other: IRNode,
             context: Optional[dict[IRNode, IRNode]] = None) -> bool:
         """
         Check if two blocks are structurally equivalent.
-        The context is a mapping of IR nodes to IR nodes that are already known "
-        "to be equivalent. This enables checking whether the use dependencies and "
-        "successors are equivalent.
+        The context is a mapping of IR nodes to IR nodes that are already known
+        to be equivalent. This enables checking whether the use dependencies and
+        successors are equivalent.
         """
         if context is None:
             context = {}
         if not isinstance(other, Block):
             return False
         if len(self.args) != len(other.args) or \
            len(self.ops) != len(other.ops):
@@ -1087,17 +1084,17 @@
 
     def is_structurally_equivalent(
             self,
             other: IRNode,
             context: Optional[dict[IRNode, IRNode]] = None) -> bool:
         """
         Check if two regions are structurally equivalent.
-        The context is a mapping of IR nodes to IR nodes that are already known "
-        "to be equivalent. This enables checking whether the use dependencies and "
-        "successors are equivalent.
+        The context is a mapping of IR nodes to IR nodes that are already known
+        to be equivalent. This enables checking whether the use dependencies and
+        successors are equivalent.
         """
         if context is None:
             context = {}
         if not isinstance(other, Region):
             return False
         if len(self.blocks) != len(other.blocks):
             return False
```

### Comparing `xdsl-0.9/xdsl/irdl.py` & `xdsl-0.9.1/xdsl/irdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
-from frozenlist import FrozenList
 from functools import reduce
 from inspect import isclass
 from typing import (Annotated, Any, Callable, Generic, Sequence, TypeAlias,
                     TypeVar, Union, cast, get_args, get_origin, get_type_hints)
-from types import UnionType, GenericAlias
+from types import UnionType, GenericAlias, FunctionType
 
 from xdsl.ir import (Attribute, Block, Data, OpResult, Operation,
                      ParametrizedAttribute, Region, SSAValue)
 from xdsl.utils.diagnostic import Diagnostic
-from xdsl.utils.exceptions import BuilderNotFoundException, VerifyException
-from xdsl.utils.hints import is_satisfying_hint
+from xdsl.utils.exceptions import (BuilderNotFoundException,
+                                   PyRDLAttrDefinitionError,
+                                   PyRDLOpDefinitionError, VerifyException)
+from xdsl.utils.hints import is_satisfying_hint, PropertyType
 
 # pyright: reportMissingParameterType=false, reportUnknownParameterType=false
 
 
 def error(op: Operation, msg: str):
     diag = Diagnostic()
     diag.add_message(op, msg)
@@ -489,23 +490,53 @@
         """Decorator used on classes to define a new operation definition."""
 
         # Get all fields of the class, including the parent classes
         clsdict: dict[str, Any] = dict()
         for parent_cls in pyrdl_def.mro()[::-1]:
             clsdict = {**clsdict, **parent_cls.__dict__}
 
+        type_hints = get_type_hints(pyrdl_def, include_extras=True)
+
+        # Get all fields of the Operation class, including their parents classes
+        opdict: dict[str, Any] = dict()
+        for parent_cls in Operation.mro()[::-1]:
+            opdict = {**opdict, **parent_cls.__dict__}
+
+        def wrong_field_exception(field_name: str) -> PyRDLOpDefinitionError:
+            raise PyRDLOpDefinitionError(
+                f"{field_name} is neither a function, or an "
+                "operand, result, region, or attribute definition. "
+                "Operands should be defined with type hints of "
+                "Annotated[Operand, <Constraint>], results with "
+                "Annotated[OpResult, <Constraint>], regions with "
+                "Region, and attributes with "
+                "OpAttr[<Constraint>]")
+
+        # Check that all fields of the operation definition are either already
+        # in Operation, or are class functions or methods.
+        for field_name, value in clsdict.items():
+            if field_name in opdict:
+                continue
+            if field_name == "irdl_options":
+                continue
+            if isinstance(
+                    value,
+                (FunctionType, PropertyType, classmethod, staticmethod)):
+                continue
+            raise wrong_field_exception(field_name)
+
         if "name" not in clsdict:
             raise Exception(
                 f"pyrdl operation definition '{pyrdl_def.__name__}' does not "
                 "define the operation name. The operation name is defined by "
                 "adding a 'name' field.")
 
         op_def = OpDef(clsdict["name"])
-        for field_name, field_type in get_type_hints(
-                pyrdl_def, include_extras=True).items():
+
+        for field_name, field_type in type_hints.items():
 
             if field_name in get_type_hints(Operation).keys():
                 continue
 
             # If the field type is an Annotated, separate the origin
             # from the arguments.
             # If the field type is not an Annotated, then the arguments should
@@ -597,14 +628,16 @@
             elif args[0] == OptRegion:
                 if (len(args) > 1
                         and args[1] == IRDLAnnotations.SingleBlockRegionAnnot):
                     op_def.regions.append(
                         (field_name, OptSingleBlockRegionDef()))
                 else:
                     op_def.regions.append((field_name, OptRegionDef()))
+            else:
+                raise wrong_field_exception(field_name)
 
         op_def.options = clsdict.get("irdl_options", [])
 
         return op_def
 
 
 class VarIRConstruct(Enum):
@@ -640,15 +673,15 @@
     if construct == VarIRConstruct.REGION:
         return op_def.regions
     assert False, "Unknown VarIRConstruct value"
 
 
 def get_op_constructs(
     op: Operation, construct: VarIRConstruct
-) -> FrozenList[SSAValue] | list[OpResult] | list[Region]:
+) -> tuple[SSAValue, ...] | list[OpResult] | list[Region]:
     """
         Get the list of arguments of the type in an operation.
         For example, if the argument type is an operand, get the list of
         operands.
         """
     if construct == VarIRConstruct.OPERAND:
         return op.operands
@@ -759,16 +792,16 @@
     # definition of the irdl operation.
     assert False, "Unexpected xDSL error while fetching variadic sizes"
 
 
 def get_operand_result_or_region(
     op: Operation, op_def: OpDef, arg_def_idx: int, previous_var_args: int,
     construct: VarIRConstruct
-) -> None | SSAValue | FrozenList[SSAValue] | list[OpResult] | Region | list[
-        Region]:
+) -> None | SSAValue | tuple[SSAValue,
+                             ...] | list[OpResult] | Region | list[Region]:
     """
     Get an operand, result, or region.
     In the case of a variadic definition, return a list of elements.
     :param op: The operation we want to get argument of.
     :param arg_def_idx: The index of the argument in the irdl definition.
     :param previous_var_args: The number of previous variadic definitions
            before this definition.
@@ -1207,18 +1240,18 @@
                                                  include_extras=True).items():
         if field_name == "name" or field_name == "parameters":
             continue
 
         origin = get_origin(field_type)
         args = get_args(field_type)
         if origin != Annotated or IRDLAnnotations.ParamDefAnnot not in args:
-            raise ValueError(
+            raise PyRDLAttrDefinitionError(
                 f"In attribute {cls.__name__} definition: Parameter " +
                 f"definition {field_name} should be defined with " +
-                f"type `ParameterDef`, got type {field_type}.")
+                f"type `ParameterDef[<Constraint>]`, got type {field_type}.")
 
         res.append((field_name, field_type))
     return res
 
 
 @dataclass
 class ParamAttrDef:
@@ -1229,14 +1262,33 @@
     @staticmethod
     def from_pyrdl(pyrdl_def: type[ParametrizedAttribute]) -> ParamAttrDef:
         # Get the fields from the class and its parents
         clsdict = dict[str, Any]()
         for parent_cls in pyrdl_def.mro()[::-1]:
             clsdict = {**clsdict, **parent_cls.__dict__}
 
+        # Get all fields of the ParametrizedAttribute class, including their
+        # parents classes
+        attrdict: dict[str, Any] = dict()
+        for parent_cls in ParametrizedAttribute.mro()[::-1]:
+            attrdict = {**attrdict, **parent_cls.__dict__}
+        attrdict = {**attrdict, **Generic.__dict__, **GenericData.__dict__}
+
+        # Check that all fields of the attribute definition are either already
+        # in ParametrizedAttribute, or are class functions or methods.
+        for field_name, value in clsdict.items():
+            if field_name in attrdict:
+                continue
+            if isinstance(
+                    value,
+                (FunctionType, PropertyType, classmethod, staticmethod)):
+                continue
+            raise PyRDLAttrDefinitionError(
+                f"{field_name} is not a parameter definition.")
+
         if "name" not in clsdict:
             raise Exception(
                 f"pyrdl attribute definition '{pyrdl_def.__name__}' does not "
                 "define the attribute name. The attribute name is defined by "
                 "adding a 'name' field.")
 
         name = clsdict["name"]
```

### Comparing `xdsl-0.9/xdsl/irdl_mlir_printer.py` & `xdsl-0.9.1/xdsl/irdl_mlir_printer.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/mlir_converter.py` & `xdsl-0.9.1/xdsl/mlir_converter.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/parser.py` & `xdsl-0.9.1/xdsl/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from enum import Enum
 from io import StringIO
 from typing import TypeVar, Iterable
 
 from xdsl.utils.exceptions import ParseError, MultipleSpansParseError
 from xdsl.dialects.memref import MemRefType, UnrankedMemrefType
 from xdsl.dialects.builtin import (
-    AnyTensorType, AnyVectorType, Float16Type, Float32Type, Float64Type,
-    FloatAttr, FunctionType, IndexType, IntegerType, Signedness, StringAttr,
-    IntegerAttr, ArrayAttr, TensorType, UnrankedTensorType, VectorType,
-    FlatSymbolRefAttr, DenseIntOrFPElementsAttr, UnregisteredOp, OpaqueAttr,
-    NoneAttr, ModuleOp, UnitAttr, i64)
+    AnyTensorType, AnyVectorType, DenseResourceAttr, Float16Type, Float32Type,
+    Float64Type, FloatAttr, FunctionType, IndexType, IntegerType, Signedness,
+    StringAttr, IntegerAttr, ArrayAttr, TensorType, UnrankedTensorType,
+    VectorType, FlatSymbolRefAttr, DenseIntOrFPElementsAttr, UnregisteredOp,
+    OpaqueAttr, NoneAttr, ModuleOp, UnitAttr, i64)
 from xdsl.ir import (SSAValue, Block, Callable, Attribute, Operation, Region,
                      BlockArgument, MLContext, ParametrizedAttribute, Data)
 
 
 @dataclass
 class BacktrackingHistory:
     """
@@ -662,18 +662,22 @@
                     "Originally declared here:",
                     [(self.blocks[block_id.text].declared_at, None)],
                     self.tokenizer.history,
                 )
             block = Block(block_id)
             self.blocks[block_id.text] = block
 
+        block_args: list[BlockArgument] = []
+
         for i, (name, type) in enumerate(args):
             arg = BlockArgument(type, block, i)
             self.ssaValues[name.text] = arg
-            block.args.append(arg)
+            block_args.append(arg)
+
+        block._args = tuple(block_args)  # type: ignore
 
         while (next_op := self.try_parse_operation()) is not None:
             block.add_op(next_op)
 
         return block
 
     def _parse_optional_block_label(
@@ -782,14 +786,25 @@
 
     def try_parse_bare_id(self) -> Span | None:
         return self.tokenizer.next_token_of_pattern(ParserCommons.bare_id)
 
     def try_parse_value_id(self) -> Span | None:
         return self.tokenizer.next_token_of_pattern(ParserCommons.value_id)
 
+    def try_parse_operand(self) -> SSAValue | None:
+        """Try to parse an operand with format `%<value-id>`."""
+        value_id = self.try_parse_value_id()
+        if value_id is None:
+            return None
+        return self.get_ssa_val(value_id)
+
+    def parse_operand(self, msg: str = "operand expected") -> SSAValue:
+        """Parse an operand with format `%<value-id>`."""
+        return self.expect(self.try_parse_operand, msg)
+
     def try_parse_suffix_id(self) -> Span | None:
         return self.tokenizer.next_token_of_pattern(ParserCommons.suffix_id)
 
     def try_parse_block_id(self) -> Span | None:
         return self.tokenizer.next_token_of_pattern(ParserCommons.block_id)
 
     def try_parse_boolean_literal(self) -> Span | None:
@@ -1200,15 +1215,16 @@
         return name, self.parse_attribute()
 
     @abstractmethod
     def parse_attribute(self) -> Attribute:
         """
         Parse attribute (either builtin or dialect)
 
-        This is different in xDSL and MLIR, so the actuall implementation is provided by the subclass
+        This is different in xDSL and MLIR, so the actuall implementation is
+        provided by the subclass
         """
         raise NotImplementedError()
 
     def try_parse_attribute(self) -> Attribute | None:
         with self.tokenizer.backtracking("attribute"):
             return self.parse_attribute()
 
@@ -1251,14 +1267,15 @@
         name = self.tokenizer.next_token(peek=True)
         with self.tokenizer.backtracking("Builtin attribute {}".format(
                 name.text)):
             self.tokenizer.consume_peeked(name)
             parsers = {
                 'dense': self._parse_builtin_dense_attr,
                 'opaque': self._parse_builtin_opaque_attr,
+                'dense_resource': self._parse_builtin_dense_resource_attr,
             }
 
             def not_implemented():
                 raise NotImplementedError()
 
             return parsers.get(name.text, not_implemented)()
 
@@ -1289,14 +1306,25 @@
             type = self.expect(self.try_parse_type,
                                "opaque attribute must be typed!")
 
         return OpaqueAttr.from_strings(*(span.string_contents
                                          for span in str_lit_list),
                                        type=type)
 
+    def _parse_builtin_dense_resource_attr(self) -> DenseResourceAttr:
+        err_msg = ("Malformed dense_resource attribute, format must be "
+                   "(`dense_resource` `<` resource-handle `>`)")
+        self.parse_characters("<", err_msg)
+        resource_handle = self.expect(self.try_parse_bare_id, err_msg)
+        self.parse_characters(">", err_msg)
+        self.parse_characters(":", err_msg)
+        type = self.expect(self.try_parse_type,
+                           "Dense resource attribute must be typed!")
+        return DenseResourceAttr.from_params(resource_handle.text, type)
+
     def _parse_builtin_dense_attr_args(self) -> Iterable[int | float]:
         """
         Dense attribute params must be:
 
         dense-attr-params           := float-literal | int-literal | list-of-dense-attrs-params
         list-of-dense-attrs-params  := `[` dense-attr-params (`,` dense-attr-params)* `]`
         """
@@ -1392,15 +1420,14 @@
         raise NotImplementedError()
 
     def _attr_dict_from_tuple_list(
             self, tuple_list: list[tuple[Span,
                                          Attribute]]) -> dict[str, Attribute]:
         """
         Convert a list of tuples (Span, Attribute) to a dictionary.
-
         This function converts the span to a string, trimming quotes from string literals
         """
 
         def span_to_str(span: Span) -> str:
             if isinstance(span, StringLiteral):
                 return span.string_contents
             return span.text
@@ -1443,16 +1470,16 @@
         Parses type-or-type-list-parens, which is used in function-type.
 
         type-or-type-list-parens ::= type | type-list-parens
         type-list-parens         ::= `(` `)` | `(` type-list-no-parens `)`
         type-list-no-parens      ::=  type (`,` type)*
         """
         if self.tokenizer.next_token_of_pattern("(") is not None:
-            args: list[Attribute] = self.parse_list_of(self.try_parse_type,
-                                                       "Expected type here!")
+            args: list[Attribute | None] = self.parse_list_of(
+                self.try_parse_type, "Expected type here!")
             self.parse_characters(")", "Unclosed function type argument list!")
         else:
             args = [self.try_parse_type()]
             if args[0] is None:
                 self.raise_error(
                     "Function type must either be single type or list of types in"
                     " parenthesis!")
@@ -1509,38 +1536,39 @@
                FunctionType | None]:
         """
         Must return a tuple consisting of:
             - a list of arguments to the operation
             - a list of successor names
             - the attributes attached to the OP
             - the regions of the op
-            - An optional function type. If not supplied, parse_op_result_list must return a second value
-              containing the types of the returned SSAValues
+            - An optional function type. If not supplied, `parse_op_result_list`
+              must return a second value containing the types of the returned SSAValues
 
         """
         raise NotImplementedError()
 
     @abstractmethod
     def _parse_op_args_list(self) -> list[Span]:
         raise NotImplementedError()
 
     # HERE STARTS A SOMEWHAT CURSED COMPATIBILITY LAYER:
-    # Since we don't want to rewrite all dialects currently, the new parser needs to expose the same
-    # Interface to the dialect definitions (to some extent). Here we implement that interface.
+    # Since we don't want to rewrite all dialects currently, the new parser needs
+    # to expose the same Interface to the dialect definitions (to some extent).
+    # Here we implement that interface.
 
     _OperationType = TypeVar("_OperationType", bound=Operation)
 
     def parse_op_with_default_format(
         self,
         op_type: type[_OperationType],
         result_types: list[Attribute],
     ) -> _OperationType:
         """
-        Compatibility wrapper so the new parser can be passed instead of the old one. Parses everything after the
-        operation name.
+        Compatibility wrapper so the new parser can be passed instead of the old one.
+        Parses everything after the operation name.
 
         This implicitly assumes XDSL format, and will fail on MLIR style operations
         """
         # TODO: remove this function and restructure custom op / irdl parsing
         assert isinstance(self, XDSLParser)
         args, successors, attributes, regions, _ = self._parse_operation_details(
         )
@@ -1633,14 +1661,20 @@
             if value is None:
                 self.raise_error(
                     "`#` must be followed by a valid dialect attribute or type!"
                 )
 
             return value
 
+        # In MLIR, a type can be parsed at any attribute location.
+        # While MLIR wraps the type in a `TypeAttr`, we do not require this
+        # in xDSL.
+        if (type := self.try_parse_type()) is not None:
+            return type
+
         # If it isn't a dialect attr, parse builtin
         builtin_val = self.try_parse_builtin_attr()
 
         if builtin_val is None:
             self.raise_error(
                 "Unknown attribute (neither builtin nor dialect could be parsed)!"
             )
```

### Comparing `xdsl-0.9/xdsl/pattern_rewriter.py` & `xdsl-0.9.1/xdsl/pattern_rewriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Any, Callable
+from typing import Callable, TypeVar
 
 from xdsl.dialects.builtin import ModuleOp
 from xdsl.ir import (Operation, Region, Block, BlockArgument, Attribute,
                      SSAValue)
 from xdsl.rewriter import Rewriter
 
 
@@ -314,37 +314,62 @@
 
 
 class RewritePattern(ABC):
     """
     A side-effect free rewrite pattern matching on a DAG.
     """
 
+    # The / in the function signature makes the previous arguments positional, see
+    # https://peps.python.org/pep-0570/
+    # This is used by the op_type_rewrite_pattern
     @abstractmethod
-    def match_and_rewrite(self, op: Operation, rewriter: PatternRewriter):
+    def match_and_rewrite(self, op: Operation, rewriter: PatternRewriter, /):
         """
         Match an operation, and optionally perform a rewrite using the rewriter.
         """
         ...
 
 
 @dataclass(eq=False, repr=False)
 class AnonymousRewritePattern(RewritePattern):
     """
     A rewrite pattern encoded by an anonymous function.
     """
-    func: Callable[[Operation, PatternRewriter], None]
+    func: Callable[[RewritePattern, Operation, PatternRewriter], None]
+
+    def __init__(
+        self,
+        func: Callable[[RewritePattern, Operation, PatternRewriter], None]
+        | Callable[[Operation, PatternRewriter], None]):
+        params = [
+            param for param in inspect.signature(func).parameters.values()
+        ]
+        if len(params) == 2:
+
+            def new_func(self: RewritePattern, op: Operation,
+                         rewriter: PatternRewriter):
+                func(op, rewriter)  # type: ignore
+
+            self.func = new_func
+        else:
+            self.func = func  # type: ignore
 
     def match_and_rewrite(self, op: Operation,
                           rewriter: PatternRewriter) -> None:
-        self.func(op, rewriter)
+        self.func(self, op, rewriter)
+
+
+_RewritePatternT = TypeVar("_RewritePatternT", bound=RewritePattern)
+_OperationT = TypeVar("_OperationT", bound=Operation)
 
 
 def op_type_rewrite_pattern(
-    func: Callable[..., None]
-) -> Callable[[Any, Any], None] | Callable[[Any, Any, Any], None]:
+    func: Callable[[_RewritePatternT, _OperationT, PatternRewriter], None]
+    | Callable[[_OperationT, PatternRewriter], None]
+) -> Callable[[_RewritePatternT, Operation, PatternRewriter], None]:
     """
     This function is intended to be used as a decorator on a RewritePatter method.
     It uses type hints to match on a specific operation type before calling the decorated
     function.
     """
     # Get the operation argument and check that it is a subclass of Operation
     params = [param for param in inspect.signature(func).parameters.values()]
@@ -359,39 +384,39 @@
                 "op_type_rewrite_pattern expects the decorated method to "
                 "have two non-self arguments.")
     else:
         if len(params) != 2:
             raise Exception(
                 "op_type_rewrite_pattern expects the decorated function to "
                 "have two arguments.")
-    expected_type = params[-2].annotation
+    expected_type: type[_OperationT] = params[-2].annotation
     if not issubclass(expected_type, Operation):
         raise Exception(
             "op_type_rewrite_pattern expects the first non-self argument"
             "type hint to be an Operation subclass")
 
     if not is_method:
 
         def op_type_rewrite_pattern_static_wrapper(
-                op: Operation, rewriter: PatternRewriter) -> None:
+                self: RewritePattern, op: Operation,
+                rewriter: PatternRewriter) -> None:
             if not isinstance(op, expected_type):
                 return None
-            func(op, rewriter)
+            func(op, rewriter)  # type: ignore
 
         return op_type_rewrite_pattern_static_wrapper
 
     def op_type_rewrite_pattern_method_wrapper(
-            self,  # type: ignore
-            op: Operation,
+            self: _RewritePatternT, op: Operation,
             rewriter: PatternRewriter) -> None:
         if not isinstance(op, expected_type):
             return None
-        func(self, op, rewriter)
+        func(self, op, rewriter)  # type: ignore
 
-    return op_type_rewrite_pattern_method_wrapper  # type: ignore
+    return op_type_rewrite_pattern_method_wrapper
 
 
 @dataclass(eq=False, repr=False)
 class GreedyRewritePatternApplier(RewritePattern):
     """
     Apply a list of patterns in order until one pattern matches,
     and then use this rewrite.
```

### Comparing `xdsl-0.9/xdsl/printer.py` & `xdsl-0.9.1/xdsl/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass, field
 from enum import Enum
-from frozenlist import FrozenList
 from typing import Iterable, TypeVar, Any, Dict, Optional, List, cast
 
 from xdsl.dialects.memref import AnyUnrankedMemrefType, MemRefType, UnrankedMemrefType
 from xdsl.ir import (BlockArgument, MLIRType, SSAValue, Block, Callable,
                      Attribute, Region, Operation, Data, ParametrizedAttribute)
 from xdsl.utils.diagnostic import Diagnostic
 from xdsl.dialects.builtin import (
     AnyIntegerAttr, AnyFloatAttr, AnyUnrankedTensorType, AnyVectorType,
-    DenseIntOrFPElementsAttr, Float16Type, Float32Type, Float64Type, FloatAttr,
-    IndexType, IntegerType, NoneAttr, OpaqueAttr, Signedness, StringAttr,
-    FlatSymbolRefAttr, IntegerAttr, ArrayAttr, IntAttr, TensorType, UnitAttr,
-    FunctionType, UnrankedTensorType, UnregisteredOp, VectorType,
-    DictionaryAttr)
+    DenseIntOrFPElementsAttr, DenseResourceAttr, Float16Type, Float32Type,
+    Float64Type, FloatAttr, IndexType, IntegerType, NoneAttr, OpaqueAttr,
+    Signedness, StringAttr, FlatSymbolRefAttr, IntegerAttr, ArrayAttr, IntAttr,
+    TensorType, UnitAttr, FunctionType, UnrankedTensorType, UnregisteredOp,
+    VectorType, DictionaryAttr)
 
 indentNumSpaces = 2
 
 
 @dataclass(eq=False, repr=False)
 class Printer:
 
@@ -55,15 +54,15 @@
             if isinstance(arg, Attribute):
                 self.print_attribute(arg)
                 continue
             if isinstance(arg, Region):
                 self.print_region(arg)
                 continue
             if isinstance(arg, Block):
-                self.print_block_name(arg)
+                self.print_block(arg)
                 continue
             if isinstance(arg, Operation):
                 self.print_op(arg)
                 continue
             text = str(arg)
             self.print_string(text)
 
@@ -222,15 +221,18 @@
 
     def print_block_name(self, block: Block) -> None:
         self.print("^")
         if block not in self._block_names:
             self._block_names[block] = self._get_new_valid_block_id()
         self.print(self._block_names[block])
 
-    def _print_named_block(self, block: Block) -> None:
+    def print_block(self, block: Block) -> None:
+        if not isinstance(block, Block):
+            raise TypeError('Expected a Block; got %s' % type(block).__name__)
+
         self.print_block_name(block)
         if len(block.args) > 0:
             self.print("(")
             self.print_list(block.args, self._print_block_arg)
             self.print(")")
         self.print(":")
         if len(block.ops) > 0:
@@ -242,43 +244,46 @@
         self.print("%")
         name = self._get_new_valid_name_id()
         self._ssa_values[arg] = name
         self.print("%s : " % name)
         self.print_attribute(arg.typ)
 
     def print_region(self, region: Region) -> None:
+        if not isinstance(region, Region):
+            raise TypeError('Expected a Region; got %s' %
+                            type(region).__name__)
         if len(region.blocks) == 0:
             self.print("{}")
             return
 
         if len(region.blocks) == 1 and len(region.blocks[0].args) == 0:
             self.print("{")
             self._print_ops(region.blocks[0].ops)
             self.print("}")
             return
 
         self.print("{")
         self._print_new_line()
         for block in region.blocks:
-            self._print_named_block(block)
+            self.print_block(block)
         self.print("}")
 
     def print_regions(self, regions: List[Region]) -> None:
         if len(regions) == 0:
             return
 
         if self.target == self.Target.MLIR:
             self.print(" (")
             self.print_list(regions, self.print_region)
             self.print(")")
         else:
             self.print(" ")
             self.print_list(regions, self.print_region, delimiter=" ")
 
-    def _print_operands(self, operands: FrozenList[SSAValue]) -> None:
+    def _print_operands(self, operands: tuple[SSAValue, ...]) -> None:
         if len(operands) == 0:
             self.print("()")
             return
 
         self.print("(")
         self._print_operand(operands[0])
         for operand in operands[1:]:
@@ -423,14 +428,21 @@
                 len(data)
             ]
             print_dense_list(data, shape)
             self.print("> : ")
             self.print(attribute.type)
             return
 
+        # Dense resources have an alias in MLIR, but not in xDSL
+        if isinstance(attribute, DenseResourceAttr):
+            handle = attribute.resource_handle.data
+            type = attribute.type
+            self.print(f"dense_resource<{handle}> : ", type)
+            return
+
         # vector types have an alias in MLIR, but not in xDSL
         if ((isinstance(attribute, VectorType)
              or isinstance(attribute, TensorType))
                 and self.target == self.Target.MLIR):
             attribute = cast(AnyVectorType, attribute)
             self.print(
                 "vector<" if isinstance(attribute, VectorType) else "tensor<")
@@ -582,14 +594,17 @@
                 self.print("(")
                 self.print_list(
                     op.results,
                     lambda result: self.print_attribute(result.typ))
                 self.print(")")
 
     def _print_op(self, op: Operation) -> None:
+        if not isinstance(op, Operation):
+            raise TypeError('Expected an Operation; got %s' %
+                            type(op).__name__)
         begin_op_pos = self._current_column
         self._print_results(op)
         if isinstance(op, UnregisteredOp):
             self.print(f'"{op.op_name.data}"')
         elif self.print_generic_format or self.target == self.Target.MLIR:
             self.print(f'"{op.name}"')
         else:
```

### Comparing `xdsl-0.9/xdsl/rewriter.py` & `xdsl-0.9.1/xdsl/rewriter.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl/utils/diagnostic.py` & `xdsl-0.9.1/xdsl/utils/diagnostic.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         from xdsl.printer import Printer
         f = StringIO()
         p = Printer(stream=f, diagnostic=self)
         toplevel = ir.get_toplevel_object()
         if isinstance(toplevel, Operation):
             p.print_op(toplevel)
         elif isinstance(toplevel, Block):
-            p._print_named_block(toplevel)  # type: ignore
+            p.print_block(toplevel)
         elif isinstance(toplevel, Region):
-            p._print_region(toplevel)  # type: ignore
+            # TOFIX: Is that ever used. Revisit the whole exception
+            p._print_region(toplevel)  # TOFIX #type: ignore
         else:
             assert "xDSL internal error: get_toplevel_object returned unknown construct"
 
         raise exception_type(message + "\n\n" + f.getvalue())
```

### Comparing `xdsl-0.9/xdsl/utils/exceptions.py` & `xdsl-0.9.1/xdsl/utils/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,26 @@
     pass
 
 
 class VerifyException(DiagnosticException):
     pass
 
 
+class PyRDLError(Exception):
+    pass
+
+
+class PyRDLOpDefinitionError(Exception):
+    pass
+
+
+class PyRDLAttrDefinitionError(Exception):
+    pass
+
+
 @dataclass
 class BuilderNotFoundException(Exception):
     """
     Exception raised when no builders are found for a given attribute type
     and a given tuple of arguments.
     """
     attribute: type[Attribute]
```

### Comparing `xdsl-0.9/xdsl/utils/hints.py` & `xdsl-0.9.1/xdsl/utils/hints.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,7 +41,18 @@
             is_satisfying_hint(arg, union_arg) for union_arg in get_args(hint))
 
     raise ValueError(f"is_satisfying_hint: unsupported type hint '{hint}'")
 
 
 annotated_type = type(Annotated[int, 0])
 """This is the type of an Annotated object."""
+
+
+class _Class:
+
+    @property
+    def property(self):
+        pass
+
+
+PropertyType = type(_Class.property)
+"""The type of a property method."""
```

### Comparing `xdsl-0.9/xdsl/xdsl_opt_main.py` & `xdsl-0.9.1/xdsl/xdsl_opt_main.py`

 * *Files identical despite different names*

### Comparing `xdsl-0.9/xdsl.egg-info/PKG-INFO` & `xdsl-0.9.1/xdsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdsl
-Version: 0.9
+Version: 0.9.1
 Summary: xDSL
 Home-page: https://xdsl.dev/
 Author: Mathieu Fehr
 Author-email: mathieu.fehr@ed.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/xdslproject/xdsl
 Project-URL: Issue Tracker, https://github.com/xdslproject/xdsl/issues
```

### Comparing `xdsl-0.9/xdsl.egg-info/SOURCES.txt` & `xdsl-0.9.1/xdsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,20 @@
 xdsl/frontend/__init__.py
 xdsl/frontend/block.py
 xdsl/frontend/code_generation.py
 xdsl/frontend/const.py
 xdsl/frontend/context.py
 xdsl/frontend/exception.py
 xdsl/frontend/op_inserter.py
+xdsl/frontend/op_resolver.py
 xdsl/frontend/program.py
 xdsl/frontend/python_code_check.py
 xdsl/frontend/symref.py
 xdsl/frontend/type_conversion.py
 xdsl/frontend/dialects/__init__.py
+xdsl/frontend/dialects/arith.py
 xdsl/frontend/dialects/builtin.py
+xdsl/tools/xdsl-opt
 xdsl/utils/__init__.py
 xdsl/utils/diagnostic.py
 xdsl/utils/exceptions.py
 xdsl/utils/hints.py
```

