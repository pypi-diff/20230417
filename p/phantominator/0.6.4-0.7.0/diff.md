# Comparing `tmp/phantominator-0.6.4.tar.gz` & `tmp/phantominator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phantominator-0.6.4.tar", last modified: Sun Apr 26 04:43:12 2020, max compression
+gzip compressed data, was "phantominator-0.7.0.tar", last modified: Sun Apr 16 22:24:01 2023, max compression
```

## Comparing `phantominator-0.6.4.tar` & `phantominator-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 nicholas  (1000) nicholas  (1000)        0 2020-04-26 04:43:12.000000 phantominator-0.6.4/
-drwxr-xr-x   0 nicholas  (1000) nicholas  (1000)        0 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)       14 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/top_level.txt
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     3670 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/PKG-INFO
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)       57 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/requires.txt
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)        1 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/dependency_links.txt
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)      422 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator.egg-info/SOURCES.txt
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     3670 2020-04-26 04:43:12.000000 phantominator-0.6.4/PKG-INFO
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)       38 2020-04-26 04:43:12.000000 phantominator-0.6.4/setup.cfg
-drwxr-xr-x   0 nicholas  (1000) nicholas  (1000)        0 2020-04-26 04:43:12.000000 phantominator-0.6.4/phantominator/
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     1326 2019-10-08 21:56:47.000000 phantominator-0.6.4/phantominator/traj.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     1183 2019-08-20 14:01:19.000000 phantominator-0.6.4/phantominator/dynamic.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)    17431 2019-09-19 21:57:58.000000 phantominator-0.6.4/phantominator/sens_coeffs.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     6818 2020-04-26 04:42:44.000000 phantominator-0.6.4/phantominator/kspace.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     8871 2019-12-28 03:41:17.000000 phantominator-0.6.4/phantominator/ct_shepp_logan.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     7837 2019-12-28 03:39:17.000000 phantominator-0.6.4/phantominator/mr_shepp_logan.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)      426 2019-12-28 03:42:39.000000 phantominator-0.6.4/phantominator/__init__.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)      676 2019-09-12 21:54:13.000000 phantominator-0.6.4/phantominator/shepp_logan.py
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)     2703 2019-12-28 04:13:29.000000 phantominator-0.6.4/README.rst
--rw-r--r--   0 nicholas  (1000) nicholas  (1000)      592 2020-04-26 04:42:07.000000 phantominator-0.6.4/setup.py
+drwxrwxr-x   0 nmckibben  (1000) nmckibben  (1000)        0 2023-04-16 22:24:01.241398 phantominator-0.7.0/
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     1061 2023-04-16 21:30:10.000000 phantominator-0.7.0/LICENSE
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     3196 2023-04-16 22:24:01.241398 phantominator-0.7.0/PKG-INFO
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     2928 2023-04-16 22:11:39.000000 phantominator-0.7.0/README.rst
+drwxrwxr-x   0 nmckibben  (1000) nmckibben  (1000)        0 2023-04-16 22:24:01.237398 phantominator-0.7.0/phantominator/
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      426 2023-04-16 21:34:49.000000 phantominator-0.7.0/phantominator/__init__.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     9636 2023-04-16 22:15:26.000000 phantominator-0.7.0/phantominator/ct_shepp_logan.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     1238 2023-04-16 21:56:32.000000 phantominator-0.7.0/phantominator/dynamic.py
+drwxrwxr-x   0 nmckibben  (1000) nmckibben  (1000)        0 2023-04-16 22:24:01.241398 phantominator-0.7.0/phantominator/examples/
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)        0 2023-04-16 21:32:39.000000 phantominator-0.7.0/phantominator/examples/__init__.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      753 2023-04-16 22:08:24.000000 phantominator-0.7.0/phantominator/examples/dynamic.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     2394 2023-04-16 22:09:15.000000 phantominator-0.7.0/phantominator/examples/gach_figs.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      782 2023-04-16 22:09:55.000000 phantominator-0.7.0/phantominator/examples/modify_parameters.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      681 2023-04-16 22:10:21.000000 phantominator-0.7.0/phantominator/examples/mr_shepp_logan.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     1535 2023-04-16 22:10:59.000000 phantominator-0.7.0/phantominator/examples/radial_coil_sens.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     1208 2023-04-16 22:17:49.000000 phantominator-0.7.0/phantominator/examples/shepp_logan.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     7137 2023-04-16 22:13:25.000000 phantominator-0.7.0/phantominator/kspace.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     8186 2023-04-16 22:07:43.000000 phantominator-0.7.0/phantominator/mr_shepp_logan.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)    17522 2023-04-16 22:05:12.000000 phantominator-0.7.0/phantominator/sens_coeffs.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      677 2023-04-16 22:05:57.000000 phantominator-0.7.0/phantominator/shepp_logan.py
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     1390 2023-04-16 22:06:48.000000 phantominator-0.7.0/phantominator/traj.py
+drwxrwxr-x   0 nmckibben  (1000) nmckibben  (1000)        0 2023-04-16 22:24:01.237398 phantominator-0.7.0/phantominator.egg-info/
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)     3196 2023-04-16 22:24:01.000000 phantominator-0.7.0/phantominator.egg-info/PKG-INFO
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      701 2023-04-16 22:24:01.000000 phantominator-0.7.0/phantominator.egg-info/SOURCES.txt
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)        1 2023-04-16 22:24:01.000000 phantominator-0.7.0/phantominator.egg-info/dependency_links.txt
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)       57 2023-04-16 22:24:01.000000 phantominator-0.7.0/phantominator.egg-info/requires.txt
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)       14 2023-04-16 22:24:01.000000 phantominator-0.7.0/phantominator.egg-info/top_level.txt
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)       38 2023-04-16 22:24:01.241398 phantominator-0.7.0/setup.cfg
+-rw-rw-r--   0 nmckibben  (1000) nmckibben  (1000)      591 2023-04-16 22:21:34.000000 phantominator-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `phantominator-0.6.4/phantominator.egg-info/PKG-INFO` & `phantominator-0.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: phantominator
-Version: 0.6.4
+Version: 0.7.0
 Summary: Generate numerical phantoms.
 Home-page: https://github.com/mckib2/phantominator
 Author: Nicholas McKibben
 Author-email: nicholas.bgp@gmail.com
-License: GPLv3
-Description: Installation
-        ============
-        
-        .. code-block:: bash
-        
-            pip install phantominator
-        
-        The goal is to have easy installation and usage for everyone.  If
-        something doesn't work, please open an issue and/or submit a pull
-        request.  We'll get it figured out.
-        
-        About
-        =====
-        
-        Python package for easy generation of numerical phantoms.  I often
-        need a simple image to try something out on.  In MATLAB, I would use
-        the `phantom` command to quickly get something to work with.  In
-        Python, it's not quite so easy, so I made this package that's quick
-        to install and use so there's as little friction as possible.  There
-        are other implementations of Shepp-Logan available from other
-        projects, but they are usually not as easy to install or include other
-        things that I don't want for this project.
-        
-        This package offers both CT and MR versions.
-        
-        Going forward, this module will no longer support Python 2.  Please do
-        the world a favor and move on to Python 3.
-        
-        Usage
-        =====
-        
-        Also see the `examples` module and docstrings.  The interface for CT
-        phantom generation is similar to MATLAB's `phantom` function.
-        
-        Basic usage:
-        
-        .. code-block:: python
-        
-            # CT phantom
-            from phantominator import shepp_logan
-            ph = shepp_logan(128)
-        
-            # MR phantom (returns proton density, T1, and T2 maps)
-            M0, T1, T2 = shepp_logan((128, 128, 20), MR=True)
-        
-        The Shepp-Logan 3D phantom has ellipsoids in [-1, 1] along the z-axis.
-        The 2D Shepp-Logan exists at z=-0.25, so if we want just a subset
-        along the z-axis with the first slice being the traditional 2D
-        phantom, we can use the `zlims` option:
-        
-        .. code-block:: python
-        
-            from phantominator import shepp_logan
-            M0, T1, T2 = shepp_logan((64, 64, 5), MR=True, zlims=(-.25, .25))
-        
-        We can also generate simple oscillating concentric circles:
-        
-        .. code-block:: python
-        
-            # Dynamic (concentric circles), 20 time frames
-            from phantominator import dynamic
-            ph = dynamic(128, 20)
-        
-        If we want to modify ellipse/ellipsoid parameters or we just want to
-        see what they are.  For example, we can get the MR ellipsoid
-        parameters like this:
-        
-        .. code-block:: python
-        
-            from phantominator import mr_ellipsoid_parameters
-            E = mr_ellipsoid_parameters()
-        
-        See docstrings for `ct_shepp_logan`, and `mr_shepp_logan` for how
-        the array `E` is structured.  It follows conventions from MATLAB's
-        phantom function.
-        
-        Arbitrary k-space sampling is supported for the single coil 2D
-        Shepp-Logan phantom:
-        
-        .. code-block:: python
-        
-            # Given k-space coordinates (kx, ky), where kx and ky are 1D
-            # arrays using the same unit conventions as BART's traj command,
-            # we can find the corresponding k-space measurements:
-            from phantominator import kspace_shepp_logan
-            k = kspace_shepp_logan(kx, ky)
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
+License: MIT
+Requires-Python: >=3.8
+License-File: LICENSE
+
+Installation
+============
+
+.. code-block:: bash
+
+    python -m pip install phantominator
+
+The goal is to have easy installation and usage for everyone.  If
+something doesn't work, please open an issue and/or submit a pull
+request.  We'll get it figured out.
+
+`pygrappa` is an optional dependency required to run the
+`phantominator.examples.radial_coil_sens` example.
+
+About
+=====
+
+Python package for easy generation of numerical phantoms.  I often
+need a simple image to try something out on.  In MATLAB, I would use
+the `phantom` command to quickly get something to work with.  In
+Python, it's not always quite so easy, so I made this package that's quick
+to install and use so there's as little friction as possible.  There
+are other implementations of Shepp-Logan available from other
+projects, but they are usually not as easy to install or include other
+things that I don't want for this project.
+
+This package offers both CT and MR versions.
+
+Going forward, this module will support Python >= 3.8.
+
+Usage
+=====
+
+Also see the `examples` module and docstrings.  The interface for CT
+phantom generation is similar to MATLAB's `phantom` function.
+
+Examples can be run as:
+
+.. code-block:: bash
+
+    # python -m phantominator.examples.[example-name], e.g.:
+    python -m phantominator.examples.shepp_logan
+
+Basic usage:
+
+.. code-block:: python
+
+    # CT phantom
+    from phantominator import shepp_logan
+    ph = shepp_logan(128)
+
+    # MR phantom (returns proton density, T1, and T2 maps)
+    M0, T1, T2 = shepp_logan((128, 128, 20), MR=True)
+
+The Shepp-Logan 3D phantom has ellipsoids in [-1, 1] along the z-axis.
+The 2D Shepp-Logan exists at z=-0.25, so if we want just a subset
+along the z-axis with the first slice being the traditional 2D
+phantom, we can use the `zlims` option:
+
+.. code-block:: python
+
+    from phantominator import shepp_logan
+    M0, T1, T2 = shepp_logan((64, 64, 5), MR=True, zlims=(-.25, .25))
+
+We can also generate simple oscillating concentric circles:
+
+.. code-block:: python
+
+    # Dynamic (concentric circles), 20 time frames
+    from phantominator import dynamic
+    ph = dynamic(128, 20)
+
+If we want to modify ellipse/ellipsoid parameters or we just want to
+see what they are.  For example, we can get the MR ellipsoid
+parameters like this:
+
+.. code-block:: python
+
+    from phantominator import mr_ellipsoid_parameters
+    E = mr_ellipsoid_parameters()
+
+See docstrings for `ct_shepp_logan`, and `mr_shepp_logan` for how
+the array `E` is structured.  It follows conventions from MATLAB's
+phantom function.
+
+Arbitrary k-space sampling is supported for the single coil 2D
+Shepp-Logan phantom:
+
+.. code-block:: python
+
+    # Given k-space coordinates (kx, ky), where kx and ky are 1D
+    # arrays using the same unit conventions as BART's traj command,
+    # we can find the corresponding k-space measurements:
+    from phantominator import kspace_shepp_logan
+    k = kspace_shepp_logan(kx, ky)
```

