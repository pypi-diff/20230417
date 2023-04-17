# Comparing `tmp/geostat-0.8.1.tar.gz` & `tmp/geostat-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-qu2ms_y7/geostat-0.8.1.tar", last modified: Wed Apr 12 16:29:55 2023, max compression
+gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-399ucofq/geostat-0.8.2.tar", last modified: Mon Apr 17 00:52:28 2023, max compression
```

## Comparing `geostat-0.8.1.tar` & `geostat-0.8.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.1/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-12 16:29:55.875049 geostat-0.8.1/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.1/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-12 16:29:33.000000 geostat-0.8.1/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-12 16:29:55.875049 geostat-0.8.1/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-12 16:29:22.000000 geostat-0.8.1/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    16578 2023-04-12 07:07:58.000000 geostat-0.8.1/src/geostat/kernel.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.1/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.1/src/geostat/mean.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.1/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.1/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.1/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.1/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.1/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.1/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.1/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.1/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.1/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.1/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.1/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.1/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.1/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.1/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.2/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-17 00:52:28.076028 geostat-0.8.2/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.2/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-17 00:49:58.000000 geostat-0.8.2/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-17 00:52:28.076028 geostat-0.8.2/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.072028 geostat-0.8.2/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-17 00:49:50.000000 geostat-0.8.2/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    16688 2023-04-17 00:19:52.000000 geostat-0.8.2/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.2/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.2/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.2/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.2/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.2/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.2/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.2/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.2/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.2/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.2/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.2/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.2/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.2/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.2/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.2/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.2/tests/test_trend.py
```

### Comparing `geostat-0.8.1/LICENSE` & `geostat-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/PKG-INFO` & `geostat-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.1
+Version: 0.8.2
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.1/README.md` & `geostat-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/pyproject.toml` & `geostat-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geostat"
-version = "0.8.1"
+version = "0.8.2"
 description = "Model spatial data with Gaussian processes"
 readme = "README.md"
 authors = [
   {name="Michael J. Stephens", email="mjstephens@usgs.gov"},
   {name="Will Chang", email="will@hypergradient.ai"}
 ]
 license = { file = "LICENSE" }
```

### Comparing `geostat-0.8.1/src/geostat/kernel.py` & `geostat-0.8.2/src/geostat/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     def vars(self):
         return []
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
         x1 = e['locs1'][..., self.axis]
         x2 = e['locs2'][..., self.axis]
-        k = tf.minimum(ed(x1, 1), ed(x2, 0)) - self.start
+        k = tf.maximum(0., tf.minimum(ed(x1, 1), ed(x2, 0)) - self.start)
         return k
 
     def reg(self, p):
         return 0.
 
 class IntSquaredExponential(Kernel):
     def __init__(self, axis, start, range='range'):
@@ -257,14 +257,15 @@
 
         r = v['range']
         sdiff = (ed(x1, 1) - ed(x2, 0)) / (r * np.sqrt(2.))
         k = -tf.square(r) * (np.sqrt(np.pi) * sdiff * tf.math.erf(sdiff) + tf.exp(-tf.square(sdiff)))
         k -= k[0:1, :]
         k -= k[:, 0:1]
         k = k[1:, 1:]
+        k = tf.maximum(0., k)
 
         return k
 
     def reg(self, p):
         return 0.
 
 class IntExponential(Kernel):
@@ -289,14 +290,15 @@
 
         r = v['range']
         sdiff = tf.abs(ed(x1, 1) - ed(x2, 0)) / r
         k = -tf.square(r) * (sdiff + tf.exp(-sdiff))
         k -= k[0:1, :]
         k -= k[:, 0:1]
         k = k[1:, 1:]
+        k = tf.maximum(0., k)
 
         return k
 
     def reg(self, p):
         return 0.
 
 class Noise(Kernel):
@@ -465,15 +467,17 @@
         dx = unbroadcast(dx, x.shape)
         da = tf.where(x <= 0.0, tf.zeros_like(a), dy * y * tf.math.log(x))
         da = unbroadcast(da, a.shape)
         return dx, da
     return y, grad
 
 def unbroadcast(x, shape):
-    excess_rank = tf.maximum(0, len(x.shape) - len(shape))
+    xrank = len(x.shape)
+    rank = len(shape)
+    excess_rank = tf.maximum(0, xrank - rank)
     x = tf.reduce_sum(x, axis=tf.range(excess_rank))
     axes_that_are_one = tf.where(tf.equal(shape, 1))[:, 0]
     x = tf.reduce_sum(x, axis=axes_that_are_one, keepdims=True)
     return x
 
 def gamma_exp(d2, gamma):
     return tf.exp(-safepow(tf.maximum(d2, 0.0), 0.5 * gamma))
```

### Comparing `geostat-0.8.1/src/geostat/krige.py` & `geostat-0.8.2/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/mean.py` & `geostat-0.8.2/src/geostat/mean.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/mesh.py` & `geostat-0.8.2/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/metric.py` & `geostat-0.8.2/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/model.py` & `geostat-0.8.2/src/geostat/model.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/op.py` & `geostat-0.8.2/src/geostat/op.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat/param.py` & `geostat-0.8.2/src/geostat/param.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/src/geostat.egg-info/PKG-INFO` & `geostat-0.8.2/src/geostat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.1
+Version: 0.8.2
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.1/src/geostat.egg-info/SOURCES.txt` & `geostat-0.8.2/src/geostat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_antiderivative.py` & `geostat-0.8.2/tests/test_antiderivative.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_delta.py` & `geostat-0.8.2/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_gp.py` & `geostat-0.8.2/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_krige.py` & `geostat-0.8.2/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_mcmc.py` & `geostat-0.8.2/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_mesh.py` & `geostat-0.8.2/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_metric.py` & `geostat-0.8.2/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_multigp.py` & `geostat-0.8.2/tests/test_multigp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.1/tests/test_trend.py` & `geostat-0.8.2/tests/test_trend.py`

 * *Files identical despite different names*

