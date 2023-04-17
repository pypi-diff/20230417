# Comparing `tmp/iphyre-0.2.0.tar.gz` & `tmp/iphyre-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphyre-0.2.0.tar", last modified: Tue Feb  7 07:14:59 2023, max compression
+gzip compressed data, was "iphyre-0.2.1.tar", last modified: Mon Apr 17 06:11:50 2023, max compression
```

## Comparing `iphyre-0.2.0.tar` & `iphyre-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 07:14:59.621379 iphyre-0.2.0/
--rw-rw-rw-   0        0        0     1080 2022-12-28 03:51:44.000000 iphyre-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1072 2023-02-07 07:14:59.621379 iphyre-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      644 2022-12-30 04:24:46.000000 iphyre-0.2.0/README.md
--rw-rw-rw-   0        0        0      512 2023-02-07 07:12:46.000000 iphyre-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-07 07:14:59.621379 iphyre-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-07 07:14:59.597375 iphyre-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:14:59.612377 iphyre-0.2.0/src/iphyre/
--rw-rw-rw-   0        0        0       82 2023-01-10 05:07:17.000000 iphyre-0.2.0/src/iphyre/__init__.py
--rw-rw-rw-   0        0        0    22641 2023-02-07 07:08:06.000000 iphyre-0.2.0/src/iphyre/games.py
--rw-rw-rw-   0        0        0    22211 2023-01-22 07:54:18.000000 iphyre-0.2.0/src/iphyre/simulator.py
--rw-rw-rw-   0        0        0     2370 2023-01-10 06:27:36.000000 iphyre-0.2.0/src/iphyre/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-07 07:14:59.620379 iphyre-0.2.0/src/iphyre.egg-info/
--rw-rw-rw-   0        0        0     1072 2023-02-07 07:14:59.000000 iphyre-0.2.0/src/iphyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-02-07 07:14:59.000000 iphyre-0.2.0/src/iphyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 07:14:59.000000 iphyre-0.2.0/src/iphyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-07 07:14:59.000000 iphyre-0.2.0/src/iphyre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:50.048005 iphyre-0.2.1/
+-rw-rw-rw-   0        0        0     1080 2022-12-28 03:51:44.000000 iphyre-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1072 2023-04-17 06:11:50.048005 iphyre-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2022-12-30 04:24:46.000000 iphyre-0.2.1/README.md
+-rw-rw-rw-   0        0        0      512 2023-04-17 06:11:12.000000 iphyre-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 06:11:50.048005 iphyre-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:50.023006 iphyre-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:50.039006 iphyre-0.2.1/src/iphyre/
+-rw-rw-rw-   0        0        0       82 2023-01-10 05:07:17.000000 iphyre-0.2.1/src/iphyre/__init__.py
+-rw-rw-rw-   0        0        0    22641 2023-04-17 05:32:01.000000 iphyre-0.2.1/src/iphyre/games.py
+-rw-rw-rw-   0        0        0    22210 2023-04-17 05:27:08.000000 iphyre-0.2.1/src/iphyre/simulator.py
+-rw-rw-rw-   0        0        0     2370 2023-01-10 06:27:36.000000 iphyre-0.2.1/src/iphyre/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:50.047006 iphyre-0.2.1/src/iphyre.egg-info/
+-rw-rw-rw-   0        0        0     1072 2023-04-17 06:11:50.000000 iphyre-0.2.1/src/iphyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-17 06:11:50.000000 iphyre-0.2.1/src/iphyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:11:50.000000 iphyre-0.2.1/src/iphyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 06:11:50.000000 iphyre-0.2.1/src/iphyre.egg-info/top_level.txt
```

### Comparing `iphyre-0.2.0/LICENSE` & `iphyre-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iphyre-0.2.0/PKG-INFO` & `iphyre-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphyre
-Version: 0.2.0
+Version: 0.2.1
 Summary: Benchmark for Interactive Physical Reasoning
 Author: CoRe
 Project-URL: Homepage, https://lishiqianhugh.github.io/IPHYRE/
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `iphyre-0.2.0/README.md` & `iphyre-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iphyre-0.2.0/pyproject.toml` & `iphyre-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "iphyre"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="CoRe"},
 ]
 description = "Benchmark for Interactive Physical Reasoning"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `iphyre-0.2.0/src/iphyre/games.py` & `iphyre-0.2.1/src/iphyre/games.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
                   [100., 340., 20.]],
          'eli': [0, 0, 1, 0, 1, 1, 1, 0, 0, 0],
          'dynamic': [0, 0, 0, 1, 0, 0, 0, 0, 1, 1],
          'spring': [[5, 3]],
          },
 }
 
-FOLD_LIST = ['basic', 'compositional', 'noisy', 'multi_ball']
+FOLD_LIST = ['basic', 'noisy', 'compositional', 'multi_ball']
 GAMES = list(PARAS.keys())
 
 MAX_OBJ_NUM = 0
 MAX_ELI_OBJ_NUM = 0
 for key in PARAS.keys():
     obj_num = len(PARAS[key]['eli'])
     if obj_num > MAX_OBJ_NUM:
```

### Comparing `iphyre-0.2.0/src/iphyre/simulator.py` & `iphyre-0.2.1/src/iphyre/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
         self.b_mass, self.b_elasticity, self.b_friction = 1.0, 0.1, 0.5
         self.l_friction, self.l_elasticity = 0.5, 0.1
         self.space = pymunk.Space()
         self.space.gravity = (0., 100.0)
         self.screen = None
 
-        self.step_reward = -10 / self.FPS
-        self.eli_reward = -100
-        self.success_reward = 500
+        self.step_reward = -1 / self.FPS
+        self.eli_reward = -10
+        self.success_reward = 1000
 
         # specific information of games
         self.blocks = PARAS[self.game]['block']
         self.balls = PARAS[self.game]['ball']
         self.shape = [1] * len(self.blocks) + [0] * len(self.balls)
         self.num_ball = len(self.balls)
         self.eli = deepcopy(PARAS[self.game]['eli'])
```

### Comparing `iphyre-0.2.0/src/iphyre/utils.py` & `iphyre-0.2.1/src/iphyre/utils.py`

 * *Files identical despite different names*

### Comparing `iphyre-0.2.0/src/iphyre.egg-info/PKG-INFO` & `iphyre-0.2.1/src/iphyre.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphyre
-Version: 0.2.0
+Version: 0.2.1
 Summary: Benchmark for Interactive Physical Reasoning
 Author: CoRe
 Project-URL: Homepage, https://lishiqianhugh.github.io/IPHYRE/
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