### Comparing `phantominator-0.6.4/PKG-INFO` & `phantominator-0.7.0/phantominator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: phantominator
-Version: 0.6.4
+Version: 0.7.0
 Summary: Generate numerical phantoms.
 Home-page: https://github.com/mckib2/phantominator
 Author: Nicholas McKibben
 Author-email: nicholas.bgp@gmail.com
-License: GPLv3
-Description: Installation
-        ============
-        
-        .. code-block:: bash
-        
-            pip install phantominator
-        
-        The goal is to have easy installation and usage for everyone.  If
-        something doesn't work, please open an issue and/or submit a pull
-        request.  We'll get it figured out.
-        
-        About
-        =====
-        
-        Python package for easy generation of numerical phantoms.  I often
-        need a simple image to try something out on.  In MATLAB, I would use
-        the `phantom` command to quickly get something to work with.  In
-        Python, it's not quite so easy, so I made this package that's quick
-        to install and use so there's as little friction as possible.  There
-        are other implementations of Shepp-Logan available from other
-        projects, but they are usually not as easy to install or include other
-        things that I don't want for this project.
-        
-        This package offers both CT and MR versions.
-        
-        Going forward, this module will no longer support Python 2.  Please do
-        the world a favor and move on to Python 3.
-        
-        Usage
-        =====
-        
-        Also see the `examples` module and docstrings.  The interface for CT
-        phantom generation is similar to MATLAB's `phantom` function.
-        
-        Basic usage:
-        
-        .. code-block:: python
-        
-            # CT phantom
-            from phantominator import shepp_logan
-            ph = shepp_logan(128)
-        
-            # MR phantom (returns proton density, T1, and T2 maps)
-            M0, T1, T2 = shepp_logan((128, 128, 20), MR=True)
-        
-        The Shepp-Logan 3D phantom has ellipsoids in [-1, 1] along the z-axis.
-        The 2D Shepp-Logan exists at z=-0.25, so if we want just a subset
-        along the z-axis with the first slice being the traditional 2D
-        phantom, we can use the `zlims` option:
-        
-        .. code-block:: python
-        
-            from phantominator import shepp_logan
-            M0, T1, T2 = shepp_logan((64, 64, 5), MR=True, zlims=(-.25, .25))
-        
-        We can also generate simple oscillating concentric circles:
-        
-        .. code-block:: python
-        
-            # Dynamic (concentric circles), 20 time frames
-            from phantominator import dynamic
-            ph = dynamic(128, 20)
-        
-        If we want to modify ellipse/ellipsoid parameters or we just want to
-        see what they are.  For example, we can get the MR ellipsoid
-        parameters like this:
-        
-        .. code-block:: python
-        
-            from phantominator import mr_ellipsoid_parameters
-            E = mr_ellipsoid_parameters()
-        
-        See docstrings for `ct_shepp_logan`, and `mr_shepp_logan` for how
-        the array `E` is structured.  It follows conventions from MATLAB's
-        phantom function.
-        
-        Arbitrary k-space sampling is supported for the single coil 2D
-        Shepp-Logan phantom:
-        
-        .. code-block:: python
-        
-            # Given k-space coordinates (kx, ky), where kx and ky are 1D
-            # arrays using the same unit conventions as BART's traj command,
-            # we can find the corresponding k-space measurements:
-            from phantominator import kspace_shepp_logan
-            k = kspace_shepp_logan(kx, ky)
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
+License: MIT
+Requires-Python: >=3.8
+License-File: LICENSE
+
+Installation
+============
+
+.. code-block:: bash
+
+    python -m pip install phantominator
+
+The goal is to have easy installation and usage for everyone.  If
+something doesn't work, please open an issue and/or submit a pull
+request.  We'll get it figured out.
+
+`pygrappa` is an optional dependency required to run the
+`phantominator.examples.radial_coil_sens` example.
+
+About
+=====
+
+Python package for easy generation of numerical phantoms.  I often
+need a simple image to try something out on.  In MATLAB, I would use
+the `phantom` command to quickly get something to work with.  In
+Python, it's not always quite so easy, so I made this package that's quick
+to install and use so there's as little friction as possible.  There
+are other implementations of Shepp-Logan available from other
+projects, but they are usually not as easy to install or include other
+things that I don't want for this project.
+
+This package offers both CT and MR versions.
+
+Going forward, this module will support Python >= 3.8.
+
+Usage
+=====
+
+Also see the `examples` module and docstrings.  The interface for CT
+phantom generation is similar to MATLAB's `phantom` function.
+
+Examples can be run as:
+
+.. code-block:: bash
+
+    # python -m phantominator.examples.[example-name], e.g.:
+    python -m phantominator.examples.shepp_logan
+
+Basic usage:
+
+.. code-block:: python
+
+    # CT phantom
+    from phantominator import shepp_logan
+    ph = shepp_logan(128)
+
+    # MR phantom (returns proton density, T1, and T2 maps)
+    M0, T1, T2 = shepp_logan((128, 128, 20), MR=True)
+
+The Shepp-Logan 3D phantom has ellipsoids in [-1, 1] along the z-axis.
+The 2D Shepp-Logan exists at z=-0.25, so if we want just a subset
+along the z-axis with the first slice being the traditional 2D
+phantom, we can use the `zlims` option:
+
+.. code-block:: python
+
+    from phantominator import shepp_logan
+    M0, T1, T2 = shepp_logan((64, 64, 5), MR=True, zlims=(-.25, .25))
+
+We can also generate simple oscillating concentric circles:
+
+.. code-block:: python
+
+    # Dynamic (concentric circles), 20 time frames
+    from phantominator import dynamic
+    ph = dynamic(128, 20)
+
+If we want to modify ellipse/ellipsoid parameters or we just want to
+see what they are.  For example, we can get the MR ellipsoid
+parameters like this:
+
+.. code-block:: python
+
+    from phantominator import mr_ellipsoid_parameters
+    E = mr_ellipsoid_parameters()
+
+See docstrings for `ct_shepp_logan`, and `mr_shepp_logan` for how
+the array `E` is structured.  It follows conventions from MATLAB's
+phantom function.
+
+Arbitrary k-space sampling is supported for the single coil 2D
+Shepp-Logan phantom:
+
+.. code-block:: python
+
+    # Given k-space coordinates (kx, ky), where kx and ky are 1D
+    # arrays using the same unit conventions as BART's traj command,
+    # we can find the corresponding k-space measurements:
+    from phantominator import kspace_shepp_logan
+    k = kspace_shepp_logan(kx, ky)
```

### Comparing `phantominator-0.6.4/phantominator/traj.py` & `phantominator-0.7.0/phantominator/traj.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-'''Sample k-space trajectories.'''
+"""Sample k-space trajectories."""
 
 from functools import partial
 
 import numpy as np
 
