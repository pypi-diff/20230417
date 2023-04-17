# Comparing `tmp/EmaCalc-0.9.5.tar.gz` & `tmp/EmaCalc-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmaCalc-0.9.5.tar", last modified: Sun Mar 19 07:18:02 2023, max compression
+gzip compressed data, was "EmaCalc-0.9.6.tar", last modified: Mon Apr 17 04:04:46 2023, max compression
```

## Comparing `EmaCalc-0.9.5.tar` & `EmaCalc-0.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-03-19 07:18:02.282003 EmaCalc-0.9.5/
--rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-0.9.5/LICENSE.txt
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-03-19 07:18:02.282076 EmaCalc-0.9.5/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)     9590 2023-03-19 07:17:01.000000 EmaCalc-0.9.5/README.md
--rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-0.9.5/pyproject.toml
--rw-r--r--   0 arne       (503) staff       (20)      962 2023-03-19 07:18:02.282358 EmaCalc-0.9.5/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-03-19 07:18:02.277673 EmaCalc-0.9.5/src/
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-03-19 07:18:02.281223 EmaCalc-0.9.5/src/EmaCalc/
--rw-r--r--   0 arne       (503) staff       (20)     5272 2023-03-19 07:06:59.000000 EmaCalc-0.9.5/src/EmaCalc/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-0.9.5/src/EmaCalc/dirichlet.py
--rw-r--r--   0 arne       (503) staff       (20)    44810 2023-03-18 08:08:12.000000 EmaCalc-0.9.5/src/EmaCalc/ema_base.py
--rw-r--r--   0 arne       (503) staff       (20)    41635 2023-03-07 08:05:15.000000 EmaCalc-0.9.5/src/EmaCalc/ema_data.py
--rw-r--r--   0 arne       (503) staff       (20)    47055 2023-03-11 05:58:38.000000 EmaCalc-0.9.5/src/EmaCalc/ema_display.py
--rw-r--r--   0 arne       (503) staff       (20)    23825 2023-03-11 06:05:31.000000 EmaCalc-0.9.5/src/EmaCalc/ema_display_format.py
--rw-r--r--   0 arne       (503) staff       (20)     9191 2022-08-21 09:20:55.000000 EmaCalc-0.9.5/src/EmaCalc/ema_file.py
--rw-r--r--   0 arne       (503) staff       (20)    28796 2023-03-08 03:30:42.000000 EmaCalc-0.9.5/src/EmaCalc/ema_group.py
--rw-r--r--   0 arne       (503) staff       (20)     8019 2022-08-20 18:28:46.000000 EmaCalc-0.9.5/src/EmaCalc/ema_latent.py
--rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-0.9.5/src/EmaCalc/ema_logging.py
--rw-r--r--   0 arne       (503) staff       (20)    14502 2022-11-29 02:42:44.000000 EmaCalc-0.9.5/src/EmaCalc/ema_model.py
--rw-r--r--   0 arne       (503) staff       (20)    14709 2023-03-07 02:35:00.000000 EmaCalc-0.9.5/src/EmaCalc/ema_nap.py
--rw-rw-rw-   0 arne       (503) staff       (20)    18893 2023-03-11 12:56:11.000000 EmaCalc-0.9.5/src/EmaCalc/ema_respondent.py
--rw-r--r--   0 arne       (503) staff       (20)    23228 2022-11-23 02:02:29.000000 EmaCalc-0.9.5/src/EmaCalc/ema_simulation.py
--rw-r--r--   0 arne       (503) staff       (20)    20379 2023-02-27 09:08:48.000000 EmaCalc-0.9.5/src/EmaCalc/ema_thresholds.py
--rw-r--r--   0 arne       (503) staff       (20)    20031 2022-08-18 08:38:01.000000 EmaCalc-0.9.5/src/EmaCalc/gauss_gamma.py
--rw-r--r--   0 arne       (503) staff       (20)    15188 2023-03-17 08:47:40.000000 EmaCalc-0.9.5/src/EmaCalc/run_ema.py
--rw-r--r--   0 arne       (503) staff       (20)    16660 2023-03-15 08:15:50.000000 EmaCalc-0.9.5/src/EmaCalc/run_sim.py
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-03-19 07:18:02.281896 EmaCalc-0.9.5/src/EmaCalc.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-03-19 07:18:02.000000 EmaCalc-0.9.5/src/EmaCalc.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      691 2023-03-19 07:18:02.000000 EmaCalc-0.9.5/src/EmaCalc.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2023-03-19 07:18:02.000000 EmaCalc-0.9.5/src/EmaCalc.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)       81 2023-03-19 07:18:02.000000 EmaCalc-0.9.5/src/EmaCalc.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)        8 2023-03-19 07:18:02.000000 EmaCalc-0.9.5/src/EmaCalc.egg-info/top_level.txt
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.549601 EmaCalc-0.9.6/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-0.9.6/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-04-17 04:04:46.549657 EmaCalc-0.9.6/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     9590 2023-03-19 07:22:45.000000 EmaCalc-0.9.6/README.md
+-rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-0.9.6/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      960 2023-04-17 04:04:46.549936 EmaCalc-0.9.6/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.542883 EmaCalc-0.9.6/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.548680 EmaCalc-0.9.6/src/EmaCalc/
+-rw-r--r--   0 arne       (503) staff       (20)     5369 2023-04-17 00:54:07.000000 EmaCalc-0.9.6/src/EmaCalc/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-0.9.6/src/EmaCalc/dirichlet.py
+-rw-r--r--   0 arne       (503) staff       (20)    50462 2023-04-13 14:27:33.000000 EmaCalc-0.9.6/src/EmaCalc/ema_base.py
+-rw-r--r--   0 arne       (503) staff       (20)    44608 2023-04-11 04:01:26.000000 EmaCalc-0.9.6/src/EmaCalc/ema_data.py
+-rw-r--r--   0 arne       (503) staff       (20)    38185 2023-04-17 04:02:27.000000 EmaCalc-0.9.6/src/EmaCalc/ema_display.py
+-rw-r--r--   0 arne       (503) staff       (20)    21804 2023-04-17 03:41:17.000000 EmaCalc-0.9.6/src/EmaCalc/ema_display_format.py
+-rw-r--r--   0 arne       (503) staff       (20)     9191 2022-08-21 09:20:55.000000 EmaCalc-0.9.6/src/EmaCalc/ema_file.py
+-rw-r--r--   0 arne       (503) staff       (20)    28796 2023-03-08 03:30:42.000000 EmaCalc-0.9.6/src/EmaCalc/ema_group.py
+-rw-r--r--   0 arne       (503) staff       (20)     8019 2022-08-20 18:28:46.000000 EmaCalc-0.9.6/src/EmaCalc/ema_latent.py
+-rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-0.9.6/src/EmaCalc/ema_logging.py
+-rw-r--r--   0 arne       (503) staff       (20)    14502 2022-11-29 02:42:44.000000 EmaCalc-0.9.6/src/EmaCalc/ema_model.py
+-rw-r--r--   0 arne       (503) staff       (20)    14769 2023-04-14 02:40:04.000000 EmaCalc-0.9.6/src/EmaCalc/ema_nap.py
+-rw-rw-rw-   0 arne       (503) staff       (20)    18893 2023-03-30 01:50:53.000000 EmaCalc-0.9.6/src/EmaCalc/ema_respondent.py
+-rw-r--r--   0 arne       (503) staff       (20)    23228 2022-11-23 02:02:29.000000 EmaCalc-0.9.6/src/EmaCalc/ema_simulation.py
+-rw-r--r--   0 arne       (503) staff       (20)    20379 2023-02-27 09:08:48.000000 EmaCalc-0.9.6/src/EmaCalc/ema_thresholds.py
+-rw-r--r--   0 arne       (503) staff       (20)    20031 2022-08-18 08:38:01.000000 EmaCalc-0.9.6/src/EmaCalc/gauss_gamma.py
+-rw-r--r--   0 arne       (503) staff       (20)    15413 2023-04-17 03:41:17.000000 EmaCalc-0.9.6/src/EmaCalc/run_ema.py
+-rw-r--r--   0 arne       (503) staff       (20)    16662 2023-04-17 00:54:07.000000 EmaCalc-0.9.6/src/EmaCalc/run_sim.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.549479 EmaCalc-0.9.6/src/EmaCalc.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      691 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       79 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)        8 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/top_level.txt
```

### Comparing `EmaCalc-0.9.5/LICENSE.txt` & `EmaCalc-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/PKG-INFO` & `EmaCalc-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 0.9.5
+Version: 0.9.6
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EmaCalc-0.9.5/README.md` & `EmaCalc-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/setup.cfg` & `EmaCalc-0.9.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy >=1.22
 	scipy >=1.7
 	matplotlib >=3.6.2
-	samppy >=1.2.2
-	pandas >=1.5
+	samppy >=1.3
+	pandas >=2.0
 	openpyxl >=3.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/__init__.py` & `EmaCalc-0.9.6/src/EmaCalc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 *** Reference:
 A Leijon, Petra von Gablenz, Inga Holube, Jalil Taghia and Karolina Smeds (2023):
 Bayesian Analysis of Ecological Momentary Assessment (EMA) Data Collected in Adults
 Before and After Hearing Rehabilitation.
 Frontiers in Digital Health, 5(1100705). doi: 10.3389/fdgth.2023.1100705
 
 *** Version History:
+* Version 0.9.6:
+Include range percentile plots and tables by groups, to show group differences
+
 * Version 0.9.5:
 Show observed and model-predicted attribute grade-counts,
     as requested by one reviewer of Frontiers (2023) paper.
 
 Changed ema_base parameter extraction -> n_parameters == model degrees of freedom,
 i.e., NO redundant model parameters.
 This leads to a slight change of arbitrary scale zero point:
@@ -111,10 +114,10 @@
             regardless of regression_effect specification. (NO GOOD! Changed in v. 0.6)
 
 * Version 0.5:
 2021-10-12, Crude version, based on CountProfileCalc-2021, and PairedCompCalc (on PyPi),
 2021-11-24, Functional beta version tested with simulated and (some) real data.
 """
 __name__ = 'EmaCalc'
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 
 __all__ = ['__version__', 'run_ema', 'run_sim']
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/dirichlet.py` & `EmaCalc-0.9.6/src/EmaCalc/dirichlet.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_base.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 The model is also slightly restricted by a weakly informative prior,
 for numerical stability in case of extreme response patterns,
 e.g., aLL ratings in the highest ordinal category.
 
 
 *** Version history:
+* Version 0.9.6:
+2023-04-02, new access functions situation_prob_df, attribute_theta_df yielding pandas result
+
 * Version 0.9.5:
 2022-11-28, changed _theta_map() to define attribute theta directly from effect parameters
             depending on restrict_attribute setting.
             One beta parameter less, if restrict_attribute is True.
             EmaParamBase._restrict_attr() no longer needed.
 2022-11-19, threshold calculations done by class methods in module ema_thresholds
 
@@ -73,21 +76,24 @@
 # *** e.g., with only alpha differences stored in xi ?
 import numpy as np
 from itertools import chain
 from collections import namedtuple
 from scipy.special import logit, expit
 from scipy.special import logsumexp, softmax
 import logging
+import pandas as pd
 
 from EmaCalc.gauss_gamma import GaussianRV
 # from EmaCalc.ema_thresholds import ThresholdsOld  # for backward compatibility
 from EmaCalc.ema_thresholds import ThresholdsFree, ThresholdsMidFixed
 
+# from EmaCalc.ema_display import aggregate_situation_prob  # ********* for TEST
+
 # ------------------------------------------------------
-__version__ = "2023-02-27"
+__version__ = "2023-04-13"
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 PRIOR_PSEUDO_RESPONDENT = 0.5  # seems to work OK
 # = hyperprior total pseudo-count re ONE real respondent
 # = prior GaussianRV.mean.learned_weight for all GMM components.
@@ -340,14 +346,47 @@
                            + 'Should not happen. Maybe too few responses?')
             logger.debug(f'alpha[too_small, :] = {alpha[too_small]}')
         u = np.exp(alpha)
         # avoid nan after normalization, should not be needed !
         u /= np.sum(u, axis=-1, keepdims=True)  # normalize within each Phase
         return u.reshape((-1, *self.emf.situation_shape))
 
+    def situation_prob_df(self, xi, groupby=None, sample_head='_sample'):
+        """Extract probability-mass for situations, given parameters,
+        used mainly by ema_display
+        :param xi: 2D array with parameter samples
+        :param groupby: (optional) tuple with situation key(s) to be included.
+            If undefined, include ALL situation dimensions as defined in self.emf
+        :param sample_head: (optional) level name of sample index
+        :return: ds = pandas Series object
+            with a MultiIndex with levels (sample_head, *groupby),
+            containing the CONDITIONAL probability for categories in groupby[0], given other groupby cases,
+            aggregated across situation dimensions NOT included in groupby.
+        """
+        u = self.situation_prob(xi)
+        # u[s, k0, k1, k2, ...] = s-th sample of conditional P[(k1, k2,...)-th situation | phase k0]
+        df_index = pd.MultiIndex.from_product([range(len(u)),
+                                               *[sit_dtype.categories
+                                                 for sit_dtype in self.emf.situation_dtypes.values()]],
+                                              names=[sample_head, *self.emf.situation_dtypes.keys()])
+        if groupby is None:
+            return pd.Series(u.reshape((-1,)), index=df_index)
+        else:
+            u /= u.shape[1]
+            # u[s, k0, k1, k2, ...] = s-th sample of prob-mass P[(k0, k1, k2,...)-th situation]
+            df = pd.Series(u.reshape((-1,)), index=df_index)
+            df = df.groupby(level=[0, *groupby], sort=False).sum()
+            # **** needed only if len(groupby) > 1
+            if len(groupby) > 1:
+                # scale to CONDITIONAL prob for categories in groupby[0], given other dimensions
+                ds_norm_factor = df.groupby(level=[0, *groupby[1:]]).transform(sum)
+                df = df / df.groupby(level=[0, *groupby[1:]]).transform(sum)
+                # CHECK: df.groupby(level=[0, *groupby[1:]], sort=False).sum() == 1., in all groups
+            return df
+
     def attribute_theta(self, xi, a):
         """Extract location of latent sensory variable, for ONE given attribute
         used only by ema_display
         :param xi: 2D array with parameter sample vectors
             xi[s, :] = s-th parameter sample vector
         :param a: attribute key = one of self.emf.attribute_grades.keys()
         :return: theta = mD array, with
@@ -356,14 +395,57 @@
         """
         a_index = list(self.emf.attribute_dtypes.keys()).index(a)
         beta_slice = self.attribute_slices[a_index].beta_slice
         # *** attribute_slices as dict instead ?
         beta = xi[..., beta_slice]
         return np.dot(beta, self.theta_map).reshape((-1, *self.emf.situation_shape))
 
+    def attribute_theta_df(self, xi, a, groupby=None, sample_head='_sample'):
+        """Extract location of latent sensory variable, for ONE given attribute,
+        given each situation category in selected situation dimension(s).
+        Used mainly by ema_display
+        :param xi: 2D array with parameter sample vectors
+            xi[s, :] = s-th parameter sample vector
+        :param a: attribute key = one of self.emf.attribute_grades.keys()
+        :param groupby: (optional) tuple with situation key(s) to be included.
+            If undefined, include ALL situation dimensions as defined in self.emf
+        :param sample_head: (optional) level name of sample index
+        :return: ds = pandas Series object
+            with a MultiIndex with levels (sample_head, *groupby),
+            containing the Attribute value samples for each category in groupby situation dimension(s),
+            aggregated across all OTHER situation_dtypes not included in groupby,
+            weighted by AVERAGE situation probabilities in those dimensions.
+        """
+        theta = self.attribute_theta(xi, a)
+        # theta[s, k0, k1, ...] = s-th sample of attribute location, in (k0, k1, ...)-th situation.
+        df_index = pd.MultiIndex.from_product([range(len(theta)),
+                                               *[sit_dtype.categories
+                                                 for sit_dtype in self.emf.situation_dtypes.values()]],
+                                              names=[sample_head, *self.emf.situation_dtypes.keys()])
+        theta_ds = pd.Series(theta.reshape((-1,)), index=df_index)
+        if groupby is None:
+            return theta_ds
+        else: # weighted average across situation dimensions not included
+            aggregate_by = list(set(self.emf.situation_dtypes.keys()) - set(groupby))
+            # = OTHER situation dimensions to be aggregated out
+            u = self.situation_prob_df(xi, sample_head=sample_head)  # *** use array access ??? ***
+            # u = Series object with same MultiIndex as theta_ds),
+            # containing the CONDITIONAL probability for categories in situation_dtypes[1:]
+            # given Phase category in situation_dtypes[0]
+            u = u / len(u.index.levels[1])
+            # u = absolute prob.mass for each sample and situation category
+            # w_cond = u / u.groupby(level=[0, *groupby], sort=False).transform(sum)
+            # # = CONDITIONAL prob.mass for categories in aggregate_by, GIVEN each category in groupby
+            w_av = u.groupby(level=[0, *aggregate_by], sort=False).transform(sum)
+            # = AVERAGE prob.mass for categories in aggregate_levels
+            # = same as ema_display.aggregate_situation_theta
+            # -> slightly less variability than w_cond
+            theta_ds = theta_ds * w_av  # w_cond  # ???
+            return theta_ds.groupby(level=[0, *groupby], sort=False).sum()
+
     def attribute_tau(self, xi, a):
         """Extract response thresholds for ONE given attribute,
         EXCEPT fixed extreme limits at -inf, +inf.
         Used only by ema_display
         :param xi: 2D array with parameter sample vectors
             xi[s, :] = s-th parameter sample vector
         :param a: attribute key = one of self.emf.attribute_grades.keys()
@@ -902,7 +984,21 @@
                                                      theta_0, true_theta_0):
                 print(f'\t\t{sc_dim_1}= {sc_1}: theta=\n', theta_1)
                 print(f'\t\t{sc_dim_1}= {sc_1}: true_theta=\n', true_theta_1)
 
     for a in emf.attribute_dtypes.keys():
         tau = p_base.attribute_tau(xi, a)
         print(f'\nAttribute {a}: tau.shape={tau.shape}. tau=\n', tau)
+
+    xi[0, 0:2] = 2.
+    print('\n***Testing situation_prob')
+    p_ds = p_base.situation_prob_df(xi, groupby=('Viktigt',))
+    print('situation prob.=\n',p_ds)
+    print('\n***Testing attribute_theta:')
+    th_ds = p_base.attribute_theta_df(xi, a='Speech')
+    print(th_ds)
+    p_ds = p_base.situation_prob_df(xi)
+    print('situation prob.=\n',p_ds)
+    th_ds = p_base.attribute_theta_df(xi, a='Speech', groupby=('CoSS',))
+    print('Speech=\n', th_ds)
+
+
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_data.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
                               'Test': ('EMA_64',)}
                     fmt='xlsx',
                     participant='sheet',    # xlsx sheet title is participant ID
                     )
 
 
 *** Version History:
+* Version 0.9.6:
+2023-04-11, bugfix EmaDataSet.join_df, .attribute_count, .attribute_mean
+
 * Version 0.9.4:
 2022-11-06: Fix to avoid FutureWarning in EmaDataSet.attribute_grade_mean
 
 * Version 0.9.3:
 2022-08-22, EmaDataSet.load(), .save() safer for pandas read, in case empty phase_key
 2022-08-16, changed EmaFrame.situations -> situation_dtypes
 2022-08-16, changed EmaFrame.attribute_grades -> attribute_dtypes
@@ -146,19 +149,20 @@
 * Version 0.5:
 2021-10-15, first functional version
 2021-11-18, groupby moved from EmaFrame -> EmaDataSet.load
 2021-11-20, EmaDataSet.ensure_complete
 2021-11-23, Group dir name MUST include both (g_factor, g_cat), e.g., 'Age_old'
 2021-11-xx, allow empty attribute_grades
 """
-# Future?:
-# *** Allow EmaFrame.attributes with tied response thresholds across several attributes ?
+# *** move grouping info -> EmaFrame, allow group categories in table column OR path string
+# *** save EmaDataSet as ONE big DataFrame file, OR separate by participants or groups
+
+# Future ?:
 # *** EmaDataSet.initialize + add method ? load = initialize + add
-# *** save EmaDataSet as ONE big DataFrame file ?
-# *** EmaDataSet store groups / subgroups hierarchically in tree structure ?
+# *** EmaDataSet store groups / subgroups hierarchically in tree structure ???
 
 import numpy as np
 from pathlib import Path
 import pandas as pd
 
 from itertools import product
 import logging
@@ -186,27 +190,28 @@
         :param ordinal_scales: dict with elements (scale_id: dtype), where
             dtype is a pd.CategoricalDtype defining ORDINAL categories for the scale.
         :param attribute_scales: dict with elements (attribute_key, scale_id), defining
             the scale used by each attribute.
             Note: Separate attributes may use the SAME ordinal scale,
                 if so specified by the researcher.
         """
+        # ******** include group_dtypes here, like situation_dtypes
         self.situation_dtypes = situation_dtypes
         self.phase_key = phase_key
         self.ordinal_scales = ordinal_scales
         self.attribute_scales = attribute_scales
 
     def __repr__(self):
         return (self.__class__.__name__ + '(\n\t\t' +
                 ',\n\t\t'.join(f'{key}={repr(v)}'
                                for (key, v) in vars(self).items()) +
                 '\n\t\t)')
 
     @classmethod
-    def setup(cls, situations=None, phase_key='Phase', attributes=None):
+    def setup(cls, situations=None, phase_key='Phase', attributes=None):  # include groups = dict here *******
         """Create the EmaFrame object defining all EMA variables to be analyzed.
         :param situations: (optional) dict or iterable with elements (dimension, category_list), where
             dimension is a string label identifying one situation "dimension",
             category_list is an iterable of labels for NOMINAL categories within this dimension.
         :param attributes: (optional) dict or iterable with elements (attribute, grades),
             attribute is string id of a rated perceptual attribute,
             grades is an iterable with ORDINAL categories, strings or integer.
@@ -546,93 +551,149 @@
         if len(self.groups) == 0:
             raise RuntimeError('No EMA data in any group.')
         for attr in self.emf.attribute_dtypes.keys():
             a_count = self.attribute_grade_count(attr)
             # = pd.DataFrame with all groups, all participants
             _check_ratings(attr, a_count)
 
+    # def join_df(self):
+    #     """Join all EMA data into ONE single pd.DataFrame instance
+    #     for all groups and all participants
+    #     :return: a single pd.DataFrame instance
+    #     """
+    #     df_list = []
+    #     for (g_tuple, g_data) in self.groups.items():
+    #         for (s, s_ema) in g_data.items():
+    #             df = Table(s_ema.copy())
+    #             df['Participant'] = s
+    #             for g in g_tuple:
+    #                 df[g[0]] = g[1]
+    #             df_list.append(df)
+    #     return pd.concat(df_list, ignore_index=True)
+
+    def group_head(self):  # TEMP fix -> EmaFrame *****
+        g_head = list(self.groups.keys())[0]  # they are all equal
+        return tuple(g_k[0] for g_k in g_head)
+
+    @staticmethod
+    def group_id(g_key):
+        """split g_key into actual group-id part
+        :param g_key: tuple of pairs (g_head, g_id)
+        :return: tuple including only g_id parts
+        """
+        return tuple(g_k[1] for g_k in g_key)
+
     def join_df(self):
         """Join all EMA data into ONE single pd.DataFrame instance
         for all groups and all participants
         :return: a single pd.DataFrame instance
         """
