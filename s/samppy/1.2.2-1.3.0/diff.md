# Comparing `tmp/samppy-1.2.2.tar.gz` & `tmp/samppy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samppy-1.2.2.tar", last modified: Thu Nov  4 14:12:27 2021, max compression
+gzip compressed data, was "samppy-1.3.0.tar", last modified: Mon Apr 17 00:35:06 2023, max compression
```

## Comparing `samppy-1.2.2.tar` & `samppy-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2021-11-04 14:12:27.017793 samppy-1.2.2/
--rw-r--r--   0 arne       (503) staff       (20)     1083 2018-08-05 14:59:07.000000 samppy-1.2.2/LICENSE.txt
--rw-r--r--   0 arne       (503) staff       (20)     3361 2021-11-04 14:12:27.017951 samppy-1.2.2/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)     2714 2021-09-29 10:25:46.000000 samppy-1.2.2/README.md
--rw-r--r--   0 arne       (503) staff       (20)      103 2021-09-24 09:50:47.000000 samppy-1.2.2/pyproject.toml
--rw-r--r--   0 arne       (503) staff       (20)      804 2021-11-04 14:12:27.018816 samppy-1.2.2/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2021-11-04 14:12:27.009088 samppy-1.2.2/src/
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2021-11-04 14:12:27.014515 samppy-1.2.2/src/samppy/
--rw-r--r--   0 arne       (503) staff       (20)      987 2021-11-03 08:33:50.000000 samppy-1.2.2/src/samppy/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    15760 2021-09-12 15:01:16.000000 samppy-1.2.2/src/samppy/credibility.py
--rw-r--r--   0 arne       (503) staff       (20)    36728 2021-11-03 08:31:02.000000 samppy-1.2.2/src/samppy/hamiltonian_sampler.py
--rw-r--r--   0 arne       (503) staff       (20)     4521 2021-09-29 10:12:32.000000 samppy-1.2.2/src/samppy/sample_entropy.py
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2021-11-04 14:12:27.017440 samppy-1.2.2/src/samppy.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)     3361 2021-11-04 14:12:27.000000 samppy-1.2.2/src/samppy.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      327 2021-11-04 14:12:27.000000 samppy-1.2.2/src/samppy.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2021-11-04 14:12:27.000000 samppy-1.2.2/src/samppy.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)       18 2021-11-04 14:12:27.000000 samppy-1.2.2/src/samppy.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)        7 2021-11-04 14:12:27.000000 samppy-1.2.2/src/samppy.egg-info/top_level.txt
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 00:35:06.087190 samppy-1.3.0/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2018-08-05 14:59:07.000000 samppy-1.3.0/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)     3950 2023-04-17 00:35:06.087234 samppy-1.3.0/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     3342 2023-04-16 07:40:36.000000 samppy-1.3.0/README.md
+-rw-r--r--   0 arne       (503) staff       (20)      103 2023-04-17 00:34:02.000000 samppy-1.3.0/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      804 2023-04-17 00:35:06.087448 samppy-1.3.0/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 00:35:06.084360 samppy-1.3.0/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 00:35:06.086370 samppy-1.3.0/src/samppy/
+-rw-r--r--   0 arne       (503) staff       (20)     1093 2023-04-16 07:25:28.000000 samppy-1.3.0/src/samppy/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    15836 2023-04-04 13:10:30.000000 samppy-1.3.0/src/samppy/credibility.py
+-rw-r--r--   0 arne       (503) staff       (20)    19439 2023-04-16 08:19:21.000000 samppy-1.3.0/src/samppy/credibility_pd.py
+-rw-r--r--   0 arne       (503) staff       (20)    36728 2021-11-03 08:31:02.000000 samppy-1.3.0/src/samppy/hamiltonian_sampler.py
+-rw-r--r--   0 arne       (503) staff       (20)     4521 2021-09-29 10:12:32.000000 samppy-1.3.0/src/samppy/sample_entropy.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 00:35:06.087067 samppy-1.3.0/src/samppy.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)     3950 2023-04-17 00:35:06.000000 samppy-1.3.0/src/samppy.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      356 2023-04-17 00:35:06.000000 samppy-1.3.0/src/samppy.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-04-17 00:35:06.000000 samppy-1.3.0/src/samppy.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       18 2023-04-17 00:35:06.000000 samppy-1.3.0/src/samppy.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)        7 2023-04-17 00:35:06.000000 samppy-1.3.0/src/samppy.egg-info/top_level.txt
```

### Comparing `samppy-1.2.2/LICENSE.txt` & `samppy-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samppy-1.2.2/PKG-INFO` & `samppy-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: samppy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Hamiltonian sampling and analysis of sampled distributions
-Home-page: UNKNOWN
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: sampling,Hamiltonian,MCMC,Bayesian,credibility,entropy
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Package **samppy** implements Hamiltonian Markov-chain sampling and
 some additional analysis methods for multivariate probability distributions.
 
 The probability distribution is represented only by
 an array of independent and identically distributed (i.i.d.) samples
 drawn from the distribution.
 