-def radial(sx, spokes, golden=False):
-    '''k-space coordinates for a radial trajectory.
+
+def radial(sx: int, spokes: int, golden: bool = False):
+    """k-space coordinates for a radial trajectory.
 
     Parameters
     ----------
     sx : int
         Number of samples along spoke.
     spokes : int
         Number of spokes.
@@ -21,36 +22,38 @@
     kx, ky : array_like
         k-space coordinates for sampling along a radial trajectory.
 
     Notes
     -----
     This is a very simple radial trajectory mainly for demonstration
     purposes.
-    '''
+    """
 
     N = sx*spokes
     kx = np.zeros(N)
     ky = np.zeros(N)
-    x = np.linspace(-1, 1, sx)*sx/2 # scale fac to match BART's traj
+    x = np.linspace(-1, 1, sx)*sx/2  # scale fac to match BART's traj
     y = np.zeros(sx)
 
     # How we get
     if golden:
-        GA = np.pi*(3 - np.sqrt(5)) # calculate GA for use if needed
+        GA = np.pi*(3 - np.sqrt(5))  # calculate GA for use if needed
         gettheta = partial(_nextspoke_golden, GA=GA)
     else:
         gettheta = partial(_nextspoke, spokes=spokes)
 
     for ii in range(spokes):
         # theta = ii/spokes*np.pi
         theta = gettheta(ii)
         ct = np.cos(theta)
         st = np.sin(theta)
         kx[ii*sx:(ii+1)*sx] = x*ct - y*st
         ky[ii*sx:(ii+1)*sx] = x*st + y*ct
-    return(kx, ky)
+    return kx, ky
+
 
-def _nextspoke(ii, spokes):
+def _nextspoke(ii: int, spokes: int) -> float:
     return ii/spokes*np.pi
 
-def _nextspoke_golden(ii, GA):
+
+def _nextspoke_golden(ii: float, GA: float) -> float:
     return GA*ii
```

### Comparing `phantominator-0.6.4/phantominator/dynamic.py` & `phantominator-0.7.0/phantominator/dynamic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-'''Simple dynamic numerical phantom.'''
+"""Simple dynamic numerical phantom."""
 
 import numpy as np
+import numpy.typing as npt
 
-def dynamic(N, nt):
-    '''Concentric circles with dynamic movement.
+
+def dynamic(N: int, nt: int) -> npt.ArrayLike:
+    """Concentric circles with dynamic movement.
 
     Parameters
     ----------
     N : int
         In-plane dimension.
     nt : int
         Number of time points.
 
     Returns
     -------
     ph : array_like
         Phantom of size (N, N, nt), time is last dimension.
