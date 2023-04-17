# Comparing `tmp/mosum-0.1.0.tar.gz` & `tmp/mosum-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosum-0.1.0.tar", max compression
+gzip compressed data, was "mosum-0.2.0.tar", max compression
```

## Comparing `mosum-0.1.0.tar` & `mosum-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1052 2023-02-01 13:51:05.315590 mosum-0.1.0/LICENSE
--rw-r--r--   0        0        0     1425 2023-02-22 13:25:56.237545 mosum-0.1.0/README.md
--rw-r--r--   0        0        0      284 2023-02-09 11:31:16.713719 mosum-0.1.0/mosum/__init__.py
--rw-r--r--   0        0        0     1603 2023-02-22 13:29:04.349908 mosum-0.1.0/mosum/bandwidth.py
--rw-r--r--   0        0        0     5664 2023-02-01 15:40:15.519354 mosum-0.1.0/mosum/bootstrap.cpp
--rw-r--r--   0        0        0        0 2023-01-11 14:05:49.578293 mosum-0.1.0/mosum/bootstrap.py
--rw-r--r--   0        0        0     9998 2023-02-27 09:28:49.118945 mosum-0.1.0/mosum/bottom_up.py
--rw-r--r--   0        0        0    12721 2023-02-08 13:40:45.332512 mosum-0.1.0/mosum/exhaust_bic.cpp
--rw-r--r--   0        0        0        0 2023-02-22 13:29:36.725979 mosum-0.1.0/mosum/local_prune.py
--rw-r--r--   0        0        0    12731 2023-02-23 09:05:07.510269 mosum-0.1.0/mosum/mosum.py
--rw-r--r--   0        0        0     6451 2023-02-09 09:22:50.959226 mosum-0.1.0/mosum/mosum_stat.py
--rw-r--r--   0        0        0      877 2023-02-22 13:30:28.018095 mosum-0.1.0/mosum/mosum_test.py
--rw-r--r--   0        0        0     2182 2023-01-18 14:18:15.067922 mosum-0.1.0/mosum/mosum_util.cpp
--rw-r--r--   0        0        0      367 2023-01-18 08:40:02.049936 mosum-0.1.0/mosum/mosum_util.h
--rw-r--r--   0        0        0     2513 2023-02-23 09:16:56.360072 mosum-0.1.0/mosum/persp3D.py
--rw-r--r--   0        0        0     2574 2023-02-22 15:54:05.358421 mosum-0.1.0/mosum/test_data.py
--rw-r--r--   0        0        0     1540 2023-02-22 13:40:24.931689 mosum-0.1.0/mosum/test_models.py
--rw-r--r--   0        0        0      645 2023-02-24 10:25:45.395882 mosum-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 mosum-0.1.0/setup.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 mosum-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-02-01 13:51:05.315590 mosum-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1425 2023-02-22 13:25:56.237545 mosum-0.2.0/README.md
+-rw-r--r--   0        0        0      439 2023-04-14 14:34:26.280359 mosum-0.2.0/mosum/__init__.py
+-rw-r--r--   0        0        0     1603 2023-02-22 13:29:04.349908 mosum-0.2.0/mosum/bandwidth.py
+-rw-r--r--   0        0        0     6833 2023-04-17 09:19:15.028869 mosum-0.2.0/mosum/bootstrap.py
+-rw-r--r--   0        0        0     6389 2023-04-17 08:57:58.784093 mosum-0.2.0/mosum/bottom_up.py
+-rw-r--r--   0        0        0    12995 2023-04-17 11:06:06.548520 mosum-0.2.0/mosum/classes.py
+-rw-r--r--   0        0        0     8411 2023-04-14 09:35:13.272661 mosum-0.2.0/mosum/exhaust_bic.py
+-rw-r--r--   0        0        0    17306 2023-04-17 09:45:47.769081 mosum-0.2.0/mosum/local_prune.py
+-rw-r--r--   0        0        0     9314 2023-04-17 09:48:01.453697 mosum-0.2.0/mosum/mosum.py
+-rw-r--r--   0        0        0     6451 2023-02-09 09:22:50.959226 mosum-0.2.0/mosum/mosum_stat.py
+-rw-r--r--   0        0        0      877 2023-02-22 13:30:28.018095 mosum-0.2.0/mosum/mosum_test.py
+-rw-r--r--   0        0        0     2182 2023-01-18 14:18:15.067922 mosum-0.2.0/mosum/mosum_util.cpp
+-rw-r--r--   0        0        0      367 2023-01-18 08:40:02.049936 mosum-0.2.0/mosum/mosum_util.h
+-rw-r--r--   0        0        0     2513 2023-02-23 09:16:56.360072 mosum-0.2.0/mosum/persp3D.py
+-rw-r--r--   0        0        0     2574 2023-02-22 15:54:05.358421 mosum-0.2.0/mosum/test_data.py
+-rw-r--r--   0        0        0     1540 2023-02-22 13:40:24.931689 mosum-0.2.0/mosum/test_models.py
+-rw-r--r--   0        0        0      675 2023-04-17 10:40:22.506543 mosum-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 mosum-0.2.0/setup.py
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 mosum-0.2.0/PKG-INFO
```

### Comparing `mosum-0.1.0/LICENSE` & `mosum-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/README.md` & `mosum-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/bandwidth.py` & `mosum-0.2.0/mosum/bandwidth.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/mosum.py` & `mosum-0.2.0/mosum/mosum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,16 @@
 import mosum
 import numpy as np
 import pandas as pd
 import sys