-        df_list = []
-        for (g_tuple, g_data) in self.groups.items():
-            for (s, s_ema) in g_data.items():
-                df = Table(s_ema.copy())
-                df['Participant'] = s
-                for g in g_tuple:
-                    df[g[0]] = g[1]
-                df_list.append(df)
-        return pd.concat(df_list, ignore_index=True)
+        g_dict = {self.group_id(g_key): pd.concat({s: s_data
+                                                   for (s, s_data) in g_data.items()},
+                                                  axis=0,
+                                                  sort=False,
+                                                  names=['Participant'])  # *** -> cls property ?
+                  for (g_key, g_data) in self.groups.items()}
+        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        return Table(df)
 
     def attribute_grade_count(self, a, groupby=None):
         """Collect table of ordinal grades for ONE attribute,
         for each (group, participant), optionally sub-divided by situation
-        :param a: selected attribute key
-        :param groupby: (optional) single situation dimension or sequence of such keys
+        :param a: ONE selected attribute key
+        :param groupby: (optional) single situation dimension or list of such dimensions
             for which separate attribute-counts are calculated.
             Counts are summed across any OTHER situation dimensions.
         :return: a pd.DataFrame object with all grade counts,
             with one row for each (group, participant, *groupby) case
             and one column for each grade category
+        2023-04-11, bugfix
         """
+        def s_count(s_data, a, groupby):
+            """Calculate participant value_count
+            :param s_data: a participant DataFrame
+            :param a: attribute key
+            :param groupby: list of situation dimension, possibly empty
+            :return: DataFrame instance with desired value counts for attribute a
+            """
+            if len(groupby) == 0:
+                return s_data[a].value_counts(sort=False)
+            else:
+                return s_data.groupby(groupby)[a].value_counts(sort=False)
+        # ------------------------------------------------------------
+
         if groupby is None:
             groupby = []
-        elif isinstance(groupby, str):  # in self.emf.situation_dtypes.keys():
+        elif isinstance(groupby, str):
             groupby = [groupby]
         groupby = [gb for gb in groupby if gb in self.emf.situation_dtypes.keys()]
-        df = self.join_df()
-        g_cols = list(set([g[0] for g_tuple in self.groups.keys() for g in g_tuple]))
-        if len(g_cols) == 1 and len(g_cols[0]) == 0:  # only ONE un-named group
-            g_cols = []
-        groupby = g_cols + ['Participant'] + groupby
-        df_count = df.groupby(groupby)[a].value_counts(sort=False).unstack()
-        return Table(df_count)
+        g_dict = {self.group_id(g_key): pd.concat({s: s_count(s_data, a, groupby)
+                                                   for (s, s_data) in g_data.items()},
+                                                  axis=0,
+                                                  sort=False,
+                                                  names=['Participant'])  # *** -> cls property ?
+                  for (g_key, g_data) in self.groups.items()}
+        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        return Table(df.unstack(a))
 
     def attribute_grade_mean(self, a=None, groupby=None):
         """Average raw attribute grades, encoded numerically as (1,.., n_grades)
         :param a: (optional) attribute label or sequence of attribute,
             if None, include all attributes
         :param groupby: (optional) single situation dimension or iterable of such keys
             for which separate attribute-means are calculated.
             Results are aggregated across any OTHER situation dimensions.
         :return: a pd.DataFrame instance with all mean Attribute grades,
             with rows Multi-indexed for Group(s), Participant, and selected Situation dimensions.
             with one column for selected attribute(s).
         """
         def recode_attr(df, a):
-            """Recode ordinal attribute grades to numerical (1,...,n_grades)
+            """Recode ordinal attribute grades linearly to numerical (1,...,n_grades)
             :param df: a pd.DataFrame instance
             :param a: list of attribute column names in df
             :return: None; df recoded in place
             """
             # *** allow external user-defined recoding function ?
             for a_i in a:
                 c = df[a_i].array.codes.copy().astype(float)
                 c[c < 0] = np.nan
                 df[a_i] = c + 1
-        # -------------------------------------------
+
+        def s_mean(s_data, a, groupby):
+            """Calculate participant value_count
+            :param s_data: a participant DataFrame
+            :param a: attribute key or list of such keys
+            :param groupby: list of situation dimension, possibly empty
+            :return: DataFrame instance with desired value counts for attribute a
+            """
+            s_data = s_data.copy()  # avoid modifying original
+            recode_attr(s_data, a)
+            if len(groupby) == 0:
+                return s_data[a].mean(numeric_only=True)
+            else:
+                return s_data.groupby(groupby)[a].mean(numeric_only=True)
+        # ------------------------------------------------------------
         if a is None:
             a = list(self.emf.attribute_dtypes.keys())
-        elif isinstance(a, str):  # a in self.emf.attribute_grades.keys():
+        elif isinstance(a, str):
             a = [a]
         a = [a_i for a_i in a if a_i in self.emf.attribute_dtypes.keys()]
         if groupby is None:
             groupby = []
-        elif isinstance(groupby, str):  # in self.emf.situation_dtypes.keys():
+        elif isinstance(groupby, str):
             groupby = [groupby]
         groupby = [gb for gb in groupby if gb in self.emf.situation_dtypes.keys()]
-        df = self.join_df()
-        g_cols = list(set([g[0] for g_tuple in self.groups.keys() for g in g_tuple]))
-        if len(g_cols) == 1 and len(g_cols[0]) == 0:
-            g_cols = []
-        groupby = g_cols + ['Participant'] + groupby
-        recode_attr(df, a)  # in place
-        return Table(df.groupby(groupby).mean(numeric_only=True))  # 2022-11-06
+        g_dict = {self.group_id(g_key): pd.concat({s: s_mean(s_data, a, groupby)
+                                                   for (s, s_data) in g_data.items()},
+                                                  axis=0,
+                                                  sort=False,
+                                                  names=['Participant'])  # *** -> cls property ?
+                  for (g_key, g_data) in self.groups.items()}
+        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        return Table(df)
 
     def nap_table(self, sit, nap_cat=None, a=None, groupby=None, p=0.95):
         """Calculate proportion of Non-overlapping Pairs = NAP result
         in ONE situation dimension with EXACTLY TWO categories, X and Y,
         = estimate of P(attribute grade in X < attribute grade in Y),
         given observed ordinal i.i.d. grade samples for attribute in situation_dtypes X and Y.
         :param sit: ONE situation dimension with TWO categories to be compared
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_display.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_display.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 result_path / group / 'random_individual' / attributes / ....
 result_path / group / 'random_individual' / situations / ....
 result_path / group / 'participants' / participant_id / attributes / ....
 result_path / group / 'participants' / participant_id / situations / ....
 result_path / 'group_effects' / 'population_mean' / attributes / ...  (if more than one group)
 
 *** Version History:
+* Version 0.9.6:
+2023-04-13, code cleanup, SituationProfile, AttributeProfile, SituationDiff, AttributeDiff
+            using Pandas access to model results via new ema_base methods
+2023-03-29, include percentile plots and tables in SituationDiff and AttributeDiff objects
+
 * Version 0.9.5:
 2023-03-07, include observed and model-estimated grade-count profiles,
             as requested by one reviewer for the Frontiers (2023) paper.
 2023-02-27, allow user to set n_samples for population-model display calculations
 
 * Version 0.9.4:
 2023-01-22, added default subdirectory names to FMT dict, to allow user control
@@ -86,27 +91,26 @@
 * Version 0.5.1
 2021-11-27, allow NO Attributes in model, check display requests, minor cleanup
 
 * Version 0.5
 2021-11-05, copied from PairedCompCalc, modified for EmaCalc
 2021-11-09, first functional version
 """
-# *************** include grade_counts in comment explanation *****************
 # ***** local superclass for pretty-printed repr() ?
 # ***** allow several Attributes in single plot ?
 
 import numpy as np
 from pathlib import Path
 import logging
-from itertools import product
 import string
+import pandas as pd
 
 from . import ema_display_format as fmt
 
-from samppy.credibility import cred_diff, cred_group_diff
+from samppy import credibility_pd as cred_pd
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 # ---------------------------- Default display parameters
 FMT = {'situations': (),    # sequence of situation dimensions or dimension-tuples to display
        'attributes': (),    # sequence of (attribute, situation_effect) to display
@@ -121,15 +125,15 @@
        'scale_unit': '',  # scale unit for attribute plot axis
        'sit_probability': 'Situation Probability',  # label in figs and tables
        'credibility': 'Credibility',  # heading in difference table
        'population_mean_dir': 'population_mean',  # directory name
        'random_individual_dir': 'random_individual',  # directory name
        'participants_dir': 'participants',  # directory name
        'group_effects_dir': 'group_effects',  # directory name
-       'n_samples': 1000,
+       'n_samples': 1000,  # number of samples for percentile calculations
        }
 
 DEFAULT_FIGURE_FORMAT = 'pdf'
 DEFAULT_TABLE_FORMAT = 'txt'
 
 
 def set_format_param(**kwargs):
@@ -252,28 +256,28 @@
 
     @classmethod
     def show(cls, emm,
              situations=None,
              attributes=None,
              grade_counts=None,
              **kwargs):
-        """Create displays for all results from an EMA study,
+        """Create requested displays for results from an EMA study,
         and store all display elements in a single structured object.
         :param emm: an ema_model.EmaModel instance, where
             emm.groups[group] is an ema_model.EmaGroupModel instance,
             emm.groups[group][participant_id] is an ema_model.EmaRespondentModel instance
         :param situations: (optional) list with selected situation dimensions to be displayed.
             situations[i] = a selected key in emm.emf.situation_dtypes, or a tuple of such keys.
         :param attributes: (optional) list with selected attribute displays to be displayed.
             attributes[i] = a tuple (attribute_key, sit_effect), where
                 attribute_key is one key in emm.emf.attribute_grades,
                 sit_effect is a situation dimension in emm.emf.situation_dtypes, or a tuple of such keys.
                 A single key will yield the main effect of the named situation dimension.
                 An effect tuple will also show interaction effects between situation dimensions,
-                IFF the model has been set up to estimate such interaction effects.
+                IFF the regression model has been set up to estimate such interaction effects.
         :param grade_counts: (optional) list with selected attribute grade counts to be displayed,
                 given as single attribute key, or tuple (attribute_key, situation) .
         :param: kwargs: (optional) dict with any other display formatting parameters
             for ema_display.FMT and / or ema_display_format.FMT and / or matplotlib
         :return: a cls instance filled with display objects
         """
         # get default scale_unit from emm, if not in kwargs:
@@ -366,15 +370,15 @@
     def display(cls, emm_g):
         """Generate all displays for ONE group
         :param emm_g: dict with elements (a_label: ema_group.EmaGroupModel)
         :return: cls instance with all displays for this group
         """
         pop_ind = None
         pop_mean = None
-        participants = None  # ***** empty dict in case no participants shown
+        participants = None
         counts = None
         if FMT['random_individual']:
             pop_ind = EmaDisplay.display(emm_g.predictive_population_ind())
         if FMT['population_mean']:
             pop_mean = EmaDisplay.display(emm_g.predictive_population_mean())
         if FMT['participants']:
             # logger.debug('Displaying participants:')
@@ -431,15 +435,15 @@
                       for a_effect in FMT['attributes']}
         return cls(situations, attributes)
 
 
 class CountDisplay:
     """Container for attribute displays of grade-count distributions,
     including both observed and model-estimated EMA-counts,
-    for ONE (Sub-)Population, (OR for ONE participant ********).
+    for ONE (Sub-)Population, (OR for ONE participant ? ********).
     """
     def __init__(self, attributes):
         """
         :param attributes: dict with (attr_effect, count-profile), where
             profile is a Profile instance for the selected attr_effect
         """
         self.attributes = attributes
