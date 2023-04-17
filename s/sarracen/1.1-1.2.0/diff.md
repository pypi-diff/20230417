# Comparing `tmp/sarracen-1.1.tar.gz` & `tmp/sarracen-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarracen-1.1.tar", last modified: Thu Mar  9 18:50:03 2023, max compression
+gzip compressed data, was "sarracen-1.2.0.tar", last modified: Mon Apr 17 00:51:45 2023, max compression
```

## Comparing `sarracen-1.1.tar` & `sarracen-1.2.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0      679 2023-03-08 20:46:38.425139 sarracen-1.1/.github/workflows/joss_paper.yml
--rw-r--r--   0        0        0       76 2023-03-08 20:46:38.425279 sarracen-1.1/.gitignore
--rw-r--r--   0        0        0      125 2023-03-08 20:46:38.425399 sarracen-1.1/.readthedocs.yaml
--rw-r--r--   0        0        0    35149 2023-03-08 20:46:38.425759 sarracen-1.1/LICENCE
--rw-r--r--   0        0        0     1445 2023-03-08 20:46:38.425951 sarracen-1.1/README.md
--rw-r--r--   0        0        0      634 2023-03-08 20:46:38.426138 sarracen-1.1/docs/Makefile
--rw-r--r--   0        0        0     1490 2023-03-08 20:46:38.426268 sarracen-1.1/docs/api.rst
--rw-r--r--   0        0        0     2153 2023-03-08 20:46:38.426414 sarracen-1.1/docs/conf.py
--rw-r--r--   0        0        0      133 2023-03-08 20:46:38.426531 sarracen-1.1/docs/examples.rst
--rw-r--r--   0        0        0     2310 2023-03-08 20:46:38.426723 sarracen-1.1/docs/examples/dustydisc.rst
--rw-r--r--   0        0        0   300231 2023-03-08 20:46:38.428967 sarracen-1.1/docs/examples/dustydisc/dustydisc-describe.png
--rw-r--r--   0        0        0   577154 2023-03-08 20:46:38.432428 sarracen-1.1/docs/examples/dustydisc/dustydisc-dust.png
--rw-r--r--   0        0        0   296363 2023-03-08 20:46:38.434636 sarracen-1.1/docs/examples/dustydisc/dustydisc-gas-sinks.png
--rw-r--r--   0        0        0   296269 2023-03-08 20:46:38.436847 sarracen-1.1/docs/examples/dustydisc/dustydisc-gas.png
--rw-r--r--   0        0        0   152484 2023-03-08 20:46:38.438050 sarracen-1.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png
--rw-r--r--   0        0        0   506967 2023-03-08 20:46:38.441377 sarracen-1.1/docs/examples/dustydisc/dustydisc-sdf.png
--rw-r--r--   0        0        0    17275 2023-03-08 20:46:38.441665 sarracen-1.1/docs/examples/dustydisc/dustydisc-value-counts.png
--rw-r--r--   0        0        0     1121 2023-03-08 20:46:38.441831 sarracen-1.1/docs/examples/ot.rst
--rw-r--r--   0        0        0    18453 2023-03-08 20:46:38.442081 sarracen-1.1/docs/examples/ot/ot-1d.png
--rw-r--r--   0        0        0   145467 2023-03-08 20:46:38.443058 sarracen-1.1/docs/examples/ot/ot-describe.png
--rw-r--r--   0        0        0   178608 2023-03-08 20:46:38.444233 sarracen-1.1/docs/examples/ot/ot-sdf.png
--rw-r--r--   0        0        0    70378 2023-03-08 20:46:38.444776 sarracen-1.1/docs/examples/ot/ot-streamlines.png
--rw-r--r--   0        0        0    48370 2023-03-08 20:46:38.445169 sarracen-1.1/docs/examples/ot/ot.png
--rw-r--r--   0        0        0     1122 2023-03-08 20:46:38.445302 sarracen-1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-03-08 20:46:38.445407 sarracen-1.1/docs/make.bat
--rw-r--r--   0        0        0    95948 2023-03-08 20:46:38.446192 sarracen-1.1/docs/paper/main_image.png
--rw-r--r--   0        0        0    13796 2023-03-08 20:46:38.446368 sarracen-1.1/docs/paper/paper.bib
--rw-r--r--   0        0        0     5957 2023-03-09 17:36:21.736765 sarracen-1.1/docs/paper/paper.md
--rw-r--r--   0        0        0     3964 2023-03-08 20:46:38.446656 sarracen-1.1/docs/quick-start.rst
--rw-r--r--   0        0        0     4814 2023-03-08 20:46:38.446786 sarracen-1.1/docs/render.rst
--rw-r--r--   0        0        0      527 2023-03-08 20:46:38.446884 sarracen-1.1/pyproject.toml
--rw-r--r--   0        0        0       75 2023-03-08 20:46:38.446973 sarracen-1.1/requirements.txt
--rw-r--r--   0        0        0      361 2023-03-09 17:36:21.736953 sarracen-1.1/sarracen/__init__.py
--rw-r--r--   0        0        0      385 2023-03-08 20:46:38.447257 sarracen-1.1/sarracen/interpolate/__init__.py
--rw-r--r--   0        0        0     4766 2023-03-08 20:46:38.447576 sarracen-1.1/sarracen/interpolate/base_backend.py
--rw-r--r--   0        0        0    25031 2023-03-08 20:46:38.447733 sarracen-1.1/sarracen/interpolate/cpu_backend.py
--rw-r--r--   0        0        0    27074 2023-03-08 20:46:38.447845 sarracen-1.1/sarracen/interpolate/gpu_backend.py
--rw-r--r--   0        0        0    51425 2023-03-09 17:36:21.737311 sarracen-1.1/sarracen/interpolate/interpolate.py
--rw-r--r--   0        0        0      212 2023-03-08 20:46:38.448400 sarracen-1.1/sarracen/kernels/__init__.py
--rw-r--r--   0        0        0     3467 2023-03-08 20:46:38.448509 sarracen-1.1/sarracen/kernels/base_kernel.py
--rw-r--r--   0        0        0      562 2023-03-08 20:46:38.448596 sarracen-1.1/sarracen/kernels/cubic_spline.py
--rw-r--r--   0        0        0    13535 2023-03-08 20:46:38.448747 sarracen-1.1/sarracen/kernels/cubic_spline_exact.py
--rw-r--r--   0        0        0      634 2023-03-08 20:46:38.448822 sarracen-1.1/sarracen/kernels/quartic_spline.py
--rw-r--r--   0        0        0      607 2023-03-08 20:46:38.448904 sarracen-1.1/sarracen/kernels/quintic_spline.py
--rw-r--r--   0        0        0        1 2023-03-08 20:46:38.449036 sarracen-1.1/sarracen/readers/__init__.py
--rw-r--r--   0        0        0      678 2023-03-08 20:46:38.449127 sarracen-1.1/sarracen/readers/read_csv.py
--rw-r--r--   0        0        0     8959 2023-03-08 20:46:38.449247 sarracen-1.1/sarracen/readers/read_marisa.py
--rw-r--r--   0        0        0     9017 2023-03-08 20:46:38.449376 sarracen-1.1/sarracen/readers/read_phantom.py
--rw-r--r--   0        0        0    28551 2023-03-09 17:36:21.737571 sarracen-1.1/sarracen/render.py
--rw-r--r--   0        0        0    18033 2023-03-08 20:46:38.449739 sarracen-1.1/sarracen/sarracen_dataframe.py
--rw-r--r--   0        0        0        0 2023-03-08 20:46:38.449835 sarracen-1.1/sarracen/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 20:46:38.449926 sarracen-1.1/sarracen/tests/readers/__init__.py
--rw-r--r--   0        0        0      969 2023-03-08 20:46:38.450018 sarracen-1.1/sarracen/tests/readers/test_read_csv.py
--rw-r--r--   0        0        0    75799 2023-03-09 17:36:21.737944 sarracen-1.1/sarracen/tests/test_interpolate.py
--rw-r--r--   0        0        0     8159 2023-03-08 20:46:38.450466 sarracen-1.1/sarracen/tests/test_kernels.py
--rw-r--r--   0        0        0    11302 2023-03-09 17:36:21.738143 sarracen-1.1/sarracen/tests/test_render.py
--rw-r--r--   0        0        0     5514 2023-03-08 20:46:38.450688 sarracen-1.1/sarracen/tests/test_sarracen_dataframe.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 sarracen-1.1/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-04-17 00:51:11.188684 sarracen-1.2.0/.github/workflows/joss_paper.yml
+-rw-r--r--   0        0        0       76 2023-04-17 00:51:11.188880 sarracen-1.2.0/.gitignore
+-rw-r--r--   0        0        0      125 2023-04-17 00:51:11.189036 sarracen-1.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    35149 2023-04-17 00:51:11.189358 sarracen-1.2.0/LICENCE
+-rw-r--r--   0        0        0     1445 2023-04-17 00:51:11.189538 sarracen-1.2.0/README.md
+-rw-r--r--   0        0        0      634 2023-04-17 00:51:11.189715 sarracen-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1712 2023-04-17 00:51:11.189922 sarracen-1.2.0/docs/api.rst
+-rw-r--r--   0        0        0     2153 2023-04-17 00:51:11.190043 sarracen-1.2.0/docs/conf.py
+-rw-r--r--   0        0        0      133 2023-04-17 00:51:11.190144 sarracen-1.2.0/docs/examples.rst
+-rw-r--r--   0        0        0     2310 2023-04-17 00:51:11.190323 sarracen-1.2.0/docs/examples/dustydisc.rst
+-rw-r--r--   0        0        0   300231 2023-04-17 00:51:11.191988 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-describe.png
+-rw-r--r--   0        0        0   577154 2023-04-17 00:51:11.195266 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-dust.png
+-rw-r--r--   0        0        0   296363 2023-04-17 00:51:11.197124 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas-sinks.png
+-rw-r--r--   0        0        0   296269 2023-04-17 00:51:11.198908 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas.png
+-rw-r--r--   0        0        0   152484 2023-04-17 00:51:11.199956 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf-sinks.png
+-rw-r--r--   0        0        0   506967 2023-04-17 00:51:11.202675 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf.png
+-rw-r--r--   0        0        0    17275 2023-04-17 00:51:11.202921 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-value-counts.png
+-rw-r--r--   0        0        0     1121 2023-04-17 00:51:11.203063 sarracen-1.2.0/docs/examples/ot.rst
+-rw-r--r--   0        0        0    18453 2023-04-17 00:51:11.203305 sarracen-1.2.0/docs/examples/ot/ot-1d.png
+-rw-r--r--   0        0        0   145467 2023-04-17 00:51:11.204116 sarracen-1.2.0/docs/examples/ot/ot-describe.png
+-rw-r--r--   0        0        0   178608 2023-04-17 00:51:11.205112 sarracen-1.2.0/docs/examples/ot/ot-sdf.png
+-rw-r--r--   0        0        0    70378 2023-04-17 00:51:11.205587 sarracen-1.2.0/docs/examples/ot/ot-streamlines.png
+-rw-r--r--   0        0        0    48370 2023-04-17 00:51:11.206005 sarracen-1.2.0/docs/examples/ot/ot.png
+-rw-r--r--   0        0        0     1138 2023-04-17 00:51:11.206139 sarracen-1.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1648 2023-04-17 00:51:11.206243 sarracen-1.2.0/docs/installation.rst
+-rw-r--r--   0        0        0      800 2023-04-17 00:51:11.206354 sarracen-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0    95948 2023-04-17 00:51:11.207023 sarracen-1.2.0/docs/paper/main_image.png
+-rw-r--r--   0        0        0    14031 2023-04-17 00:51:11.207197 sarracen-1.2.0/docs/paper/paper.bib
+-rw-r--r--   0        0        0     5953 2023-04-17 00:51:11.207327 sarracen-1.2.0/docs/paper/paper.md
+-rw-r--r--   0        0        0     3484 2023-04-17 00:51:11.207450 sarracen-1.2.0/docs/quick-start.rst
+-rw-r--r--   0        0        0     4814 2023-04-17 00:51:11.207605 sarracen-1.2.0/docs/render.rst
+-rw-r--r--   0        0        0      527 2023-04-17 00:51:11.207721 sarracen-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-04-17 00:51:11.207809 sarracen-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      363 2023-04-17 00:51:11.207950 sarracen-1.2.0/sarracen/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-17 00:51:11.208083 sarracen-1.2.0/sarracen/interpolate/__init__.py
+-rw-r--r--   0        0        0     4766 2023-04-17 00:51:11.208403 sarracen-1.2.0/sarracen/interpolate/base_backend.py
+-rw-r--r--   0        0        0    24755 2023-04-17 00:51:11.208617 sarracen-1.2.0/sarracen/interpolate/cpu_backend.py
+-rw-r--r--   0        0        0    27110 2023-04-17 00:51:11.208770 sarracen-1.2.0/sarracen/interpolate/gpu_backend.py
+-rw-r--r--   0        0        0    55074 2023-04-17 00:51:11.209147 sarracen-1.2.0/sarracen/interpolate/interpolate.py
+-rw-r--r--   0        0        0      212 2023-04-17 00:51:11.209355 sarracen-1.2.0/sarracen/kernels/__init__.py
+-rw-r--r--   0        0        0     3467 2023-04-17 00:51:11.209488 sarracen-1.2.0/sarracen/kernels/base_kernel.py
+-rw-r--r--   0        0        0      562 2023-04-17 00:51:11.209590 sarracen-1.2.0/sarracen/kernels/cubic_spline.py
+-rw-r--r--   0        0        0    13535 2023-04-17 00:51:11.209724 sarracen-1.2.0/sarracen/kernels/cubic_spline_exact.py
+-rw-r--r--   0        0        0      634 2023-04-17 00:51:11.209820 sarracen-1.2.0/sarracen/kernels/quartic_spline.py
+-rw-r--r--   0        0        0      607 2023-04-17 00:51:11.209913 sarracen-1.2.0/sarracen/kernels/quintic_spline.py
+-rw-r--r--   0        0        0        1 2023-04-17 00:51:11.210036 sarracen-1.2.0/sarracen/readers/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-17 00:51:11.210127 sarracen-1.2.0/sarracen/readers/read_csv.py
+-rw-r--r--   0        0        0     8959 2023-04-17 00:51:11.210252 sarracen-1.2.0/sarracen/readers/read_marisa.py
+-rw-r--r--   0        0        0     9017 2023-04-17 00:51:11.210386 sarracen-1.2.0/sarracen/readers/read_phantom.py
+-rw-r--r--   0        0        0    29829 2023-04-17 00:51:11.210506 sarracen-1.2.0/sarracen/render.py
+-rw-r--r--   0        0        0    19956 2023-04-17 00:51:11.210693 sarracen-1.2.0/sarracen/sarracen_dataframe.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:51:11.210799 sarracen-1.2.0/sarracen/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:51:11.210889 sarracen-1.2.0/sarracen/tests/readers/__init__.py
+-rw-r--r--   0        0        0      969 2023-04-17 00:51:11.210978 sarracen-1.2.0/sarracen/tests/readers/test_read_csv.py
+-rw-r--r--   0        0        0    84917 2023-04-17 00:51:11.211350 sarracen-1.2.0/sarracen/tests/test_interpolate.py
+-rw-r--r--   0        0        0     8159 2023-04-17 00:51:11.211500 sarracen-1.2.0/sarracen/tests/test_kernels.py
+-rw-r--r--   0        0        0    11302 2023-04-17 00:51:11.211642 sarracen-1.2.0/sarracen/tests/test_render.py
+-rw-r--r--   0        0        0     5514 2023-04-17 00:51:11.211798 sarracen-1.2.0/sarracen/tests/test_sarracen_dataframe.py
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 sarracen-1.2.0/PKG-INFO
```

### Comparing `sarracen-1.1/.github/workflows/joss_paper.yml` & `sarracen-1.2.0/.github/workflows/joss_paper.yml`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/LICENCE` & `sarracen-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/README.md` & `sarracen-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/Makefile` & `sarracen-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/api.rst` & `sarracen-1.2.0/docs/api.rst`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,40 @@
 
 =============
 API Reference
 =============
 
 .. currentmodule:: sarracen
 
+File reading
+------------
+
+Sarracen can read all general file formats supported by pandas (csv, notably).
+
+For SPH codes, Sarracen supports reading the native binary format of the `Phantom
+SPH code <https://phantomsph.bitbucket.io>`_. Raise an issue on our GitHub if you
+would like Sarracen to be able to read the file format for other SPH codes (or
+make a pull request!).
+
+.. autosummary::
+   :toctree: api/
+
+   read_csv
+   read_phantom
+   read_marisa
+
+
 SarracenDataFrame
 -----------------
 
