# Comparing `tmp/monashspa-1.9.4.tar.gz` & `tmp/monashspa-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monashspa-1.9.4.tar", last modified: Fri Feb 24 03:59:48 2023, max compression
+gzip compressed data, was "monashspa-1.9.9.tar", last modified: Mon Apr 17 05:37:11 2023, max compression
```

## Comparing `monashspa-1.9.4.tar` & `monashspa-1.9.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.056664 monashspa-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-02-24 03:59:08.000000 monashspa-1.9.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-24 03:59:48.056664 monashspa-1.9.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.036664 monashspa-1.9.4/monashspa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.040664 monashspa-1.9.4/monashspa/PHS1011/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS1011/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.044664 monashspa-1.9.4/monashspa/PHS2061/
--rw-r--r--   0 runner    (1001) docker     (123)   414641 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)  1071220 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Guitar_Pluck.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1546304 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Synthesiser.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Synthesiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/PHS20x1UncertaintiesData.csv
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2061/fitting_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.048664 monashspa-1.9.4/monashspa/PHS2062/
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_chisquare_illustration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_data_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_fit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_short_2_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_short_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/PHS2062_pendulum_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2062/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.048664 monashspa-1.9.4/monashspa/PHS2081/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS2081/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3000/
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/PET.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/betaray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/holes_in_ge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/microwave_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/mossbauer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/muon.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/optical_tweezers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/reflex_klystron.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/resistivity_germanium.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/rubidium_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/thermoelectricity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3000/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/tutorials/PHS3000UncertaintiesData.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3000/tutorials/fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3302/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3302/calorimeter/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121585 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/calorimeter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/calorimeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/calorimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.052664 monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/d0_lifetime.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15723 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/d0_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-24 03:59:47.000000 monashspa-1.9.4/monashspa/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.056664 monashspa-1.9.4/monashspa/common/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/admca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/download_gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/common/picoscope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.056664 monashspa-1.9.4/monashspa/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.056664 monashspa-1.9.4/monashspa/tests/PHS2061/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/PHS2061/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/PHS2061/fitting_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.056664 monashspa-1.9.4/monashspa/tests/PHS3000/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/PHS3000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/PHS3000/fitting_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/PHS3000/optical_tweezers.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-02-24 03:59:08.000000 monashspa-1.9.4/monashspa/tests/testing_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:59:48.040664 monashspa-1.9.4/monashspa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-24 03:59:48.000000 monashspa-1.9.4/monashspa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-02-24 03:59:48.000000 monashspa-1.9.4/monashspa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 03:59:48.000000 monashspa-1.9.4/monashspa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-24 03:59:48.000000 monashspa-1.9.4/monashspa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-24 03:59:48.000000 monashspa-1.9.4/monashspa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 03:59:48.056664 monashspa-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-02-24 03:59:08.000000 monashspa-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-04-17 05:36:34.000000 monashspa-1.9.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 05:37:11.721417 monashspa-1.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.709417 monashspa-1.9.9/monashspa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.709417 monashspa-1.9.9/monashspa/PHS1011/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS1011/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.713417 monashspa-1.9.9/monashspa/PHS2061/
+-rw-r--r--   0 runner    (1001) docker     (123)   414641 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1071220 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Guitar_Pluck.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1546304 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Synthesiser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Synthesiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/PHS20x1UncertaintiesData.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2061/fitting_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS2062/
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_chisquare_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_data_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_fit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_short_2_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_short_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/PHS2062_pendulum_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2062/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS2081/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS2081/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS3000/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/PET.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/betaray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/holes_in_ge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/microwave_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/mossbauer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/muon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/optical_tweezers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/reflex_klystron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/resistivity_germanium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/rubidium_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/thermoelectricity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS3000/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/tutorials/PHS3000UncertaintiesData.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3000/tutorials/fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS3302/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS3302/calorimeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121585 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/calorimeter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/calorimeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.717417 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/calorimeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/d0_lifetime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15723 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/d0_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/monashspa/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/admca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/download_gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/common/picoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/monashspa/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/monashspa/tests/PHS2061/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/PHS2061/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/PHS2061/fitting_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.721417 monashspa-1.9.9/monashspa/tests/PHS3000/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/PHS3000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/PHS3000/fitting_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/PHS3000/optical_tweezers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 05:36:34.000000 monashspa-1.9.9/monashspa/tests/testing_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:11.709417 monashspa-1.9.9/monashspa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 05:37:11.000000 monashspa-1.9.9/monashspa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:37:11.721417 monashspa-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-17 05:36:34.000000 monashspa-1.9.9/setup.py
```

### Comparing `monashspa-1.9.4/COPYING` & `monashspa-1.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/PKG-INFO` & `monashspa-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monashspa
-Version: 1.9.4
+Version: 1.9.9
 Summary: Library of useful data analysis tools for Monash University Physics & Astronomy students
 Home-page: https://monashspa.readthedocs.io
 Author: School of Physics & Astronomy, Monash University
 License: GPLv3
 Project-URL: Documentation, https://monashspa.readthedocs.io
 Project-URL: Source Code, https://github.com/Monash-University-Physics-Astronomy/monashspa
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `monashspa-1.9.4/monashspa/PHS1011/__init__.py` & `monashspa-1.9.9/monashspa/PHS1011/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.ipynb` & `monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.py` & `monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Fourier_Analysis.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Guitar_Pluck.wav` & `monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Guitar_Pluck.wav`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Synthesiser.ipynb` & `monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Synthesiser.ipynb`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS2061_Q3_Synthesiser.py` & `monashspa-1.9.9/monashspa/PHS2061/PHS2061_Q3_Synthesiser.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/PHS20x1UncertaintiesData.csv` & `monashspa-1.9.9/monashspa/PHS2061/PHS20x1UncertaintiesData.csv`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/__init__.py` & `monashspa-1.9.9/monashspa/PHS2061/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2061/fitting_tutorial.py` & `monashspa-1.9.9/monashspa/PHS2061/fitting_tutorial.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_chisquare_illustration.py` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_chisquare_illustration.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_data_creation.py` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_data_creation.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_data.csv` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_data.csv`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_fit.ipynb` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_fit.ipynb`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_fit.py` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_fit.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_gas_short_2_data.csv` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_gas_short_2_data.csv`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/PHS2062_pendulum_fit.py` & `monashspa-1.9.9/monashspa/PHS2062/PHS2062_pendulum_fit.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2062/__init__.py` & `monashspa-1.9.9/monashspa/PHS2062/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS2081/__init__.py` & `monashspa-1.9.9/monashspa/PHS2081/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/PET.py` & `monashspa-1.9.9/monashspa/PHS3000/PET.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/__init__.py` & `monashspa-1.9.9/monashspa/PHS3000/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/betaray.py` & `monashspa-1.9.9/monashspa/PHS3000/betaray.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/holes_in_ge.py` & `monashspa-1.9.9/monashspa/PHS3000/holes_in_ge.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/microwave_transmission.py` & `monashspa-1.9.9/monashspa/PHS3000/microwave_transmission.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/mossbauer.py` & `monashspa-1.9.9/monashspa/PHS3000/mossbauer.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/muon.py` & `monashspa-1.9.9/monashspa/PHS3000/muon.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/optical_tweezers.py` & `monashspa-1.9.9/monashspa/PHS3000/optical_tweezers.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/reflex_klystron.py` & `monashspa-1.9.9/monashspa/PHS3000/reflex_klystron.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/resistivity_germanium.py` & `monashspa-1.9.9/monashspa/PHS3000/resistivity_germanium.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/rubidium_spectroscopy.py` & `monashspa-1.9.9/monashspa/PHS3000/rubidium_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/thermoelectricity.py` & `monashspa-1.9.9/monashspa/PHS3000/thermoelectricity.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/tutorials/PHS3000UncertaintiesData.csv` & `monashspa-1.9.9/monashspa/PHS3000/tutorials/PHS3000UncertaintiesData.csv`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3000/tutorials/__init__.py` & `monashspa-1.9.9/monashspa/PHS3000/tutorials/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 
 from ..optical_tweezers import trap_k_theory as __trap_k_theory
 
 def model_1(r, w, I):
     # scale parameters
     r = r*1e-3
     w = w*1e-4
