# Comparing `tmp/icat-iml-0.1.0.tar.gz` & `tmp/icat-iml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icat-iml-0.1.0.tar", last modified: Mon Apr 17 15:34:32 2023, max compression
+gzip compressed data, was "icat-iml-0.1.1.tar", last modified: Mon Apr 17 19:35:53 2023, max compression
```

## Comparing `icat-iml-0.1.0.tar` & `icat-iml-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 15:34:32.138563 icat-iml-0.1.0/
--rw-r--r--   0 81n      (42021) users      (100)     1524 2023-04-17 14:53:45.000000 icat-iml-0.1.0/LICENSE
--rw-r--r--   0 81n      (42021) users      (100)      712 2023-04-17 15:34:32.138563 icat-iml-0.1.0/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)      211 2023-04-17 14:10:52.000000 icat-iml-0.1.0/README.md
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 15:34:32.134563 icat-iml-0.1.0/icat/
--rw-r--r--   0 81n      (42021) users      (100)       22 2023-04-17 14:11:15.000000 icat-iml-0.1.0/icat/__init__.py
--rw-r--r--   0 81n      (42021) users      (100)    23409 2023-04-17 14:58:08.000000 icat-iml-0.1.0/icat/anchorlist.py
--rw-r--r--   0 81n      (42021) users      (100)    17062 2023-04-17 14:58:08.000000 icat-iml-0.1.0/icat/anchors.py
--rw-r--r--   0 81n      (42021) users      (100)    17837 2023-04-17 14:58:12.000000 icat-iml-0.1.0/icat/data.py
--rw-r--r--   0 81n      (42021) users      (100)     3297 2023-04-17 13:46:04.000000 icat-iml-0.1.0/icat/histogram.py
--rw-r--r--   0 81n      (42021) users      (100)     3738 2023-04-17 14:58:08.000000 icat-iml-0.1.0/icat/histograms.py
--rw-r--r--   0 81n      (42021) users      (100)     7117 2023-04-17 14:58:08.000000 icat-iml-0.1.0/icat/instance.py
--rw-r--r--   0 81n      (42021) users      (100)    13184 2023-04-17 13:46:04.000000 icat-iml-0.1.0/icat/model.py
--rw-r--r--   0 81n      (42021) users      (100)     5524 2023-04-17 14:58:08.000000 icat-iml-0.1.0/icat/table.py
--rw-r--r--   0 81n      (42021) users      (100)     9433 2023-04-17 14:58:12.000000 icat-iml-0.1.0/icat/view.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 15:34:32.138563 icat-iml-0.1.0/icat_iml.egg-info/
--rw-r--r--   0 81n      (42021) users      (100)      712 2023-04-17 15:34:32.000000 icat-iml-0.1.0/icat_iml.egg-info/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)      547 2023-04-17 15:34:32.000000 icat-iml-0.1.0/icat_iml.egg-info/SOURCES.txt
--rw-r--r--   0 81n      (42021) users      (100)        1 2023-04-17 15:34:32.000000 icat-iml-0.1.0/icat_iml.egg-info/dependency_links.txt
--rw-r--r--   0 81n      (42021) users      (100)       62 2023-04-17 15:34:32.000000 icat-iml-0.1.0/icat_iml.egg-info/requires.txt
--rw-r--r--   0 81n      (42021) users      (100)        5 2023-04-17 15:34:32.000000 icat-iml-0.1.0/icat_iml.egg-info/top_level.txt
--rw-r--r--   0 81n      (42021) users      (100)       31 2023-04-17 14:58:06.000000 icat-iml-0.1.0/pyproject.toml
--rw-r--r--   0 81n      (42021) users      (100)       38 2023-04-17 15:34:32.138563 icat-iml-0.1.0/setup.cfg
--rw-r--r--   0 81n      (42021) users      (100)     1060 2023-04-17 15:26:53.000000 icat-iml-0.1.0/setup.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 15:34:32.138563 icat-iml-0.1.0/tests/
--rw-r--r--   0 81n      (42021) users      (100)     6467 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_anchorlist.py
--rw-r--r--   0 81n      (42021) users      (100)     9102 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_anchors.py
--rw-r--r--   0 81n      (42021) users      (100)     3813 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_datamanager.py
--rw-r--r--   0 81n      (42021) users      (100)     4099 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_histograms.py
--rw-r--r--   0 81n      (42021) users      (100)     2522 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_instance.py
--rw-r--r--   0 81n      (42021) users      (100)      374 2023-04-17 13:46:04.000000 icat-iml-0.1.0/tests/test_integrations.py
--rw-r--r--   0 81n      (42021) users      (100)     9266 2023-04-17 14:58:07.000000 icat-iml-0.1.0/tests/test_model.py
--rw-r--r--   0 81n      (42021) users      (100)     3885 2023-04-17 14:58:07.000000 icat-iml-0.1.0/tests/test_view.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:35:53.581402 icat-iml-0.1.1/
+-rw-r--r--   0 81n      (42021) users      (100)     1524 2023-04-17 14:53:45.000000 icat-iml-0.1.1/LICENSE
+-rw-r--r--   0 81n      (42021) users      (100)     1115 2023-04-17 19:35:53.581402 icat-iml-0.1.1/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)      614 2023-04-17 17:30:21.000000 icat-iml-0.1.1/README.md
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:35:53.581402 icat-iml-0.1.1/icat/
+-rw-r--r--   0 81n      (42021) users      (100)       22 2023-04-17 19:33:27.000000 icat-iml-0.1.1/icat/__init__.py
+-rw-r--r--   0 81n      (42021) users      (100)    23409 2023-04-17 14:58:08.000000 icat-iml-0.1.1/icat/anchorlist.py
+-rw-r--r--   0 81n      (42021) users      (100)    17062 2023-04-17 14:58:08.000000 icat-iml-0.1.1/icat/anchors.py
+-rw-r--r--   0 81n      (42021) users      (100)    17837 2023-04-17 14:58:12.000000 icat-iml-0.1.1/icat/data.py
+-rw-r--r--   0 81n      (42021) users      (100)     3297 2023-04-17 13:46:04.000000 icat-iml-0.1.1/icat/histogram.py
+-rw-r--r--   0 81n      (42021) users      (100)     3738 2023-04-17 14:58:08.000000 icat-iml-0.1.1/icat/histograms.py
+-rw-r--r--   0 81n      (42021) users      (100)     7117 2023-04-17 14:58:08.000000 icat-iml-0.1.1/icat/instance.py
+-rw-r--r--   0 81n      (42021) users      (100)    13184 2023-04-17 13:46:04.000000 icat-iml-0.1.1/icat/model.py
+-rw-r--r--   0 81n      (42021) users      (100)     5524 2023-04-17 14:58:08.000000 icat-iml-0.1.1/icat/table.py
+-rw-r--r--   0 81n      (42021) users      (100)     9433 2023-04-17 14:58:12.000000 icat-iml-0.1.1/icat/view.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:35:53.581402 icat-iml-0.1.1/icat_iml.egg-info/
+-rw-r--r--   0 81n      (42021) users      (100)     1115 2023-04-17 19:35:53.000000 icat-iml-0.1.1/icat_iml.egg-info/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)      547 2023-04-17 19:35:53.000000 icat-iml-0.1.1/icat_iml.egg-info/SOURCES.txt
+-rw-r--r--   0 81n      (42021) users      (100)        1 2023-04-17 19:35:53.000000 icat-iml-0.1.1/icat_iml.egg-info/dependency_links.txt
+-rw-r--r--   0 81n      (42021) users      (100)      103 2023-04-17 19:35:53.000000 icat-iml-0.1.1/icat_iml.egg-info/requires.txt
+-rw-r--r--   0 81n      (42021) users      (100)        5 2023-04-17 19:35:53.000000 icat-iml-0.1.1/icat_iml.egg-info/top_level.txt
+-rw-r--r--   0 81n      (42021) users      (100)       31 2023-04-17 14:58:06.000000 icat-iml-0.1.1/pyproject.toml
+-rw-r--r--   0 81n      (42021) users      (100)       38 2023-04-17 19:35:53.581402 icat-iml-0.1.1/setup.cfg
+-rw-r--r--   0 81n      (42021) users      (100)     1134 2023-04-17 19:24:04.000000 icat-iml-0.1.1/setup.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:35:53.581402 icat-iml-0.1.1/tests/
+-rw-r--r--   0 81n      (42021) users      (100)     6467 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_anchorlist.py
+-rw-r--r--   0 81n      (42021) users      (100)     9102 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_anchors.py
+-rw-r--r--   0 81n      (42021) users      (100)     3813 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_datamanager.py
+-rw-r--r--   0 81n      (42021) users      (100)     4099 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_histograms.py
+-rw-r--r--   0 81n      (42021) users      (100)     2522 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_instance.py
+-rw-r--r--   0 81n      (42021) users      (100)      374 2023-04-17 13:46:04.000000 icat-iml-0.1.1/tests/test_integrations.py
+-rw-r--r--   0 81n      (42021) users      (100)     9266 2023-04-17 14:58:07.000000 icat-iml-0.1.1/tests/test_model.py
+-rw-r--r--   0 81n      (42021) users      (100)     3885 2023-04-17 14:58:07.000000 icat-iml-0.1.1/tests/test_view.py
```

### Comparing `icat-iml-0.1.0/LICENSE` & `icat-iml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/anchorlist.py` & `icat-iml-0.1.1/icat/anchorlist.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/anchors.py` & `icat-iml-0.1.1/icat/anchors.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/data.py` & `icat-iml-0.1.1/icat/data.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/histogram.py` & `icat-iml-0.1.1/icat/histogram.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/histograms.py` & `icat-iml-0.1.1/icat/histograms.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/instance.py` & `icat-iml-0.1.1/icat/instance.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/model.py` & `icat-iml-0.1.1/icat/model.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/table.py` & `icat-iml-0.1.1/icat/table.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat/view.py` & `icat-iml-0.1.1/icat/view.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/icat_iml.egg-info/SOURCES.txt` & `icat-iml-0.1.1/icat_iml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/setup.py` & `icat-iml-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     python_requires=">=3.10",
     packages=["icat"],
     install_requires=[
         "panel~=0.14.4",
         "numpy~=1.23.4",
         "pandas~=1.5.1",
         "scikit-learn~=1.1.3",
+        "ipyvuetify~=1.8.4",
+        "ipywidgets<=8.0",
+        "altair",
     ],
 )
```

### Comparing `icat-iml-0.1.0/tests/test_anchorlist.py` & `icat-iml-0.1.1/tests/test_anchorlist.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_anchors.py` & `icat-iml-0.1.1/tests/test_anchors.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_datamanager.py` & `icat-iml-0.1.1/tests/test_datamanager.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_histograms.py` & `icat-iml-0.1.1/tests/test_histograms.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_instance.py` & `icat-iml-0.1.1/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_model.py` & `icat-iml-0.1.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.0/tests/test_view.py` & `icat-iml-0.1.1/tests/test_view.py`

 * *Files identical despite different names*