-A SarracenDataFrame extends the pandas DataFrame class. It holds SPH particle data. They attempt to find particle position, velocity, smoothing length, mass and density within the data so that they can be used to interpolate and render the data.
+A SarracenDataFrame is a subclass of the pandas DataFrame class. It holds SPH
+particle data. SarracenDataFrames will attempt to identify columns which hold
+particle positions, velocities, smoothing lengths, masses and densities so that
+they can be used for interpolation and rendering. Global simulation values are
+stored in ``params``, which is a standard Python dictionary.
 
 Constructor
 """""""""""
 .. autosummary::
    :toctree: api/
    :nosignatures:
 
@@ -43,27 +65,14 @@
 
 .. autosummary::
    :toctree: api/
 
    SarracenDataFrame.sph_interpolate
 
 
-File reading
-------------
-
-Sarracen can read the native binary format of the Phantom SPH code (`https://phantomsph.bitbucket.io <https://phantomsph.bitbucket.io/>`_). Contact us if you want Sarracen to be able to read the file format for other SPH codes (or make a pull request!).
-
-.. autosummary::
-   :toctree: api/
-
-   read_phantom
-   read_csv
-   read_marisa
-
-
 Kernels
 -------
 
 The default smoothing kernel is the cubic spline. Additional smoothing kernels are included within Sarracen.
 
 .. autosummary::
    :toctree: api/
```

### Comparing `sarracen-1.1/docs/conf.py` & `sarracen-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc.rst` & `sarracen-1.2.0/docs/examples/dustydisc.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-describe.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-dust.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-dust.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-gas-sinks.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-gas.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-sdf.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/dustydisc/dustydisc-value-counts.png` & `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-value-counts.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot.rst` & `sarracen-1.2.0/docs/examples/ot.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot/ot-1d.png` & `sarracen-1.2.0/docs/examples/ot/ot-1d.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot/ot-describe.png` & `sarracen-1.2.0/docs/examples/ot/ot-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot/ot-sdf.png` & `sarracen-1.2.0/docs/examples/ot/ot-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot/ot-streamlines.png` & `sarracen-1.2.0/docs/examples/ot/ot-streamlines.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/examples/ot/ot.png` & `sarracen-1.2.0/docs/examples/ot/ot.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/index.rst` & `sarracen-1.2.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
 ======================
 Sarracen documentation
 ======================
 
 Sarracen is a Python library for analysis and visualization of smoothed particle hydrodynamics (SPH) data.
 
-It is built upon the pandas and Matplotlib data and visualization libraries.  SPH data can be loaded into a pandas DataFrame structure that has been extended to support SPH. Visualizations of the data use the SPH kernel, and a variety of rendering options are available. All SPH interpolation functions are optimized using Numba into machine code with both multi-threaded and CUDA enabled routines. Our primary intended application is for astrophysical SPH simulations.
+It is built upon the pandas and Matplotlib data and visualization libraries.  SPH data can be loaded into a pandas
+DataFrame structure that has been extended to support SPH. Visualizations of the data use the SPH kernel, and a variety
+of rendering options are available. All SPH interpolation functions are optimized using Numba into machine code with
+both multi-threaded and CUDA enabled routines. Our primary intended application is for astrophysical SPH simulations.
 
-Visit the :ref:`quick start guide <quick_start>` to learn the basics of Sarracen. For details on specific functions, consult the :ref:`API reference <api>`. The codebase can be found on `Github <https://github.com/ttricco/sarracen/>`_.
+Visit the :ref:`quick start guide <quick_start>` to learn the basics of Sarracen. For details on specific functions,
+consult the :ref:`API reference <api>`. The codebase can be found on `GitHub <https://github.com/ttricco/sarracen/>`_.
 
 .. toctree::
    :maxdepth: 1
    :caption: Contents:
 
+   installation
    quick-start
    render
    examples
    api
 
 
 Indices and tables
```

### Comparing `sarracen-1.1/docs/make.bat` & `sarracen-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/paper/main_image.png` & `sarracen-1.2.0/docs/paper/main_image.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/docs/paper/paper.bib` & `sarracen-1.2.0/docs/paper/paper.bib`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 @ARTICLE{lucy:1977,
        author = {{Lucy}, L.~B.},
         title = "{A numerical approach to the testing of the fission hypothesis.}",
-      journal = {\aj},
+      journal = {Astronomical Journal},
      keywords = {Binary Stars, Hypotheses, Nuclear Fission, Numerical Analysis, Protostars, Stellar Evolution, Astronomical Models, Difference Equations, Gas Dynamics, Monte Carlo Method, Numerical Stability, Particle Motion, Stellar Rotation, Astrophysics},
          year = 1977,
         month = dec,
        volume = {82},
         pages = {1013-1024},
           doi = {10.1086/112164},
        adsurl = {https://ui.adsabs.harvard.edu/abs/1977AJ.....82.1013L},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 
 @ARTICLE{gm:1977,
        author = {{Gingold}, R.~A. and {Monaghan}, J.~J.},
         title = "{Smoothed particle hydrodynamics: theory and application to non-spherical stars.}",
-      journal = {\mnras},
+      journal = {Monthly Notices of the Royal Astronomical Society},
      keywords = {Hydrodynamics, Particle Theory, Stellar Models, Astrophysics, Stellar Rotation, Stellar Structure, Astrophysics},
          year = 1977,
         month = nov,
        volume = {181},
         pages = {375-389},
           doi = {10.1093/mnras/181.3.375},
        adsurl = {https://ui.adsabs.harvard.edu/abs/1977MNRAS.181..375G},
@@ -59,29 +59,29 @@
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 
 
 @ARTICLE{phantom,
        author = {{Price}, Daniel J. and {Wurster}, James and {Tricco}, Terrence S. and {Nixon}, Chris and {Toupin}, St{\'e}ven and {Pettitt}, Alex and {Chan}, Conrad and {Mentiplay}, Daniel and {Laibe}, Guillaume and {Glover}, Simon and {Dobbs}, Clare and {Nealon}, Rebecca and {Liptai}, David and {Worpel}, Hauke and {Bonnerot}, Cl{\'e}ment and {Dipierro}, Giovanni and {Ballabio}, Giulia and {Ragusa}, Enrico and {Federrath}, Christoph and {Iaconi}, Roberto and {Reichardt}, Thomas and {Forgan}, Duncan and {Hutchison}, Mark and {Constantino}, Thomas and {Ayliffe}, Ben and {Hirsh}, Kieran and {Lodato}, Giuseppe},
         title = "{Phantom: A Smoothed Particle Hydrodynamics and Magnetohydrodynamics Code for Astrophysics}",
-      journal = {\pasa},
+      journal = {Publications of the Astronomical Society of Australia},
      keywords = {accretion, accretion disks, hydrodynamics, ISM: general, magnetohydrodynamics (MHD), methods: numerical, Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Earth and Planetary Astrophysics, Astrophysics - Astrophysics of Galaxies, Astrophysics - High Energy Astrophysical Phenomena, Astrophysics - Solar and Stellar Astrophysics},
          year = 2018,
         month = sep,
        volume = {35},
           eid = {e031},
         pages = {e031},
           doi = {10.1017/pasa.2018.25},
 archivePrefix = {arXiv},
 }
 
 @ARTICLE{gasoline2,
        author = {{Wadsley}, James W. and {Keller}, Benjamin W. and {Quinn}, Thomas R.},
         title = "{Gasoline2: a modern smoothed particle hydrodynamics code}",
-      journal = {\mnras},
+      journal = {Monthly Notices of the Royal Astronomical Society},
      keywords = {hydrodynamics, methods: numerical, Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Cosmology and Nongalactic Astrophysics},
          year = 2017,
         month = oct,
        volume = {471},
        number = {2},
         pages = {2357-2369},
           doi = {10.1093/mnras/stx1643},
@@ -108,15 +108,15 @@
 }
 
 
 
 @ARTICLE{splash,
        author = {{Price}, Daniel J.},
         title = "{splash: An Interactive Visualisation Tool for Smoothed Particle Hydrodynamics Simulations}",
-      journal = {\pasa},
+      journal = {Publications of the Astronomical Society of Australia},
      keywords = {hydrodynamics, methods: numerical, Astrophysics},
          year = 2007,
         month = oct,
        volume = {24},
        number = {3},
         pages = {159-173},
           doi = {10.1071/AS07022},
@@ -126,15 +126,15 @@
        adsurl = {https://ui.adsabs.harvard.edu/abs/2007PASA...24..159P},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 
 @ARTICLE{yt,
        author = {{Turk}, Matthew J. and {Smith}, Britton D. and {Oishi}, Jeffrey S. and {Skory}, Stephen and {Skillman}, Samuel W. and {Abel}, Tom and {Norman}, Michael L.},
         title = "{yt: A Multi-code Analysis Toolkit for Astrophysical Simulation Data}",
-      journal = {\apjs},
+      journal = {Astrophysical Journal Supplement Series},
      keywords = {cosmology: theory, methods: data analysis, methods: numerical, Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Cosmology and Nongalactic Astrophysics},
          year = 2011,
         month = jan,
        volume = {192},
        number = {1},
           eid = {9},
         pages = {9},
@@ -205,15 +205,15 @@
   editor    = { van der {W}alt, {S}t\'efan and {M}illman, {J}arrod},
   doi       = { 10.25080/Majora-92bf1922-00a }
 }
 
 @ARTICLE{numpy,
        author = {{Harris}, Charles R. and {Millman}, K. Jarrod and {van der Walt}, St{\'e}fan J. and {Gommers}, Ralf and {Virtanen}, Pauli and {Cournapeau}, David and {Wieser}, Eric and {Taylor}, Julian and {Berg}, Sebastian and {Smith}, Nathaniel J. and {Kern}, Robert and {Picus}, Matti and {Hoyer}, Stephan and {van Kerkwijk}, Marten H. and {Brett}, Matthew and {Haldane}, Allan and {del R{\'\i}o}, Jaime Fern{\'a}ndez and {Wiebe}, Mark and {Peterson}, Pearu and {G{\'e}rard-Marchant}, Pierre and {Sheppard}, Kevin and {Reddy}, Tyler and {Weckesser}, Warren and {Abbasi}, Hameer and {Gohlke}, Christoph and {Oliphant}, Travis E.},
         title = "{Array programming with NumPy}",
-      journal = {\nat},
+      journal = {Nature},
      keywords = {Computer Science - Mathematical Software, Statistics - Computation},
          year = 2020,
         month = sep,
        volume = {585},
        number = {7825},
         pages = {357-362},
           doi = {10.1038/s41586-020-2649-2},
```

### Comparing `sarracen-1.1/docs/paper/paper.md` & `sarracen-1.2.0/docs/paper/paper.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Summary
 
 `Sarracen` is a Python package for analyzing and visualizing smoothed particle
 hydrodynamics (SPH) data. SPH is a method of fluid simulation that discretizes
 fluid elements into a collection of particles [@gm:1977; @lucy:1977; @monaghan:2005;
 @price:2012]. This approach works well for many astrophysical problems of interest,
 and as such there are a number of SPH codes widely used for astrophysical 
-simulations, e.g., [@gasoline2; @phantom; @swift]. `Sarracen` offers a variety of 
+simulations, e.g., @gasoline2, @phantom, @swift. `Sarracen` offers a variety of 
 SPH interpolation methods to aid in analysis and visualization of SPH data. It is 
 built in Python so that users can leverage the robust scientific libraries that are 
 available. Much of the core of `Sarracen` is built upon `pandas` and `Matplotlib`. 
 Users familiar with these packages should be able to use `Sarracen` to do complex 
 analyses without difficulty. Our intended use is for astrophysical SPH data, but 
 anticipate that our package may be useful in other scientific domains. 
 
@@ -84,15 +84,15 @@
 `Sarracen` includes multiple choices for the smoothing kernel, with the cubic spline 
 as default. 
 
 For 3D data, a quantity may be interpolated to a 3D fixed grid, to a 2D grid 
 representing a slice through the data, or to a 1D line that cuts through the volume. 
 Column integrated line-of-sight interpolation is included. Interpolation of 2D data 
 is also supported. Additionally, `Sarracen` implements the mapping method of 
-[@petkova:2018], which exactly computes the volume-averaged quantity within each 
+@petkova:2018, which exactly computes the volume-averaged quantity within each 
 cell of a fixed grid by analytically computing the integral of the kernel function 
 over the volume of each cell. `Sarracen` can render interpolated grids with 
 `Matplotlib` using API syntax inspired by `Seaborn` [@seaborn]. Vector quantities, 
 such as velocity, can be rendered with streamlines or arrow plots. `Sarracen` uses 
 `SciPy` to support view rotation, with the rotation specified by Euler angles, a 
 rotation vector, rotation matrix or quaternions.
```

### Comparing `sarracen-1.1/docs/quick-start.rst` & `sarracen-1.2.0/docs/quick-start.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 .. _quick_start:
 
 =================
 Quick Start Guide
 =================
 
-Installation
-------------
-
-The latest stable release and associated dependencies can be installed from PyPi:
-
-.. code-block::
-
-    pip install sarracen
-
-This is the recommended way to install Sarracen.
-
-The latest development snapshot is available on the GitHub repository. Either clone the repository and add it to your path so that it can be imported, or install directly through pip:
-
-.. code-block::
-
-    pip install git+https://github.com/ttricco/sarracen.git
-
 
 
 Loading data into a SarracenDataFrame
 -------------------------------------
 
 SarracenDataFrame extends the pandas DataFrame. Thus, Sarracen can read all the file formats that pandas supports.
 
 Additionally, Sarracen can read the native binary format of `Phantom <https://phantomsph.bitbucket.io>`_. We would like to support file formats for other SPH codes in future. Contact us if you wish to have your code supported (or raise an issue).
 
 Loading Phantom data is as straightforward as
 
-.. code-block::
-
-   sdf = sarracen.read_phantom('dumpfile')
+>>> import sarracen
+>>>
+>>> sdf = sarracen.read_phantom('dumpfile')
 
 This call can separate different particle species into their own SarracenDataFrame. By default, sink particles are separated, and a list of SarracenDataFrames is returned in such a case. For example, if you data contains SPH particles plus sink particles, a sensible call would be
 
-.. code-block::
-
-   sdf, sdf_sinks = sarracen.read_phantom('dumpfile')
+>>> import sarracen
+>>>
+>>> sdf, sdf_sinks = sarracen.read_phantom('dumpfile')
 
 If you encounter any bugs with file reading for your particular set up, please contact us or raise an issue.
 
 
 Analysis
 --------
 
@@ -71,18 +54,14 @@
 pandas Primer
 -------------
 
 The pandas DataFrame (and hence SarracenDataFrame) is a swiss army knife of data manipulation. Columns in the data frame can be combined together mathematically, new columns assigned with little effort, and subsets of data extracted with a straightforward API.
 
 The below will compute the magnitude of the velocity and store the result as a new column in the data frame. Note the use of numpy.
 
-.. code-block::
-
-   sdf['vmag'] = np.sqrt(sdf['vx']**2 + sdf['vy']**2 + sdf['vz']**2)
+>>> sdf['vmag'] = np.sqrt(sdf['vx']**2 + sdf['vy']**2 + sdf['vz']**2)
 
 Extracting subsets of data can be done using boolean logic to slice into the data frame. The example below computes the average speed of particles above a certain critical density threshold. The first set of square brackets will return a `copy` of the data frame containing only the particles that have density greater than ``rho_crit``, while the second square brackets accesses the column ``vmag`` of that copy.
 
-.. code-block::
-
-   rho_crit = 1.0e10
-   sdf.calc_density()
-   sdf[sdf['rho'] > rho_crit]['vmag'].mean()
+>>> rho_crit = 1.0e10
+>>> sdf.calc_density()
+>>> sdf[sdf['rho'] > rho_crit]['vmag'].mean()
```

### Comparing `sarracen-1.1/docs/render.rst` & `sarracen-1.2.0/docs/render.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/pyproject.toml` & `sarracen-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/interpolate/base_backend.py` & `sarracen-1.2.0/sarracen/interpolate/base_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/interpolate/cpu_backend.py` & `sarracen-1.2.0/sarracen/interpolate/cpu_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,14 @@
             dz = np.float64(z_slice) - z_data
         else:
             dz = np.zeros(x_data.size)
 
         term = w_data / h_data ** n_dims
 
         output_local = np.zeros((get_num_threads(), y_pixels, x_pixels))
-        # normalization_local = None
-        # if normalize:
-            # normalization_local = np.zeros((get_num_threads(), y_pixels, x_pixels))
 
         # thread safety: each thread has its own grid, which are combined after interpolation
         for thread in prange(get_num_threads()):
             block_size = x_data.size / get_num_threads()
             range_start = int(thread * block_size)
             range_end = int((thread + 1) * block_size)
 
@@ -163,16 +160,14 @@
 
                 for jpix in range(jpixmax - jpixmin):
                     for ipix in range(ipixmax - ipixmin):
                         if np.sqrt(q2[jpix][ipix]) > kernel_radius:
                             continue
                         wab = weight_function(np.sqrt(q2[jpix][ipix]), n_dims)
                         output_local[thread][jpix + jpixmin, ipix + ipixmin] += term[i] * wab
-                        # if normalize:
-                        #     normalization_local[thread][jpix + jpixmin, ipix + ipixmin] +=
 
         for i in range(get_num_threads()):
             output += output_local[i]
 
         return output
 
     # Underlying CPU numba-compiled code for exact interpolation of 2D data to a 2D grid.
@@ -190,18 +185,18 @@
             range_start = int(thread * block_size)
             range_end = int((thread + 1) * block_size)
 
             # iterate through the indexes of non-filtered particles
             for i in range(range_start, range_end):
 
                 # determine maximum and minimum pixels that this particle contributes to
-                ipixmin = int(np.rint((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx))
-                jpixmin = int(np.rint((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy))
-                ipixmax = int(np.rint((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx))
-                jpixmax = int(np.rint((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy))
+                ipixmin = int(np.floor((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx))
+                jpixmin = int(np.floor((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy))
+                ipixmax = int(np.ceil((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx))
+                jpixmax = int(np.ceil((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy))
 
                 if ipixmax < 0 or ipixmin >= x_pixels or jpixmax < 0 or jpixmin >= y_pixels:
                     continue
                 if ipixmin < 0:
                     ipixmin = 0
                 if ipixmax > x_pixels:
                     ipixmax = x_pixels
@@ -436,18 +431,18 @@
             range_start = int(thread * block_size)
             range_end = int((thread + 1) * block_size)
 
             # iterate through the indexes of non-filtered particles
             for i in range(range_start, range_end):
 
                 # determine maximum and minimum pixels that this particle contributes to
-                ipixmin = int(np.rint((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx))
-                jpixmin = int(np.rint((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy))
-                ipixmax = int(np.rint((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx))
-                jpixmax = int(np.rint((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy))
+                ipixmin = int(np.floor((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx))
+                jpixmin = int(np.floor((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy))
+                ipixmax = int(np.ceil((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx))
+                jpixmax = int(np.ceil((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy))
 
                 # The width of the z contribution of this particle.
                 # = 2 * kernel_radius * h[i], where kernel_radius is 2 for the cubic spline kernel.
                 pixwidthz = 4 * h_data[i]
 
                 if ipixmax < 0 or ipixmin >= x_pixels or jpixmax < 0 or jpixmin >= y_pixels:
                     continue
```

### Comparing `sarracen-1.1/sarracen/interpolate/gpu_backend.py` & `sarracen-1.2.0/sarracen/interpolate/gpu_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,18 +197,18 @@
         @cuda.jit
         def _2d_func(x_data, y_data, w_data, h_data, image):
             i = cuda.grid(1)
             if i < len(x_data):
                 term = w_data[i] / h_data[i] ** 2
 
                 # determine maximum and minimum pixels that this particle contributes to
-                ipixmin = round((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx)
-                jpixmin = round((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy)
-                ipixmax = round((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx)
-                jpixmax = round((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy)
+                ipixmin = math.floor((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx)
+                jpixmin = math.floor((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy)
+                ipixmax = math.ceil((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx)
+                jpixmax = math.ceil((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy)
 
                 if ipixmax < 0 or ipixmin >= x_pixels or jpixmax < 0 or jpixmin >= y_pixels:
                     return
                 if ipixmin < 0:
                     ipixmin = 0
                 if ipixmax > x_pixels:
                     ipixmax = x_pixels
@@ -463,18 +463,18 @@
         def _3d_func(x_data, y_data, w_data, h_data, image):
             i = cuda.grid(1)
             if i < len(x_data):
                 dfac = h_data[i] ** 3 / (pixwidthx * pixwidthy * norm3d)
                 term = norm3d * w_data[i] / h_data[i] ** 3
 
                 # determine maximum and minimum pixels that this particle contributes to
-                ipixmin = round((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx)
-                jpixmin = round((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy)
-                ipixmax = round((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx)
-                jpixmax = round((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy)
+                ipixmin = math.floor((x_data[i] - 2 * h_data[i] - x_min) / pixwidthx)
+                jpixmin = math.floor((y_data[i] - 2 * h_data[i] - y_min) / pixwidthy)
+                ipixmax = math.ceil((x_data[i] + 2 * h_data[i] - x_min) / pixwidthx)
+                jpixmax = math.ceil((y_data[i] + 2 * h_data[i] - y_min) / pixwidthy)
 
                 # The width of the z contribution of this particle.
                 # = 2 * kernel_radius * h[i], where kernel_radius is 2 for the cubic spline kernel.
                 pixwidthz = 4 * h_data[i]
 
                 if ipixmax < 0 or ipixmin >= x_pixels or jpixmax < 0 or jpixmin >= y_pixels:
                     return
```

### Comparing `sarracen-1.1/sarracen/interpolate/interpolate.py` & `sarracen-1.2.0/sarracen/interpolate/interpolate.py`

 * *Files 5% similar despite different names*

```diff
@@ -337,19 +337,32 @@
     mass_data = _get_mass(data)
     if dens_weight:
         return target_data * mass_data
     else:
         rho_data = _get_density(data)
         return target_data * mass_data / rho_data
 
+def _get_smoothing_lengths(data: 'SarracenDataFrame', hmin: float, x_pixels: int, y_pixels: int,
+                           xlim: Tuple[float, float], ylim: Tuple[float, float]):
+    """ Return the smoothing length data, imposing a minimum length if hmin is True. """
+    
+    if hmin:
+        pix_size = (xlim[1] - xlim[0]) / x_pixels
+        pix_size = np.maximum(pix_size, (ylim[1] - ylim[0]) / y_pixels)
+        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+    else:
+        h_data = data[data._hcol].to_numpy()
+
+    return h_data
+
 
 def interpolate_2d(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, kernel: BaseKernel = None,
                    x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
-                   ylim: Tuple[float, float] = None, exact: bool = False,
-                   backend: str = None, dens_weight: bool = False, normalize: bool = True) -> np.ndarray:
+                   ylim: Tuple[float, float] = None, exact: bool = False, backend: str = None,
+                   dens_weight: bool = False, normalize: bool = True, hmin: bool = False) -> np.ndarray:
     """
     Interpolate particle data across two directional axes to a 2D grid of pixels.
 
     Interpolate the data within a SarracenDataFrame to a 2D grid, by interpolating the values
     of a target variable. The contributions of all particles near the interpolation area are
     summed and stored to a 2D grid.
 
