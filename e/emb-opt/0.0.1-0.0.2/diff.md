# Comparing `tmp/emb_opt-0.0.1.tar.gz` & `tmp/emb_opt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emb_opt-0.0.1.tar", last modified: Thu Apr  6 20:16:08 2023, max compression
+gzip compressed data, was "emb_opt-0.0.2.tar", last modified: Mon Apr 17 16:50:22 2023, max compression
```

## Comparing `emb_opt-0.0.1.tar` & `emb_opt-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-06 20:16:08.637699 emb_opt-0.0.1/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    11337 2023-01-20 02:50:04.000000 emb_opt-0.0.1/LICENSE
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      111 2023-01-20 02:50:04.000000 emb_opt-0.0.1/MANIFEST.in
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      909 2023-04-06 20:16:08.637699 emb_opt-0.0.1/PKG-INFO
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      207 2023-04-04 22:08:26.000000 emb_opt-0.0.1/README.md
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-06 20:16:08.637699 emb_opt-0.0.1/emb_opt/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       22 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/__init__.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     7594 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/_modidx.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-06 20:16:08.637699 emb_opt-0.0.1/emb_opt/backends/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/backends/__init__.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2076 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/backends/chroma.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1691 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/backends/faiss.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1608 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/backends/hf.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2104 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/backends/qdrant.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2873 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/core.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      184 2023-04-05 17:20:40.000000 emb_opt-0.0.1/emb_opt/imports.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2896 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/query_update.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3213 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/runner.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1239 2023-04-06 19:08:36.000000 emb_opt-0.0.1/emb_opt/utils.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-06 20:16:08.637699 emb_opt-0.0.1/emb_opt.egg-info/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      909 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/PKG-INFO
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      534 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/SOURCES.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/dependency_links.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       36 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/entry_points.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-04 21:43:10.000000 emb_opt-0.0.1/emb_opt.egg-info/not-zip-safe
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       66 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/requires.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        8 2023-04-06 20:16:08.000000 emb_opt-0.0.1/emb_opt.egg-info/top_level.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1021 2023-04-06 18:15:45.000000 emb_opt-0.0.1/settings.ini
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       38 2023-04-06 20:16:08.637699 emb_opt-0.0.1/setup.cfg
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2560 2023-01-20 02:50:04.000000 emb_opt-0.0.1/setup.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:50:22.441037 emb_opt-0.0.2/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    11337 2023-01-20 02:50:04.000000 emb_opt-0.0.2/LICENSE
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      111 2023-01-20 02:50:04.000000 emb_opt-0.0.2/MANIFEST.in
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2333 2023-04-17 16:50:22.441037 emb_opt-0.0.2/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1631 2023-04-06 20:32:04.000000 emb_opt-0.0.2/README.md
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:50:22.437036 emb_opt-0.0.2/emb_opt/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       22 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     8410 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/_modidx.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:50:22.441037 emb_opt-0.0.2/emb_opt/backends/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:28:05.000000 emb_opt-0.0.2/emb_opt/backends/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2076 2023-04-17 16:28:05.000000 emb_opt-0.0.2/emb_opt/backends/chroma.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1691 2023-04-17 16:28:05.000000 emb_opt-0.0.2/emb_opt/backends/faiss.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1608 2023-04-17 16:28:05.000000 emb_opt-0.0.2/emb_opt/backends/hf.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2107 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/backends/qdrant.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     4540 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/core.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      204 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/imports.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3006 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/query_update.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3626 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/runner.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3546 2023-04-17 16:49:35.000000 emb_opt-0.0.2/emb_opt/utils.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:50:22.441037 emb_opt-0.0.2/emb_opt.egg-info/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2333 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      534 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       36 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/entry_points.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-04 21:43:10.000000 emb_opt-0.0.2/emb_opt.egg-info/not-zip-safe
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       66 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/requires.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        8 2023-04-17 16:50:22.000000 emb_opt-0.0.2/emb_opt.egg-info/top_level.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      914 2023-04-17 16:49:35.000000 emb_opt-0.0.2/settings.ini
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       38 2023-04-17 16:50:22.441037 emb_opt-0.0.2/setup.cfg
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2560 2023-01-20 02:50:04.000000 emb_opt-0.0.2/setup.py
```

### Comparing `emb_opt-0.0.1/LICENSE` & `emb_opt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emb_opt-0.0.1/emb_opt/_modidx.py` & `emb_opt-0.0.2/emb_opt/_modidx.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,18 @@
                                          'emb_opt.backends.qdrant.QdrantDatabase.__init__': ( 'qdrant.html#qdrantdatabase.__init__',
                                                                                               'emb_opt/backends/qdrant.py'),
                                          'emb_opt.backends.qdrant.QdrantDatabase.query': ( 'qdrant.html#qdrantdatabase.query',
                                                                                            'emb_opt/backends/qdrant.py')},
             'emb_opt.core': { 'emb_opt.core.Filter': ('core.html#filter', 'emb_opt/core.py'),
                               'emb_opt.core.Filter.__call__': ('core.html#filter.__call__', 'emb_opt/core.py'),
                               'emb_opt.core.Filter.__init__': ('core.html#filter.__init__', 'emb_opt/core.py'),
+                              'emb_opt.core.GradQueryDB': ('core.html#gradquerydb', 'emb_opt/core.py'),
+                              'emb_opt.core.GradQueryDB.__init__': ('core.html#gradquerydb.__init__', 'emb_opt/core.py'),
+                              'emb_opt.core.GradQueryDB.clean_results': ('core.html#gradquerydb.clean_results', 'emb_opt/core.py'),
+                              'emb_opt.core.GradQueryDB.query': ('core.html#gradquerydb.query', 'emb_opt/core.py'),
                               'emb_opt.core.PassThroughFilter': ('core.html#passthroughfilter', 'emb_opt/core.py'),
                               'emb_opt.core.PassThroughFilter.__call__': ('core.html#passthroughfilter.__call__', 'emb_opt/core.py'),
                               'emb_opt.core.PassThroughFilter.__init__': ('core.html#passthroughfilter.__init__', 'emb_opt/core.py'),
                               'emb_opt.core.QueryResult': ('core.html#queryresult', 'emb_opt/core.py'),
                               'emb_opt.core.QueryResult.__init__': ('core.html#queryresult.__init__', 'emb_opt/core.py'),
                               'emb_opt.core.QueryResult.to_dict': ('core.html#queryresult.to_dict', 'emb_opt/core.py'),
                               'emb_opt.core.Score': ('core.html#score', 'emb_opt/core.py'),
@@ -55,15 +59,18 @@
                                       'emb_opt.query_update.TopKUpdate.__call__': ( 'query_update.html#topkupdate.__call__',
                                                                                     'emb_opt/query_update.py'),
                                       'emb_opt.query_update.TopKUpdate.__init__': ( 'query_update.html#topkupdate.__init__',
                                                                                     'emb_opt/query_update.py')},
             'emb_opt.runner': { 'emb_opt.runner.Runner': ('runner.html#runner', 'emb_opt/runner.py'),
                                 'emb_opt.runner.Runner.__init__': ('runner.html#runner.__init__', 'emb_opt/runner.py'),
                                 'emb_opt.runner.Runner.search': ('runner.html#runner.search', 'emb_opt/runner.py'),
+                                'emb_opt.runner.Runner.step': ('runner.html#runner.step', 'emb_opt/runner.py'),
                                 'emb_opt.runner.SearchLog': ('runner.html#searchlog', 'emb_opt/runner.py'),
                                 'emb_opt.runner.SearchLog.__init__': ('runner.html#searchlog.__init__', 'emb_opt/runner.py'),
                                 'emb_opt.runner.SearchLog.add_entry': ('runner.html#searchlog.add_entry', 'emb_opt/runner.py'),
                                 'emb_opt.runner.SearchLog.compile_results': ('runner.html#searchlog.compile_results', 'emb_opt/runner.py'),
                                 'emb_opt.runner.SearchLog.compile_trajectories': ( 'runner.html#searchlog.compile_trajectories',
                                                                                    'emb_opt/runner.py')},
