# Comparing `tmp/weac-2.3.1.tar.gz` & `tmp/weac-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weac-2.3.1.tar", last modified: Fri Aug  5 17:59:58 2022, max compression
+gzip compressed data, was "weac-2.3.2.tar", last modified: Mon Apr 17 09:55:35 2023, max compression
```

## Comparing `weac-2.3.1.tar` & `weac-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-05 17:59:58.494453 weac-2.3.1/
--rw-r--r--   0 runner     (501) staff       (20)     1522 2022-08-05 17:59:34.000000 weac-2.3.1/CITATION.cff
--rw-r--r--   0 runner     (501) staff       (20)      129 2022-08-05 17:59:34.000000 weac-2.3.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       39 2022-08-05 17:59:34.000000 weac-2.3.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    16107 2022-08-05 17:59:58.494750 weac-2.3.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    15395 2022-08-05 17:59:34.000000 weac-2.3.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-05 17:59:58.482339 weac-2.3.1/build/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-05 17:59:58.494100 weac-2.3.1/build/weac.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      266 2022-08-05 17:59:58.000000 weac-2.3.1/build/weac.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-05 17:59:58.489525 weac-2.3.1/img/
--rw-r--r--   0 runner     (501) staff       (20)    70202 2022-08-05 17:59:34.000000 weac-2.3.1/img/bc.png
--rw-r--r--   0 runner     (501) staff       (20)    17056 2022-08-05 17:59:34.000000 weac-2.3.1/img/layering.png
--rw-r--r--   0 runner     (501) staff       (20)    82279 2022-08-05 17:59:34.000000 weac-2.3.1/img/logo.png
--rw-r--r--   0 runner     (501) staff       (20)    37795 2022-08-05 17:59:34.000000 weac-2.3.1/img/model.png
--rw-r--r--   0 runner     (501) staff       (20)    69175 2022-08-05 17:59:34.000000 weac-2.3.1/img/profiles.png
--rw-r--r--   0 runner     (501) staff       (20)    30453 2022-08-05 17:59:34.000000 weac-2.3.1/img/systems.png
--rw-r--r--   0 runner     (501) staff       (20)       90 2022-08-05 17:59:34.000000 weac-2.3.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      988 2022-08-05 17:59:58.495724 weac-2.3.1/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-05 17:59:58.493654 weac-2.3.1/weac/
--rw-r--r--   0 runner     (501) staff       (20)      359 2022-08-05 17:59:34.000000 weac-2.3.1/weac/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    26878 2022-08-05 17:59:34.000000 weac-2.3.1/weac/eigensystem.py
--rw-r--r--   0 runner     (501) staff       (20)     1980 2022-08-05 17:59:34.000000 weac-2.3.1/weac/inverse.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1770 2022-08-05 17:59:34.000000 weac-2.3.1/weac/layered.py
--rw-r--r--   0 runner     (501) staff       (20)    53733 2022-08-05 17:59:34.000000 weac-2.3.1/weac/mixins.py
--rw-r--r--   0 runner     (501) staff       (20)    20502 2022-08-05 17:59:34.000000 weac-2.3.1/weac/plot.py
--rw-r--r--   0 runner     (501) staff       (20)     4636 2022-08-05 17:59:34.000000 weac-2.3.1/weac/tools.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 09:55:35.305057 weac-2.3.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1440 2023-04-17 09:55:08.000000 weac-2.3.2/CITATION.cff
+-rw-r--r--   0 runner     (501) staff       (20)      129 2023-04-17 09:55:08.000000 weac-2.3.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       39 2023-04-17 09:55:08.000000 weac-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    16651 2023-04-17 09:55:35.305353 weac-2.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    15939 2023-04-17 09:55:08.000000 weac-2.3.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 09:55:35.289532 weac-2.3.2/build/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 09:55:35.304705 weac-2.3.2/build/weac.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      266 2023-04-17 09:55:35.000000 weac-2.3.2/build/weac.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 09:55:35.300129 weac-2.3.2/img/
+-rw-r--r--   0 runner     (501) staff       (20)    70202 2023-04-17 09:55:08.000000 weac-2.3.2/img/bc.png
+-rw-r--r--   0 runner     (501) staff       (20)    17056 2023-04-17 09:55:08.000000 weac-2.3.2/img/layering.png
+-rw-r--r--   0 runner     (501) staff       (20)    82279 2023-04-17 09:55:08.000000 weac-2.3.2/img/logo.png
+-rw-r--r--   0 runner     (501) staff       (20)    37795 2023-04-17 09:55:08.000000 weac-2.3.2/img/model.png
+-rw-r--r--   0 runner     (501) staff       (20)    69175 2023-04-17 09:55:08.000000 weac-2.3.2/img/profiles.png
+-rw-r--r--   0 runner     (501) staff       (20)    30453 2023-04-17 09:55:08.000000 weac-2.3.2/img/systems.png
+-rw-r--r--   0 runner     (501) staff       (20)       90 2023-04-17 09:55:08.000000 weac-2.3.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-17 09:55:35.306736 weac-2.3.2/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 09:55:35.304116 weac-2.3.2/weac/
+-rw-r--r--   0 runner     (501) staff       (20)      359 2023-04-17 09:55:08.000000 weac-2.3.2/weac/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    26881 2023-04-17 09:55:08.000000 weac-2.3.2/weac/eigensystem.py
+-rw-r--r--   0 runner     (501) staff       (20)     1980 2023-04-17 09:55:08.000000 weac-2.3.2/weac/inverse.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1770 2023-04-17 09:55:08.000000 weac-2.3.2/weac/layered.py
+-rw-r--r--   0 runner     (501) staff       (20)    53733 2023-04-17 09:55:08.000000 weac-2.3.2/weac/mixins.py
+-rw-r--r--   0 runner     (501) staff       (20)    20502 2023-04-17 09:55:08.000000 weac-2.3.2/weac/plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     5338 2023-04-17 09:55:08.000000 weac-2.3.2/weac/tools.py
```

### Comparing `weac-2.3.1/PKG-INFO` & `weac-2.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weac
-Version: 2.3.1
+Version: 2.3.2
 Summary: Weak layer anticrack nucleation model
 Home-page: https://github.com/2phi/weac
 Author: 2phi GbR
 Author-email: mail@2phi.de
 License: Proprietary
 Project-URL: Demo, https://github.com/2phi/weac/blob/main/demo/demo.ipynb
 Project-URL: Documentation, https://2phi.github.io/weac
