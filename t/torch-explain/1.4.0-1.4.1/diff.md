# Comparing `tmp/torch_explain-1.4.0.tar.gz` & `tmp/torch_explain-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_explain-1.4.0.tar", last modified: Mon Mar 13 17:49:04 2023, max compression
+gzip compressed data, was "torch_explain-1.4.1.tar", last modified: Mon Apr 17 06:22:30 2023, max compression
```

## Comparing `torch_explain-1.4.0.tar` & `torch_explain-1.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.119108 torch_explain-1.4.0/
--rwxrwxrwx   0 root         (0) root         (0)    11558 2021-04-10 16:35:22.000000 torch_explain-1.4.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       26 2021-04-10 16:35:22.000000 torch_explain-1.4.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)    12553 2023-03-13 17:49:04.119318 torch_explain-1.4.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    11497 2023-03-13 17:45:04.000000 torch_explain-1.4.0/README.rst
--rwxrwxrwx   0 root         (0) root         (0)       48 2022-06-28 14:29:09.000000 torch_explain-1.4.0/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      148 2023-03-13 17:49:04.119832 torch_explain-1.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2235 2022-06-28 14:29:09.000000 torch_explain-1.4.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.109957 torch_explain-1.4.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-28 14:16:39.000000 torch_explain-1.4.0/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4737 2023-03-13 15:43:46.000000 torch_explain-1.4.0/tests/test_cem.py
--rwxrwxrwx   0 root         (0) root         (0)    11806 2023-03-13 16:15:13.000000 torch_explain-1.4.0/tests/test_logic_layer.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2023-03-13 15:55:57.000000 torch_explain-1.4.0/tests/test_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.110617 torch_explain-1.4.0/torch_explain/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-03-13 15:56:23.000000 torch_explain-1.4.0/torch_explain/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-03-13 17:47:46.000000 torch_explain-1.4.0/torch_explain/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.113911 torch_explain-1.4.0/torch_explain/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      104 2023-03-13 14:44:06.000000 torch_explain-1.4.0/torch_explain/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1712 2023-03-13 15:20:42.000000 torch_explain-1.4.0/torch_explain/datasets/benchmarks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.115365 torch_explain-1.4.0/torch_explain/logic/
--rwxrwxrwx   0 root         (0) root         (0)      370 2023-03-13 16:08:55.000000 torch_explain-1.4.0/torch_explain/logic/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6048 2023-03-13 16:11:08.000000 torch_explain-1.4.0/torch_explain/logic/metrics.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.116794 torch_explain-1.4.0/torch_explain/logic/nn/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 07:06:23.000000 torch_explain-1.4.0/torch_explain/logic/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21037 2023-03-13 16:04:06.000000 torch_explain-1.4.0/torch_explain/logic/nn/entropy.py
--rwxrwxrwx   0 root         (0) root         (0)    11038 2021-06-23 07:41:49.000000 torch_explain-1.4.0/torch_explain/logic/nn/psi.py
--rwxrwxrwx   0 root         (0) root         (0)     1052 2023-03-13 16:06:44.000000 torch_explain-1.4.0/torch_explain/logic/nn/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     3251 2023-03-13 15:54:45.000000 torch_explain-1.4.0/torch_explain/logic/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.117898 torch_explain-1.4.0/torch_explain/nn/
--rwxrwxrwx   0 root         (0) root         (0)      184 2023-03-13 15:26:10.000000 torch_explain-1.4.0/torch_explain/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3669 2023-03-13 15:36:41.000000 torch_explain-1.4.0/torch_explain/nn/concepts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.118825 torch_explain-1.4.0/torch_explain/nn/functional/
--rwxrwxrwx   0 root         (0) root         (0)      172 2021-06-23 07:23:21.000000 torch_explain-1.4.0/torch_explain/nn/functional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      848 2022-05-31 08:15:20.000000 torch_explain-1.4.0/torch_explain/nn/functional/loss.py
--rwxrwxrwx   0 root         (0) root         (0)     1356 2021-06-23 07:26:08.000000 torch_explain-1.4.0/torch_explain/nn/functional/prune.py
--rwxrwxrwx   0 root         (0) root         (0)     2351 2023-03-13 15:50:39.000000 torch_explain-1.4.0/torch_explain/nn/logic.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-13 17:49:04.113151 torch_explain-1.4.0/torch_explain.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    12553 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      912 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      138 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-03-13 17:49:04.000000 torch_explain-1.4.0/torch_explain.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.189907 torch_explain-1.4.1/
+-rwxrwxrwx   0 root         (0) root         (0)    11558 2021-04-10 16:35:22.000000 torch_explain-1.4.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       26 2021-04-10 16:35:22.000000 torch_explain-1.4.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)    12554 2023-04-17 06:22:30.190182 torch_explain-1.4.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    11497 2023-03-13 17:45:04.000000 torch_explain-1.4.1/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)       48 2022-06-28 14:29:09.000000 torch_explain-1.4.1/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      148 2023-04-17 06:22:30.190884 torch_explain-1.4.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2236 2023-03-13 18:00:22.000000 torch_explain-1.4.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.176680 torch_explain-1.4.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-28 14:16:39.000000 torch_explain-1.4.1/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4737 2023-03-13 15:43:46.000000 torch_explain-1.4.1/tests/test_cem.py
+-rwxrwxrwx   0 root         (0) root         (0)    11806 2023-03-13 16:15:13.000000 torch_explain-1.4.1/tests/test_logic_layer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2023-03-13 15:55:57.000000 torch_explain-1.4.1/tests/test_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.177728 torch_explain-1.4.1/torch_explain/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-03-13 15:56:23.000000 torch_explain-1.4.1/torch_explain/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-17 06:22:07.000000 torch_explain-1.4.1/torch_explain/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.181007 torch_explain-1.4.1/torch_explain/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-03-13 14:44:06.000000 torch_explain-1.4.1/torch_explain/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1712 2023-03-13 15:20:42.000000 torch_explain-1.4.1/torch_explain/datasets/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.182666 torch_explain-1.4.1/torch_explain/logic/
+-rwxrwxrwx   0 root         (0) root         (0)      370 2023-03-13 16:08:55.000000 torch_explain-1.4.1/torch_explain/logic/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6048 2023-03-13 16:11:08.000000 torch_explain-1.4.1/torch_explain/logic/metrics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.185199 torch_explain-1.4.1/torch_explain/logic/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 07:06:23.000000 torch_explain-1.4.1/torch_explain/logic/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21093 2023-04-17 06:20:19.000000 torch_explain-1.4.1/torch_explain/logic/nn/entropy.py
+-rwxrwxrwx   0 root         (0) root         (0)    11038 2021-06-23 07:41:49.000000 torch_explain-1.4.1/torch_explain/logic/nn/psi.py
+-rwxrwxrwx   0 root         (0) root         (0)     1052 2023-03-13 16:06:44.000000 torch_explain-1.4.1/torch_explain/logic/nn/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3251 2023-03-13 15:54:45.000000 torch_explain-1.4.1/torch_explain/logic/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.187107 torch_explain-1.4.1/torch_explain/nn/
+-rwxrwxrwx   0 root         (0) root         (0)      184 2023-03-13 15:26:10.000000 torch_explain-1.4.1/torch_explain/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3669 2023-03-13 15:36:41.000000 torch_explain-1.4.1/torch_explain/nn/concepts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.189300 torch_explain-1.4.1/torch_explain/nn/functional/
+-rwxrwxrwx   0 root         (0) root         (0)      172 2021-06-23 07:23:21.000000 torch_explain-1.4.1/torch_explain/nn/functional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      848 2022-05-31 08:15:20.000000 torch_explain-1.4.1/torch_explain/nn/functional/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)     1356 2021-06-23 07:26:08.000000 torch_explain-1.4.1/torch_explain/nn/functional/prune.py
+-rwxrwxrwx   0 root         (0) root         (0)     2351 2023-03-13 15:50:39.000000 torch_explain-1.4.1/torch_explain/nn/logic.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.180154 torch_explain-1.4.1/torch_explain.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    12554 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      912 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      138 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/top_level.txt
```

### Comparing `torch_explain-1.4.0/LICENSE` & `torch_explain-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/PKG-INFO` & `torch_explain-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torch_explain
-Version: 1.4.0
-Summary: PyTorch Explain: Logic Explained Networks in Python.
+Version: 1.4.1
+Summary: PyTorch Explain: Explainable Deep Learning in Python.
 Home-page: https://github.com/pietrobarbiero/pytorch_explain
 Download-URL: https://github.com/pietrobarbiero/pytorch_explain
 Maintainer: P. Barbiero
 Maintainer-email: barbiero@tutanota.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `torch_explain-1.4.0/README.rst` & `torch_explain-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/setup.py` & `torch_explain-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # get __version__ from _version.py
 ver_file = os.path.join('torch_explain', '_version.py')
 with open(ver_file) as f:
     exec(f.read())
 
 DISTNAME = 'torch_explain'
-DESCRIPTION = 'PyTorch Explain: Logic Explained Networks in Python.'
+DESCRIPTION = 'PyTorch Explain: Explainable Deep Learning in Python.'
 with codecs.open('README.rst') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'P. Barbiero'
 MAINTAINER_EMAIL = 'barbiero@tutanota.com'
 URL = 'https://github.com/pietrobarbiero/pytorch_explain'
 LICENSE = 'Apache 2.0'
 DOWNLOAD_URL = 'https://github.com/pietrobarbiero/pytorch_explain'
```

