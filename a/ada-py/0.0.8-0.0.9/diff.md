# Comparing `tmp/ada-py-0.0.8.tar.gz` & `tmp/ada-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/adapy/adapy/dist/tmpqwvtbfkd/ada-py-0.0.8.tar", last modified: Sun Apr 11 19:30:36 2021, max compression
+gzip compressed data, was "/home/runner/work/adapy/adapy/dist/tmpqcgagrt9/ada-py-0.0.9.tar", last modified: Fri Apr 16 12:31:23 2021, max compression
```

## Comparing `ada-py-0.0.8.tar` & `ada-py-0.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35164 2021-04-11 19:30:28.000000 ada-py-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-11 19:30:28.000000 ada-py-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6866 2021-04-11 19:30:36.182532 ada-py-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4562 2021-04-11 19:30:28.000000 ada-py-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-04-11 19:30:28.000000 ada-py-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2021-04-11 19:30:36.182532 ada-py-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.174532 ada-py-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.174532 ada-py-0.0.8/src/ada/
--rw-r--r--   0 runner    (1001) docker     (121)   168117 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.174532 ada-py-0.0.8/src/ada/base/
--rw-r--r--   0 runner    (1001) docker     (121)    11441 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32203 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/base/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.174532 ada-py-0.0.8/src/ada/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10007 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/bimserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/blender.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    28012 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/ifc_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    23625 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/ifc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    84019 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/
--rw-r--r--   0 runner    (1001) docker     (121)    71921 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    22754 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/abaqus/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/abaqus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4587 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/abaqus/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/abaqus/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)    45280 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/abaqus/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    58703 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/abaqus/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/calculix/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/calculix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/calculix/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/calculix/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)    14945 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/calculix/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/code_aster/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/code_aster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/code_aster/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)    14284 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/code_aster/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/io_meshio/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/io_meshio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/io_meshio/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/io_meshio/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14868 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/mesh/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/mesh/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/sesam/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/sesam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29246 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/sesam/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    13530 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/sesam/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/usfos/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/usfos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16972 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/usfos/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9381 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/fem/io/xdmf/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/xdmf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/xdmf/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/xdmf/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8231 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/io/xdmf/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/fem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/materials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.178532 ada-py-0.0.8/src/ada/materials/metals/
--rw-r--r--   0 runner    (1001) docker     (121)    14862 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/materials/metals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/src/ada/materials/polymers/
--rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/materials/polymers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17522 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/materials/polymers/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/materials/polymers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/src/ada/param_models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/param_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5021 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/param_models/basic_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/param_models/basic_structural_components.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/param_models/fem_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/src/ada/sections/
--rw-r--r--   0 runner    (1001) docker     (121)    22194 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/src/ada/sections/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    15308 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/sections/resources/ProfileDB.json
--rw-r--r--   0 runner    (1001) docker     (121)     9370 2021-04-11 19:30:28.000000 ada-py-0.0.8/src/ada/sections/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:30:36.182532 ada-py-0.0.8/src/ada_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6866 2021-04-11 19:30:36.000000 ada-py-0.0.8/src/ada_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2021-04-11 19:30:36.000000 ada-py-0.0.8/src/ada_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-11 19:30:36.000000 ada-py-0.0.8/src/ada_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-04-11 19:30:36.000000 ada-py-0.0.8/src/ada_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-11 19:30:36.000000 ada-py-0.0.8/src/ada_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35164 2021-04-16 12:31:15.000000 ada-py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-16 12:31:15.000000 ada-py-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7754 2021-04-16 12:31:23.430581 ada-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5306 2021-04-16 12:31:15.000000 ada-py-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-04-16 12:31:15.000000 ada-py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2021-04-16 12:31:23.430581 ada-py-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.422581 ada-py-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.422581 ada-py-0.0.9/src/ada/
+-rw-r--r--   0 runner    (1001) docker     (121)   168216 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.422581 ada-py-0.0.9/src/ada/base/
+-rw-r--r--   0 runner    (1001) docker     (121)    11443 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32203 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/base/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.422581 ada-py-0.0.9/src/ada/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     1687 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10007 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/bimserver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/blender.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27928 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/ifc_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23625 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/ifc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84019 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/
+-rw-r--r--   0 runner    (1001) docker     (121)    72561 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22754 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/abaqus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4587 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/abaqus/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4167 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/abaqus/execute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45280 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/abaqus/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58703 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/abaqus/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/calculix/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/calculix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/calculix/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3925 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/calculix/execute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14945 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/calculix/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/code_aster/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/code_aster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3360 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/code_aster/execute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14284 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/code_aster/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/io_meshio/
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/io_meshio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/io_meshio/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2832 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/io_meshio/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14868 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/mesh/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/mesh/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/sesam/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/sesam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29246 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/sesam/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15697 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/sesam/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/usfos/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/usfos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16972 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/usfos/writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9381 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/fem/io/xdmf/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/xdmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/xdmf/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/xdmf/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8231 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/io/xdmf/writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/fem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/materials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.426581 ada-py-0.0.9/src/ada/materials/metals/
+-rw-r--r--   0 runner    (1001) docker     (121)    14862 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/materials/metals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/src/ada/materials/polymers/
+-rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/materials/polymers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17522 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/materials/polymers/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/materials/polymers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/src/ada/param_models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/param_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5021 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/param_models/basic_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/param_models/basic_structural_components.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/param_models/fem_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/src/ada/sections/
+-rw-r--r--   0 runner    (1001) docker     (121)    22585 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/src/ada/sections/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)    15308 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/sections/resources/ProfileDB.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9370 2021-04-16 12:31:15.000000 ada-py-0.0.9/src/ada/sections/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 12:31:23.430581 ada-py-0.0.9/src/ada_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7754 2021-04-16 12:31:23.000000 ada-py-0.0.9/src/ada_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1999 2021-04-16 12:31:23.000000 ada-py-0.0.9/src/ada_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-16 12:31:23.000000 ada-py-0.0.9/src/ada_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-04-16 12:31:23.000000 ada-py-0.0.9/src/ada_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-16 12:31:23.000000 ada-py-0.0.9/src/ada_py.egg-info/top_level.txt
```

### Comparing `ada-py-0.0.8/LICENSE` & `ada-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/PKG-INFO` & `ada-py-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ada-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Assembly for Design & Analysis - A toolkit for structural analysis and design
 Home-page: https://github.com/krande/adapy
 Author: Kristoffer H. Andersen
 Author-email: kristoffer_andersen@outlook.com
 License: GNU GPLv3
 Project-URL: Code, https://github.com/krande/adapy
 Project-URL: Issues, https://github.com/krande/adapy/issues
 Description: # ADA - Assembly for Design & Analysis
         
