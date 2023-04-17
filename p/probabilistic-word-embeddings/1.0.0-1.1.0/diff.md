# Comparing `tmp/probabilistic_word_embeddings-1.0.0.tar.gz` & `tmp/probabilistic_word_embeddings-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.0.0.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.1.0.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.0.0.tar` & `probabilistic_word_embeddings-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7424 2023-04-03 10:42:26.292889 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0     9400 2023-04-04 13:40:34.971850 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0     8533 2023-03-24 16:02:14.633144 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-03-28 11:37:58.307437 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     4915 2023-04-17 07:32:28.780974 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     3492 2023-03-23 10:38:08.130487 probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      473 2023-04-17 07:37:33.905658 probabilistic_word_embeddings-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.0.0/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-03 10:42:26.292889 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0     9400 2023-04-04 13:40:34.971850 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0     9826 2023-04-17 09:54:17.143703 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-03-28 11:37:58.307437 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     4915 2023-04-17 07:32:28.780974 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     3492 2023-03-23 10:38:08.130487 probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-04-17 09:55:48.627387 probabilistic_word_embeddings-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.1.0/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.1.0/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/estimation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,14 +118,53 @@
         corr, p_value = rank_correlation(merged_df["similarity_x"], merged_df["similarity_y"])
 
         rows.append([dataset, corr, len(merged_df), p_value])
         #print(f"Rank Correlation {corr}")
 
     return pd.DataFrame(rows, columns=["Dataset", "Rank Correlation", "No. of Observations", "p-value"])
 
+def nearest_neighbors(embedding, words, K=25):
+    """
+    Evaluate embedding performance on word analogy tasks.
+    
+    Args:
+        embedding: embedding as pwe.embeddings.Embedding
+        dataset (pd.DataFrame): Dataframe where each row has four words, word1 - word2 + word3 ≈ word4
+    """
+    e = copy.deepcopy(embedding)
+    words = [wd for wd in words if wd in embedding]
+    r = len(words)
+    X = embedding[words]
+
+    inv_vocab = {v: k for k, v in e.vocabulary.items()}
+    eliminate = list(range(len(inv_vocab)))
+    eliminate = [0.0 if ("_c" in inv_vocab[i] or inv_vocab[i] in words) else 1.0 for i in eliminate]
+    eliminate = tf.transpose(tf.constant([eliminate], dtype=tf.float64))
+
+    X, _ = tf.linalg.normalize(X, axis=1)
+
+    theta, _ = tf.linalg.normalize(e.theta, axis=1)
+    e.theta.assign(theta)
+
+    Ex = tf.linalg.tensordot(e.theta, X, axes=[1,1])
+    tiled_eliminate = tf.tile(eliminate, [1,r])
+    Ex = tf.multiply(Ex, tiled_eliminate)
+
+    rows = []
+
+    for i in range(r):
+        y_hat = Ex[:,i]
+        _, tops = tf.math.top_k(y_hat, k=K)
+        topwords = [inv_vocab[int(i)] for i in tops]
+        rows.append([words[i]] + topwords)
+    
+    columns = ["target"] + [f"@{i+1}" for i in range(K)]
+    df = pd.DataFrame(rows, columns=columns)
+    return df
+
 def evaluate_analogy(embedding, dataset, K=25):
     """
     Evaluate embedding performance on word analogy tasks.
     
     Args:
         embedding: embedding as pwe.embeddings.Embedding
         dataset (pd.DataFrame): Dataframe where each row has four words, word1 - word2 + word3 ≈ word4
```

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/preprocessing.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.1.0/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.0.0/setup.py` & `probabilistic_word_embeddings-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'progressbar2',
  'scikit-learn',
  'tensorflow-probability>=0.11,<0.12',
  'tensorflow>=2.2,<3.0']
 
 setup_kwargs = {
     'name': 'probabilistic-word-embeddings',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Probabilistic Word Embeddings for Python',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `probabilistic_word_embeddings-1.0.0/PKG-INFO` & `probabilistic_word_embeddings-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.0.0
+Version: 1.1.0
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

