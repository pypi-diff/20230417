# Comparing `tmp/imbalance_metrics-0.0.5.tar.gz` & `tmp/imbalance_metrics-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbalance_metrics-0.0.5.tar", last modified: Sat Apr 15 18:36:00 2023, max compression
+gzip compressed data, was "imbalance_metrics-0.0.6.tar", last modified: Mon Apr 17 17:00:09 2023, max compression
```

## Comparing `imbalance_metrics-0.0.5.tar` & `imbalance_metrics-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:00.515350 imbalance_metrics-0.0.5/
--rw-rw-rw-   0        0        0    35149 2023-04-11 01:48:50.000000 imbalance_metrics-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     6275 2023-04-15 18:36:00.515350 imbalance_metrics-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5296 2023-04-15 03:48:49.000000 imbalance_metrics-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:00.490877 imbalance_metrics-0.0.5/imbalance_metrics/
--rw-rw-rw-   0        0        0      102 2023-04-11 18:51:46.000000 imbalance_metrics-0.0.5/imbalance_metrics/__init__.py
--rw-rw-rw-   0        0        0     9220 2023-04-15 18:17:27.000000 imbalance_metrics-0.0.5/imbalance_metrics/classification_metrics.py
--rw-rw-rw-   0        0        0     9031 2023-04-07 14:43:50.000000 imbalance_metrics-0.0.5/imbalance_metrics/regression_metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:00.513352 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/
--rw-rw-rw-   0        0        0     6275 2023-04-15 18:36:00.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-15 18:36:00.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:36:00.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 03:54:07.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2023-04-15 18:36:00.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-15 18:36:00.000000 imbalance_metrics-0.0.5/imbalance_metrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 18:36:00.516349 imbalance_metrics-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1342 2023-04-15 18:33:14.000000 imbalance_metrics-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:09.689695 imbalance_metrics-0.0.6/
+-rw-rw-rw-   0        0        0    35149 2023-04-11 01:48:50.000000 imbalance_metrics-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     6527 2023-04-17 17:00:09.689695 imbalance_metrics-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5548 2023-04-17 16:58:10.000000 imbalance_metrics-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:09.674402 imbalance_metrics-0.0.6/imbalance_metrics/
+-rw-rw-rw-   0        0        0      102 2023-04-11 18:51:46.000000 imbalance_metrics-0.0.6/imbalance_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9305 2023-04-16 21:19:53.000000 imbalance_metrics-0.0.6/imbalance_metrics/classification_metrics.py
+-rw-rw-rw-   0        0        0     9031 2023-04-07 14:43:50.000000 imbalance_metrics-0.0.6/imbalance_metrics/regression_metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:09.688662 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/
+-rw-rw-rw-   0        0        0     6527 2023-04-17 17:00:09.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-17 17:00:09.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:00:09.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 03:54:07.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-04-17 17:00:09.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-17 17:00:09.000000 imbalance_metrics-0.0.6/imbalance_metrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:00:09.689695 imbalance_metrics-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2023-04-17 16:55:18.000000 imbalance_metrics-0.0.6/setup.py
```

### Comparing `imbalance_metrics-0.0.5/LICENSE` & `imbalance_metrics-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `imbalance_metrics-0.0.5/PKG-INFO` & `imbalance_metrics-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbalance_metrics
-Version: 0.0.5
+Version: 0.0.6
 Summary: Perfromance metrics for imbalanced classification and imbalanced regression tasks
 Home-page: https://github.com/paobranco/ImbalanceMetrics
 Author: Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco
 Author-email: stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca
 Keywords: imbalanced learning,classification,regression,metrics
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -40,29 +40,32 @@
 ## install developer version
 pip install git+https://github.com/paobranco/ImbalanceMetrics.git
 ```
 
 ## Usage (Classification)
 ```python
 import pandas as pd
-from sklearn.tree import DecisionTreeClassifier
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 from imbalance_metrics import classification_metrics as cm
-df = pd.read_csv('poker-9_vs_7(processed).csv', header=None)
-X,y=df.drop(columns=[10]),df[10]
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
-clf = DecisionTreeClassifier(max_depth=100)
+df = pd.read_csv('glass0.csv', header=None)
+X,y=df.drop(columns=[9]),df[9]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.40)
+clf = RandomForestClassifier(random_state=42)
 clf.fit(X_train,y_train)
 y_pred=clf.predict(X_test)
 y_proba=clf.predict_proba(X_test)
-gmean = cm.gmean_score(y_test, y_pred)
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True) # By default 1 as positive
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True,pos_label=0) # 0 as positive
-p_man,r_man,pra_man=cm.pr_manning(y_test,y_proba,True)
-cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,6)
+y_phi = cm.calculate_classification_phi(y_test) # Relevance by class frequency
+gmean = cm.gmean_score(y_test, y_pred) # Weighted gmean 
+p_d0,r_d0,pra_d0=cm.pr_davis(y_test,y_proba,True) # Default minority as positive
+p_d1,r_d1,pra_d1=cm.pr_davis(y_test,y_proba,True,pos_label=1) # 1 as positive
+p_m0,r_m0,pra_m0=cm.pr_manning(y_test,y_proba,True) # Default minority as positive
+p_m1,r_m1,pra_m1=cm.pr_manning(y_test,y_proba,True,pos_label=1) # 1 as positive 
+cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,5)
+cv_manning=cm.cross_validate_auc(clf,X,y,cm.pr_manning,5)
 ```
 
 ## Usage (Regression)
 ```python
 import pandas as pd
 from sklearn.svm import SVR
 from sklearn.model_selection import train_test_split
```

