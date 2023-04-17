# Comparing `tmp/dcmetro-0.1.3.tar.gz` & `tmp/dcmetro-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcmetro-0.1.3.tar", last modified: Fri Apr  7 00:47:13 2023, max compression
+gzip compressed data, was "dcmetro-0.1.4.tar", last modified: Mon Apr 17 02:05:04 2023, max compression
```

## Comparing `dcmetro-0.1.3.tar` & `dcmetro-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-07 00:47:13.442307 dcmetro-0.1.3/
--rw-r--r--   0 harunferaidon   (501) staff       (20)     1061 2023-04-06 04:00:36.000000 dcmetro-0.1.3/LICENSE.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)     2546 2023-04-07 00:47:13.442483 dcmetro-0.1.3/PKG-INFO
--rw-r--r--   0 harunferaidon   (501) staff       (20)     2310 2023-04-07 00:46:51.000000 dcmetro-0.1.3/README.md
-drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-07 00:47:13.422749 dcmetro-0.1.3/dcmetro.egg-info/
--rw-r--r--   0 harunferaidon   (501) staff       (20)     2546 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/PKG-INFO
--rw-r--r--   0 harunferaidon   (501) staff       (20)      438 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/SOURCES.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)        1 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/dependency_links.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)       60 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/entry_points.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)       27 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/requires.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)        4 2023-04-07 00:47:13.000000 dcmetro-0.1.3/dcmetro.egg-info/top_level.txt
--rw-r--r--   0 harunferaidon   (501) staff       (20)       79 2023-04-07 00:47:13.443096 dcmetro-0.1.3/setup.cfg
--rw-r--r--   0 harunferaidon   (501) staff       (20)      707 2023-04-07 00:47:06.000000 dcmetro-0.1.3/setup.py
-drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-07 00:47:13.423316 dcmetro-0.1.3/src/
--rw-r--r--   0 harunferaidon   (501) staff       (20)        0 2023-04-04 00:34:40.000000 dcmetro-0.1.3/src/__init__.py
-drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-07 00:47:13.441477 dcmetro-0.1.3/src/main/
--rw-r--r--   0 harunferaidon   (501) staff       (20)        0 2023-03-28 20:16:32.000000 dcmetro-0.1.3/src/main/__init__.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)     2260 2023-04-07 00:36:46.000000 dcmetro-0.1.3/src/main/app.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)     1930 2023-04-06 04:00:36.000000 dcmetro-0.1.3/src/main/build_graph.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)     6689 2023-04-07 00:33:34.000000 dcmetro-0.1.3/src/main/commands.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)    11170 2023-04-04 05:08:25.000000 dcmetro-0.1.3/src/main/constants.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)     1843 2023-04-04 00:34:40.000000 dcmetro-0.1.3/src/main/dijkstra.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)      574 2023-04-04 05:08:25.000000 dcmetro-0.1.3/src/main/generate_station_codes.py
--rw-r--r--   0 harunferaidon   (501) staff       (20)     1098 2023-04-04 05:08:25.000000 dcmetro-0.1.3/src/main/get_station_distances.py
+drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-17 02:05:04.864412 dcmetro-0.1.4/
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     1061 2023-04-06 04:00:36.000000 dcmetro-0.1.4/LICENSE.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     2844 2023-04-17 02:05:04.864608 dcmetro-0.1.4/PKG-INFO
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     2586 2023-04-17 02:04:54.000000 dcmetro-0.1.4/README.md
+drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-17 02:05:04.856177 dcmetro-0.1.4/dcmetro.egg-info/
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     2844 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/PKG-INFO
+-rw-r--r--   0 harunferaidon   (501) staff       (20)      438 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/SOURCES.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)        1 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/dependency_links.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)       60 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/entry_points.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)       27 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/requires.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)        4 2023-04-17 02:05:04.000000 dcmetro-0.1.4/dcmetro.egg-info/top_level.txt
+-rw-r--r--   0 harunferaidon   (501) staff       (20)       79 2023-04-17 02:05:04.865461 dcmetro-0.1.4/setup.cfg
+-rw-r--r--   0 harunferaidon   (501) staff       (20)      735 2023-04-17 02:02:43.000000 dcmetro-0.1.4/setup.py
+drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-17 02:05:04.856752 dcmetro-0.1.4/src/
+-rw-r--r--   0 harunferaidon   (501) staff       (20)        0 2023-04-04 00:34:40.000000 dcmetro-0.1.4/src/__init__.py
+drwxr-xr-x   0 harunferaidon   (501) staff       (20)        0 2023-04-17 02:05:04.863478 dcmetro-0.1.4/src/main/
+-rw-r--r--   0 harunferaidon   (501) staff       (20)        0 2023-03-28 20:16:32.000000 dcmetro-0.1.4/src/main/__init__.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     2260 2023-04-07 00:36:46.000000 dcmetro-0.1.4/src/main/app.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     1930 2023-04-06 04:00:36.000000 dcmetro-0.1.4/src/main/build_graph.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     6689 2023-04-07 00:33:34.000000 dcmetro-0.1.4/src/main/commands.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)    11170 2023-04-04 05:08:25.000000 dcmetro-0.1.4/src/main/constants.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     1843 2023-04-04 00:34:40.000000 dcmetro-0.1.4/src/main/dijkstra.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)      574 2023-04-04 05:08:25.000000 dcmetro-0.1.4/src/main/generate_station_codes.py
+-rw-r--r--   0 harunferaidon   (501) staff       (20)     1098 2023-04-04 05:08:25.000000 dcmetro-0.1.4/src/main/get_station_distances.py
```

### Comparing `dcmetro-0.1.3/LICENSE.txt` & `dcmetro-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/PKG-INFO` & `dcmetro-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: dcmetro
-Version: 0.1.3
+Version: 0.1.4
 Summary: Console app for sending commands to get live information on the DC Metro
 Author: Harun Feraidon
 License: MIT
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DC Metro Command Line Tool
 ![Imgur](https://i.imgur.com/rE4AKgU.gif)
 
 ## What is it
-With this application, you can submit concise commands via your terminal to request and then receive information.
+[![PyPI version](https://badge.fury.io/py/dcmetro.svg)](https://badge.fury.io/py/dcmetro)
+
+A command line app for sending commands to get live information on the DC Metro. You can find the shortest path between two stations, an estimation of the rail time between two stations, and the current arrival times for your metro station.
+[PyPi page here](https://pypi.org/project/dcmetro/0.1.3/)
 
 ## Setup
 1. Setup a python virtual environment. `python3 -m venv venv`
 2. Activate your python virtual environment. `source venv/bin/activate`
 3. Install with `pip install dcmetro`.
 4. (OPTIONAL, BUT RECOMMENDED) Skipping this step means you will be using a community API key. Creating your own API token will be more reliable. Setup a WMATA API token [here](https://developer.wmata.com). Run `echo 'API_KEY = "<YOUR TOKEN HERE>"' > .env`
 5. Run `dcmetro` to start.
```

### Comparing `dcmetro-0.1.3/README.md` & `dcmetro-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # DC Metro Command Line Tool
 ![Imgur](https://i.imgur.com/rE4AKgU.gif)
 
 ## What is it
-With this application, you can submit concise commands via your terminal to request and then receive information.
+[![PyPI version](https://badge.fury.io/py/dcmetro.svg)](https://badge.fury.io/py/dcmetro)
+
+A command line app for sending commands to get live information on the DC Metro. You can find the shortest path between two stations, an estimation of the rail time between two stations, and the current arrival times for your metro station.
+[PyPi page here](https://pypi.org/project/dcmetro/0.1.3/)
 
 ## Setup
 1. Setup a python virtual environment. `python3 -m venv venv`
 2. Activate your python virtual environment. `source venv/bin/activate`
 3. Install with `pip install dcmetro`.
 4. (OPTIONAL, BUT RECOMMENDED) Skipping this step means you will be using a community API key. Creating your own API token will be more reliable. Setup a WMATA API token [here](https://developer.wmata.com). Run `echo 'API_KEY = "<YOUR TOKEN HERE>"' > .env`
 5. Run `dcmetro` to start.
```

### Comparing `dcmetro-0.1.3/dcmetro.egg-info/PKG-INFO` & `dcmetro-0.1.4/dcmetro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: dcmetro
-Version: 0.1.3
+Version: 0.1.4
 Summary: Console app for sending commands to get live information on the DC Metro
 Author: Harun Feraidon
 License: MIT
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DC Metro Command Line Tool
 ![Imgur](https://i.imgur.com/rE4AKgU.gif)
 
 ## What is it
-With this application, you can submit concise commands via your terminal to request and then receive information.
+[![PyPI version](https://badge.fury.io/py/dcmetro.svg)](https://badge.fury.io/py/dcmetro)
+
+A command line app for sending commands to get live information on the DC Metro. You can find the shortest path between two stations, an estimation of the rail time between two stations, and the current arrival times for your metro station.
+[PyPi page here](https://pypi.org/project/dcmetro/0.1.3/)
 
 ## Setup
 1. Setup a python virtual environment. `python3 -m venv venv`
 2. Activate your python virtual environment. `source venv/bin/activate`
 3. Install with `pip install dcmetro`.
 4. (OPTIONAL, BUT RECOMMENDED) Skipping this step means you will be using a community API key. Creating your own API token will be more reliable. Setup a WMATA API token [here](https://developer.wmata.com). Run `echo 'API_KEY = "<YOUR TOKEN HERE>"' > .env`
 5. Run `dcmetro` to start.
```

### Comparing `dcmetro-0.1.3/setup.py` & `dcmetro-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), "r") as f:
     long_description = f.read()
 
 setup(
     name='dcmetro',
+    python_requires='>3.9',
     packages=find_packages(include=["src", "src.main"]),
-    version='0.1.3',
+    version='0.1.4',
     description='Console app for sending commands to get live information on the DC Metro',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Harun Feraidon',
     license='MIT',
     entry_points={
         "console_scripts": [
```

### Comparing `dcmetro-0.1.3/src/main/app.py` & `dcmetro-0.1.4/src/main/app.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/build_graph.py` & `dcmetro-0.1.4/src/main/build_graph.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/commands.py` & `dcmetro-0.1.4/src/main/commands.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/constants.py` & `dcmetro-0.1.4/src/main/constants.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/dijkstra.py` & `dcmetro-0.1.4/src/main/dijkstra.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/generate_station_codes.py` & `dcmetro-0.1.4/src/main/generate_station_codes.py`

 * *Files identical despite different names*

### Comparing `dcmetro-0.1.3/src/main/get_station_distances.py` & `dcmetro-0.1.4/src/main/get_station_distances.py`

 * *Files identical despite different names*

