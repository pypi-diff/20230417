# Comparing `tmp/monod-0.2.5.0.tar.gz` & `tmp/monod-0.2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monod-0.2.5.0.tar", last modified: Fri Dec  2 00:00:27 2022, max compression
+gzip compressed data, was "monod-0.2.6.0.tar", last modified: Mon Apr 17 16:52:42 2023, max compression
```

## Comparing `monod-0.2.5.0.tar` & `monod-0.2.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2022-12-02 00:00:27.218342 monod-0.2.5.0/
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1341 2022-05-30 19:26:51.000000 monod-0.2.5.0/LICENSE
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1457 2022-12-02 00:00:27.219342 monod-0.2.5.0/PKG-INFO
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      973 2022-06-15 16:21:56.000000 monod-0.2.5.0/README.md
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)       86 2022-05-30 19:14:34.000000 monod-0.2.5.0/pyproject.toml
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      675 2022-12-02 00:00:27.219342 monod-0.2.5.0/setup.cfg
-drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2022-12-02 00:00:27.168344 monod-0.2.5.0/src/
-drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2022-12-02 00:00:27.218342 monod-0.2.5.0/src/monod/
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        0 2022-05-30 19:12:13.000000 monod-0.2.5.0/src/monod/__init__.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    36473 2022-11-18 22:42:36.000000 monod-0.2.5.0/src/monod/analysis.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    25817 2022-11-25 19:36:33.000000 monod-0.2.5.0/src/monod/cme_toolbox.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     2732 2022-08-29 21:59:28.000000 monod-0.2.5.0/src/monod/drivers.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    12319 2022-09-13 20:39:23.000000 monod-0.2.5.0/src/monod/extract_data.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    76847 2022-11-25 19:36:33.000000 monod-0.2.5.0/src/monod/inference.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1089 2022-08-29 21:59:28.000000 monod-0.2.5.0/src/monod/plot_aesthetics.py
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    24326 2022-11-08 06:16:59.000000 monod-0.2.5.0/src/monod/preprocess.py
-drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2022-12-02 00:00:27.218342 monod-0.2.5.0/src/monod.egg-info/
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1457 2022-12-02 00:00:27.000000 monod-0.2.5.0/src/monod.egg-info/PKG-INFO
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      398 2022-12-02 00:00:27.000000 monod-0.2.5.0/src/monod.egg-info/SOURCES.txt
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        1 2022-12-02 00:00:27.000000 monod-0.2.5.0/src/monod.egg-info/dependency_links.txt
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)       45 2022-12-02 00:00:27.000000 monod-0.2.5.0/src/monod.egg-info/requires.txt
--rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        6 2022-12-02 00:00:27.000000 monod-0.2.5.0/src/monod.egg-info/top_level.txt
+drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2023-04-17 16:52:42.270509 monod-0.2.6.0/
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1341 2022-05-30 19:26:51.000000 monod-0.2.6.0/LICENSE
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1457 2023-04-17 16:52:42.270509 monod-0.2.6.0/PKG-INFO
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      973 2022-06-15 16:21:56.000000 monod-0.2.6.0/README.md
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)       86 2022-05-30 19:14:34.000000 monod-0.2.6.0/pyproject.toml
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      675 2023-04-17 16:52:42.270509 monod-0.2.6.0/setup.cfg
+drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2023-04-17 16:52:42.218511 monod-0.2.6.0/src/
+drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2023-04-17 16:52:42.269509 monod-0.2.6.0/src/monod/
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        0 2022-05-30 19:12:13.000000 monod-0.2.6.0/src/monod/__init__.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    36473 2023-04-17 16:49:31.000000 monod-0.2.6.0/src/monod/analysis.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    26280 2023-04-17 16:51:29.000000 monod-0.2.6.0/src/monod/cme_toolbox.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     2732 2022-08-29 21:59:28.000000 monod-0.2.6.0/src/monod/drivers.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    12783 2023-04-17 16:51:28.000000 monod-0.2.6.0/src/monod/extract_data.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    76847 2022-11-25 19:36:33.000000 monod-0.2.6.0/src/monod/inference.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1089 2022-08-29 21:59:28.000000 monod-0.2.6.0/src/monod/plot_aesthetics.py
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)    24326 2023-04-17 16:50:37.000000 monod-0.2.6.0/src/monod/preprocess.py
+drwxrwxr-x   0 ggorin    (1000) ggorin    (1000)        0 2023-04-17 16:52:42.269509 monod-0.2.6.0/src/monod.egg-info/
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)     1457 2023-04-17 16:52:42.000000 monod-0.2.6.0/src/monod.egg-info/PKG-INFO
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)      398 2023-04-17 16:52:42.000000 monod-0.2.6.0/src/monod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        1 2023-04-17 16:52:42.000000 monod-0.2.6.0/src/monod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)       45 2023-04-17 16:52:42.000000 monod-0.2.6.0/src/monod.egg-info/requires.txt
+-rw-rw-r--   0 ggorin    (1000) ggorin    (1000)        6 2023-04-17 16:52:42.000000 monod-0.2.6.0/src/monod.egg-info/top_level.txt
```

### Comparing `monod-0.2.5.0/LICENSE` & `monod-0.2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/PKG-INFO` & `monod-0.2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monod
-Version: 0.2.5.0
+Version: 0.2.6.0
 Summary: the Monod package fits CME models to sequencing data.
 Home-page: https://github.com/pachterlab/monod
 Author: Gennady Gorin, Lior Pachter
 Author-email: ggorin@caltech.edu, lpachter@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `monod-0.2.5.0/README.md` & `monod-0.2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/setup.cfg` & `monod-0.2.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = monod
-version = 0.2.5.0
+version = 0.2.6.0
 author = Gennady Gorin, Lior Pachter
 author_email = ggorin@caltech.edu, lpachter@caltech.edu
 description = the Monod package fits CME models to sequencing data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pachterlab/monod
 classifiers =
```

