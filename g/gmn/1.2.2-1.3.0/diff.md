# Comparing `tmp/gmn-1.2.2.tar.gz` & `tmp/gmn-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmn-1.2.2.tar", last modified: Sun Apr  9 13:24:15 2023, max compression
+gzip compressed data, was "gmn-1.3.0.tar", last modified: Mon Apr 17 04:21:22 2023, max compression
```

## Comparing `gmn-1.2.2.tar` & `gmn-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1230 2023-01-22 19:41:24.028603 gmn-1.2.2/LICENSE
--rw-r--r--   0        0        0     1322 2023-01-29 07:05:47.285818 gmn-1.2.2/README.md
--rw-r--r--   0        0        0       13 2023-01-27 13:57:37.995327 gmn-1.2.2/gmn/.gitignore
--rw-r--r--   0        0        0     6699 2023-03-08 04:49:52.241122 gmn-1.2.2/gmn/Auxiliary.py
--rw-r--r--   0        0        0     3046 2023-01-25 03:48:19.264248 gmn-1.2.2/gmn/CLI_Parser.py
--rw-r--r--   0        0        0      392 2023-03-04 06:39:05.624426 gmn-1.2.2/gmn/Common.py
--rw-r--r--   0        0        0     3431 2023-03-06 08:51:20.000000 gmn-1.2.2/gmn/ConfigParser.py
--rw-r--r--   0        0        0     5833 2023-03-26 13:38:02.501344 gmn-1.2.2/gmn/Forecast.py
--rw-r--r--   0        0        0     7046 2023-03-05 16:51:46.316401 gmn-1.2.2/gmn/GMN.py
--rw-r--r--   0        0        0    10032 2023-04-09 13:11:22.241734 gmn-1.2.2/gmn/Generate.py
--rw-r--r--   0        0        0     4659 2023-03-03 05:23:53.492313 gmn-1.2.2/gmn/Network.py
--rw-r--r--   0        0        0     7553 2023-03-19 14:58:48.732784 gmn-1.2.2/gmn/Node.py
--rw-r--r--   0        0        0     4328 2023-02-08 08:59:39.839083 gmn-1.2.2/gmn/Parameters.py
--rw-r--r--   0        0        0     8182 2023-02-10 19:21:31.793640 gmn-1.2.2/gmn/Plot.py
--rw-r--r--   0        0        0      504 2023-01-23 10:49:28.000000 gmn-1.2.2/gmn/__init__.py
--rw-r--r--   0        0        0      802 2023-04-09 10:57:16.607135 gmn-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       13 2023-02-03 10:09:54.014690 gmn-1.2.2/tests/.gitignore
--rw-r--r--   0        0        0     1264 2023-02-09 04:47:08.694737 gmn-1.2.2/tests/A.cfg
--rw-r--r--   0        0        0    12332 2023-02-09 04:59:26.061315 gmn-1.2.2/tests/DataOut_ABCD_A1_CMI_E7_tau-3.csv
--rw-r--r--   0        0        0    12304 2023-02-03 08:52:46.847535 gmn-1.2.2/tests/DataOut_ABCD_CMI_E7_tau-3.csv
--rw-r--r--   0        0        0    12330 2023-03-07 19:41:05.403257 gmn-1.2.2/tests/DataOut_ABCD_Forecast_E7_tau-3.csv
--rw-r--r--   0        0        0     1237 2023-03-07 17:11:16.942370 gmn-1.2.2/tests/gmn_forecast1.cfg
--rw-r--r--   0        0        0     1227 2023-02-09 04:46:13.606204 gmn-1.2.2/tests/gmn_test1.cfg
--rw-r--r--   0        0        0     1236 2023-02-09 05:09:36.048791 gmn-1.2.2/tests/gmn_test_readNode.cfg
--rw-r--r--   0        0        0     3980 2023-03-11 09:50:45.149403 gmn-1.2.2/tests/tests.py
--rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 gmn-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1317 2023-04-17 04:15:50.482039 gmn-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1322 2023-01-29 07:05:47.285818 gmn-1.3.0/README.md
+-rw-r--r--   0        0        0       13 2023-01-27 13:57:37.995327 gmn-1.3.0/gmn/.gitignore
+-rw-r--r--   0        0        0     6699 2023-03-08 04:49:52.241122 gmn-1.3.0/gmn/Auxiliary.py
+-rw-r--r--   0        0        0     3287 2023-04-16 19:40:31.153505 gmn-1.3.0/gmn/CLI_Parser.py
+-rw-r--r--   0        0        0      392 2023-03-04 06:39:05.624426 gmn-1.3.0/gmn/Common.py
+-rw-r--r--   0        0        0     3431 2023-03-06 08:51:20.000000 gmn-1.3.0/gmn/ConfigParser.py
+-rw-r--r--   0        0        0     5833 2023-03-26 13:38:02.501344 gmn-1.3.0/gmn/Forecast.py
+-rw-r--r--   0        0        0     7046 2023-04-14 09:11:50.258819 gmn-1.3.0/gmn/GMN.py
+-rw-r--r--   0        0        0    10032 2023-04-09 13:11:22.241734 gmn-1.3.0/gmn/Generate.py
+-rw-r--r--   0        0        0     4659 2023-03-03 05:23:53.492313 gmn-1.3.0/gmn/Network.py
+-rw-r--r--   0        0        0     7475 2023-04-16 18:51:39.171110 gmn-1.3.0/gmn/Node.py
+-rw-r--r--   0        0        0     4328 2023-02-08 08:59:39.839083 gmn-1.3.0/gmn/Parameters.py
+-rw-r--r--   0        0        0     8182 2023-02-10 19:21:31.793640 gmn-1.3.0/gmn/Plot.py
+-rw-r--r--   0        0        0      504 2023-01-23 10:49:28.000000 gmn-1.3.0/gmn/__init__.py
+-rw-r--r--   0        0        0      802 2023-04-16 18:44:18.777846 gmn-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-02-03 10:09:54.014690 gmn-1.3.0/tests/.gitignore
+-rw-r--r--   0        0        0     1264 2023-02-09 04:47:08.694737 gmn-1.3.0/tests/A.cfg
+-rw-r--r--   0        0        0    12332 2023-02-09 04:59:26.061315 gmn-1.3.0/tests/DataOut_ABCD_A1_CMI_E7_tau-3.csv
+-rw-r--r--   0        0        0    12304 2023-02-03 08:52:46.847535 gmn-1.3.0/tests/DataOut_ABCD_CMI_E7_tau-3.csv
+-rw-r--r--   0        0        0    12330 2023-03-07 19:41:05.403257 gmn-1.3.0/tests/DataOut_ABCD_Forecast_E7_tau-3.csv
+-rw-r--r--   0        0        0     1237 2023-03-07 17:11:16.942370 gmn-1.3.0/tests/gmn_forecast1.cfg
+-rw-r--r--   0        0        0     1227 2023-02-09 04:46:13.606204 gmn-1.3.0/tests/gmn_test1.cfg
+-rw-r--r--   0        0        0     1236 2023-02-09 05:09:36.048791 gmn-1.3.0/tests/gmn_test_readNode.cfg
+-rw-r--r--   0        0        0     3980 2023-03-11 09:50:45.149403 gmn-1.3.0/tests/tests.py
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 gmn-1.3.0/PKG-INFO
```

### Comparing `gmn-1.2.2/LICENSE` & `gmn-1.3.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Copyright 2023 OIST Biologic Nonlinear Dynamics Data Science Unit.
+Copyright 2023 Gerald Pao.
 All Rights Reserved.
 
 Permission to copy, modify, and distribute this software and its
 documentation for educational, research and non-profit purposes,
 without fee, and without a written agreement is hereby granted,
 provided that the above copyright notice, this paragraph and the
 following three paragraphs appear in all copies.
 
 Those desiring to incorporate this software into commercial products
