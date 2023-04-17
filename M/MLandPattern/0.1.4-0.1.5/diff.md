# Comparing `tmp/MLandPattern-0.1.4.tar.gz` & `tmp/MLandPattern-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.1.4.tar", last modified: Sun Apr 16 12:45:24 2023, max compression
+gzip compressed data, was "MLandPattern-0.1.5.tar", last modified: Mon Apr 17 08:32:22 2023, max compression
```

## Comparing `MLandPattern-0.1.4.tar` & `MLandPattern-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.832422 MLandPattern-0.1.4/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.828932 MLandPattern-0.1.4/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)     5772 2023-04-16 12:40:00.000000 MLandPattern-0.1.4/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.4/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.831236 MLandPattern-0.1.4/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-16 12:45:24.832021 MLandPattern-0.1.4/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.4/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-04-16 12:45:24.832584 MLandPattern-0.1.4/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-04-16 12:37:29.000000 MLandPattern-0.1.4/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-17 08:32:22.741313 MLandPattern-0.1.5/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-17 08:32:22.737796 MLandPattern-0.1.5/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)     8231 2023-04-17 08:30:10.000000 MLandPattern-0.1.5/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.5/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-17 08:32:22.740248 MLandPattern-0.1.5/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-17 08:32:22.000000 MLandPattern-0.1.5/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-04-17 08:32:22.000000 MLandPattern-0.1.5/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-04-17 08:32:22.000000 MLandPattern-0.1.5/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-04-17 08:32:22.000000 MLandPattern-0.1.5/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-17 08:32:22.740835 MLandPattern-0.1.5/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.5/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-04-17 08:32:22.741468 MLandPattern-0.1.5/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-04-17 08:30:22.000000 MLandPattern-0.1.5/setup.py
```

### Comparing `MLandPattern-0.1.4/MLandPattern/MLandPattern.py` & `MLandPattern-0.1.5/MLandPattern/MLandPattern.py`

 * *Files 25% similar despite different names*

```diff
@@ -71,85 +71,122 @@
     each row
     """
     mean = mean_of_matrix_rows(matrix)
     centered_data = matrix - mean
     return centered_data
 
 
-#  Calculates the Sample Covariance Matrix
-def covariance(centered_matrix):
+def covariance(matrix, centered = 0):
     """
     Calculates the Sample Covariance Matrix of a centered-matrix
