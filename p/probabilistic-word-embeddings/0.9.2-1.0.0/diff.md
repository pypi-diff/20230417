# Comparing `tmp/probabilistic-word-embeddings-0.9.2.tar.gz` & `tmp/probabilistic_word_embeddings-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic-word-embeddings-0.9.2.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.0.0.tar", max compression
```

## Comparing `probabilistic-word-embeddings-0.9.2.tar` & `probabilistic_word_embeddings-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2115 2022-04-28 10:27:39.631983 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-02-16 16:06:30.469562 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     6797 2022-05-16 17:54:47.894479 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0     3700 2022-05-25 10:14:41.969967 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0     5654 2022-05-05 10:00:22.873362 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3009 2022-02-11 12:52:21.852326 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     2663 2022-04-28 10:28:32.816091 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     2250 2022-04-25 11:59:33.390004 probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      426 2022-05-30 14:05:02.420688 probabilistic-word-embeddings-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      764 2022-05-30 14:06:14.251613 probabilistic-word-embeddings-0.9.2/setup.py
--rw-r--r--   0        0        0      632 2022-05-30 14:06:14.251838 probabilistic-word-embeddings-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-03 10:42:26.292889 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0     9400 2023-04-04 13:40:34.971850 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0     8533 2023-03-24 16:02:14.633144 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-03-28 11:37:58.307437 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     4915 2023-04-17 07:32:28.780974 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     3492 2023-03-23 10:38:08.130487 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-04-17 07:37:33.905658 probabilistic_word_embeddings-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.0.0/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.0.0/PKG-INFO
```

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 We strive to keep all functionality clear, concise and easy to use.
 For instance, MAP estimation of the basic Bernoulli Embeddings only requires a couple of lines of code:
 
 ```py
 from probabilistic_word_embeddings.embeddings import Embedding
 from probabilistic_word_embeddings.preprocessing import preprocess_standard
 from probabilistic_word_embeddings.estimation import map_estimate
-from probabilistic_word_embeddings.evaluation import get_eval_file, embedding_similarities, evaluate_word_similarity
+from probabilistic_word_embeddings.evaluation import embedding_similarities, evaluate_word_similarity
 import tensorflow as tf
 
 with open("wiki.txt") as f:
     text = f.read().lower().split()
 text, vocabulary = preprocess_standard(text)
 
 e = Embedding(vocabulary=vocabulary, dimensionality=100)
@@ -25,22 +25,64 @@
 print(similarity)
 
 # Save the embedding
 e.save("embeddings.pkl")
 ```
 
 The estimation of _dynamic_ Bernoulli embeddings is relatively straightforward, too.
+
+```py
+from probabilistic_word_embeddings.embeddings import LaplacianEmbedding
+from probabilistic_word_embeddings.preprocessing import preprocess_partitioned
+from probabilistic_word_embeddings.estimation import map_estimate
+import networkx as nx
+import pandas as pd
+import re, itertools
+
+# Aggregate to yearly string objects and their associated years
+df = pd.read_csv("dynamic.csv")
+texts, years = [], sorted(list(set(df["year"])))
+for year in years:
+    current = df[df["year"] == year]
+    text = " ".join(current["speech"])
+    text = re.sub(r"\W+ ", '', text).lower()
+    texts.append(text.split())
+
+# Preprocess
+texts, vocabulary = preprocess_partitioned(texts, years)
+text = list(itertools.chain(*texts))
+print(text[:10], text[-10:])
+
+# Create side information graph, dog_2010 ~ dog_2011 etc.
+g = nx.Graph()
+for year0, year1 in zip(years[:-1], years[1:]):
+    for wd in set([wd.split("_")[0] for wd in vocabulary]):
+        wd0 = f"{wd}_{year0}"
+        wd1 = f"{wd}_{year1}"
+        if wd0 in vocabulary and wd1 in vocabulary:
+            g.add_edge(wd0, wd1)
+print(list(g.edges)[:10])
+
+# Define embedding and perform MAP estimation
+dim = 100
+e = LaplacianEmbedding(vocabulary, dim, g)
+e = map_estimate(e, text, model="cbow", ws=5, epochs=5, evaluate=False)
+
+# Save embedding
+e.save("dynamic_embedding.pkl")
+```
+
 Additionally, informative priors can be added to trace shifts in word meaning:
 
 ```py
 import networkx as nx
 from probabilistic_word_embeddings.embeddings import Embedding, LaplacianEmbedding
 from probabilistic_word_embeddings.preprocessing import preprocess_standard
 from probabilistic_word_embeddings.estimation import map_estimate
