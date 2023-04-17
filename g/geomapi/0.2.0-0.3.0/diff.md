# Comparing `tmp/geomapi-0.2.0.tar.gz` & `tmp/geomapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapi-0.2.0.tar", last modified: Tue Apr 11 15:06:27 2023, max compression
+gzip compressed data, was "geomapi-0.3.0.tar", last modified: Mon Apr 17 15:38:30 2023, max compression
```

## Comparing `geomapi-0.2.0.tar` & `geomapi-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.706006 geomapi-0.2.0/
--rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-04-11 15:04:48.000000 geomapi-0.2.0/LICENSE
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-11 15:06:27.706006 geomapi-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-04-11 15:04:48.000000 geomapi-0.2.0/README.md
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/developmenttests/
--rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-04-11 15:04:48.000000 geomapi-0.2.0/developmenttests/QualityCompare.py
--rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-04-11 15:04:48.000000 geomapi-0.2.0/developmenttests/QualityCompare_gui.py
--rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-04-11 15:04:59.000000 geomapi-0.2.0/developmenttests/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/context.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/ifc_to_nodes.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/import_e57.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/geomapi/
--rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/nodes/
--rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    34991 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/imagenode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/linesetnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/node.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/orthonode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/sessionnode.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/
--rw-rw-rw-   0 root         (0) daemon       (1)    45354 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/alignmenttools/
--rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/match.py
--rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/params.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/completiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/completiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/inspectiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/inspectiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/machinelearningtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/machinelearningtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/progresstools/
--rw-rw-rw-   0 root         (0) daemon       (1)    35729 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/progresstools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/validationtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    23868 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/validationtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/utils/
--rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)   108378 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/imageutils.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/geomapi.egg-info/
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) daemon       (1)     1539 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) daemon       (1)        1 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) daemon       (1)      194 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) daemon       (1)       30 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-04-11 15:04:49.000000 geomapi-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-04-11 15:06:27.706006 geomapi-0.2.0/setup.cfg
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.706006 geomapi-0.2.0/test/
--rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_alignmenttools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_completiontools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    24257 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_imageutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_imgnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_node.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_progresstools.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_sessionnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_tools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_utils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.033697 geomapi-0.3.0/
+-rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-04-17 15:37:01.000000 geomapi-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-17 15:38:30.033697 geomapi-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-04-17 15:37:01.000000 geomapi-0.3.0/README.md
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/developmenttests/
+-rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-04-17 15:37:01.000000 geomapi-0.3.0/developmenttests/QualityCompare.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-04-17 15:37:01.000000 geomapi-0.3.0/developmenttests/QualityCompare_gui.py
+-rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-04-17 15:37:12.000000 geomapi-0.3.0/developmenttests/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/context.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/ifc_to_nodes.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/import_e57.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/geomapi/
+-rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/nodes/
+-rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    34991 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/imagenode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/linesetnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/orthonode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/sessionnode.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    45354 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/alignmenttools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/match.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/params.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/completiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/completiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/inspectiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/inspectiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/machinelearningtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/machinelearningtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/progresstools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    35729 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/progresstools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/validationtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    23868 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/validationtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/utils/
+-rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)   108378 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/imageutils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/geomapi.egg-info/
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) daemon       (1)     1539 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) daemon       (1)        1 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) daemon       (1)      194 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) daemon       (1)       30 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-04-17 15:37:02.000000 geomapi-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-04-17 15:38:30.033697 geomapi-0.3.0/setup.cfg
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.033697 geomapi-0.3.0/test/
+-rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_alignmenttools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_completiontools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    24257 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_imageutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_imgnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_progresstools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_sessionnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_tools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_utils.py
```

### Comparing `geomapi-0.2.0/LICENSE` & `geomapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/PKG-INFO` & `geomapi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <=3.10
+Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![geomapiLogo](https://gitlab.kuleuven.be/uploads/-/system/project/avatar/7619/GeoMapiLogo.png?width=64)
 
 # GeomAPI
```

### Comparing `geomapi-0.2.0/README.md` & `geomapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/developmenttests/QualityCompare.py` & `geomapi-0.3.0/developmenttests/QualityCompare.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/developmenttests/QualityCompare_gui.py` & `geomapi-0.3.0/developmenttests/QualityCompare_gui.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/developmenttests/ifc_to_nodes.py` & `geomapi-0.3.0/developmenttests/ifc_to_nodes.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/developmenttests/import_e57.py` & `geomapi-0.3.0/developmenttests/import_e57.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/bimnode.py` & `geomapi-0.3.0/geomapi/nodes/bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/geometrynode.py` & `geomapi-0.3.0/geomapi/nodes/geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/imagenode.py` & `geomapi-0.3.0/geomapi/nodes/imagenode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/linesetnode.py` & `geomapi-0.3.0/geomapi/nodes/linesetnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/meshnode.py` & `geomapi-0.3.0/geomapi/nodes/meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/node.py` & `geomapi-0.3.0/geomapi/nodes/node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/orthonode.py` & `geomapi-0.3.0/geomapi/nodes/orthonode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/pointcloudnode.py` & `geomapi-0.3.0/geomapi/nodes/pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/nodes/sessionnode.py` & `geomapi-0.3.0/geomapi/nodes/sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/__init__.py` & `geomapi-0.3.0/geomapi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/alignmenttools/__init__.py` & `geomapi-0.3.0/geomapi/tools/alignmenttools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/alignmenttools/match.py` & `geomapi-0.3.0/geomapi/tools/alignmenttools/match.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/alignmenttools/params.py` & `geomapi-0.3.0/geomapi/tools/alignmenttools/params.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/completiontools/__init__.py` & `geomapi-0.3.0/geomapi/tools/completiontools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/machinelearningtools/__init__.py` & `geomapi-0.3.0/geomapi/tools/machinelearningtools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/progresstools/__init__.py` & `geomapi-0.3.0/geomapi/tools/progresstools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/tools/validationtools/__init__.py` & `geomapi-0.3.0/geomapi/tools/validationtools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/utils/__init__.py` & `geomapi-0.3.0/geomapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/utils/geometryutils.py` & `geomapi-0.3.0/geomapi/utils/geometryutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/utils/geospatialutils.py` & `geomapi-0.3.0/geomapi/utils/geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi/utils/imageutils.py` & `geomapi-0.3.0/geomapi/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/geomapi.egg-info/PKG-INFO` & `geomapi-0.3.0/geomapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <=3.10
+Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![geomapiLogo](https://gitlab.kuleuven.be/uploads/-/system/project/avatar/7619/GeoMapiLogo.png?width=64)
 
 # GeomAPI
```

### Comparing `geomapi-0.2.0/geomapi.egg-info/SOURCES.txt` & `geomapi-0.3.0/geomapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/setup.cfg` & `geomapi-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = geomapi
-version = 0.2.0
+version = 0.3.0
 author = Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 description = A standard library to manage geomatic data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 keywords = Geomatics, alignment, monitoring, validation, progress, point clouds, computer vision, deep learning
 License = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-python_requires = <=3.10
+python_requires = <=3.11
 install_requires = 
 	open3d
 	opencv-python
 	pye57
 	numpy
 	numpy-quaternion
 	rdflib
```

### Comparing `geomapi-0.2.0/test/test_alignmenttools.py` & `geomapi-0.3.0/test/test_alignmenttools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_bimnode.py` & `geomapi-0.3.0/test/test_bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_completiontools.py` & `geomapi-0.3.0/test/test_completiontools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_geometrynode.py` & `geomapi-0.3.0/test/test_geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_geometryutils.py` & `geomapi-0.3.0/test/test_geometryutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_geospatialutils.py` & `geomapi-0.3.0/test/test_geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_imageutils.py` & `geomapi-0.3.0/test/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_imgnode.py` & `geomapi-0.3.0/test/test_imgnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_meshnode.py` & `geomapi-0.3.0/test/test_meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_node.py` & `geomapi-0.3.0/test/test_node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_pointcloudnode.py` & `geomapi-0.3.0/test/test_pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_progresstools.py` & `geomapi-0.3.0/test/test_progresstools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_sessionnode.py` & `geomapi-0.3.0/test/test_sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_tools.py` & `geomapi-0.3.0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.2.0/test/test_utils.py` & `geomapi-0.3.0/test/test_utils.py`

 * *Files identical despite different names*