-        A toolkit for structural analysis and design that focus on interoperability between
+        A python library for structural analysis and design that focus on interoperability between
         IFC and various Finite Element formats.
         
         This library is still undergoing significant development so expect there to be occasional bugs and breaking changes.
         
         Try the latest build online here
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Krande/adapy/main)
@@ -87,31 +87,50 @@
         
         a = beam_ex1()
         
         a.to_fem("MyCantilever_abaqus", "abaqus", overwrite=True, execute=True, run_ext=True)
         a.to_fem("MyCantilever_calculix", "calculix", overwrite=True, execute=True)
         ```
         
-        after the execution is finished you can look at the results
+        after the execution is finished you can look at the results (in Paraview or Abaqus CAE for the results from 
+        calculix and/or abaqus respectively)
+        
         
         ![Paraview Results](docs/_static/figures/fem_beam_paraview.png)
         ![Abaqus Results](docs/_static/figures/fem_beam_abaqus.png)
         
+        or if your prefer to keep it in python here is a way you can use meshio to read the results from calculix and do your
+        postprocessing using python only.
+        
+        ```python
+        from ada.config import Settings
+        import meshio
+        
+        vtu = Settings.scratch_dir / "MyCantilever_calculix" / "MyCantilever_calculix.vtu"
+        mesh = meshio.read(vtu)
+        
+        # Von Mises stresses and displacement at a point @ index=0
+        print(mesh.point_data['S'][0])
+        print(mesh.point_data['U'][0])
+        ```
+        
+        In short `beam_ex1` creates a `Beam` object which it uses to create a shell element `FEM` mesh using 
+        a mesh recipe [create_beam_mesh](https://github.com/Krande/adapy/blob/c594ccbfbdd2ea9384fa8a4721a65580331b4a09/src/ada/fem/io/mesh/recipes.py#L99-L223). 
+        The recipe uses [GMSH](https://gmsh.info/) to construct elements on nodes. 
         
-        In short `beam_ex1` creates a `Beam` object which it uses to create a FEM mesh comprised of shell elements using GMSH. 
         
         The current reasoning is to work with a base representation of beam/plates and have the ability
         to easily create a FEM representation of any of the base objects in 1D (beam elements), 
         2D (shell elements) or 3D (elements) using your own meshing recipes (i.e. not just build a mesh, but a recipe for 
         building meshes).
         
         
         **Note!**
         
-        This example assumes you have installed Abaqus and Calculix locally on your computer.
+        The above example assumes you have installed Abaqus and Calculix locally on your computer.
         
         To set correct paths to your installations of Abaqus or Calculix you wish to use there are a few ways of doing so.
         
         1. Add directory path of abaqus.bat or ccx.exe to your system path.
         2. Add directory paths to system environment variables. This can be done by using the control panel or running the following from a cmd prompt with administrator rights:
             
         ```cmd