@@ -502,68 +506,31 @@
         """Generate a probability-profile display for selected distribution and factor
         :param xi: 2D array of parameter-vector samples drawn from m_xi
         :param m_xi: a population or individual model instance
         :param sit_keys: tuple of one or more key(s) selected from emf.situation_dtypes.keys()
         :return: single cls instance showing CONDITIONAL probabilities
             for sit_keys[0], GIVEN each combination (j1,..., jD) for sit_keys[1], ...
         """
-        # *** ema_base to present samples as DataFrame ? ***********
-        emf = m_xi.base.emf
-        u = m_xi.base.situation_prob(xi)
-        u /= u.shape[1]  # = JOINT prob mass, incl. TestPhase: sum(u) == 1
-        u = aggregate_situation_prob(u, emf, sit_keys)
-        # Now with reordered and aggregated joint probabilities
-        # for selected subset of situation dimensions, such that
-        # u[s, j0, j1, ...] = s-th sample of joint probability for
-        # emf.situation_dtypes[sit_keys[0]][j0], emf.situation_dtypes[sit_keys[1]][j1], ... etc.
-        # u.shape == (u.shape[0], *emf.situation_shape[emf.situation_axes(sit_keys)])
-        if len(sit_keys) > 1:
-            s = np.sum(u, axis=1, keepdims=True)
-            # too_small = s <= 0
-            n_underflow = np.sum(s <= 0.)
-            if n_underflow > 0:
-                logger.warning(f'Situation display: {n_underflow} prob. sample(s) == 0, '
-                               + f'with {sit_keys}. '
-                               + 'Should not happen! Maybe too few EMA records?')
-                s = np.maximum(s, np.finfo(float).tiny)
-            u /= s
-            # u[:, i, ...] = samples for CONDITIONAL probability of i-th category in sit_keys[0],
-            # GIVEN ...-th category product of sit_keys[1:]
-            u = u.reshape((*u.shape[:2], -1))
-            # now linear-indexed in 3D with
-            # u[:, :, j] = prob given j-th product of sit_keys[2:], if any given
-            # case_labels[2] = all sit_keys[2:] joined  # ****************** !!!!
-        q = np.percentile(u, FMT['percentiles'], axis=0)
-        # --------------------------------------- percentile table as DataFrame:
-        case_labels = dict(_case_labels(emf.situation_dtypes, sit_keys))
-        df = fmt.tab_percentiles(q, perc=FMT['percentiles'],
-                                 case_labels=case_labels,
-                                 )  # *** replaced by ema_base access method ??? ********
-        perc = fmt.fig_percentiles(df, case_labels=case_labels,
-                                   y_label=FMT['sit_probability'],
-                                   file_label='',
-                                   # colors=FMT['colors'],
-                                   # markers=FMT['markers'],
-                                   y_min=0.
-                                   )
+        quantiles = np.array(FMT['percentiles']) / 100.
+        u_ds = m_xi.base.situation_prob_df(xi, groupby=sit_keys)
+        # = pd.Series object with MultiIndex axes [sample, *sit_keys]
+        q_ds = u_ds.groupby(level=list(sit_keys),
+                            sort=False).quantile(quantiles,
+                                                 numeric_only=True)
+        # = pd.Series object with MultiIndex axes [*sit_keys, quantiles]
+        tab_perc = fmt.tab_percentiles(q_ds)
+        fig_perc = fmt.fig_percentiles(tab_perc, y_label=FMT['sit_probability'], file_label='', y_min=0.)
         # ---------------------------------------- sit_keys differences
         # NOTE: Comparing CONDITIONAL probabilities of categories in FIRST sit_keys dimension,
         # GIVEN categories in other dimensions.
-        d = cred_diff(u, diff_axis=1, sample_axis=0, case_axis=2,
-                      p_lim=FMT['credibility_limit'])
-        diff_df = fmt.tab_credible_diff(d,
-                                        y_label=FMT['sit_probability'],
-                                        diff_head=sit_keys[0:1],
-                                        diff_labels=_product_labels(emf.situation_dtypes, sit_keys[0:1]),
-                                        cred_head=FMT['credibility'],
-                                        case_head=sit_keys[1:],
-                                        case_labels=_product_labels(emf.situation_dtypes, sit_keys[1:]),
-                                        )
+        d_pd = cred_pd.cred_diff(u_ds, diff_axis=sit_keys[0], case_axis=sit_keys[1:], p_lim=FMT['credibility_limit'])
+        tab_diff = fmt.tab_credible_diff(d_pd, diff_head=sit_keys[0:1], cred_head=FMT['credibility'],
+                                         case_head=sit_keys[1:], y_label=FMT['sit_probability'])
         # ---------------------------------------------------------------------
-        return cls(plot=perc, tab=df, diff=diff_df)
+        return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 class AttributeProfile(Profile):
     """Container for displays of ONE attribute value effect of situation(s),
     in ONE (Sub-)Population, OR for ONE respondent.
 
     NOTE: Latent-variable results are displayed for each Attribute,
@@ -576,56 +543,37 @@
     def display(cls, xi, m_xi, a_effect):
         """Create displays for a single attribute and requested situation effects
         :param xi: 2D array of parameter-vector samples drawn from m_xi
         :param m_xi: a population or individual model instance
         :param a_effect: tuple(attribute_key, sit_keys)
         :return: single cls instance with all displays
         """
-        # *** theta aggregation replaced by ema_base DataFrane access method ??? ********
-        emf = m_xi.base.emf
-        u = m_xi.base.situation_prob(xi)
-        u /= u.shape[1]  # = JOINT prob mass, incl. Phase: sum(u) == 1
         (a, sit_keys) = a_effect
-        # a = attribute key, sit_keys = tuple of situation keys
-        theta = m_xi.base.attribute_theta(xi, a)
-        # theta[s, k0, k1,...] = s-th sample of attribute a, given (k0, k1,...)-th situation
-        theta = aggregate_situation_theta(theta, u, emf, sit_keys)  # *** new attribute_theta_df method ??? ****
-        # theta[s, j0, j1,...] = s-th sample of attribute a,
-        #   given (situations[sit_keys[0]][j0], situations[sit_keys[1]][j1], ...)
+        # --------------------------------------- thresholds, optional:
         if FMT['grade_thresholds']:
             tau = np.median(m_xi.base.attribute_tau(xi, a), axis=0)
-            # tau[l] = l-th median rating threshold for attribute a
+            # tau[l] = l-th median rating threshold for attribute a, SAME for all situations
         else:
             tau = None
-        q = np.percentile(theta, FMT['percentiles'], axis=0)
         # --------------------------------------- percentile table:
-        case_labels = dict(_case_labels(emf.situation_dtypes, sit_keys))
-        df = fmt.tab_percentiles(q, perc=FMT['percentiles'],
-                                 case_labels=case_labels,
-                                 file_label=a
-                                 )
-        perc = fmt.fig_percentiles(df, case_labels=case_labels,
-                                   y_label=a + ' (' + str(FMT['scale_unit']) + ')',
-                                   file_label=a,  # *** needed ?
-                                   cat_limits=tau,
-                                   )
+        theta_ds =  m_xi.base.attribute_theta_df(xi, a, groupby=sit_keys)
+        # = pd.Series with MultiIndex [samples, *sit_keys]
+        quantiles = np.array(FMT['percentiles']) / 100.
+        theta_q = theta_ds.groupby(level=sit_keys, sort=False).quantile(quantiles)
+        tab_perc = fmt.tab_percentiles(theta_q, file_label=a)
+        fig_perc = fmt.fig_percentiles(tab_perc, y_label=a + ' (' + str(FMT['scale_unit']) + ')',
+                                       file_label=a,
+                                       cat_limits=tau)
         # ---------------------------------------- attr differences
-        # NOTE: comparing all situation-categories, in all requested sc dimensions
-        th_1 = theta.reshape((theta.shape[0], -1))
-        # all sit_keys dimensions flattened into th_1[:, 1]
-        d = cred_diff(th_1, diff_axis=1, sample_axis=0,
-                      p_lim=FMT['credibility_limit'])
-        diff_df = fmt.tab_credible_diff(d,
-                                        y_label=a,  # for table header
-                                        file_label=a,
-                                        diff_head=sit_keys,
-                                        diff_labels=_product_labels(emf.situation_dtypes, sit_keys),
-                                        cred_head=FMT['credibility'],
-                                        )
-        return cls(plot=perc, tab=df, diff=diff_df)
+        # NOTE: comparing all situation-categories, in all requested sit_keys dimensions
+        d_pd = cred_pd.cred_diff(theta_ds, diff_axis=sit_keys, p_lim=FMT['credibility_limit'])
+        tab_diff = fmt.tab_credible_diff(d_pd, diff_head=sit_keys, cred_head=FMT['credibility'],
+                                         y_label=a,
+                                         file_label=a)
+        return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 # --------------------------------- classes for differences between groups
 class GroupEffectSet:
     """Container for displays of differences between populations,
     as represented by participants in separate groups
     """
@@ -671,18 +619,16 @@
 
 class EmaGroupDiff:
     """Container for displays of differences between (Sub-)Populations
     represented by separate ema_model.EmaGroupModel instances.
     """
     def __init__(self, situations, attributes):
         """
-        :param situations: dict with (situation_tuple, SituationDiff instance), where
-            profile is a Profile instance for the selected situation_tuple
+        :param situations: dict with (situation_tuple, SituationDiff instance)
         :param attributes: dict with (attr_effect, AttributeDiff instance), where