-from probabilistic_word_embeddings.evaluation import get_eval_file, embedding_similarities, evaluate_word_similarity
+from probabilistic_word_embeddings.evaluation import embedding_similarities, evaluate_word_similarity
 from scipy.spatial.distance import cosine as cos_dist
 import tensorflow as tf
 
 with open("wiki.txt") as f:
     text = f.read().lower().split()
 text, vocabulary = preprocess_standard(text)
```

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 class Embedding:
     '''
     Generic class for probabilistic embeddings.
     '''
     def __init__(self, vocabulary=None, dimensionality=100, lambda0=1.0, shared_context_vectors=True, saved_model_path=None):
         if saved_model_path is None:
+            if isinstance(vocabulary, dict):
+                vocabulary = set(vocabulary.keys())
             if not isinstance(vocabulary, set):
-                raise TypeError("vocabulary must be a set")
+                raise TypeError("vocabulary must be provided as a set, e.g. {'some','example', 'words'}, or a dict {'some': 0.1, 'example': 0.2, 'words': 0.7}")
             keys = list(vocabulary)
             if not shared_context_vectors:
                 keys = keys + list(set([key + "_c" for key in keys]))
                 self.vocabulary = {wd: ix for ix, wd in enumerate(sorted(keys))}
             else:
                 context_keys = {key + "_c": key.split("_")[0] + "_c" for key in keys}
                 all_indices = {key: ix for ix, key in enumerate(list(keys) + list(set(context_keys.values())))}
@@ -38,15 +40,15 @@
             with open(saved_model_path, "rb") as f:
                 d = pickle.load(f)
             self.vocabulary = d["vocabulary"]
             self.tf_vocabulary = dict_to_tf(self.vocabulary)
             self.theta = tf.Variable(d["theta"])
             self.lambda0 = d["lambda0"]
 
-    #@tf.function
+    @tf.function
     def __getitem__(self, item):
         if type(item) == str:
             return self.theta[self.vocabulary[item]]
         elif isinstance(item, list):
             item = tf.constant(item)
         ix = self.tf_vocabulary.lookup(item)
         return tf.gather(self.theta, ix, axis=0)
@@ -55,21 +57,24 @@
         #self.theta = self.theta - self.theta[]
         if type(item) == str:
             item = [item]
             new_value = tf.expand_dims(new_value, axis=0)
         if isinstance(item, list):
             item = tf.constant(item)
         ix = self.tf_vocabulary.lookup(item)
+        if tf.unique(ix)[0].shape != ix.shape:
+            warnings.warn("Duplicate indices detected in __setitem__")
         ix = list(ix.numpy())
         ix = [[i] for i in ix]
         old_value = self[item]
         old_scattered = tf.scatter_nd(ix, old_value, self.theta.shape)
         new_scattered = tf.scatter_nd(ix, new_value, self.theta.shape)
         
-        self.theta = self.theta - old_scattered + new_scattered
+        self.theta.assign_add(new_scattered)
+        self.theta.assign_sub(old_scattered)
     
     def __contains__(self, key):
         if type(key) == str:
             return key in self.vocabulary
         ix = self.tf_vocabulary.lookup(key)
         return ix != -1
 
@@ -101,15 +106,15 @@
         d["lambda0"] = self.lambda0
         if hasattr(self, 'lambda1'):
             d["lambda1"] = self.lambda1
         if hasattr(self, 'graph'):
             d["graph"] = self.graph
 
         with open(path, "wb") as f:
-            pickle.dump(d, f)
+            pickle.dump(d, f, protocol=4)
 
 class LaplacianEmbedding(Embedding):
     """
     Probabilistic embedding with a Laplacian graph prior
     """
     def __init__(self, vocabulary=None, dimensionality=100, graph=None, lambda0=1.0, lambda1=1.0, shared_context_vectors=True, saved_model_path=None):
         if saved_model_path is None:
@@ -119,14 +124,15 @@
             super().__init__(vocabulary, dimensionality, lambda0=lambda0, shared_context_vectors=shared_context_vectors)
             for wd in list(graph.nodes):
                 if wd in graph.nodes and wd not in self.vocabulary:
                     graph.remove_node(wd)
                     omitted_word_warning = f"'{wd}' does not exist in embedding vocabulary and will be omitted."
                     warnings.warn(omitted_word_warning)
             self.graph = graph
+            self.edges_i = None
         else:
             with open(saved_model_path, "rb") as f:
                 d = pickle.load(f)
             self.vocabulary = d["vocabulary"]
             self.tf_vocabulary = dict_to_tf(self.vocabulary)
             self.theta = tf.Variable(d["theta"])
             self.lambda0 = d["lambda0"]
@@ -141,18 +147,24 @@
             batch_size (int): Batch size. Used to scale the log prob for the whole dataset.
             data_size (int): Whole dataset size. Used to scale the log prob for the whole dataset.
         
         Returns:
             Log probability as tf.EagerTensor
         """
         g = self.graph
-        triple = [(e_i, e_j, g[e_i][e_j].get("weight", 1.0)) for e_i, e_j in g.edges]
-        edges_i, edges_j, weights = zip(*triple)
-        edges_i, edges_j = tf.constant(edges_i), tf.constant(edges_j)
-        weights = tf.constant(weights, dtype=tf.float64) * self.lambda1
+        if self.edges_i is None:
+            triple = [(e_i, e_j, g[e_i][e_j].get("weight", 1.0)) for e_i, e_j in g.edges]
+            edges_i, edges_j, weights = zip(*triple)
+            edges_i, edges_j = tf.constant(edges_i), tf.constant(edges_j)
+            weights = tf.constant(weights, dtype=tf.float64) * self.lambda1
+            self.edges_i = edges_i
+            self.edges_j = edges_j
+            self.edge_weights = weights
+
+        edges_i, edges_j, weights = self.edges_i, self.edges_j, self.edge_weights
         theta_i, theta_j = self[edges_i], self[edges_j]
         diffs = theta_i - theta_j
         squared_diffs = tf.reduce_sum(tf.multiply(diffs, diffs), axis=-1)
         weighted_diff_sum = tf.reduce_sum(tf.multiply(squared_diffs, weights))
         diagonal_sum = tf.reduce_sum(tf.multiply(self.theta, self.theta)) * self.lambda0
         plain_loss = - 0.5 * (diagonal_sum + weighted_diff_sum)
         return (batch_size / data_size) * plain_loss
```