-    '''
+    """
 
     ph = np.zeros((N, N, nt))
     X, Y = np.meshgrid(
         np.linspace(-1, 1, N),
         np.linspace(-1, 1, N))
 
     # Make an outer circle
```

### Comparing `phantominator-0.6.4/phantominator/sens_coeffs.py` & `phantominator-0.7.0/phantominator/sens_coeffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-'''Hard coded sensitivity map coefficients.'''
+"""Hard coded sensitivity map coefficients."""
+
+from typing import Tuple
 
 import numpy as np
+import numpy.typing as npt
+
+
+def _sens_info() -> Tuple[int, int]:
+    """Gives back max coil number of coefficient number."""
+    return 8, 36
 
-def _sens_info():
-    '''Gives back max coil number of coefficient number.'''
-    return (8, 36)
 
-def _sens_coeffs(coil): # pylint: disable=R0911
-    '''Get coefficients for a specified coil.
+def _sens_coeffs(coil) -> npt.ArrayLike:  # pylint: disable=R0911
+    """Get coefficients for a specified coil.
 
     Notes
     -----
     36 coefficients per coil for the sinusoidal model generated
     from MRIPhantomv0-8, the publicly available software implementing
     the simulations described in [1]_.
 
     References
     ----------
     .. [1] Guerquin-Kern, Matthieu, et al. "Realistic analytical
            phantoms for parallel magnetic resonance imaging." IEEE
            Transactions on Medical Imaging 31.3 (2011): 626-636.
-    '''
+    """
 