-            'emb_opt.utils': { 'emb_opt.utils.pack_dataset': ('utils.html#pack_dataset', 'emb_opt/utils.py'),
+            'emb_opt.utils': { 'emb_opt.utils.compute_rl_grad': ('utils.html#compute_rl_grad', 'emb_opt/utils.py'),
+                               'emb_opt.utils.pack_dataframe': ('utils.html#pack_dataframe', 'emb_opt/utils.py'),
+                               'emb_opt.utils.pack_dataset': ('utils.html#pack_dataset', 'emb_opt/utils.py'),
                                'emb_opt.utils.whiten': ('utils.html#whiten', 'emb_opt/utils.py')}}}
```

### Comparing `emb_opt-0.0.1/emb_opt/backends/chroma.py` & `emb_opt-0.0.2/emb_opt/backends/chroma.py`

 * *Files identical despite different names*

### Comparing `emb_opt-0.0.1/emb_opt/backends/faiss.py` & `emb_opt-0.0.2/emb_opt/backends/faiss.py`

 * *Files identical despite different names*

### Comparing `emb_opt-0.0.1/emb_opt/backends/hf.py` & `emb_opt-0.0.2/emb_opt/backends/hf.py`

 * *Files identical despite different names*

### Comparing `emb_opt-0.0.1/emb_opt/backends/qdrant.py` & `emb_opt-0.0.2/emb_opt/backends/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.collection_name = collection_name
         self.k = k
         self.search_request_kwargs = search_request_kwargs if search_request_kwargs else {}
     
     def query(self, query_vectors: np.ndarray) -> Dataset:
         
         search_queries = [
-                models.SearchRequest(vector=list(i), 
+                models.SearchRequest(vector=i.tolist(), 
                                      limit=self.k, 
                                      with_payload=True, 
                                      with_vector=True,
                                      **self.search_request_kwargs
                                     ) 
                 for i in query_vectors
                     ]
```

### Comparing `emb_opt-0.0.1/emb_opt/query_update.py` & `emb_opt-0.0.2/emb_opt/query_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_query_update.ipynb.
 
 # %% auto 0
 __all__ = ['QueryUpdate', 'RLUpdate', 'TopKUpdate']
 
 # %% ../nbs/02_query_update.ipynb 3
 from .imports import *
-from .utils import pack_dataset, whiten
+from .utils import pack_dataset, compute_rl_grad
 from .backends.hf import HFDatabase
 from .core import Score
 
 # %% ../nbs/02_query_update.ipynb 5
 class QueryUpdate():
     'Query update base class'
     def __call__(self, 
@@ -18,39 +18,35 @@
                 ) -> np.ndarray: # new query vectors
         return query_vectors
 
 # %% ../nbs/02_query_update.ipynb 7
 class RLUpdate(QueryUpdate):
     'Reinforcement Learning update'
     def __init__(self, 
-                 lr: float # learning rate
+                 lr: float, # learning rate
+                 distance_penalty: float=0.0, # query distance penalty
+                 scale_distance_penalty: bool=True # if True, penalty = penalty/LR (removed LR bias on penalty)
                 ):
         self.lr = lr
+        self.distance_penalty = distance_penalty
+        
+        if scale_distance_penalty:
+            self.distance_penalty = self.distance_penalty/self.lr
         
     def __call__(self, 
                  query_vectors: np.ndarray, # query vectors
                  query_dataset: Dataset # scored dataset
                 ) -> np.ndarray: # new query vectors
         
-        packed_dict = pack_dataset(query_dataset, 'query_idx', ['embedding', 'score'])
-        grads = []
-        
-        for query_idx in range(query_vectors.shape[0]):
-            embs = np.array(packed_dict[query_idx]['embedding'])
-            scores = np.array(packed_dict[query_idx]['score'])
+        grads = compute_rl_grad(query_vectors, query_dataset, self.distance_penalty)
 
-            advantages = whiten(scores)
-            grad = (advantages[:,None] * (2*(query_vectors[query_idx][None] - embs))).mean(0)
-            grads.append(grad)
-
-        grads = np.array(grads)
         updated_query_vectors = query_vectors - self.lr*grads
         return updated_query_vectors
 
-# %% ../nbs/02_query_update.ipynb 10
+# %% ../nbs/02_query_update.ipynb 11
 class TopKUpdate(QueryUpdate):
     'Top K update'
     def __init__(self, 
                  k: int, # top k value
                  score_weighting: bool=True # if True, top k average is weighted by score
                 ):
         self.k = k
@@ -61,22 +57,25 @@
                  query_dataset: Dataset # scored dataset
                 ) -> np.ndarray: # new query vectors
         
         packed_dict = pack_dataset(query_dataset, 'query_idx', ['embedding', 'score'])
         new_queries = []
         
         for query_idx in range(query_vectors.shape[0]):
