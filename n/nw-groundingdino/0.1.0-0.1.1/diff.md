# Comparing `tmp/nw_groundingdino-0.1.0.tar.gz` & `tmp/nw_groundingdino-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nw_groundingdino-0.1.0.tar", last modified: Mon Apr 17 04:13:39 2023, max compression
+gzip compressed data, was "nw_groundingdino-0.1.1.tar", last modified: Mon Apr 17 07:01:08 2023, max compression
```

## Comparing `nw_groundingdino-0.1.0.tar` & `nw_groundingdino-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.218455 nw_groundingdino-0.1.0/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    11354 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/LICENSE
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    13205 2023-04-17 04:13:39.218249 nw_groundingdino-0.1.0/PKG-INFO
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     9976 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/README.md
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.211351 nw_groundingdino-0.1.0/groundingdino/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/__init__.py
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.211696 nw_groundingdino-0.1.0/groundingdino/models/
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.213678 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)      823 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.214606 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       37 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7972 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     6866 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    29339 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    12242 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    11825 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    16691 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    15482 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    36805 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     4020 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    10087 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)      754 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/__init__.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     2143 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/models/registry.py
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.217043 nw_groundingdino-0.1.0/groundingdino/util/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       71 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/__init__.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3905 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/box_ops.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1157 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7997 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/inference.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3303 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/logger.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    23348 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/misc.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    14380 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/slconfig.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     5377 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/slio.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1567 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/time_counter.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    17712 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/utils.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    12047 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/visualizer.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3489 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.0/groundingdino/util/vl_utils.py
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       22 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/groundingdino/version.py
-drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 04:13:39.218012 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    13205 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/PKG-INFO
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1358 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/SOURCES.txt
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)        1 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/dependency_links.txt
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       99 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/requires.txt
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       14 2023-04-17 04:13:39.000000 nw_groundingdino-0.1.0/nw_groundingdino.egg-info/top_level.txt
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       38 2023-04-17 04:13:39.218493 nw_groundingdino-0.1.0/setup.cfg
--rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7140 2023-04-17 04:13:25.000000 nw_groundingdino-0.1.0/setup.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.039024 nw_groundingdino-0.1.1/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    11354 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/LICENSE
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    13205 2023-04-17 07:01:08.038793 nw_groundingdino-0.1.1/PKG-INFO
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     9976 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/README.md
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.031690 nw_groundingdino-0.1.1/groundingdino/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/__init__.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.031913 nw_groundingdino-0.1.1/groundingdino/datasets/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:00:26.000000 nw_groundingdino-0.1.1/groundingdino/datasets/__init__.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     9711 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.032456 nw_groundingdino-0.1.1/groundingdino/models/
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.034660 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)      823 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.035422 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       37 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7972 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     6866 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    29339 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    12242 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    11825 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    16691 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    15482 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    36805 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     4020 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    10087 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)      754 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/__init__.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     2143 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/models/registry.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.037794 nw_groundingdino-0.1.1/groundingdino/util/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       71 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/__init__.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3905 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/box_ops.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1157 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7997 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/inference.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3303 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/logger.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    23348 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/misc.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    14380 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/slconfig.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     5377 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/slio.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1567 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/time_counter.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    17712 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/utils.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    12047 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/visualizer.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     3489 2023-04-11 12:30:43.000000 nw_groundingdino-0.1.1/groundingdino/util/vl_utils.py
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       22 2023-04-17 07:01:07.000000 nw_groundingdino-0.1.1/groundingdino/version.py
+drwxr-xr-x   0 shaoshuai.shao   (501) staff       (20)        0 2023-04-17 07:01:08.038576 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)    13205 2023-04-17 07:01:07.000000 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/PKG-INFO
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     1430 2023-04-17 07:01:08.000000 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/SOURCES.txt
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)        1 2023-04-17 07:01:07.000000 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/dependency_links.txt
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       99 2023-04-17 07:01:07.000000 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/requires.txt
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       14 2023-04-17 07:01:07.000000 nw_groundingdino-0.1.1/nw_groundingdino.egg-info/top_level.txt
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)       38 2023-04-17 07:01:08.039074 nw_groundingdino-0.1.1/setup.cfg
+-rw-r--r--   0 shaoshuai.shao   (501) staff       (20)     7140 2023-04-17 07:00:52.000000 nw_groundingdino-0.1.1/setup.py
```

### Comparing `nw_groundingdino-0.1.0/LICENSE` & `nw_groundingdino-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/PKG-INFO` & `nw_groundingdino-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nw_groundingdino
-Version: 0.1.0
+Version: 0.1.1
 Summary: open-set object detector
 Home-page: https://github.com/IDEA-Research/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nw_groundingdino-0.1.0/README.md` & `nw_groundingdino-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/__init__.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/bertwarper.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/fuse_modules.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/groundingdino.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/transformer.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/GroundingDINO/utils.py` & `nw_groundingdino-0.1.1/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/__init__.py` & `nw_groundingdino-0.1.1/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/models/registry.py` & `nw_groundingdino-0.1.1/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/box_ops.py` & `nw_groundingdino-0.1.1/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/get_tokenlizer.py` & `nw_groundingdino-0.1.1/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/inference.py` & `nw_groundingdino-0.1.1/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/logger.py` & `nw_groundingdino-0.1.1/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/misc.py` & `nw_groundingdino-0.1.1/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/slconfig.py` & `nw_groundingdino-0.1.1/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/slio.py` & `nw_groundingdino-0.1.1/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/time_counter.py` & `nw_groundingdino-0.1.1/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/utils.py` & `nw_groundingdino-0.1.1/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/visualizer.py` & `nw_groundingdino-0.1.1/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/groundingdino/util/vl_utils.py` & `nw_groundingdino-0.1.1/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `nw_groundingdino-0.1.0/nw_groundingdino.egg-info/PKG-INFO` & `nw_groundingdino-0.1.1/nw_groundingdino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nw-groundingdino
-Version: 0.1.0
+Version: 0.1.1
 Summary: open-set object detector
 Home-page: https://github.com/IDEA-Research/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nw_groundingdino-0.1.0/nw_groundingdino.egg-info/SOURCES.txt` & `nw_groundingdino-0.1.1/nw_groundingdino.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.py
 groundingdino/__init__.py
 groundingdino/version.py
+groundingdino/datasets/__init__.py
+groundingdino/datasets/transforms.py
 groundingdino/models/__init__.py
 groundingdino/models/registry.py
 groundingdino/models/GroundingDINO/__init__.py
 groundingdino/models/GroundingDINO/bertwarper.py
 groundingdino/models/GroundingDINO/fuse_modules.py
 groundingdino/models/GroundingDINO/groundingdino.py
 groundingdino/models/GroundingDINO/ms_deform_attn.py
```

### Comparing `nw_groundingdino-0.1.0/setup.py` & `nw_groundingdino-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     with open("LICENSE", "r", encoding="utf-8") as f:
         license = f.read()
 
     write_version_file()
 
     setup(
         name="nw_groundingdino",
-        version="0.1.0",
+        version="0.1.1",
         author="International Digital Economy Academy, Shilong Liu",
         url="https://github.com/IDEA-Research/GroundingDINO",
         description="open-set object detector",
         license=license,
         install_requires=parse_requirements("requirements.txt"),
         packages=find_packages(
             exclude=(
```