@@ -145,15 +164,14 @@
         For developers interested in contributing to this project feel free to make a fork, experiment and create a pull request
         when you have something you would like to add/change/remove. 
         
         Before making a pull request you need to lint with, isort, flake8 and black 
         
         ````
         pip install black isort flake8
-        cd src/ada
         isort .
         flake8 .
         black .
         ````
         
         
         ## Project Responsible ###
```

### Comparing `ada-py-0.0.8/README.md` & `ada-py-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ADA - Assembly for Design & Analysis
 
-A toolkit for structural analysis and design that focus on interoperability between
+A python library for structural analysis and design that focus on interoperability between
 IFC and various Finite Element formats.
 
 This library is still undergoing significant development so expect there to be occasional bugs and breaking changes.
 
 Try the latest build online here
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Krande/adapy/main)
@@ -77,31 +77,50 @@
 
 a = beam_ex1()
 
 a.to_fem("MyCantilever_abaqus", "abaqus", overwrite=True, execute=True, run_ext=True)
 a.to_fem("MyCantilever_calculix", "calculix", overwrite=True, execute=True)
 ```
 
-after the execution is finished you can look at the results
+after the execution is finished you can look at the results (in Paraview or Abaqus CAE for the results from 
+calculix and/or abaqus respectively)
+
 
 ![Paraview Results](docs/_static/figures/fem_beam_paraview.png)
 ![Abaqus Results](docs/_static/figures/fem_beam_abaqus.png)
 
+or if your prefer to keep it in python here is a way you can use meshio to read the results from calculix and do your
+postprocessing using python only.
+
+```python
+from ada.config import Settings
+import meshio
+
+vtu = Settings.scratch_dir / "MyCantilever_calculix" / "MyCantilever_calculix.vtu"
+mesh = meshio.read(vtu)
+
+# Von Mises stresses and displacement at a point @ index=0
+print(mesh.point_data['S'][0])
+print(mesh.point_data['U'][0])
+```
+
+In short `beam_ex1` creates a `Beam` object which it uses to create a shell element `FEM` mesh using 
+a mesh recipe [create_beam_mesh](https://github.com/Krande/adapy/blob/c594ccbfbdd2ea9384fa8a4721a65580331b4a09/src/ada/fem/io/mesh/recipes.py#L99-L223). 
+The recipe uses [GMSH](https://gmsh.info/) to construct elements on nodes. 
 
-In short `beam_ex1` creates a `Beam` object which it uses to create a FEM mesh comprised of shell elements using GMSH. 
 
 The current reasoning is to work with a base representation of beam/plates and have the ability
 to easily create a FEM representation of any of the base objects in 1D (beam elements), 
 2D (shell elements) or 3D (elements) using your own meshing recipes (i.e. not just build a mesh, but a recipe for 
 building meshes).
 
 
 **Note!**
 
-This example assumes you have installed Abaqus and Calculix locally on your computer.
+The above example assumes you have installed Abaqus and Calculix locally on your computer.
 
 To set correct paths to your installations of Abaqus or Calculix you wish to use there are a few ways of doing so.
 
 1. Add directory path of abaqus.bat or ccx.exe to your system path.
 2. Add directory paths to system environment variables. This can be done by using the control panel or running the following from a cmd prompt with administrator rights:
     
 ```cmd
@@ -135,15 +154,14 @@
 For developers interested in contributing to this project feel free to make a fork, experiment and create a pull request
 when you have something you would like to add/change/remove. 
 
 Before making a pull request you need to lint with, isort, flake8 and black 
 
 ````
 pip install black isort flake8
-cd src/ada
 isort .
 flake8 .
 black .
 ````
 
 
 ## Project Responsible ###
```

### Comparing `ada-py-0.0.8/setup.cfg` & `ada-py-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ada-py
-version = 0.0.8
+version = 0.0.9
 author = Kristoffer H. Andersen
 author_email = kristoffer_andersen@outlook.com
 description = Assembly for Design & Analysis - A toolkit for structural analysis and design
 url = https://github.com/krande/adapy
 project_urls = 
 	Code=https://github.com/krande/adapy
 	Issues=https://github.com/krande/adapy/issues