@@ -371,14 +384,17 @@
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     ndarray (2-Dimensional)
         The interpolated output image, in a 2-dimensional numpy array. Dimensions are
         structured in reverse order, where (x, y) -> [y, x].
 
@@ -400,33 +416,35 @@
     x_pixels, y_pixels = _set_pixels(x_pixels, y_pixels, xlim, ylim)
     _check_boundaries(x_pixels, y_pixels, xlim, ylim)
     w_data = _get_weight(data, target, dens_weight)
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
+
     grid = get_backend(backend). \
-           interpolate_2d_render(data[x].to_numpy(), data[y].to_numpy(), w_data, data[data._hcol].to_numpy(), kernel.w,
+           interpolate_2d_render(data[x].to_numpy(), data[y].to_numpy(), w_data, h_data, kernel.w,
                               kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1], exact)
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend). \
-                    interpolate_2d_render(data[x].to_numpy(), data[y].to_numpy(), w_norm, data[data._hcol].to_numpy(),
+                    interpolate_2d_render(data[x].to_numpy(), data[y].to_numpy(), w_norm, h_data,
                                           kernel.w, kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0],
                                           ylim[1], exact)
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
 
 
 def interpolate_2d_vec(data: 'SarracenDataFrame', target_x: str, target_y: str, x: str = None, y: str = None,
                        kernel: BaseKernel = None, x_pixels: int = None, y_pixels: int = None,
                        xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None, exact: bool = False,
-                       backend: str = None, dens_weight: bool = False, normalize: bool = True):
+                       backend: str = None, dens_weight: bool = False, normalize: bool = True, hmin: bool = False):
     """
     Interpolate vector particle data across two directional axes to a 2D grid of particles.
 
     Interpolate the data within a SarracenDataFrame to a 2D grid, by interpolating the values
     of a target vector. The contributions of all vectors near the interpolation area are
     summed and stored to a 2D grid.
 
@@ -448,14 +466,17 @@
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     output_x, output_y: ndarray (2-Dimensional)
         The interpolated output images, in a 2-dimensional numpy arrays. Dimensions are
         structured in reverse order, where (x, y) -> [y, x].
 
@@ -476,40 +497,41 @@
     xlim, ylim = _snap_boundaries(data, x, y, xlim, ylim)
     x_pixels, y_pixels = _set_pixels(x_pixels, y_pixels, xlim, ylim)
     _check_boundaries(x_pixels, y_pixels, xlim, ylim)
 
     wx_data = _get_weight(data, target_x, dens_weight)
     wy_data = _get_weight(data, target_y, dens_weight)
 
-
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
+
     gridx, gridy = get_backend(backend).\
-           interpolate_2d_render_vec(data[x].to_numpy(), data[y].to_numpy(), wx_data, wy_data, data['h'].to_numpy(),
+           interpolate_2d_render_vec(data[x].to_numpy(), data[y].to_numpy(), wx_data, wy_data, h_data,
                                      kernel.w, kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0],
                                      ylim[1], exact)
 
     if normalize:
         wx_norm = _get_weight(data, np.array([1] * len(wx_data)), dens_weight)
         wy_norm = _get_weight(data, np.array([1] * len(wy_data)), dens_weight)
         norm_gridx, norm_gridy = get_backend(backend).\
                                  interpolate_2d_render_vec(data[x].to_numpy(), data[y].to_numpy(), wx_norm, wy_norm,
-                                                           data['h'].to_numpy(), kernel.w, kernel.get_radius(),
+                                                           h_data, kernel.w, kernel.get_radius(),
                                                            x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1],
                                                            exact)
         gridx = np.nan_to_num(gridx / norm_gridx)
         gridy = np.nan_to_num(gridy / norm_gridy)
 
     return (gridx, gridy)
 
 def interpolate_2d_line(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None,
                         kernel: BaseKernel = None, pixels: int = None, xlim: Tuple[float, float] = None,
                         ylim: Tuple[float, float] = None, backend: str = None, dens_weight: bool = False,
-                        normalize: bool = True) -> np.ndarray:
+                        normalize: bool = True, hmin: bool = False) -> np.ndarray:
     """
     Interpolate particle data across two directional axes to a 1D cross-section line.
 
     Interpolate the data within a SarracenDataFrame to a 1D line, by interpolating the values
     of a target variable. The contributions of all particles near the specified line are
     summed and stored to a 1-dimensional array.
 
@@ -528,14 +550,17 @@
     xlim, ylim: tuple of float, optional
         Starting and ending coordinates of the cross-section line (in particle data space). Defaults to
         the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     np.ndarray (1-Dimensional)
         The resulting interpolated output.
 
     Raises
@@ -566,32 +591,38 @@
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
     pixels = pixels if pixels is not None else 512
 
     if pixels <= 0:
         raise ValueError('pixcount must be greater than zero!')
 
+    if hmin:
+        pix_size = np.sqrt((xlim[1] - xlim[0])**2 + (ylim[1] - ylim[0])**2) / pixels
+        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+    else:
+        h_data = data[data._hcol].to_numpy()
+
     grid = get_backend(backend).\
-           interpolate_2d_cross(data[x].to_numpy(), data[y].to_numpy(), w_data, data['h'].to_numpy(), kernel.w,
+           interpolate_2d_cross(data[x].to_numpy(), data[y].to_numpy(), w_data, h_data, kernel.w,
                                 kernel.get_radius(), pixels, xlim[0], xlim[1], ylim[0], ylim[1])
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend). \
-                    interpolate_2d_cross(data[x].to_numpy(), data[y].to_numpy(), w_norm, data['h'].to_numpy(),
+                    interpolate_2d_cross(data[x].to_numpy(), data[y].to_numpy(), w_norm, h_data,
                                          kernel.w, kernel.get_radius(), pixels, xlim[0], xlim[1], ylim[0], ylim[1])
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
 
 
 def interpolate_3d_line(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
                         kernel: BaseKernel = None, pixels: int = None, xlim: Tuple[float, float] = None,
                         ylim: Tuple[float, float] = None, zlim: Tuple[float, float] = None, backend: str = None,
-                        dens_weight: bool = False, normalize: bool = True):
+                        dens_weight: bool = False, normalize: bool = True, hmin: bool = False):
     """
     Interpolate vector particle data across three directional axes to a 1D line.
 
     Interpolate the data within a SarracenDataFrame to a 1D line, by interpolating the values
     of a target variable. The contributions of all particles near the interpolation line are
     summed and stored to a 1D array.
 
@@ -611,14 +642,17 @@
     xlim, ylim, zlim: tuple of float, optional
         Starting and ending coordinates of the cross-section line (in particle data space). Defaults to
         the minimum and maximum values of `x`, `y`, and `z`.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
        If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     output: ndarray (1-Dimensional)
         The interpolated output line.
 
     Raises
@@ -659,35 +693,41 @@
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     if pixels <= 0:
         raise ValueError('pixcount must be greater than zero!')
 
+    if hmin:
+        pix_size = np.sqrt((xlim[1] - xlim[0])**2 + (ylim[1] - ylim[0])**2 + (zlim[1] - zlim[0])**2) / pixels
+        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+    else:
+        h_data = data[data._hcol].to_numpy()
+
     grid = get_backend(backend) \
-           .interpolate_3d_line(data[x].to_numpy(), data[y].to_numpy(), data[z].to_numpy(), w_data, data['h'].to_numpy(),
+           .interpolate_3d_line(data[x].to_numpy(), data[y].to_numpy(), data[z].to_numpy(), w_data, h_data,
                                 kernel.w, kernel.get_radius(), pixels, xlim[0], xlim[1], ylim[0], ylim[1], zlim[0],
                                 zlim[1])
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend) \
                     .interpolate_3d_line(data[x].to_numpy(), data[y].to_numpy(), data[z].to_numpy(), w_norm,
-                                         data['h'].to_numpy(), kernel.w, kernel.get_radius(), pixels, xlim[0], xlim[1],
+                                         h_data, kernel.w, kernel.get_radius(), pixels, xlim[0], xlim[1],
                                          ylim[0], ylim[1], zlim[0], zlim[1])
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
 
 
 def interpolate_3d_proj(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, kernel: BaseKernel = None,
                    integral_samples: int = 1000, rotation: np.ndarray = None, origin: np.ndarray = None,
                    x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                    ylim: Tuple[float, float] = None, exact: bool = False, backend: str = None,
-                   dens_weight: bool = None, normalize: bool = True):
+                   dens_weight: bool = None, normalize: bool = True, hmin: bool = False):
     """
     Interpolate 3D particle data to a 2D grid of pixels.
 
     Interpolates three-dimensional particle data in a SarracenDataFrame. The data
     is interpolated to a 2D grid of pixels, by summing contributions in columns which
     span the z-axis.
 
@@ -718,14 +758,17 @@
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to True for column-integrated views,
         when the target is not density, and False for everything else.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     ndarray (2-Dimensional)
         The interpolated output image, in a 2-dimensional numpy array. Dimensions are
         structured in reverse order, where (x, y) -> [y, x].
 
@@ -759,33 +802,36 @@
 
     x_data, y_data, z_data = _rotate_xyz(data, x, y, z, rotation, origin)
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     weight_function = kernel.get_column_kernel_func(integral_samples)
 
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
+
     grid = get_backend(backend) \
-           .interpolate_3d_projection(x_data, y_data, z_data, w_data, data['h'].to_numpy(), weight_function,
+           .interpolate_3d_projection(x_data, y_data, z_data, w_data, h_data, weight_function,
                                   kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1], exact)
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend) \
-                    .interpolate_3d_projection(x_data, y_data, z_data, w_norm, data['h'].to_numpy(), weight_function,
+                    .interpolate_3d_projection(x_data, y_data, z_data, w_norm, h_data, weight_function,
                                               kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0],
                                               ylim[1], exact)
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
 
 def interpolate_3d_vec(data: 'SarracenDataFrame', target_x: str, target_y: str, target_z: str, x: str = None,
                        y: str = None, kernel: BaseKernel = None, integral_samples: int = 1000,
                        rotation: np.ndarray = None, origin: np.ndarray = None, x_pixels: int = None,
                        y_pixels: int = None, xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None,
-                       exact: bool = False, backend: str = None, dens_weight: bool = False, normalize: bool = True):
+                       exact: bool = False, backend: str = None, dens_weight: bool = False, normalize: bool = True,
+                       hmin: bool = False):
     """
     Interpolate 3D vector particle data to a 2D grid of pixels.
 
     Interpolates three-dimensional vector particle data in a SarracenDataFrame. The data
     is interpolated to a 2D grid of pixels, by summing contributions in columns which
     span the z-axis.
 
@@ -815,14 +861,17 @@
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     output_x, output_y: ndarray (2-Dimensional)
         The interpolated output images. Dimensions are structured in reverse order, where (x, y) -> [y, x].
 
     Raises
@@ -852,42 +901,43 @@
     x_data, y_data, _ = _rotate_xyz(data, x, y, z, rotation, origin)
     if target_z not in data.columns:
         raise KeyError(f"z-directional target column '{target_z}' does not exist in the provided dataset.")
     target_x_data, target_y_data, _ = _rotate_data(data, target_x, target_y, target_z, rotation, origin)
 
     wx_data = _get_weight(data, target_x_data, dens_weight)
     wy_data = _get_weight(data, target_y_data, dens_weight)
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     weight_function = kernel.get_column_kernel_func(integral_samples)
     gridx, gridy = get_backend(backend) \
-                   .interpolate_3d_projection_vec(x_data, y_data, wx_data, wy_data, data['h'].to_numpy(),
+                   .interpolate_3d_projection_vec(x_data, y_data, wx_data, wy_data, h_data,
                                                   weight_function, kernel.get_radius(), x_pixels, y_pixels, xlim[0],
                                                   xlim[1], ylim[0], ylim[1], exact)
     if normalize:
         wx_norm = _get_weight(data, np.array([1] * len(wx_data)), dens_weight)
         wy_norm = _get_weight(data, np.array([1] * len(wy_data)), dens_weight)
         norm_gridx, norm_gridy = get_backend(backend) \
-                    .interpolate_3d_projection_vec(x_data, y_data, wx_norm, wy_norm, data['h'].to_numpy(),
+                    .interpolate_3d_projection_vec(x_data, y_data, wx_norm, wy_norm, h_data,
                                                   weight_function, kernel.get_radius(), x_pixels, y_pixels, xlim[0],
                                                   xlim[1], ylim[0], ylim[1], exact)
         gridx = np.nan_to_num(gridx / norm_gridx)
         gridy = np.nan_to_num(gridy / norm_gridy)
 
     return (gridx, gridy)
 
 
 
 def interpolate_3d_cross(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
                          z_slice: float = None, kernel: BaseKernel = None, rotation: np.ndarray = None,
                          origin: np.ndarray = None, x_pixels: int = None, y_pixels: int = None,
                          xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None, backend: str = None,
-                         dens_weight: bool = False, normalize: bool = True):
+                         dens_weight: bool = False, normalize: bool = True, hmin: bool = False):
     """
     Interpolate 3D particle data to a 2D grid, using a 3D cross-section.
 
     Interpolates particle data in a SarracenDataFrame across three directional axes to a 2D
     grid of pixels. A cross-section is taken of the 3D data at a specific value of z, and
     the contributions of particles near the plane are interpolated to a 2D grid.
 
@@ -916,14 +966,17 @@
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     ndarray (2-Dimensional)
         The interpolated output image, in a 2-dimensional numpy array. Dimensions are
         structured in reverse order, where (x, y) -> [y, x].
 
@@ -954,35 +1007,36 @@
     x_pixels, y_pixels = _set_pixels(x_pixels, y_pixels, xlim, ylim)
     _check_boundaries(x_pixels, y_pixels, xlim, ylim)
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     x_data, y_data, z_data = _rotate_xyz(data, x, y, z, rotation, origin)
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
 
     grid = get_backend(backend) \
