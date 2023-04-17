# Comparing `tmp/sense2vec-2.0.1.tar.gz` & `tmp/sense2vec-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense2vec-2.0.1.tar", last modified: Thu Dec  8 10:26:00 2022, max compression
+gzip compressed data, was "sense2vec-2.0.2.tar", last modified: Mon Apr 17 13:23:56 2023, max compression
```

## Comparing `sense2vec-2.0.1.tar` & `sense2vec-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 10:26:00.589634 sense2vec-2.0.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2022-12-08 10:25:31.000000 sense2vec-2.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2022-12-08 10:25:31.000000 sense2vec-2.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    54236 2022-12-08 10:26:00.589634 sense2vec-2.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    53161 2022-12-08 10:25:31.000000 sense2vec-2.0.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)       86 2022-12-08 10:25:31.000000 sense2vec-2.0.1/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 10:26:00.581634 sense2vec-2.0.1/sense2vec/
--rw-r--r--   0 vsts      (1001) docker     (122)      374 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10126 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/component.py
--rw-r--r--   0 vsts      (1001) docker     (122)    27895 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/prodigy_recipes.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14062 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/sense2vec.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 10:26:00.585634 sense2vec-2.0.1/sense2vec/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 10:26:00.585634 sense2vec-2.0.1/sense2vec/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      270 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/cache
--rw-r--r--   0 vsts      (1001) docker     (122)       43 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      214 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/freqs.json
--rw-r--r--   0 vsts      (1001) docker     (122)       51 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/key2row
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/strings.json
--rw-r--r--   0 vsts      (1001) docker     (122)     2688 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/data/vectors
--rw-r--r--   0 vsts      (1001) docker     (122)     4786 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/test_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1715 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6445 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/test_sense2vec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2489 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6420 2022-12-08 10:25:31.000000 sense2vec-2.0.1/sense2vec/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 10:26:00.585634 sense2vec-2.0.1/sense2vec.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    54236 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      737 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      375 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      151 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-12-08 10:26:00.000000 sense2vec-2.0.1/sense2vec.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)     1812 2022-12-08 10:26:00.589634 sense2vec-2.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2022-12-08 10:25:31.000000 sense2vec-2.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:56.673763 sense2vec-2.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-04-17 13:23:38.000000 sense2vec-2.0.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-17 13:23:38.000000 sense2vec-2.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    54236 2023-04-17 13:23:56.673763 sense2vec-2.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    53161 2023-04-17 13:23:38.000000 sense2vec-2.0.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       86 2023-04-17 13:23:38.000000 sense2vec-2.0.2/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:56.669763 sense2vec-2.0.2/sense2vec/
+-rw-r--r--   0 vsts      (1001) docker     (122)      374 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10126 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27895 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/prodigy_recipes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14469 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/sense2vec.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:56.669763 sense2vec-2.0.2/sense2vec/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:56.669763 sense2vec-2.0.2/sense2vec/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      270 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/cache
+-rw-r--r--   0 vsts      (1001) docker     (122)       43 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      214 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/freqs.json
+-rw-r--r--   0 vsts      (1001) docker     (122)       51 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/key2row
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/strings.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     2688 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/data/vectors
+-rw-r--r--   0 vsts      (1001) docker     (122)     4786 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/test_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      400 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/test_issue155.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1715 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6445 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/test_sense2vec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2489 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6420 2023-04-17 13:23:38.000000 sense2vec-2.0.2/sense2vec/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 13:23:56.669763 sense2vec-2.0.2/sense2vec.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    54236 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      770 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      375 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      151 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 13:23:56.000000 sense2vec-2.0.2/sense2vec.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)     1812 2023-04-17 13:23:56.673763 sense2vec-2.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-04-17 13:23:38.000000 sense2vec-2.0.2/setup.py
```

### Comparing `sense2vec-2.0.1/LICENSE` & `sense2vec-2.0.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (C) 2019 ExplosionAI GmbH
+Copyright (C) 2019-2023 ExplosionAI GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sense2vec-2.0.1/PKG-INFO` & `sense2vec-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense2vec
-Version: 2.0.1
+Version: 2.0.2
 Summary: Contextually-keyed word vectors
 Home-page: https://github.com/explosion/sense2vec
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sense2vec Version: 2.0.1 Summary: Contextually-
+Metadata-Version: 2.1 Name: sense2vec Version: 2.0.2 Summary: Contextually-
 keyed word vectors Home-page: https://github.com/explosion/sense2vec Author:
 Explosion Author-email: contact@explosion.ai License: MIT Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `sense2vec-2.0.1/README.md` & `sense2vec-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/component.py` & `sense2vec-2.0.2/sense2vec/component.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/prodigy_recipes.py` & `sense2vec-2.0.2/sense2vec/prodigy_recipes.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/sense2vec.py` & `sense2vec-2.0.2/sense2vec/sense2vec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Tuple, List, Union, Sequence, Dict, Callable, Any
 from pathlib import Path
 from spacy.vectors import Vectors
 from spacy.strings import StringStore
 from spacy.util import SimpleFrozenDict
+from thinc.api import NumpyOps
 import numpy
 import srsly
 
 from .util import registry, cosine_similarity
 
 
 class Sense2Vec(object):
@@ -243,15 +244,19 @@
         key (unicode / int): The key to check.
         ignore_case (bool): Check for uppercase, lowercase and titlecase.
         RETURNS (list): The string keys of other entries with different senses.
         """
         result = []
         key = key if isinstance(key, str) else self.strings[key]
         word, orig_sense = self.split_key(key)
-        versions = set([word, word.lower(), word.upper(), word.title()]) if ignore_case else [word]
+        versions = (
+            set([word, word.lower(), word.upper(), word.title()])
+            if ignore_case
+            else [word]
+        )
         for text in versions:
             for sense in self.senses:
                 new_key = self.make_key(text, sense)
                 if sense != orig_sense and new_key in self:
                     result.append(new_key)
         return result
 
@@ -266,15 +271,19 @@
             set / empty, all senses in the vectors are used.
         ignore_case (bool): Check for uppercase, lowercase and titlecase.
         RETURNS (unicode): The best-matching key or None.
         """
         sense_options = senses or self.senses
         if not sense_options:
             return None
-        versions = set([word, word.lower(), word.upper(), word.title()]) if ignore_case else [word]
+        versions = (
+            set([word, word.lower(), word.upper(), word.title()])
+            if ignore_case
+            else [word]
+        )
         freqs = []
         for text in versions:
             for sense in sense_options:
                 key = self.make_key(text, sense)
                 if key in self:
                     freq = self.get_freq(key, -1)
                     freqs.append((freq, key))
@@ -300,14 +309,17 @@
 
         bytes_data (bytes): The data to load.
         exclude (list): Names of serialization fields to exclude.
         RETURNS (Sense2Vec): The loaded object.
         """
         data = srsly.msgpack_loads(bytes_data)
         self.vectors = Vectors().from_bytes(data["vectors"])
+        # Pin vectors to the CPU so that we don't end up comparing
+        # numpy and cupy arrays.
+        self.vectors.to_ops(NumpyOps())
         self.freqs = dict(data.get("freqs", []))
         self.cfg.update(data.get("cfg", {}))
         if "strings" not in exclude and "strings" in data:
             self.strings = StringStore().from_bytes(data["strings"])
         if "cache" not in exclude and "cache" in data:
             self.cache = data.get("cache", {})
         self._row2key = None
@@ -336,14 +348,17 @@
         RETURNS (Sense2Vec): The loaded object.
         """
         path = Path(path)
         strings_path = path / "strings.json"
         freqs_path = path / "freqs.json"
         cache_path = path / "cache"
         self.vectors = Vectors().from_disk(path)
+        # Pin vectors to the CPU so that we don't end up comparing
+        # numpy and cupy arrays.
+        self.vectors.to_ops(NumpyOps())
         self.cfg.update(srsly.read_json(path / "cfg"))
         if freqs_path.exists():
             self.freqs = dict(srsly.read_json(freqs_path))
         if "strings" not in exclude and strings_path.exists():
             self.strings = StringStore().from_disk(strings_path)
         if "cache" not in exclude and cache_path.exists():
             self.cache = srsly.read_msgpack(cache_path)
```

