# Comparing `tmp/sbcoyote-1.3.7.tar.gz` & `tmp/sbcoyote-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcoyote-1.3.7.tar", max compression
+gzip compressed data, was "sbcoyote-1.4.0.tar", max compression
```

## Comparing `sbcoyote-1.3.7.tar` & `sbcoyote-1.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.3.7/LICENSE
--rw-r--r--   0        0        0     1812 2023-04-06 23:40:48.980565 sbcoyote-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    10355 2023-02-23 20:29:46.172339 sbcoyote-1.3.7/README.md
--rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.3.7/rkviewer/__init__.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.3.7/rkviewer/canvas/__init__.py
--rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.3.7/rkviewer/canvas/canvas.py
--rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.3.7/rkviewer/canvas/data.py
--rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.3.7/rkviewer/canvas/elements.py
--rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.3.7/rkviewer/canvas/geometry.py
--rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.3.7/rkviewer/canvas/overlays.py
--rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.3.7/rkviewer/canvas/state.py
--rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.3.7/rkviewer/canvas/utils.py
--rw-r--r--   0        0        0    18996 2023-02-16 03:57:51.515820 sbcoyote-1.3.7/rkviewer/config.py
--rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.3.7/rkviewer/controller.py
--rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.3.7/rkviewer/events.py
--rw-r--r--   0        0        0    97893 2023-04-06 00:05:27.465051 sbcoyote-1.3.7/rkviewer/forms.py
--rw-r--r--   0        0        0    94813 2023-03-29 18:22:11.285164 sbcoyote-1.3.7/rkviewer/iodine.py
--rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.3.7/rkviewer/json/dark-settings.json
--rw-r--r--   0        0        0     3329 2023-02-06 19:51:01.343848 sbcoyote-1.3.7/rkviewer/json/default-settings.json
--rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.3.7/rkviewer/json/settings.json
--rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.3.7/rkviewer/main.py
--rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.3.7/rkviewer/mvc.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.3.7/rkviewer/plugin/__init__.py
--rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.3.7/rkviewer/plugin/api.py
--rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.3.7/rkviewer/plugin/canvas.py
--rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.3.7/rkviewer/plugin/classes.py
--rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.3.7/rkviewer/plugin/events.py
--rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.3.7/rkviewer/plugin_manage.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.3.7/rkviewer/resources/__init__.py
--rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.3.7/rkviewer/resources/AlignBottom_XP.png
--rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.3.7/rkviewer/resources/alignHorizCenter_XP.png
--rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.3.7/rkviewer/resources/alignHorizEqually_XP.png
--rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.3.7/rkviewer/resources/alignLeft_XP.png
--rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.3.7/rkviewer/resources/alignOnGrid_XP.png
--rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.3.7/rkviewer/resources/alignRight_XP.png
--rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.3.7/rkviewer/resources/alignTop_XP.png
--rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.3.7/rkviewer/resources/alignVertCenter_XP.png
--rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.3.7/rkviewer/resources/alignVertEqually_XP.png
--rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.3.7/rkviewer/resources/info-2-16.png
--rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.3.7/rkviewer/utils.py
--rw-r--r--   0        0        0    47494 2023-04-06 23:40:44.717960 sbcoyote-1.3.7/rkviewer/view.py
--rw-r--r--   0        0        0     8861 2023-04-05 18:55:40.926273 sbcoyote-1.3.7/rkviewer_plugins/addReaction.py
--rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.3.7/rkviewer_plugins/align_circle.py
--rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.3.7/rkviewer_plugins/arrow_designer.py
--rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.3.7/rkviewer_plugins/exportAntimony.py
--rw-r--r--   0        0        0    67466 2023-03-30 18:47:20.839876 sbcoyote-1.3.7/rkviewer_plugins/exportSBML.py
--rw-r--r--   0        0        0   152356 2023-03-30 18:44:02.927726 sbcoyote-1.3.7/rkviewer_plugins/importSBML.py
--rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.3.7/rkviewer_plugins/modelMetrics.py
--rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.3.7/rkviewer_plugins/networkX.py
--rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.3.7/rkviewer_plugins/randomNetwork.py
--rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.3.7/rkviewer_plugins/structuralAnalysis.py
--rw-r--r--   0        0        0    11910 1970-01-01 00:00:00.000000 sbcoyote-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1835 2023-04-17 19:01:31.262321 sbcoyote-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10373 2023-04-07 19:29:33.141010 sbcoyote-1.4.0/README.md
+-rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.4.0/rkviewer/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.4.0/rkviewer/canvas/__init__.py
+-rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.4.0/rkviewer/canvas/canvas.py
+-rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.4.0/rkviewer/canvas/data.py
+-rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.4.0/rkviewer/canvas/elements.py
+-rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.4.0/rkviewer/canvas/geometry.py
+-rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.4.0/rkviewer/canvas/overlays.py
+-rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.4.0/rkviewer/canvas/state.py
+-rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.4.0/rkviewer/canvas/utils.py
+-rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.4.0/rkviewer/config.py
+-rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.4.0/rkviewer/controller.py
+-rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.4.0/rkviewer/events.py
+-rw-r--r--   0        0        0    98431 2023-04-14 18:57:17.020026 sbcoyote-1.4.0/rkviewer/forms.py
+-rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.4.0/rkviewer/iodine.py
+-rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.4.0/rkviewer/json/.default-settings.json
+-rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.4.0/rkviewer/json/dark-settings.json
+-rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.4.0/rkviewer/json/settings.json
+-rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.4.0/rkviewer/main.py
+-rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.4.0/rkviewer/mvc.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.4.0/rkviewer/plugin/__init__.py
+-rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.4.0/rkviewer/plugin/api.py
+-rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.4.0/rkviewer/plugin/canvas.py
+-rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.4.0/rkviewer/plugin/classes.py
+-rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.4.0/rkviewer/plugin/events.py
+-rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.4.0/rkviewer/plugin_manage.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.4.0/rkviewer/resources/__init__.py
+-rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.4.0/rkviewer/resources/AlignBottom_XP.png
+-rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.4.0/rkviewer/resources/alignHorizCenter_XP.png
+-rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.4.0/rkviewer/resources/alignHorizEqually_XP.png
+-rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.4.0/rkviewer/resources/alignLeft_XP.png
+-rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.4.0/rkviewer/resources/alignOnGrid_XP.png
+-rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignRight_XP.png
+-rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignTop_XP.png
+-rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignVertCenter_XP.png
+-rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.4.0/rkviewer/resources/alignVertEqually_XP.png
+-rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.4.0/rkviewer/resources/info-2-16.png
+-rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.4.0/rkviewer/utils.py
+-rw-r--r--   0        0        0    47660 2023-04-17 19:01:36.166032 sbcoyote-1.4.0/rkviewer/view.py
+-rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.4.0/rkviewer_plugins/addReaction.py
+-rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.4.0/rkviewer_plugins/align_circle.py
+-rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.4.0/rkviewer_plugins/arrow_designer.py
+-rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.4.0/rkviewer_plugins/exportAntimony.py
+-rw-r--r--   0        0        0    67844 2023-04-14 22:49:04.000455 sbcoyote-1.4.0/rkviewer_plugins/exportSBML.py
+-rw-r--r--   0        0        0   154343 2023-04-17 17:29:27.368209 sbcoyote-1.4.0/rkviewer_plugins/importSBML.py
+-rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.4.0/rkviewer_plugins/modelMetrics.py
+-rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.4.0/rkviewer_plugins/networkX.py
+-rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.4.0/rkviewer_plugins/randomNetwork.py
+-rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.4.0/rkviewer_plugins/structuralAnalysis.py
+-rw-r--r--   0        0        0    11928 1970-01-01 00:00:00.000000 sbcoyote-1.4.0/PKG-INFO
```

### Comparing `sbcoyote-1.3.7/LICENSE` & `sbcoyote-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/pyproject.toml` & `sbcoyote-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "SBcoyote"
-version = "1.3.7"
+version = "1.4.0"
 description = "SBcoyote: An Extensible Python Based Reaction Editor and Viewer."
 readme = "README.md"
 authors = ["Jin Xu and Gary Geng et al <jxu2019@uw.edu>"]
 packages = [
-    { include = "rkviewer" },
+    #{ include = "*" }
+    { include = "rkviewer"},
     { include = "rkviewer_plugins"},
 ]
 classifiers=[
     'Development Status :: 4 - Beta',
 
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
```

### Comparing `sbcoyote-1.3.7/README.md` & `sbcoyote-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 ## Visualization Example
 
 Here is a visualization example by SBcoyote for the large-scale Escherichia coli core 
 metabolism network (King et al., 2015; Orth et al., 2010).
 
 <img src="https://raw.githubusercontent.com/sys-bio/SBcoyote/main/examples/ecoli.png" width="500" height="400">
 
-## Installment options for Developers
+## Installation Options for Developers
 
 ### Installing with Poetry
 1. If you do not have poetry installed on your computer, follow the quick steps shown [here](https://python-poetry.org/docs/).
-2. Once you have poetry installed, you will download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”. You want to make sure you know where you have downloaded this. Unzip the folder to your desired directory.
-3. Next, open your terminal and navigate to the directory containing SBcoyote.
+2. Once you have poetry installed, you will download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”, then unzip the folder to your desired directory. Make a note of the directory location as you will need it for the next step.
+3. Open your terminal and navigate to the directory containing SBcoyote.
 4. Once inside the main folder of the application you can install the dependencies. To install the base dependencies simply run `poetry install`. To install the optional ones as well, run `poetry install -E simulation`. Note that this step may take a while. To learn more about which set of dependencies is right for you, refer to the [Dependencies](#Dependencies) section below.
 5. Finally, you will run the application with the command `poetry run SBcoyote`.
 
 After you have completed all of these steps, you will not have to repeat them every time you want to run the application. Once the setup is done you will only need to open the terminal, navigate into the folder that contains your SBcoyote application, and run the command `poetry run SBcoyote`.
 
 ### Installing without Poetry
-Again, we strongly advise following the steps above, as it makes the set-up process much faster and simpler. However, to install SBcoyote without Poetry, here is the process you will follow:
+We strongly advise following the steps above as it makes the set-up process much faster and simpler. However, to install SBcoyote without Poetry, here is the process you will follow:
 
-1. First, download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”. You want to make sure you know where you have downloaded this. Unzip the folder to your desired directory.
-2. Next, open your terminal and navigate to the directory containing SBcoyote.
+1. First, download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”, then unzip the folder to your desired directory. Make a note of the directory location as you will need it for the next step.
+2. Open your terminal and navigate to the directory containing SBcoyote.
 3. To install the base set of dependencies, you will run `pip install -r requirements.txt`. Then if you want to install the optional dependencies as well, run `pip install -r requirements-simulation.txt`. To learn more about which set of dependencies is right for you, refer to the [Dependencies](#Dependencies) section below.
 4. Finally, you will run the application with the command `python -m rkviewer.main`.
 After you have completed all of these steps, you will not have to repeat them every time you want to run the application. Once the setup is done you will only need to open the terminal, navigate into the folder that contains your SBcoyote application, and run the command `python -m rkviewer.main`.
 
 ### Running
 * If you have poetry, simply run `poetry run SBcoyote`.
 * Otherwise, in your virtual environment, run `python -m rkviewer.main`.
@@ -119,15 +119,15 @@
 * To run a specific test suite, run e.g. `python -m unittest test.api.test_node`.
 * Or even more specific: `python -m unittest test.api.test_node.TestNode.test_add_nodes`.
 * To profile the application, run `python -m cProfile -o rkviewer.stat main.py`.
 * To visualize the profile result, run `tuna rkviewer.stat`.
 
 ### Building Local Docs
 * Run `sphinx-apidoc -f -o docs/source/rkviewer rkviewer rkviewer/plugin rkviewer/resources ` to regenerate the full reference doc source
-code, if new files were added to the package rkviewer.
+code if new files were added to the package rkviewer.
 * Run `sphinx-build -b html docs\source docs\build`.
 
 ### Note on Style
 Usually snake_case is used for function names. However, to retain some degree of backwards
 compatibility for wxPython, subclasses of wxPython classes use PascalCase for their methods, e.g. `Canvas::RegisterAllChildren`.
 
 ### TODOs
```

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/canvas.py` & `sbcoyote-1.4.0/rkviewer/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/data.py` & `sbcoyote-1.4.0/rkviewer/canvas/data.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/elements.py` & `sbcoyote-1.4.0/rkviewer/canvas/elements.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/geometry.py` & `sbcoyote-1.4.0/rkviewer/canvas/geometry.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/overlays.py` & `sbcoyote-1.4.0/rkviewer/canvas/overlays.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/state.py` & `sbcoyote-1.4.0/rkviewer/canvas/state.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/canvas/utils.py` & `sbcoyote-1.4.0/rkviewer/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/config.py` & `sbcoyote-1.4.0/rkviewer/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     # vertical gap between toolbars and canvas
     vgap = Pixel(missing=2)
     # horizontal gap between toolbars and canvas
     hgap = Pixel(missing=2)
     canvas_outside_bg = ColorField(missing=Color(160, 160, 160))
     mode_panel_width = Pixel(missing=100)
     toolbar_height = Pixel(missing=75)
-    edit_panel_width = Pixel(missing=260)
+    edit_panel_width = Pixel(missing=400)
     node_fill = ColorField(missing=Color(255, 204, 153, 200))
     node_border = ColorField(missing=Color(255, 108, 9))
     node_width = Dim(missing=50)
     node_height = Dim(missing=30)
     # node_corner_radius = Dim(missing=0.15)
     node_border_width = Dim(missing=2)
     node_font_size = Pixel(missing=10)
```

### Comparing `sbcoyote-1.3.7/rkviewer/controller.py` & `sbcoyote-1.4.0/rkviewer/controller.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/events.py` & `sbcoyote-1.4.0/rkviewer/events.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/forms.py` & `sbcoyote-1.4.0/rkviewer/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,18 +208,18 @@
         self.form = form
         self.labels = dict()
         self.badges = dict()
         self._label_font = wx.Font(wx.FontInfo().Bold())
         info_image = wx.Image(resource_path('info-2-16.png'), wx.BITMAP_TYPE_PNG)
         self._info_bitmap = wx.Bitmap(info_image)
         self._info_length = 16
-        sizer = self.InitAndGetSizer()
+        sizer = self.InitAndGetSizer(self.GetParent().GetParent().GetSize()[0])
         self.SetSizer(sizer)
 
-    def InitAndGetSizer(self) -> wx.GridSizer:
+    def InitAndGetSizer(self, edit_panel_width) -> wx.GridSizer:
         VGAP = 8
         HGAP = 5
         MORE_LEFT_PADDING = 0  # Left padding in addition to vgap
         MORE_TOP_PADDING = 2  # Top padding in addition to hgap
         MORE_RIGHT_PADDING = 0
 
         sizer = wx.GridBagSizer(vgap=VGAP, hgap=HGAP)
@@ -232,17 +232,16 @@
         sizer.Add(self._info_length, 0, wx.GBPosition(0, 3), wx.GBSpan(1, 1))
         # Add spacer of width 5 on the 3rd column. This results in a right padding of 5 + hgap
         sizer.Add(MORE_RIGHT_PADDING, 0, wx.GBPosition(0, 4), wx.GBSpan(1, 1))
 
         # Ensure the input field takes up some percentage of width
         # Note that we might want to adjust this when scrollbars are displayed, but only in case
         # there is not enough width to display everything
-        width = self.GetSize()[0]
-        right_width = (width - VGAP * 3 - MORE_LEFT_PADDING - MORE_RIGHT_PADDING -
-                       self._info_length) * 0.7
+        right_width = (edit_panel_width - VGAP * 3 - MORE_LEFT_PADDING - MORE_RIGHT_PADDING -
+                       self._info_length) * .7
         sizer.Add(int(right_width), 0, wx.GBPosition(0, 2), wx.GBSpan(1, 1))
         sizer.AddGrowableCol(0, 3)
         sizer.AddGrowableCol(1, 7)
         return sizer
 
     def AppendControl(self, label_str: str, ctrl: wx.Control):
         """Append a control, its label, and its info badge to the last row of the sizer.
@@ -446,14 +445,17 @@
         return float_ctrl_fn
 
 class PrimitiveGrid(FieldGrid):
     form: 'NodeForm'
     def __init__(self, parent, form: 'NodeForm'):
         super().__init__(parent, form)
         self.update_callbacks = list()
+        # need another GetParent() in addition to FieldGrid's call
+        sizer = self.InitAndGetSizer(self.GetParent().GetParent().GetParent().GetSize()[0])
+        self.SetSizer(sizer)
 
     def UpdateValues(self, nodes):
         '''Update the values in the primitive fields.
 
         Requires:
             The FieldGrid contains the up-to-date field widgets for the given composite shape.
         '''
@@ -711,15 +713,16 @@
     _label_font: wx.Font  #: font for the form input label.
     _info_bitmap: wx.Bitmap  # :  bitmap for the info badge (icon), for when an input is invalid.
     _info_length: int  #: length of the square reserved for _info_bitmap
     _title: wx.StaticText  #: title of the form
     self_changes: bool  #: flag for if edits were made but the controller hasn't updated the view yet
 
     def __init__(self, parent, canvas: Canvas, controller: IController):
-        super().__init__(parent, style=wx.VSCROLL)
+        #super().__init__(parent, style=wx.VSCROLL)
+        super().__init__(parent, style = wx.ALWAYS_SHOW_SB)
         self.SetForegroundColour(get_theme('toolbar_fg'))
         self.SetBackgroundColour(get_theme('toolbar_bg'))
         self.canvas = canvas
         self.controller = controller
         self.net_index = 0
         self._title = wx.StaticText(self, style=wx.ALIGN_CENTER)  # only displayed when node(s) are selected
         title_font = wx.Font(wx.FontInfo(10))
@@ -1496,15 +1499,15 @@
 
     def CreateControls(self):
         self.id_ctrl = self.main_section.CreateTextCtrl()
         self.id_ctrl.Bind(wx.EVT_TEXT, self._OnIdText)
         self.main_section.AppendControl('identifier', self.id_ctrl)
 
         self.ratelaw_ctrl = self.main_section.CreateTextCtrl()
-        self.ratelaw_ctrl.Bind(wx.EVT_TEXT, self._OnRateLawText)
+        #self.ratelaw_ctrl.Bind(wx.EVT_TEXT, self._OnRateLawText)
         self.main_section.AppendControl('rate law', self.ratelaw_ctrl)
 
         self.fill_ctrl, self.fill_alpha_ctrl = self.main_section.CreateColorControl(
             'fill color', 'fill opacity',
             self._OnFillColorChanged, self._FillAlphaCallback)
 
         self.stroke_width_ctrl = self.main_section.CreateTextCtrl()
@@ -1638,16 +1641,16 @@
         reaction = self.canvas.reaction_idx_map[next(iter(self._selected_idx))]
         centroid_map = self.canvas.GetReactionCentroids(self.net_index)
         centroid = centroid_map[reaction.index]
         if checked:
             self.auto_center_ctrl.Enable()
             self.auto_center_ctrl.SetValue(True)
             self.auto_center_ctrl.SetLabel("On")
-            self.center_pos_ctrl.Disable()
             self.center_pos_ctrl.ChangeValue('')
+            self.center_pos_ctrl.Disable()
             with self.controller.group_action():
                 self.controller.set_reaction_center(self.net_index, reaction.index, None)
                 # Move centroid handle along if centroid changed.
                 if reaction.center_pos is not None:
                     offset = centroid - reaction.center_pos
                     if offset != Vec2():
                         self.controller.set_center_handle(
@@ -1820,41 +1823,46 @@
         if len(self._selected_idx) == 1:
             [reaction] = reactions
             reai = reaction.index
             self.id_ctrl.Enable()
             fill = reaction.fill_color
             fill_alpha = reaction.fill_color.Alpha()
             ratelaw_text = reaction.rate_law
-            self.ratelaw_ctrl.Enable()
+            #self.ratelaw_ctrl.Enable()
+            self.ratelaw_ctrl.Disable()
             
             self.auto_center_ctrl.Enable()
             auto_set = reaction.center_pos is None
             self.auto_center_ctrl.SetValue(auto_set)
             if auto_set:
                 self.auto_center_ctrl.SetLabel("On")
+                self.center_pos_ctrl.ChangeValue(' ')
             else:
                 self.auto_center_ctrl.SetLabel("Off")
             self.center_pos_ctrl.Enable(not auto_set)
             if reaction.center_pos is not None:
                 centroid = reaction.center_pos
                 self.center_pos_ctrl.ChangeValue('{}, {}'.format(
                     no_rzeros(centroid.x, prec), no_rzeros(centroid.y, prec)
                 ))
 
             self._UpdateStoichFields(reai, self._GetSrcStoichs(reai), self._GetDestStoichs(reai))
             self.modifiers_ctrl.Enable()
             self._modifiers = reaction.modifiers
             self._UpdateModifierSelection()
         else:
+
             self.id_ctrl.Disable()
             fill, fill_alpha = GetMultiColor(list(r.fill_color for r in reactions))
             ratelaw_text = 'multiple'
             self.ratelaw_ctrl.Disable()
-
+            self.auto_center_ctrl.SetValue(False)
+            self.auto_center_ctrl.SetLabel("Off")
             self.auto_center_ctrl.Disable()
+            self.center_pos_ctrl.ChangeValue(' ')
             self.center_pos_ctrl.Disable()
 
             self._UpdateStoichFields(0, [], [])
             self.modifiers_ctrl.Disable()
             self._modifiers = set()
             self._UpdateModifierSelection()
```

### Comparing `sbcoyote-1.3.7/rkviewer/iodine.py` & `sbcoyote-1.4.0/rkviewer/iodine.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/json/dark-settings.json` & `sbcoyote-1.4.0/rkviewer/json/dark-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/json/default-settings.json` & `sbcoyote-1.4.0/rkviewer/json/.default-settings.json`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         "drag_border_width": 1,
         "drag_fill": [
             0,
             140,
             255,
             20
         ],
-        "edit_panel_width": 260,
+        "edit_panel_width": 400,
         "handle_color": [
             0,
             140,
             255
         ],
         "hgap": 2,
         "highlighted_handle_color": [
```

### Comparing `sbcoyote-1.3.7/rkviewer/json/settings.json` & `sbcoyote-1.4.0/rkviewer/json/settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/main.py` & `sbcoyote-1.4.0/rkviewer/main.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/mvc.py` & `sbcoyote-1.4.0/rkviewer/mvc.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/plugin/api.py` & `sbcoyote-1.4.0/rkviewer/plugin/api.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/plugin/canvas.py` & `sbcoyote-1.4.0/rkviewer/plugin/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/plugin/classes.py` & `sbcoyote-1.4.0/rkviewer/plugin/classes.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/plugin_manage.py` & `sbcoyote-1.4.0/rkviewer/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/resources/alignRight_XP.png` & `sbcoyote-1.4.0/rkviewer/resources/alignRight_XP.png`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/utils.py` & `sbcoyote-1.4.0/rkviewer/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer/view.py` & `sbcoyote-1.4.0/rkviewer/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,16 +295,17 @@
         self.AppendNormalButton('Reactants', canvas.MarkSelectedAsReactants,
                                 sizer, tooltip='Mark selected nodes as reactants')
         self.AppendNormalButton('Products', canvas.MarkSelectedAsProducts,
                                 sizer, tooltip='Mark selected nodes as products')
         self.AppendNormalButton('Create Rxn', canvas.CreateReactionFromMarked,
                                 sizer, tooltip='Create reaction from marked reactants and products')
 
-        # self.AppendSeparator(sizer)
-        # self.AppendToggleButtonUniUni('UniUni', sizer, tooltip='Add a UniUni reaction')
+        self.AppendSeparator(sizer)
+        #self.AppendNormalButtonUniUni('UniUni', sizer, tooltip='Add UniUni reactions')
+
 
         self.SetSizer(sizer)
 
     def AppendModeButton(self, label: str, mode: InputMode, sizer: wx.Sizer):
         if get_theme ('btn_border'):
             btn = wx.ToggleButton(self, label=label)
         else:
@@ -338,26 +339,30 @@
         btn.SetBackgroundColour(get_theme ('btn_bg'))
         btn.SetForegroundColour(get_theme ('btn_fg'))
         if tooltip is not None:
             btn.SetToolTip(tooltip)
         btn.Bind(wx.EVT_BUTTON, lambda _: callback())
         sizer.Add(btn, wx.SizerFlags().Align(wx.ALIGN_CENTER).Border(wx.TOP, 10))
 
-    def AppendToggleButtonUniUni(self, label: str, sizer: wx.Sizer, tooltip: str = None):
-
+    def AppendNormalButtonUniUni(self, label: str, sizer: wx.Sizer, tooltip: str = None):
         if get_theme ('btn_border'):
-           btn = wx.ToggleButton(self, label=label)
+           btn = wx.Button(self, label=label)
         else:
-           btn = wx.ToggleButton(self, label=label, style=wx.BORDER_NONE)
+           btn = wx.Button(self, label=label, style=wx.BORDER_NONE)
+
+        def addUniUni(evt):
+            addReaction.AddReaction.__init__(self)
+            addReaction.AddReaction.on_selection_did_change(self, evt)
+            addReaction.AddReaction.UniUni(self, evt)
 
         btn.SetBackgroundColour(get_theme ('btn_bg'))
         btn.SetForegroundColour(get_theme ('btn_fg'))
         if tooltip is not None:
             btn.SetToolTip(tooltip)
-        btn.Bind(wx.EVT_TOGGLEBUTTON, addReaction.AddReaction._UniUni(self))
+        btn.Bind(wx.EVT_TOGGLEBUTTON, addUniUni)
         sizer.Add(btn, wx.SizerFlags().Align(wx.ALIGN_CENTER).Border(wx.TOP, 10))
 
     def AppendSeparator(self, sizer: wx.Sizer):
         sizer.Add((0, 10))
     
 
 
@@ -696,15 +701,15 @@
         self.Bind(wx.EVT_MENU, callback, item)
         self.menu_events.append((callback, item))
         return item
 
     def onAboutDlg(self, event):
         info = wx.adv.AboutDialogInfo()
         info.SetName("SBcoyote")
-        info.SetVersion("1.3.7")
+        info.SetVersion("1.4.0")
         info.SetCopyright("(c) 2023 UW Sauro Lab")
         info.SetDescription("An Extensible Python-Based Reaction Editor and Viewer.")
         info.SetWebSite("https://github.com/sys-bio/SBcoyote",
                         "Home Page")  # TODO update home page?
         info.SetDevelopers(["Jin Xu", "Gary Geng", "Nhan D. Nguyen", "Carmen Perena-Corte","Claire Samuels", "Herbert M. Sauro"])# TODO update authors
         info.SetLicense("MIT")
```

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/addReaction.py` & `sbcoyote-1.4.0/rkviewer_plugins/addReaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,30 +193,14 @@
          self.bibiState = False
          self.BiUni_btn.SetValue (False)
          self.UniBi_btn.SetValue (False)
          self.BiBi_btn.SetValue (False)            
       else:
          self.uniuniState = False
 
-   def _UniUni(self, state = True):
-      """
-      Handler for the "UniUni" button in view.py.
-      """
-
-      if state == True:  
-         self.src = []
-         self.dest = []
-         # This code is to make the buttons work as a radionbutton
-         self.uniuniState = True
-         self.biuniState = False
-         self.unibiState = False
-         self.bibiState = False
-      else:
-         self.uniuniState = False
-
    def BiUni(self, evt):
       """
       Handler for the "BiUni" button. add a BiUni reaction.
       """
       state = evt.GetEventObject().GetValue()
       if state == True:  
          self.src = []
```

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/align_circle.py` & `sbcoyote-1.4.0/rkviewer_plugins/align_circle.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/arrow_designer.py` & `sbcoyote-1.4.0/rkviewer_plugins/arrow_designer.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/exportAntimony.py` & `sbcoyote-1.4.0/rkviewer_plugins/exportAntimony.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/exportSBML.py` & `sbcoyote-1.4.0/rkviewer_plugins/exportSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 Export the network on canvas to an SBML string as save it as a file.
-Version 1.0.6: Author: Jin Xu (2023)
+Version 1.0.7: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from inspect import Parameter
 import wx
 from wx.core import Width
 from rkviewer.plugin.classes import PluginMetadata, WindowedPlugin, PluginCategory
 from rkviewer.plugin import api
 from rkviewer.plugin.api import Node, Vec2, Reaction, Color, get_node_by_index
 import os
 from libsbml import * # does not have to import in the main.py too
 import re # to process kinetic_law string
+from rkviewer.config import get_theme
 
 class ExportSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ExportSBML',
         author='Jin Xu',
-        version='1.0.6',
+        version='1.0.7',
         short_desc='Export SBML.',
         long_desc='Export the SBML String from the network on canvas and save it to a file.',
         category=PluginCategory.MODELS
     )
 
 
     def create_window(self, dialog):
@@ -252,15 +253,15 @@
                         species.setName(spec_name)
                         species.setSBOTerm(spec_SBO)
                         comp_idx = allNodes[i].comp_idx
                         if comp_idx != -1:
                             comp_id = allcompartments[comp_idx].id 
                             species.setCompartment(comp_id)  
                         else:
-                            species.setCompartment("_compartment_default_") 
+                           species.setCompartment("_compartment_default_") #why "_compartment_default_"
                         species.setInitialConcentration(allNodes[i].concentration)	
                         species.setHasOnlySubstanceUnits(False)
                         species.setBoundaryCondition(False)
                         species.setConstant(False)             
                         if allNodes[i].floating_node == False:
                             species.setBoundaryCondition(True)
                             species.setConstant(True)   
@@ -280,16 +281,16 @@
                         if ' ' in spec_id:
                             spec_id = spec_id.replace(' ', '_')
                         if spec_id not in spec_id_list:
                             spec_id_list.append(spec_id)
                         species = model.createSpecies()
                         species.setId(spec_id)
                         species.setName(spec_name)
-                        species.setSBOTerm(spec_SBO)
-                        species.setCompartment(comp_id)
+                        species.setSBOTerm(spec_SBO) 
+                        species.setCompartment(comp_id) #why "_compartment_default_"
                         species.setInitialConcentration(allNodes[i].concentration)	
                         species.setHasOnlySubstanceUnits(False)
                         species.setBoundaryCondition(False)
                         species.setConstant(False)             
                         if allNodes[i].floating_node == False:
                             species.setBoundaryCondition(True)
                             species.setConstant(True)
@@ -318,31 +319,31 @@
                     temp_spec_id = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).id
                     if ' ' in temp_spec_id:
                         temp_spec_id = temp_spec_id.replace(' ', '_')
                     mod.append(temp_spec_id)
 
                 kinetic_law_from_user = allReactions[i].rate_law
                 
-                # if kinetic_law_from_user == '':
-                kinetic_law = ''
-                kinetic_law = kinetic_law + 'E' + str (i) + '*(k' + str (i) 
-                parameter_id_value_dict_self_pre['E' + str(i)] = 0.1
-                parameter_id_value_dict_self_pre['k' + str(i)] = 0.1
-
-                for j in range(rct_num):
-                    kinetic_law = kinetic_law + '*' + rct[j]
-                    
-                if isReversible:
-                    kinetic_law = kinetic_law + ' - k' + str (i) + 'r'
-                    parameter_id_value_dict_self_pre['k' + str (i) + 'r'] = 0.1
-                    for j in range(prd_num):
-                        kinetic_law = kinetic_law + '*' + prd[j]
-                kinetic_law = kinetic_law + ')'
-                # else:
-                #     kinetic_law = kinetic_law_from_user
+                if kinetic_law_from_user == '':
+                    kinetic_law = ''
+                    kinetic_law = kinetic_law + 'E' + str (i) + '*(k' + str (i) 
+                    parameter_id_value_dict_self_pre['E' + str(i)] = 0.1
+                    parameter_id_value_dict_self_pre['k' + str(i)] = 0.1
+
+                    for j in range(rct_num):
+                        kinetic_law = kinetic_law + '*' + rct[j]
+                        
+                    if isReversible:
+                        kinetic_law = kinetic_law + ' - k' + str (i) + 'r'
+                        parameter_id_value_dict_self_pre['k' + str (i) + 'r'] = 0.1
+                        for j in range(prd_num):
+                            kinetic_law = kinetic_law + '*' + prd[j]
+                    kinetic_law = kinetic_law + ')'
+                else:
+                    kinetic_law = kinetic_law_from_user
 
                 reaction = model.createReaction()
                 reaction.setId(allReactions[i].id)
                 reaction.setReversible(False)
                 reaction.setFast(False)
                 if isReversible:
                     reaction.setReversible(True)
@@ -413,17 +414,21 @@
                 wx.MessageBox("There is no layout information.", "Message", wx.OK | wx.ICON_INFORMATION)
 
 
             #
             # Creates a Layout object via LayoutModelPlugin object.
             #
             layout = mplugin.createLayout()
-            layout.setId("COYOTO_layout")
-            layout_width = 10000 - 20
-            layout_height = 6200 - 20
+            layout.setId("SBcoyote_layout")
+            def_canvas_width = get_theme('real_canvas_width')
+            def_canvas_height = get_theme('real_canvas_height')
+            #layout_width = 10000 - 20
+            #layout_height = 6200 - 20
+            layout_width = def_canvas_width - 20.
+            layout_height = def_canvas_height - 20.
             layout.setDimensions(Dimensions(layoutns, layout_width, layout_height))
             # random network (40+800x, 40+800y)
 
             #create the CompartmentGlyph and SpeciesGlyphs
             if numCompartments != 0:
                 for i in range(numCompartments):   
                     comp_id=allcompartments[i].id
```

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/importSBML.py` & `sbcoyote-1.4.0/rkviewer_plugins/importSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Import an SBML string from a file and visualize it to a network on canvas.
-Version 1.1.6: Author: Jin Xu (2023)
+Version 1.1.7: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from ast import Num
 from inspect import Parameter
@@ -18,20 +18,21 @@
 from rkviewer.plugin.api import Node, Vec2, Reaction, Color, get_nodes
 import os
 import simplesbml # does not have to import in the main.py too
 from libsbml import *
 import math
 import random as _random
 import pandas as pd
+from rkviewer.config import get_theme
 
 class IMPORTSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ImportSBML',
         author='Jin Xu',
-        version='1.1.6',
+        version='1.1.7',
         short_desc='Import SBML.',
         long_desc='Import an SBML String from a file and visualize it as a network on canvas.',
         category=PluginCategory.MODELS
     )
 
     def create_window(self, dialog):
         """
@@ -193,18 +194,20 @@
                     raise Exception("There is no layout.") 
                 # Get the first Layout object via LayoutModelPlugin object.
                 #
                 # if mplugin is None:
                 #     if showDialogues:
                 #         wx.MessageBox("There is no layout information, so positions are randomly assigned.", "Message", wx.OK | wx.ICON_INFORMATION)
                 # else:
-                def_canvas_width = 10000.
-                def_canvas_height = 6200.
-                def_comp_width = def_canvas_width-20.
-                def_comp_height = def_canvas_height-20.
+                #def_canvas_width = 10000.
+                #def_canvas_height = 6200.
+                def_canvas_width = get_theme('real_canvas_width')
+                def_canvas_height = get_theme('real_canvas_height')
+                def_comp_width = def_canvas_width - 20.
+                def_comp_height = def_canvas_height - 20.
                 if mplugin is not None:
                     layout = mplugin.getLayout(0)
                     # if layout is None:
                     #     if showDialogues:
                     #         wx.MessageBox("There is no layout information, so positions are randomly assigned.", "Message", wx.OK | wx.ICON_INFORMATION)
                     # else:
                     try:
@@ -287,20 +290,39 @@
                                 width = rxn_boundingbox.getWidth()
                                 height = rxn_boundingbox.getHeight()
                                 pos_x = rxn_boundingbox.getX()
                                 pos_y = rxn_boundingbox.getY()
                                 if center_pt == []:
                                     if pos_x == 0 and pos_y == 0 and width == 0 and height == 0: #LinearChain.xml
                                         center_pt = []
+                                        #if the boudingbox can not give the info for the center point,
+                                        #look for the common point of the start and end points
+                                        start_end_pt = []
+                                        for j in range(numSpecRefGlyphs):     
+                                            specRefGlyph = reactionGlyph.getSpeciesReferenceGlyph(j)   
+                                            curve = specRefGlyph.getCurve()                                  
+                                            for segment in curve.getListOfCurveSegments():
+                                                line_start_x = segment.getStart().getXOffset()
+                                                line_start_y = segment.getStart().getYOffset()
+                                                line_end_x = segment.getEnd().getXOffset()
+                                                line_end_y = segment.getEnd().getYOffset()
+                                                line_start_pt =  [line_start_x, line_start_y]
+                                                line_end_pt = [line_end_x, line_end_y]
+                                                if line_start_pt in start_end_pt:
+                                                    center_pt = line_start_pt
+                                                if line_end_pt in start_end_pt:
+                                                    center_pt = line_end_pt
+                                                else:
+                                                    start_end_pt.append(line_start_pt)
+                                                    start_end_pt.append(line_end_pt)
                                     else:
                                         center_pt = [pos_x+.5*width, pos_y+.5*height]
                                 center_sz = [width, height]
                             except:
                                 pass
-
                             
                             reaction_center_list.append(center_pt)
                             #reaction_size_list.append(center_sz)
                             
                             reaction_id = reactionGlyph.getReactionId()
                            
                             reaction_id_list.append(reaction_id)
@@ -547,20 +569,20 @@
                                             text_content = spec_name
                                         else:
                                             text_content = spec_id
                                     spec_text_content_list.append(text_content)
                                     spec_text_alignment_list.append(alignment_name)
                                     spec_text_position_list.append(position_name)
                                     spec_concentration_list.append(concentration)
-                                
-                                if center_handle == []:
-                                    center_handle.append(center_handle_candidate)
 
                               
                                 if role == "substrate" or role == "sidesubstrate": #it is a rct
+                                    #the center handle is supposed to be from the reactant
+                                    if center_handle == []:
+                                        center_handle.append(center_handle_candidate)
                                     #rct_specGlyph_temp_list.append(specGlyph_id)
                                     rct_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
                                 elif role == "product" or role == "sideproduct": #it is a prd
                                     #prd_specGlyph_temp_list.append(specGlyph_id)
                                     prd_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
                                 elif role == "modifier" or role == 'activator': #it is a modifier
                                     mod_specGlyph_temp_list.append(specGlyph_id)
@@ -1372,15 +1394,14 @@
                                     nodeIdx_list.append(nodeIdx_temp)
                                     nodeIdx_specGlyph_alias_list.append([nodeIdx_temp,tempGlyph_id])
                                 
                                 comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
                                 for xx in range(numComps):
                                     if comp_id == Comps_ids[xx]:
                                         api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx) 
-                                
                                 for k in range(numCompGlyphs):
                                     if len(comp_id_list) !=0 and comp_id == comp_id_list[k]:
                                         comp_node_list[k].append(nodeIdx_temp)
                         for j in range(numBoundaryNodes):
                             if temp_id == BoundaryNodes_ids[j]:
                                 if temp_id not in id_list:
                                     flag_local = 0
@@ -1455,30 +1476,30 @@
                                     #api.set_node_shape_property(net_index, nodeIdx_temp, -1, "font_size", int(text_font_size))
                                     id_list.append(temp_id)
                                     nodeIdx_list.append(nodeIdx_temp)
                                     nodeIdx_specGlyph_alias_list.append([nodeIdx_temp,tempGlyph_id])
                                 
                                 comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
                                 for xx in range(numComps):
-                                    if comp_id == Comps_ids[xx]:
-                                        api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx)
-                                        
+                                    if comp_id == Comps_ids[xx]:            
+                                        api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx)             
+                                     
                                 for k in range(numCompGlyphs):
                                     if len(comp_id) != 0 and comp_id == comp_id_list[k]:
                                         comp_node_list[k].append(nodeIdx_temp)
 
                     if len(comp_id_list) != 0 or numComps != 0:
                         for i in range(numComps):
                             temp_id = Comps_ids[i]
                             if temp_id == '_compartment_default_': 
                                 #numNodes is different from len(nodeIdx_list) because of alias node
                                 node_list_default = [item for item in range(len(nodeIdx_list))]
                                 for j in range(len(node_list_default)):
                                     try:
-                                        api.set_compartment_of_node(net_index=net_index, node_index=node_list_default[j], comp_index=i) 
+                                        api.set_compartment_of_node(net_index=net_index, node_index=node_list_default[j], comp_index=i)
                                     except:
                                         pass # Orphan nodes are removed
                             for j in range(numCompGlyphs):
                                 if comp_id_list[j] == temp_id:
                                     node_list_temp = comp_node_list[j]
                                 else:
                                     node_list_temp = []
```

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/modelMetrics.py` & `sbcoyote-1.4.0/rkviewer_plugins/modelMetrics.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/networkX.py` & `sbcoyote-1.4.0/rkviewer_plugins/networkX.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/randomNetwork.py` & `sbcoyote-1.4.0/rkviewer_plugins/randomNetwork.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/rkviewer_plugins/structuralAnalysis.py` & `sbcoyote-1.4.0/rkviewer_plugins/structuralAnalysis.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.3.7/PKG-INFO` & `sbcoyote-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcoyote
-Version: 1.3.7
+Version: 1.4.0
 Summary: SBcoyote: An Extensible Python Based Reaction Editor and Viewer.
 Author: Jin Xu and Gary Geng et al
 Author-email: jxu2019@uw.edu
 Requires-Python: >=3.7.1,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -67,30 +67,30 @@
 ## Visualization Example
 
 Here is a visualization example by SBcoyote for the large-scale Escherichia coli core 
 metabolism network (King et al., 2015; Orth et al., 2010).
 
 <img src="https://raw.githubusercontent.com/sys-bio/SBcoyote/main/examples/ecoli.png" width="500" height="400">
 
-## Installment options for Developers
+## Installation Options for Developers
 
 ### Installing with Poetry
 1. If you do not have poetry installed on your computer, follow the quick steps shown [here](https://python-poetry.org/docs/).
-2. Once you have poetry installed, you will download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”. You want to make sure you know where you have downloaded this. Unzip the folder to your desired directory.
-3. Next, open your terminal and navigate to the directory containing SBcoyote.
+2. Once you have poetry installed, you will download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”, then unzip the folder to your desired directory. Make a note of the directory location as you will need it for the next step.
+3. Open your terminal and navigate to the directory containing SBcoyote.
 4. Once inside the main folder of the application you can install the dependencies. To install the base dependencies simply run `poetry install`. To install the optional ones as well, run `poetry install -E simulation`. Note that this step may take a while. To learn more about which set of dependencies is right for you, refer to the [Dependencies](#Dependencies) section below.
 5. Finally, you will run the application with the command `poetry run SBcoyote`.
 
 After you have completed all of these steps, you will not have to repeat them every time you want to run the application. Once the setup is done you will only need to open the terminal, navigate into the folder that contains your SBcoyote application, and run the command `poetry run SBcoyote`.
 
 ### Installing without Poetry
-Again, we strongly advise following the steps above, as it makes the set-up process much faster and simpler. However, to install SBcoyote without Poetry, here is the process you will follow:
+We strongly advise following the steps above as it makes the set-up process much faster and simpler. However, to install SBcoyote without Poetry, here is the process you will follow:
 
-1. First, download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”. You want to make sure you know where you have downloaded this. Unzip the folder to your desired directory.
-2. Next, open your terminal and navigate to the directory containing SBcoyote.
+1. First, download SBcoyote. Click the green button at the top of this page that says “Code” and choose “Download ZIP”, then unzip the folder to your desired directory. Make a note of the directory location as you will need it for the next step.
+2. Open your terminal and navigate to the directory containing SBcoyote.
 3. To install the base set of dependencies, you will run `pip install -r requirements.txt`. Then if you want to install the optional dependencies as well, run `pip install -r requirements-simulation.txt`. To learn more about which set of dependencies is right for you, refer to the [Dependencies](#Dependencies) section below.
 4. Finally, you will run the application with the command `python -m rkviewer.main`.
 After you have completed all of these steps, you will not have to repeat them every time you want to run the application. Once the setup is done you will only need to open the terminal, navigate into the folder that contains your SBcoyote application, and run the command `python -m rkviewer.main`.
 
 ### Running
 * If you have poetry, simply run `poetry run SBcoyote`.
 * Otherwise, in your virtual environment, run `python -m rkviewer.main`.
@@ -159,15 +159,15 @@
 * To run a specific test suite, run e.g. `python -m unittest test.api.test_node`.
 * Or even more specific: `python -m unittest test.api.test_node.TestNode.test_add_nodes`.
 * To profile the application, run `python -m cProfile -o rkviewer.stat main.py`.
 * To visualize the profile result, run `tuna rkviewer.stat`.
 
 ### Building Local Docs
 * Run `sphinx-apidoc -f -o docs/source/rkviewer rkviewer rkviewer/plugin rkviewer/resources ` to regenerate the full reference doc source
-code, if new files were added to the package rkviewer.
+code if new files were added to the package rkviewer.
 * Run `sphinx-build -b html docs\source docs\build`.
 
 ### Note on Style
 Usually snake_case is used for function names. However, to retain some degree of backwards
 compatibility for wxPython, subclasses of wxPython classes use PascalCase for their methods, e.g. `Canvas::RegisterAllChildren`.
 
 ### TODOs
```