```

### Comparing `ada-py-0.0.8/src/ada/__init__.py` & `ada-py-0.0.9/src/ada/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,26 +346,26 @@
             self.add_pipe(pipe)
 
         all_walls = [wall for p in a.get_all_subparts() for wall in p.walls] + a.walls
         for wall in all_walls:
             self.add_wall(wall)
 
     def read_step_file(
-        self, cad_ref, name=None, scale=None, transform=None, rotate=None, colour=None, opacity=1.0, units="m"
+        self, step_path, name=None, scale=None, transform=None, rotate=None, colour=None, opacity=1.0, units="m"
     ):
         """
 
-        :param cad_ref:
-        :param name:
-        :param scale:
-        :param transform:
-        :param rotate:
-        :param colour:
-        :param opacity:
-        :return:
+        :param step_path: Can be path to stp file or path to directory of step files.
+        :param name: Desired name of destination Shape object
+        :param scale: Scale the step content upon import
+        :param transform: Transform the step content upon import
+        :param rotate: Rotate step content upon import
+        :param colour: Assign a specific colour upon import
+        :param opacity: Assign Opacity upon import
+        :param units: Unit of the imported STEP file. Default is 'm'
         """
         import math
 
         from OCC.Core.BRepBuilderAPI import BRepBuilderAPI_Transform
         from OCC.Core.gp import gp_Ax1, gp_Dir, gp_Pnt, gp_Trsf, gp_Vec
         from OCC.Extend.DataExchange import read_step_file
         from OCC.Extend.TopologyUtils import TopologyExplorer
@@ -393,26 +393,22 @@
             s = []
             t = TopologyExplorer(shp_)
             for solid in t.solids():
                 s.append(solid)
             return s
 
         shapes = []
-        if type(cad_ref) is str and ".stp" in cad_ref:
-            cad_file_path = pathlib.Path(cad_ref)
-            if cad_file_path.is_file():
-                shapes += extract_subshapes(read_step_file(str(cad_file_path)))
-            elif cad_file_path.is_dir():
-                shapes += walk_shapes(cad_file_path)
-            else:
-                raise Exception(
-                    'step_ref "{}" does not represent neither file or folder found on system'.format(cad_ref)
-                )
+
+        cad_file_path = pathlib.Path(step_path)
+        if cad_file_path.is_file():
+            shapes += extract_subshapes(read_step_file(str(cad_file_path)))
+        elif cad_file_path.is_dir():
+            shapes += walk_shapes(cad_file_path)
         else:
-            raise Exception('step_ref type "{}" is not recognized'.format(type(cad_ref)))
+            raise Exception(f'step_ref "{step_path}" does not represent neither file or folder found on system')
 
         shapes = [transform_shape(s) for s in shapes]
         if len(shapes) > 0:
             ada_name = name if name is not None else "CAD" + str(len(self.shapes) + 1)
             for i, shp in enumerate(shapes):
                 ada_shape = Shape(ada_name + "_" + str(i), shp, colour, opacity, units=units)
                 self.add_shape(ada_shape)
```

### Comparing `ada-py-0.0.8/src/ada/base/__init__.py` & `ada-py-0.0.9/src/ada/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
         if _Settings.convert_bad_names:
             logging.debug("Converting bad name")
-            value = value.replace("/", "").replace("=", "")
+            value = value.replace("/", "_").replace("=", "")
             if str.isnumeric(value[0]):
-                value = "ADA" + value
+                value = "ADA_" + value
 
         if "/" in value:
             logging.debug(f'Character "/" found in {value}')
 
         self._name = value.strip()
 
     @property
```

### Comparing `ada-py-0.0.8/src/ada/base/renderer.py` & `ada-py-0.0.9/src/ada/base/renderer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/config/__init__.py` & `ada-py-0.0.9/src/ada/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/core/bimserver.py` & `ada-py-0.0.9/src/ada/core/bimserver.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/core/blender.py` & `ada-py-0.0.9/src/ada/core/blender.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/core/containers.py` & `ada-py-0.0.9/src/ada/core/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,20 +402,17 @@
 
         s, t = i_check(A, C, AB, CD)
 
         AB_ = A + s * AB
         CD_ = C + t * CD
 
         t_ = roundoff(t)
-        if 0 <= t_ <= 1:
-            if t_ == 0 or t_ == 1:
-                pass
-            else:
-                logging.debug(f"Beam cross-check indicates that the beams {bm1} and {bm2} are most probably parallel")
-                return None
+        if 0 < t_ < 1:
+            logging.debug(f"Beam cross-check indicates that the beams {bm1} and {bm2} are most probably parallel")
+            return None
 
         if p_check(AB, CD):
             logging.debug(f"beams {bm1} {bm2} are parallel")
             return None
 
         if v_len(AB_ - CD_) > outofplane_tol:
             return None