### Comparing `monod-0.2.5.0/src/monod/analysis.py` & `monod-0.2.6.0/src/monod/analysis.py`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/src/monod/cme_toolbox.py` & `monod-0.2.6.0/src/monod/cme_toolbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,32 +140,50 @@
 
         Returns
         -------
         name: tuple of str
             TeX-formatted log-parameter names for the current transcriptional model.
             Useful for plot labels.
         """
+        param_str = []
         if self.bio_model == "Constitutive":
-            return (r"$\log_{10} \beta$", r"$\log_{10} \gamma$")
+            param_str += [r"$\log_{10} \beta$", r"$\log_{10} \gamma$"]
         elif self.bio_model == "Delay":
-            return (r"$\log_{10} b$", r"$\log_{10} \beta$", r"$\log_{10} \tau^{-1}$")
+            param_str += [
+                r"$\log_{10} b$",
+                r"$\log_{10} \beta$",
+                r"$\log_{10} \tau^{-1}$",
+            ]
         elif self.bio_model == "DelayedSplicing":
-            return (r"$\log_{10} b$", r"$\log_{10} \tau^{-1}$", r"$\log_{10} \gamma$")
+            param_str += [
+                r"$\log_{10} b$",
+                r"$\log_{10} \tau^{-1}$",
+                r"$\log_{10} \gamma$",
+            ]
         elif self.bio_model == "Bursty":
-            return (r"$\log_{10} b$", r"$\log_{10} \beta$", r"$\log_{10} \gamma$")
+            param_str += [r"$\log_{10} b$", r"$\log_{10} \beta$", r"$\log_{10} \gamma$"]
         elif self.bio_model == "Extrinsic":
-            return (r"$\log_{10} \alpha$", r"$\log_{10} \beta$", r"$\log_{10} \gamma$")
+            param_str += [
+                r"$\log_{10} \alpha$",
+                r"$\log_{10} \beta$",
+                r"$\log_{10} \gamma$",
+            ]
         elif self.bio_model == "CIR":
-            return (r"$\log_{10} b$", r"$\log_{10} \beta$", r"$\log_{10} \gamma$")
+            param_str += [r"$\log_{10} b$", r"$\log_{10} \beta$", r"$\log_{10} \gamma$"]
         else:
             raise ValueError(
                 "Please select a biological noise model from {}.".format(
                     self.available_biomodels
                 )
             )
+        if self.amb_model == "Equal":
+            param_str += [r"$\log_{10} p$"]
+        elif self.amb_model == "Unequal":
+            param_str += [r"$\log_{10} p_N$", r"$\log_{10} p_M$"]
+        return param_str
 
     def get_num_params(self):
         """Return the number of parameters for the model instance.
         Note that these are gene-specific parameters, i.e., global technical noise
         parameters are not used here.
 
         Returns