-    I = I*1e11
+    I = 4/1.11803*I*1e11
     
     # set parameters we are not exposing
     eccentricity = 1.1
     alpha = 1.25
 
-    return __trap_k_theory(r, w, alpha, eccentricity, I)
+    return __trap_k_theory(r, w, alpha, eccentricity, I)
```

### Comparing `monashspa-1.9.4/monashspa/PHS3000/tutorials/fitting.py` & `monashspa-1.9.9/monashspa/PHS3000/tutorials/fitting.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/__init__.py` & `monashspa-1.9.9/monashspa/PHS3302/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/__init__.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/calorimeter.ipynb` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/calorimeter.ipynb`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/calorimeter.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/calorimeter.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/calorimeter.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/calorimeter.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/layer.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/layer.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/particle.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/particle.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/calorimeter/model/simulation.py` & `monashspa-1.9.9/monashspa/PHS3302/calorimeter/model/simulation.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/__init__.py` & `monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/d0_lifetime.ipynb` & `monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/d0_lifetime.ipynb`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/PHS3302/d0_lifetime/d0_lifetime.py` & `monashspa-1.9.9/monashspa/PHS3302/d0_lifetime/d0_lifetime.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/__init__.py` & `monashspa-1.9.9/monashspa/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/__init__.py` & `monashspa-1.9.9/monashspa/common/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/admca.py` & `monashspa-1.9.9/monashspa/common/admca.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/csv_reader.py` & `monashspa-1.9.9/monashspa/common/csv_reader.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/download_gdrive.py` & `monashspa-1.9.9/monashspa/common/download_gdrive.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/figures.py` & `monashspa-1.9.9/monashspa/common/figures.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/fitting.py` & `monashspa-1.9.9/monashspa/common/fitting.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/common/picoscope.py` & `monashspa-1.9.9/monashspa/common/picoscope.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/PHS2061/__init__.py` & `monashspa-1.9.9/monashspa/tests/PHS2061/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/PHS2061/fitting_tutorial.py` & `monashspa-1.9.9/monashspa/tests/PHS2061/fitting_tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         'A_0': 20.573035990441486,
         'u_A_0': 0.6181473325960677,
         'l': 0.005004779941925933,
         'u_l': 0.00015840653659960648,
         'halflife': 138.49703455557113,
         'u_halflife': 4.38357646646529,
     }
-    precision = 2e-7
+    precision = 1e-3
     
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def nonlinear_fit_with_independent_as_t():
@@ -78,15 +78,15 @@
         'A_0': 20.573035990441486,
         'u_A_0': 0.6181473325960677,
         'l': 0.005004779941925933,
         'u_l': 0.00015840653659960648,
         'halflife': 138.49703455557113,
         'u_halflife': 4.38357646646529,
     }
-    precision = 2e-7
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit_model():
@@ -116,15 +116,15 @@
         'm': -0.004897938859868103,
         'u_m': 0.0001633020007207088,
         'halflife': 141.51813658584769,
         'u_halflife': 4.718351025589936,
         'A_0': 20.664948544330286,
         'u_A_0': 0.6327709546990624,
     }
-    precision = 1e-5
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit():
@@ -146,15 +146,15 @@
     ### Expected results ###
     expected_results = {
         'intercept': 3.02843895796932,
         'u_intercept': 0.030620495054301592,
         'slope': -0.004897938859868103,
         'u_slope': 0.0001633020007207088,
     }
-    precision = 1e-7
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def do_tests():
@@ -175,8 +175,8 @@
         print('')
         print('    There were {num_failures:d} failed PHS2061 fitting tests'.format(num_failures=len(failed_tests)))
     print('')
 
     return failed_tests
 
 if __name__ == "__main__":
-    do_tests()
+    do_tests()
```