-           .interpolate_3d_cross(x_data, y_data, z_data, z_slice, w_data, data['h'].to_numpy(), kernel.w,
+           .interpolate_3d_cross(x_data, y_data, z_data, z_slice, w_data, h_data, kernel.w,
                               kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1])
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend) \
-                    .interpolate_3d_cross(x_data, y_data, z_data, z_slice, w_norm, data['h'].to_numpy(), kernel.w,
+                    .interpolate_3d_cross(x_data, y_data, z_data, z_slice, w_norm, h_data, kernel.w,
                                           kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1])
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
 
 
 def interpolate_3d_cross_vec(data: 'SarracenDataFrame', target_x: str, target_y: str, target_z: str,
                              z_slice: float = None, x: str = None, y: str = None, z: str = None,
                              kernel: BaseKernel = None, rotation: np.ndarray = None, origin: np.ndarray = None,
                              x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                              ylim: Tuple[float, float] = None, backend: str = None, dens_weight: bool = False,
-                             normalize: bool = True):
+                             normalize: bool = True, hmin: bool = False):
     """
     Interpolate 3D vector particle data to a 2D grid, using a 3D cross-section.
 
     Interpolates vector particle data in a SarracenDataFrame across three directional axes to a 2D
     grid of pixels. A cross-section is taken of the 3D data at a specific value of z, and
     the contributions of vectors near the plane are interpolated to a 2D grid.
 
@@ -1011,14 +1065,17 @@
     xlim, ylim: float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     output_x, output_y: ndarray (2-Dimensional)
         The interpolated output images. Dimensions are structured in reverse order, where (x, y) -> [y, x].
 
     Raises
@@ -1045,42 +1102,43 @@
     _check_boundaries(x_pixels, y_pixels, xlim, ylim)
 
     x_data, y_data, z_data = _rotate_xyz(data, x, y, z, rotation, origin)
     target_x_data, target_y_data, _ = _rotate_data(data, target_x, target_y, target_z, rotation, origin)
 
     wx_data = _get_weight(data, target_x_data, dens_weight)
     wy_data = _get_weight(data, target_y_data, dens_weight)
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     gridx, gridy = get_backend(backend) \
-                   .interpolate_3d_cross_vec(x_data, y_data, z_data, z_slice, wx_data, wy_data, data['h'].to_numpy(),
+                   .interpolate_3d_cross_vec(x_data, y_data, z_data, z_slice, wx_data, wy_data, h_data,
                                              kernel.w, kernel.get_radius(), x_pixels, y_pixels, xlim[0], xlim[1],
                                              ylim[0], ylim[1])
 
     if normalize:
         wx_norm = _get_weight(data, np.array([1] * len(wx_data)), dens_weight)
         wy_norm = _get_weight(data, np.array([1] * len(wy_data)), dens_weight)
         norm_gridx, norm_gridy = get_backend(backend) \
                                  .interpolate_3d_cross_vec(x_data, y_data, z_data, z_slice, wx_norm, wy_norm,
-                                                           data['h'].to_numpy(), kernel.w, kernel.get_radius(),
+                                                           h_data, kernel.w, kernel.get_radius(),
                                                            x_pixels, y_pixels, xlim[0], xlim[1], ylim[0], ylim[1])
         gridx = np.nan_to_num(gridx / norm_gridx)
         gridy = np.nan_to_num(gridy / norm_gridy)
 
     return (gridx, gridy)
 
 
 def interpolate_3d_grid(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
                         kernel: BaseKernel = None, rotation: np.ndarray = None, rot_origin: np.ndarray = None,
                         x_pixels: int = None, y_pixels: int = None, z_pixels: int = None,
                         xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None,
                         zlim: Tuple[float, float] = None, backend: str = None, dens_weight: bool = False,
-                        normalize: bool = True):
+                        normalize: bool = True, hmin: bool = False):
     """
     Interpolate 3D particle data to a 3D grid of pixels
 
     Interpolates particle data in a SarracenDataFrame across three directional axes to a 3D
     grid of pixels. The contributions of all particles near each 3D cell are summed and
     stored in the 3D grid.
 
@@ -1107,14 +1165,17 @@
     xlim, ylim, zlim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x`, `y` and `z`.
     backend: ['cpu', 'gpu']
         The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
     -------
     ndarray (3-Dimensional)
         The interpolated output image, in a 3-dimensional numpy array. Dimensions are structured in reverse order,
         where (x, y, z) -> [z, y, x].
 
@@ -1149,23 +1210,24 @@
     if z_pixels <= 0:
         raise ValueError("`z_pixels` must be greater than zero!")
 
     kernel = kernel if kernel is not None else data.kernel
     backend = backend if backend is not None else data.backend
 
     x_data, y_data, z_data = _rotate_xyz(data, x, y, data.zcol, rotation, rot_origin)
+    h_data = _get_smoothing_lengths(data, hmin, x_pixels, y_pixels, xlim, ylim)
 
     grid = get_backend(backend) \
-           .interpolate_3d_grid(x_data, y_data, z_data, w_data, data['h'].to_numpy(), kernel.w, kernel.get_radius(),
+           .interpolate_3d_grid(x_data, y_data, z_data, w_data, h_data, kernel.w, kernel.get_radius(),
                                 x_pixels, y_pixels, z_pixels, xlim[0], xlim[1], ylim[0], ylim[1], zlim[0], zlim[1])
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
         norm_grid = get_backend(backend) \
-                    .interpolate_3d_grid(x_data, y_data, z_data, w_norm, data['h'].to_numpy(), kernel.w,
+                    .interpolate_3d_grid(x_data, y_data, z_data, w_norm, h_data, kernel.w,
                                          kernel.get_radius(), x_pixels, y_pixels, z_pixels, xlim[0], xlim[1],
                                          ylim[0], ylim[1], zlim[0], zlim[1])
         grid = np.nan_to_num(grid / norm_grid)
 
     return grid
```

### Comparing `sarracen-1.1/sarracen/kernels/base_kernel.py` & `sarracen-1.2.0/sarracen/kernels/base_kernel.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/kernels/cubic_spline.py` & `sarracen-1.2.0/sarracen/kernels/cubic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/kernels/cubic_spline_exact.py` & `sarracen-1.2.0/sarracen/kernels/cubic_spline_exact.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/kernels/quartic_spline.py` & `sarracen-1.2.0/sarracen/kernels/quartic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/kernels/quintic_spline.py` & `sarracen-1.2.0/sarracen/kernels/quintic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/readers/read_csv.py` & `sarracen-1.2.0/sarracen/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/readers/read_marisa.py` & `sarracen-1.2.0/sarracen/readers/read_marisa.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/readers/read_phantom.py` & `sarracen-1.2.0/sarracen/readers/read_phantom.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/render.py` & `sarracen-1.2.0/sarracen/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 def render(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
            xsec: Union[float, bool] = None, kernel: BaseKernel = None, x_pixels: int = None, y_pixels: int = None,
            xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None, cmap: Union[str, Colormap] = 'gist_heat',
            cbar: bool = True, cbar_kws: dict = {}, cbar_ax: Axes = None, ax: Axes = None, exact: bool = None,
            backend: str = None, integral_samples: int = 1000, rotation: np.ndarray = None,
            rot_origin: np.ndarray = None, log_scale: bool = False, dens_weight: bool = None, normalize: bool = True,
-           **kwargs) -> Axes:
+           hmin: bool = False, **kwargs) -> Axes:
     """
     Render a scalar SPH target variable to a grid plot.
 
     Parameters
     ----------
     data : SarracenDataFrame
         Particle data, in a SarracenDataFrame.
@@ -177,14 +177,17 @@
     log_scale: bool
         Whether to use a logarithmic scale for color coding.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to True for column-integrated views,
         when the target is not density, and False for everything else.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
     kwargs: other keyword arguments
         Keyword arguments to pass to ax.imshow.
 
     Returns
     -------
     Axes
         The resulting matplotlib axes, which contain the 2d rendered image.
@@ -247,21 +250,21 @@
             if dens_weight is None:
                 dens_weight = False
         else:
             interpolation_type = '3d'
 
     if interpolation_type == '2d':
         img = interpolate_2d(data, target, x, y, kernel, x_pixels, y_pixels, xlim, ylim, exact, backend, dens_weight,
-                             normalize)
+                             normalize, hmin)
     elif interpolation_type == '3d_cross':
         img = interpolate_3d_cross(data, target, x, y, z, xsec, kernel, rotation,
-                                   rot_origin, x_pixels, y_pixels, xlim, ylim, backend, dens_weight, normalize)
+                                   rot_origin, x_pixels, y_pixels, xlim, ylim, backend, dens_weight, normalize, hmin)
     elif interpolation_type == '3d':
         img = interpolate_3d_proj(data, target, x, y, kernel, integral_samples, rotation, rot_origin, x_pixels,
-                             y_pixels, xlim, ylim, exact, backend, dens_weight, normalize)
+                             y_pixels, xlim, ylim, exact, backend, dens_weight, normalize, hmin)
     else:
         raise ValueError('`data` is not a valid number of dimensions.')
 
     if ax is None:
         ax = plt.gca()
 
     x, y = _default_axes(data, x, y)
@@ -291,15 +294,15 @@
 
     return ax
 
 
 def lineplot(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
              kernel: BaseKernel = None, pixels: int = 512, xlim: Tuple[float, float] = None,
              ylim: Tuple[float, float] = None, zlim: Tuple[float, float] = None, ax: Axes = None, backend: str = None,
-             log_scale: bool = False, dens_weight: bool = False, normalize: bool = True, **kwargs):
+             log_scale: bool = False, dens_weight: bool = False, normalize: bool = True, hmin: bool = False, **kwargs):
     """
     Render a scalar SPH target variable to line plot.
 
     Parameters
     ----------
     data : SarracenDataFrame
         Particle data, in a SarracenDataFrame.
@@ -320,14 +323,17 @@
         specified in `data`.
     log_scale: bool
         Whether to use a logarithmic scale for color coding.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to False.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
     kwargs: other keyword arguments
         Keyword arguments to pass to sns.lineplot.
 
     Returns
     -------
     Axes
         The resulting matplotlib axes, which contain the 2d rendered image.
@@ -339,18 +345,19 @@
         if the specified `x` and `y` minimum and maximums result in an invalid region.
     KeyError
         If `target`, `x`, `y`, mass, density, or smoothing length columns do not
         exist in `data`.
     """
 
     if data.get_dim() == 2:
-        img = interpolate_2d_line(data, target, x, y, kernel, pixels, xlim, ylim, backend, dens_weight, normalize)
+        img = interpolate_2d_line(data, target, x, y, kernel, pixels, xlim, ylim, backend, dens_weight, normalize,
+                                  hmin)
     else:
         img = interpolate_3d_line(data, target, x, y, z, kernel, pixels, xlim, ylim, zlim, backend, dens_weight,
-                                  normalize)
+                                  normalize, hmin)
 
     if isinstance(xlim, float) or isinstance(xlim, int):
         xlim = xlim, xlim
     if isinstance(ylim, float) or isinstance(ylim, int):
         ylim = ylim, ylim
 
     x, y = _default_axes(data, x, y)
@@ -396,15 +403,15 @@
 
 
 def streamlines(data: 'SarracenDataFrame', target: Union[Tuple[str, str], Tuple[str, str, str]], x: str = None,
                 y: str = None, z: str = None, xsec: int = None, kernel: BaseKernel = None,
                 integral_samples: int = 1000, rotation: np.ndarray = None, rot_origin: np.ndarray = None,
                 x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                 ylim: Tuple[float, float] = None, ax: Axes = None, exact: bool = None, backend: str = None,
-                dens_weight: bool = None, normalize: bool = True, **kwargs) -> Axes:
+                dens_weight: bool = None, normalize: bool = True, hmin: bool = False, **kwargs) -> Axes:
     """
     Create an SPH interpolated streamline plot of a target vector.
 
     Render the data within a SarracenDataFrame to a 2D matplotlib object, by rendering the values
     of a target vector. The contributions of all particles near the rendered area are summed and
     stored to a 2D grid for the x & y axes of the target vector. This data is then used to create
     a streamline plot using ax.streamlines().
@@ -442,14 +449,17 @@
     backend: ['cpu', 'gpu']
         The computation backend to use when rendering this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to True for column-integrated views
         and False for everything else.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
     kwargs: other keyword arguments
         Keyword arguments to pass to ax.streamlines()
 
     Returns
     -------
     Axes
         The resulting matplotlib axes, which contains the streamline plot.
@@ -478,21 +488,23 @@
         if xsec is not None:
             interpolation_type = '3d_cross'
         else:
             interpolation_type = '3d'
 
     if interpolation_type == '2d':
         img = interpolate_2d_vec(data, target[0], target[1], x, y, kernel, x_pixels, y_pixels, xlim, ylim, exact,
-                                 backend, dens_weight, normalize)
+                                 backend, dens_weight, normalize, hmin)
     elif interpolation_type == '3d_cross':
         img = interpolate_3d_cross_vec(data, target[0], target[1], target[2], xsec, x, y, z, kernel, rotation,
-                                       rot_origin, x_pixels, y_pixels, xlim, ylim, backend, dens_weight, normalize)
+                                       rot_origin, x_pixels, y_pixels, xlim, ylim, backend, dens_weight, normalize,
+                                       hmin)
     elif interpolation_type == '3d':
         img = interpolate_3d_vec(data, target[0], target[1], target[2], x, y, kernel, integral_samples, rotation,
-                                 rot_origin, x_pixels, y_pixels, xlim, ylim, exact, backend, dens_weight, normalize)
+                                 rot_origin, x_pixels, y_pixels, xlim, ylim, exact, backend, dens_weight, normalize,
+                                 hmin)
     else:
         raise ValueError('`data` is not a valid number of dimensions.')
 
     if ax is None:
         ax = plt.gca()
 
     x, y = _default_axes(data, x, y)
@@ -518,15 +530,16 @@
 
 
 def arrowplot(data: 'SarracenDataFrame', target: Union[Tuple[str, str], Tuple[str, str, str]], x: str = None,
               y: str = None, z: str = None, xsec: float = None, kernel: BaseKernel = None,
               integral_samples: int = 1000, rotation: np.ndarray = None, rot_origin: np.ndarray = None,
               x_arrows: int = None, y_arrows: int = None, xlim: Tuple[float, float] = None,
               ylim: Tuple[float, float] = None, ax: Axes = None, qkey: bool = True, qkey_kws=None, exact: bool = None,
-              backend: str = None, dens_weight: bool = None, normalize: bool = True, **kwargs) -> Axes:
+              backend: str = None, dens_weight: bool = None, normalize: bool = True, hmin: bool = False,
+              **kwargs) -> Axes:
     """
     Create an SPH interpolated vector field plot of a target vector.
 
     Render the data within a SarracenDataFrame to a 2D matplotlib object, by rendering the values
     of a target vector. The contributions of all particles near the rendered area are summed and
     stored to a 2D grid for the x & y axes of the target vector. This data is then used to create
     an arrow plot using ax.quiver().
@@ -567,14 +580,17 @@
     backend: ['cpu', 'gpu']
         The computation backend to use when rendering this data. Defaults to the backend specified in `data`.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to True for column-integrated views
         and False for everything else.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
+    hmin: bool
+        If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+        contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
     kwargs: other keyword arguments
         Keyword arguments to pass to ax.quiver()
 
     Returns
     -------
     Axes
         The resulting matplotlib axes, which contains the arrow plot.
@@ -606,21 +622,23 @@
         if xsec is not None:
             interpolation_type = '3d_cross'
         else:
             interpolation_type = '3d'
 
     if interpolation_type == '2d':
         img = interpolate_2d_vec(data, target[0], target[1], x, y, kernel, x_arrows, y_arrows, xlim, ylim, exact,
-                                 backend, dens_weight, normalize)
+                                 backend, dens_weight, normalize, hmin)
     elif interpolation_type == '3d_cross':
         img = interpolate_3d_cross_vec(data, target[0], target[1], target[2], xsec, x, y, z, kernel, rotation,
-                                       rot_origin, x_arrows, y_arrows, xlim, ylim, backend, dens_weight, normalize)
+                                       rot_origin, x_arrows, y_arrows, xlim, ylim, backend, dens_weight, normalize,
+                                       hmin)
     elif interpolation_type == '3d':
         img = interpolate_3d_vec(data, target[0], target[1], target[2], x, y, kernel, integral_samples, rotation,
-                                 rot_origin, x_arrows, y_arrows, xlim, ylim, exact, backend, dens_weight, normalize)
+                                 rot_origin, x_arrows, y_arrows, xlim, ylim, exact, backend, dens_weight, normalize,
+                                 hmin)
     else:
         raise ValueError('`data` is not a valid number of dimensions.')
 
 
     if ax is None:
         ax = plt.gca()
```

### Comparing `sarracen-1.1/sarracen/sarracen_dataframe.py` & `sarracen-1.2.0/sarracen/sarracen_dataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,82 @@
         func.__doc__ = copy_func.__doc__
         return func
     return wrapper
 
 
 class SarracenDataFrame(DataFrame):
     """
-    A pandas DataFrame which contains relevant data for SPH data visualizations.
+    A SarracenDataFrame is a pandas DataFrame with support for SPH data.
+
+    A SarracenDataFrame is a subclass of the pandas DataFrame class designed to hold SPH particle
+    data. Global simulation values are stored in ``params``, which is a standard Python dictionary.
+
+    Interpolation and rendering functionality requires (at a minimum) particle positions, smoothing
+    lengths and masses. SarracenDataFrames will attempt to identify columns which hold these data.
+    For uniform, constant mass particles, the particle mass can be specified in the ``params``
+    dictionary.
 
-    This is an extended version of the pandas DataFrame class, which contains several
-    derived parameters used in the `render.py` and `interpolate.py` modules. The labels
-    of columns containing x, y, and z directional data, and the labels of columns containing
-    mass, density, and smoothing length information are all stored. As well, the kernel
-    used for all interpolation operations, and the units for each data column.
-
-    See Also
-    --------
-    readers : Functions for creating SarracenDataFrame objects from exported SPH data.
     """
+
     _metadata = ['_params', '_units', '_xcol', '_ycol', '_zcol', '_hcol', '_mcol', '_rhocol', '_kernel']
 
     def __init__(self, data=None, params=None, *args, **kwargs):
         """
-        Create a new `SarracenDataFrame`, and automatically detect important columns.
+        Construct a SarracenDataFrame from a NumPy array, dictionary, DataFrame or Iterable object.
 
         Parameters
         ----------
-        data : ndarray (structured or homogeneous), Iterable, DataFrame, or dict.
-            Raw particle data passed to the DataFrame super-initializer.
-        params : dict
-            Miscellaneous dataset-level parameters.
-        *args : tuple
-            Additional arguments to the DataFrame super-initializer.
+        data : ndarray, Iterable, DataFrame, or dict.
+            Raw particle data which is passed to the pandas DataFrame constructor. Data can be specified
+            in a dictionary, NumPy array or another DataFrame.
+        params : dict, optional
+            Global parameters from the simulation (time, hfact, etc). If constant, uniform mass particles
+            are used, then the key ``mass`` stores the particle mass (rather than specifying per particle).
+        *args : tuple, optional
+            Additional arguments to pass to the pandas DataFrame constructor.
         **kwargs : dict, optional