-or use for commercial purposes should contact: GERALD.PAO@OIST.JP
+or use for commercial purposes should contact: GeraldPao@gmail.com
 
-IN NO EVENT SHALL OIST BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT,
-SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS,
-ARISING OUT OF THE USE OF THIS SOFTWARE, EVEN IF OIST HAS BEEN ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
+IN NO EVENT SHALL GERALD PAO, SPONSORS, OR DEVELOPERS OF THE SOFTWARE
+BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR
+CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF OIST HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGE.
  
-THE SOFTWARE PROVIDED HEREIN IS ON AN "AS IS" BASIS, AND OIST HAS NO
-OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
-MODIFICATIONS. OIST MAKES NO REPRESENTATIONS AND EXTENDS NO WARRANTIES
-OF ANY KIND, EITHER IMPLIED OR EXPRESS, INCLUDING, BUT NOT LIMITED
+THE SOFTWARE PROVIDED HEREIN IS ON AN "AS IS" BASIS, AND GERALD PAO,
+SPONSORS, OR DEVELOPERS OF THE SOFTWARE HAVE NO OBLIGATION TO PROVIDE
+MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS. GERALD PAO,
+SPONSORS, AND DEVELOPERS MAKE NO REPRESENTATION AND EXTEND NO WARRANTIES
+OF ANY KIND, EITHER IMPLIED OR EXPRESSED, INCLUDING, BUT NOT LIMITED
 TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A
 PARTICULAR PURPOSE, OR THAT THE USE OF THE SOFTWARE WILL NOT
 INFRINGE ANY PATENT, TRADEMARK OR OTHER RIGHTS.
