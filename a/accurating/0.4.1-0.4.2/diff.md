# Comparing `tmp/accurating-0.4.1.tar.gz` & `tmp/accurating-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.1.tar", max compression
+gzip compressed data, was "accurating-0.4.2.tar", max compression
```

## Comparing `accurating-0.4.1.tar` & `accurating-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.1/LICENSE
--rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.1/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.1/accurating/__init__.py
--rw-r--r--   0        0        0     8271 2023-04-17 01:12:08.446217 accurating-0.4.1/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.1/accurating/tests/__init__.py
--rw-r--r--   0        0        0     2152 2023-04-17 03:27:19.264149 accurating-0.4.1/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-17 04:10:00.673880 accurating-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 accurating-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.2/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.2/accurating/__init__.py
+-rw-r--r--   0        0        0     8407 2023-04-17 05:13:50.431970 accurating-0.4.2/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.2/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     2471 2023-04-17 05:14:30.265058 accurating-0.4.2/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-17 05:15:29.458691 accurating-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 accurating-0.4.2/PKG-INFO
```

### Comparing `accurating-0.4.1/LICENSE` & `accurating-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.1/README.md` & `accurating-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `accurating-0.4.1/accurating/model.py` & `accurating-0.4.2/accurating/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
     max_steps: int = 1_000_000
     """Limits the number of passes over the dataset."""
 
     do_log: bool = False
     """Enables additional logging."""
 
+    initial_lr: float = 10000.0
+    """It is automatically adjusted, but sometimes it is too large and blows up."""
+
 
 @dataclasses.dataclass
 class Model:
     """Trained model."""
 
     rating: np.ndarray
     """Currently the seasons have to be small integers.
@@ -148,20 +151,20 @@
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
         # return jnp.mean(winner_win_prob_log) - 0.005*jnp.mean(cons ** 2)
 
     # Optimize for these params:
     rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
     params = dataclasses.asdict(
-        Model(rating=rating, player_name=data.player_name))
+        Model(rating=rating, player_name=None))
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
-    lr = 10000.  # initial learning rate
+    lr = config.initial_lr
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
     last_eval = -1
     last_grad = tree_map(jnp.zeros_like, params)
     last_reset_step = 0
 
     for i in range(config.max_steps):
@@ -191,15 +194,15 @@
                 params, eval, grad = last_params, last_eval, last_grad
             else:
                 if (i - last_reset_step) % 12 == 0:
                     lr *= 1.5
                 last_params, last_eval, last_grad = params, eval, grad
             momentum = tree_map(lambda m, g: m_lr * m + g, momentum, grad)
             params = tree_map(lambda p, m: p + lr * m, params, momentum)
-    return Model(**params)
+    return Model(rating=params['rating'], player_name=data.player_name)
 
 
 def data_from_dicts(matches) -> MatchResultArrays:
     player_set = set()
 
     for match in matches:
         player_set.add(match['p1'])
```

### Comparing `accurating-0.4.1/accurating/tests/model_test.py` & `accurating-0.4.2/accurating/tests/model_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,26 +55,37 @@
         "p2": "Caesar",
         "winner": "Leon",
         "season": 0
       },
       {
         "p1": "Caesar",
         "p2": "Alusia",
+        "winner": "Caesar",
+        "season": 1
+      },
+      {
+        "p1": "Leon",
+        "p2": "Alusia",
         "winner": "Alusia",
         "season": 1
       }
     ]
     """
     matches = json.loads(json_str)
     data = accurating.data_from_dicts(matches)
 
     player_name = ['Alusia', 'Caesar', 'Leon']
-    p1 = np.array([2, 1])
-    p2 = np.array([1, 0])
-    p1_win_prob = np.array([1., 0.])
-    season = np.array([0, 1])
+    p1 = np.array([2, 1, 2])
+    p2 = np.array([1, 0, 0])
+    p1_win_prob = np.array([1., 1., 0])
+    season = np.array([0, 1, 1])
 
     assert data.player_name == player_name
     assert_array_equal(data.p1, p1)
     assert_array_equal(data.p2, p2)
     assert_array_equal(data.p1_win_prob, p1_win_prob)
     assert_array_equal(data.season, season)
+
+    cfg = accurating.Config(season_rating_stability=0.5,
+                            smoothing=0.1, max_steps=5, do_log=True, initial_lr=1.0,)
+    model = accurating.fit(data, cfg)
+    del model
```

### Comparing `accurating-0.4.1/pyproject.toml` & `accurating-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.1"
+version = "0.4.2"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.4.1/PKG-INFO` & `accurating-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.1
+Version: 0.4.2
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