### Comparing `imbalance_metrics-0.0.5/README.md` & `imbalance_metrics-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,32 @@
 ## install developer version
 pip install git+https://github.com/paobranco/ImbalanceMetrics.git
 ```
 
 ## Usage (Classification)
 ```python
 import pandas as pd
-from sklearn.tree import DecisionTreeClassifier
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 from imbalance_metrics import classification_metrics as cm
-df = pd.read_csv('poker-9_vs_7(processed).csv', header=None)
-X,y=df.drop(columns=[10]),df[10]
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
-clf = DecisionTreeClassifier(max_depth=100)
+df = pd.read_csv('glass0.csv', header=None)
+X,y=df.drop(columns=[9]),df[9]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.40)
+clf = RandomForestClassifier(random_state=42)
 clf.fit(X_train,y_train)
 y_pred=clf.predict(X_test)
 y_proba=clf.predict_proba(X_test)
-gmean = cm.gmean_score(y_test, y_pred)
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True) # By default 1 as positive
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True,pos_label=0) # 0 as positive
-p_man,r_man,pra_man=cm.pr_manning(y_test,y_proba,True)
-cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,6)
+y_phi = cm.calculate_classification_phi(y_test) # Relevance by class frequency
+gmean = cm.gmean_score(y_test, y_pred) # Weighted gmean 
+p_d0,r_d0,pra_d0=cm.pr_davis(y_test,y_proba,True) # Default minority as positive
+p_d1,r_d1,pra_d1=cm.pr_davis(y_test,y_proba,True,pos_label=1) # 1 as positive
+p_m0,r_m0,pra_m0=cm.pr_manning(y_test,y_proba,True) # Default minority as positive
+p_m1,r_m1,pra_m1=cm.pr_manning(y_test,y_proba,True,pos_label=1) # 1 as positive 
+cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,5)
+cv_manning=cm.cross_validate_auc(clf,X,y,cm.pr_manning,5)
 ```
 
 ## Usage (Regression)
 ```python
 import pandas as pd
 from sklearn.svm import SVR
 from sklearn.model_selection import train_test_split
```

### Comparing `imbalance_metrics-0.0.5/imbalance_metrics/classification_metrics.py` & `imbalance_metrics-0.0.6/imbalance_metrics/classification_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,47 +19,49 @@
         #print("Using minority class "+str(minor)+" as positive class")
         return minor
 
 def get_pr(y_true, y_probabilities,pos_label= None):
     precision, recall, _ = precision_recall_curve(y_true, y_probabilities,pos_label=pos_label)
     return precision, recall
 
-def calculate_classification_phi(y_true,per_sample = False, return_phi = False):
+def calculate_classification_phi(y_true,phi_option = 1, return_phi_per_class = False):
     """
     Calculates the Phi relvance value for each class of 'y'.
 
     Parameters
     ----------
     y_true : array-like
         Input data for which phi value needs to be calculated.
 
-    per_sample : bool, default = False
-        If False, Using inverse of the classes prevalence to weight each class 
-        If True, using inverse of the classes prevalence to weight each sample 
+    phi_option : int, default = 1
+        If 1, Classes weighted by inverse frequency 
+        If 2, Same as Option 1 but divided by class frequency 
 
-    return_phi : bool, default = False
-        Whether to return the Phi relevance value of each class.
+    return_phi_per_class : bool, default = False
+        Whether to return the Phi relevance value of each class or each sample
     Returns
     -------
     y_phi : array-like
-        If return_phi = False, Phi values for each element of 'y_true'.
-        If return_phi = True, Phi values for each class of 'y_true'.
+        If return_phi_per_class = False, Phi values for each element of 'y_true'.
+        If return_phi_per_class = True, Phi values for each class of 'y_true'.
     """
     sum_inverse = y_true.value_counts().apply(lambda x: 1 / x).sum()
     phi = y_true.value_counts().apply(lambda x: (1 / x) / sum_inverse)