-            Additional keyword arguments to the DataFrame super-initializer.
+            Additional keyword arguments to pass to the pandas DataFrame constructor.
+
+        See Also
+        --------
+        :func:`read_csv` : Read data from a comma separated values (csv) file.
+        :func:`read_phantom` : Read data from the Phantom SPH code.
+
+        Examples
+        --------
+        Constructing using a Python dictionary.
+
+        >>> particles = {'x': [1.0, 2.0, 3.0], 'y': [2.0, 2.0, 2.0], 'h': [3.0, 3.5, 4.0]}
+        >>> sdf = sarracen.SarracenDataFrame(particles)
+        >>> sdf
+            x     y     h
+        0   1.0   2.0   3.0
+        1   2.0   2.0   3.5
+        2   3.0   2.0   4.0
+
+        Constructing using a two-dimensional NumPy array.
+
+        >>> particles = np.array([[1.0, 2.0, 3.0], [2.0, 2.0, 3.5], [3.0, 2.0, 4.0]])
+        >>> sdf = sarracen.SarracenDataFrame(particles, columns=['x', 'y', 'h'])
+        >>> sdf
+            x     y     h
+        0   1.0   2.0   3.0
+        1   2.0   2.0   3.5
+        2   3.0   2.0   4.0
+
+        Constant mass particles can specify mass in the ``params`` dictionary, rather than per particle.
+
+        >>> particles = {'x': [1.0, 2.0, 3.0], 'y': [2.0, 2.0, 2.0], 'h': [3.0, 3.5, 4.0]}
+        >>> params = {'mass': 0.2, 'hfact': 1.2}
+        >>> sdf = sarracen.SarracenDataFrame(particles, params)
+        >>> sdf.params
+        {'mass': 0.2, 'hfact': 1.2}
+
         """
+
         # call pandas DataFrame constructor
         super().__init__(data, *args, **kwargs)
 
         if params is None:
             params = dict()
         self._params = None
         self.params = params
@@ -173,54 +212,56 @@
 
     @_copy_doc(render)
     def render(self, target: str, x: str = None, y: str = None, z: str = None, xsec: float = None,
                kernel: BaseKernel = None, x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                ylim: Tuple[float, float] = None, cmap: Union[str, Colormap] = 'gist_heat', cbar: bool = True,
                cbar_kws: dict = {}, cbar_ax: Axes = None, ax: Axes = None, exact: bool = None, backend: str = None,
                integral_samples: int = 1000, rotation: np.ndarray = None, rot_origin: np.ndarray = None,
-               log_scale: bool = None, dens_weight: bool = None, normalize: bool = False, **kwargs) -> Axes:
+               log_scale: bool = None, dens_weight: bool = None, normalize: bool = False, hmin: bool = False,
+               **kwargs) -> Axes:
         return render(self, target, x, y, z, xsec, kernel, x_pixels, y_pixels, xlim, ylim, cmap, cbar, cbar_kws,
                       cbar_ax, ax, exact, backend, integral_samples, rotation, rot_origin, log_scale, dens_weight,
-                      normalize, **kwargs)
+                      normalize, hmin, **kwargs)
 
     @_copy_doc(lineplot)
     def lineplot(self, target: str, x: str = None, y: str = None, z: str = None,
                  kernel: BaseKernel = None, pixels: int = 512, xlim: Tuple[float, float] = None,
                  ylim: Tuple[float, float] = None, zlim: Tuple[float, float] = None, ax: Axes = None,
                  backend: str = None, log_scale: bool = False, dens_weight: bool = None, normalize: bool = False,
-                 **kwargs):
+                 hmin: bool = False, **kwargs):
         return lineplot(self, target, x, y, z, kernel, pixels, xlim, ylim, zlim, ax, backend, log_scale, dens_weight,
-                        normalize, **kwargs)
+                        normalize, hmin, **kwargs)
 
     @_copy_doc(streamlines)
     def streamlines(self, target: Union[Tuple[str, str], Tuple[str, str, str]], x: str = None, y: str = None,
                     z: str = None, xsec: int = None, kernel: BaseKernel = None, integral_samples: int = 1000,
                     rotation: np.ndarray = None, rot_origin: np.ndarray = None, x_pixels: int = None,
                     y_pixels: int = None, xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None,
                     ax: Axes = None, exact: bool = None, backend: str = None, dens_weight: bool = False,
-                    normalize: bool = False, **kwargs) -> Axes:
+                    normalize: bool = False, hmin: bool = False, **kwargs) -> Axes:
         return streamlines(self, target, x, y, z, xsec, kernel, integral_samples, rotation, rot_origin, x_pixels,
-                           y_pixels, xlim, ylim, ax, exact, backend, dens_weight, normalize, **kwargs)
+                           y_pixels, xlim, ylim, ax, exact, backend, dens_weight, normalize, hmin, **kwargs)
 
     @_copy_doc(arrowplot)
     def arrowplot(self, target: Union[Tuple[str, str], Tuple[str, str, str]], x: str = None, y: str = None,
                   z: str = None, xsec: int = None, kernel: BaseKernel = None, integral_samples: int = 1000,
                   rotation: np.ndarray = None, rot_origin: np.ndarray = None, x_arrows: int = None,
                   y_arrows: int = None, xlim: Tuple[float, float] = None, ylim: Tuple[float, float] = None,
                   ax: Axes = None, qkey: bool = True, qkey_kws: dict = None, exact: bool = None, backend: str = None,
-                  dens_weight: bool = None, normalize: bool = False, **kwargs) -> Axes:
+                  dens_weight: bool = None, normalize: bool = False, hmin: bool = False, **kwargs) -> Axes:
         return arrowplot(self, target, x, y, z, xsec, kernel, integral_samples, rotation, rot_origin, x_arrows,
-                         y_arrows, xlim, ylim, ax, qkey, qkey_kws, exact, backend, dens_weight, normalize, **kwargs)
+                         y_arrows, xlim, ylim, ax, qkey, qkey_kws, exact, backend, dens_weight, normalize, hmin,
+                         **kwargs)
 
     def sph_interpolate(self, target: str, x: str = None, y: str = None, z: str = None, kernel: BaseKernel = None,
                         rotation: np.ndarray = None, rot_origin: np.ndarray = None, x_pixels: int = None,
                         y_pixels: int = None, z_pixels: int = None, xlim: Tuple[float, float] = None,
                         ylim: Tuple[float, float] = None, zlim: Tuple[float, float] = None,
                         exact: bool = None, backend: str = 'cpu', dens_weight: bool = False,
-                        normalize: bool = False) -> np.ndarray:
+                        normalize: bool = False, hmin: bool = False) -> np.ndarray:
         """
         Interpolate this data to a 2D or 3D grid, depending on the dimensionality of the data.
 
         Parameters
         ----------
         target: str
             The column label of the target data.
@@ -245,14 +286,17 @@
             Whether to use exact interpolation of the data. Only applies to 2D datasets.
         backend: ['cpu', 'gpu']
             The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
         dens_weight: bool
             If True, the target will be multiplied by density. Defaults to False.
         normalize: bool
             If True, will normalize the interpolation. Defaults to False (this may change in future versions).
+        hmin: bool
+            If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
+            contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
         Returns
         -------
         ndarray (n-Dimensional)
             The interpolated output image, in a multi-dimensional numpy array. The number of dimensions match the
             dimensions of the data. Dimensions are structured in reverse order, where (x, y, z) -> [z, y, x].
 
@@ -268,18 +312,18 @@
         """
         if self.get_dim() == 2:
             if xlim is None:
                 xlim = (None, None)
             if ylim is None:
                 ylim = (None, None)
             return interpolate_2d(self, target, x, y, kernel, x_pixels, y_pixels, xlim, ylim, exact, backend,
-                                  dens_weight, normalize)
+                                  dens_weight, normalize, hmin)
         elif self.get_dim() == 3:
             return interpolate_3d_grid(self, target, x, y, z, kernel, rotation, rot_origin, x_pixels, y_pixels,
-                                       z_pixels, xlim, ylim, zlim, backend, dens_weight, normalize)
+                                       z_pixels, xlim, ylim, zlim, backend, dens_weight, normalize, hmin)
 
     @property
     def params(self):
         """
         dict: Miscellaneous dataset-level parameters.
 
         Raises
```

### Comparing `sarracen-1.1/sarracen/tests/readers/test_read_csv.py` & `sarracen-1.2.0/sarracen/tests/readers/test_read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/tests/test_interpolate.py` & `sarracen-1.2.0/sarracen/tests/test_interpolate.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,86 +34,86 @@
     # Weight for 2D interpolation & 3D column interpolation.
     w = sdf['m'] / (sdf['rho'] * sdf['h'] ** 2)
 
     # A mapping of pixel indices to x / y values in particle space.
     real = -kernel.get_radius() + (np.arange(0, 25) + 0.5) * (2 * kernel.get_radius() / 25)
 
     image = interpolate_2d(sdf, 'A', x_pixels=25,  y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_2d_vec(sdf, 'A', 'B', x_pixels=25, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] ==\
                    approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] ==\
                    approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == \
                    approx(w[0] * sdf['B'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
 
     image = interpolate_2d_line(sdf, 'A', pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for x in range(25):
         assert image[x] == approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(2) * np.abs(real[x]) / sdf['h'][0], 2))
 
     # Convert the previous 2D dataframe to a 3D dataframe.
     sdf['z'] = -0.5
     sdf['C'] = 10
     sdf.zcol = 'z'
 
     column_func = kernel.get_column_kernel_func(1000)
 
     image = interpolate_3d_proj(sdf, 'A', x_pixels=25, y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     image_vec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=25, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] ==\
                    approx(w[0] * sdf['A'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] == \
                    approx(w[0] * sdf['A'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == \
                    approx(w[0] * sdf['B'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
 
     # Weight for 3D cross-sections.
     w = sdf['m'] / (sdf['rho'] * sdf['h'] ** 3)
 
     image = interpolate_3d_cross(sdf, 'A', z_slice=0, x_pixels=25, y_pixels=25,
                                  xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=25, y_pixels=25,
                                          xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == approx(w[0] * sdf['A'][0] *
                                          kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2) / sdf['h'][0], 3))
             assert image_vec[0][y][x] == approx(w[0] * sdf['A'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2)
                                                          / sdf['h'][0], 3))
             assert image_vec[1][y][x] == approx(w[0] * sdf['B'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2)
                                                          / sdf['h'][0], 3))
 
     bounds = (-kernel.get_radius(), kernel.get_radius())
     image = interpolate_3d_grid(sdf, 'A', x_pixels=25, y_pixels=25, z_pixels=25, xlim=bounds, ylim=bounds,
-                                zlim=bounds, normalize=False)
+                                zlim=bounds, normalize=False, hmin=False)
     for z in range(25):
         for y in range(25):
             for x in range(25):
                 assert image[z][y][x] == approx(w[0] * sdf['A'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + (real[z] + 0.5) ** 2)
                                                          / sdf['h'][0], 3))
 
     image = interpolate_3d_line(sdf, 'A', pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
                                 ylim=(-kernel.get_radius(), kernel.get_radius()),
-                                zlim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                zlim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for x in range(25):
         assert image[x] == approx(w[0] * sdf['A'][0] *
                                   kernel.w(np.sqrt(2 * real[x] ** 2 + (real[x] + 0.5) ** 2) / sdf['h'][0], 3))
 
 
 @mark.parametrize("backend", backends)
 def test_single_repeated_particle(backend):
@@ -136,86 +136,86 @@
     # Multiplying by repetitions here is done for ease of use.
     w = repetitions * sdf['m'] / (sdf['rho'] * sdf['h'] ** 2)
 
     # A mapping of pixel indices to x / y values in particle space.
     real = -kernel.get_radius() + (np.arange(0, 25) + 0.5) * (2 * kernel.get_radius() / 25)
 
     image = interpolate_2d(sdf, 'A', x_pixels=25, y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_2d_vec(sdf, 'A', 'B', x_pixels=25, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == \
                    approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] == \
                    approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == \
                    approx(w[0] * sdf['B'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
 
     image = interpolate_2d_line(sdf, 'A', pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for x in range(25):
         assert image[x] == approx(w[0] * sdf['A'][0] * kernel.w(np.sqrt(2) * np.abs(real[x]) / sdf['h'][0], 2))
 
     # Convert the previous 2D dataframe to a 3D dataframe.
     sdf['z'] = -0.5
     sdf['C'] = 10
     sdf.zcol = 'z'
 
     column_func = kernel.get_column_kernel_func(1000)
 
     image = interpolate_3d_proj(sdf, 'A', x_pixels=25, y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     image_vec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=25, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == \
                    approx(w[0] * sdf['A'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] == \
                    approx(w[0] * sdf['A'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == \
                    approx(w[0] * sdf['B'][0] * column_func(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf['h'][0], 2))
 
     # Weight for 3D cross-sections
     w = repetitions * sdf['m'] / (sdf['rho'] * sdf['h'] ** 3)
 
     image = interpolate_3d_cross(sdf, 'A', z_slice=0, x_pixels=25, y_pixels=25,
                                  xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=25, y_pixels=25,
                                          xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == approx(w[0] * sdf['A'][0] *
                                          kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2) / sdf['h'][0], 3))
             assert image_vec[0][y][x] == approx(w[0] * sdf['A'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2)
                                                          / sdf['h'][0], 3))
             assert image_vec[1][y][x] == approx(w[0] * sdf['B'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 0.5 ** 2)
                                                          / sdf['h'][0], 3))
 
     bounds = (-kernel.get_radius(), kernel.get_radius())
     image = interpolate_3d_grid(sdf, 'A', x_pixels=25, y_pixels=25, z_pixels=25, xlim=bounds, ylim=bounds, zlim=bounds,
-                                normalize=False)
+                                normalize=False, hmin=False)
     for z in range(25):
         for y in range(25):
             for x in range(25):
                 assert image[z][y][x] == approx(w[0] * sdf['A'][0] *
                                                 kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + (real[z] + 0.5) ** 2)
                                                          / sdf['h'][0], 3))
 
     image = interpolate_3d_line(sdf, 'A', pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
                                 ylim=(-kernel.get_radius(), kernel.get_radius()),
-                                zlim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                zlim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for x in range(25):
         assert image[x] == approx(w[0] * sdf['A'][0] *
                                   kernel.w(np.sqrt(2 * real[x] ** 2 + (real[x] + 0.5) ** 2) / sdf['h'][0], 3))
 
 
 @mark.parametrize("backend", backends)
 def test_dimension_check(backend):
@@ -226,30 +226,30 @@
     df = pd.DataFrame({'x': [0, 1], 'y': [0, 1], 'P': [1, 1], 'Ax': [1, 1], 'Ay': [1, 1], 'h': [1, 1],
                        'rho': [1, 1], 'm': [1, 1]})
     sdf = SarracenDataFrame(df, params=dict())
     sdf.backend = backend
 
     for func in [interpolate_3d_proj, interpolate_3d_cross]:
         with raises(TypeError):
-            func(sdf, 'P', normalize=False)
+            func(sdf, 'P', normalize=False, hmin=False)
     for func in [interpolate_3d_vec, interpolate_3d_cross_vec, interpolate_3d_grid]:
         with raises(TypeError):
-            func(sdf, 'Ax', 'Ay', 'Az', normalize=False)
+            func(sdf, 'Ax', 'Ay', 'Az', normalize=False, hmin=False)
 
     # Next, test a basic 3D dataframe passed to 2D interpolation functions.
     df = pd.DataFrame({'x': [0, 1], 'y': [0, 1], 'z': [0, 1], 'P': [1, 1], 'Ax': [1, 1], 'Ay': [1, 1], 'Az': [1, 1],
                        'h': [1, 1], 'rho': [1, 1], 'm': [1, 1]})
     sdf = SarracenDataFrame(df, params=dict())
     sdf.backend = backend
 
     for func in [interpolate_2d, interpolate_2d_line, interpolate_3d_line]:
         with raises(TypeError):
-            func(sdf, 'P', normalize=False)
+            func(sdf, 'P', normalize=False, hmin=False)
     with raises(TypeError):
-        interpolate_2d_vec(sdf, 'Ax', 'Ay', normalize=False)
+        interpolate_2d_vec(sdf, 'Ax', 'Ay', normalize=False, hmin=False)
 
 
 @mark.parametrize("backend", backends)
 def test_3d_xsec_equivalency(backend):
     """
     A single 3D column integration of a dataframe should be equivalent to the average of several evenly spaced 3D
     cross-sections.
@@ -260,26 +260,26 @@
     kernel = CubicSplineKernel()
     sdf.kernel = kernel
     sdf.backend = backend
 
     samples = 250
 
     column_image = interpolate_3d_proj(sdf, 'A', x_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                       dens_weight=False, normalize=False)
+                                       dens_weight=False, normalize=False, hmin=False)
     column_image_vec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                          dens_weight=False, normalize=False)
+                                          dens_weight=False, normalize=False, hmin=False)
 
     xsec_image = np.zeros((50, 50))
     xsec_image_vec = [np.zeros((50, 50)), np.zeros((50, 50))]
     for z in np.linspace(0, kernel.get_radius() * sdf['h'][0], samples):
         xsec_image += interpolate_3d_cross(sdf, 'A', z_slice=z, x_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                           normalize=False)
+                                           normalize=False, hmin=False)
 
         vec_sample = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', z, x_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                              normalize=False)
+                                              normalize=False, hmin=False)
         xsec_image_vec[0] += vec_sample[0]
         xsec_image_vec[1] += vec_sample[1]
 
     # Scale each cross-section summation to be equivalent to the column integration.
     xsec_image *= kernel.get_radius() * sdf['h'][0] * 2 / samples
     xsec_image_vec[0] *= kernel.get_radius() * sdf['h'][0] * 2 / samples
     xsec_image_vec[1] *= kernel.get_radius() * sdf['h'][0] * 2 / samples
@@ -301,22 +301,22 @@
     # returns zero for an unknown reason.
     df = pd.DataFrame({'x': [0], 'y': [0], 'A': [4], 'h': [0.9], 'rho': [0.4], 'm': [0.03]})
     sdf = SarracenDataFrame(df, params=dict())
     kernel = CubicSplineKernel()
     sdf.kernel = kernel
     sdf.backend = backend
 
-    true_image = interpolate_2d(sdf, 'A', x_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    true_image = interpolate_2d(sdf, 'A', x_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
 
     # A mapping of pixel indices to x & y values in particle space.
     real = -1 + (np.arange(0, 50) + 0.5) * (2 / 50)
 
     reconstructed_image = np.zeros((50, 50))
     for y in range(50):
-        reconstructed_image[y, :] = interpolate_2d_line(sdf, 'A', pixels=50, xlim=(-1, 1), ylim=(real[y], real[y]), normalize=False)
+        reconstructed_image[y, :] = interpolate_2d_line(sdf, 'A', pixels=50, xlim=(-1, 1), ylim=(real[y], real[y]), normalize=False, hmin=False)
     assert_allclose(reconstructed_image, true_image)
 
     # reconstructed_image = np.zeros((50, 50))
     # for x in range(50):
     #     reconstructed_image[:, x] = interpolate_2d_line(sdf, 'A', pixels=50, xlim=(real[x], real[x]), ylim=(-1, 1))
     # assert_allclose(reconstructed_image, true_image)
 
@@ -342,40 +342,40 @@
 
     # Weight for 2D interpolation, and 3D column interpolation.
     w = sdf_2['m'] / (sdf_2['rho'] * sdf_2['h'] ** 2)
 
     # A mapping of pixel indices to x / y values in particle space.
     real = (np.arange(0, 25) + 0.5) * (2 / 25)
 
-    image = interpolate_2d(sdf_2, 'A', x_pixels=25,  y_pixels=25, normalize=False)
-    image_vec = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=25,  y_pixels=25, normalize=False)
+    image = interpolate_2d(sdf_2, 'A', x_pixels=25,  y_pixels=25, normalize=False, hmin=False)
+    image_vec = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=25,  y_pixels=25, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert approx(w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_2['h'][0], 2)
                           + w[1] * sdf_2['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
                                                             / sdf_2['h'][1], 2)) == image[y][x]
             assert approx(w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_2['h'][0], 2)
                           + w[1] * sdf_2['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
                                                             / sdf_2['h'][1], 2)) == image_vec[0][y][x]
             assert approx(w[0] * sdf_2['B'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_2['h'][0], 2)
                           + w[1] * sdf_2['B'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
                                                             / sdf_2['h'][1], 2)) == image_vec[1][y][x]
 
-    image = interpolate_2d_line(sdf_2, 'A', pixels=25, normalize=False)
+    image = interpolate_2d_line(sdf_2, 'A', pixels=25, normalize=False, hmin=False)
     for x in range(25):
         assert approx(w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[x] ** 2) / sdf_2['h'][0], 2)
                       + w[1] * sdf_2['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - x] ** 2)
                                                         / sdf_2['h'][1], 2)) == image[x]
 
     c_kernel = kernel.get_column_kernel_func(1000)
 
     image = interpolate_3d_proj(sdf_3, 'A', x_pixels=25, y_pixels=25,
-                                dens_weight=False, normalize=False)
+                                dens_weight=False, normalize=False, hmin=False)
     image_vec = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=25, y_pixels=25,
-                                   dens_weight=False, normalize=False)
+                                   dens_weight=False, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert approx(w[0] * sdf_3['A'][0] * c_kernel(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_3['h'][0], 2)
                           + w[1] * sdf_3['A'][1] * c_kernel(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
                                                             / sdf_3['h'][1], 2)) == image[y][x]
             assert approx(w[0] * sdf_3['A'][0] * c_kernel(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_3['h'][0], 2)
                           + w[1] * sdf_3['A'][1] * c_kernel(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
@@ -383,29 +383,29 @@
             assert approx(w[0] * sdf_3['B'][0] * c_kernel(np.sqrt(real[x] ** 2 + real[y] ** 2) / sdf_3['h'][0], 2)
                           + w[1] * sdf_3['B'][1] * c_kernel(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2)
                                                             / sdf_3['h'][1], 2)) == image_vec[1][y][x]
 
     # Weight for 3D cross-section interpolation.
     w = sdf_3['m'] / (sdf_3['rho'] * sdf_3['h'] ** 3)
 
-    image = interpolate_3d_cross(sdf_3, 'A', x_pixels=25, y_pixels=25, normalize=False)
-    image_vec = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=25, y_pixels=25, normalize=False)
+    image = interpolate_3d_cross(sdf_3, 'A', x_pixels=25, y_pixels=25, normalize=False, hmin=False)
+    image_vec = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=25, y_pixels=25, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert approx(w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 1) / sdf_3['h'][0], 3)
                           + w[1] * sdf_3['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2 + 1)
                                                             / sdf_3['h'][1], 3)) == image[y][x]
             assert approx(w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 1) / sdf_3['h'][0], 3)
                           + w[1] * sdf_3['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2 + 1)
                                                             / sdf_3['h'][1], 3)) == image_vec[0][y][x]
             assert approx(w[0] * sdf_3['B'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + 1) / sdf_3['h'][0], 3)
                           + w[1] * sdf_3['B'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2 + 1)
                                                             / sdf_3['h'][1], 3)) == image_vec[1][y][x]
 
-    image = interpolate_3d_grid(sdf_3, 'A', x_pixels=25, y_pixels=25, z_pixels=25, normalize=False)
+    image = interpolate_3d_grid(sdf_3, 'A', x_pixels=25, y_pixels=25, z_pixels=25, normalize=False, hmin=False)
     for z in range(25):
         for y in range(25):
             for x in range(25):
                 assert approx(
                     w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real[x] ** 2 + real[y] ** 2 + real[z] ** 2)
                                                     / sdf_3['h'][0], 3) +
                     w[1] * sdf_3['A'][1] * kernel.w(np.sqrt(real[24 - x] ** 2 + real[24 - y] ** 2 + real[24 - z] ** 2)
@@ -418,47 +418,47 @@
     Interpolation with flipped x & y axes should be equivalent to the transpose of regular interpolation.
     """
     df = pd.DataFrame({'x': [-1, 1], 'y': [1, -1], 'A': [2, 1.5], 'B': [5, 4], 'h': [1.1, 1.3], 'rho': [0.55, 0.45],
                        'm': [0.04, 0.05]})
     sdf = SarracenDataFrame(df, params=dict())
     sdf.backend = backend
 
-    image1 = interpolate_2d(sdf, 'A', x_pixels=20,  y_pixels=20, normalize=False)
-    image2 = interpolate_2d(sdf, 'A', x='y', y='x', x_pixels=20,  y_pixels=20, normalize=False)
+    image1 = interpolate_2d(sdf, 'A', x_pixels=20,  y_pixels=20, normalize=False, hmin=False)
+    image2 = interpolate_2d(sdf, 'A', x='y', y='x', x_pixels=20,  y_pixels=20, normalize=False, hmin=False)
     assert_allclose(image1, image2.T)
 
-    image1 = interpolate_2d_vec(sdf, 'A', 'B', x_pixels=20, y_pixels=20, normalize=False)
-    image2 = interpolate_2d_vec(sdf, 'A', 'B', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False)
+    image1 = interpolate_2d_vec(sdf, 'A', 'B', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
+    image2 = interpolate_2d_vec(sdf, 'A', 'B', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0].T)
     assert_allclose(image1[1], image2[1].T)
 
     df = pd.DataFrame({'x': [-1, 1], 'y': [1, -1], 'z': [-1, 1], 'A': [2, 1.5], 'B': [5, 4], 'C': [2.5, 3],
                        'h': [1.1, 1.3], 'rho': [0.55, 0.45], 'm': [0.04, 0.05]})
     sdf = SarracenDataFrame(df, params=dict())
 
-    image1 = interpolate_3d_proj(sdf, 'A', x_pixels=20,  y_pixels=20, normalize=False)
-    image2 = interpolate_3d_proj(sdf, 'A', x='y', y='x', x_pixels=20,  y_pixels=20, normalize=False)
+    image1 = interpolate_3d_proj(sdf, 'A', x_pixels=20,  y_pixels=20, normalize=False, hmin=False)
+    image2 = interpolate_3d_proj(sdf, 'A', x='y', y='x', x_pixels=20,  y_pixels=20, normalize=False, hmin=False)
     assert_allclose(image1, image2.T)
 
-    image1 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, normalize=False)
-    image2 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x='y', y='x', x_pixels=50, y_pixels=50, normalize=False)
+    image1 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, normalize=False, hmin=False)
+    image2 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x='y', y='x', x_pixels=50, y_pixels=50, normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0].T)
     assert_allclose(image1[1], image2[1].T)
 