-The package includes three modules:
+The package includes four modules:
 
 * Module **hamiltonian_sampler** implements Hamiltonian Markov-Chain sampling.
     A *HamiltonianSampler* instance can generate
     random samples of a multivariate probability distribution,
     defined only by an non-normalized *log-likelihood* function,
     and the *gradient* of that function.
 
@@ -38,50 +36,61 @@
     Class `HamiltonianSampler` defines a standard isotropic sampler.
     Class `HamiltonianBoundedSampler` is a subclass also allowing
     one- or two-sided interval limits for all vector elements.
 
 * Module **credibility** includes functions to estimate *jointly credible differences*
     and/or *correlations* between pairs of elements
     in a random vector with a multivariate probability distribution,
-    represented only by samples.
+    represented only by samples. 
+    
+* A separate module **credibility_pd** has the same functionality, 
+    but operates on input data in Pandas DataFrame or Series format.
 
 * Module **sample_entropy** includes a function to estimate the *differential entropy*
     of a multivariate probability distribution, represented only by samples.
     The entropy is estimated by the Kozachenko-Leonenko nearest-neighbor approximation
     (Singh and Poczos, 2016).
 
 ## Usage
 
 This package was developed mainly for use by another project.
 It is distributed separately because it may be useful for other purposes.
 
 The Hamiltonian sampler code was inspired by the LAHMC project by
 Jasha Sohlstein. The present implementation includes
 some safety features to facilitate its use.
-The present sampler does *not* include sampling within a general subspace manifold.
+The present sampler does *not* include sampling within a general subspace manifold,
+but it allows bounded ranges for vector elements.
 
 ## Requirements
 
-The package requires Python 3.6 with Numpy and Scipy installed.
-It has been tested with Numpy v. 1.17 and Scipy v. 1.5.4.
+The package requires recent versions of Numpy and Scipy. 
+These are automatically installed.
+Pandas is not installed automatically, 
+because the module requiring Pandas input 
+will only be called from a program that already uses Pandas.
 
 ## References
 
 R M Neal (2011): MCMC using Hamiltonian dynamics. Ch. 5 in
 Brooks et al. (eds) *Handbook of Markov Chain Monte Carlo*.
 Chapman and Hall / CRC Press.
 
 A. Leijon, G. E. Henter, and M. Dahlquist (2016):
 Bayesian analysis of phoneme confusion matrices.
 *IEEE Transactions on Audio, Speech, and Language Processing* 24(3):469–482.
 (Describes an application of credible-difference calculation.)
 