-    if coil == 0: # pylint: disable=R1705
+    if coil == 0:  # pylint: disable=R1705
         return np.array([
             -0.000492664219250141 + 1j*0.00243037030094894,
             0.00288946657806461 - 1j*0.0191953858873134,
             -0.0105363006844095 + 1j*0.0604610659193525,
             0.0123853502735897 - 1j*0.0498374567765950,
             -0.00920408874684275 + 1j*0.0632845329625142,
             0.000358598059238050 + 1j*0.00886701389084563,
```

### Comparing `phantominator-0.6.4/phantominator/kspace.py` & `phantominator-0.7.0/phantominator/kspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-'''Analytical form of Shepp-Logan kspace.'''
+"""Analytical form of Shepp-Logan kspace."""
 
 from time import time
-import numpy as np
-try:
-    from math import tau
-except:
-    tau = 2*np.pi
+from math import tau
+from typing import Optional
 
-from scipy.special import j1 # pylint: disable=E0611
+import numpy as np
+import numpy.typing as npt
+from scipy.special import j1
 
 from phantominator import (
-    ct_shepp_logan_params_2d, ct_modified_shepp_logan_params_2d)
+    ct_shepp_logan_params_2d,
+    ct_modified_shepp_logan_params_2d
+)
 from phantominator.sens_coeffs import _sens_coeffs, _sens_info
 
 
 def kspace_shepp_logan(
-        kx, ky=None, modified=True, E=None, ncoil=None):
-    '''2D Shepp-Logan phantom kspace measurements at points (kx, ky).
+        kx: npt.ArrayLike, ky: Optional[npt.ArrayLike] = None,
+        modified: bool = True,
+        E: Optional[npt.ArrayLike] = None,
+        ncoil: int = None) -> npt.ArrayLike:
+    """2D Shepp-Logan phantom kspace measurements at points (kx, ky).
 
     Parameters
     ----------
     kx, ky : array_like
         1D arrays corresponding to kspace coordinates.  Coordinate
         units are the same as those returned by BART's traj function.
         If ky=None, then kx should be a complex-valued array
         corresponding to kx + 1j*ky.
     modified : bool, optional
         Use original grey-scale values as given or use modified
         values for better contrast.
     E : array_like, optional
         See ct_shepp_logan for details.
+    ncoil : int, optional
+        Generate sensitivity maps for ncoil coils.
 
     Returns
     -------
     k : array_like
         1D array of kspace measurements corresponding to coordinates
         (kx, ky).
 
     References
     ----------
     .. [1] Van de Walle, Rik, et al. "Reconstruction of MR images
            from data acquired on a general nonregular grid by
            pseudoinverse calculation." IEEE transactions on medical
            imaging 19.12 (2000): 1160-1167.
-    '''
+    """
 
     if ky is None:
         k = np.asarray(kx)
     else:
         kx, ky = np.asarray(kx), np.asarray(ky)
         assert kx.shape == ky.shape, (
             'kx and ky must be the same size!')
@@ -73,20 +79,20 @@
         MAX_COIL, NUM_COEFF = _sens_info()
         assert ncoil <= MAX_COIL, (
             'Only %d coils possible to simulate!' % MAX_COIL)
         t0 = time()
 
         # Build up the coefficient matrix, we'll do all coils for
         # each ellipse at the same time for efficiency
-        coeffs = np.zeros((ncoil, NUM_COEFF), dtype=np.complex)
+        coeffs = np.zeros((ncoil, NUM_COEFF), dtype=complex)
         for cc in range(ncoil):
             coeffs[cc, :] = _sens_coeffs(cc)
 
         # Add up all the ellipse kspaces with all coils
-        val = np.zeros((k.size, ncoil), dtype=np.complex)
+        val = np.zeros((k.size, ncoil), dtype=complex)
         for ii in range(E.shape[0]):
             # Have to get screwy with the center coordinates to make
             # it work.  Not sure what's different between us and
             # MATLAB script...
             val += _kspace_ellipse_sens(
                 k, ys[ii]/2, -xs[ii]/2, grey[ii], major[ii],
                 minor[ii], alphas[ii], coeffs).T
@@ -95,59 +101,62 @@
             time() - t0, ncoil))
         return val
 
     # Same for kspace coordinates.  Factor of 2 to match up with
     # BART's traj function
     # FIXME: Scaling removed so that this matches Matlab mriphantom.
     #        Which was is correct?
-    #k /= 2
+    # k /= 2
 
     # Sum of ellipses
     return np.sum(_kspace_ellipse(k, E), axis=-1)
 
-def _kspace_ellipse(k, E):
-    '''Generates Fourier transform of (an array of) a general ellipse.
+
+def _kspace_ellipse(k: npt.ArrayLike, E: npt.ArrayLike) -> npt.ArrayLike:
+    """Generates Fourier transform of (an array of) a general ellipse.
 
     Notes
     -----
     Implements equation [21] in [1]_.
-    '''
+    """
     k = np.asarray(k)
     rho, A, B, xc, yc, alpha = np.asarray(E).T
     E = rho*A*B
     Ec = xc + 1j*yc
-    ret = np.empty(shape=np.shape(k) + np.shape(E), dtype=np.complex)
+    ret = np.empty(shape=np.shape(k) + np.shape(E), dtype=complex)
     zero = np.isclose(k, 0)
     ret[zero] = .5*tau*E  # lim a->0: j1(tau * a) / a = .5 * tau
     k = k[~zero, None]
     if k.size:
         k, theta = abs(k), np.angle(k)
         t, gamma = abs(Ec), np.angle(Ec)
         athetak = _a(A, B, theta, alpha)*k
         rotation = np.exp(-1j*tau*k*t*np.cos(gamma - theta))
         ret[~zero] = rotation*E*j1(tau*athetak)/athetak
     return ret
 
-def _a(A, B, theta, alpha):
+
+def _a(A: npt.ArrayLike, B: npt.ArrayLike, theta: npt.ArrayLike, alpha: npt.ArrayLike) -> npt.ArrayLike:
     return np.sqrt(
         A**2*np.cos(theta - alpha)**2 + B**2*np.sin(theta - alpha)**2)
 
+
 def _kspace_ellipse_sens(k, xc, yc, rho, A, B, theta, coeffs):
-    '''Fourier transform of ellipse with polynomial sensitivity map.
-    '''
+    """Fourier transform of ellipse with polynomial sensitivity map."""
 
     width = np.array([B, A])
     ct, st = np.cos(theta), np.sin(theta)
     Rmat = np.array([[ct, -st], [st, ct]])
     Dmat = np.diag(width/2)
 
     return rho*MRDataEllipseSinusoidal(k, Dmat, Rmat, xc, yc, coeffs)
 
+
 def MRDataEllipseSinusoidal(k, Dmat, Rmat, xc, yc, coeffs):
-    '''Sinusoidal model'''
+    """Sinusoidal model"""
     N = coeffs.shape[1]
     L = int(np.floor(np.sqrt(N)))
 
     k = np.concatenate((k.real[None, :], k.imag[None, :]), axis=0)
     Nk = k.shape[1]
 
     ky, kx = np.meshgrid(
@@ -168,14 +177,15 @@
     ind_big = np.abs(modw) >= 1e-10
     Gval[ind_big] = j1(modw[ind_big])/modw[ind_big]
     Gval[~ind_big] = .5*(1 - (modw[~ind_big]/2)**2/2)
 
     return tau*np.linalg.det(Dmat)*coeffs @ (
         np.exp(1j*tau*(xc*kx + yc*ky))*Gval)
 
+
 if __name__ == '__main__':
     pass
     # # Example usage (requires pygrappa package to be installed!)
     # from phantominator.traj import radial
     # from scipy.cluster.vq import whiten # pylint: disable=C0412
     # import matplotlib.pyplot as plt
     # from pygrappa import radialgrappaop, grog # pylint: disable=E0611
```

### Comparing `phantominator-0.6.4/phantominator/ct_shepp_logan.py` & `phantominator-0.7.0/phantominator/ct_shepp_logan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # -*- coding: utf-8 -*-
-'''The canonical Shepp-Logan phantom used for CT simulations.'''
+"""The canonical Shepp-Logan phantom used for CT simulations."""
+
+from typing import Tuple, Optional, Union
 
 import numpy as np
+import numpy.typing as npt
+
 
 def ct_shepp_logan(
-        N, modified=True, E=None, ret_E=False, zlims=(-1, 1)):
-    '''Generate a Shepp-Logan phantom of size (N, N).
+        N: Union[int, npt.ArrayLike],
+        modified: bool = True,
+        E: Optional[npt.ArrayLike] = None,
+        ret_E: bool = False,
+        zlims: Tuple[float, float] = (-1, 1)) -> Union[npt.ArrayLike, Tuple[npt.ArrayLike, npt.ArrayLike]]:
+    """Generate a Shepp-Logan phantom of size (N, N).
 
     Parameters
     ----------
     N : int or array_like
         Matrix size, (N, N) or (M, N) or (L, M, N).
     modified : bool, optional
         Use original grey-scale values as given in [1]_.  Most
         implementations use modified values for better contrast (for
         example, see [3]_ and [4]_).
     E : array_like, optional
         For 2D: ex6 numeric matrix defining e ellipses.  The six
         columns of E are:
 
+            - Gray value of the ellipse (in [0, 1])
             - Length of the horizontal semiaxis of the ellipse
             - Length of the vertical semiaxis of the ellipse
             - x-coordinate of the center of the ellipse (in [-1, 1])
             - y-coordinate of the center of the ellipse (in [-1, 1])
             - Angle between the horizontal semiaxis of the ellipse
               and the x-axis of the image (in rad)
 
@@ -75,37 +84,36 @@
     .. [5] Toft, Peter Aundal, and John Aasted Sørensen. "The Radon
            transform-theory and implementation." (1996).
     .. [6] Koay, Cheng Guan, Joelle E. Sarlls, and Evren Özarslan.
            "Three‐dimensional analytical magnetic resonance imaging
            phantom in the Fourier domain." Magnetic Resonance in
            Medicine: An Official Journal of the International Society
            for Magnetic Resonance in Medicine 58.2 (2007): 430-436.
-    '''
+    """
 
     # Get size of phantom
     if np.isscalar(N):
         M, N = N, N