### Comparing `monashspa-1.9.4/monashspa/tests/PHS3000/__init__.py` & `monashspa-1.9.9/monashspa/tests/PHS3000/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/PHS3000/fitting_tutorial.py` & `monashspa-1.9.9/monashspa/tests/PHS3000/fitting_tutorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         'A_0': 20.573035990441486,
         'u_A_0': 0.6181473325960677,
         'l': 0.005004779941925933,
         'u_l': 0.00015840653659960648,
         'halflife': 138.49703455557113,
         'u_halflife': 4.38357646646529,
     }
-    precision = 2e-7
+    precision = 1e-3
     
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def nonlinear_fit_with_independent_as_t():
@@ -78,15 +78,15 @@
         'A_0': 20.573035990441486,
         'u_A_0': 0.6181473325960677,
         'l': 0.005004779941925933,
         'u_l': 0.00015840653659960648,
         'halflife': 138.49703455557113,
         'u_halflife': 4.38357646646529,
     }
-    precision = 2e-7
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit_model():
@@ -116,15 +116,15 @@
         'm': -0.004897938859868103,
         'u_m': 0.0001633020007207088,
         'halflife': 141.51813658584769,
         'u_halflife': 4.718351025589936,
         'A_0': 20.664948544330286,
         'u_A_0': 0.6327709546990624,
     }
-    precision = 1e-5
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit():
@@ -146,15 +146,15 @@
     ### Expected results ###
     expected_results = {
         'intercept': 3.02843895796932,
         'u_intercept': 0.030620495054301592,
         'slope': -0.004897938859868103,
         'u_slope': 0.0001633020007207088,
     }