+A. Leijon, P. von Gablenz, I. Holube, J. Taghia, and K. Smeds (2023).
+Bayesian analysis of ecological momentary assessment (EMA) data
+collected in adults before and after hearing rehabilitation. 
+*Frontiers in Digital Health*, 5(1100705).
+[download](https://www.frontiersin.org/articles/10.3389/fdgth.2023.1100705/full)
+
 F Perez-Cruz (2008): Estimation of Information Theoretic Measures
 for Continuous Random Variables.
 *Advances in Neural Information Processing Systems 21 (NIPS 2008)*.
 
 S Singh and B Poczos (2016): Analysis of k-nearest neighbor distances
 with application to entropy estimation.
 *arXiv:1603.08578 [math.ST]*.
 
-
-
```

### Comparing `samppy-1.2.2/setup.cfg` & `samppy-1.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 author_email = leijon@kth.se
 description = Hamiltonian sampling and analysis of sampled distributions
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
 classifiers = 
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.9
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Information Analysis
 keywords = 
 	sampling
 	Hamiltonian
@@ -22,17 +22,17 @@
 	credibility
 	entropy
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.9
 install_requires = 
-	numpy >=1.17
+	numpy >=1.23
 	scipy
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `samppy-1.2.2/src/samppy/__init__.py` & `samppy-1.3.0/src/samppy/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """This package includes modules for standard Hamiltonian MCMC sampling
 and for some analyses of the posterior distribution
 defined by an array of (possibly Hamiltonian-generated) samples.
 
 *** Version history:
+* Version 1.3.0:
+2023-04-16, new module credibility_pd.py, for Pandas input data format
 
 * Version 1.2.2:
 2021-11-03, removed logger.setlevel(DEBUG), to inherit __main__ logger level
 
 * Version 1.2.1:
 2021-09-12, cleanup doc and some bugfix in module credibility
 2021-09-29, stricter test for Markov chain stability in module hamiltonian_sampler
@@ -20,10 +22,10 @@
     Require Generator class from numpy.random v 1.17
 
 * Version 1.0.5, 2018-09-13, minor cleanup, fixes
 
 * Version 1.0.3, 2018-08-15, first published version
 """
 __name__ = 'samppy'
-__version__ = '1.2.2'
-__all__ = ['hamiltonian_sampler', 'credibility', 'sample_entropy']
+__version__ = '1.3.0'
+__all__ = ['hamiltonian_sampler', 'credibility', 'credibility_pd', 'sample_entropy']
```

### Comparing `samppy-1.2.2/src/samppy/credibility.py` & `samppy-1.3.0/src/samppy/credibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """This module calculates jointly credible differences
 between elements of random vectors, represented by
 sample vectors drawn from a multivariate distribution.
 
+This is the original version, with functions taking input as numpy arrays.
+
 Method reference:
 A. Leijon, G. E. Henter, and M. Dahlquist.
 Bayesian analysis of phoneme confusion matrices.
 IEEE Transactions on Audio, Speech, and Language Processing 24(3):469–482, 2016.
 
 *** Version History:
```

### Comparing `samppy-1.2.2/src/samppy/hamiltonian_sampler.py` & `samppy-1.3.0/src/samppy/hamiltonian_sampler.py`

 * *Files identical despite different names*

### Comparing `samppy-1.2.2/src/samppy/sample_entropy.py` & `samppy-1.3.0/src/samppy/sample_entropy.py`

 * *Files identical despite different names*

### Comparing `samppy-1.2.2/src/samppy.egg-info/PKG-INFO` & `samppy-1.3.0/src/samppy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: samppy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Hamiltonian sampling and analysis of sampled distributions
-Home-page: UNKNOWN
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: sampling,Hamiltonian,MCMC,Bayesian,credibility,entropy
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Package **samppy** implements Hamiltonian Markov-chain sampling and
 some additional analysis methods for multivariate probability distributions.
 
 The probability distribution is represented only by
 an array of independent and identically distributed (i.i.d.) samples
 drawn from the distribution.
 
-The package includes three modules:
+The package includes four modules:
 
 * Module **hamiltonian_sampler** implements Hamiltonian Markov-Chain sampling.
     A *HamiltonianSampler* instance can generate
     random samples of a multivariate probability distribution,
     defined only by an non-normalized *log-likelihood* function,
     and the *gradient* of that function.
 
@@ -38,50 +36,61 @@
     Class `HamiltonianSampler` defines a standard isotropic sampler.
     Class `HamiltonianBoundedSampler` is a subclass also allowing
     one- or two-sided interval limits for all vector elements.
 
 * Module **credibility** includes functions to estimate *jointly credible differences*
     and/or *correlations* between pairs of elements
     in a random vector with a multivariate probability distribution,
-    represented only by samples.
+    represented only by samples. 
+    
+* A separate module **credibility_pd** has the same functionality, 
+    but operates on input data in Pandas DataFrame or Series format.
 
 * Module **sample_entropy** includes a function to estimate the *differential entropy*
     of a multivariate probability distribution, represented only by samples.
     The entropy is estimated by the Kozachenko-Leonenko nearest-neighbor approximation
     (Singh and Poczos, 2016).
 
 ## Usage
 
 This package was developed mainly for use by another project.
 It is distributed separately because it may be useful for other purposes.
 
 The Hamiltonian sampler code was inspired by the LAHMC project by
 Jasha Sohlstein. The present implementation includes
 some safety features to facilitate its use.
-The present sampler does *not* include sampling within a general subspace manifold.
+The present sampler does *not* include sampling within a general subspace manifold,
+but it allows bounded ranges for vector elements.
 
 ## Requirements
 
-The package requires Python 3.6 with Numpy and Scipy installed.
-It has been tested with Numpy v. 1.17 and Scipy v. 1.5.4.
+The package requires recent versions of Numpy and Scipy. 
+These are automatically installed.
+Pandas is not installed automatically, 
+because the module requiring Pandas input 
+will only be called from a program that already uses Pandas.
 
 ## References
 
 R M Neal (2011): MCMC using Hamiltonian dynamics. Ch. 5 in
 Brooks et al. (eds) *Handbook of Markov Chain Monte Carlo*.
 Chapman and Hall / CRC Press.
 
 A. Leijon, G. E. Henter, and M. Dahlquist (2016):
 Bayesian analysis of phoneme confusion matrices.
 *IEEE Transactions on Audio, Speech, and Language Processing* 24(3):469–482.
 (Describes an application of credible-difference calculation.)
 
+A. Leijon, P. von Gablenz, I. Holube, J. Taghia, and K. Smeds (2023).
+Bayesian analysis of ecological momentary assessment (EMA) data
+collected in adults before and after hearing rehabilitation. 
+*Frontiers in Digital Health*, 5(1100705).
+[download](https://www.frontiersin.org/articles/10.3389/fdgth.2023.1100705/full)
+
 F Perez-Cruz (2008): Estimation of Information Theoretic Measures
 for Continuous Random Variables.
 *Advances in Neural Information Processing Systems 21 (NIPS 2008)*.
 
 S Singh and B Poczos (2016): Analysis of k-nearest neighbor distances
 with application to entropy estimation.
 *arXiv:1603.08578 [math.ST]*.
 
-
-
```