```

### Comparing `ada-py-0.0.8/src/ada/core/ifc_template.py` & `ada-py-0.0.9/src/ada/core/ifc_template.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/core/ifc_utils.py` & `ada-py-0.0.9/src/ada/core/ifc_utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/core/utils.py` & `ada-py-0.0.9/src/ada/core/utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/__init__.py` & `ada-py-0.0.9/src/ada/fem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import numpy as np
 
 from . import constants as co
 from .containers import FemElements, FemSections, FemSets
 
 __all__ = [
     "Amplitude",
@@ -2085,26 +2087,28 @@
     def amplitude_name(self):
         return self._amplitude_name
 
 
 class Mass(FemBase):
     """
 
-    :param name:
-    :param fem_set:
-    :param mass:
-    :param mass_type:
-    :param ptype:
+    :param name: Name of set
+    :param fem_set: Fem Set (of element or nodal type)
+    :type fem_set: FemSet
+    :param mass: Mass magnitude
+    :param mass_type: Type of mass. See _valid_types. Default is 'MASS'
+    :param ptype: Point mass type. Can be None, 'Isotropic' or 'Anisotropic'
     :param units:
     :param metadata:
     :param parent:
-    :type fem_set: FemSet
+
     """
 
     _valid_types = ["MASS", "NONSTRUCTURAL MASS", "ROTARY INERTIA"]
+    _valid_ptypes = [None, "ISOTROPIC", "ANISOTROPIC"]
 
     def __init__(
         self,
         name,
         fem_set,
         mass,
         mass_type=None,
@@ -2113,18 +2117,23 @@
         metadata=None,
         parent=None,
     ):
         super().__init__(name, metadata, parent)
         self._fem_set = fem_set
         if mass is None:
             raise ValueError("Mass cannot be None")
+        if type(mass) not in (list, tuple):
+            logging.info(f"Mass {type(mass)} converted to list of len=1. Assume equal mass in all 3 transl. DOFs.")
+            mass = [mass]
         self._mass = mass
         self._mass_type = mass_type if mass_type is not None else "MASS"
         if self.type not in Mass._valid_types:
-            raise ValueError(f'Mass type "{self.type}" is not supported')
+            raise ValueError(f'Mass type "{self.type}" is not in list of supported types {self._valid_types}')
+        if ptype not in self._valid_ptypes:
+            raise ValueError(f'Mass point type "{ptype}" is not in list of supported types {self._valid_ptypes}')
         self.point_mass_type = ptype
         self._units = units
 
     @property
     def type(self):
         return self._mass_type.upper()
 
@@ -2135,19 +2144,19 @@
         """
         return self._fem_set
 
     @property
     def mass(self):
         if self.point_mass_type is None:
             if self.type == "MASS":
-                if (len(self._mass) == 1) is False:
+                if type(self._mass) in (list, tuple):
                     raise ValueError("Mass can only be a scalar number for Isotropic mass")
-                return self._mass[0]
+                return float(self._mass[0])
             else:
-                return self._mass
+                return float(self._mass)
         elif self.point_mass_type == "ISOTROPIC":
             if (len(self._mass) == 1) is False:
                 raise ValueError("Mass can only be a scalar number for Isotropic mass")
             return self._mass[0]
         elif self.point_mass_type == "ANISOTROPIC":
             if (len(self._mass) == 3) is False:
                 raise ValueError("Mass must be specified for 3 dofs for Anisotropic mass")
```

### Comparing `ada-py-0.0.8/src/ada/fem/containers.py` & `ada-py-0.0.9/src/ada/fem/containers.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/__init__.py` & `ada-py-0.0.9/src/ada/fem/io/__init__.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/abaqus/common.py` & `ada-py-0.0.9/src/ada/fem/io/abaqus/common.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/abaqus/execute.py` & `ada-py-0.0.9/src/ada/fem/io/abaqus/execute.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/abaqus/reader.py` & `ada-py-0.0.9/src/ada/fem/io/abaqus/reader.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/abaqus/writer.py` & `ada-py-0.0.9/src/ada/fem/io/abaqus/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/calculix/execute.py` & `ada-py-0.0.9/src/ada/fem/io/calculix/execute.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/calculix/writer.py` & `ada-py-0.0.9/src/ada/fem/io/calculix/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/code_aster/execute.py` & `ada-py-0.0.9/src/ada/fem/io/code_aster/execute.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/code_aster/writer.py` & `ada-py-0.0.9/src/ada/fem/io/code_aster/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/io_meshio/__init__.py` & `ada-py-0.0.9/src/ada/fem/io/io_meshio/__init__.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/io_meshio/reader.py` & `ada-py-0.0.9/src/ada/fem/io/io_meshio/reader.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/io_meshio/writer.py` & `ada-py-0.0.9/src/ada/fem/io/io_meshio/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/mesh/common.py` & `ada-py-0.0.9/src/ada/fem/io/mesh/common.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/mesh/recipes.py` & `ada-py-0.0.9/src/ada/fem/io/mesh/recipes.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/sesam/reader.py` & `ada-py-0.0.9/src/ada/fem/io/sesam/reader.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/sesam/writer.py` & `ada-py-0.0.9/src/ada/fem/io/sesam/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,17 @@
 COMPUTER: X86 Windows         INSTALLATION:
 USER:     {user}            ACCOUNT:     \n"""
             )
             d.write(units)
             d.write(self._materials_str)
             d.write(self._sections_str)
             d.write(self._nodes_str)