-        is2D = True
-    else:
-        if len(N) == 2:
-            M, N = N[:]
-            is2D = True
-        elif len(N) == 3:
-            L, M, N = N[:]
-            is2D = False
-        else:
-            raise ValueError('Dimension must be scalar, 2D, or 3D!')
+        return ct_shepp_logan_2d(M, N, modified, E, ret_E)
 
-    # Give back either a 2D or 3D phantom
-    if is2D:
+    if len(N) == 2:
+        M, N = N[:]
         return ct_shepp_logan_2d(M, N, modified, E, ret_E)
-    return ct_shepp_logan_3d(L, M, N, modified, E, ret_E, zlims)
+    elif len(N) == 3:
+        L, M, N = N[:]
+        return ct_shepp_logan_3d(L, M, N, modified, E, ret_E, zlims)
+    else:
+        raise ValueError('Dimension N must be scalar, 2D, or 3D!')
 
-def ct_shepp_logan_2d(M, N, modified, E, ret_E):
-    '''Make a 2D phantom.'''
+
+def ct_shepp_logan_2d(M: int, N: int,
+                      modified: bool,
+                      E: Optional[npt.ArrayLike],
+                      ret_E: bool) -> Union[npt.ArrayLike, Tuple[npt.ArrayLike, npt.ArrayLike]]:
+    """Make a 2D phantom."""
 
     # Get the ellipse parameters the user asked for
     if E is None:
         if modified:
             E = ct_modified_shepp_logan_params_2d()
         else:
             E = ct_shepp_logan_params_2d()
@@ -115,40 +123,45 @@
     major = E[:, 1]
     minor = E[:, 2]
     xs = E[:, 3]
     ys = E[:, 4]
     theta = E[:, 5]
 
     # 2x2 square => FOV = (-1, 1)
-    X, Y = np.meshgrid( # meshgrid needs linspace in opposite order
+    X, Y = np.meshgrid(  # meshgrid needs linspace in opposite order
         np.linspace(-1, 1, N),
         np.linspace(-1, 1, M))
     ph = np.zeros((M, N))
     ct = np.cos(theta)
     st = np.sin(theta)
 
     for ii in range(E.shape[0]):
         xc, yc = xs[ii], ys[ii]
         a, b = major[ii], minor[ii]
         ct0, st0 = ct[ii], st[ii]
 
         # Find indices falling inside the ellipse
         idx = (
-            ((X - xc)*ct0 + (Y - yc)*st0)**2/a**2 +
-            ((X - xc)*st0 - (Y - yc)*ct0)**2/b**2 <= 1)
+                ((X - xc) * ct0 + (Y - yc) * st0) ** 2 / a ** 2 +
+                ((X - xc) * st0 - (Y - yc) * ct0) ** 2 / b ** 2 <= 1)
 
         # Sum of ellipses
         ph[idx] += grey[ii]
 
     if ret_E:
-        return(ph, E)
+        return ph, E
     return ph
 
-def ct_shepp_logan_3d(L, M, N, modified, E, ret_E, zlims):
-    '''Make a 3D phantom.'''
+
+def ct_shepp_logan_3d(L: int, M: int, N: int,
+                      modified: bool,
+                      E: Optional[npt.ArrayLike],
+                      ret_E: bool,
+                      zlims: Tuple[float, float]) -> Union[npt.ArrayLike, Tuple[npt.ArrayLike, npt.ArrayLike]]:
+    """Make a 3D phantom."""
 
     # Make sure zlims are appropriate
     assert len(zlims) == 2, (
         'zlims must be a tuple with 2 entries: upper and lower '
         'bounds!')
     assert zlims[0] <= zlims[1], (
         'zlims: lower bound must be first entry!')
@@ -167,15 +180,15 @@
     zaxis = E[:, 3]
     xs = E[:, 4]
     ys = E[:, 5]
     zs = E[:, 6]
     theta = E[:, 7]
 
     # Initialize array
-    X, Y, Z = np.meshgrid( # meshgrid does X, Y backwards
+    X, Y, Z = np.meshgrid(  # meshgrid does X, Y backwards
         np.linspace(-1, 1, M),
         np.linspace(-1, 1, L),
         np.linspace(zlims[0], zlims[1], N))
     ct = np.cos(theta)
     st = np.sin(theta)
     ph = np.zeros((L, M, N))
 
@@ -184,87 +197,91 @@
         xc, yc, zc = xs[ii], ys[ii], zs[ii]
         a, b, c = xaxis[ii], yaxis[ii], zaxis[ii]
         ct0, st0 = ct[ii], st[ii]
 
         # Find indices falling inside the ellipsoid, ellipses only
         # rotated in xy plane
         idx = (
-            ((X - xc)*ct0 + (Y - yc)*st0)**2/a**2 +
-            ((X - xc)*st0 - (Y - yc)*ct0)**2/b**2 +
-            (Z - zc)**2/c**2 <= 1)
+                ((X - xc) * ct0 + (Y - yc) * st0) ** 2 / a ** 2 +
+                ((X - xc) * st0 - (Y - yc) * ct0) ** 2 / b ** 2 +
+                (Z - zc) ** 2 / c ** 2 <= 1)
 
         # Add ellipses together
         ph[idx] += gray[ii]
 
     if ret_E:
-        return(ph, E)
+        return ph, E
     return ph
 
-def ct_shepp_logan_params_2d():
-    '''Return parameters for original Shepp-Logan phantom.
+
+def ct_shepp_logan_params_2d() -> npt.ArrayLike:
+    """Return parameters for original Shepp-Logan phantom.
 
     Returns
     -------
     E : array_like, shape (10, 6)
         Parameters for the 10 ellipses used to construct the phantom.
-    '''
+    """
 
-    E = np.zeros((10, 6)) # (10, [A, a, b, xc, yc, theta])
+    E = np.zeros((10, 6))  # (10, [A, a, b, xc, yc, theta])
     E[:, 0] = [2, -.98, -.02, -.02, .01, .01, .01, .01, .01, .01]
     E[:, 1] = [
         .69, .6624, .11, .16, .21, .046, .046, .046, .023, .023]
     E[:, 2] = [.92, .874, .31, .41, .25, .046, .046, .023, .023, .046]
     E[:, 3] = [0, 0, .22, -.22, 0, 0, 0, -.08, 0, .06]
     E[:, 4] = [0, -.0184, 0, 0, .35, .1, -.1, -.605, -.605, -.605]
     E[:, 5] = np.deg2rad([0, 0, -18, 18, 0, 0, 0, 0, 0, 0])
     return E
 
-def ct_modified_shepp_logan_params_2d():
-    '''Return parameters for modified Shepp-Logan phantom.
+
+def ct_modified_shepp_logan_params_2d() -> npt.ArrayLike:
+    """Return parameters for modified Shepp-Logan phantom.
 
     Returns
     -------
     E : array_like, shape (10, 6)
         Parameters for the 10 ellipses used to construct the phantom.
-    '''
+    """
     E = ct_shepp_logan_params_2d()
     E[:, 0] = [1, -0.8, -0.2, -0.2, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
     return E
 
-def ct_shepp_logan_params_3d():
-    '''Ellipsoid parameters for 3D Shepp-Logan.
+
+def ct_shepp_logan_params_3d() -> npt.ArrayLike:
+    """Ellipsoid parameters for 3D Shepp-Logan.
 
     Returns
     -------
     E : array_like, shape (10, 8)
         Parameters for the 10 ellipsoids used to construct phantom.
-    '''
+    """
 
     E = np.zeros((10, 8))
     # [ gray, x, y, z, a, b, c, theta ]
     E[0, :] = [2, 0.69, 0.92, 0.9, 0, 0, 0, 0]
     E[1, :] = [-.8, 0.6624, 0.874, 0.88, 0, 0, 0, 0]
-    E[2, :] = [-.2, 0.41, 0.16, 0.21, -0.22, 0, -0.25, 3*np.pi/5]
-    E[3, :] = [-.2, 0.31, 0.11, 0.22, 0.22, 0, -0.25, 2*np.pi/5]
+    E[2, :] = [-.2, 0.41, 0.16, 0.21, -0.22, 0, -0.25, 3 * np.pi / 5]
+    E[3, :] = [-.2, 0.31, 0.11, 0.22, 0.22, 0, -0.25, 2 * np.pi / 5]
     E[4, :] = [.2, 0.21, 0.25, 0.5, 0, 0.35, -0.25, 0]
     E[5, :] = [.2, 0.046, 0.046, 0.046, 0, 0.1, -0.25, 0]
     E[6, :] = [.1, 0.046, 0.023, 0.02, -0.08, -0.65, -0.25, 0]
-    E[7, :] = [.1, 0.046, 0.023, 0.02, 0.06, -0.65, -0.25, np.pi/2]
-    E[8, :] = [.2, 0.056, 0.04, 0.1, 0.06, -0.105, 0.625, np.pi/2]
+    E[7, :] = [.1, 0.046, 0.023, 0.02, 0.06, -0.65, -0.25, np.pi / 2]
+    E[8, :] = [.2, 0.056, 0.04, 0.1, 0.06, -0.105, 0.625, np.pi / 2]
     E[9, :] = [-.2, 0.056, 0.056, 0.1, 0, 0.1, 0.625, 0]
     return E
 
-def ct_modified_shepp_logan_params_3d():
-    '''Return parameters for modified Shepp-Logan phantom.
+
+def ct_modified_shepp_logan_params_3d() -> npt.ArrayLike:
+    """Return parameters for modified Shepp-Logan phantom.
 
     Returns
     -------
     E : array_like, shape (10, 8)
         Parameters for the 10 ellipsoids used to construct phantom.
-    '''
+    """
     E = ct_shepp_logan_params_3d()
     E[:, 0] = [1, -0.8, -0.2, -0.2, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
     return E
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `phantominator-0.6.4/phantominator/mr_shepp_logan.py` & `phantominator-0.7.0/phantominator/mr_shepp_logan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # -*- coding: utf-8 -*-
-'''Shepp-Logan phantom for use with MR simulations.'''
+"""Shepp-Logan phantom for use with MR simulations."""
+
+from typing import Union, Optional, Tuple, Dict
 
 import numpy as np
+import numpy.typing as npt
+
 
-def mr_shepp_logan(N, E=None, B0=3, T2star=False, zlims=(-1, 1)):
-    '''Shepp-Logan phantom with MR tissue parameters.
+def mr_shepp_logan(N: Union[int, npt.ArrayLike],
+                   E: Optional[npt.ArrayLike] = None,
+                   B0: float = 3.0,
+                   T2star: bool = False,
+                   zlims: Tuple[float, float] = (-1, 1)) -> Tuple[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike]:
+    """Shepp-Logan phantom with MR tissue parameters.
 
     Parameters
     ----------
     N : int or array_like
         Matrix size, (N, N, N), or (L, M, N).
     E : array_like, optional
         ex13 numeric matrix defining e ellipses.  The columns of E
@@ -25,15 +33,15 @@
             - Parameter A for T1 determination
             - Parameter C for T1 determination
             - Explicit T1 value (in sec, or np.nan if model is used)
             - T2 value (in sec)
             - chi (change in magnetic susceptibility)
 
         If spin density is negative, M0, T1, and T2 will be subtracted
