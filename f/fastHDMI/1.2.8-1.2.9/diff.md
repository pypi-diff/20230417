# Comparing `tmp/fastHDMI-1.2.8.tar.gz` & `tmp/fastHDMI-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastHDMI-1.2.8.tar", last modified: Wed Jan 11 02:23:02 2023, max compression
+gzip compressed data, was "fastHDMI-1.2.9.tar", last modified: Wed Jan 11 04:28:24 2023, max compression
```

## Comparing `fastHDMI-1.2.8.tar` & `fastHDMI-1.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.2.8/LICENSE
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4825 2023-01-05 11:57:51.000000 fastHDMI-1.2.8/README.md
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      996 2023-01-11 02:17:00.000000 fastHDMI-1.2.8/pyproject.toml
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/setup.cfg
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/src/
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/src/fastHDMI/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   171268 2023-01-11 02:21:58.000000 fastHDMI-1.2.8/src/fastHDMI/__init__.py
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 02:23:02.534267 fastHDMI-1.2.8/src/fastHDMI.egg-info/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 02:23:02.000000 fastHDMI-1.2.8/src/fastHDMI.egg-info/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      201 2023-01-11 02:23:02.000000 fastHDMI-1.2.8/src/fastHDMI.egg-info/SOURCES.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-01-11 02:23:02.000000 fastHDMI-1.2.8/src/fastHDMI.egg-info/dependency_links.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-01-11 02:23:02.000000 fastHDMI-1.2.8/src/fastHDMI.egg-info/top_level.txt
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.2.9/LICENSE
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4825 2023-01-05 11:57:51.000000 fastHDMI-1.2.9/README.md
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      996 2023-01-11 04:25:53.000000 fastHDMI-1.2.9/pyproject.toml
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/setup.cfg
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/fastHDMI/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   171269 2023-01-11 04:27:25.000000 fastHDMI-1.2.9/src/fastHDMI/__init__.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/fastHDMI.egg-info/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      201 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/SOURCES.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/dependency_links.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/top_level.txt
```

### Comparing `fastHDMI-1.2.8/LICENSE` & `fastHDMI-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.2.8/PKG-INFO` & `fastHDMI-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.2.8
+Version: 1.2.9
 Summary: Use fast FFT-based mutual information and accelerated gradient method to filter out and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fastHDMI-1.2.8/README.md` & `fastHDMI-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.2.8/pyproject.toml` & `fastHDMI-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "numpy>=1.14.2", "numba>=0.54.1", "KDEpy>=1.1.0", "scikit-learn>=1.0.2", "bed_reader", "multiprocess>=0.70.6",  "bed-reader", "pandas>=1.4.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastHDMI"
-version = "1.2.8"
+version = "1.2.9"
 authors = [
   { name="Kai Yang", email="kai.yang2@mail.mcgill.ca" },
 ]
 description = "Use fast FFT-based mutual information and accelerated gradient method to filter out and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `fastHDMI-1.2.8/src/fastHDMI/__init__.py` & `fastHDMI-1.2.9/src/fastHDMI/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # first estimate the pmf
     p0 = _np.sum(b == 0) / len(b)
     p1 = _np.sum(b == 1) / len(b)
     p2 = 1. - p0 - p1
     _a = _scaler().fit_transform(a.reshape(-1, 1)).flatten()
     # this step is just to get the boundary width for the joint density grid
     # the three conditional density estimates need to be evaluated on the joint density grid
-    a_temp, _ = _FFTKDE(kernel=kernel, bw=bw).fit(data=a).evaluate(N)
+    a_temp, _ = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a).evaluate(N)
     # estimate cond density
     _b0 = (b == 0)
     if _np.sum(_b0) > 2:
         # here proceed to kde only if there are more than 5 data points
         y_cond_p0 = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a[_b0])
 #         y_cond_p0 = gaussian_kde(_a[_b0])
     else:
```

### Comparing `fastHDMI-1.2.8/src/fastHDMI.egg-info/PKG-INFO` & `fastHDMI-1.2.9/src/fastHDMI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.2.8
+Version: 1.2.9
 Summary: Use fast FFT-based mutual information and accelerated gradient method to filter out and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