-    if return_phi:
+    if return_phi_per_class:
         return phi
     else:
         y_phi = y_true.map(phi)
-        if not per_sample:
+        if phi_option == 1:
             return y_phi
-        else: 
+        elif phi_option == 2: 
             y_count = y_true.map(y_true.value_counts())
             new_y_phi= y_phi/y_count
             return new_y_phi
+        else: 
+            raise Exception()
 
 def gmean_score(y_true, y_pred, weighted = True):
     """
     Calculates geometric mean score.
 
     Parameters
     ----------
@@ -84,15 +86,15 @@
 
     recalls = []
     for i in range(len(classes)):
         TP = matrix[i, i]
         FN = np.sum(matrix[i, :]) - TP
         recall = TP / (TP + FN)
         if weighted:
-            phi = calculate_classification_phi(y_true, return_phi = True)
+            phi = calculate_classification_phi(y_true, return_phi_per_class = True)
             recall = recall * phi[classes[i]]
         recalls.append(recall)
 
     recalls_product = 1
     for r in recalls:
         recalls_product *= r
```

### Comparing `imbalance_metrics-0.0.5/imbalance_metrics/regression_metrics.py` & `imbalance_metrics-0.0.6/imbalance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `imbalance_metrics-0.0.5/imbalance_metrics.egg-info/PKG-INFO` & `imbalance_metrics-0.0.6/imbalance_metrics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbalance-metrics
-Version: 0.0.5
+Version: 0.0.6
 Summary: Perfromance metrics for imbalanced classification and imbalanced regression tasks
 Home-page: https://github.com/paobranco/ImbalanceMetrics
 Author: Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco
 Author-email: stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca
 Keywords: imbalanced learning,classification,regression,metrics
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -40,29 +40,32 @@
 ## install developer version
 pip install git+https://github.com/paobranco/ImbalanceMetrics.git
 ```
 
 ## Usage (Classification)
 ```python
 import pandas as pd
-from sklearn.tree import DecisionTreeClassifier
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 from imbalance_metrics import classification_metrics as cm
-df = pd.read_csv('poker-9_vs_7(processed).csv', header=None)
-X,y=df.drop(columns=[10]),df[10]
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
-clf = DecisionTreeClassifier(max_depth=100)
+df = pd.read_csv('glass0.csv', header=None)
+X,y=df.drop(columns=[9]),df[9]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.40)
+clf = RandomForestClassifier(random_state=42)
 clf.fit(X_train,y_train)
 y_pred=clf.predict(X_test)
 y_proba=clf.predict_proba(X_test)
-gmean = cm.gmean_score(y_test, y_pred)
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True) # By default 1 as positive
-p_dav,r_dav,pra_dav=cm.pr_davis(y_test,y_proba,True,pos_label=0) # 0 as positive
-p_man,r_man,pra_man=cm.pr_manning(y_test,y_proba,True)
-cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,6)
+y_phi = cm.calculate_classification_phi(y_test) # Relevance by class frequency
+gmean = cm.gmean_score(y_test, y_pred) # Weighted gmean 
+p_d0,r_d0,pra_d0=cm.pr_davis(y_test,y_proba,True) # Default minority as positive
+p_d1,r_d1,pra_d1=cm.pr_davis(y_test,y_proba,True,pos_label=1) # 1 as positive
+p_m0,r_m0,pra_m0=cm.pr_manning(y_test,y_proba,True) # Default minority as positive
+p_m1,r_m1,pra_m1=cm.pr_manning(y_test,y_proba,True,pos_label=1) # 1 as positive 
+cv_davis=cm.cross_validate_auc(clf,X,y,cm.pr_davis,5)
+cv_manning=cm.cross_validate_auc(clf,X,y,cm.pr_manning,5)
 ```
 
 ## Usage (Regression)
 ```python
 import pandas as pd
 from sklearn.svm import SVR
 from sklearn.model_selection import train_test_split
```

### Comparing `imbalance_metrics-0.0.5/setup.py` & `imbalance_metrics-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='imbalance_metrics',
-      version='0.0.5',
+      version='0.0.6',
       description='Perfromance metrics for imbalanced classification and imbalanced regression tasks',
       long_description = open('README.md').read(),
       long_description_content_type = "text/markdown",
       url='https://github.com/paobranco/ImbalanceMetrics',
       author='Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco',
       author_email = 'stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca',
       classifiers = [
```