-    image1 = interpolate_3d_cross(sdf, 'A', x_pixels=50, y_pixels=50, normalize=False)
-    image2 = interpolate_3d_cross(sdf, 'A', x='y', y='x', x_pixels=50, y_pixels=50, normalize=False)
+    image1 = interpolate_3d_cross(sdf, 'A', x_pixels=50, y_pixels=50, normalize=False, hmin=False)
+    image2 = interpolate_3d_cross(sdf, 'A', x='y', y='x', x_pixels=50, y_pixels=50, normalize=False, hmin=False)
     assert_allclose(image1, image2.T)
 
-    image1 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', x_pixels=20, y_pixels=20, normalize=False)
-    image2 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False)
+    image1 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
+    image2 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0].T)
     assert_allclose(image1[1], image2[1].T)
 
-    image1 = interpolate_3d_grid(sdf, 'A', x_pixels=20, y_pixels=20, normalize=False)
-    image2 = interpolate_3d_grid(sdf, 'A', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False)
+    image1 = interpolate_3d_grid(sdf, 'A', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
+    image2 = interpolate_3d_grid(sdf, 'A', x='y', y='x', x_pixels=20, y_pixels=20, normalize=False, hmin=False)
     assert_allclose(image1, image2.transpose(0, 2, 1))
 
 
 @mark.parametrize("backend", backends)
 def test_default_kernel(backend):
     """
     Interpolation should use the kernel supplied to the function. If no kernel is supplied, the kernel attached to the
@@ -474,71 +474,71 @@
     sdf_3.kernel = kernel
     sdf_2.backend = backend
     sdf_3.backend = backend
 
     # First, test that the dataframe kernel is used in cases with no kernel supplied.
 
     # Each interpolation is performed over one pixel, offering an easy way to check the kernel used by the function.
-    image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 2)
-    image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image[0] == kernel.w(0, 2)
     assert image[1] == kernel.w(0, 2)
 
-    image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 2)
 
-    image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.get_column_kernel()[0]
-    image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image[0] == kernel.get_column_kernel()[0]
     assert image[1] == kernel.get_column_kernel()[0]
 
-    image = interpolate_3d_cross(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_cross(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
-    image = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image[0] == kernel.w(0, 3)
     assert image[1] == kernel.w(0, 3)
 
     image = interpolate_3d_grid(sdf_3, 'A', x_pixels=1, y_pixels=1, z_pixels=1, xlim=(-1, 1), ylim=(-1, 1),
-                                zlim=(-1, 1), normalize=False)
+                                zlim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
 
-    image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
 
     # Next, test that the kernel supplied to the function is actually used.
     kernel = QuinticSplineKernel()
-    image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image == kernel.w(0, 2)
-    image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image[0] == kernel.w(0, 2)
     assert image[1] == kernel.w(0, 2)
 
-    image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image == kernel.w(0, 2)
 
-    image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image == kernel.get_column_kernel()[0]
-    image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image[0] == kernel.get_column_kernel()[0]
     assert image[1] == kernel.get_column_kernel()[0]
 
-    image = interpolate_3d_cross(sdf_3, 'A', kernel=kernel, x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+    image = interpolate_3d_cross(sdf_3, 'A', kernel=kernel, x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
     image = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1),
-                                     kernel=kernel, normalize=False)
+                                     kernel=kernel, normalize=False, hmin=False)
     assert image[0] == kernel.w(0, 3)
     assert image[1] == kernel.w(0, 3)
 
     image = interpolate_3d_grid(sdf_3, 'A', x_pixels=1, y_pixels=1, z_pixels=1, xlim=(-1, 1), ylim=(-1, 1),
-                                zlim=(-1, 1), kernel=kernel, normalize=False)
+                                zlim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
 
-    image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False)
+    image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), kernel=kernel, normalize=False, hmin=False)
     assert image == kernel.w(0, 3)
 
 
 @mark.parametrize("backend", backends)
 def test_column_samples(backend):
     """
     3D column interpolation should use the number of integral samples supplied as an argument.
@@ -548,15 +548,15 @@
     kernel = QuinticSplineKernel()
     sdf_3.kernel = kernel
     sdf_3.backend = backend
 
     # 2 samples is used here, since a column kernel with 2 samples will be drastically different than the
     # default kernel of 1000 samples.
     image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1),
-                                integral_samples=2, normalize=False)
+                                integral_samples=2, normalize=False, hmin=False)
     assert image == kernel.get_column_kernel(2)[0]
 
 
 # this test is incredibly slow on the GPU backend (30min+) so it only runs on the CPU
 # backend for now.
 #@mark.parametrize("backend", backends)
 def test_pixel_arguments():
@@ -577,27 +577,27 @@
 
     # 3D grid interpolation
     for axes in [('x', 'y', 'z'), ('x', 'z', 'y'), ('y', 'z', 'x'), ('y', 'x', 'z'), ('z', 'x', 'y'), ('z', 'y', 'x')]:
         ratio01 = np.abs(df_3[axes[0]][1] - df_3[axes[0]][0]) / np.abs(df_3[axes[1]][1] - df_3[axes[1]][0])
         ratio02 = np.abs(df_3[axes[0]][1] - df_3[axes[0]][0]) / np.abs(df_3[axes[2]][1] - df_3[axes[2]][0])
         ratio12 = np.abs(df_3[axes[1]][1] - df_3[axes[1]][0]) / np.abs(df_3[axes[2]][1] - df_3[axes[2]][0])
 
-        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], normalize=False)
+        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], normalize=False, hmin=False)
         assert image.shape[2] / image.shape[1] == approx(ratio01, rel=1e-2)
         assert image.shape[1] / image.shape[0] == approx(ratio12, rel=1e-2)
         assert image.shape[2] / image.shape[0] == approx(ratio02, rel=1e-2)
 
-        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], x_pixels=default_pixels, normalize=False)
+        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], x_pixels=default_pixels, normalize=False, hmin=False)
         assert image.shape == (round(default_pixels / ratio02), round(default_pixels / ratio01), default_pixels)
 
-        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], y_pixels=default_pixels, normalize=False)
+        image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], y_pixels=default_pixels, normalize=False, hmin=False)
         assert image.shape == (round(default_pixels / ratio12), default_pixels, round(default_pixels * ratio01))
 
         image = interpolate_3d_grid(sdf_3, 'A', x=axes[0], y=axes[1], z=axes[2], x_pixels=default_pixels,
-                                    y_pixels=default_pixels, z_pixels=default_pixels, normalize=False)
+                                    y_pixels=default_pixels, z_pixels=default_pixels, normalize=False, hmin=False)
         assert image.shape == (default_pixels, default_pixels, default_pixels)
 
     # Non-vector functions
     for func in [interpolate_2d, interpolate_3d_proj, interpolate_3d_cross]:
         for axes in [('x', 'y'), ('x', 'z'), ('y', 'z'), ('y', 'x'), ('z', 'x'), ('z', 'y')]:
             # The ratio of distance between particles in the second axis versus the distance between particles in
             # the first axis.
@@ -608,67 +608,67 @@
                 continue
 
             # The dataframe is selected to ensure the correct number of dimensions.
             sdf = sdf_2 if func is interpolate_2d else sdf_3
 
             # With no pixels specified, the pixels in the image will match the ratio of the data.
             # The loose tolerance here accounts for the integer rounding.
-            image = func(sdf, 'A', x=axes[0], y=axes[1], normalize=False)
+            image = func(sdf, 'A', x=axes[0], y=axes[1], normalize=False, hmin=False)
             assert image.shape[0] / image.shape[1] == approx(ratio, rel=1e-2)
 
             # With one axis specified, the pixels in the other axis will be selected to match the ratio of the data.
-            image = func(sdf, 'A', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False)
+            image = func(sdf, 'A', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False, hmin=False)
             assert image.shape == (round(default_pixels * ratio), default_pixels)
 
-            image = func(sdf, 'A', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False)
+            image = func(sdf, 'A', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False, hmin=False)
             assert image.shape == (default_pixels, round(default_pixels / ratio))
 
             # With both axes specified, the pixels will simply match the specified counts.
-            image = func(sdf, 'A', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False)
+            image = func(sdf, 'A', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False, hmin=False)
             assert image.shape == (default_pixels, default_pixels * 2)
 
     # 3D Vector-based functions
     for func in [interpolate_3d_vec, interpolate_3d_cross_vec]:
         for axes in [('x', 'y'), ('x', 'z'), ('y', 'z'), ('y', 'x'), ('z', 'x'), ('z', 'y')]:
             ratio = np.abs(df_3[axes[1]][1] - df_3[axes[1]][0]) / np.abs(df_3[axes[0]][1] - df_3[axes[0]][0])
 
             # Here, the tests are performed for both vector directions.
-            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], normalize=False)
+            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], normalize=False, hmin=False)
             assert image[0].shape[0] / image[0].shape[1] == approx(ratio, rel=1e-2)
             assert image[1].shape[0] / image[1].shape[1] == approx(ratio, rel=1e-2)
 
-            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False)
+            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False, hmin=False)
             assert image[0].shape == (round(default_pixels * ratio), default_pixels)
             assert image[1].shape == (round(default_pixels * ratio), default_pixels)
 
-            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False)
+            image = func(sdf_3, 'A', 'B', 'C', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False, hmin=False)
             assert image[0].shape == (default_pixels, round(default_pixels / ratio))
             assert image[1].shape == (default_pixels, round(default_pixels / ratio))
 
-            image = func(sdf_3, 'A', 'B', 'C', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False)
+            image = func(sdf_3, 'A', 'B', 'C', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False, hmin=False)
             assert image[0].shape == (default_pixels, default_pixels * 2)
             assert image[1].shape == (default_pixels, default_pixels * 2)
 
     # 2D vector interpolation
     for axes in [('x', 'y'), ('y', 'x')]:
         ratio = np.abs(df_3[axes[1]][1] - df_3[axes[1]][0]) / np.abs(df_3[axes[0]][1] - df_3[axes[0]][0])
 