### Comparing `probabilistic-word-embeddings-0.9.2/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,36 +27,47 @@
         # Map 1 => 1, 0 => -1
         x = 2 * x - 1
         logits = tf.multiply(logits, x)
 
     ps = tf.math.sigmoid(logits)
     log_ps = tf.math.log(ps)
     return log_ps
-    
+
+def generate_batch(data, ws=5, ns=5, batch_size=20000, start_ix=0, dataset_ix=0, ns_data=None, model="cbow"):
+    assert model in ["cbow", "sgns"]
+    if model == "cbow":
+        return generate_cbow_batch(data, ws=ws, ns=ns, batch=batch_size, start_ix=start_ix, ns_data=ns_data)
+    if model == "sgns":
+        return generate_sgns_batch(data, ws=ws, ns=ns, batch=batch_size, start_ix=start_ix, ns_data=ns_data)
+        
 # Generate a random i,j batch of the data.
 #@tf.function
-def generate_sgns_batch(data, ws=5, ns=5, batch=150000, start_ix=0, dataset_ix=0):
-    i,j = _generate_cbow_batch(data, tf.constant(ws), tf.constant(ns), tf.constant(batch), tf.constant(start_ix))
+def generate_sgns_batch(data, ws=5, ns=5, batch=150000, start_ix=0, ns_data=None):
+    if ns_data is None:
+        ns_data = data
+    i,j = _generate_cbow_batch(data, ns_data, tf.constant(ws), tf.constant(ns), tf.constant(batch), tf.constant(start_ix))
     
     i = tf.transpose(tf.tile([i], [ws * 2, 1]))
     
     i = tf.reshape(i, [ws * 2 * (1 + ns) * batch])
     j = tf.reshape(j, [ws * 2 * (1 + ns) * batch])
     x = tf.concat([tf.ones(ws * 2 * batch,dtype=tf.float64), tf.zeros(ws * 2 * ns * batch, dtype=tf.float64)], axis=0,)
     return i,j,x
 
 # Generate a random i,j batch of the data.