```

### Comparing `monod-0.2.5.0/src/monod/drivers.py` & `monod-0.2.6.0/src/monod/drivers.py`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/src/monod/extract_data.py` & `monod-0.2.6.0/src/monod/extract_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -277,15 +277,17 @@
             list of attributes to store, provided in extract_data.
         *input_data
             attributes to store, as enumerated in the class definition.
         """
         for j in range(len(input_data)):
             setattr(self, attr_names[j], input_data[j])
 
-    def get_noise_decomp(self, sizefactor="pf", lognormalize=True, pcount=0):
+    def get_noise_decomp(
+        self, sizefactor="pf", lognormalize=True, pcount=0, which_variance_measure="CV2"
+    ):
         """
         This method performs normalization and variance stabilization on the raw data, and
         reports the fractions of normalized variance retained and removed as a result of the process.
         The unspliced and spliced species are analyzed independently.
 
         Parameters
         ----------
@@ -308,28 +310,39 @@
 
         """
         f = np.zeros((self.n_genes, 2, 2))  # genes -- bio vs tech -- species
 
         S = np.copy(self.layers[1])
         U = np.copy(self.layers[0])
 
-        CV2_S = S.var(1) / S.mean(1) ** 2
-        CV2_U = U.var(1) / U.mean(1) ** 2
+        if which_variance_measure == "CV2":
+            var_fun = lambda X: X.var(1) / (X.mean(1) ** 2)
+        elif which_variance_measure == "var":
+            var_fun = lambda X: X.var(1)
+        elif which_variance_measure == "Fano":
+            var_fun = lambda X: X.var(1) / (X.mean(1))
+
+        var_S = var_fun(S)
+        var_U = var_fun(U)
+        # CV2_S = S.var(1) / S.mean(1) ** 2
+        # CV2_U = U.var(1) / U.mean(1) ** 2
 
         S = normalize_count_matrix(S, sizefactor, lognormalize, pcount)
         U = normalize_count_matrix(U, sizefactor, lognormalize, pcount)
 
-        CV2_S_norm = S.var(1) / S.mean(1) ** 2
-        CV2_U_norm = U.var(1) / U.mean(1) ** 2
+        var_S_norm = var_fun(S)
+        var_U_norm = var_fun(U)
+        # CV2_S_norm = S.var(1) / S.mean(1) ** 2
+        # CV2_U_norm = U.var(1) / U.mean(1) ** 2
 
         # compute fraction of CV2 eliminated for unspliced and spliced
-        f[:, 0, 0] = CV2_U_norm / CV2_U
+        f[:, 0, 0] = var_U_norm / var_U
         f[:, 1, 0] = 1 - f[:, 0, 0]
 
-        f[:, 0, 1] = CV2_S_norm / CV2_S
+        f[:, 0, 1] = var_S_norm / var_S
         f[:, 1, 1] = 1 - f[:, 0, 1]
         return f
 
 
 def normalize_count_matrix(
     X, sizefactor="pf", lognormalize=True, pcount=0, logbase="e"
 ):
```

### Comparing `monod-0.2.5.0/src/monod/inference.py` & `monod-0.2.6.0/src/monod/inference.py`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/src/monod/plot_aesthetics.py` & `monod-0.2.6.0/src/monod/plot_aesthetics.py`

 * *Files identical despite different names*

### Comparing `monod-0.2.5.0/src/monod/preprocess.py` & `monod-0.2.6.0/src/monod/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pytz
 import collections
 import csv
 import warnings
 import scipy
 from scipy import sparse
 
-code_ver_global = "025"  # bumping up version early Nov
+code_ver_global = "026"  # bumping up version early Nov
 
 ########################
 ## Debug and error logging
 ########################
 import logging, sys
 
 logging.basicConfig(stream=sys.stdout)
```

### Comparing `monod-0.2.5.0/src/monod.egg-info/PKG-INFO` & `monod-0.2.6.0/src/monod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monod
-Version: 0.2.5.0
+Version: 0.2.6.0
 Summary: the Monod package fits CME models to sequencing data.
 Home-page: https://github.com/pachterlab/monod
 Author: Gennady Gorin, Lior Pachter
 Author-email: ggorin@caltech.edu, lpachter@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