-        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], normalize=False)
+        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], normalize=False, hmin=False)
         assert image[0].shape[0] / image[0].shape[1] == approx(ratio, rel=1e-2)
         assert image[1].shape[0] / image[1].shape[1] == approx(ratio, rel=1e-2)
 
-        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False)
+        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], x_pixels=default_pixels, normalize=False, hmin=False)
         assert image[0].shape == (round(default_pixels * ratio), default_pixels)
         assert image[1].shape == (round(default_pixels * ratio), default_pixels)
 
-        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False)
+        image = interpolate_2d_vec(sdf_2, 'A', 'B', x=axes[0], y=axes[1], y_pixels=default_pixels, normalize=False, hmin=False)
         assert image[0].shape == (default_pixels, round(default_pixels / ratio))
         assert image[1].shape == (default_pixels, round(default_pixels / ratio))
 
-        image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False)
+        image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=default_pixels * 2, y_pixels=default_pixels, normalize=False, hmin=False)
         assert image[0].shape == (default_pixels, default_pixels * 2)
         assert image[1].shape == (default_pixels, default_pixels * 2)
 
 
 @mark.parametrize("backend", backends)
 def test_irregular_bounds(backend):
     """
@@ -685,18 +685,18 @@
     w = sdf['m'] / (sdf['rho'] * sdf['h'] ** 2)
 
     # A mapping of pixel indices to x / y values in particle space.
     real_x = -kernel.get_radius() + (np.arange(0, 50) + 0.5) * (2 * kernel.get_radius() / 50)
     real_y = -kernel.get_radius() + (np.arange(0, 25) + 0.5) * (2 * kernel.get_radius() / 25)
 
     image = interpolate_2d(sdf, 'A', x_pixels=50, y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_2d_vec(sdf, 'A', 'B', x_pixels=50, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(50):
             assert image[y][x] == approx(
                 w[0] * sdf['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == approx(
@@ -706,49 +706,49 @@
     sdf['C'] = 5
     sdf['z'] = -0.5
     sdf.zcol = 'z'
 
     column_func = kernel.get_column_kernel_func(1000)
 
     image = interpolate_3d_proj(sdf, 'A', x_pixels=50, y_pixels=25, xlim=(-kernel.get_radius(), kernel.get_radius()),
-                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                           ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     image_vec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=25,
                                    xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False)
+                                   ylim=(-kernel.get_radius(), kernel.get_radius()), dens_weight=False, normalize=False, hmin=False)
     for y in range(25):
         for x in range(50):
             assert image[y][x] == approx(
                 w[0] * sdf['A'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf['A'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf['h'][0], 2))
             assert image_vec[1][y][x] == approx(
                 w[0] * sdf['B'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf['h'][0], 2))
 
     # Weight for 3D cross-section interpolation.
     w = sdf['m'] / (sdf['rho'] * sdf['h'] ** 3)
 
     image = interpolate_3d_cross(sdf, 'A', z_slice=0, x_pixels=50, y_pixels=25,
                                  xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                 ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     image_vec = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=25,
                                          xlim=(-kernel.get_radius(), kernel.get_radius()),
-                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False)
+                                         ylim=(-kernel.get_radius(), kernel.get_radius()), normalize=False, hmin=False)
     for y in range(25):
         for x in range(50):
             assert image[y][x] == approx(
                 w[0] * sdf['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf['h'][0], 3))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf['h'][0], 3))
             assert image_vec[1][y][x] == approx(
                 w[0] * sdf['B'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf['h'][0], 3))
 
     real_z = -kernel.get_radius() + 0.5 + (np.arange(0, 15) + 0.5) * (2 * kernel.get_radius() / 15)
     limit = -kernel.get_radius(), kernel.get_radius()
 
-    image = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=25, z_pixels=15, xlim=limit, ylim=limit, zlim=limit, normalize=False)
+    image = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=25, z_pixels=15, xlim=limit, ylim=limit, zlim=limit, normalize=False, hmin=False)
     for z in range(15):
         for y in range(25):
             for x in range(50):
                 assert image[z][y][x] == approx(
                     w[0] * sdf['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + real_z[z] ** 2) / sdf['h'][0], 3))
 
 
@@ -773,61 +773,61 @@
     # Weight for 2D interpolation, and 3D column interpolation.
     w = sdf_2['m'] / (sdf_2['rho'] * sdf_2['h'] ** 2)
 
     # A mapping of pixel indices to x / y values in particle space.
     real_x = 1 + (np.arange(0, 25) + 0.5) * (1 / 25)
     real_y = 1 + (np.arange(0, 25) + 0.5) * (1 / 25)
 
-    image = interpolate_2d(sdf_2, 'A', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False)
-    image_vec = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False)
-    line = interpolate_2d_line(sdf_2, 'A', pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False)
+    image = interpolate_2d(sdf_2, 'A', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False, hmin=False)
+    image_vec = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False, hmin=False)
+    line = interpolate_2d_line(sdf_2, 'A', pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False, hmin=False)
     for y in range(25):
         assert line[y] == approx(
             w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real_x[y] ** 2 + real_y[y] ** 2) / sdf_2['h'][0], 2))
         for x in range(25):
             assert image[y][x] == approx(
                 w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_2['h'][0], 2))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf_2['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_2['h'][0], 2))
             assert image_vec[1][y][x] == approx(
                 w[0] * sdf_2['B'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_2['h'][0], 2))
 
     column_func = kernel.get_column_kernel_func(1000)
 
     image = interpolate_3d_proj(sdf_3, 'A', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2),
-                                dens_weight=False, normalize=False)
+                                dens_weight=False, normalize=False, hmin=False)
     image_vec = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2),
-                                   dens_weight=False, normalize=False)
+                                   dens_weight=False, normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == approx(
                 w[0] * sdf_3['A'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_3['h'][0], 2))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf_3['A'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_3['h'][0], 2))
             assert image_vec[1][y][x] == approx(
                 w[0] * sdf_3['B'][0] * column_func(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2) / sdf_3['h'][0], 2))
 
     # Weight for 3D cross-sections.
     w = sdf_3['m'] / (sdf_3['rho'] * sdf_3['h'] ** 3)
 
-    image = interpolate_3d_cross(sdf_3, 'A', z_slice=0, x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False)
-    image_vec = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', 0, x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False)
+    image = interpolate_3d_cross(sdf_3, 'A', z_slice=0, x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False, hmin=False)
+    image_vec = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', 0, x_pixels=25, y_pixels=25, xlim=(1, 2), ylim=(1, 2), normalize=False, hmin=False)
     for y in range(25):
         for x in range(25):
             assert image[y][x] == approx(
                 w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf_3['h'][0], 3))
             assert image_vec[0][y][x] == approx(
                 w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf_3['h'][0], 3))
             assert image_vec[1][y][x] == approx(
                 w[0] * sdf_3['B'][0] * kernel.w(np.sqrt(real_x[x] ** 2 + real_y[y] ** 2 + 0.5 ** 2) / sdf_3['h'][0], 3))
 
     real_z = 0.5 + (np.arange(0, 25) + 0.5) * (1 / 25)
 
     image = interpolate_3d_grid(sdf_3, 'A', x_pixels=25, y_pixels=25, z_pixels=25, xlim=(1, 2), ylim=(1, 2),
-                                zlim=(1, 2), normalize=False)
+                                zlim=(1, 2), normalize=False, hmin=False)
 
     for z in range(25):
         for y in range(25):
             for x in range(25):
                 assert image[z][y][x] == approx(
                     w[0] * sdf_3['A'][0] * kernel.w(np.sqrt(real_x[x]**2 + real_y[y]**2 + real_z[z]**2) / sdf_3['h'][0], 3))
 
@@ -875,21 +875,21 @@
     sdf.backend = backend
 
     column_kernel = kernel.get_column_kernel_func(1000)
 
     rot_z, rot_y, rot_x = 129, 34, 50
 
     image_col = interpolate_3d_proj(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                               rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], dens_weight=False, normalize=False)
+                               rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], dens_weight=False, normalize=False, hmin=False)
     image_cross = interpolate_3d_cross(sdf, 'A', z_slice=0, rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0],
-                                       x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                       x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     image_colvec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                      rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], dens_weight=False, normalize=False)
+                                      rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], dens_weight=False, normalize=False, hmin=False)
     image_crossvec = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=50, xlim=(-1, 1),
-                                              ylim=(-1, 1), rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False)
+                                              ylim=(-1, 1), rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False, hmin=False)
 
     w_col = sdf['m'] / (sdf['rho'] * sdf['h'] ** 2)
     w_cross = sdf['m'] / (sdf['rho'] * sdf['h'] ** 3)
 
     pos_x, pos_y, pos_z = rotate((1, 1, 1), rot_z, rot_y, rot_x)
     target_x, target_y, target_z = rotate((4, 5, 6), rot_z, rot_y, rot_x)
 
@@ -907,15 +907,15 @@
                 np.sqrt((pos_x - real[x]) ** 2 + (pos_y - real[y]) ** 2 + pos_z ** 2) / sdf['h'][0], 3))
             assert image_crossvec[0][y][x] == approx(w_cross[0] * target_x * kernel.w(
                 np.sqrt((pos_x - real[x]) ** 2 + (pos_y - real[y]) ** 2 + pos_z ** 2) / sdf['h'][0], 3))
             assert image_crossvec[1][y][x] == approx(w_cross[0] * target_y * kernel.w(
                 np.sqrt((pos_x - real[x]) ** 2 + (pos_y - real[y]) ** 2 + pos_z ** 2) / sdf['h'][0], 3))
 
     image_grid = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=50, z_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                     zlim=(-1, 1), rotation=[rot_z, rot_y, rot_x], rot_origin=[0, 0, 0], normalize=False)
+                                     zlim=(-1, 1), rotation=[rot_z, rot_y, rot_x], rot_origin=[0, 0, 0], normalize=False, hmin=False)
 
     for z in range(50):
         for y in range(50):
             for x in range(50):
                 assert image_grid[z][y][x] == \
                        approx(w_cross[0] * sdf['A'][0] * kernel.w(np.sqrt((pos_x - real[x]) ** 2
                                                                           + (pos_y - real[y]) ** 2
@@ -934,48 +934,48 @@
     kernel = CubicSplineKernel()
     sdf.kernel = kernel
     sdf.backend = backend
 
     rot_z, rot_y, rot_x = 67, -34, 91
 
     image1 = interpolate_3d_proj(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                            rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False)
+                            rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False, hmin=False)
     image2 = interpolate_3d_proj(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
                                  rotation=Rotation.from_euler('zyx', [rot_z, rot_y, rot_x], degrees=True),
-                                 origin=[0, 0, 0], normalize=False)
+                                 origin=[0, 0, 0], normalize=False, hmin=False)
     assert_allclose(image1, image2)
 
     image1 = interpolate_3d_cross(sdf, 'A', z_slice=0, rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], x_pixels=50,
-                                  y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                  y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     image2 = interpolate_3d_cross(sdf, 'A', z_slice=0,
                                   rotation=Rotation.from_euler('zyx', [rot_z, rot_y, rot_x], degrees=True),
-                                  origin=[0, 0, 0], x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                  origin=[0, 0, 0], x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert_allclose(image1, image2)
 
     image1 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                  rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False)
+                                  rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False, hmin=False)
     image2 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
                                   rotation=Rotation.from_euler('zyx', [rot_z, rot_y, rot_x], degrees=True),
-                                  origin=[0, 0, 0], normalize=False)
+                                  origin=[0, 0, 0], normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0])
     assert_allclose(image1[1], image2[1])
 
     image1 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                      rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False)
+                                      rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False, hmin=False)
     image2 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
                                       rotation=Rotation.from_euler('zyx', [rot_z, rot_y, rot_x], degrees=True),
-                                      origin=[0, 0, 0], normalize=False)
+                                      origin=[0, 0, 0], normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0])
     assert_allclose(image1[1], image2[1])
 
     image1 = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), zlim=(-1, 1),
-                                 rotation=[rot_z, rot_y, rot_x], rot_origin=[0, 0, 0], normalize=False)
+                                 rotation=[rot_z, rot_y, rot_x], rot_origin=[0, 0, 0], normalize=False, hmin=False)
     image2 = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), zlim=(-1, 1),
                                  rotation=Rotation.from_euler('zyx', [rot_z, rot_y, rot_x], degrees=True),
-                                 rot_origin=[0, 0, 0], normalize=False)
+                                 rot_origin=[0, 0, 0], normalize=False, hmin=False)
     assert_allclose(image1, image2)
 
 
 @mark.parametrize("backend", backends)
 def test_quaternion_rotation(backend):
     """
     An alternate rotation (in this case, a quaternion) defined using scipy should function properly.
@@ -987,21 +987,21 @@
     sdf.kernel = kernel
     sdf.backend = backend
 
     column_kernel = kernel.get_column_kernel_func(1000)
 
     quat = Rotation.from_quat([5, 3, 8, 1])
     image_col = interpolate_3d_proj(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), rotation=quat,
-                               origin=[0, 0, 0], dens_weight=False, normalize=False)
+                               origin=[0, 0, 0], dens_weight=False, normalize=False, hmin=False)
     image_colvec = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                      rotation=quat, origin=[0, 0, 0], dens_weight=False, normalize=False)
+                                      rotation=quat, origin=[0, 0, 0], dens_weight=False, normalize=False, hmin=False)
     image_cross = interpolate_3d_cross(sdf, 'A', z_slice=0, rotation=quat, origin=[0, 0, 0], x_pixels=50, y_pixels=50,
-                                       xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                       xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     image_crossvec = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=50, xlim=(-1, 1),
-                                              ylim=(-1, 1), rotation=quat, origin=[0, 0, 0], normalize=False)
+                                              ylim=(-1, 1), rotation=quat, origin=[0, 0, 0], normalize=False, hmin=False)
 
     w_col = sdf['m'] / (sdf['rho'] * sdf['h'] ** 2)
     w_cross = sdf['m'] / (sdf['rho'] * sdf['h'] ** 3)
 
     pos = quat.apply([1, 1, 1])
     val = quat.apply([sdf['A'][0], sdf['B'][0], sdf['C'][0]])
     real = -1 + (np.arange(0, 50) + 0.5) * (1 / 25)
@@ -1021,15 +1021,15 @@
 
             assert image_crossvec[0][y][x] == approx(w_cross[0] * val[0] * kernel.w(
                 np.sqrt((pos[0] - real[x]) ** 2 + (pos[1] - real[y]) ** 2 + pos[2] ** 2) / sdf['h'][0], 3))
             assert image_crossvec[1][y][x] == approx(w_cross[0] * val[1] * kernel.w(
                 np.sqrt((pos[0] - real[x]) ** 2 + (pos[1] - real[y]) ** 2 + pos[2] ** 2) / sdf['h'][0], 3))
 
     image_grid = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=50, z_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                     zlim=(-1, 1), rotation=quat, rot_origin=[0, 0, 0], normalize=False)
+                                     zlim=(-1, 1), rotation=quat, rot_origin=[0, 0, 0], normalize=False, hmin=False)
 
     for z in range(50):
         for y in range(50):
             for x in range(50):
                 assert image_grid[z][y][x] == approx(w_cross[0] * sdf['A'][0] * kernel.w(
                     np.sqrt((pos[0] - real[x]) ** 2 + (pos[1] - real[y]) ** 2 + (pos[2] - real[z]) ** 2)
                     / sdf['h'][0], 3))
@@ -1048,17 +1048,17 @@
     sdf.kernel = kernel
     sdf.backend = backend
 
     real = -1 + (np.arange(0, 50) + 0.5) * (1 / 25)
     pixel_x, pixel_y = 12, 30
 
     for func in [interpolate_3d_proj, interpolate_3d_cross]:
-        image = func(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+        image = func(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
         image_rot = func(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), rotation=[237, 0, 0],
-                         origin=[real[pixel_x], real[pixel_y], 0], normalize=False)
+                         origin=[real[pixel_x], real[pixel_y], 0], normalize=False, hmin=False)
 
         assert image[pixel_y][pixel_x] == approx(image_rot[pixel_y][pixel_x])
 
 
 @mark.parametrize("backend", backends)
 def test_axes_rotation_separation(backend):
     """
@@ -1067,43 +1067,43 @@
     """
     df = pd.DataFrame({'x': [-1, 1], 'y': [1, -1], 'z': [1, -1], 'A': [2, 1.5], 'B': [2, 2], 'C': [4, 3],
                        'h': [1.1, 1.3], 'rho': [0.55, 0.45], 'm': [0.04, 0.05]})
     sdf = SarracenDataFrame(df, params=dict())
     sdf.backend = backend
 
     image1 = interpolate_3d_proj(sdf, 'A', x_pixels=50,  y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                 rotation=[234, 90, 48], normalize=False)
+                                 rotation=[234, 90, 48], normalize=False, hmin=False)
     image2 = interpolate_3d_proj(sdf, 'A', x='y', y='x', x_pixels=50,  y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                 rotation=[234, 90, 48], normalize=False)
+                                 rotation=[234, 90, 48], normalize=False, hmin=False)
     assert_allclose(image1, image2.T)
 
     image1 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                rotation=[234, 90, 48], normalize=False)
+                                rotation=[234, 90, 48], normalize=False, hmin=False)
     image2 = interpolate_3d_vec(sdf, 'A', 'B', 'C', x='y', y='x', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                rotation=[234, 90, 48], normalize=False)
+                                rotation=[234, 90, 48], normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0].T)
     assert_allclose(image1[1], image2[1].T)
 
     image1 = interpolate_3d_cross(sdf, 'A', z_slice=0, rotation=[234, 90, 48], x_pixels=50, y_pixels=50, xlim=(-1, 1),
-                                  ylim=(-1, 1), normalize=False)
+                                  ylim=(-1, 1), normalize=False, hmin=False)
     image2 = interpolate_3d_cross(sdf, 'A', x='y', y='x', z_slice=0, rotation=[234, 90, 48], x_pixels=50, y_pixels=50,
-                                  xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                  xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
     assert_allclose(image1, image2.T)
 
     image1 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                      rotation=[234, 90, 48], normalize=False)
