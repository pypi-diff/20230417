# Comparing `tmp/rexify-0.1.8.tar.gz` & `tmp/rexify-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rexify-0.1.8.tar", max compression
+gzip compressed data, was "rexify-0.1.9.tar", max compression
```

## Comparing `rexify-0.1.8.tar` & `rexify-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1071 2023-04-08 22:33:31.072963 rexify-0.1.8/LICENSE
--rw-r--r--   0        0        0     4845 2023-04-08 22:33:31.072963 rexify-0.1.8/README.md
--rw-r--r--   0        0        0     2831 2023-04-08 22:33:33.200977 rexify-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      136 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/__init__.py
--rw-r--r--   0        0        0     3754 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/data.py
--rw-r--r--   0        0        0        0 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/__init__.py
--rw-r--r--   0        0        0     2565 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/base.py
--rw-r--r--   0        0        0     4165 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/extractor.py
--rw-r--r--   0        0        0      206 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/__init__.py
--rw-r--r--   0        0        0      399 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/category.py
--rw-r--r--   0        0        0      346 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/custom.py
--rw-r--r--   0        0        0     3988 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/entity.py
--rw-r--r--   0        0        0     1130 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/event.py
--rw-r--r--   0        0        0     1809 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/id.py
--rw-r--r--   0        0        0      402 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/number.py
--rw-r--r--   0        0        0     4398 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/features/transform/sequence.py
--rw-r--r--   0        0        0       37 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/__init__.py
--rw-r--r--   0        0        0      807 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/base.py
--rw-r--r--   0        0        0       38 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/callbacks/__init__.py
--rw-r--r--   0        0        0     1310 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/callbacks/index.py
--rw-r--r--   0        0        0      721 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/index.py
--rw-r--r--   0        0        0     1358 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/lookup.py
--rw-r--r--   0        0        0       34 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/ranking/__init__.py
--rw-r--r--   0        0        0      624 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/ranking/base.py
--rw-r--r--   0        0        0      619 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/ranking/event.py
--rw-r--r--   0        0        0     1778 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/ranking/ranking.py
--rw-r--r--   0        0        0     4957 2023-04-08 22:33:31.072963 rexify-0.1.8/rexify/models/recommender.py
--rw-r--r--   0        0        0       38 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/retrieval/__init__.py
--rw-r--r--   0        0        0     1838 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/retrieval/candidate.py
--rw-r--r--   0        0        0     3032 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/retrieval/query.py
--rw-r--r--   0        0        0     2131 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/retrieval/retrieval.py
--rw-r--r--   0        0        0     2293 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/retrieval/tower.py
--rw-r--r--   0        0        0     2011 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/models/sequential.py
--rw-r--r--   0        0        0     2686 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/schema.py
--rw-r--r--   0        0        0      676 2023-04-08 22:33:31.076963 rexify-0.1.8/rexify/utils.py
--rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 rexify-0.1.8/setup.py
--rw-r--r--   0        0        0     6528 1970-01-01 00:00:00.000000 rexify-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-17 15:12:58.348973 rexify-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4845 2023-04-17 15:12:58.348973 rexify-0.1.9/README.md
+-rw-r--r--   0        0        0     2831 2023-04-17 15:13:01.236965 rexify-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      136 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/__init__.py
+-rw-r--r--   0        0        0     3754 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/data.py
+-rw-r--r--   0        0        0        0 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/__init__.py
+-rw-r--r--   0        0        0     2565 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/base.py
+-rw-r--r--   0        0        0     4282 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/extractor.py
+-rw-r--r--   0        0        0      206 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/category.py
+-rw-r--r--   0        0        0      346 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/custom.py
+-rw-r--r--   0        0        0     3988 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/entity.py
+-rw-r--r--   0        0        0     1130 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/event.py
+-rw-r--r--   0        0        0     1809 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/id.py
+-rw-r--r--   0        0        0      402 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/number.py
+-rw-r--r--   0        0        0     4398 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/features/transform/sequence.py
+-rw-r--r--   0        0        0       37 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/base.py
+-rw-r--r--   0        0        0       38 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/callbacks/__init__.py
+-rw-r--r--   0        0        0     1310 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/callbacks/index.py
+-rw-r--r--   0        0        0      721 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/index.py
+-rw-r--r--   0        0        0     1358 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/lookup.py
+-rw-r--r--   0        0        0       34 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/ranking/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/ranking/base.py
+-rw-r--r--   0        0        0      619 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/ranking/event.py
+-rw-r--r--   0        0        0     1778 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/ranking/ranking.py
+-rw-r--r--   0        0        0     5076 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/recommender.py
+-rw-r--r--   0        0        0       38 2023-04-17 15:12:58.348973 rexify-0.1.9/rexify/models/retrieval/__init__.py
+-rw-r--r--   0        0        0     1838 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/models/retrieval/candidate.py
+-rw-r--r--   0        0        0     3032 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/models/retrieval/query.py
+-rw-r--r--   0        0        0     2131 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/models/retrieval/retrieval.py
+-rw-r--r--   0        0        0     2293 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/models/retrieval/tower.py
+-rw-r--r--   0        0        0     2011 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/models/sequential.py
+-rw-r--r--   0        0        0     2686 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/schema.py
+-rw-r--r--   0        0        0      676 2023-04-17 15:12:58.352973 rexify-0.1.9/rexify/utils.py
+-rw-r--r--   0        0        0     6528 1970-01-01 00:00:00.000000 rexify-0.1.9/PKG-INFO
```

### Comparing `rexify-0.1.8/LICENSE` & `rexify-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/README.md` & `rexify-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/pyproject.toml` & `rexify-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rexify"
-version = "0.1.8"
+version = "0.1.9"
 description = "Streamlined Recommender System workflows with TensorFlow and Kubeflow"
 authors = ["José Medeiros <joseprsm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rexify.readthedocs.io"
 packages = [{ include = "rexify" }]
 classifiers = [
```

### Comparing `rexify-0.1.8/rexify/data.py` & `rexify-0.1.9/rexify/data.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/features/base.py` & `rexify-0.1.9/rexify/features/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/features/extractor.py` & `rexify-0.1.9/rexify/features/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,18 +100,14 @@
         return self._users
 
     @property
     def items(self):
         return self._items
 
     @property
-    def load_fn(self):
-        return self._load_fn
-
-    @property
     def model_params(self):
         return self._model_params
 
     @property
     def ranking_features(self):
         return self._ppl.steps[0][1].ranking_features
 
@@ -126,7 +122,15 @@
     @property
     def window_size(self):
         return self._window_size
 
     @property
     def custom_transformers(self):
         return self._custom_transformers
+
+    @property
+    def item_encoder(self):
+        return self._item_transformer.encoder[0]
+
+    @property
+    def user_encoder(self):
+        return self._user_transformer.encoder[0]
```

### Comparing `rexify-0.1.8/rexify/features/transform/entity.py` & `rexify-0.1.9/rexify/features/transform/entity.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/features/transform/event.py` & `rexify-0.1.9/rexify/features/transform/event.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/features/transform/id.py` & `rexify-0.1.9/rexify/features/transform/id.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/features/transform/sequence.py` & `rexify-0.1.9/rexify/features/transform/sequence.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/base.py` & `rexify-0.1.9/rexify/models/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/callbacks/index.py` & `rexify-0.1.9/rexify/models/callbacks/index.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/index.py` & `rexify-0.1.9/rexify/models/index.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/lookup.py` & `rexify-0.1.9/rexify/models/lookup.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/ranking/base.py` & `rexify-0.1.9/rexify/models/ranking/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/ranking/event.py` & `rexify-0.1.9/rexify/models/ranking/event.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/ranking/ranking.py` & `rexify-0.1.9/rexify/models/ranking/ranking.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/recommender.py` & `rexify-0.1.9/rexify/models/recommender.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,7 +117,11 @@
             "user_dims": self._user_dims,
             "output_layers": self._output_layers,
             "feature_layers": self._feature_layers,
             "ranking_layers": self._ranking_layers,
             "ranking_features": self._ranking_features,
             "ranking_weights": self._ranking_weights,
         }
+
+    @classmethod
+    def load(cls, export_dir: str) -> tf.keras.Model:
+        return tf.saved_model.load(export_dir)
```

### Comparing `rexify-0.1.8/rexify/models/retrieval/candidate.py` & `rexify-0.1.9/rexify/models/retrieval/candidate.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/retrieval/query.py` & `rexify-0.1.9/rexify/models/retrieval/query.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/retrieval/retrieval.py` & `rexify-0.1.9/rexify/models/retrieval/retrieval.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/retrieval/tower.py` & `rexify-0.1.9/rexify/models/retrieval/tower.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/models/sequential.py` & `rexify-0.1.9/rexify/models/sequential.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/schema.py` & `rexify-0.1.9/rexify/schema.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/rexify/utils.py` & `rexify-0.1.9/rexify/utils.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.8/setup.py` & `rexify-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['rexify',
- 'rexify.features',
- 'rexify.features.transform',
- 'rexify.models',
- 'rexify.models.callbacks',
- 'rexify.models.ranking',
- 'rexify.models.retrieval']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['kfp>=1.8.0,<2.0.0',
- 'numpy>=1.22.3',
- 'pandas>=1.4.0,<2.0.0',
- 'scikit-learn>=1.0.0,<2.0.0',
- 'tensorflow_recommenders>=0.7.2']
-
-extras_require = \
-{':sys_platform != "darwin"': ['tensorflow==2.9.0', 'scann>=1.2.0,<2.0.0'],
- ':sys_platform == "darwin"': ['tensorflow_metal==0.5.0',
-                               'tensorflow_macos==2.9.0']}
-
-setup_kwargs = {
-    'name': 'rexify',
-    'version': '0.1.8',
-    'description': 'Streamlined Recommender System workflows with TensorFlow and Kubeflow',
-    'long_description': '<p align="center">\n    <br>\n    <img src="https://storage.googleapis.com/rexify/1659986918545.png" height="200"/>\n    <br>\n<p>\n\n<p align="center">\n    <a href="https://circleci.com/gh/joseprsm/rexify">\n        <img alt="Build" src="https://img.shields.io/circleci/build/github/joseprsm/rexify?style=flat-square">\n    </a>\n    <a href="https://github.com/joseprsm/rexify/blob/main/LICENSE">\n        <img alt="License" src="https://img.shields.io/github/license/joseprsm/rexify?style=flat-square">\n    </a>\n    <a href="https://rexify.readthedocs.io">\n        <img alt="Documentation" src="https://img.shields.io/badge/documentation-online-success?style=flat-square">\n    </a>\n    <a href="https://pypi.org/project/rexify/">\n        <img alt="GitHub release" src="https://img.shields.io/github/v/release/joseprsm/rexify?style=flat-square">\n    </a>\n</p>\n\nRexify is a library to streamline recommender systems model development.\n\nIn essence, Rexify adapts dynamically to your data, and outputs high-performing TensorFlow\nmodels that may be used wherever you want, independently of your data. Rexify also includes\nmodules to deal with feature engineering as Scikit-Learn Transformers and Pipelines.\n\nWith Rexify, users may easily train Recommender Systems models, just by specifying what their\ndata looks like. Rexify also comes equipped with pre-built machine learning pipelines which can\nbe used serverlessly. \n\n## What is Rexify?\n\nRexify is a low-code personalization tool, that makes use of traditional machine learning \nframeworks, such as Scikit-Learn and TensorFlow, to create scalable Recommender Systems\nworkflows that anyone can use.\n\n### Who is it for?\n\nRexify is a project that simplifies and standardizes the workflow of recommender systems. It is \nmostly geared towards people with little to no machine learning knowledge, that want to implement\nsomewhat scalable Recommender Systems in their applications.\n\n## Installation\n\nThe easiest way to install Rexify is via `pip`:\n\n```shell\npip install rexify\n```\n\n## Quick Tour\n\nRexify is meant to be usable right out of the box. All you need to set up your model is interaction\ndata - something that kind of looks like this:\n\n| user_id | item_id | timestamp  | event_type  |\n|---------|---------|------------|-------------|\n| 22      | 67      | 2021/05/13 | Purchase    |\n| 37      | 9       | 2021/04/11 | Page View   |\n| 22      | 473     | 2021/04/11 | Add to Cart |\n| ...     | ...     | ...        | ...         |\n| 358     | 51      | 2021/04/11 | Purchase    |\n\nAdditionally, we\'ll have to have configured a schema for the data.\nThis schema is what will allow Rexify to generate a dynamic model and preprocessing steps.\nThe schema should be comprised of two dictionaries (`user`, `ìtem`) and two key-value \npairs: `event_type` (which should point to the column of the event type) and `timestamp` (\nwhich should point to the timestamp column)\n\nEach of these dictionaries should consist of features and internal data types, \nsuch as: `id`, `category`, `number`. More data types will be available \nin the future.\n\n```json\n{\n  "user": {\n    "user_id": "id",\n    "age": "number"\n  },\n  "item": {\n    "item_id": "id",\n    "category": "category"\n  },\n  "timestamp": "timestamp"\n  "event_type": "event_type"\n}\n```\n\nEssentially, what Rexify will do is take the schema, and dynamically adapt to the data.\n\nThere are two main components in Rexify workflows: `FeatureExtractor` and `Recommender`.\n\nThe `FeatureExtractor` is a scikit-learn Transformer that basically takes the schema of \nthe data, and transforms the event data accordingly. Another method `.make_dataset()`, \nconverts the transformed data into a `tf.data.Dataset`, all correctly configured to be fed\nto the `Recommender` model.\n\n`Recommender` is a `tfrs.Model` that basically implements the Query and Candidate towers. \nDuring training, the Query tower will take the user ID, user features, and context, to \nlearn an embedding; the Candidate tower will do the same for the item ID and its features. \n\nMore information about how the `FeatureExtractor` and the `Recommender` works can be found \n[here](https://rexify.readthedocs.io/en/latest/overview/architecture.html). \n\nA sample Rexify workflow should sort of look like this:\n\n````python\n\nimport pandas as pd\n\nfrom rexify import Schema, FeatureExtractor, Recommender\n\nevents = pd.read_csv(\'path/to/events/data\')\n\nschema = Schema.load(\'path/to/schema\')\n\nfeat = FeatureExtractor(schema, users=\'path/to/users/data\', items=\'path/to/events/data\')\nx = feat.fit_transform(events)\nx = feat.make_dataset(x)\n\nmodel = Recommender(**feat.model_params)\nmodel.compile()\nmodel.fit(events, batch_size=512)\n````\n\nWhen training is complete, you\'ll have a trained `tf.keras.Model` ready to be used, as\nyou normally would. \n\n## License\n\n[MIT](https://github.com/joseprsm/rexify/blob/main/LICENSE)\n',
-    'author': 'José Medeiros',
-    'author_email': 'joseprsm@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.11',
+Metadata-Version: 2.1
+Name: rexify
+Version: 0.1.9
+Summary: Streamlined Recommender System workflows with TensorFlow and Kubeflow
+License: MIT
+Author: José Medeiros
+Author-email: joseprsm@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: kfp (>=1.8.0,<2.0.0)
+Requires-Dist: numpy (>=1.22.3)
+Requires-Dist: pandas (>=1.4.0,<2.0.0)
+Requires-Dist: scann (>=1.2.0,<2.0.0) ; sys_platform != "darwin"
+Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
+Requires-Dist: tensorflow (==2.9.0) ; sys_platform != "darwin"
+Requires-Dist: tensorflow_macos (==2.9.0) ; sys_platform == "darwin"
+Requires-Dist: tensorflow_metal (==0.5.0) ; sys_platform == "darwin"
+Requires-Dist: tensorflow_recommenders (>=0.7.2)
+Project-URL: Documentation, https://rexify.readthedocs.io
+Description-Content-Type: text/markdown
+
+<p align="center">
+    <br>
+    <img src="https://storage.googleapis.com/rexify/1659986918545.png" height="200"/>
+    <br>
+<p>
+
+<p align="center">
+    <a href="https://circleci.com/gh/joseprsm/rexify">
+        <img alt="Build" src="https://img.shields.io/circleci/build/github/joseprsm/rexify?style=flat-square">
+    </a>
+    <a href="https://github.com/joseprsm/rexify/blob/main/LICENSE">
+        <img alt="License" src="https://img.shields.io/github/license/joseprsm/rexify?style=flat-square">
+    </a>
+    <a href="https://rexify.readthedocs.io">
+        <img alt="Documentation" src="https://img.shields.io/badge/documentation-online-success?style=flat-square">
+    </a>
+    <a href="https://pypi.org/project/rexify/">
+        <img alt="GitHub release" src="https://img.shields.io/github/v/release/joseprsm/rexify?style=flat-square">
+    </a>
+</p>
+
+Rexify is a library to streamline recommender systems model development.
+
+In essence, Rexify adapts dynamically to your data, and outputs high-performing TensorFlow
+models that may be used wherever you want, independently of your data. Rexify also includes
+modules to deal with feature engineering as Scikit-Learn Transformers and Pipelines.
+
+With Rexify, users may easily train Recommender Systems models, just by specifying what their
+data looks like. Rexify also comes equipped with pre-built machine learning pipelines which can
+be used serverlessly. 
+
+## What is Rexify?
+
+Rexify is a low-code personalization tool, that makes use of traditional machine learning 
+frameworks, such as Scikit-Learn and TensorFlow, to create scalable Recommender Systems
+workflows that anyone can use.
+
+### Who is it for?
+
+Rexify is a project that simplifies and standardizes the workflow of recommender systems. It is 
+mostly geared towards people with little to no machine learning knowledge, that want to implement
+somewhat scalable Recommender Systems in their applications.
+
+## Installation
+
+The easiest way to install Rexify is via `pip`:
+
+```shell
+pip install rexify
+```
+
+## Quick Tour
+
+Rexify is meant to be usable right out of the box. All you need to set up your model is interaction
+data - something that kind of looks like this:
+
+| user_id | item_id | timestamp  | event_type  |
+|---------|---------|------------|-------------|
+| 22      | 67      | 2021/05/13 | Purchase    |
+| 37      | 9       | 2021/04/11 | Page View   |
+| 22      | 473     | 2021/04/11 | Add to Cart |
+| ...     | ...     | ...        | ...         |
+| 358     | 51      | 2021/04/11 | Purchase    |
+
+Additionally, we'll have to have configured a schema for the data.
+This schema is what will allow Rexify to generate a dynamic model and preprocessing steps.
+The schema should be comprised of two dictionaries (`user`, `ìtem`) and two key-value 
+pairs: `event_type` (which should point to the column of the event type) and `timestamp` (
+which should point to the timestamp column)
+
+Each of these dictionaries should consist of features and internal data types, 
+such as: `id`, `category`, `number`. More data types will be available 
+in the future.
+
+```json
+{
+  "user": {
+    "user_id": "id",
+    "age": "number"
+  },
+  "item": {
+    "item_id": "id",
+    "category": "category"
+  },
+  "timestamp": "timestamp"
+  "event_type": "event_type"
 }
+```
+
+Essentially, what Rexify will do is take the schema, and dynamically adapt to the data.
+
+There are two main components in Rexify workflows: `FeatureExtractor` and `Recommender`.
+
+The `FeatureExtractor` is a scikit-learn Transformer that basically takes the schema of 
+the data, and transforms the event data accordingly. Another method `.make_dataset()`, 
+converts the transformed data into a `tf.data.Dataset`, all correctly configured to be fed
+to the `Recommender` model.
+
+`Recommender` is a `tfrs.Model` that basically implements the Query and Candidate towers. 
+During training, the Query tower will take the user ID, user features, and context, to 
+learn an embedding; the Candidate tower will do the same for the item ID and its features. 
+
+More information about how the `FeatureExtractor` and the `Recommender` works can be found 
+[here](https://rexify.readthedocs.io/en/latest/overview/architecture.html). 
+
+A sample Rexify workflow should sort of look like this:
+
+````python
+
+import pandas as pd
+
+from rexify import Schema, FeatureExtractor, Recommender
+
+events = pd.read_csv('path/to/events/data')
+
+schema = Schema.load('path/to/schema')
+
+feat = FeatureExtractor(schema, users='path/to/users/data', items='path/to/events/data')
+x = feat.fit_transform(events)
+x = feat.make_dataset(x)
+
+model = Recommender(**feat.model_params)
+model.compile()
+model.fit(events, batch_size=512)
+````
+
+When training is complete, you'll have a trained `tf.keras.Model` ready to be used, as
+you normally would. 
+
+## License
 
+[MIT](https://github.com/joseprsm/rexify/blob/main/LICENSE)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,76 +1,77 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['rexify',
-'rexify.features', 'rexify.features.transform', 'rexify.models',
-'rexify.models.callbacks', 'rexify.models.ranking', 'rexify.models.retrieval']
-package_data = \ {'': ['*']} install_requires = \ ['kfp>=1.8.0,<2.0.0',
-'numpy>=1.22.3', 'pandas>=1.4.0,<2.0.0', 'scikit-learn>=1.0.0,<2.0.0',
-'tensorflow_recommenders>=0.7.2'] extras_require = \ {':sys_platform !=
-"darwin"': ['tensorflow==2.9.0', 'scann>=1.2.0,<2.0.0'], ':sys_platform ==
-"darwin"': ['tensorflow_metal==0.5.0', 'tensorflow_macos==2.9.0']} setup_kwargs
-= { 'name': 'rexify', 'version': '0.1.8', 'description': 'Streamlined
-Recommender System workflows with TensorFlow and Kubeflow', 'long_description':
-'
-                                      \n
-        \n [https://storage.googleapis.com/rexify/1659986918545.png]\n
-                                      \n
-\n\n
-     \n \n_[Build]\n\n \n_[License]\n\n \n_[Documentation]\n\n \n_[GitHub
-                                 release]\n\n
-\n\nRexify is a library to streamline recommender systems model
-development.\n\nIn essence, Rexify adapts dynamically to your data, and outputs
-high-performing TensorFlow\nmodels that may be used wherever you want,
-independently of your data. Rexify also includes\nmodules to deal with feature
-engineering as Scikit-Learn Transformers and Pipelines.\n\nWith Rexify, users
-may easily train Recommender Systems models, just by specifying what
-their\ndata looks like. Rexify also comes equipped with pre-built machine
-learning pipelines which can\nbe used serverlessly. \n\n## What is
-Rexify?\n\nRexify is a low-code personalization tool, that makes use of
-traditional machine learning \nframeworks, such as Scikit-Learn and TensorFlow,
-to create scalable Recommender Systems\nworkflows that anyone can use.\n\n###
-Who is it for?\n\nRexify is a project that simplifies and standardizes the
-workflow of recommender systems. It is \nmostly geared towards people with
-little to no machine learning knowledge, that want to implement\nsomewhat
-scalable Recommender Systems in their applications.\n\n## Installation\n\nThe
-easiest way to install Rexify is via `pip`:\n\n```shell\npip install
-rexify\n```\n\n## Quick Tour\n\nRexify is meant to be usable right out of the
-box. All you need to set up your model is interaction\ndata - something that
-kind of looks like this:\n\n| user_id | item_id | timestamp | event_type |\n|--
--------|---------|------------|-------------|\n| 22 | 67 | 2021/05/13 |
-Purchase |\n| 37 | 9 | 2021/04/11 | Page View |\n| 22 | 473 | 2021/04/11 | Add
-to Cart |\n| ... | ... | ... | ... |\n| 358 | 51 | 2021/04/11 | Purchase
-|\n\nAdditionally, we\'ll have to have configured a schema for the data.\nThis
-schema is what will allow Rexify to generate a dynamic model and preprocessing
-steps.\nThe schema should be comprised of two dictionaries (`user`, `Ã¬tem`)
-and two key-value \npairs: `event_type` (which should point to the column of
-the event type) and `timestamp` (\nwhich should point to the timestamp
-column)\n\nEach of these dictionaries should consist of features and internal
-data types, \nsuch as: `id`, `category`, `number`. More data types will be
-available \nin the future.\n\n```json\n{\n "user": {\n "user_id": "id",\n
-"age": "number"\n },\n "item": {\n "item_id": "id",\n "category": "category"\n
-},\n "timestamp": "timestamp"\n "event_type":
-"event_type"\n}\n```\n\nEssentially, what Rexify will do is take the schema,
-and dynamically adapt to the data.\n\nThere are two main components in Rexify
-workflows: `FeatureExtractor` and `Recommender`.\n\nThe `FeatureExtractor` is a
-scikit-learn Transformer that basically takes the schema of \nthe data, and
-transforms the event data accordingly. Another method `.make_dataset()`,
-\nconverts the transformed data into a `tf.data.Dataset`, all correctly
-configured to be fed\nto the `Recommender` model.\n\n`Recommender` is a
-`tfrs.Model` that basically implements the Query and Candidate towers. \nDuring
-training, the Query tower will take the user ID, user features, and context, to
-\nlearn an embedding; the Candidate tower will do the same for the item ID and
-its features. \n\nMore information about how the `FeatureExtractor` and the
-`Recommender` works can be found \n[here](https://rexify.readthedocs.io/en/
-latest/overview/architecture.html). \n\nA sample Rexify workflow should sort of
-look like this:\n\n````python\n\nimport pandas as pd\n\nfrom rexify import
-Schema, FeatureExtractor, Recommender\n\nevents = pd.read_csv(\'path/to/events/
-data\')\n\nschema = Schema.load(\'path/to/schema\')\n\nfeat = FeatureExtractor
-(schema, users=\'path/to/users/data\', items=\'path/to/events/data\')\nx =
-feat.fit_transform(events)\nx = feat.make_dataset(x)\n\nmodel = Recommender
-(**feat.model_params)\nmodel.compile()\nmodel.fit(events,
-batch_size=512)\n````\n\nWhen training is complete, you\'ll have a trained
-`tf.keras.Model` ready to be used, as\nyou normally would. \n\n## License\n\n
-[MIT](https://github.com/joseprsm/rexify/blob/main/LICENSE)\n', 'author':
-'JosÃ© Medeiros', 'author_email': 'joseprsm@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'python_requires': '>=3.8,<3.11', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: rexify Version: 0.1.9 Summary: Streamlined
+Recommender System workflows with TensorFlow and Kubeflow License: MIT Author:
+JosÃ© Medeiros Author-email: joseprsm@gmail.com Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Dist: kfp
+(>=1.8.0,<2.0.0) Requires-Dist: numpy (>=1.22.3) Requires-Dist: pandas
+(>=1.4.0,<2.0.0) Requires-Dist: scann (>=1.2.0,<2.0.0) ; sys_platform !=
+"darwin" Requires-Dist: scikit-learn (>=1.0.0,<2.0.0) Requires-Dist: tensorflow
+(==2.9.0) ; sys_platform != "darwin" Requires-Dist: tensorflow_macos (==2.9.0)
+; sys_platform == "darwin" Requires-Dist: tensorflow_metal (==0.5.0) ;
+sys_platform == "darwin" Requires-Dist: tensorflow_recommenders (>=0.7.2)
+Project-URL: Documentation, https://rexify.readthedocs.io Description-Content-
+Type: text/markdown
+
+          [https://storage.googleapis.com/rexify/1659986918545.png]
+              [Build] [License] [Documentation] [GitHub_release]
+Rexify is a library to streamline recommender systems model development. In
+essence, Rexify adapts dynamically to your data, and outputs high-performing
+TensorFlow models that may be used wherever you want, independently of your
+data. Rexify also includes modules to deal with feature engineering as Scikit-
+Learn Transformers and Pipelines. With Rexify, users may easily train
+Recommender Systems models, just by specifying what their data looks like.
+Rexify also comes equipped with pre-built machine learning pipelines which can
+be used serverlessly. ## What is Rexify? Rexify is a low-code personalization
+tool, that makes use of traditional machine learning frameworks, such as
+Scikit-Learn and TensorFlow, to create scalable Recommender Systems workflows
+that anyone can use. ### Who is it for? Rexify is a project that simplifies and
+standardizes the workflow of recommender systems. It is mostly geared towards
+people with little to no machine learning knowledge, that want to implement
+somewhat scalable Recommender Systems in their applications. ## Installation
+The easiest way to install Rexify is via `pip`: ```shell pip install rexify ```
+## Quick Tour Rexify is meant to be usable right out of the box. All you need
+to set up your model is interaction data - something that kind of looks like
+this: | user_id | item_id | timestamp | event_type | |---------|---------|-----
+-------|-------------| | 22 | 67 | 2021/05/13 | Purchase | | 37 | 9 | 2021/04/
+11 | Page View | | 22 | 473 | 2021/04/11 | Add to Cart | | ... | ... | ... |
+... | | 358 | 51 | 2021/04/11 | Purchase | Additionally, we'll have to have
+configured a schema for the data. This schema is what will allow Rexify to
+generate a dynamic model and preprocessing steps. The schema should be
+comprised of two dictionaries (`user`, `Ã¬tem`) and two key-value pairs:
+`event_type` (which should point to the column of the event type) and
+`timestamp` ( which should point to the timestamp column) Each of these
+dictionaries should consist of features and internal data types, such as: `id`,
+`category`, `number`. More data types will be available in the future. ```json
+{ "user": { "user_id": "id", "age": "number" }, "item": { "item_id": "id",
+"category": "category" }, "timestamp": "timestamp" "event_type": "event_type" }
+``` Essentially, what Rexify will do is take the schema, and dynamically adapt
+to the data. There are two main components in Rexify workflows:
+`FeatureExtractor` and `Recommender`. The `FeatureExtractor` is a scikit-learn
+Transformer that basically takes the schema of the data, and transforms the
+event data accordingly. Another method `.make_dataset()`, converts the
+transformed data into a `tf.data.Dataset`, all correctly configured to be fed
+to the `Recommender` model. `Recommender` is a `tfrs.Model` that basically
+implements the Query and Candidate towers. During training, the Query tower
+will take the user ID, user features, and context, to learn an embedding; the
+Candidate tower will do the same for the item ID and its features. More
+information about how the `FeatureExtractor` and the `Recommender` works can be
+found [here](https://rexify.readthedocs.io/en/latest/overview/
+architecture.html). A sample Rexify workflow should sort of look like this:
+````python import pandas as pd from rexify import Schema, FeatureExtractor,
+Recommender events = pd.read_csv('path/to/events/data') schema = Schema.load
+('path/to/schema') feat = FeatureExtractor(schema, users='path/to/users/data',
+items='path/to/events/data') x = feat.fit_transform(events) x =
+feat.make_dataset(x) model = Recommender(**feat.model_params) model.compile()
+model.fit(events, batch_size=512) ```` When training is complete, you'll have a
+trained `tf.keras.Model` ready to be used, as you normally would. ## License
+[MIT](https://github.com/joseprsm/rexify/blob/main/LICENSE)
```

