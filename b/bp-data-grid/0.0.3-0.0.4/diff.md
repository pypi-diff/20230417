# Comparing `tmp/bp_data_grid-0.0.3.tar.gz` & `tmp/bp_data_grid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-0.0.3.tar", last modified: Mon Apr 17 11:30:35 2023, max compression
+gzip compressed data, was "bp_data_grid-0.0.4.tar", last modified: Mon Apr 17 12:54:09 2023, max compression
```

## Comparing `bp_data_grid-0.0.3.tar` & `bp_data_grid-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.064272 bp_data_grid-0.0.3/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-0.0.3/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-0.0.3/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-17 11:30:35.063705 bp_data_grid-0.0.3/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-10 05:35:41.000000 bp_data_grid-0.0.3/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.048283 bp_data_grid-0.0.3/bp_data_grid.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-17 11:30:34.000000 bp_data_grid-0.0.3/bp_data_grid.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-04-17 11:30:35.000000 bp_data_grid-0.0.3/bp_data_grid.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-17 11:30:34.000000 bp_data_grid-0.0.3/bp_data_grid.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-17 11:30:34.000000 bp_data_grid-0.0.3/bp_data_grid.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-04-17 11:30:34.000000 bp_data_grid-0.0.3/bp_data_grid.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.049617 bp_data_grid-0.0.3/data_grid/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2112 2023-04-17 08:10:27.000000 bp_data_grid-0.0.3/data_grid/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.044236 bp_data_grid-0.0.3/data_grid/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.051248 bp_data_grid-0.0.3/data_grid/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 11:30:35.062209 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-04-17 10:43:24.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-17 10:43:24.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1524825 2023-04-17 10:43:24.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/index-dffa65a7.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-04-17 10:43:24.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/index.es-650b637d-a0b9f247.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-04-17 10:43:24.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-17 10:46:12.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-17 10:43:23.000000 bp_data_grid-0.0.3/data_grid/frontend/dist/vite.svg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-0.0.3/data_grid/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-17 11:30:35.064548 bp_data_grid-0.0.3/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      623 2023-04-17 11:30:21.000000 bp_data_grid-0.0.3/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.646991 bp_data_grid-0.0.4/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-0.0.4/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-0.0.4/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-17 12:54:09.646653 bp_data_grid-0.0.4/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-10 05:35:41.000000 bp_data_grid-0.0.4/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.638291 bp_data_grid-0.0.4/bp_data_grid.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-17 12:54:09.000000 bp_data_grid-0.0.4/bp_data_grid.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-04-17 12:54:09.000000 bp_data_grid-0.0.4/bp_data_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-17 12:54:09.000000 bp_data_grid-0.0.4/bp_data_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-17 12:54:09.000000 bp_data_grid-0.0.4/bp_data_grid.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-04-17 12:54:09.000000 bp_data_grid-0.0.4/bp_data_grid.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.639207 bp_data_grid-0.0.4/data_grid/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-17 12:52:56.000000 bp_data_grid-0.0.4/data_grid/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.632103 bp_data_grid-0.0.4/data_grid/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.640244 bp_data_grid-0.0.4/data_grid/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 12:54:09.645907 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-04-17 10:43:24.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-17 10:43:24.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1524825 2023-04-17 10:43:24.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/index-dffa65a7.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-04-17 10:43:24.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/index.es-650b637d-a0b9f247.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-04-17 10:43:24.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-17 10:46:12.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-17 10:43:23.000000 bp_data_grid-0.0.4/data_grid/frontend/dist/vite.svg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-0.0.4/data_grid/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-17 12:54:09.647114 bp_data_grid-0.0.4/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      623 2023-04-17 12:53:43.000000 bp_data_grid-0.0.4/setup.py
```

### Comparing `bp_data_grid-0.0.3/LICENSE` & `bp_data_grid-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/bp_data_grid.egg-info/SOURCES.txt` & `bp_data_grid-0.0.4/bp_data_grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/__init__.py` & `bp_data_grid-0.0.4/data_grid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,48 +30,48 @@
     )
 else:
     __data_grid_component_function = components.declare_component(
         "data_grid", url="http://localhost:4000"
     )
 
 
-def __query_builder(
+def __data_grid(
     rows=[],
     columns=[],
     title="",
     on_click=None,
     key="b-data-grid",
     args: tuple = (),
 ):
     register_callback(key, on_click, *args)
     render_count = get_component_rerender_count(key)
-    query_builder_value = __data_grid_component_function(
+    data_grid_value = __data_grid_component_function(
         key=key,
         rows=rows,
         columns=columns,
         title=title,
         render_count=render_count,
     )
     set_component_rerender_count(key)
-    return query_builder_value
+    return data_grid_value
 
 
 def handle_datagrid_change(
     widget_key,
 ):
     response = st.session_state.get(widget_key)
 
 def data_grid(
     key: str = "data-grid",
     rows: List = [],
     columns: List = [],
     title: str = ""
     
 ):
-    return __query_builder(
+    return __data_grid(
         rows=rows,
         columns=columns,
         title=title,
         key=key,
         on_click=handle_datagrid_change,
         args=(
             key,
```

### Comparing `bp_data_grid-0.0.3/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js` & `bp_data_grid-0.0.4/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/frontend/dist/assets/index-dffa65a7.js` & `bp_data_grid-0.0.4/data_grid/frontend/dist/assets/index-dffa65a7.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/frontend/dist/assets/index.es-650b637d-a0b9f247.js` & `bp_data_grid-0.0.4/data_grid/frontend/dist/assets/index.es-650b637d-a0b9f247.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js` & `bp_data_grid-0.0.4/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/frontend/dist/vite.svg` & `bp_data_grid-0.0.4/data_grid/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/data_grid/register.py` & `bp_data_grid-0.0.4/data_grid/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.3/setup.py` & `bp_data_grid-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_grid",
-    version="0.0.3",
+    version="0.0.4",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Show data in data grid",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

