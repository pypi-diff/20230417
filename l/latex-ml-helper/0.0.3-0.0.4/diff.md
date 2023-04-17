# Comparing `tmp/latex_ml_helper-0.0.3.tar.gz` & `tmp/latex_ml_helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.3.tar", last modified: Sun Apr 16 18:14:27 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.0.4.tar", last modified: Sun Apr 16 19:52:33 2023, max compression
```

## Comparing `latex_ml_helper-0.0.3.tar` & `latex_ml_helper-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.668154 latex_ml_helper-0.0.3/
--rw-rw-rw-   0        0        0      657 2023-04-16 18:14:27.668154 latex_ml_helper-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.664154 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.667154 latex_ml_helper-0.0.3/libraries/
--rw-rw-rw-   0        0        0      184 2023-04-16 17:45:57.000000 latex_ml_helper-0.0.3/libraries/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.3/libraries/copy.py
--rw-rw-rw-   0        0        0     1951 2023-04-16 18:12:59.000000 latex_ml_helper-0.0.3/libraries/definitions.py
--rw-rw-rw-   0        0        0     7677 2023-04-16 17:45:43.000000 latex_ml_helper-0.0.3/libraries/snippets.py
--rw-rw-rw-   0        0        0       42 2023-04-16 18:14:27.669154 latex_ml_helper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-04-16 18:13:30.000000 latex_ml_helper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:52:33.177848 latex_ml_helper-0.0.4/
+-rw-rw-rw-   0        0        0      657 2023-04-16 19:52:33.177848 latex_ml_helper-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 19:52:33.173848 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-04-16 19:52:33.000000 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-16 19:52:33.000000 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:52:33.000000 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 19:52:33.000000 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 19:52:33.000000 latex_ml_helper-0.0.4/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 19:52:33.176848 latex_ml_helper-0.0.4/libraries/
+-rw-rw-rw-   0        0        0      290 2023-04-16 19:51:25.000000 latex_ml_helper-0.0.4/libraries/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.4/libraries/copy.py
+-rw-rw-rw-   0        0        0     3727 2023-04-16 18:38:54.000000 latex_ml_helper-0.0.4/libraries/definitions.py
+-rw-rw-rw-   0        0        0     8095 2023-04-16 18:52:16.000000 latex_ml_helper-0.0.4/libraries/snippets.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:52:33.177848 latex_ml_helper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-04-16 19:52:21.000000 latex_ml_helper-0.0.4/setup.py
```

### Comparing `latex_ml_helper-0.0.3/PKG-INFO` & `latex_ml_helper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.3/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.0.4/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.3/libraries/snippets.py` & `latex_ml_helper-0.0.4/libraries/snippets.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,26 @@
             x2 = -(self.theta[0] + self.theta[1] * x1) / self.theta[2]
             plt.plot(x1, x2, 'r')
             
         plt.show()    
 """
     return copy_text(text, copy)
 
+def SVM_Line(copy = False):
+    text = """
+theta_0 = -0.5
+theta = np.array([1, 1])
+xx = np.linspace(-0.5, 1.5, 100)
+yy = -(theta[0] / theta[1]) * xx - theta_0 / theta[1]
+#
+xx = np.linspace(np.min(X)-1, np.max(X)+1, 1000)
+yy = -(model.coef_[0][0] / model.coef_[0][1]) * xx - (model.intercept_ / model.coef_[0][1])
+"""
+    return copy_text(text, copy)
+
 def SVM_Margin(copy = False):
     text = """
 X, y = make_blobs(n_samples=40, centers=2, random_state=1)
 clf = LinearSVC(random_state=0).fit(X, y)
 dec_func = clf.decision_function(X)
 support_vector_indices = np.where(np.abs(dec_func) <= 1 + 1e-15)
 support_vectors = X[support_vector_indices]
@@ -220,18 +232,19 @@
     y_pred.append(np.argmax(sm))
     print(sm, np.argmax(sm))
 y_pred = np.array(y_pred)
 print(confusion_matrix(y_true, y_pred))
 """
     return copy_text(text, copy)
 
-def Help(copy = False):
+def HelpSnippets(copy = False):
     text = """
 Imports <- Importi
 Loss <- Loss funkcija
 Perc <- Perceptron algoritam
+SVM_Line <- Support Vector Machine sa linijom
 SVM_Margin <- Support Vector Machine sa marginom
 Contour <- Konture
 Scaler <- Skaliranje
 SoftMax <- SoftMax
 """
     return copy_text(text, copy)
```

### Comparing `latex_ml_helper-0.0.3/setup.py` & `latex_ml_helper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
```