```

### Comparing `gmn-1.2.2/README.md` & `gmn-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Auxiliary.py` & `gmn-1.3.0/gmn/Auxiliary.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/CLI_Parser.py` & `gmn-1.3.0/gmn/CLI_Parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 
     parser.add_argument('-c', '--cores',
                         dest    = 'cores', type = int, 
                         action  = 'store',
                         default = 4,
                         help    = 'Multiprocessing cores.')
 
+    parser.add_argument('-t', '--threads',
+                        dest    = 'threads', type = int,
+                        action  = 'store',
+                        default = 2,
+                        help    = 'OpenMP threads (kedm).')
+
     parser.add_argument('-P', '--Plot',
                         dest    = 'Plot',
                         action  = 'store_true',
                         default = False,
                         help    = 'Plot.')
 
     parser.add_argument('-S', '--StatePlot',
```

### Comparing `gmn-1.2.2/gmn/ConfigParser.py` & `gmn-1.3.0/gmn/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Forecast.py` & `gmn-1.3.0/gmn/Forecast.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/GMN.py` & `gmn-1.3.0/gmn/GMN.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Generate.py` & `gmn-1.3.0/gmn/Generate.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Network.py` & `gmn-1.3.0/gmn/Network.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Node.py` & `gmn-1.3.0/gmn/Node.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,16 @@
     from sklearn              import neighbors
     from sklearn.svm          import SVR
     from sklearn.linear_model import LinearRegression
 except ImportError as err:
     print( err, "SVR, knn, Linear not available" )
 
 try:
-    from os import environ # JP Need to query not hardwire
-    environ[ 'OMP_PROC_BIND' ] = 'spread'  # kedm : OpenMP settings
-    environ[ 'OMP_PLACES'    ] = 'threads'
+    from os import environ
+    environ[ 'OMP_PROC_BIND' ] = 'false' # Kokkos warning OpenMP
     from kedm import simplex as kedm_simplex
     from kedm import smap    as kedm_smap
 except ImportError as err:
     print( err, "kedm not available" )
 
 # Local modules 
 from gmn.ConfigParser import ReadConfig
```

### Comparing `gmn-1.2.2/gmn/Parameters.py` & `gmn-1.3.0/gmn/Parameters.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/gmn/Plot.py` & `gmn-1.3.0/gmn/Plot.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/pyproject.toml` & `gmn-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "matplotlib",
     "scikit-learn",
 ]
 build-backend = "pdm.pep517.api"
 
 [project]
 name = "gmn"
-version = "1.2.2"
+version = "1.3.0"
 authors = [
     { name = "Joseph Park", email = "JosephPark@IEEE.org" },
     { name = "Gerald Pao", email = "Gerald.Pao@OIST.jp" },
 ]
 description = "Generative Manifold Networks"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `gmn-1.2.2/tests/A.cfg` & `gmn-1.3.0/tests/A.cfg`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/DataOut_ABCD_A1_CMI_E7_tau-3.csv` & `gmn-1.3.0/tests/DataOut_ABCD_A1_CMI_E7_tau-3.csv`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/DataOut_ABCD_CMI_E7_tau-3.csv` & `gmn-1.3.0/tests/DataOut_ABCD_CMI_E7_tau-3.csv`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/DataOut_ABCD_Forecast_E7_tau-3.csv` & `gmn-1.3.0/tests/DataOut_ABCD_Forecast_E7_tau-3.csv`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/gmn_forecast1.cfg` & `gmn-1.3.0/tests/gmn_forecast1.cfg`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/gmn_test1.cfg` & `gmn-1.3.0/tests/gmn_test1.cfg`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/gmn_test_readNode.cfg` & `gmn-1.3.0/tests/gmn_test_readNode.cfg`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/tests/tests.py` & `gmn-1.3.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gmn-1.2.2/PKG-INFO` & `gmn-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmn
-Version: 1.2.2
+Version: 1.3.0
 Summary: Generative Manifold Networks
 Author-email: Joseph Park <JosephPark@IEEE.org>,Gerald Pao <Gerald.Pao@OIST.jp>
 Requires-Python: >=3.8
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Documentation, https://nonlineardynamicsdsu.github.io/gmn/
```