-            embs = np.array(packed_dict[query_idx]['embedding'])
-            scores = np.array(packed_dict[query_idx]['score'])
-
-            topk_idxs = scores.argsort()[::-1][:self.k]
-            topk_embs = embs[topk_idxs]
-            topk_scores = scores[topk_idxs]
-
-            if self.score_weighting:
-                new_queries.append(np.average(topk_embs, 0, weights=topk_scores))
+            if len(packed_dict[query_idx]['score'])>0:
+                embs = np.array(packed_dict[query_idx]['embedding'])
+                scores = np.array(packed_dict[query_idx]['score'])
+
+                topk_idxs = scores.argsort()[::-1][:self.k]
+                topk_embs = embs[topk_idxs]
+                topk_scores = scores[topk_idxs]
+
+                if self.score_weighting:
+                    new_queries.append(np.average(topk_embs, 0, weights=topk_scores))
+                else:
+                    new_queries.append(np.average(topk_embs, 0))
             else:
-                new_queries.append(np.average(topk_embs, 0))
+                new_queries.append(query_vectors[query_idx])
 
         query_vectors = np.array(new_queries)
         
         return query_vectors
```

### Comparing `emb_opt-0.0.1/emb_opt/runner.py` & `emb_opt-0.0.2/emb_opt/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/07_runner.ipynb.
 
 # %% auto 0
 __all__ = ['SearchLog', 'Runner']
 
 # %% ../nbs/07_runner.ipynb 3
 from .imports import *
