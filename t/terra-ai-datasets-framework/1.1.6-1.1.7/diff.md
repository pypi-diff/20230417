# Comparing `tmp/terra_ai_datasets_framework-1.1.6.tar.gz` & `tmp/terra_ai_datasets_framework-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets_framework-1.1.6.tar", last modified: Fri Apr 14 16:13:33 2023, max compression
+gzip compressed data, was "terra_ai_datasets_framework-1.1.7.tar", last modified: Mon Apr 17 11:40:42 2023, max compression
```

## Comparing `terra_ai_datasets_framework-1.1.6.tar` & `terra_ai_datasets_framework-1.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets_framework-1.1.6/setup.py` & `terra_ai_datasets_framework-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
```

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/create.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/arrays.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                         if not use_generator or use_generator and put_data.type == LayerInputTypeChoice.Text:
                             col_array.append(
                                 sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                             )
 
                     if self.preprocessing.get(col_name) and split == "train":
                         if put_data.type == LayerInputTypeChoice.Text:
-                            if put_data.parameters.preprocessing != TextProcessTypes.word_to_vec:
+                            if put_data.parameters.preprocessing in [TextProcessTypes.embedding, TextProcessTypes.bag_of_words]:
                                 self.preprocessing[col_name].fit_on_texts(col_array)
 
                     if self.preprocessing.get(col_name) and not use_generator:
                         col_array = preprocess_put_array(
                             np.array(col_array), put_data, self.preprocessing[col_name]
                         )
                     if not use_generator:
```

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/utils.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/utils.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 # --- Text validators ---
 class TextModeTypes(str, Enum):
     full = "Full"
     length_and_step = "Length and step"
 
 
 class TextProcessTypes(str, Enum):
+    none = "None"
     embedding = "Embedding"
     bag_of_words = "Bag of words"
     word_to_vec = "Word2Vec"
 
 
 class TextValidator(BaseModel):
     filters: str = '–—!"#$%&()*+,-./:;<=>?@[\\]^«»№_`{|}~\t\n\xa0–\ufeff'
```

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/visualize.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/visualize.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/load.py` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/SOURCES.txt` & `terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/tests/test_classification.py` & `terra_ai_datasets_framework-1.1.7/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/tests/test_regression.py` & `terra_ai_datasets_framework-1.1.7/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/tests/test_segmentation.py` & `terra_ai_datasets_framework-1.1.7/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.6/tests/test_timeseries.py` & `terra_ai_datasets_framework-1.1.7/tests/test_timeseries.py`

 * *Files identical despite different names*

