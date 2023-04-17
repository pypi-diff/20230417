# Comparing `tmp/asi4py-0.0.8.tar.gz` & `tmp/asi4py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asi4py-0.0.8.tar", last modified: Sun Jul 24 19:24:16 2022, max compression
+gzip compressed data, was "asi4py-0.0.9.tar", last modified: Mon Jul 25 15:16:35 2022, max compression
```

## Comparing `asi4py-0.0.8.tar` & `asi4py-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 19:24:16.752297 asi4py-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-07-19 20:58:13.000000 asi4py-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4435 2022-07-24 19:24:16.752297 asi4py-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 20:58:13.000000 asi4py-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-07-24 19:24:06.000000 asi4py-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-24 19:24:16.752297 asi4py-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 19:24:16.751297 asi4py-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 19:24:16.751297 asi4py-0.0.8/src/asi4py/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:16:07.000000 asi4py-0.0.8/src/asi4py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2022-07-20 15:54:10.000000 asi4py-0.0.8/src/asi4py/asecalc.py
--rw-rw-rw-   0 root         (0) root         (0)     6533 2022-07-22 17:47:20.000000 asi4py-0.0.8/src/asi4py/pyasi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 19:24:16.752297 asi4py-0.0.8/src/asi4py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4435 2022-07-24 19:24:16.000000 asi4py-0.0.8/src/asi4py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2022-07-24 19:24:16.000000 asi4py-0.0.8/src/asi4py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-24 19:24:16.000000 asi4py-0.0.8/src/asi4py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-24 19:24:16.000000 asi4py-0.0.8/src/asi4py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-07-24 19:24:16.000000 asi4py-0.0.8/src/asi4py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-25 15:16:35.158103 asi4py-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-07-19 20:58:13.000000 asi4py-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4435 2022-07-25 15:16:35.158103 asi4py-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 20:58:13.000000 asi4py-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      652 2022-07-25 15:00:32.000000 asi4py-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-07-25 15:16:35.158103 asi4py-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-25 15:16:35.157103 asi4py-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-25 15:16:35.158103 asi4py-0.0.9/src/asi4py/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:16:07.000000 asi4py-0.0.9/src/asi4py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2022-07-20 15:54:10.000000 asi4py-0.0.9/src/asi4py/asecalc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6458 2022-07-25 14:39:49.000000 asi4py-0.0.9/src/asi4py/pyasi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-25 15:16:35.158103 asi4py-0.0.9/src/asi4py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4435 2022-07-25 15:16:35.000000 asi4py-0.0.9/src/asi4py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2022-07-25 15:16:35.000000 asi4py-0.0.9/src/asi4py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-25 15:16:35.000000 asi4py-0.0.9/src/asi4py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-25 15:16:35.000000 asi4py-0.0.9/src/asi4py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-07-25 15:16:35.000000 asi4py-0.0.9/src/asi4py.egg-info/top_level.txt
```

### Comparing `asi4py-0.0.8/LICENSE` & `asi4py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asi4py-0.0.8/PKG-INFO` & `asi4py-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```

### Comparing `asi4py-0.0.8/README.md` & `asi4py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `asi4py-0.0.8/pyproject.toml` & `asi4py-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asi4py"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Pavel Stishenko", email="pstishenko@gmail.com" },
 ]
 description = "A Python wrapper for Atomic Simulation Interface API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `asi4py-0.0.8/src/asi4py/asecalc.py` & `asi4py-0.0.9/src/asi4py/asecalc.py`

 * *Files identical despite different names*

### Comparing `asi4py-0.0.8/src/asi4py/pyasi.py` & `asi4py-0.0.9/src/asi4py/pyasi.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,14 @@
   def close(self):
     curdir = os.getcwd()
     try:
       os.chdir(self.work_dir)
       self.lib.ASI_finalize()
       handle = self.lib._handle
       del self.lib
-      res = libdl.dlclose(handle)
-      assert res == 0, "dlclose = {res}"
       if self.mpi_comm.Get_rank() == 0:
         os.system(f"cat {self.logfile} >> total.log")
     finally:
       os.chdir(curdir)
     
   def run(self):
     curdir = os.getcwd()
```

### Comparing `asi4py-0.0.8/src/asi4py.egg-info/PKG-INFO` & `asi4py-0.0.9/src/asi4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```