-        instead of cummulatively added.
+        instead of cumulatively added.
     B0 : float, optimal
         Field strength (in Tesla).
     T2star : bool, optional
         Use magnetic susceptibility values to return T2star values
         instead of T2. Gyromagnetic ratio is assumed to be that of
         hydrogen.
     zlims : tuple, optional
@@ -61,15 +69,15 @@
 
     References
     ----------
     .. [1] Gach, H. Michael, Costin Tanase, and Fernando Boada.
            "2D & 3D Shepp-Logan phantom standards for MRI." 2008 19th
            International Conference on Systems Engineering. IEEE,
            2008.
-    '''
+    """
 
     # Determine size of phantom
     if np.isscalar(N):
         L, M, N = N, N, N
     else:
         L, M, N = N[:]
 
@@ -96,30 +104,25 @@
     As = E[:, 8]
     Cs = E[:, 9]
     T1 = E[:, 10]
     T2 = E[:, 11]
     chis = E[:, 12]
 
     # Initialize array
-    X, Y, Z = np.meshgrid( # meshgrid does X, Y backwards
+    X, Y, Z = np.meshgrid(  # meshgrid does X, Y backwards
         np.linspace(-1, 1, M),
         np.linspace(-1, 1, L),
         np.linspace(zlims[0], zlims[1], N))
     ct = np.cos(theta)
     st = np.sin(theta)
     sgn = np.sign(M0)
     T1s = np.zeros((L, M, N))
     T2s = np.zeros((L, M, N))
     M0s = np.zeros((L, M, N))
 
-    # We'll need the gyromagnetic ratio if returning T2star values
-    if T2star:
-        # see https://en.wikipedia.org/wiki/Gyromagnetic_ratio:
-        gamma0 = 267.52219 # 10^6 rad⋅s−1⋅T⋅−1
-
     # Put ellipses where they need to be
     for ii in range(E.shape[0]):
         xc, yc, zc = xs[ii], ys[ii], zs[ii]
         a, b, c = xaxis[ii], yaxis[ii], zaxis[ii]
         ct0, st0 = ct[ii], st[ii]
 
         # Find indices falling inside the ellipsoid, ellipses only
@@ -130,36 +133,39 @@
             (Z - zc)**2/c**2 <= 1)
 
         # Add ellipses together -- subtract of M0 is negative
         M0s[idx] += M0[ii]
 
         # Use T2star values if user asked for them
         if T2star:
+            # We'll need the gyromagnetic ratio if returning T2star values
+            # see https://en.wikipedia.org/wiki/Gyromagnetic_ratio:
+            gamma0 = 267.52219  # 10^6 rad⋅s−1⋅T⋅−1
             T2s[idx] += sgn[ii]/(1/T2[ii] + gamma0*np.abs(
                 B0*chis[ii]))
         else:
             T2s[idx] += sgn[ii]*T2[ii]
 
         # Use T1 model if not given explicit T1 value
         if np.isnan(T1[ii]):
             T1s[idx] += sgn[ii]*As[ii]*(B0**Cs[ii])
         else:
             T1s[idx] += sgn[ii]*T1[ii]
 
-    return(M0s, T1s, T2s)
+    return M0s, T1s, T2s
 
 
-def mr_ellipsoid_parameters():
-    '''Returns parameters of ellipsoids.
+def mr_ellipsoid_parameters() -> npt.ArrayLike:
+    """Returns parameters of ellipsoids.
 
     Returns
     -------
     E : array_like
         Parameters for the ellipsoids used to construct the phantom.
-    '''
+    """
     params = _mr_relaxation_parameters()
 
     E = np.zeros((15, 13))
     # [:, [x, y, z, a, b, c, theta, m0, A, C, (t1), t2, chi]]
     E[0, :] = [
         0, 0, 0, .72, .95, .93, 0, .8,
         *params['scalp']]
@@ -230,27 +236,28 @@
     Eneg = Eneg[:-1, :]
 
     # Put both ellipsoid groups together
     E = np.concatenate((E, Eneg), axis=0)
 
     return E
 
-def _mr_relaxation_parameters():
-    '''Returns MR relaxation parameters for certain tissues.
+
+def _mr_relaxation_parameters() -> Dict[str, npt.ArrayLike]:
+    """Returns MR relaxation parameters for certain tissues.
 
     Returns
     -------
     params : dict
         Gives entries as [A, C, (t1), t2, chi]
 
     Notes
     -----
     If t1 is None, the model T1 = A*B0^C will be used.  If t1 is not
     np.nan, then specified t1 will be used.
-    '''
+    """
 
     # params['tissue-name'] = [A, C, (t1 value if explicit), t2, chi]
     params = dict()
     params['scalp'] = [.324, .137, np.nan, .07, -7.5e-6]
     params['marrow'] = [.533, .088, np.nan, .05, -8.85e-6]
     params['csf'] = [np.nan, np.nan, 4.2, 1.99, -9e-6]
     params['blood-clot'] = [1.35, .34, np.nan, .2, -9e-6]
```

### Comparing `phantominator-0.6.4/README.rst` & `phantominator-0.7.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 Installation
 ============
 
 .. code-block:: bash
 
-    pip install phantominator
+    python -m pip install phantominator
 
 The goal is to have easy installation and usage for everyone.  If
 something doesn't work, please open an issue and/or submit a pull
 request.  We'll get it figured out.
 
+`pygrappa` is an optional dependency required to run the
+`phantominator.examples.radial_coil_sens` example.
+
 About
 =====
 
 Python package for easy generation of numerical phantoms.  I often
 need a simple image to try something out on.  In MATLAB, I would use
 the `phantom` command to quickly get something to work with.  In
-Python, it's not quite so easy, so I made this package that's quick
+Python, it's not always quite so easy, so I made this package that's quick
 to install and use so there's as little friction as possible.  There
 are other implementations of Shepp-Logan available from other
 projects, but they are usually not as easy to install or include other
 things that I don't want for this project.
 
 This package offers both CT and MR versions.
 
-Going forward, this module will no longer support Python 2.  Please do
-the world a favor and move on to Python 3.
+Going forward, this module will support Python >= 3.8.
 
 Usage
 =====
 
 Also see the `examples` module and docstrings.  The interface for CT
 phantom generation is similar to MATLAB's `phantom` function.
 
+Examples can be run as:
+
+.. code-block:: bash
+
+    # python -m phantominator.examples.[example-name], e.g.:
+    python -m phantominator.examples.shepp_logan
+
 Basic usage:
 
 .. code-block:: python
 
     # CT phantom
     from phantominator import shepp_logan
     ph = shepp_logan(128)
```

