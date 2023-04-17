# Comparing `tmp/iloscar-0.2.3b0.tar.gz` & `tmp/iloscar-0.2.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-0.2.3b0.tar", last modified: Mon Apr 17 20:38:34 2023, max compression
+gzip compressed data, was "iloscar-0.2.4b0.tar", last modified: Mon Apr 17 20:52:32 2023, max compression
```

## Comparing `iloscar-0.2.3b0.tar` & `iloscar-0.2.4b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:38:34.525909 iloscar-0.2.3b0/
--rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:38:34.525659 iloscar-0.2.3b0/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)    17746 2023-04-17 20:16:31.000000 iloscar-0.2.3b0/README.md
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:38:34.522825 iloscar-0.2.3b0/iloscar/
--rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.2.3b0/iloscar/__init__.py
--rw-rw-r--   0 shihan     (504) staff       (20)     1748 2023-04-17 20:31:15.000000 iloscar-0.2.3b0/iloscar/app.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:38:34.524109 iloscar-0.2.3b0/iloscar/dat_y0/
--rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.2.3b0/iloscar/dat_y0/petm_steady.dat
--rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.2.3b0/iloscar/dat_y0/preind_steady.dat
--rw-rw-r--   0 shihan     (504) staff       (20)   106518 2023-04-17 20:14:07.000000 iloscar-0.2.3b0/iloscar/iLOSCAR_backend.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:38:34.525083 iloscar-0.2.3b0/iloscar/pages/
--rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-17 20:15:49.000000 iloscar-0.2.3b0/iloscar/pages/Function.py
--rw-rw-r--   0 shihan     (504) staff       (20)    26246 2023-04-17 20:37:12.000000 iloscar-0.2.3b0/iloscar/pages/forward.py
--rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-17 20:15:56.000000 iloscar-0.2.3b0/iloscar/pages/home.py
--rw-rw-r--   0 shihan     (504) staff       (20)    46214 2023-04-17 20:25:57.000000 iloscar-0.2.3b0/iloscar/pages/inverse.py
--rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.2.3b0/iloscar/style.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:38:34.523715 iloscar-0.2.3b0/iloscar.egg-info/
--rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:38:34.000000 iloscar-0.2.3b0/iloscar.egg-info/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-17 20:38:34.000000 iloscar-0.2.3b0/iloscar.egg-info/SOURCES.txt
--rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-17 20:38:34.000000 iloscar-0.2.3b0/iloscar.egg-info/dependency_links.txt
--rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-17 20:38:34.000000 iloscar-0.2.3b0/iloscar.egg-info/requires.txt
--rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-17 20:38:34.000000 iloscar-0.2.3b0/iloscar.egg-info/top_level.txt
--rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-17 20:38:34.525971 iloscar-0.2.3b0/setup.cfg
--rw-r--r--   0 shihan     (504) staff       (20)     1451 2023-04-17 20:37:39.000000 iloscar-0.2.3b0/setup.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:52:32.073929 iloscar-0.2.4b0/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:52:32.073696 iloscar-0.2.4b0/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)    17746 2023-04-17 20:16:31.000000 iloscar-0.2.4b0/README.md
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:52:32.070873 iloscar-0.2.4b0/iloscar/
+-rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.2.4b0/iloscar/__init__.py
+-rw-rw-r--   0 shihan     (504) staff       (20)     1748 2023-04-17 20:31:15.000000 iloscar-0.2.4b0/iloscar/app.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:52:32.072174 iloscar-0.2.4b0/iloscar/dat_y0/
+-rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.2.4b0/iloscar/dat_y0/petm_steady.dat
+-rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.2.4b0/iloscar/dat_y0/preind_steady.dat
+-rw-rw-r--   0 shihan     (504) staff       (20)   106518 2023-04-17 20:14:07.000000 iloscar-0.2.4b0/iloscar/iLOSCAR_backend.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:52:32.073092 iloscar-0.2.4b0/iloscar/pages/
+-rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-17 20:15:49.000000 iloscar-0.2.4b0/iloscar/pages/Function.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    26246 2023-04-17 20:37:12.000000 iloscar-0.2.4b0/iloscar/pages/forward.py
+-rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-17 20:15:56.000000 iloscar-0.2.4b0/iloscar/pages/home.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    46215 2023-04-17 20:49:42.000000 iloscar-0.2.4b0/iloscar/pages/inverse.py
+-rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.2.4b0/iloscar/style.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:52:32.071759 iloscar-0.2.4b0/iloscar.egg-info/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:52:31.000000 iloscar-0.2.4b0/iloscar.egg-info/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-17 20:52:32.000000 iloscar-0.2.4b0/iloscar.egg-info/SOURCES.txt
+-rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-17 20:52:31.000000 iloscar-0.2.4b0/iloscar.egg-info/dependency_links.txt
+-rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-17 20:52:31.000000 iloscar-0.2.4b0/iloscar.egg-info/requires.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-17 20:52:31.000000 iloscar-0.2.4b0/iloscar.egg-info/top_level.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-17 20:52:32.073987 iloscar-0.2.4b0/setup.cfg
+-rw-r--r--   0 shihan     (504) staff       (20)     1451 2023-04-17 20:51:16.000000 iloscar-0.2.4b0/setup.py
```

### Comparing `iloscar-0.2.3b0/PKG-INFO` & `iloscar-0.2.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.2.3b0
+Version: 0.2.4b0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.2.3b0/README.md` & `iloscar-0.2.4b0/README.md`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/app.py` & `iloscar-0.2.4b0/iloscar/app.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/dat_y0/petm_steady.dat` & `iloscar-0.2.4b0/iloscar/dat_y0/petm_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/dat_y0/preind_steady.dat` & `iloscar-0.2.4b0/iloscar/dat_y0/preind_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/iLOSCAR_backend.py` & `iloscar-0.2.4b0/iloscar/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/pages/Function.py` & `iloscar-0.2.4b0/iloscar/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/pages/forward.py` & `iloscar-0.2.4b0/iloscar/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/pages/home.py` & `iloscar-0.2.4b0/iloscar/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar/pages/inverse.py` & `iloscar-0.2.4b0/iloscar/pages/inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
         if key == 'Success':
             return False, 'Progressing...'
     else:
         return True, []
 # run the model
 @callback(output = [ Output('info_integration_inv', 'children'), Output('ysol_inv', 'data'), Output('tsol_inv', 'data')],
         inputs = Input('progress_bar_inv','hidden'),
-        state = State('paramters_inv', 'data'),
+        state = State('parameters_inv', 'data'),
         background = True,
         running=[
        (Output("run_inv", "disabled"), True, False),
        (Output('cancel_run_inv', 'disabled'), False, True),
    ],
         progress = [Output('progress_bar_inv', 'value'), Output('progress_bar_inv', 'max')],
         cancel = [Input('cancel_run_inv','n_clicks')],
```

### Comparing `iloscar-0.2.3b0/iloscar/style.py` & `iloscar-0.2.4b0/iloscar/style.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.3b0/iloscar.egg-info/PKG-INFO` & `iloscar-0.2.4b0/iloscar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.2.3b0
+Version: 0.2.4b0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.2.3b0/setup.py` & `iloscar-0.2.4b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.3-beta'
+VERSION = '0.2.4-beta'
 DESCRIPTION = 'iLOSCAR'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar",
     version=VERSION,
```