-from .utils import pack_dataset
+from .utils import pack_dataframe
 from .core import VectorDatabase, Score, Filter, PassThroughFilter
 from .query_update import QueryUpdate
 
+from .backends.hf import HFDatabase
+from .query_update import RLUpdate
+
 # %% ../nbs/07_runner.ipynb 4
 class SearchLog():
     'Logs results from `Runner`'
     def __init__(self):
         self.batch_log = {}
         
     def add_entry(self, 
                   iteration: int, 
                   query_vectors: np.ndarray, 
                   query_results: Dataset
                  ):
-        self.batch_log[iteration] = {'queries' : query_vectors, 'results' : query_results}
+        self.batch_log[iteration] = {'queries' : query_vectors, 'results' : query_results.to_pandas()}
         
     def compile_results(self) -> Dataset:
         results = []
         seen_keys = set()
 
         for k,v in self.batch_log.items():
             query_results = v['results']
 
-            for row in query_results.to_list():
+            for idx, row in query_results.iterrows():
+                row = dict(row)
                 if not (row['db_idx'] in seen_keys):
                     row.pop('query_idx')
                     row.pop('distance')
                     results.append(row)
                     seen_keys.update({row['db_idx']})
-
-        return Dataset.from_list(results)
+                    
+        output = pd.DataFrame(results)
+        output = output.sort_values('score', ascending=False)
+        output = output.reset_index(drop=True)
+        return output
     
     def compile_trajectories(self) -> dict:
         
         n_queries = self.batch_log[0]['queries'].shape[0]
         n_iters = len(self.batch_log.keys())
         trajectories = {i:{'query_vectors':[], 'scores':[]} for i in range(n_queries)}
         
         for iteration in range(n_iters):
             queries = self.batch_log[iteration]['queries']
-            score_dict = pack_dataset(self.batch_log[iteration]['results'], 'query_idx', ['score'])
+            score_dict = pack_dataframe(self.batch_log[iteration]['results'], 'query_idx', ['score'])
             
             for query_idx in range(n_queries):
                 trajectories[query_idx]['query_vectors'].append(queries[query_idx])
                 trajectories[query_idx]['scores'].append(score_dict[query_idx]['score'])
 
         for query_idx in range(n_queries):
             trajectories[query_idx]['query_vectors'] = np.stack(trajectories[query_idx]['query_vectors'])
@@ -68,23 +75,28 @@
                 ):
         
         self.vector_db = vector_db
         self.score = score
         self.query_update = query_update
         self.filter = filter if filter else PassThroughFilter()
         
+    def step(self, iteration, query_vectors, log=None):
+        query_results = self.vector_db.query(query_vectors)
+        query_results = self.filter(query_results)
+        query_results = self.score(query_results)
+
+        if log:
+            log.add_entry(iteration, query_vectors, query_results)
+
+        query_vectors = self.query_update(query_vectors, query_results)
+        return query_vectors
+        
     def search(self, 
                query_vectors: np.ndarray, 
                iterations: int
               ) -> SearchLog:
         log = SearchLog()
         
         for i in range(iterations):
-            query_results = self.vector_db.query(query_vectors)
-            query_results = self.filter(query_results)
-            query_results = self.score(query_results)
-            
-            log.add_entry(i, query_vectors, query_results)
-            
-            query_vectors = self.query_update(query_vectors, query_results)
+            query_vectors = self.step(i, query_vectors, log)
             
         return log
```

### Comparing `emb_opt-0.0.1/emb_opt.egg-info/SOURCES.txt` & `emb_opt-0.0.2/emb_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emb_opt-0.0.1/setup.py` & `emb_opt-0.0.2/setup.py`

 * *Files identical despite different names*