-def generate_cbow_batch(data, ws=5, ns=5, batch=150000, start_ix=0, dataset_ix=0):
+def generate_cbow_batch(data, ws=5, ns=5, batch=150000, start_ix=0, ns_data=None):
     #settings = tf.constant([ws, ns, batch, start_ix, dataset_ix])
-    i,j = _generate_cbow_batch(data, tf.constant(ws), tf.constant(ns), tf.constant(batch), tf.constant(start_ix))
+    if ns_data is None:
+        ns_data = data
+    i,j = _generate_cbow_batch(data, ns_data, tf.constant(ws), tf.constant(ns), tf.constant(batch), tf.constant(start_ix))
     x = tf.concat([tf.ones(batch, dtype=tf.float64), tf.zeros(ns * batch, dtype=tf.float64)], axis=0,)
     return i,j,x
 
 @tf.function
-def _generate_cbow_batch(data, ws, ns, batch, start_ix):
+def _generate_cbow_batch(data, ns_data, ws, ns, batch, start_ix):
     #ws, ns, batch, start_ix, dataset_ix = settings
     # the dog saw the cat
     # data = [0, 1, 2, ..., 0, 3]
     #data = datasets[dataset_ix]
     N = data.shape[0]
 
     i = tf.range(start_ix, start_ix + batch, dtype=tf.int32) % N
@@ -73,15 +84,15 @@
     # Negative sampling
     ns_i = tf.random.uniform(maxval=N, shape=[batch * ns], dtype=tf.int32)
     ns_j = tf.tile(j, [ns, 1])
 
     # Get word types at the indices i, j
     i = tf.gather(data , i_return)
     j = tf.gather(data , j)
-    ns_i = tf.gather(data , ns_i)
+    ns_i = tf.gather(ns_data , ns_i)
     ns_j = tf.gather(data , ns_j)
 
     # Concatenate positive and negative samples
     i = tf.concat([i, ns_i], axis=0)
     j = tf.concat([j, ns_j], axis=0)
     
     # add context marker
```

### Comparing `probabilistic-word-embeddings-0.9.2/setup.py` & `probabilistic_word_embeddings-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 packages = \
 ['probabilistic_word_embeddings']
 
 package_data = \
 {'': ['*'], 'probabilistic_word_embeddings': ['data/eval/*']}
 
 install_requires = \
-['progressbar2', 'tensorflow-probability>=0.11,<0.12', 'tensorflow>=2.2,<3.0']
+['networkx',
+ 'pandas',
+ 'progressbar2',
+ 'scikit-learn',
+ 'tensorflow-probability>=0.11,<0.12',
+ 'tensorflow>=2.2,<3.0']
 
 setup_kwargs = {
     'name': 'probabilistic-word-embeddings',
-    'version': '0.9.2',
+    'version': '1.0.0',
     'description': 'Probabilistic Word Embeddings for Python',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `probabilistic-word-embeddings-0.9.2/PKG-INFO` & `probabilistic_word_embeddings-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 0.9.2
+Version: 1.0.0
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: networkx
+Requires-Dist: pandas
 Requires-Dist: progressbar2
+Requires-Dist: scikit-learn
 Requires-Dist: tensorflow (>=2.2,<3.0)
 Requires-Dist: tensorflow-probability (>=0.11,<0.12)
```