-            profile is a Profile instance for the selected attr_effect
         """
         self.situations = situations
         self.attributes = attributes
 
     def save(self, path, **kwargs):
         """Save all stored display objects in specified (sub-)tree
         """
@@ -719,210 +665,94 @@
         """Generate a probability-profile display for selected distribution and factor
         :param xi: list of 2D arrays of parameter-vector samples
             len(xi) == len(emm.groups)
         :param emm: ema_model.EmaModel object
         :param sit_keys: tuple of one or more key(s) selected from emf.situation_dtypes.keys()
         :return: single cls instance
         """
-        emf = emm.base.emf
-        u = [emm.base.situation_prob(xi_g) for xi_g in xi]
-        # u[g][s, k0, k1, ...] = s-th sample of (k0, k1,...)-th situation prob in g-th population
-        for u_g in u:
-            u_g /= u_g.shape[1]  # = JOINT prob mass, incl. k0 = TestPhase index:
-            # sum(u_g) == 1
-        u = [aggregate_situation_prob(u_g, emf, sit_keys)
-             for u_g in u]
-        # Now with reordered and aggregated joint probabilities
-        # for selected subset of situation dimensions, such that
-        # u[g, s, j0, j1, ...] = s-th sample of joint probability for
-        # emf.situation_dtypes[sit_keys[0]][j0], emf.situation_dtypes[sit_keys[1]][j1], ... etc.
-        # file_name = '_'.join(sit_keys)
-        if len(sit_keys) > 1:
-            u_check = []
-            for u_g in u:
-                s = np.sum(u_g, axis=1, keepdims=True)
-                n_underflow = np.sum(s <= 0.)
-                if n_underflow > 0:
-                    logger.warning(f'SituationDiff display: {n_underflow} prob. sample(s) == 0. '
-                                   + 'Should not happen! Maybe too few responses?')
-                    s = np.maximum(s, np.finfo(float).tiny)
-                u_check.append(u_g / s)
-            u = u_check
-            # u = [u_g / np.sum(u_g, axis=1, keepdims=True)
-            #      for u_g in u]
-            # u[g][s, i, ...] = samples for CONDITIONAL probability of i-th category in sit_keys[0],
-            # GIVEN ...-th category product of sit_keys[1:]
-            u = [u_g.reshape((u_g.shape[0], -1))
-                 for u_g in u]
-            # now each u_g linear-indexed in 2D with
-            # u[g][s, j] = j-th product of sit_keys
-        # ---------------------------------------- sit_keys differences
-        # NOTE: Comparing CONDITIONAL probabilities of categories in FIRST sit_keys dimension,
-        # GIVEN categories in other dimensions.
-        d = cred_group_diff(u, sample_axis=0, case_axis=1,
-                            p_lim=FMT['credibility_limit'])
+        # --------------------------------- situation prob. vs (sit_keys, groups):
         group_head = [tuple(gk[0] for gk in g_key)
-                      for g_key in emm.groups]  # [0] all same
+                      for g_key in emm.groups][0] # [0] all same
         group_cat = [tuple(gk[1] for gk in g_key)
                      for g_key in emm.groups]
-        diff = fmt.tab_credible_diff(d,
-                                     y_label=FMT['sit_probability'],
-                                     diff_head=group_head[0],
-                                     diff_labels=group_cat,
-                                     case_head=sit_keys,
-                                     case_labels=_product_labels(emf.situation_dtypes, sit_keys),
-                                     cred_head=FMT['credibility'],
-                                     )
-        # ---------------------------------------------------------------------
-        return cls(diff=diff)
+        u_groups = {g: emm.base.situation_prob_df(xi_g, groupby=sit_keys)
+                    for (g, xi_g) in zip(group_cat, xi)}
+        # = dict of pd.Series objects, each with MultiIndex [sample, *sit_keys]
+        u_ds = pd.concat(u_groups, axis=0, names=list(group_head))
+        quantiles = np.array(FMT['percentiles']) / 100.
+        u_q = u_ds.groupby(level=list(sit_keys) + list(group_head),
+                           sort=False).quantile(quantiles,
+                                                numeric_only=True)
+        # = pd.Series with MultiIndex [*sit_keys, quantiles]
+        tab_perc = fmt.tab_percentiles(u_q)
+        fig_perc = fmt.fig_percentiles(tab_perc, y_label=FMT['sit_probability'], file_label='', y_min=0.)
+        # ---------------------------------------- group differences by sit_keys
+        # NOTE: Comparing CONDITIONAL probabilities of categories in FIRST sit_keys dimension,
+        # GIVEN categories in other dimensions.
+        d_pd = cred_pd.cred_group_diff(u_groups, group_axis=group_head,
+                                       case_axis=sit_keys,
+                                       p_lim=FMT['credibility_limit'])
+        tab_diff = fmt.tab_credible_diff(d_pd, diff_head=group_head, cred_head=FMT['credibility'], case_head=sit_keys,
+                                         y_label=FMT['sit_probability'])
+        return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 class AttributeDiff(Profile):
     """Container for all displays of group differences in ONE Attribute-by-Situation effect
     """
-    # **** allow several attributes in one display ? ***************
     @classmethod
     def display(cls, xi, emm, a_effect):
         """Create displays for a single attribute and requested situation effects
         :param xi: list of 2D arrays of parameter-vector samples
             len(xi) == len(emm.groups)
         :param a_effect: tuple (attr_key, sit_keys), where
             sit_keys is a tuple of one or more key(s) selected from emf.situation_dtypes.keys()
         :param emm: ema_model.EmaModel object
         :return: single cls instance
         """
-        emf = emm.base.emf
-        u = [emm.base.situation_prob(xi_g) for xi_g in xi]
-        # u[g][s, k0, k1, ...] = s-th sample of (k0, k1,...)-th situation prob in g-th population
-        for u_g in u:
-            u_g /= u_g.shape[1]  # = JOINT prob mass, incl. k0 = TestPhase index:
-            # sum(u_g) == 1
-        (a, sc) = a_effect
-        # a = attribute key, sit_keys = tuple of situation keys
-        # file_name = a + '_vs_' + '*'.join(sc)
-        theta = [emm.base.attribute_theta(xi_g, a)
-                 for xi_g in xi]
-        # theta[g][s, k0, k1,...] = s-th sample of attribute a, given (k0, k1,...)-th situation
-        theta = [aggregate_situation_theta(theta_g, u_g, emf, sc)
-                 for (theta_g, u_g) in zip(theta, u)]
-        # theta[s, j0, j1,...] = s-th sample of attribute a,
-        #   given (situations[sit_keys[0]][j0], situations[sit_keys[1]][j1], ...)
-        #   averaged across OTHER situations, weighted by situation-probabilities.
-        # ---------------------------------------- attr differences
-        # NOTE: comparing all situation-categories, in all requested sc dimensions
-        th_1 = [theta_g.reshape((theta_g.shape[0], -1))
-                for theta_g in theta]
-        # all sit_keys dimensions flattened into th_1[g][s, :]
-        d = cred_group_diff(th_1, sample_axis=0, case_axis=1,
-                            p_lim=FMT['credibility_limit'])
+        (a, sit_keys) = a_effect
+        if FMT['grade_thresholds']:
+            tau = np.array([emm.base.attribute_tau(xi_g, a)
+                     for xi_g in xi])
+            # tau[g, s, :] = s-th sample of threshold array for g-th group
+            tau = tau.reshape((-1, tau.shape[-1]))
+            # tau[gs, :] = gs-th sample across all groups
+            tau = np.median(tau, axis=0)
+            # tau[l] = l-th median rating threshold for attribute a
+        else:
+            tau = None
+        # --------------------------------------- percentile table
         group_head = [tuple(gk[0] for gk in g_key)
-                      for g_key in emm.groups]  # [0] all same
+                      for g_key in emm.groups][0]  # [0] all same
         group_cat = [tuple(gk[1] for gk in g_key)
                      for g_key in emm.groups]
-        diff = fmt.tab_credible_diff(d,
-                                     y_label=a,
-                                     file_label=a,
-                                     diff_head=group_head[0],
-                                     diff_labels=group_cat,
-                                     case_head=sc,
-                                     case_labels=_product_labels(emf.situation_dtypes, sc),
-                                     cred_head=FMT['credibility'],
-                                     # high_low=FMT['high_low'],
-                                     # and_head=FMT['and_head']
-                                     )
-        # ---------------------------------------------------------------------
-        return cls(diff=diff)
+        theta_groups = {g: emm.base.attribute_theta_df(xi_g, a, groupby=sit_keys)
+                        for (g, xi_g) in zip(group_cat, xi)}
+        theta_ds = pd.concat(theta_groups, axis=0, names=list(group_head))
+        quantiles = np.array(FMT['percentiles']) / 100.
+        theta_q = theta_ds.groupby(level=list(sit_keys) + list(group_head),
+                                    sort=False).quantile(quantiles,
+                                                         numeric_only=True)
+        tab_perc = fmt.tab_percentiles(theta_q, file_label=a)
+        fig_perc = fmt.fig_percentiles(tab_perc, y_label=a + ' (' + str(FMT['scale_unit']) + ')', file_label=a,
+                                       cat_limits=tau)
+        # ---------------------------------------- attribute differences between groups
+        # NOTE: comparing all situation-categories, in all requested sc dimensions
+        d_pd = cred_pd.cred_group_diff(theta_groups,
+                                       group_axis=group_head,
+                                       case_axis=sit_keys,
+                                       p_lim=FMT['credibility_limit'])
+        tab_diff = fmt.tab_credible_diff(d_pd, diff_head=group_head,
+                                         cred_head=FMT['credibility'],
+                                         case_head=sit_keys,
+                                         y_label=a, file_label=a)
+        return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 # ---------------------------------- Help functions:
-def aggregate_situation_prob(u, emf, sc):
-    """Aggregate probability-mass samples to keep only selected factor axes
-    :param u: multi-dim array with probability-mass samples
-        u[s, k0, k1,...] = s-th sample of JOINT prob
-            for (k0, k1,...)-th situation, as defined by emf.situation_dtypes.items()
-        u.shape == (n_samples, *emf.situation_shape)
-    :param emf: ema_data.EmaFrame instance for model generating u
-    :param sc: tuple with selected situation keys to display
-    :return: array uf with aggregated joint probabilities
-        uf[s, j0, j1, ...] = s-th sample of joint probability for
-        situation[sc[0]][j0], situation[sc[1]][j1], ... etc.
-        uf.shape == (u.shape[0], *emf.situation_shape[emf.situation_axes(sc)])
-    """
-    axes = tuple(1 + i for i in emf.situation_axes(sc))
-    uf = np.moveaxis(u, axes, tuple(range(1, 1+len(axes))))
-    # with desired sit_keys axes first after 0
-    sum_axes = tuple(range(1+len(axes), uf.ndim))
-    uf = np.sum(uf, axis=sum_axes)
-    # summed across all OTHER axes, except those in sit_keys
-    return uf
-
-
-def aggregate_situation_theta(th, u, emf, sc):
-    """Aggregate attribute location sample arrays to keep only selected factor axes
-    :param th: multi-dim array with attribute-location samples
-        th[s, k0, k1,...] = s-th sample of latent variable theta
-            in (k0, k1,...)-th situation, as defined by emf.situation_dtypes.items()
-        th.shape == (n_samples, *emf.situation_shape)
-    :param u: multi-dim array with corresponding samples of normalized situation probabilities
-        u[s, k0, k1, ...] = s-th sample of normalized probability of (k0, k1,...)-th situation
-        sum_(k0, k1, ...) u[s, k0, k1, ...] == 1, for all s
-        u.shape == th.shape
-    :param emf: ema_data.EmaFrame instance for model generating u
-    :param sc: tuple with selected situation keys to display
-    :return: th_a = array with aggregated attribute locations
-        th_a[s, j0, j1, ...] = s-th sample of conditional attribute location,
-        GIVEN situation[sc[0]][j0], situation[sc[1]][j1], ... etc.
-        averaged across all OTHER situation_dtypes not included in sc.
-        th_a.shape == (n_samples, *emf.situation_shape[emf.situation_axes(sc)])
-
-    2021-12-17, probability-averaged across non-included situation_dtypes
-    """
-    keep_axes = tuple(1 + i for i in emf.situation_axes(sc))
-    w = np.sum(u, axis=keep_axes, keepdims=True)
-    # = normalized situation prob, for every sample
-    th = np.moveaxis(th, keep_axes, tuple(range(1, 1 + len(keep_axes))))
-    w = np.moveaxis(w, keep_axes, tuple(range(1, 1 + len(keep_axes))))
-    # th and w now with desired sit_keys axes first after sample-axis = 0
-    aggregate_axes = tuple(range(1+len(keep_axes), th.ndim))
-    # = all OTHER axes, except those in sit_keys
-    # th_old = np.mean(th, axis=aggregate_axes)
-    # # averaged across all aggregate_axes. version <= 0.6
-    th = np.sum(th * w, axis=aggregate_axes)
-    # = probability-averaged across all aggregate_axes. version >= 0.7
-    return th
-
-
-def _case_labels(label_dict, key_list):  # v 0.9
-    """Selected case Labels
-    :param label_dict: a dict with elements (factor_key, factor_cat), where
-        factor_key is a key to a EmaFrame situation_dtypes or attribute_grades,
-        factor_cat is a pd.CategoricalDtype instance defining factor_key categories
-    :param key_list: sequence of factor_key cases to be included
-    :return: labels = list of tuples, with
-        i-th tuple = (key_list[i], label_dict[key_list[i].categories)
-    """
-    # **** return dict instead ??? **************
-    return [(gf, label_dict[gf].categories) for gf in key_list]
-
-
-def _product_labels(label_dict, key_list):  # v 0.9
-    """Iterator of tuples, each
-    a product of one category from each desired factor dimension
-    :param label_dict: a dict with elements (factor_key, factor_cat), where
-        factor_key is a key to a EmaFrame situation_dtypes or attribute_grades,
-        factor_cat is a pd.CategoricalDtype instance defining factor_key categories
-    :param key_list: list of keys to label_dict
-    :return: labels = list with tuples, with
-        ...-th tuple = (label_dict[keys[0][i0], ..., label_dict[keys[D][iD])
-        where D = len(keys)
-        with last index iD varying fastest, i0 slowest, in the product tuples
-    """
-    return [*product(*(label_dict[gf].categories for gf in key_list))]
-
-
 def _dir_name(g, sep='_'):
     """make sure group name is a possible directory name
     :param g: string or tuple of strings
     :return: string to be used as directory
     """
     if type(g) is tuple:  # several strings
         g = sep.join(_dir_name(g_s, sep='_')
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_display_format.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_display_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 Plot properties may be controlled by
 1: specifying matplotlib style sheet(s) by keyword argument mpl_style
 2: setting specific matplotlib parameters at runtime by keyword argument mpl_params
 3: setting specific parameters in FMT, e.g., 'colors' and 'markers'
 
 *** Version History:
+* Version 0.9.6:
+2023-04-16, some plot parameters -> FMT for user control
+2023-04-12, new simplified tab_percentle_pd, tab_credible_difference_pd
+2023-03-31, new help function make_product_name *** NO LONGER NEEDED
+
 * Version 0.9.5:
 2023-03-07, fig_category_barplot allow both observed and model-predicted quantile data
 
 * Version 0.9.4:
 2023-01-22, Bug fix in output file name creation, to avoid problem under Windows.
             Added 'interaction_sep' and 'condition_sep' in FMT dict, for user control.
             Added try...catch for any errors in ResultPlot.save() and ResultTable.save()
@@ -38,53 +43,47 @@
 2022-01-13, changed EmaDisplaySet.show format argument: show_intervals -> grade_thresholds
 
 * Version 0.7:
 2021-12-19, function nap_table to format NAP results
 
 2021-11-07, copied and modified PairedCompCalc -> EmaCalc
 """
-# *** AVOID explicit plot-style commands, rely on rcParams or style sheets instead
-# *** Try package pathvalidate to check that result filenames are allowed ? ***
-# *** Or just try...catch ?
-
 import numpy as np
-from itertools import cycle, product
+from itertools import cycle
 import matplotlib.pyplot as plt
 import logging
 import pandas as pd
 
 from .ema_file import Table
 
-# plt.rcParams.update({'figure.max_open_warning': 0})
-# suppress warning for many open figures
-# plt.rcParams.update({'axes.labelsize': 'x-large'})  # use kwarg mpl_params instead
-# plt.rcParams.update({'axes.labelweight': 'bold'})
-
 logger = logging.getLogger(__name__)
 
 
-FMT = {'colors': 'rbgk',  # to distinguish results in plots, cyclic use
+FMT = {'colors': 'rbgk',    # to distinguish results in plots, cyclic use
        'markers': 'oxs*_',  # corresponding markers, cyclic use
+       'x_space': 0.3,      # clean space between x_tick categories
        'interaction_sep': '\u00D7',  # mult.sign. separating situation labels in result file names
-       'condition_sep': '_',  # separating attribute and its conditioning situation(s) in file names
+       'condition_sep': '_',    # separating attribute and its conditioning situation(s) in file names
+       'max_plot_cases': 30,    # max cases in percentile plots
+       'max_case_heads': 2,     # limit in plot legends
        }
 
 # NOTE: FMT['colors'] and FMT['markers'] override matplotlib.rcParams.axes.prop_cycle,
 #   because prop_cycle allows only equal lengths of 'colors' and 'markers'.
 #   The FMT['colors'] and FMT['markers'] are used cyclically,
 #   so the default sequences with unequal lengths will combine
 #   into a sequence with many combinations, before repeating itself.
 
 
 def set_format_param(mpl_style=None, mpl_params=None, **kwargs):
     """Set / modify format parameters.
     Called before any displays are generated.
     :param mpl_style: (optional) matplotlib style sheet, or list of style sheets
     :param mpl_params: (optional) dict with matplotlib (k, v) rcParam settings
-    :param kwargs: dict with any formatting variables
+    :param kwargs: dict with any formatting variables to be stored in FMT
     :return: None
     """
     if mpl_style is not None:
         plt.style.use(mpl_style)
     if mpl_params is not None:
         plt.rcParams.update(mpl_params)
     other_fmt = dict()
@@ -115,15 +114,15 @@
     def fig(self):
         return self.ax.figure
 
     def save(self, path,
              figure_format,
              **kwargs):
         """Save figure to given path
-        :param path: Path to directory where figure has been saved
+        :param path: Path to directory for saving self
         :param figure_format: figure-format string code -> file-name suffix
         :param kwargs (optional) any additional kwargs, *** NOT USED ***
         :return: None
         """
         # *** select subset of kwargs allowed by savefig() ?
         # NO, depends on Matplotlib backend!
         f = (path / self.name).with_suffix('.' + figure_format)
@@ -177,119 +176,126 @@
             kwargs['index'] = False  # override Pandas default = True
         super().save(path, **kwargs)
 
 
 # ---------------------------------------- Formatting functions:
 
 def fig_percentiles(df,
-                    case_labels,
                     y_label='',
                     file_label='',
                     cat_limits=None,
-                    x_space=0.3,
-                    colors=FMT['colors'],
-                    markers=FMT['markers'],
                     y_min=None,
                     y_max=None,
                     **kwargs):
     """create a figure with percentile results
     as defined in a given pd.DataFrame instance
     :param df: pd.DataFrame instance with primary percentile data, with
-        one row for each case category, as defined in df.index elements
+        one row for each case category, as defined in df.index.values elements,
         one column for each percentile value.
-    :param case_labels: dict with elements (case_factor_i, case_labels_i),
-        that were used to construct table df, with
-        case_factor_i = key string for i-th case dimension,
-            = name of i-th level of df.index
-        case_labels_i = list of labels for i-th case dimension
-            = categories in df.index.levels[i]
-        df.n_rows == prod_i len(case_labels_i)
+    :param x_label: (optional) string for x-axis label, instead of df.index.names[0]
+    :param x_tick_labels: (optional) list of x tick labels, instead of df.index.levels[0]
+    :param y_label: (optional) string for y-axis label
     :param y_label: (optional) string for y-axis label
     :param cat_limits: 1D array with response-interval limits (medians)
     :param file_label: (optional) string as first part of file name
-    :param x_space: (optional) min space outside min and max x_tick values
     :param colors: (optional) sequence of color codes to separate results in plots
     :param markers: (optional) sequence of marker codes to separate results in plots
         len(colors) != len(markers) -> many different combinations
     :param y_min: (optional) enforced lower limit of vertical axis
     :param y_max: (optional) enforced upper limit of vertical axis
     :param kwargs: (optional) dict with any additional keyword arguments for plot commands.
     :return: ResultPlot instance with plot axis with all results
     NOTE: plot will use df.index.level[0] categories as x-axis labels,
     and index.level[1:] as plot labels in the legend
     """
-    def plot_one_case(case_i, x, y_i, c, m):
+    # ----------------------------------- set up plot design:
+    # x_space = FMT['x_space']
+    if df is None:
+        return None
+    if df.index.nlevels == 1:
+        x_label = df.index.name
+        x_tick_labels = list(df.index.values)
+        case_head = ()
+        case_list = [()]
+    elif df.index.nlevels == 2:
+        x_label = df.index.names[0]
+        x_tick_labels = list(dict.fromkeys([c[0] for c in df.index.values]))
+        case_head = df.index.names[1]
+        case_list = list(dict.fromkeys([c[1] for c in df.index.values]))
+    else:
+        x_label = df.index.names[0]
+        x_tick_labels = list(dict.fromkeys([c[0] for c in df.index.values]))
+        case_head = tuple(df.index.names[1:])
+        case_list = list(dict.fromkeys([c[1:] for c in df.index.values]))
+        # in order as appearing in df
+    if df.shape[0] > FMT['max_plot_cases']:
+        logger.warning(f'Too many {x_label}, {case_head} cases to plot. Increase max_plot_cases if necessary.')
+        return None
+    n_cases = len(case_list)
+    dx = (1. - FMT['x_space']) / n_cases
+    # = x step between range plots for separate cases
+    x_offset = {c: (i - (n_cases - 1) / 2) * dx
+                for (i, c) in enumerate(case_list)}
+    case_color = {c: col for (c, col) in zip(case_list, cycle(FMT['colors']))}
+    case_marker = {c: mark for (c, mark) in zip(case_list, cycle(FMT['markers']))}
+    # ------------------------------------------------------------------------
+    def plot_one(ax, row_index, y):
         """
-        :param case_i: case label
-        :param x: 1D array with x values
-        :param y_i: 2D array with y values
-            y_i[p, i] = p-th percentile value for x[i]
-            len(x) == y_i.shape[-1]
-        :param c: color code
-        :param m: marker code
+        :param ax: axis for plot
+        :param row_index: index label(s) for ONE row in df
+        :param y: 1D array with corresponding y = values in ONE row
+            y[p] = p-th percentile value
         :return: None
         """
-        n_perc = y_i.shape[0]
-        if n_perc == 1:  # only marker
-            line = ax.plot(x, y_i[0],
+        if df.index.nlevels == 1:
+            x_tick = row_ind
+            x_case = ()
+        elif df.index.nlevels == 2:
+            x_tick = row_ind[0]
+            x_case = row_ind[1]
+        else:
+            x_tick = row_ind[0]
+            x_case = row_ind[1:]
+        x = x_tick_labels.index(x_tick) + x_offset[x_case]
+        x = x * np.ones_like(y)
+        c = case_color[x_case]
+        m = case_marker[x_case]
+        if len(y) == 1:  # only single marker
+            line = ax.plot(x, y,
                            linestyle='', color=c,
                            marker=m, markeredgecolor=c, markerfacecolor='w',
                            **kwargs)
-        elif n_perc == 2:  # only vertical range, no markers
-            line = ax.plot(np.tile(x, (2, 1)),
-                           y_i,
+        elif len(y) == 2:  # vertical range, no markers
+            line = ax.plot(x, y,
                            linestyle='solid', color=c,
                            marker=m, markeredgecolor=c, markerfacecolor='w',
                            **kwargs)
         else:  # vertical range, and markers for intermediate percentiles
-            ax.plot(np.tile(x, (2, 1)),
-                    [y_i[0], y_i[-1]],
+            y = sorted(list(y))
+            ax.plot([x[0], x[-1]], [y[0], y[-1]],
                     linestyle='solid', color=c,
                     **kwargs)
-            line = ax.plot(np.tile(x, (y_i.shape[0] - 2, 1)),
-                           y_i[1:-1],
-                           linestyle='solid', color=c,
+            line = ax.plot(x[1:-1], y[1:-1],
+                           linestyle='solid', color=c,  # to get line+marker into label
                            marker=m, markeredgecolor=c, markerfacecolor='w',
                            **kwargs)
-        line[0].set_label(str(case_head) + '=' + str(case_i))
-    # ----------------------------------------------------------
+        if x_tick == x_tick_labels[0]:
+            if type(case_head) is tuple and len(case_head) > FMT['max_case_heads']:
+                line[0].set_label(str(x_case))
+            else:
+                line[0].set_label(str(case_head) + '=' + str(x_case))
 
-    case_keys = [*case_labels.keys()]
-    case_cats = [*case_labels.values()]
-    # *** df.index.levels are NOT used because they are sorted alphabetically, NOT in tabulated order
-    assert df.shape[0] == np.prod([len(cc_i) for cc_i in case_cats]), 'case_labels must match df size'
-    x_label = case_keys[0]
-    x_tick_labels = list(case_cats[0])
-    if len(case_keys) == 1:
-        (case_head, case_list) = ('', [''])  # make ONE empty sub-case to facilitate indexing
-    elif len(case_keys) == 2:
-        (case_head, case_list) = (case_keys[1], case_cats[1])
-    else:
-        (case_head, case_list) = (case_keys[1:], [*product(*case_cats[1:])])
-    n_cases = len(case_list)
     # ------------------------------------------------------------------
     fig, ax = plt.subplots()
-    dx = (1. - x_space) / n_cases
-    # = x step between range plots for separate cases
-    x = np.arange(len(x_tick_labels)) - (n_cases - 1) * dx / 2
-    # = x position for first case
-    if df.index.nlevels == 1:
-        plot_one_case('', x, df.loc[x_tick_labels].values.T,
-                      colors[0], markers[0])
-    else:
-        for (case_i, c, m) in zip(case_list,
-                                  cycle(colors),
-                                  cycle(markers)):
-            y_i = df.xs(case_i, level=case_head)
-            y_i = y_i.loc[x_tick_labels].values.T
-            plot_one_case(case_i, x, y_i, c, m)
-            x += dx
+    for (row_ind, y) in df.iterrows():
+        plot_one(ax, row_ind, y)
+
     (x_min, x_max) = ax.get_xlim()
-    x_min = min(x_min, -x_space)
-    x_max = max(x_max, len(x_tick_labels) - 1 + x_space)
+    x_min = min(x_min, -FMT['x_space'])
+    x_max = max(x_max, len(x_tick_labels) - 1 + FMT['x_space'])
     ax.set_xlim(x_min, x_max)
     if cat_limits is not None:
         _plot_response_intervals(ax, cat_limits)
     ax.set_xticks(np.arange(len(x_tick_labels)))
     xticks = [str(c) for c in x_tick_labels]
     ax.set_xticklabels(xticks,
                        **_x_tick_style(xticks))
@@ -323,15 +329,14 @@
 
 
 def fig_category_barplot(df,
                          x_label,
                          y_label,
                          df_q=None,
                          file_label='',
-                         colors=FMT['colors'],
                          y_min=None,
                          y_max=None,
                          mpl_params=None,  # *** not needed? called only from ema_display ***
                          **kwargs
                          ):
     """Bar plot of DataFrame values,
     to be displayed with one sequence of vertical bars along x-axis for each row,
@@ -340,50 +345,48 @@
     :param df: a DataFrame instance,
         one row for each selected situation category, one column for each grade
     :param df_q: (optional) DataFrame instance with quantiles
         similar to df, but expanded with one row for each (situation category, quantile)
     :param x_label: x-axis label string
     :param y_label: y-axis label string
     :param file_label: plot name for saving file
-    :param colors: (optional) color sequence
     :param y_min: (optional) enforced lower limit of vertical axis *** NOT USED
     :param y_max: (optional) enforced upper limit of vertical axis *** NOT USED
     :param mpl_param: (optional) dict with matplotlib rcParam settings
     :param kwargs: (optional) dict with keyword arguments for plot commands *** NOT USED
     :return: a ResultPlot instance
     """
     if mpl_params is not None:
         plt.rcParams.update(mpl_params)
     fig, ax = plt.subplots()
     assert df.ndim > 1, 'Input must be DataFrame'
-    # if df.ndim == 1:  # just a series, convert to a single row, Checked externally!!! ******
-    #     df = df.to_frame().T  # **** better to use transposed input like DataFrame.plot.hist *****
-    #     if df_q is not None:
-    #         fill_value = df.index.values[0]
-    #         i = ((fill_value, q) for q in df_q.index.values)
-    #         df_q = df_q.set_index(keys=i)
     (n_cases, n_x) = df.shape
     x = np.arange(n_x)
     bar_space = 0.02  # space to allow all bar edges to be visible
     w = 0.8 / n_cases - bar_space
     if len(df.index.names) > 1:
         case_head = tuple(df.index.names)
     else:
         case_head = df.index.name
     x_dev = (w + bar_space) * (np.arange(n_cases) - (n_cases - 1) / 2)
     for (d, c, case) in zip(x_dev,
-                            cycle(colors),
+                            cycle(FMT['colors']),
                             df.index.values):
         y = df.loc[case].to_numpy()
+        # *** check case_head vs FMT['max_case_head'] ***
+        if type(case_head) is tuple and len(case_head) > FMT['max_case_heads']:
+            case_legend = str(case)
+        else:
+            case_legend = str(case_head) + '= ' + str(case)
         ax.bar(x + d, height=y,
                width=w, edgecolor=c, facecolor='w',  # ************
-               label=str(case_head) + '= ' + str(case))
+               label=case_legend)
     if df_q is not None:
         for (d, c, case) in zip(x_dev,
-                                cycle(colors),
+                                cycle(FMT['colors']),
                                 df.index.values):
             y = df_q.loc[case].to_numpy()
             ax.plot(np.tile(x + d, (len(y),1)), y, '-', color=c, linewidth=2)
     ax.set_xticks(np.arange(n_x))
     xticks = [str(c) for c in df.columns.values]
     ax.set_xticklabels(xticks,
                        **_x_tick_style(xticks))
@@ -396,130 +399,95 @@
         f_name = file_label
     fig.set_tight_layout(tight=True)
     return ResultPlot(ax, name=f_name)
 
 
 # ----------------------------------------- table displays:
 
-def tab_percentiles(q_perc,
-                    perc,
-                    case_labels,
-                    file_label=''
-                    ):
-    """Create pd.DataFrame with all percentile results.
-    This function is general and can handle any dimensionality of the data.
-    :param q_perc: 2D or mD array with quality percentiles, stored as
-        q_perc[p, c0,...] = p-th percentile in (c0,...)-th case condition
-    :param perc: sequence of percentage values in range 0-100
-        len(perc) == q_perc.shape[0]
-    :param case_labels: (sequence OR ???) dict with elements (case_factor_i, case_labels_i), where
-        case_factor_i is key string for i-th case dimension,
-        case_labels_i is list of labels for i-th case dimension
-        in the same order as the index order of q_perc, i.e.,
-        len(case_labels_i) == q_perc.shape[i+1].
-        Thus, q_perc[p, ...,c_i,...] = p-th percentile for case_labels_i[c_i], i = 0,...,
+def tab_percentiles(q_ds, file_label=''):
+    """Re-format a pd.DataFrame with percentile results.
+    :param q_ds: a pd.Series instance with quantiles as last index axis,
+        and cases in other index axes.
     :param file_label: (optional) string as first part of file name
     :return: a ResultTable(pd.DataFrame) instance,
         with one column for each percentile,
-        and one row for each combination product of case labels.
-        Number of table rows == prod q_perc.shape[1:] == prod_i len(case_labels_i)
+        and one row for each combination product of cases considered.
     """
-    case_labels = dict(case_labels)  # if not already dict, *** require dict ? ******
-    case_shape = tuple(len(c_labels) for c_labels in case_labels.values())
-    n_rows = np.prod(case_shape, dtype=int)
-    # = number of table rows as defined by case_labels
-    n_perc = len(perc)
-    assert n_perc == q_perc.shape[0], 'Incompatible q_perc.shape[0] != n of percentiles'
-    assert n_rows == np.prod(q_perc.shape[1:], dtype=int), 'Incompatible size of case_list and q_perc'
-    assert case_shape == q_perc.shape[1:], 'Incompatible shape of q_perc and case_labels'
-    df = pd.DataFrame({f'{p_i:.1f}%': q_i
-                       for (p_i, q_i) in zip(perc,
-                                             q_perc.reshape((n_perc, -1)))},
-                      index=pd.MultiIndex.from_product([*case_labels.values()],
-                                                       names=[*case_labels.keys()]))
+    tab_perc = q_ds.unstack()
+    case_head = tab_perc.index.names
+    tab_perc.columns = [f'{q:.1%}' for q in tab_perc.columns]
     if len(file_label) > 0:
         file_label += FMT['condition_sep']
-    f_name = file_label + FMT['interaction_sep'].join(case_labels.keys())
-    return ResultTable(df, name=f_name)
+    f_name = file_label + FMT['interaction_sep'].join(case_head)
+    return ResultTable(tab_perc, name=f_name)
 
 
 def tab_credible_diff(diff,
-                      diff_labels,
                       diff_head,
                       cred_head,
-                      case_labels=(),
                       case_head=(),
                       y_label='',
                       file_label='',
-                      and_label='and',  # label in And column
-                      and_head=('', '')
+                      and_label='and',  # label in And column  -> FMT ***
+                      and_head=('', '')  # -> FMT ***
                       ):
-    """Create table with credible differences among results
-    :param diff: list of tuples ((i,j), p) OR ((i,j,c), p),
+    """Create table with credible differences among results -- pandas version
+    :param diff: list of tuples (((i,j), c0,...), p),
         defining jointly credible differences, indicating that
-        prob{ quality of diff_labels[i] > quality of diff_labels[j]}, OR
-        prob{ quality of diff_labels[i] > quality of diff_labels[j] | case_labels[c] }
+        prob{ quality of diff catgory i > quality of category j, given case category c
         AND all previous pairs } == p
-    :param diff_labels: list of tuples with labels of compared random-vector elements
-        diff_labels[i] = (label_0,...)
-        diff[...] == ((i,j, c), p) <=> diff_labels[i] > diff_labels[j] with prob p,
-            at case_labels[c], if case_labels are defined.
-        len(diff_labels) == max possible diff category index (i, j)
+        i, j are either a string label or a tuple of such labels
+        c0,... is one or more case labels
     :param diff_head: tuple of keys for heading of diff_labels column in table
-        len(diff_head) == len(diff_labels[i]) for all i
+        len(diff_head) == len(i) == len(j) if tuple, or len(diff_head) == 1
     :param cred_head: string for header of Credibility column
-    :param case_labels: (optional) sequence of tuples
-        case_labels[c] == (case_label1, case_label2, ...), such that
-        diff[...] == ((i,j, c), p) <=> diff[...] is valid given case_labels[c]
-        len(case_labels) == max possible case index c in diff
     :param case_head: (optional) tuple of case keys, one for each case-dimension table column
-        len(case_head) == len(case_labels[c]) for any c
+        len(case_head) == len(c0,...)
     :param y_label: (optional) string with label of tabulated attribute
     :param file_label: (optional) string for first part of file name
     :param and_label: (optional) joining AND label in first column
     :param and_head: (optional) tuple with two strings for head first column
     :return: ResultTable object with header lines + one line for each credible difference
     """
     if len(diff) == 0:
         return None
     y_head_i = y_label + ' >'
     y_head_j = y_label
     # --------------------- table columns as dicts:
     col = {and_head:  [' '] + [and_label] * (len(diff) - 1)}  # first column with only AND flags
+    diff_i = [(ijc[0][0] if type(ijc[0][0]) is tuple else (ijc[0][0],)) for (ijc, p) in diff]
+    diff_j = [(ijc[0][1] if type(ijc[0][1]) is tuple else (ijc[0][1],)) for (ijc, p) in diff]
+    diff_c = [ijc[1:] for (ijc, p) in diff]
+    diff_p = [p for (ijc, p) in diff]
     # --------- column(s) for higher results:
-    diff_i = [diff_labels[d[0][0]]
-              for d in diff]
-    col |= {(y_head_i, d_head_k): [d_val[k] for d_val in diff_i]
+    col |= {(y_head_i, d_head_k): [d[k] for d in diff_i]
             for (k, d_head_k) in enumerate(diff_head)}
     # --------- column(s) for lower results:
-    diff_j = [diff_labels[d[0][1]]
-              for d in diff]
-    col |= {(y_head_j, d_head_k): [d_val[k] for d_val in diff_j]
+    col |= {(y_head_j, d_head_k): [d[k] for d in diff_j]
             for (k, d_head_k) in enumerate(diff_head)}  # cols for lesser results
     # --------- column(s) for optional case labels:
     if len(case_head) > 0:
-        diff_c = [case_labels[d[0][2]]
-                  for d in diff]
-        col |= {('', c_head_k): [c_val[k] for c_val in diff_c]
+        # diff_c = [case_labels[d[0][2]]
+        #           for d in diff]
+        col |= {('', c_head_k): [d[k] for d in diff_c]
                 for (k, c_head_k) in enumerate(case_head)}
     # --------- credibility column:
-    col |= {('', cred_head): [d[1] for d in diff]}
-    df = pd.DataFrame(col)
+    col |= {('', cred_head): diff_p}
+    df = pd.DataFrame(col)  # do all this in samppy.credibility_pd ? ***********
     # each column name is a tuple with two elements -> MultiIndex with two levels
-    df = df.reindex(columns=pd.MultiIndex.from_tuples(df.columns))
+    # df = df.reindex(columns=pd.MultiIndex.from_tuples(df.columns))  # ****** Needed ?
     if len(file_label) > 0:
         file_label += FMT['condition_sep']
     f_name = file_label + FMT['interaction_sep'].join(diff_head) + '-diff'
     if len(case_head) > 0:
         f_name += FMT['condition_sep'] + FMT['interaction_sep'].join(case_head)
     return DiffTable(df, name=f_name)
 
 
 # -------------------------------------- display adjustment functions
-
 def harmonize_ylim(axes_list, y_min=None, y_max=None):
     """Adjust several plots to equal vertical range
     :param axes_list: sequence of plt.Axes instances
     :param y_min: (optional) extra user-defined minimum
     :param y_max: (optional) extra user-defined maximum
     :return: None
     """
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_file.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_file.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_group.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_group.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_latent.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_latent.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_logging.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_logging.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_model.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_model.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_nap.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_nap.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         rows MultiIndex-ed by elements of group_cols, and
         columns MultiIndex-ed as (g_i, low), (g_i, nap), (g_i, high), where
             g_i is a grade label in grade_cols, and
             low is the lower conf.interval limit
             nap is the NAP point estimate,
             high is the upper conf.interval limit
         All calculated values show NAP for Second re. First category in col.
+        Result table is sorted by categories in group_cols.
     """
     def calc_nap(group_name, group_df):
         """Calculate NAP results for given (sub-grouped) DataFrame
         :param group_name: single column or tuple of column names to mark in result
         :param group_df: a pd.DataFrame object
         :return: a dict with all NAP results as (key, value) pairs
         """
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_respondent.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_respondent.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
             for which separate attribute-counts are calculated.
             Counts are summed across any OTHER situation dimensions.
         :param sample_head: (optional) header name for sample index
         :return: a pd.DataFrame object with all grade counts,
             with one row for each (sample, *groupby) multi-index combination
             and one column for each grade category.
         """
-        # *** use only total observed count to estimate situation-count distribution ? *********
+        # *** use only total observed count to estimate situation-count distribution ! *********
         emf = self.base.emf
         a_index = list(emf.attribute_dtypes.keys()).index(a)
         if groupby is None:
             groupby = []
         elif isinstance(groupby, str):
             groupby = [groupby]
         theta = self.base.attribute_theta(self.xi, a)
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_simulation.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_simulation.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/ema_thresholds.py` & `EmaCalc-0.9.6/src/EmaCalc/ema_thresholds.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/gauss_gamma.py` & `EmaCalc-0.9.6/src/EmaCalc/gauss_gamma.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.5/src/EmaCalc/run_ema.py` & `EmaCalc-0.9.6/src/EmaCalc/run_ema.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                          )
     # NOTE: situations and attributes keys will be parts of result file names,
     # so they can include only characters allowed in file names.
 
     # NOTE: situations and attributes always analyzed as Categorical variables,
     # even if the categories / grades are defined by numeric labels.
     # The rank order of attribute grades is defined by the order as listed here,
-    # not by, e.g., alphabetical or numerical order of the grade labels.
+    # NOT by, e.g., alphabetical or numerical order of the grade labels.
 
     # NOTE: if EQUAL grades are used for more than one attribute,
     # the model still assumes separate rating scales for each attribute.
     # However, if grade sequences are IDENTICAL objects for more than one attribute,
     # the model uses the SAME rating scale for those attributes.
     #
     # Example:
@@ -118,15 +118,15 @@
     #                         'Hard',
     #                         'Easy',
     #                         'Very Easy',
     #                         'Perfect']
     # emf = EmaFrame.setup(situations=situations,
     #                      phase_key='Phase',
     #                      attributes={'Speech': common_ordinal_scale,
-    #                                  'Comfort': common_ordinal_scale}
+    #                                  'Comfort': common_ordinal_scale}  # SAME scale for both attributes
     #                      )
 
     # In either case, response thresholds are always estimated separately for each participant.
 
     # ------ 2: Load data from previously saved file(s):
 
     # NOTE: if 'grouping' is defined, group directory names must match given labels,
@@ -134,30 +134,30 @@
     # With template example: data_path / 'Age_old' is top of directory tree with data files.
     # If several 'grouping' factors are defined, the directory tree structure must match the factors.
     # If no grouping is defined: data_path is top of directory tree with all data files
 
     ds = EmaDataSet.load(emf, data_path,
                          # fmt='csv',  # None: try any file format
                          # grouping=None,  # default: include all participants as ONE unnamed group
-                         grouping={'Age': ('old',),  # analyze only group Age=old
-                                   },
-                         # grouping={'Age': ('young','old')},  # analyze both Age groups separately
+                         # grouping={'Age': ('old',),  # analyze only group Age=old
+                         #           },
+                         grouping={'Age': ('young','old')},  # analyze both Age groups separately
                          # participant='file',  # default
                          # participant='sheet',   # participant ID defined in xlsx sheet title, OR
                          # participant='SubjectID',  # participant IDs defined in column 'SubjectID'
                          # rename_cols={'Hearing Aid: 'HA'},  # dict with (file, new) column names
                          # header=0,  # first table row shows column headers
                          # converters={'Comfort': _recode_comfort, ...},  # user-defined mapping(s)
                          # ... any additional arguments to Pandas read_xxx function, if needed
                          )
     logger.info(f'Using data ds=\n{ds}')
 
     # ----------------- (Optional) show rating counts for all participants
     for attr in emf.attribute_dtypes.keys():
-        a_count = ds.attribute_grade_count(attr)
+        a_count = ds.attribute_grade_count(attr, groupby='HA')
         logger.info(str(attr) + '_grade_count:\n' + a_count.to_string())
         logger.info(str(attr) + ': sum grade_count= ' + f'{np.sum(a_count.to_numpy())}')
         # a_count.save(result_path / (str(attr) + '_grades.csv'))
 
     # ----------------- (Optional) show mean grades and NAP results for all participants
     mean_grades = ds.attribute_grade_mean(groupby=('HA', 'CoSS'))
     mean_grades.save(result_path / 'Attribute_mean_grades.txt', float_format='%.2f')
@@ -220,16 +220,15 @@
         logger.info('Model pickle-dumped as ' + f.name)
 
     # ------ 4: Generate result displays:
 
     # -------- Re-load learned EmaModel (optional, if saved):
     # with (work_path / model_file).open('rb') as f:
     #     emm = pickle.load(f)
-
-
+    # -------------------------------------------------
     emd = EmaDisplaySet.show(emm,
                              situations=['CoSS',  # CoSS probabilities, aggregated across HA
                                          ('CoSS', 'HA'),  # CoSS probabilities, conditional on HA
                                          ('HA', 'CoSS'),  # HA probabilities, conditional on CoSS
                                          ],
                              attributes=[('Speech', 'CoSS'),  # Speech, main effect of CoSS
                                          ('Speech', 'HA'),    # Speech, main effect of HA
@@ -240,19 +239,19 @@
                                            ('Comfort', 'HA')],  # *** version 0.9.5 ***
                              random_individual=True,  # random individual in population
                              population_mean=True,  # population mean
                              participants=False,  # individual results: True -> MANY plots and tables
                              grade_thresholds=True,  # response thresholds in attribute plots
                              percentiles=[2.5, 25, 50, 75, 97.5],  # in profile plots and tables
                              credibility_limit=0.7,  # minimum credibility in difference tables
-                             n_samples=10000,  # default=1000, for percentile calculations
+                             # n_samples=10000,  # default=1000, for percentile calculations
                              mpl_params={'figure.max_open_warning': 0,
                                          'axes.labelsize': 'x-large'},  # -> matplotlib.rcParam
                              # mpl_style='my_style_sheet',
-                             # ... any other ema_display.FMT settings
+                             # ... any other ema_display.FMT or ema_display_format.FMT settings
                              )
     # NOTE: joint (=interaction) effects are correct only if included in model regression_effects
 
     # ------------------------------- (optionally) edit display elements, if desired
     for g_disp in emd.groups.values():
         harmonize_ylim([g_disp.population_mean.attributes[('Speech', ('CoSS', 'HA'))].plot.ax,
                         g_disp.random_individual.attributes[('Speech', ('CoSS', 'HA'))].plot.ax,
@@ -263,17 +262,18 @@
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
 
     # -> matching y-axis limits: nice for plots to be shown side by side
 
     # ------------------------------- save all result displays
     emd.save(result_path,
-             figure_format='pdf',  # or any other format allowed by Matplotlib
-             table_format='tex',  # or csv, txt, xlsx, or other allowed by ema_file and Pandas
-             float_format='%.2f',  # any other parameters for Pandas table-writer function
+             figure_format='pdf',   # or any other format allowed by Matplotlib
+             table_format='txt',    # or csv, tex, xlsx, or other allowed by ema_file and Pandas
+                                    # NOTE: tex requires jinja2 to be installed manually
+             float_format='%.2f',   # any other parameters for Pandas table-writer function
              )
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
     #          # sep='\t'  # -> tab-delimited
     #          )
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc/run_sim.py` & `EmaCalc-0.9.6/src/EmaCalc/run_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,17 +207,17 @@
     # ------------------------------- Learn Analysis Model from simulated data set:
 
     # -------- Test re-loading simulated data from saved files (optional):
     logging.info('Simulated EMA data re-loaded from ' + str(data_path) + f' as {file_format} files')
     ds = EmaDataSet.load(emf, data_path,
                          fmt=file_format,
                          # grouping=None,  # default: include all participants as ONE unnamed group
-                         grouping={'Age': ('old',),  # analyze only Age=old
-                                   },
-                         # grouping={'Age': ('young','old')},  # analyze both Age groups separately
+                         # grouping={'Age': ('old',),  # analyze only Age=old
+                         #           },
+                         grouping={'Age': ('young','old')},  # analyze both Age groups separately
                          participant='file',  # 'sheet' only for Excel-style file formats
                          )
 
     logger.info(f'Using data ds=\n{ds}')
 
     # Model ordinal-regression effects of situations on each Attribute:
     # regression_effects = ['HA',     # main linear regression effect only
@@ -289,15 +289,15 @@
         harmonize_ylim([g_disp.population_mean.situations[('CoSS', 'HA')].plot.ax,
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
 
     # ------------------------------- save all result displays
     emd.save(result_path,
              figure_format='pdf',  # or any other format allowed by Matplotlib
-             table_format='tex',  # or any other format allowed by Pandas
+             table_format='txt',  # or any other format allowed by Pandas
              float_format='%.2f',  # any other parameters for Pandas table-writer function
              )
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
     #          # sep='\t'  # -> tab-delimited
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc.egg-info/PKG-INFO` & `EmaCalc-0.9.6/src/EmaCalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 0.9.5
+Version: 0.9.6
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EmaCalc-0.9.5/src/EmaCalc.egg-info/SOURCES.txt` & `EmaCalc-0.9.6/src/EmaCalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