@@ -95,24 +95,33 @@
 8. [Contact](#contact)
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About the project
 
-WEAC implements closed-form analytical models for the [mechanical analysis of dry-snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020), the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020), and, in particular, allows for the analysis of stratified snow covers. The model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-loaded buried weak layers.
+WEAC implements closed-form analytical models for the [mechanical analysis of dry-snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020), the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020), and, in particular, allows for the [analysis of stratified snow covers](https://doi.org/10.5194/tc-17-1475-2023). The model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-loaded buried weak layers.
 
 <img src="https://github.com/2phi/weac/raw/main/img/systems.png" alt="Systems" width="500"/>
 
-Please refer to the companion papers for model derivations, illustrations, dimensions, material properties, and kinematics:
+Cite the repository as:
+```
+Rosendahl, P. L. & Weissgraeber, P. (2022). Weak Layer Anticrack Nucleation Model (WEAC). Zenodo. https://doi.org/10.5281/zenodo.5773113
+```
+
+Read the [📄 white paper](https://doi.org/10.5194/tc-17-1475-2023) for model derivations, illustrations, dimensions, material properties, and kinematics:
+
+- Weißgraeber, P. & Rosendahl, P. L. (2023). A closed-form model for layered snow slabs. The Cryosphere, 17(4), 1475–1496. https://doi.org/10.5194/tc-17-1475-2023
+
+For more background info, please refer to the companion papers:
 
-- Rosendahl, P. L., & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 1: Slabs on compliant and collapsible weak layers. The Cryosphere, 14(1), 115–130. https://doi.org/10.5194/tc-14-115-2020
-- Rosendahl, P. L., & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 2: Coupled mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1), 131–145. https://doi.org/10.5194/tc-14-131-2020
+- Rosendahl, P. L. & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 1: Slabs on compliant and collapsible weak layers. The Cryosphere, 14(1), 115–130. https://doi.org/10.5194/tc-14-115-2020
+- Rosendahl, P. L. & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 2: Coupled mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1), 131–145. https://doi.org/10.5194/tc-14-131-2020
 
