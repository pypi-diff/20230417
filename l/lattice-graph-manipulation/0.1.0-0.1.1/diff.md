# Comparing `tmp/Lattice-Graph-Manipulation-0.1.0.tar.gz` & `tmp/Lattice-Graph-Manipulation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lattice-Graph-Manipulation-0.1.0.tar", last modified: Mon Apr 17 01:42:28 2023, max compression
+gzip compressed data, was "Lattice-Graph-Manipulation-0.1.1.tar", last modified: Mon Apr 17 08:27:28 2023, max compression
```

## Comparing `Lattice-Graph-Manipulation-0.1.0.tar` & `Lattice-Graph-Manipulation-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1070 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.0/LICENSE
--rw-r--r--   0        0        0     3643 2023-04-16 21:36:33.181824 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv
--rw-r--r--   0        0        0     7806 2023-04-16 21:36:33.208492 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf
--rw-r--r--   0        0        0      528 2023-04-16 21:39:55.546127 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv
--rw-r--r--   0        0        0     6413 2023-04-16 21:39:55.562795 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv.pdf
--rw-r--r--   0        0        0     3643 2023-04-16 21:39:26.018518 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv
--rw-r--r--   0        0        0     7811 2023-04-16 21:39:26.038519 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf
--rw-r--r--   0        0        0      287 2023-04-16 23:48:35.740878 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv
--rw-r--r--   0        0        0     4730 2023-04-16 23:48:35.764212 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv.pdf
--rw-r--r--   0        0        0      603 2023-04-16 21:35:09.825570 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/Digraph.gv
--rw-r--r--   0        0        0     6440 2023-04-16 21:35:09.848903 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/Digraph.gv.pdf
--rw-r--r--   0        0        0        0 2023-04-16 21:00:24.727352 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/__init__.py
--rw-r--r--   0        0        0      642 2023-04-16 21:36:33.148489 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv
--rw-r--r--   0        0        0     6435 2023-04-16 21:36:33.175157 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf
--rw-r--r--   0        0        0      528 2023-04-16 21:39:46.689183 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv
--rw-r--r--   0        0        0     6403 2023-04-16 21:39:46.709184 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf
--rw-r--r--   0        0        0      642 2023-04-16 21:39:55.566128 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv
--rw-r--r--   0        0        0     6439 2023-04-16 21:39:55.586129 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf
--rw-r--r--   0        0        0      642 2023-04-16 21:39:25.991851 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv
--rw-r--r--   0        0        0     6445 2023-04-16 21:39:26.015185 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf
--rw-r--r--   0        0        0     3643 2023-04-16 21:39:55.589462 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv
--rw-r--r--   0        0        0     7805 2023-04-16 21:39:55.609463 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv.pdf
--rw-r--r--   0        0        0     1055 2023-04-16 23:49:48.851041 Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/simple_examples.py
--rw-r--r--   0        0        0        9 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.0/README.md
--rw-r--r--   0        0        0       61 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/__init__.py
--rw-r--r--   0        0        0       99 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/edge/__init__.py
--rw-r--r--   0        0        0      569 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/edge/edge.py
--rw-r--r--   0        0        0      440 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/edge/traversaledge.py
--rw-r--r--   0        0        0      114 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/graph/__init__.py
--rw-r--r--   0        0        0     1615 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/graph/bbtree.py
--rw-r--r--   0        0        0     3883 2023-04-16 21:39:25.921848 Lattice-Graph-Manipulation-0.1.0/lattice/graph/graph.py
--rw-r--r--   0        0        0      872 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/graph/tree.py
--rw-r--r--   0        0        0       43 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/node/__init__.py
--rw-r--r--   0        0        0      875 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.0/lattice/node/node.py
--rw-r--r--   0        0        0      369 2023-04-17 01:39:00.115325 Lattice-Graph-Manipulation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3643 2023-04-16 21:36:33.181824 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv
+-rw-r--r--   0        0        0     7806 2023-04-16 21:36:33.208492 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf
+-rw-r--r--   0        0        0      528 2023-04-16 21:39:55.546127 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv
+-rw-r--r--   0        0        0     6413 2023-04-16 21:39:55.562795 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv.pdf
+-rw-r--r--   0        0        0     3643 2023-04-16 21:39:26.018518 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv
+-rw-r--r--   0        0        0     7811 2023-04-16 21:39:26.038519 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf
+-rw-r--r--   0        0        0      287 2023-04-16 23:48:35.740878 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv
+-rw-r--r--   0        0        0     4730 2023-04-16 23:48:35.764212 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv.pdf
+-rw-r--r--   0        0        0      603 2023-04-16 21:35:09.825570 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv
+-rw-r--r--   0        0        0     6440 2023-04-16 21:35:09.848903 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv.pdf
+-rw-r--r--   0        0        0        0 2023-04-16 21:00:24.727352 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-16 21:36:33.148489 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv
+-rw-r--r--   0        0        0     6435 2023-04-16 21:36:33.175157 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf
+-rw-r--r--   0        0        0      528 2023-04-16 21:39:46.689183 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv
+-rw-r--r--   0        0        0     6403 2023-04-16 21:39:46.709184 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf
+-rw-r--r--   0        0        0      642 2023-04-16 21:39:55.566128 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv
+-rw-r--r--   0        0        0     6439 2023-04-16 21:39:55.586129 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf
+-rw-r--r--   0        0        0      642 2023-04-16 21:39:25.991851 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv
+-rw-r--r--   0        0        0     6445 2023-04-16 21:39:26.015185 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf
+-rw-r--r--   0        0        0     3643 2023-04-16 21:39:55.589462 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv
+-rw-r--r--   0        0        0     7805 2023-04-16 21:39:55.609463 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv.pdf
+-rw-r--r--   0        0        0     1055 2023-04-16 23:49:48.851041 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/simple_examples.py
+-rw-r--r--   0        0        0        9 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.1/README.md
+-rw-r--r--   0        0        0       61 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/__init__.py
+-rw-r--r--   0        0        0       99 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/edge.py
+-rw-r--r--   0        0        0      440 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/traversaledge.py
+-rw-r--r--   0        0        0      114 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/__init__.py
+-rw-r--r--   0        0        0     1615 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/bbtree.py
+-rw-r--r--   0        0        0     3883 2023-04-16 21:39:25.921848 Lattice-Graph-Manipulation-0.1.1/lattice/graph/graph.py
+-rw-r--r--   0        0        0      872 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/tree.py
+-rw-r--r--   0        0        0       43 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/node/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/node/node.py
+-rw-r--r--   0        0        0      368 2023-04-17 08:27:21.116437 Lattice-Graph-Manipulation-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-0.1.1/PKG-INFO
```

### Comparing `Lattice-Graph-Manipulation-0.1.0/LICENSE` & `Lattice-Graph-Manipulation-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/Digraph.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/Digraph.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv.pdf` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/Lattice_Scripts/simple_examples.py` & `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/simple_examples.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/lattice/edge/edge.py` & `Lattice-Graph-Manipulation-0.1.1/lattice/edge/edge.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/lattice/graph/bbtree.py` & `Lattice-Graph-Manipulation-0.1.1/lattice/graph/bbtree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/lattice/graph/graph.py` & `Lattice-Graph-Manipulation-0.1.1/lattice/graph/graph.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/lattice/graph/tree.py` & `Lattice-Graph-Manipulation-0.1.1/lattice/graph/tree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.0/lattice/node/node.py` & `Lattice-Graph-Manipulation-0.1.1/lattice/node/node.py`

 * *Files identical despite different names*