### Comparing `torch_explain-1.4.0/tests/test_cem.py` & `torch_explain-1.4.1/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/tests/test_logic_layer.py` & `torch_explain-1.4.1/tests/test_logic_layer.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/tests/test_utils.py` & `torch_explain-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/datasets/benchmarks.py` & `torch_explain-1.4.1/torch_explain/datasets/benchmarks.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/logic/metrics.py` & `torch_explain-1.4.1/torch_explain/logic/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/logic/nn/entropy.py` & `torch_explain-1.4.1/torch_explain/logic/nn/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
     if train_mask is None:
         train_mask = torch.arange(len(c))
 
     if val_mask is None:
         val_mask = train_mask
 
+    if test_mask is None:
+        test_mask = val_mask
+
     explanations = {}
     local_explanations = {}
     for class_id in range(y.shape[1]):
         explanation, local_explanations_raw = explain_class(model, c, y, train_mask, val_mask, target_class=class_id,
                                                             edge_index=edge_index,
                                                             max_minterm_complexity=max_minterm_complexity,
                                                             topk_explanations=topk_explanations, try_all=try_all,
```

### Comparing `torch_explain-1.4.0/torch_explain/logic/nn/psi.py` & `torch_explain-1.4.1/torch_explain/logic/nn/psi.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/logic/nn/utils.py` & `torch_explain-1.4.1/torch_explain/logic/nn/utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/logic/utils.py` & `torch_explain-1.4.1/torch_explain/logic/utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/nn/concepts.py` & `torch_explain-1.4.1/torch_explain/nn/concepts.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/nn/functional/loss.py` & `torch_explain-1.4.1/torch_explain/nn/functional/loss.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/nn/functional/prune.py` & `torch_explain-1.4.1/torch_explain/nn/functional/prune.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain/nn/logic.py` & `torch_explain-1.4.1/torch_explain/nn/logic.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.0/torch_explain.egg-info/PKG-INFO` & `torch_explain-1.4.1/torch_explain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torch-explain
-Version: 1.4.0
-Summary: PyTorch Explain: Logic Explained Networks in Python.
+Version: 1.4.1
+Summary: PyTorch Explain: Explainable Deep Learning in Python.
 Home-page: https://github.com/pietrobarbiero/pytorch_explain
 Download-URL: https://github.com/pietrobarbiero/pytorch_explain
 Maintainer: P. Barbiero
 Maintainer-email: barbiero@tutanota.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `torch_explain-1.4.0/torch_explain.egg-info/SOURCES.txt` & `torch_explain-1.4.1/torch_explain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