-from matplotlib import pyplot as plt
 
+from mosum.classes import mosum_obj
 from mosum.mosum_test import criticalValue, pValue
 from mosum.mosum_stat import mosum_stat, eta_criterion_help
-
-
-class mosum_obj:
-    """mosum object"""
-
-    def __init__(self, x, G_left, G_right, var_est_method, var_custom, boundary_extension, stat, unscaledStatistic,
-                 var_estimation,
-                 threshold, alpha, threshold_custom, threshold_value, criterion, eta, epsilon, cpts, cpts_info,
-                 do_confint, ci):
-        """init method"""
-        self.x = x
-        self.G_left = G_left
-        self.G_right = G_right
-        self.var_est_method = var_est_method
-        self.var_custom = var_custom
-        self.boundary_extension = boundary_extension
-        self.stat = stat
-        self.rollsums = unscaledStatistic
-        self.var_estimation = var_estimation
-        self.threshold = threshold
-        self.alpha = alpha
-        self.threshold_custom = threshold_custom
-        self.threshold_value = threshold_value
-        self.criterion = criterion
-        self.eta = eta
-        self.epsilon = epsilon
-        self.cpts = np.array(cpts, int)
-        self.cpts_info = cpts_info
-        self.do_confint = do_confint
-        self.ci = ci  # note
-
-    def plot(self, display=['data', 'mosum'][0], cpts_col='red', critical_value_col='blue', xlab='Time'):
-        """plot method - plots data or detector"""
-        plt.clf()
-        x_plot = np.arange(0,len(self.x))
-        if (display == 'mosum'):
-            plt.plot(x_plot, self.stat, ls='-', color="black")
-            plt.axhline(self.threshold_value, color=critical_value_col)
-        if (display == 'data'):
-            if(len(self.cpts)>0):
-                brks = np.concatenate((0, self.cpts, len(self.x)), axis=None)
-            else:
-                brks = np.array([0, len(self.x)])
-            fhat = self.x * 0
-            for kk in np.arange(0,(len(brks) - 1)):
-                int = np.arange(brks[kk],brks[kk + 1])
-                fhat[int] = np.mean(self.x[int])
-            plt.plot(x_plot, self.x, ls='-', color="black")
-            plt.xlabel(xlab)
-            plt.title("v")
-            plt.plot(x_plot, fhat, color = 'darkgray', ls = '-', lw = 2)
-        for p in self.cpts:
-            plt.axvline(x_plot[(p-1)]+1, color='red')
-
-
-    def summary(self):
-        """summary method"""
-        n = len(self.x)
-        if (len(self.cpts) > 0):
-            ans = self.cpts_info
-            ans.p_value = round(ans.p_value, 3)
-            ans.jump = round(ans.jump, 3)
-        out = 'change points detected at alpha = ' + str(self.alpha) + ' according to ' + self.criterion + '-criterion'
-        if (self.criterion == 'eta'): out = out + ' with eta = ' + str(self.eta)
-        if (self.criterion == 'epsilon'): out = out + ' with epsilon = ' + str(self.epsilon)
-        out = out + ' and ' + self.var_est_method + ' variance estimate:'
-        print(out)
-        if (len(self.cpts) > 0):
-            print(ans)
-        else:
-            print('no change point is found')
-
-    def print(self):
-        """print method"""
-        n = len(self.x)
-        if (len(self.cpts) > 0):
-            ans = self.cpts_info
-            ans.p_value = round(ans.p_value, 3)
-            ans.jump = round(ans.jump, 3)
-        out = 'change points detected with bandwidths (' + str(self.G_left) + ',' + str(
-            self.G_right) + ') at alpha = ' + str(self.alpha) + ' according to ' + self.criterion + '-criterion'
-        if (self.criterion == 'eta'): out = out + (' with eta = ' + str(self.eta))
-        if (self.criterion == 'epsilon'): out = out + (' with epsilon = ' + str(self.epsilon))
-        out = out + (' and ' + self.var_est_method + ' variance estimate:')
-        print(out)
-        if (len(self.cpts) > 0):
-            print(ans)
-        else:
-            print('no change point is found')
+from mosum.bootstrap import confint_mosum_cpts
 
 
 def mosum(x, G, G_right=float("nan"), var_est_method=['mosum', 'mosum_min', 'mosum_max', 'custom'][0],
           var_custom=None, boundary_extension=True,
           threshold=['critical_value', 'custom'][0], alpha=.1,
           threshold_custom=float("nan"), criterion=['eta', 'epsilon'][0],
           eta=0.4, epsilon=0.2, do_confint=False,
@@ -216,15 +128,15 @@
 
     # adjust, in case of no boundary CUSUM extension
     if not m.boundary_extension: exceedings[n - G_right] = False
 
     if criterion == 'epsilon':
         # get number of subsequent exceedings
         ex_len = pd.Series(exceedings)  # rlencode(exceedings)[1]
-        exceedingsCount = np.array(exceedings * pd.Series(ex_len.groupby(ex_len).cumcount().add(1)))
+        exceedingsCount = np.array(exceedings * pd.Series(ex_len.cumsum()-ex_len.cumsum().where(~ex_len).ffill().fillna(0).astype(int)))
         # get exceeding-intervals of fitting length
         minIntervalSize = max([1, (G_min + G_max) / 2 * epsilon])
         intervalEndPoints = np.array(np.where(np.diff(exceedingsCount) <= -minIntervalSize)[0])
         intervalBeginPoints = intervalEndPoints - exceedingsCount[intervalEndPoints] + 1
         if not m.boundary_extension:
             # manually adjust right border
             if exceedings[n - G_right - 1] & (not (n - G_right) in intervalEndPoints):  # check all this
@@ -257,25 +169,30 @@
         if not m.boundary_extension:
             localMaxima[n-G_right-1] = True
         p_candidates = np.where(exceedings & localMaxima) #np.asarray(exceedings & localMaxima).nonzero() #
         changePoints = eta_criterion_help(p_candidates[0], m.stat, eta, G_left, G_right)
 
     n_cps = len(changePoints)
     if n_cps == 0:
-        cpts_info = None
+        cpts_info = pd.DataFrame({"cpts": [],
+                                  "G_left": [],
+                                  "G_right": [],
+                                  "p_value": [],
+                                  "jump": []})
+
     else:
         outcps = changePoints.astype(int)
         cpts_info = pd.DataFrame({"cpts": outcps,
                                   "G_left": np.full(n_cps, G_left),
                                   "G_right": np.full(n_cps, G_right),
                                   "p_value": pValue(m.stat[outcps], n, G_left, G_right),
                                   "jump": np.sqrt((G_left + G_right) / G_left / G_right) * m.stat[outcps]})
-    # if do_confint:
-    #    ret$ci < - confint.mosum.cpts(ret, level=level, N_reps=N_reps)
-    #    ret$do.confint < - TRUE
-    ci = None
+
 
     out = mosum_obj(x, G_left, G_right, var_est_method, var_custom, boundary_extension, m.stat, m.rollsums,
                     m.var_estimation,
                     threshold, alpha, threshold_custom, threshold_val, criterion, eta, epsilon, changePoints, cpts_info,
-                    do_confint, ci)
+                    False, None)
+    if do_confint:
+        out.ci = confint_mosum_cpts(out, level=level, N_reps=N_reps)
+        out.do_confint = True
     return out