-    :param vector: a numpy row vector
-    :return: the vector reshaped as a column vector
+    :param matrix: Matrix of data points
+    :param centered: Flag to determine if matrix data is centered (default is False)
+    :return: The data covariance matrix
     """
-    n = centered_matrix.shape[1]
-    cov = np.dot(centered_matrix, centered_matrix.T)
+    if not centered:
+        matrix = center_data(matrix)
+    n = matrix.shape[1]
+    cov = np.dot(matrix, matrix.T)
     cov = np.multiply(cov, 1/n)
     return cov
 
 
-#  Calculates the eigen value and vectors for a matrix and returns them in ascending order
 def eigen(matrix):
+    """
+    Calculates the eigen value and vectors for a matrix
+    :param matrix: Matrix of data points
+    :return: eigen values, eigen vectors
+    """
     if matrix.shape[0] == matrix.shape[1]:
         s, U = np.linalg.eigh(matrix)
         return s, U
     else:
         s, U = np.linalg.eig(matrix)
         return s, U
 
 
-#  Calculates the PCA dimension reduction to an m-dimension space, returning the projection matrix P
 def PCA(attribute_matrix, m):
-    mu = mean_of_matrix_rows(attribute_matrix)
+    """
+    Calculates the PCA dimension reduction of a matrix to a m-dimension sub-space
+    :param attribute_matrix: matrix with the datapoints, with each row being a point
+    :param m: number of dimensions of the targeted sub-space
+    :return: a projection matrix P
+    """
     DC = center_data(attribute_matrix)
-    C = covariance(DC)
+    C = covariance(DC, 1)
     s, U = eigen(C)
     P = U[:, ::-1][:, 0:m]
     return P
 
 
-def covariance_within_class(matrix_values, label, class_labels):
+def covariance_within_class(matrix_values, label):
+    """
+    Calculates the average covariance within all the classes in a dataset
+    :param matrix_values: matrix with the values associated to the parameters of the dataset
+    :param label: vector with the label values associated with the dataset
+    :return: a matrix with the total average covariance within each class
+    """
+    class_labels = np.unique(label)
     within_cov = np.zeros((matrix_values.shape[0], matrix_values.shape[0]))
     n = matrix_values.size
-    for i in range(len(class_labels)):
+    for i in class_labels:
         centered_matrix = center_data(matrix_values[:, label == i])
-        cov_matrix = covariance(centered_matrix)
+        cov_matrix = covariance(centered_matrix, 1)
         cov_matrix = np.multiply(cov_matrix, centered_matrix.size)
         within_cov = np.add(within_cov, cov_matrix)
     within_cov = np.divide(within_cov, n)
     return within_cov
 
 
-def covariance_between_class(matrix_values, label, class_labels):
+def covariance_between_class(matrix_values, label):
+    """
+    Calculates the total covariance between all the classes in a dataset
+    :param matrix_values: matrix with the values associated to the parameters of the dataset
+    :param label: vector with the label values associated with the dataset
+    :return: a matrix with the covariance between each class
+    """
+    class_labels = np.unique(label)
     between_cov = np.zeros((matrix_values.shape[0], matrix_values.shape[0]))
     N = matrix_values.size
     m_general = mean_of_matrix_rows(matrix_values)
     for i in range(len(class_labels)):
         values = matrix_values[:, label == i]
         nc = values.size
         m_class = mean_of_matrix_rows(values)
         norm_means = np.subtract(m_class, m_general)
         matr = np.multiply(nc, np.dot(norm_means, norm_means.T))
         between_cov = np.add(between_cov, matr)
     between_cov = np.divide(between_cov, N)
     return between_cov
 
 
-def between_within_covariance (matrix_values, label, class_labels):
-    Sw = covariance_within_class(matrix_values, label, class_labels)
-    Sb = covariance_between_class(matrix_values, label, class_labels)
+def between_within_covariance (matrix_values, label):
+    """
+    Calculates both the average within covariance, and the between covariance of all classes on a dataset
+    :param matrix_values: matrix with the values associated to the parameters of the dataset
+    :param label: vector with the label values associated with the dataset
+    :return:a matrix with the total average covariance within each class, and the covariance between each class
+    """
+    Sw = covariance_within_class(matrix_values, label)
+    Sb = covariance_between_class(matrix_values, label)
     return Sw, Sb
 
 
-def LDA1(matrix_values, label, class_labels, m):
+def LDA1(matrix_values, label, m):
+    """
+    Calculates the Lineal Discriminant Analysis to perform dimension reduction
+    :param matrix_values: matrix with the datapoints, with each row being a point
+    :param label: vector with the label values associated with the dataset
+    :param m: number of dimensions of the targeted sub-space
+    :return: the LDA directions matrix (W), and the orthogonal sub-space of the directions (U)
+    """
+    class_labels = np.unique(label)
     [Sw, Sb] = between_within_covariance(matrix_values, label, class_labels)
     s, U = scipy.linalg.eigh(Sb, Sw)
     W = U[:, ::-1][:, 0:m]
-    print(W)
     UW, _, _ = np.linalg.svd(W)
     U = UW[:, 0:m]
     return W, U
 
 
 #  General method to graph a class-related data into a 2d scatter plot
 def graphic_scatter_2d(matrix, labels, names, x_axis="Axis 1", y_axis="Axis 2"):
@@ -158,14 +195,21 @@
     plt.xlabel(x_axis)
     plt.ylabel(y_axis)
     plt.legend()
     plt.show()
 
 
 def logpdf_GAU_ND(x, mu, C):
+    """
+    Calculates the Logarithmic MultiVariate Gaussian Density for a set of vector values
+    :param x: matrix of the datapoints of a dataset, with a size (n x m) 
+    :param mu: row vector with the mean associated to each dimension
+    :param C: Covariance matrix
+    :return: a matrix with the Gaussian Density associated with each point of X, over each dimension
+    """
     M = C.shape[1]
     inv_C = np.linalg.inv(C)
     [_, log_C] = np.linalg.slogdet(C)
     log_2pi = math.log(2*math.pi)
     y = np.zeros(x.shape[1]) if M == 1 else np.zeros(x.shape)
     for i in range(x.shape[1]):
         norm_x = vcol(x[:, i]) - mu
@@ -176,12 +220,19 @@
             y[i] = MVG
         else:
             y[:, i] = MVG
     return y
 
 
 def logLikelihood (X, mu, c):
+    """
+    Calculates the Logarithmic Maximum Likelihood estimator
+    :param X: matrix of the datapoints of a dataset, with a size (n x m) 
+    :param mu: row vector with the mean associated to each dimension
+    :param c: Covariance matrix
+    :return: the logarithm of the likelihood of the datapoints, and the associated gaussian density
+    """
     M = c.shape[1]
     logN = logpdf_GAU_ND(X, mu, c)
     print(logN.shape)
     acum = logN.sum(1) if M != 1 else logN.sum()
     return acum
```