+            d.write(self._mass_str)
             d.write(self._bc_str)
+            d.write(self._hinges_str)
             d.write(self._elem_str)
             d.write(self._loads_str)
             d.write("IEND                0.00            0.00            0.00            0.00")
 
         print(f'Created an Sesam input deck at "{analysis_dir}"')
 
     @property
@@ -207,15 +209,15 @@
                     )
 
                     if SectionCat.is_i_profile(section.type):
                         sec_str += self.write_ff(
                             "GIORH",
                             [
                                 (secid, section.h, section.t_w, section.w_top),
-                                (section.t_ftop, section.w_top, section.t_ftop, p.Sfy),
+                                (section.t_ftop, section.w_btn, section.t_fbtn, p.Sfy),
                                 (p.Sfz,),
                             ],
                         )
                     elif SectionCat.is_hp_profile(section.type):
                         sec_str += self.write_ff(
                             "GLSEC",
                             [
@@ -232,14 +234,18 @@
                             ],
                         )
                     elif SectionCat.is_circular_profile(section.type):
                         sec_str += self.write_ff(
                             "GPIPE",
                             [(secid, section.r - section.wt, section.r, section.wt), (p.Sfy, p.Sfz)],
                         )
+                    elif SectionCat.is_flatbar(section.type):
+                        sec_str += self.write_ff(
+                            "GBARM", [(secid, section.h, section.w_top, section.w_btn), (p.Sfy, p.Sfz)]
+                        )
                     else:
                         logging.error(f'Unable to convert "{section}". This will be exported as general section only')
 
             elif fem_sec.type == "shell":
                 if fem_sec.thickness not in thick_map.keys():
                     sh_id = next(shid)
                     thick_map[fem_sec.thickness] = sh_id
@@ -274,31 +280,50 @@
                         (el.id, el.id, SesamReader.eltype_2_sesam(el.type), 0),
                         ([n.id for n in el.nodes]),
                     ],
                 )
                 for el in elements
             ]
         )
-        for el in elements:
+
+        def write_elem(el):
+            """
+
+            :param el:
+            :type el: ada.fem.Elem
+            :return: input str for Elem
+            """
             fem_sec = el.fem_sec
             assert isinstance(fem_sec, FemSection)
             if fem_sec.type == "beam":
                 sec_id = fem_sec.section.metadata["numid"]
             elif fem_sec.type == "shell":
                 sec_id = self._thick_map[fem_sec.thickness]
             else:
                 raise ValueError(f'Unsupported elem type "{fem_sec.type}"')
-            out_str += self.write_ff(
+
+            fixno = el.metadata.get("fixno", None)
+            if fixno is None:
+                last_tuples = [(sec_id, 0, 0, 1)]
+            else:
+                h1_fix, h2_fix = fixno
+                last_tuples = [(sec_id, -1, 0, 1), (h1_fix, h2_fix)]
+
+            return self.write_ff(
                 "GELREF1",
                 [
                     (el.id, el.fem_sec.material.id, 0, 0),
                     (0, 0, 0, 0),
-                    (sec_id, 0, 0, 1),
-                ],
+                ]
+                + last_tuples,
             )