+                                      rotation=[234, 90, 48], normalize=False, hmin=False)
     image2 = interpolate_3d_cross_vec(sdf, 'A', 'B', 'C', 0, x='y', y='x', x_pixels=50, y_pixels=50, xlim=(-1, 1),
-                                      ylim=(-1, 1), rotation=[234, 90, 48], normalize=False)
+                                      ylim=(-1, 1), rotation=[234, 90, 48], normalize=False, hmin=False)
     assert_allclose(image1[0], image2[0].T)
     assert_allclose(image1[1], image2[1].T)
 
     image1 = interpolate_3d_grid(sdf, 'A', x_pixels=50, y_pixels=50, z_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                 zlim=(-1, 1), rotation=[234, 90, 48], normalize=False)
+                                 zlim=(-1, 1), rotation=[234, 90, 48], normalize=False, hmin=False)
     image2 = interpolate_3d_grid(sdf, 'A', x='y', y='x', x_pixels=50, y_pixels=50, z_pixels=50, xlim=(-1, 1),
-                                 ylim=(-1, 1), zlim=(-1, 1), rotation=[234, 90, 48], normalize=False)
+                                 ylim=(-1, 1), zlim=(-1, 1), rotation=[234, 90, 48], normalize=False, hmin=False)
     assert_allclose(image1, image2.transpose(0, 2, 1))
 
 
 @mark.parametrize("backend", backends)
 def test_axes_rotation_equivalency(backend):
     """
     A rotated interpolation (at multiples of 90 degrees) should be equivalent to a transformed interpolation with
@@ -1120,16 +1120,16 @@
     for i_z in range(4):
         for i_y in range(4):
             for i_x in range(4):
                 rot_x, rot_y, rot_z = i_x * 90, i_y * 90, i_z * 90
 
                 for func in [interpolate_3d_proj, interpolate_3d_cross]:
                     image1 = func(sdf, 'A', x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1),
-                                  rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False)
-                    image2 = func(sdf, 'A', x=x, y=y, x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False)
+                                  rotation=[rot_z, rot_y, rot_x], origin=[0, 0, 0], normalize=False, hmin=False)
+                    image2 = func(sdf, 'A', x=x, y=y, x_pixels=50, y_pixels=50, xlim=(-1, 1), ylim=(-1, 1), normalize=False, hmin=False)
                     image2 = image2 if not flip_x else np.flip(image2, 1)
                     image2 = image2 if not flip_y else np.flip(image2, 0)
                     assert_allclose(image1, image2)
 
                 y, z = z, y
                 flip_y, flip_z = not flip_z, flip_y
             x, z = z, x
@@ -1150,36 +1150,36 @@
     sdf_3 = SarracenDataFrame(df_3, params=dict())
 
     sdf_2.backend = backend
     sdf_3.backend = backend
 
     for b in [(-3, 3, 3, -3, 20, 20), (3, 3, 3, 3, 20, 20), (-3, 3, -3, 3, 0, 0)]:
         with raises(ValueError):
-            interpolate_2d(sdf_2, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4], y_pixels=b[5], normalize=False)
+            interpolate_2d(sdf_2, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4], y_pixels=b[5], normalize=False, hmin=False)
         with raises(ValueError):
             interpolate_2d_vec(sdf_2, 'A', 'B', 'C', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4],
-                               y_pixels=b[5], normalize=False)
+                               y_pixels=b[5], normalize=False, hmin=False)
         # the first case will not fail for this type of interpolation.
         if not b[0] == -3 and not b[3] == -3:
             with raises(ValueError):
-                interpolate_2d_line(sdf_2, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), pixels=b[4], normalize=False)
+                interpolate_2d_line(sdf_2, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), pixels=b[4], normalize=False, hmin=False)
         with raises(ValueError):
-            interpolate_3d_proj(sdf_3, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4], y_pixels=b[5], normalize=False)
+            interpolate_3d_proj(sdf_3, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4], y_pixels=b[5], normalize=False, hmin=False)
         with raises(ValueError):
             interpolate_3d_vec(sdf_3, 'A', 'B', 'C', xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4],
-                               y_pixels=b[5], normalize=False)
+                               y_pixels=b[5], normalize=False, hmin=False)
         with raises(ValueError):
             interpolate_3d_cross(sdf_3, 'A', z_slice=0, x_pixels=b[4], y_pixels=b[5], xlim=(b[0], b[1]),
-                                 ylim=(b[2], b[3]), normalize=False)
+                                 ylim=(b[2], b[3]), normalize=False, hmin=False)
         with raises(ValueError):
             interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', 0, xlim=(b[0], b[1]), ylim=(b[2], b[3]), x_pixels=b[4],
-                                     y_pixels=b[5], normalize=False)
+                                     y_pixels=b[5], normalize=False, hmin=False)
         with raises(ValueError):
             interpolate_3d_grid(sdf_3, 'A', xlim=(b[0], b[1]), ylim=(b[2], b[3]), zlim=(-3, 3), x_pixels=b[4],
-                                y_pixels=b[5], z_pixels=10, normalize=False)
+                                y_pixels=b[5], z_pixels=10, normalize=False, hmin=False)
 
 
 @mark.parametrize("backend", backends)
 def test_required_columns(backend):
     """
     Interpolation without one of the required columns will result in a KeyError.
     """
@@ -1194,31 +1194,31 @@
 
     sdf_2.backend = backend
     sdf_3.backend = backend
 
     for column in ['m', 'h']:
         sdf_dropped = sdf_2.drop(column, axis=1)
         with raises(KeyError):
-            interpolate_2d(sdf_dropped, 'A', normalize=False)
+            interpolate_2d(sdf_dropped, 'A', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_2d_line(sdf_dropped, 'A', normalize=False)
+            interpolate_2d_line(sdf_dropped, 'A', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_2d_vec(sdf_dropped, 'A', 'B', normalize=False)
+            interpolate_2d_vec(sdf_dropped, 'A', 'B', normalize=False, hmin=False)
 
         sdf_dropped = sdf_3.drop(column, axis=1)
         with raises(KeyError):
-            interpolate_3d_proj(sdf_dropped, 'A', normalize=False)
+            interpolate_3d_proj(sdf_dropped, 'A', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_3d_cross(sdf_dropped, 'A', normalize=False)
+            interpolate_3d_cross(sdf_dropped, 'A', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_3d_vec(sdf_dropped, 'A', 'B', 'C', normalize=False)
+            interpolate_3d_vec(sdf_dropped, 'A', 'B', 'C', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_3d_cross_vec(sdf_dropped, 'A', 'B', 'C', normalize=False)
+            interpolate_3d_cross_vec(sdf_dropped, 'A', 'B', 'C', normalize=False, hmin=False)
         with raises(KeyError):
-            interpolate_3d_grid(sdf_dropped, 'A', normalize=False)
+            interpolate_3d_grid(sdf_dropped, 'A', normalize=False, hmin=False)
 
 
 @mark.parametrize("backend", backends)
 def test_exact_interpolation(backend):
     """
     Exact interpolation over the entire effective area of a kernel should return 1 over the particle bounds, multiplied by the weight.
     """
@@ -1229,19 +1229,19 @@
     sdf_3 = SarracenDataFrame(df_3, params=dict())
     sdf_3.backend = backend
 
     kernel = CubicSplineKernel()
     w = sdf_2['m'] * sdf_2['A'] / (sdf_2['rho'] * sdf_2['h'] ** 2)
 
     bound = kernel.get_radius() * sdf_2['h'][0]
-    image = interpolate_2d(sdf_2, 'A', xlim=(-bound, bound), ylim=(-bound, bound), x_pixels=1, exact=True, normalize=False)
+    image = interpolate_2d(sdf_2, 'A', xlim=(-bound, bound), ylim=(-bound, bound), x_pixels=1, exact=True, normalize=False, hmin=False)
 
     assert image.sum() == approx(w[0] * sdf_2['h'][0] ** 2 / (4 * bound ** 2))
 
-    image = interpolate_3d_proj(sdf_3, 'A', xlim=(-bound, bound), ylim=(-bound, bound), x_pixels=1, exact=True, dens_weight=False, normalize=False)
+    image = interpolate_3d_proj(sdf_3, 'A', xlim=(-bound, bound), ylim=(-bound, bound), x_pixels=1, exact=True, dens_weight=False, normalize=False, hmin=False)
 
     assert image.sum() == approx(w[0] * sdf_2['h'][0] ** 2 / (4 * bound ** 2))
 
 
 @mark.parametrize("backend", backends)
 def test_density_weighted(backend):
     """
@@ -1261,44 +1261,43 @@
         if dens_weight:
             weight2d = sdf_2['m'][0] / (sdf_2['h'][0] ** 2)
             weight3d = sdf_2['m'][0] / (sdf_2['h'][0] ** 3)
         else:
             weight2d = sdf_2['m'][0] / (sdf_2['rho'][0] * sdf_2['h'][0] ** 2)
             weight3d = sdf_2['m'][0] / (sdf_2['rho'][0] * sdf_2['h'][0] ** 3)
 
-        image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_2d(sdf_2, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image == weight2d * sdf_2['A'][0] * kernel.w(0, 2)
-        image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_2d_vec(sdf_2, 'A', 'B', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight2d * sdf_2['A'][0] * kernel.w(0, 2)
         assert image[1] == weight2d * sdf_2['B'][0] * kernel.w(0, 2)
 
-        image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_2d_line(sdf_2, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight2d * sdf_2['A'][0] * kernel.w(0, 2)
 
-        image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_3d_proj(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight2d * sdf_2['A'][0] * kernel.get_column_kernel()[0]
-        image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_3d_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight2d * sdf_2['A'][0] * kernel.get_column_kernel()[0]
         assert image[1] == weight2d * sdf_2['B'][0] * kernel.get_column_kernel()[0]
 
-        image = interpolate_3d_cross(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_3d_cross(sdf_3, 'A', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight3d * sdf_2['A'][0] * kernel.w(0, 3)
-        image = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_3d_cross_vec(sdf_3, 'A', 'B', 'C', x_pixels=1, y_pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight3d * sdf_2['A'][0] * kernel.w(0, 3)
         assert image[1] == weight3d * sdf_2['B'][0] * kernel.w(0, 3)
 
         image = interpolate_3d_grid(sdf_3, 'A', x_pixels=1, y_pixels=1, z_pixels=1, xlim=(-1, 1), ylim=(-1, 1),
-                                    zlim=(-1, 1), dens_weight=dens_weight, normalize=False)
+                                    zlim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight3d * sdf_2['A'][0] * kernel.w(0, 3)
 
-        image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False)
+        image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1), dens_weight=dens_weight, normalize=False, hmin=False)
         assert image[0] == weight3d * sdf_2['A'][0] * kernel.w(0, 3)
 
 
-
 @mark.parametrize("backend", backends)
 def test_normalize_interpolation(backend):
     sdf_2 = SarracenDataFrame({'x': [0], 'y': [0], 'A': [2], 'B': [3], 'h': [0.5], 'rho': [0.25], 'm': [0.75]},
                               params=dict())
     sdf_3 = SarracenDataFrame({'x': [0], 'y': [0], 'z': [0], 'A': [2], 'B': [3], 'C': [4], 'h': [0.5], 'rho': [0.25],
                                'm': [0.75]}, params=dict())
 
@@ -1353,7 +1352,146 @@
                                     zlim=(-1, 1), dens_weight=False, normalize=normalize)
         assert image[0] == weight3d * sdf_2['A'][0] / norm3d
 
         image = interpolate_3d_line(sdf_3, 'A', pixels=1, xlim=(-1, 1), ylim=(-1, 1),
                                     dens_weight=False, normalize=normalize)
         assert image[0] == weight3d * sdf_2['A'][0] / norm3d
 
+
+@mark.parametrize("backend", backends)
+def test_exact_interpolation_culling(backend):
+    sdf_2 = SarracenDataFrame({'x': [0], 'y': [0], 'A': [2], 'h': [0.4], 'rho': [0.1], 'm': [1]}, params=dict())
+    sdf_2.backend = backend
+    sdf_3 = SarracenDataFrame({'x': [0], 'y': [0], 'z': [0], 'A': [2], 'h': [0.4], 'rho': [0.1], 'm': [1]},
+                              params=dict())
+    sdf_3.backend = backend
+
+    image_2 = sdf_2.sph_interpolate('A', xlim=(-1, 1), ylim=(-1, 1), x_pixels=5, exact=True)
+    image_3 = interpolate_3d_proj(sdf_3, 'A', xlim=(-1, 1), ylim=(-1, 1), x_pixels=5, exact=True)
+
+    assert image_2[2, 4] != 0
+    assert image_3[2, 4] != 0
+
+
+@mark.parametrize("backend", backends)
+def test_minimum_smoothing_length_2d(backend):
+    """ Test that the minimum smoothing length evaluates correctly. """
+
+    pixels = 5
+    xlim, ylim = (-1, 1), (-1, 1)
+    hmin = 0.5 * (xlim[1] - xlim[0]) / pixels
+
+    sdf_a = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'h': [hmin, hmin, 0.3, 0.25, hmin, hmin, 0.2, hmin],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_b = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'h': [0.01, 0.01, 0.3, 0.25, 0.01, 0.01, 0.2, 0.01],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_a.backend = backend
+    sdf_b.backend = backend
+
+    for interpolate in [interpolate_2d]:
+        grid = interpolate(data=sdf_a, target='rho', xlim=xlim, ylim=ylim, x_pixels=pixels, y_pixels=pixels,
+                           normalize=False, hmin=False)
+        grid_hmin = interpolate(data=sdf_b, target='rho', xlim=xlim, ylim=ylim, x_pixels=pixels, y_pixels=pixels,
+                                normalize=False, hmin=True)
+
+        assert (grid == grid_hmin).all()
+
+
+@mark.parametrize("backend", backends)
+def test_minimum_smoothing_length_3d(backend):
+    """ Test that the minimum smoothing length evaluates correctly. """
+
+    pixels = 5
+    xlim, ylim = (-1, 1), (-1, 1)
+    hmin = 0.5 * (xlim[1] - xlim[0]) / pixels
+
+    sdf_a = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'rz': [0.1, 0.32, 0.03, -0.3, -0.2, 0.1, -0.06, 0.22],
+                                             'h': [hmin, hmin, 0.3, 0.25, hmin, hmin, 0.2, hmin],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_b = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'rz': [0.1, 0.32, 0.03, -0.3, -0.2, 0.1, -0.06, 0.22],
+                                             'h': [0.01, 0.01, 0.3, 0.25, 0.01, 0.01, 0.2, 0.01],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_a.backend = backend
+    sdf_b.backend = backend
+
+    for interpolate in [interpolate_3d_cross, interpolate_3d_proj, interpolate_3d_grid]:
+        grid = interpolate(data=sdf_a, target='rho', xlim=xlim, ylim=ylim, x_pixels=pixels, y_pixels=pixels,
+                           normalize=False, hmin=False)
+        grid_hmin = interpolate(data=sdf_b, target='rho', xlim=xlim, ylim=ylim, x_pixels=pixels, y_pixels=pixels,
+                                normalize=False, hmin=True)
+
+        assert (grid == grid_hmin).all()
+
+
+@mark.parametrize("backend", backends)
+def test_minimum_smoothing_length_1d_lines(backend):
+    """ Test that the minimum smoothing length evaluates correctly. """
+
+    pixels = 5
+    xlim, ylim, zlim = (-1, 1), (-0.5, 0.5), (-0.5, 0.5)
+
+    hmin = 0.5 * np.sqrt((xlim[1] - xlim[0]) ** 2 + (ylim[1] - ylim[0]) ** 2) / pixels
+
+    sdf_a = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'h': [hmin, hmin, 0.3, 0.25, hmin, hmin, hmin, hmin],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_b = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'h': [0.01, 0.01, 0.3, 0.25, 0.01, 0.01, 0.2, 0.01],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_a.backend = backend
+    sdf_b.backend = backend
+
+    grid = interpolate_2d_line(data=sdf_a, target='rho', xlim=xlim, ylim=ylim, pixels=pixels,
+                               normalize=False, hmin=False)
+    grid_hmin = interpolate_2d_line(data=sdf_b, target='rho', xlim=xlim, ylim=ylim, pixels=pixels,
+                                    normalize=False, hmin=True)
+
+    assert (grid == grid_hmin).all()
+
+    hmin = 0.5 * np.sqrt((xlim[1] - xlim[0]) ** 2 + (ylim[1] - ylim[0]) ** 2 + (zlim[1] - zlim[0]) ** 2) / pixels
+
+    sdf_a = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'rz': [0.1, 0.32, 0.03, -0.3, -0.2, 0.1, -0.06, 0.22],
+                                             'h': [hmin, hmin, 0.3, 0.25, hmin, hmin, hmin, hmin],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_b = SarracenDataFrame(data={'rx': [0.3, -0.1, 0.1, 0.1, 0.05, -0.05, -0.25, -0.2],
+                                             'ry': [0.0, 0.1, -0.1, 0.0, -0.05, 0.07, -0.3, -0.2],
+                                             'rz': [0.1, 0.32, 0.03, -0.3, -0.2, 0.1, -0.06, 0.22],
+                                             'h': [0.01, 0.01, 0.3, 0.25, 0.01, 0.01, 0.2, 0.01],
+                                             'm': [0.56] * 8},
+                                       params={'hfact': 1.2})
+
+    sdf_a.backend = backend
+    sdf_b.backend = backend
+
+    grid = interpolate_3d_line(data=sdf_a, target='rho', xlim=xlim, ylim=ylim, zlim=zlim, pixels=pixels,
+                               normalize=False, hmin=False)
+    grid_hmin = interpolate_3d_line(data=sdf_b, target='rho', xlim=xlim, ylim=ylim, zlim=zlim, pixels=pixels,
+                                    normalize=False, hmin=True)
+
+    assert (grid == grid_hmin).all()
+
```

### Comparing `sarracen-1.1/sarracen/tests/test_kernels.py` & `sarracen-1.2.0/sarracen/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/tests/test_render.py` & `sarracen-1.2.0/sarracen/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/sarracen/tests/test_sarracen_dataframe.py` & `sarracen-1.2.0/sarracen/tests/test_sarracen_dataframe.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.1/PKG-INFO` & `sarracen-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarracen
-Version: 1.1
+Version: 1.2.0
 Summary: SPH analysis and visualization
 Author-email: "Terrence S. Tricco" <tstricco@mun.ca>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: numba>=0.55.1
 Requires-Dist: pandas>=1.4
```