-Written in [🐍 Python](https://www.python.org) and built with [<span style="color:#498B60">⚛</span> Atom](https://atom.io), [🐙 GitKraken](https://www.gitkraken.com), and [🪐 Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was written and built in [🌋 MATLAB](https://www.mathworks.com/products/matlab.html). 
+Written in [🐍 Python](https://www.python.org) and built with [💻 Visual Studio Code](https://code.visualstudio.com), [🐙 GitKraken](https://www.gitkraken.com), and [🪐 Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was written and built in [🌋 MATLAB](https://www.mathworks.com/products/matlab.html).
 
 <!-- 
 [![Python](https://img.shields.io/badge/Python-306998.svg?style=flat-square&logo=python&logoColor=white&label&labelColor=gray)](https://www.python.org)
 [![Jupyter](https://img.shields.io/badge/Jupyter-e67124.svg?style=flat-square&logo=jupyter&logoColor=white&label&labelColor=gray)](https://jupyter.org)
 [![Atom](https://img.shields.io/badge/Atom-498b60.svg?style=flat-square&logo=atom&logoColor=white&label&labelColor=gray)](https://atom.io)
 [![GitKraken](https://img.shields.io/badge/GitKraken-179287.svg?style=flat-square&logo=gitkraken&logoColor=white&label&labelColor=gray)](https://www.gitkraken.com) -->
 
@@ -128,14 +137,15 @@
 or clone the repo
 ```sh
 git clone https://github.com/2phi/weac
 ```
 for local use.
 
 Needs
+- [Python](https://www.python.org/downloads/release/python-3100/) &ge; 3.10
 - [Numpy](https://numpy.org/) for matrix operations
 - [Scipy](https://www.scipy.org/) for solving optimization problems
 - [Pandas](https://pandas.pydata.org/) for data handling
 - [Matplotlib](https://matplotlib.org/) for plotting
 
 <!-- USAGE EXAMPLES -->
 ## Usage
@@ -256,15 +266,15 @@
 4. Push to the branch (`git push origin feature/amazingfeature`)
 5. Open a pull request
 
 
 <!-- LICENSE -->
 ## License
 
-Copyright 2phi GbR, 2020-2022.
+Copyright 2phi GbR, 2020-2023.
 
 We currently do not offer an open source license. Please contact us for private licensing options.
 
 
 <!-- CONTACT -->
 ## Contact
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: weac Version: 2.3.1 Summary: Weak layer anticrack
+Metadata-Version: 2.1 Name: weac Version: 2.3.2 Summary: Weak layer anticrack
 nucleation model Home-page: https://github.com/2phi/weac Author: 2phi GbR
 Author-email: mail@2phi.de License: Proprietary Project-URL: Demo, https://
 github.com/2phi/weac/blob/main/demo/demo.ipynb Project-URL: Documentation,
 https://2phi.github.io/weac Project-URL: Issues and feature requests, https://
 github.com/2phi/weac/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Scientific/Engineering Requires-Python:
@@ -24,103 +24,111 @@
                     ## Contents 1. [About the project](#about-the-project) 2.
 [Installation](#installation) 3. [Usage](#usage) 4. [Roadmap](#roadmap) 5.
 [Release history](#release-history) 6. [How to contribute](#how-to-contribute)
 7. [License](#license) 8. [Contact](#contact)  ## About the project WEAC
 implements closed-form analytical models for the [mechanical analysis of dry-
 snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020),
 the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020),
-and, in particular, allows for the analysis of stratified snow covers. The
-model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-
-loaded buried weak layers. [Systems] Please refer to the companion papers for
-model derivations, illustrations, dimensions, material properties, and
-kinematics: - Rosendahl, P. L., & WeiÃgraeber, P. (2020). Modeling snow slab
-avalanches caused by weak-layer failure â Part 1: Slabs on compliant and
-collapsible weak layers. The Cryosphere, 14(1), 115â130. https://doi.org/
-10.5194/tc-14-115-2020 - Rosendahl, P. L., & WeiÃgraeber, P. (2020). Modeling
-snow slab avalanches caused by weak-layer failure â Part 2: Coupled mixed-
-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1),
+and, in particular, allows for the [analysis of stratified snow covers](https:/
+/doi.org/10.5194/tc-17-1475-2023). The model covers propagation saw tests (a),
+and uncracked (b) or cracked (c) skier-loaded buried weak layers. [Systems]
+Cite the repository as: ``` Rosendahl, P. L. & Weissgraeber, P. (2022). Weak
+Layer Anticrack Nucleation Model (WEAC). Zenodo. https://doi.org/10.5281/
+zenodo.5773113 ``` Read the [ð white paper](https://doi.org/10.5194/tc-17-
+1475-2023) for model derivations, illustrations, dimensions, material
+properties, and kinematics: - WeiÃgraeber, P. & Rosendahl, P. L. (2023). A
+closed-form model for layered snow slabs. The Cryosphere, 17(4), 1475â1496.
+https://doi.org/10.5194/tc-17-1475-2023 For more background info, please refer
+to the companion papers: - Rosendahl, P. L. & WeiÃgraeber, P. (2020). Modeling
+snow slab avalanches caused by weak-layer failure â Part 1: Slabs on
+compliant and collapsible weak layers. The Cryosphere, 14(1), 115â130. https:
+//doi.org/10.5194/tc-14-115-2020 - Rosendahl, P. L. & WeiÃgraeber, P. (2020).
+Modeling snow slab avalanches caused by weak-layer failure â Part 2: Coupled
+mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1),
 131â145. https://doi.org/10.5194/tc-14-131-2020 Written in [ð Python]
-(https://www.python.org) and built with [â Atom](https://atom.io), [ð
-GitKraken](https://www.gitkraken.com), and [ðª Jupyter](https://jupyter.org).
-Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was
-written and built in [ð MATLAB](https://www.mathworks.com/products/
-matlab.html).   ## Installation Install globally using the `pip` Package
-Installer for Python ```sh pip install -U weac ``` or clone the repo ```sh git
-clone https://github.com/2phi/weac ``` for local use. Needs - [Numpy](https://
-numpy.org/) for matrix operations - [Scipy](https://www.scipy.org/) for solving
-optimization problems - [Pandas](https://pandas.pydata.org/) for data handling
-- [Matplotlib](https://matplotlib.org/) for plotting  ## Usage The following
-describes the basic usage of WEAC. Please refer to the [demo](https://
-github.com/2phi/weac/blob/main/demo/demo.ipynb) for more examples and read the
-[documentation](https://2phi.github.io/weac/) for details. Load the module.
-```python import weac ``` Choose a snow profile from the database (see [demo]
-(https://github.com/2phi/weac/blob/main/demo/demo.ipynb)) or create your own as
-a 2D array where the columns are density (kg/m^2) and layer thickness (mm). One
-row corresponds to one layer counted from top (below surface) to bottom (above
-weak layer). ```python myprofile = [[170, 100], # (1) surface layer [190, 40],
-# (2) [230, 130], # : [250, 20], # : [210, 70], # (i) [380, 20], # : [280,
-100]] # (N) last slab layer above weak layer ``` Create a model instance with
-optional custom layering. ```python skier = weac.Layered(system='skier',
-layers=myprofile) ``` Calculate lists of segment lengths, locations of
-foundations, and position and magnitude of skier loads from the inputs total
-length `L` (mm), crack length `a` (mm), and skier weight `m` (kg). We can
-choose to analyze the situtation before a crack appears even if a crack length
-> 0 is set by replacing the `'crack'` key thorugh the `'nocrack'` key.
-```python segments = skier.calc_segments(L=10000, a=300, m=80)['crack'] ```
-Assemble the system of linear equations and solve the boundary-value problem
-for the free constants `C` providing the inclination `phi` (counterclockwise
-positive) in degrees. ```python C = skier.assemble_and_solve(phi=38,
-**segments) ``` Prepare the output by rasterizing the solution vector at all
-horizontal positions `xsl` (slab). The result is returned in the form of the
-ndarray `z`. We also get `xwl` (weak layer) that only contains x-coordinates
-that are supported by a foundation. ```python xsl, z, xwl =
-skier.rasterize_solution(C=C, phi=38, **segments) ``` Visualize the results.
-```python # Visualize deformations as a contour plot weac.plot.deformed(skier,
-xsl=xsl_skier, xwl=xwl_skier, z=z_skier, phi=inclination, window=200,
-scale=200, field='principal') # Plot slab displacements (using x-coordinates of
-all segments, xsl) weac.plot.displacements(skier, x=xsl, z=z, **segments) #
-Plot weak-layer stresses (using only x-coordinates of bedded segments, xwl)
-weac.plot.stresses(skier, x=xwl, z=z, **segments) ``` Compute output quantities
-for exporting or plotting. ```python # Slab deflections (using x-coordinates of
-all segments, xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z,
-unit='um') # Weak-layer shear stress (using only x-coordinates of bedded
-segments, xwl) x_cm, tau_kPa = skier.get_weaklayer_shearstress(x=xwl, z=z,
-unit='kPa') ```  ## Roadmap See the [open issues](https://github.com/2phi/weac/
-issues) for a list of proposed features and known issues. ### v2.5 - [ ] Finite
-fracture mechanics implementation for layered snow covers ### v2.4 - [ ]
-Implement anistropic weak layer - [ ] Add demo gif ## Release history ### v2.3
-- Stress plots on deformed contours - PSTs now account for slab touchdown ###
-v2.2 - Sign of inclination `phi` consistent with the coordinate system
-(positive counterclockwise) - Dimension arguments to field-quantity methods
-added - Improved aspect ratio of profile views and contour plots - Improved
-plot labels - Convenience methods for the export of weak-layer stresses and
-slab deformations provided - Wrapper for (re)calculation of the fundamental
-system added - Now allows for distributed surface loads ### v2.1 - Consistent
-use of coordinate system with downward pointing z-axis - Consitent top-to-
-bottom numbering of slab layers - Implementation of PSTs cut from either left
-or right side ### v2.0 - Completely rewritten in ð Python - Coupled bending-
-extension ODE solver implemented - Stress analysis of arbitrarily layered snow
-slabs - FEM validation of - displacements - weak-layer stresses - energy
-release rates in weak layers - Documentation - Demo and examples ### v1.0 -
-Written in ð MATLAB - Deformation analysis of homogeneous snow labs - Weak-
-layer stress prediction - Energy release rates of cracks in weak layers -
-Finite fracture mechanics implementation - Prediction of anticrack nucleation
-## How to contribute 1. Fork the project 2. Create your feature branch (`git
-checkout -b feature/amazingfeature`) 3. Commit your changes (`git commit -
-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin feature/
-amazingfeature`) 5. Open a pull request  ## License Copyright 2phi GbR, 2020-
-2022. We currently do not offer an open source license. Please contact us for
-private licensing options.  ## Contact E-mail: mail@2phi.de Â· Web: https://
-2phi.de Â· Project Link: [https://github.com/2phi/weac](https://github.com/
-2phi/weac) Â· Project DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://
-dx.doi.org/10.5281/zenodo.5773113)   [contributors-badge]: https://
-img.shields.io/github/contributors/2phi/weac.svg?style=flat-
-square&logo=github&color=yellow [forks-badge]: https://img.shields.io/github/
-forks/2phi/weac.svg?&color=blueviolet&style=flat-square&logo=github [stars-
-badge]: https://img.shields.io/github/stars/2phi/weac.svg?style=flat-
+(https://www.python.org) and built with [ð» Visual Studio Code](https://
+code.visualstudio.com), [ð GitKraken](https://www.gitkraken.com), and [ðª
+Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/
+2phi/weac/releases/tag/v1.0.0) was written and built in [ð MATLAB](https://
+www.mathworks.com/products/matlab.html).   ## Installation Install globally
+using the `pip` Package Installer for Python ```sh pip install -U weac ``` or
+clone the repo ```sh git clone https://github.com/2phi/weac ``` for local use.
+Needs - [Python](https://www.python.org/downloads/release/python-3100/) ≥ 3.10
+- [Numpy](https://numpy.org/) for matrix operations - [Scipy](https://
+www.scipy.org/) for solving optimization problems - [Pandas](https://
+pandas.pydata.org/) for data handling - [Matplotlib](https://matplotlib.org/
+) for plotting  ## Usage The following describes the basic usage of WEAC.
+Please refer to the [demo](https://github.com/2phi/weac/blob/main/demo/
+demo.ipynb) for more examples and read the [documentation](https://
+2phi.github.io/weac/) for details. Load the module. ```python import weac ```
+Choose a snow profile from the database (see [demo](https://github.com/2phi/
+weac/blob/main/demo/demo.ipynb)) or create your own as a 2D array where the
+columns are density (kg/m^2) and layer thickness (mm). One row corresponds to
+one layer counted from top (below surface) to bottom (above weak layer).
+```python myprofile = [[170, 100], # (1) surface layer [190, 40], # (2) [230,
+130], # : [250, 20], # : [210, 70], # (i) [380, 20], # : [280, 100]] # (N) last
+slab layer above weak layer ``` Create a model instance with optional custom
+layering. ```python skier = weac.Layered(system='skier', layers=myprofile) ```
+Calculate lists of segment lengths, locations of foundations, and position and
+magnitude of skier loads from the inputs total length `L` (mm), crack length
+`a` (mm), and skier weight `m` (kg). We can choose to analyze the situtation
+before a crack appears even if a crack length > 0 is set by replacing the
+`'crack'` key thorugh the `'nocrack'` key. ```python segments =
+skier.calc_segments(L=10000, a=300, m=80)['crack'] ``` Assemble the system of
+linear equations and solve the boundary-value problem for the free constants
+`C` providing the inclination `phi` (counterclockwise positive) in degrees.
+```python C = skier.assemble_and_solve(phi=38, **segments) ``` Prepare the
+output by rasterizing the solution vector at all horizontal positions `xsl`
+(slab). The result is returned in the form of the ndarray `z`. We also get
+`xwl` (weak layer) that only contains x-coordinates that are supported by a
+foundation. ```python xsl, z, xwl = skier.rasterize_solution(C=C, phi=38,
+**segments) ``` Visualize the results. ```python # Visualize deformations as a
+contour plot weac.plot.deformed(skier, xsl=xsl_skier, xwl=xwl_skier, z=z_skier,
+phi=inclination, window=200, scale=200, field='principal') # Plot slab
+displacements (using x-coordinates of all segments, xsl)
+weac.plot.displacements(skier, x=xsl, z=z, **segments) # Plot weak-layer
+stresses (using only x-coordinates of bedded segments, xwl) weac.plot.stresses
+(skier, x=xwl, z=z, **segments) ``` Compute output quantities for exporting or
+plotting. ```python # Slab deflections (using x-coordinates of all segments,
+xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z, unit='um') # Weak-layer
+shear stress (using only x-coordinates of bedded segments, xwl) x_cm, tau_kPa =
+skier.get_weaklayer_shearstress(x=xwl, z=z, unit='kPa') ```  ## Roadmap See the
+[open issues](https://github.com/2phi/weac/issues) for a list of proposed
+features and known issues. ### v2.5 - [ ] Finite fracture mechanics
+implementation for layered snow covers ### v2.4 - [ ] Implement anistropic weak
+layer - [ ] Add demo gif ## Release history ### v2.3 - Stress plots on deformed
+contours - PSTs now account for slab touchdown ### v2.2 - Sign of inclination
+`phi` consistent with the coordinate system (positive counterclockwise) -
+Dimension arguments to field-quantity methods added - Improved aspect ratio of
+profile views and contour plots - Improved plot labels - Convenience methods
+for the export of weak-layer stresses and slab deformations provided - Wrapper
+for (re)calculation of the fundamental system added - Now allows for
+distributed surface loads ### v2.1 - Consistent use of coordinate system with
+downward pointing z-axis - Consitent top-to-bottom numbering of slab layers -
+Implementation of PSTs cut from either left or right side ### v2.0 - Completely
+rewritten in ð Python - Coupled bending-extension ODE solver implemented -
+Stress analysis of arbitrarily layered snow slabs - FEM validation of -
+displacements - weak-layer stresses - energy release rates in weak layers -
+Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
+Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
+Energy release rates of cracks in weak layers - Finite fracture mechanics
+implementation - Prediction of anticrack nucleation  ## How to contribute 1.
+Fork the project 2. Create your feature branch (`git checkout -b feature/
+amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
+feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
+Open a pull request  ## License Copyright 2phi GbR, 2020-2023. We currently do
+not offer an open source license. Please contact us for private licensing
+options.  ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
+Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
+DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
+zenodo.5773113)   [contributors-badge]: https://img.shields.io/github/
+contributors/2phi/weac.svg?style=flat-square&logo=github&color=yellow [forks-
+badge]: https://img.shields.io/github/forks/2phi/
+weac.svg?&color=blueviolet&style=flat-square&logo=github [stars-badge]: https:/
+/img.shields.io/github/stars/2phi/weac.svg?style=flat-
 square&logo=github&color=orange [issues-badge]: https://img.shields.io/github/
 issues/2phi/weac.svg?style=flat-square&logo=github [pypi-badge]: https://
 img.shields.io/pypi/v/
 weac.svg?logo=python&logoColor=white&color=f46b58&style=flat-square [pypi-
 downloads-badge]: https://img.shields.io/pypi/dm/
 weac.svg?logo=python&logoColor=white&color=red&style=flat-square [python-dist-
 badge]: https://img.shields.io/pypi/pyversions/weac.svg?style=flat-
```

### Comparing `weac-2.3.1/README.md` & `weac-2.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,24 +75,33 @@
 8. [Contact](#contact)
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About the project
 
-WEAC implements closed-form analytical models for the [mechanical analysis of dry-snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020), the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020), and, in particular, allows for the analysis of stratified snow covers. The model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-loaded buried weak layers.
+WEAC implements closed-form analytical models for the [mechanical analysis of dry-snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020), the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020), and, in particular, allows for the [analysis of stratified snow covers](https://doi.org/10.5194/tc-17-1475-2023). The model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-loaded buried weak layers.
 
 <img src="https://github.com/2phi/weac/raw/main/img/systems.png" alt="Systems" width="500"/>
 
-Please refer to the companion papers for model derivations, illustrations, dimensions, material properties, and kinematics:
+Cite the repository as:
+```
+Rosendahl, P. L. & Weissgraeber, P. (2022). Weak Layer Anticrack Nucleation Model (WEAC). Zenodo. https://doi.org/10.5281/zenodo.5773113
+```
+
+Read the [📄 white paper](https://doi.org/10.5194/tc-17-1475-2023) for model derivations, illustrations, dimensions, material properties, and kinematics:
+
+- Weißgraeber, P. & Rosendahl, P. L. (2023). A closed-form model for layered snow slabs. The Cryosphere, 17(4), 1475–1496. https://doi.org/10.5194/tc-17-1475-2023
+
+For more background info, please refer to the companion papers:
 
-- Rosendahl, P. L., & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 1: Slabs on compliant and collapsible weak layers. The Cryosphere, 14(1), 115–130. https://doi.org/10.5194/tc-14-115-2020
-- Rosendahl, P. L., & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 2: Coupled mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1), 131–145. https://doi.org/10.5194/tc-14-131-2020
+- Rosendahl, P. L. & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 1: Slabs on compliant and collapsible weak layers. The Cryosphere, 14(1), 115–130. https://doi.org/10.5194/tc-14-115-2020
+- Rosendahl, P. L. & Weißgraeber, P. (2020). Modeling snow slab avalanches caused by weak-layer failure – Part 2: Coupled mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1), 131–145. https://doi.org/10.5194/tc-14-131-2020
 
-Written in [🐍 Python](https://www.python.org) and built with [<span style="color:#498B60">⚛</span> Atom](https://atom.io), [🐙 GitKraken](https://www.gitkraken.com), and [🪐 Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was written and built in [🌋 MATLAB](https://www.mathworks.com/products/matlab.html). 
+Written in [🐍 Python](https://www.python.org) and built with [💻 Visual Studio Code](https://code.visualstudio.com), [🐙 GitKraken](https://www.gitkraken.com), and [🪐 Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was written and built in [🌋 MATLAB](https://www.mathworks.com/products/matlab.html).
 
 <!-- 
 [![Python](https://img.shields.io/badge/Python-306998.svg?style=flat-square&logo=python&logoColor=white&label&labelColor=gray)](https://www.python.org)
 [![Jupyter](https://img.shields.io/badge/Jupyter-e67124.svg?style=flat-square&logo=jupyter&logoColor=white&label&labelColor=gray)](https://jupyter.org)
 [![Atom](https://img.shields.io/badge/Atom-498b60.svg?style=flat-square&logo=atom&logoColor=white&label&labelColor=gray)](https://atom.io)
 [![GitKraken](https://img.shields.io/badge/GitKraken-179287.svg?style=flat-square&logo=gitkraken&logoColor=white&label&labelColor=gray)](https://www.gitkraken.com) -->
 
@@ -108,14 +117,15 @@
 or clone the repo
 ```sh
 git clone https://github.com/2phi/weac
 ```
 for local use.
 
 Needs
+- [Python](https://www.python.org/downloads/release/python-3100/) &ge; 3.10
 - [Numpy](https://numpy.org/) for matrix operations
 - [Scipy](https://www.scipy.org/) for solving optimization problems
 - [Pandas](https://pandas.pydata.org/) for data handling
 - [Matplotlib](https://matplotlib.org/) for plotting
 
 <!-- USAGE EXAMPLES -->
 ## Usage
@@ -236,15 +246,15 @@
 4. Push to the branch (`git push origin feature/amazingfeature`)
 5. Open a pull request
 
 
 <!-- LICENSE -->
 ## License
 
-Copyright 2phi GbR, 2020-2022.
+Copyright 2phi GbR, 2020-2023.
 
 We currently do not offer an open source license. Please contact us for private licensing options.
 
 
 <!-- CONTACT -->
 ## Contact
```

#### html2text {}

```diff
@@ -15,103 +15,111 @@
                     ## Contents 1. [About the project](#about-the-project) 2.
 [Installation](#installation) 3. [Usage](#usage) 4. [Roadmap](#roadmap) 5.
 [Release history](#release-history) 6. [How to contribute](#how-to-contribute)
 7. [License](#license) 8. [Contact](#contact)  ## About the project WEAC
 implements closed-form analytical models for the [mechanical analysis of dry-
 snow slabs on compliant weak layers](https://doi.org/10.5194/tc-14-115-2020),
 the [prediction of anticrack onset](https://doi.org/10.5194/tc-14-131-2020),
-and, in particular, allows for the analysis of stratified snow covers. The
-model covers propagation saw tests (a), and uncracked (b) or cracked (c) skier-
-loaded buried weak layers. [Systems] Please refer to the companion papers for
-model derivations, illustrations, dimensions, material properties, and
-kinematics: - Rosendahl, P. L., & WeiÃgraeber, P. (2020). Modeling snow slab
-avalanches caused by weak-layer failure â Part 1: Slabs on compliant and
-collapsible weak layers. The Cryosphere, 14(1), 115â130. https://doi.org/
-10.5194/tc-14-115-2020 - Rosendahl, P. L., & WeiÃgraeber, P. (2020). Modeling
-snow slab avalanches caused by weak-layer failure â Part 2: Coupled mixed-
-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1),
+and, in particular, allows for the [analysis of stratified snow covers](https:/
+/doi.org/10.5194/tc-17-1475-2023). The model covers propagation saw tests (a),
+and uncracked (b) or cracked (c) skier-loaded buried weak layers. [Systems]
+Cite the repository as: ``` Rosendahl, P. L. & Weissgraeber, P. (2022). Weak
+Layer Anticrack Nucleation Model (WEAC). Zenodo. https://doi.org/10.5281/
+zenodo.5773113 ``` Read the [ð white paper](https://doi.org/10.5194/tc-17-
+1475-2023) for model derivations, illustrations, dimensions, material
+properties, and kinematics: - WeiÃgraeber, P. & Rosendahl, P. L. (2023). A
+closed-form model for layered snow slabs. The Cryosphere, 17(4), 1475â1496.
+https://doi.org/10.5194/tc-17-1475-2023 For more background info, please refer
+to the companion papers: - Rosendahl, P. L. & WeiÃgraeber, P. (2020). Modeling
+snow slab avalanches caused by weak-layer failure â Part 1: Slabs on
+compliant and collapsible weak layers. The Cryosphere, 14(1), 115â130. https:
+//doi.org/10.5194/tc-14-115-2020 - Rosendahl, P. L. & WeiÃgraeber, P. (2020).
+Modeling snow slab avalanches caused by weak-layer failure â Part 2: Coupled
+mixed-mode criterion for skier-triggered anticracks. The Cryosphere, 14(1),
 131â145. https://doi.org/10.5194/tc-14-131-2020 Written in [ð Python]
-(https://www.python.org) and built with [â Atom](https://atom.io), [ð
-GitKraken](https://www.gitkraken.com), and [ðª Jupyter](https://jupyter.org).
-Note that [release v1.0](https://github.com/2phi/weac/releases/tag/v1.0.0) was
-written and built in [ð MATLAB](https://www.mathworks.com/products/
-matlab.html).   ## Installation Install globally using the `pip` Package
-Installer for Python ```sh pip install -U weac ``` or clone the repo ```sh git
-clone https://github.com/2phi/weac ``` for local use. Needs - [Numpy](https://
-numpy.org/) for matrix operations - [Scipy](https://www.scipy.org/) for solving
-optimization problems - [Pandas](https://pandas.pydata.org/) for data handling
-- [Matplotlib](https://matplotlib.org/) for plotting  ## Usage The following
-describes the basic usage of WEAC. Please refer to the [demo](https://
-github.com/2phi/weac/blob/main/demo/demo.ipynb) for more examples and read the
-[documentation](https://2phi.github.io/weac/) for details. Load the module.
-```python import weac ``` Choose a snow profile from the database (see [demo]
-(https://github.com/2phi/weac/blob/main/demo/demo.ipynb)) or create your own as
-a 2D array where the columns are density (kg/m^2) and layer thickness (mm). One
-row corresponds to one layer counted from top (below surface) to bottom (above
-weak layer). ```python myprofile = [[170, 100], # (1) surface layer [190, 40],
-# (2) [230, 130], # : [250, 20], # : [210, 70], # (i) [380, 20], # : [280,
-100]] # (N) last slab layer above weak layer ``` Create a model instance with
-optional custom layering. ```python skier = weac.Layered(system='skier',
-layers=myprofile) ``` Calculate lists of segment lengths, locations of
-foundations, and position and magnitude of skier loads from the inputs total
-length `L` (mm), crack length `a` (mm), and skier weight `m` (kg). We can
-choose to analyze the situtation before a crack appears even if a crack length
-> 0 is set by replacing the `'crack'` key thorugh the `'nocrack'` key.
-```python segments = skier.calc_segments(L=10000, a=300, m=80)['crack'] ```
-Assemble the system of linear equations and solve the boundary-value problem
-for the free constants `C` providing the inclination `phi` (counterclockwise
-positive) in degrees. ```python C = skier.assemble_and_solve(phi=38,
-**segments) ``` Prepare the output by rasterizing the solution vector at all
-horizontal positions `xsl` (slab). The result is returned in the form of the
-ndarray `z`. We also get `xwl` (weak layer) that only contains x-coordinates
-that are supported by a foundation. ```python xsl, z, xwl =
-skier.rasterize_solution(C=C, phi=38, **segments) ``` Visualize the results.
-```python # Visualize deformations as a contour plot weac.plot.deformed(skier,
-xsl=xsl_skier, xwl=xwl_skier, z=z_skier, phi=inclination, window=200,
-scale=200, field='principal') # Plot slab displacements (using x-coordinates of
-all segments, xsl) weac.plot.displacements(skier, x=xsl, z=z, **segments) #
-Plot weak-layer stresses (using only x-coordinates of bedded segments, xwl)
-weac.plot.stresses(skier, x=xwl, z=z, **segments) ``` Compute output quantities
-for exporting or plotting. ```python # Slab deflections (using x-coordinates of
-all segments, xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z,
-unit='um') # Weak-layer shear stress (using only x-coordinates of bedded
-segments, xwl) x_cm, tau_kPa = skier.get_weaklayer_shearstress(x=xwl, z=z,
-unit='kPa') ```  ## Roadmap See the [open issues](https://github.com/2phi/weac/
-issues) for a list of proposed features and known issues. ### v2.5 - [ ] Finite
-fracture mechanics implementation for layered snow covers ### v2.4 - [ ]
-Implement anistropic weak layer - [ ] Add demo gif ## Release history ### v2.3
-- Stress plots on deformed contours - PSTs now account for slab touchdown ###
-v2.2 - Sign of inclination `phi` consistent with the coordinate system
-(positive counterclockwise) - Dimension arguments to field-quantity methods
-added - Improved aspect ratio of profile views and contour plots - Improved
-plot labels - Convenience methods for the export of weak-layer stresses and
-slab deformations provided - Wrapper for (re)calculation of the fundamental
-system added - Now allows for distributed surface loads ### v2.1 - Consistent
-use of coordinate system with downward pointing z-axis - Consitent top-to-
-bottom numbering of slab layers - Implementation of PSTs cut from either left
-or right side ### v2.0 - Completely rewritten in ð Python - Coupled bending-
-extension ODE solver implemented - Stress analysis of arbitrarily layered snow
-slabs - FEM validation of - displacements - weak-layer stresses - energy
-release rates in weak layers - Documentation - Demo and examples ### v1.0 -
-Written in ð MATLAB - Deformation analysis of homogeneous snow labs - Weak-
-layer stress prediction - Energy release rates of cracks in weak layers -
-Finite fracture mechanics implementation - Prediction of anticrack nucleation
-## How to contribute 1. Fork the project 2. Create your feature branch (`git
-checkout -b feature/amazingfeature`) 3. Commit your changes (`git commit -
-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin feature/
-amazingfeature`) 5. Open a pull request  ## License Copyright 2phi GbR, 2020-
-2022. We currently do not offer an open source license. Please contact us for
-private licensing options.  ## Contact E-mail: mail@2phi.de Â· Web: https://
-2phi.de Â· Project Link: [https://github.com/2phi/weac](https://github.com/
-2phi/weac) Â· Project DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://
-dx.doi.org/10.5281/zenodo.5773113)   [contributors-badge]: https://
-img.shields.io/github/contributors/2phi/weac.svg?style=flat-
-square&logo=github&color=yellow [forks-badge]: https://img.shields.io/github/
-forks/2phi/weac.svg?&color=blueviolet&style=flat-square&logo=github [stars-
-badge]: https://img.shields.io/github/stars/2phi/weac.svg?style=flat-
+(https://www.python.org) and built with [ð» Visual Studio Code](https://
+code.visualstudio.com), [ð GitKraken](https://www.gitkraken.com), and [ðª
+Jupyter](https://jupyter.org). Note that [release v1.0](https://github.com/
+2phi/weac/releases/tag/v1.0.0) was written and built in [ð MATLAB](https://
+www.mathworks.com/products/matlab.html).   ## Installation Install globally
+using the `pip` Package Installer for Python ```sh pip install -U weac ``` or
+clone the repo ```sh git clone https://github.com/2phi/weac ``` for local use.
+Needs - [Python](https://www.python.org/downloads/release/python-3100/) ≥ 3.10
+- [Numpy](https://numpy.org/) for matrix operations - [Scipy](https://
+www.scipy.org/) for solving optimization problems - [Pandas](https://
+pandas.pydata.org/) for data handling - [Matplotlib](https://matplotlib.org/
+) for plotting  ## Usage The following describes the basic usage of WEAC.
+Please refer to the [demo](https://github.com/2phi/weac/blob/main/demo/
+demo.ipynb) for more examples and read the [documentation](https://
+2phi.github.io/weac/) for details. Load the module. ```python import weac ```
+Choose a snow profile from the database (see [demo](https://github.com/2phi/
+weac/blob/main/demo/demo.ipynb)) or create your own as a 2D array where the
+columns are density (kg/m^2) and layer thickness (mm). One row corresponds to
+one layer counted from top (below surface) to bottom (above weak layer).
+```python myprofile = [[170, 100], # (1) surface layer [190, 40], # (2) [230,
+130], # : [250, 20], # : [210, 70], # (i) [380, 20], # : [280, 100]] # (N) last
+slab layer above weak layer ``` Create a model instance with optional custom
+layering. ```python skier = weac.Layered(system='skier', layers=myprofile) ```
+Calculate lists of segment lengths, locations of foundations, and position and
+magnitude of skier loads from the inputs total length `L` (mm), crack length
+`a` (mm), and skier weight `m` (kg). We can choose to analyze the situtation
+before a crack appears even if a crack length > 0 is set by replacing the
+`'crack'` key thorugh the `'nocrack'` key. ```python segments =
+skier.calc_segments(L=10000, a=300, m=80)['crack'] ``` Assemble the system of
+linear equations and solve the boundary-value problem for the free constants
+`C` providing the inclination `phi` (counterclockwise positive) in degrees.
+```python C = skier.assemble_and_solve(phi=38, **segments) ``` Prepare the
+output by rasterizing the solution vector at all horizontal positions `xsl`
+(slab). The result is returned in the form of the ndarray `z`. We also get
+`xwl` (weak layer) that only contains x-coordinates that are supported by a
+foundation. ```python xsl, z, xwl = skier.rasterize_solution(C=C, phi=38,
+**segments) ``` Visualize the results. ```python # Visualize deformations as a
+contour plot weac.plot.deformed(skier, xsl=xsl_skier, xwl=xwl_skier, z=z_skier,
+phi=inclination, window=200, scale=200, field='principal') # Plot slab
+displacements (using x-coordinates of all segments, xsl)
+weac.plot.displacements(skier, x=xsl, z=z, **segments) # Plot weak-layer
+stresses (using only x-coordinates of bedded segments, xwl) weac.plot.stresses
+(skier, x=xwl, z=z, **segments) ``` Compute output quantities for exporting or
+plotting. ```python # Slab deflections (using x-coordinates of all segments,
+xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z, unit='um') # Weak-layer
+shear stress (using only x-coordinates of bedded segments, xwl) x_cm, tau_kPa =
+skier.get_weaklayer_shearstress(x=xwl, z=z, unit='kPa') ```  ## Roadmap See the
+[open issues](https://github.com/2phi/weac/issues) for a list of proposed
+features and known issues. ### v2.5 - [ ] Finite fracture mechanics
+implementation for layered snow covers ### v2.4 - [ ] Implement anistropic weak
+layer - [ ] Add demo gif ## Release history ### v2.3 - Stress plots on deformed
+contours - PSTs now account for slab touchdown ### v2.2 - Sign of inclination
+`phi` consistent with the coordinate system (positive counterclockwise) -
+Dimension arguments to field-quantity methods added - Improved aspect ratio of
+profile views and contour plots - Improved plot labels - Convenience methods
+for the export of weak-layer stresses and slab deformations provided - Wrapper
+for (re)calculation of the fundamental system added - Now allows for
+distributed surface loads ### v2.1 - Consistent use of coordinate system with
+downward pointing z-axis - Consitent top-to-bottom numbering of slab layers -
+Implementation of PSTs cut from either left or right side ### v2.0 - Completely
+rewritten in ð Python - Coupled bending-extension ODE solver implemented -
+Stress analysis of arbitrarily layered snow slabs - FEM validation of -
+displacements - weak-layer stresses - energy release rates in weak layers -
+Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
+Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
+Energy release rates of cracks in weak layers - Finite fracture mechanics
+implementation - Prediction of anticrack nucleation  ## How to contribute 1.
+Fork the project 2. Create your feature branch (`git checkout -b feature/
+amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
+feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
+Open a pull request  ## License Copyright 2phi GbR, 2020-2023. We currently do
+not offer an open source license. Please contact us for private licensing
+options.  ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
+Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
+DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
+zenodo.5773113)   [contributors-badge]: https://img.shields.io/github/
+contributors/2phi/weac.svg?style=flat-square&logo=github&color=yellow [forks-
+badge]: https://img.shields.io/github/forks/2phi/
+weac.svg?&color=blueviolet&style=flat-square&logo=github [stars-badge]: https:/
+/img.shields.io/github/stars/2phi/weac.svg?style=flat-
 square&logo=github&color=orange [issues-badge]: https://img.shields.io/github/
 issues/2phi/weac.svg?style=flat-square&logo=github [pypi-badge]: https://
 img.shields.io/pypi/v/
 weac.svg?logo=python&logoColor=white&color=f46b58&style=flat-square [pypi-
 downloads-badge]: https://img.shields.io/pypi/dm/
 weac.svg?logo=python&logoColor=white&color=red&style=flat-square [python-dist-
 badge]: https://img.shields.io/pypi/pyversions/weac.svg?style=flat-
```

### Comparing `weac-2.3.1/img/bc.png` & `weac-2.3.2/img/bc.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/img/layering.png` & `weac-2.3.2/img/layering.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/img/logo.png` & `weac-2.3.2/img/logo.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/img/model.png` & `weac-2.3.2/img/model.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/img/profiles.png` & `weac-2.3.2/img/profiles.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/img/systems.png` & `weac-2.3.2/img/systems.png`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/setup.cfg` & `weac-2.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weac
-version = 2.3.1
+version = 2.3.2
 author = 2phi GbR
 author_email = mail@2phi.de
 description = Weak layer anticrack nucleation model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/2phi/weac
 project_urls =
```

### Comparing `weac-2.3.1/weac/eigensystem.py` & `weac-2.3.2/weac/eigensystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=invalid-name,too-many-instance-attributes
 # pylint: disable=too-many-arguments,too-many-locals
 
 # Third party imports
 import numpy as np
 
 # Project imports
-from weac.tools import gerling, calc_center_of_gravity, load_dummy_profile
+from weac.tools import bergfeld, calc_center_of_gravity, load_dummy_profile
 
 
 class Eigensystem:
     """
     Base class for a layered beam on an elastic foundation.
 
     Provides geometry, material and loading attributes, and methods
@@ -176,15 +176,15 @@
             'E': E              # Young's modulus (MPa)
         }
 
         # Recalculate the fundamental system after properties have changed
         if update:
             self.calc_fundamental_system()
 
-    def set_beam_properties(self, layers, phi=0, C0=6.0, C1=4.60,
+    def set_beam_properties(self, layers, phi=0, C0=6.5, C1=4.4,
                             nu=0.25, update=False):
         """
         Set material and properties geometry of beam (slab).
 
         Arguments
         ---------
         layers : list or str
@@ -192,31 +192,31 @@
             Columns are density (kg/m^3) and thickness (mm). One row
             corresponds to one layer. If entered as str, last split
             must be available in database.
         phi : float
             Inclination of the slab (degrees).
         C0 : float, optional
             Multiplicative constant of Young modulus parametrization
-            according to Gerling et al. (2017). Default is 6.0.
+            according to Bergfeld et al. (2023). Default is 6.0.
         C1 : float, optional
             Exponent of Young modulus parameterization according to
-            Gerling et al. (2017). Default is 4.6.
+            Bergfeld et al. (2023). Default is 4.6.
         nu : float, optional
             Possion's ratio. Default is 0.25
         update : bool, optional
             If true, recalculate the fundamental system after
             foundation properties have changed.
         """
         if isinstance(layers, str):
             # Read layering and Young's modulus from database
             layers, E = load_dummy_profile(layers.split()[-1])
         else:
             # Compute Young's modulus from density parametrization
             layers = np.array(layers)
-            E = gerling(layers[:, 0], C0=C0, C1=C1)  # Young's modulus
+            E = bergfeld(layers[:, 0], C0=C0, C1=C1)  # Young's modulus
 
         # Derive other elastic properties
         nu = nu*np.ones(layers.shape[0])         # Global poisson's ratio
         G = E/(2*(1 + nu))                       # Shear modulus
         self.k = 5/6                             # Shear correction factor
 
         # Compute total slab thickness and center of gravity
```

### Comparing `weac-2.3.1/weac/inverse.py` & `weac-2.3.2/weac/inverse.py`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/weac/layered.py` & `weac-2.3.2/weac/layered.py`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/weac/mixins.py` & `weac-2.3.2/weac/mixins.py`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/weac/plot.py` & `weac-2.3.2/weac/plot.py`

 * *Files identical despite different names*

### Comparing `weac-2.3.1/weac/tools.py` & `weac-2.3.2/weac/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,40 @@
     Returns
     -------
     E : float or ndarray
         Young's modulus (MPa).
     """
     return C0*1e-10*rho**C1
 
+
+def bergfeld(rho, rho0=917, C0=6.5, C1=4.4):
+    """
+    Compute Young's modulus from density according to Bergfeld et al. (2023).
+
+    Arguments
+    ---------
+    rho : float or ndarray
+        Density (kg/m^3).
+    rho0 : float, optional
+        Density of ice (kg/m^3). Default is 917.
+    C0 : float, optional
+        Multiplicative constant of Young modulus parametrization
+        according to Bergfeld et al. (2023). Default is 6.5.
+    C1 : float, optional
+        Exponent of Young modulus parameterization according to
+        Bergfeld et al. (2023). Default is 4.4.
+
+    Returns
+    -------
+    E : float or ndarray
+        Young's modulus (MPa).
+    """
+    return C0*1e3*(rho/rho0)**C1
+
+
 def tensile_strength_slab(rho, unit='kPa'):
     """
     Estimate the tensile strenght of a slab layer from its density.
 
     Uses the density parametrization of Sigrist (2006).
 
     Arguments
```