```

### Comparing `mosum-0.1.0/mosum/mosum_stat.py` & `mosum-0.2.0/mosum/mosum_stat.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/mosum_test.py` & `mosum-0.2.0/mosum/mosum_test.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/mosum_util.cpp` & `mosum-0.2.0/mosum/mosum_util.cpp`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/persp3D.py` & `mosum-0.2.0/mosum/persp3D.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/test_data.py` & `mosum-0.2.0/mosum/test_data.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/mosum/test_models.py` & `mosum-0.2.0/mosum/test_models.py`

 * *Files identical despite different names*

### Comparing `mosum-0.1.0/pyproject.toml` & `mosum-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "mosum"
-version = "0.1.0"
+version = "0.2.0"
 description = "Moving Sum Based Procedures for Changes in the Mean"
 authors = ["Dom Owens <dom.owens@bristol.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [{ include = "mosum"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-numpy = "^1.24.1"
+python = ">=3.9,<3.10"
+numpy = ">=1.23.5,<1.24"
 pandas = "^1.5.3"
 matplotlib = "^3.6.3"
+numba = "^0.53"
 
 [tool.poetry.dev-dependencies]
 python = "^3.9"
 pytest = "^7.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `mosum-0.1.0/setup.py` & `mosum-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 packages = \
 ['mosum']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'pandas>=1.5.3,<2.0.0']
+['matplotlib>=3.6.3,<4.0.0',
+ 'numba>=0.53,<0.54',
+ 'numpy>=1.23.5,<1.24',
+ 'pandas>=1.5.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mosum',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Moving Sum Based Procedures for Changes in the Mean',
     'long_description': '# mosum.py: Moving Sum Based Procedures for Changes in the Mean\n\nA python port of the R package mosum <https://CRAN.R-project.org/package=mosum>.\nImplementations of MOSUM-based statistical procedures and algorithms for detecting multiple changes in the mean. \nThis comprises the MOSUM procedure for estimating multiple mean changes from Eichinger and Kirch (2018) <doi:10.3150/16-BEJ887> \nand the multiscale algorithmic extension from Cho and Kirch (2022) <doi:10.1007/s10463-021-00811-5>, \nas well as the bootstrap procedure for generating confidence intervals about the locations of change points as proposed in Cho and Kirch (2022) <doi:10.1016/j.csda.2022.107552>. \nSee also Meier, Kirch and Cho (2021) <doi:10.18637/jss.v097.i08> which accompanies the R package.\n\n## Installation\n\n```bash\n$ pip install mosum\n```\n\n## Usage\n\nmosum.py can be used as follows to detect changes in the mean of a time series\n\n```python\nimport mosum\n#   simulate data\nxx = mosum.testData("blocks")["x"]\n# detect changes\nxx_m  = mosum.mosum(xx, G = 50, criterion = "eta", boundary_extension = True)\n# summary and print methods\nxx_m.summary()\nxx_m.print()\n# plot the output\nxx_m.plot(display="mosum")\nfrom matplotlib import pyplot as plt\nplt.show()\n```\n\n## License\n\nmosum.py was created by Dom Owens, based on the R package "mosum", originally by Alexander Meier, Haeran Cho, and Claudia Kirch.\nIt is licensed under the terms of the MIT license.',
     'author': 'Dom Owens',
     'author_email': 'dom.owens@bristol.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.9,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mosum-0.1.0/PKG-INFO` & `mosum-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mosum
-Version: 0.1.0
+Version: 0.2.0
 Summary: Moving Sum Based Procedures for Changes in the Mean
 License: MIT
 Author: Dom Owens
 Author-email: dom.owens@bristol.ac.uk
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: numba (>=0.53,<0.54)
+Requires-Dist: numpy (>=1.23.5,<1.24)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # mosum.py: Moving Sum Based Procedures for Changes in the Mean
 
 A python port of the R package mosum <https://CRAN.R-project.org/package=mosum>.
 Implementations of MOSUM-based statistical procedures and algorithms for detecting multiple changes in the mean.
```