+
+        for el in elements:
+            out_str += write_elem(el)
+
         return out_str
 
     @property
     def _nodes_str(self):
         """
         GNODE: GNODE NODEX NODENO NDOF ODOF NODEX
 
@@ -317,24 +342,66 @@
         else:
 
             out_str = "".join([self.write_ff("GNODE", [(no.id, no.id, 6, 123456)]) for no in nodes])
             out_str += "".join([self.write_ff("GCOORD", [(no.id, no[0], no[1], no[2])]) for no in nodes])
             return out_str
 
     @property
+    def _mass_str(self):
+        out_str = ""
+
+        for mass in self._gmass.values():
+            for m in mass.fem_set.members:
+                if type(mass.mass) is float:
+                    masses = [mass.mass for _ in range(0, 3)] + [0, 0, 0]
+                else:
+                    raise NotImplementedError()
+                data = (tuple([m.id, 6] + masses[:2]), tuple(masses[2:]))
+                out_str += self.write_ff("BNMASS", data)
+        return out_str
+
+    @property
     def _bc_str(self):
         out_str = ""
         for bc in self._gbcs:
             for m in bc.fem_set.members:
                 dofs = [1 if i in bc.dofs else 0 for i in range(1, 7)]
                 data = [tuple([m.id, 6] + dofs[:2]), tuple(dofs[2:])]
                 out_str += self.write_ff("BNBCD", data)
         return out_str
 
     @property
+    def _hinges_str(self):
+        from ada.core.utils import Counter
+
+        out_str = ""
+        h = Counter(0)
+
+        def write_hinge(hinge):
+            dofs = [0 if i in hinge else 1 for i in range(1, 7)]
+            fix_id = next(h)
+            data = [tuple([fix_id, 3, 0, 0]), tuple(dofs[:4]), tuple(dofs[4:])]
+            return fix_id, self.write_ff("BELFIX", data)
+
+        for el in self._gelements:
+            h1, h2 = el.metadata.get("h1", None), el.metadata.get("h2", None)
+            if h2 is None and h1 is None:
+                continue
+            h1_fix, h2_fix = 0, 0
+            if h1 is not None:
+                h1_fix, res_str = write_hinge(h1)
+                out_str += res_str
+            if h2 is not None:
+                h2_fix, res_str = write_hinge(h2)
+                out_str += res_str
+            el.metadata["fixno"] = h1_fix, h2_fix
+
+        return out_str
+
+    @property
     def _loads_str(self):
         out_str = ""
         for i, l in enumerate(self._gloads):
             assert isinstance(l, Load)
             lid = i + 1
             out_str += self.write_ff("TDLOAD", [(4, lid, 100 + len(l.name), 0), (l.name,)])
             if l.type in ["acc", "grav"]:
```

### Comparing `ada-py-0.0.8/src/ada/fem/io/usfos/writer.py` & `ada-py-0.0.9/src/ada/fem/io/usfos/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/utils.py` & `ada-py-0.0.9/src/ada/fem/io/utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/xdmf/common.py` & `ada-py-0.0.9/src/ada/fem/io/xdmf/common.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/xdmf/reader.py` & `ada-py-0.0.9/src/ada/fem/io/xdmf/reader.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/io/xdmf/writer.py` & `ada-py-0.0.9/src/ada/fem/io/xdmf/writer.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/fem/utils.py` & `ada-py-0.0.9/src/ada/fem/utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/materials/metals/__init__.py` & `ada-py-0.0.9/src/ada/materials/metals/__init__.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/materials/polymers/__init__.py` & `ada-py-0.0.9/src/ada/materials/polymers/__init__.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/materials/polymers/models.py` & `ada-py-0.0.9/src/ada/materials/polymers/models.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/materials/polymers/utils.py` & `ada-py-0.0.9/src/ada/materials/polymers/utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/param_models/basic_module.py` & `ada-py-0.0.9/src/ada/param_models/basic_module.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/param_models/basic_structural_components.py` & `ada-py-0.0.9/src/ada/param_models/basic_structural_components.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/param_models/fem_models.py` & `ada-py-0.0.9/src/ada/param_models/fem_models.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/sections/__init__.py` & `ada-py-0.0.9/src/ada/sections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,20 @@
     def _calc_circular(self):
 
         s = self.parent
         self._Ax = math.pi * s.r ** 2
         self._Iy = (math.pi * s.r ** 4) / 4
         self._Iz = self._Iy
 
+    def _calc_flatbar(self):
+        s = self.parent
+        self._Ax = (s.w_btn + s.w_top) / 2 * s.h
+        self._Iy = s.w_top * s.h ** 3 / 12
+        self._Iz = s.h * s.w_top ** 3 / 12
+
     def _calc_channel(self):
         """
 
         :return:
         """
         posweb = True
         s = self.parent
@@ -307,14 +313,16 @@
             pass  # it is known
         elif self.parent.type in SectionCat.tubular:
             self._calc_tubular()
         elif SectionCat.is_hp_profile(self.parent.type):
             self._calc_angular()
         elif self.parent.type in SectionCat.channels:
             self._calc_channel()
+        elif SectionCat.is_flatbar(self.parent.type):
+            self._calc_flatbar()
         else:
             raise Exception(
                 f'section type "{self.parent.type}" is not yet supported in the cross section parameter calculations'
             )
 
     @property
     def parent(self):
@@ -786,7 +794,11 @@
     @classmethod
     def is_hp_profile(cls, bmtype):
         return True if bmtype.upper() in cls.angular else False
 
     @classmethod
     def is_circular_profile(cls, bmtype):
         return True if bmtype.upper() in cls.tubular + cls.circular else False
+
+    @classmethod
+    def is_flatbar(cls, bmtype):
+        return True if bmtype.upper() in cls.flatbar else False
```

### Comparing `ada-py-0.0.8/src/ada/sections/resources/ProfileDB.json` & `ada-py-0.0.9/src/ada/sections/resources/ProfileDB.json`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada/sections/utils.py` & `ada-py-0.0.9/src/ada/sections/utils.py`

 * *Files identical despite different names*

### Comparing `ada-py-0.0.8/src/ada_py.egg-info/PKG-INFO` & `ada-py-0.0.9/src/ada_py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ada-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Assembly for Design & Analysis - A toolkit for structural analysis and design
 Home-page: https://github.com/krande/adapy
 Author: Kristoffer H. Andersen
 Author-email: kristoffer_andersen@outlook.com
 License: GNU GPLv3
 Project-URL: Code, https://github.com/krande/adapy
 Project-URL: Issues, https://github.com/krande/adapy/issues
 Description: # ADA - Assembly for Design & Analysis
         
-        A toolkit for structural analysis and design that focus on interoperability between
+        A python library for structural analysis and design that focus on interoperability between
         IFC and various Finite Element formats.
         
         This library is still undergoing significant development so expect there to be occasional bugs and breaking changes.
         
         Try the latest build online here
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Krande/adapy/main)
@@ -87,31 +87,50 @@
         
         a = beam_ex1()
         
         a.to_fem("MyCantilever_abaqus", "abaqus", overwrite=True, execute=True, run_ext=True)
         a.to_fem("MyCantilever_calculix", "calculix", overwrite=True, execute=True)
         ```
         
-        after the execution is finished you can look at the results
+        after the execution is finished you can look at the results (in Paraview or Abaqus CAE for the results from 
+        calculix and/or abaqus respectively)
+        
         
         ![Paraview Results](docs/_static/figures/fem_beam_paraview.png)
         ![Abaqus Results](docs/_static/figures/fem_beam_abaqus.png)
         
+        or if your prefer to keep it in python here is a way you can use meshio to read the results from calculix and do your
+        postprocessing using python only.
+        
+        ```python
+        from ada.config import Settings
+        import meshio
+        
+        vtu = Settings.scratch_dir / "MyCantilever_calculix" / "MyCantilever_calculix.vtu"
+        mesh = meshio.read(vtu)
+        
+        # Von Mises stresses and displacement at a point @ index=0
+        print(mesh.point_data['S'][0])
+        print(mesh.point_data['U'][0])
+        ```
+        
+        In short `beam_ex1` creates a `Beam` object which it uses to create a shell element `FEM` mesh using 
+        a mesh recipe [create_beam_mesh](https://github.com/Krande/adapy/blob/c594ccbfbdd2ea9384fa8a4721a65580331b4a09/src/ada/fem/io/mesh/recipes.py#L99-L223). 
+        The recipe uses [GMSH](https://gmsh.info/) to construct elements on nodes. 
         
-        In short `beam_ex1` creates a `Beam` object which it uses to create a FEM mesh comprised of shell elements using GMSH. 
         
         The current reasoning is to work with a base representation of beam/plates and have the ability
         to easily create a FEM representation of any of the base objects in 1D (beam elements), 
         2D (shell elements) or 3D (elements) using your own meshing recipes (i.e. not just build a mesh, but a recipe for 
         building meshes).
         
         
         **Note!**
         
-        This example assumes you have installed Abaqus and Calculix locally on your computer.
+        The above example assumes you have installed Abaqus and Calculix locally on your computer.
         
         To set correct paths to your installations of Abaqus or Calculix you wish to use there are a few ways of doing so.
         
         1. Add directory path of abaqus.bat or ccx.exe to your system path.
         2. Add directory paths to system environment variables. This can be done by using the control panel or running the following from a cmd prompt with administrator rights:
             
         ```cmd
@@ -145,15 +164,14 @@
         For developers interested in contributing to this project feel free to make a fork, experiment and create a pull request
         when you have something you would like to add/change/remove. 
         
         Before making a pull request you need to lint with, isort, flake8 and black 
         
         ````
         pip install black isort flake8
-        cd src/ada
         isort .
         flake8 .
         black .
         ````
         
         
         ## Project Responsible ###
```

### Comparing `ada-py-0.0.8/src/ada_py.egg-info/SOURCES.txt` & `ada-py-0.0.9/src/ada_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