### Comparing `sense2vec-2.0.1/sense2vec/tests/data/vectors` & `sense2vec-2.0.2/sense2vec/tests/data/vectors`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/tests/test_component.py` & `sense2vec-2.0.2/sense2vec/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/tests/test_model.py` & `sense2vec-2.0.2/sense2vec/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/tests/test_sense2vec.py` & `sense2vec-2.0.2/sense2vec/tests/test_sense2vec.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/tests/test_util.py` & `sense2vec-2.0.2/sense2vec/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec/util.py` & `sense2vec-2.0.2/sense2vec/util.py`

 * *Files identical despite different names*

### Comparing `sense2vec-2.0.1/sense2vec.egg-info/PKG-INFO` & `sense2vec-2.0.2/sense2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense2vec
-Version: 2.0.1
+Version: 2.0.2
 Summary: Contextually-keyed word vectors
 Home-page: https://github.com/explosion/sense2vec
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sense2vec Version: 2.0.1 Summary: Contextually-
+Metadata-Version: 2.1 Name: sense2vec Version: 2.0.2 Summary: Contextually-
 keyed word vectors Home-page: https://github.com/explosion/sense2vec Author:
 Explosion Author-email: contact@explosion.ai License: MIT Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `sense2vec-2.0.1/sense2vec.egg-info/SOURCES.txt` & `sense2vec-2.0.2/sense2vec.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 sense2vec.egg-info/dependency_links.txt
 sense2vec.egg-info/entry_points.txt
 sense2vec.egg-info/requires.txt
 sense2vec.egg-info/top_level.txt
 sense2vec.egg-info/zip-safe
 sense2vec/tests/__init__.py
 sense2vec/tests/test_component.py
+sense2vec/tests/test_issue155.py
 sense2vec/tests/test_model.py
 sense2vec/tests/test_sense2vec.py
 sense2vec/tests/test_util.py
 sense2vec/tests/data/cache
 sense2vec/tests/data/cfg
 sense2vec/tests/data/freqs.json
 sense2vec/tests/data/key2row
```

### Comparing `sense2vec-2.0.1/setup.cfg` & `sense2vec-2.0.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.0.1
+version = 2.0.2
 description = Contextually-keyed word vectors
 url = https://github.com/explosion/sense2vec
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