-    precision = 1e-7
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit_dual_custom_model():
@@ -186,15 +186,15 @@
         'm': -0.004897938859868103,
         'u_m': 0.0001633020007207088,
         'halflife': 141.51813658584769,
         'u_halflife': 4.718351025589936,
         'A_0': 20.664948544330286,
         'u_A_0': 0.6327709546990624,
     }
-    precision = 1e-5
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def linear_fit_dual_custom_named_model():
@@ -226,15 +226,15 @@
         'm1m': -0.004897938859868103,
         'u_m1m': 0.0001633020007207088,
         'halflife': 141.51813658584769,
         'u_halflife': 4.718351025589936,
         'A_0': 20.664948544330286,
         'u_A_0': 0.6327709546990624,
     }
-    precision = 1e-5
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def non_linear_fit_part_c():
@@ -275,15 +275,15 @@
         'D2': 6.705149651134903, 
         'u_D2': 0.14122328218157232, 
         'c': 2.636117481366362, 
         'u_c': 0.06764023986252798, 
         'FWHM': 4.311684392863958, 
         'u_FWHM': 0.045406161696634036
     }
-    precision = 1e-5
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def nonlinear_fit_part_c2():
```

### Comparing `monashspa-1.9.4/monashspa/tests/PHS3000/optical_tweezers.py` & `monashspa-1.9.9/monashspa/tests/PHS3000/optical_tweezers.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/__init__.py` & `monashspa-1.9.9/monashspa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/__main__.py` & `monashspa-1.9.9/monashspa/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa/tests/fitting.py` & `monashspa-1.9.9/monashspa/tests/fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ### Expected results ###
     expected_results = {
         'slope': 1.903875935,
         'u_slope': 0.045590672,
         'intercept': 1.011763758,
         'u_intercept': 0.177550159,
     }
-    precision = 1e-7
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 
@@ -75,15 +75,15 @@
     ### Expected results (from WFIT) ###
     expected_results = {
         'slope': 1.866046353,
         'u_slope': 0.064841588,
         'intercept': 1.124423955,
         'u_intercept': 0.387570521,
     }
-    precision = 2e-8
+    precision = 1e-3
 
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def test_failed_fit_1():
@@ -134,15 +134,15 @@
         'A_0': 20.573035990441486,
         'u_A_0': 0.6181473325960677,
         'l': 0.005004779941925933,
         'u_l': 0.00015840653659960648,
         'halflife': 138.49703455557113,
         'u_halflife': 4.38357646646529,
     }
-    precision = 2e-7
+    precision = 1e-3
     
     ### Check results match within precision ###
     success = compare_dictionary(results, expected_results, precision)
 
     return success
 
 def test_failed_fit_2():
@@ -188,8 +188,8 @@
         print('    There were {num_failures:d} failed common fitting tests'.format(num_failures=len(failed_tests)))
         
     print('')
 
     return failed_tests
 
 if __name__ == "__main__":
-    do_tests()
+    do_tests()
```

### Comparing `monashspa-1.9.4/monashspa/tests/testing_helpers.py` & `monashspa-1.9.9/monashspa/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/monashspa.egg-info/PKG-INFO` & `monashspa-1.9.9/monashspa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monashspa
-Version: 1.9.4
+Version: 1.9.9
 Summary: Library of useful data analysis tools for Monash University Physics & Astronomy students
 Home-page: https://monashspa.readthedocs.io
 Author: School of Physics & Astronomy, Monash University
 License: GPLv3
 Project-URL: Documentation, https://monashspa.readthedocs.io
 Project-URL: Source Code, https://github.com/Monash-University-Physics-Astronomy/monashspa
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `monashspa-1.9.4/monashspa.egg-info/SOURCES.txt` & `monashspa-1.9.9/monashspa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monashspa-1.9.4/setup.py` & `monashspa-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 # Define the current version of the library
 # Update this before building and publishing a new version
 # see https://semver.org/ for guidelines on how to modify the version string
-VERSION = '1.9.4'
+VERSION = '1.9.9'
 # version information generated by our GitHub Action (see .github/workflows/release.yml)
 CURRENT_TAG = os.environ.get('GHA_TAG_VERSION')
 CURRENT_GIT_COMMIT_HASH = os.environ.get('GHA_GIT_COMMIT')
 if CURRENT_TAG is not None:
     print('GitHub Action debug: tag=', CURRENT_TAG)
 if CURRENT_GIT_COMMIT_HASH is not None:
     print('GitHub Action debug: git hash=', CURRENT_GIT_COMMIT_HASH)
```

