# Comparing `tmp/mymlcustomtools-0.0.5.tar.gz` & `tmp/mymlcustomtools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mymlcustomtools-0.0.5.tar", last modified: Mon Apr 17 15:22:01 2023, max compression
+gzip compressed data, was "dist\mymlcustomtools-0.0.6.tar", last modified: Mon Apr 17 15:23:50 2023, max compression
```

## Comparing `mymlcustomtools-0.0.5.tar` & `mymlcustomtools-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:22:01.635387 mymlcustomtools-0.0.5/
--rw-rw-rw-   0        0        0      321 2023-04-17 15:22:01.635387 mymlcustomtools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 15:22:01.619768 mymlcustomtools-0.0.5/mymlcustomtools/
--rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.5/mymlcustomtools/__init__.py
--rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.5/mymlcustomtools/imports.py
--rw-rw-rw-   0        0        0     1976 2023-04-17 15:21:27.000000 mymlcustomtools-0.0.5/mymlcustomtools/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:22:01.635387 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/
--rw-rw-rw-   0        0        0      321 2023-04-17 15:22:01.000000 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-17 15:22:01.000000 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:22:01.000000 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-17 15:22:01.000000 mymlcustomtools-0.0.5/mymlcustomtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:22:01.635387 mymlcustomtools-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-04-17 15:22:00.000000 mymlcustomtools-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/
+-rw-rw-rw-   0        0        0      321 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.440769 mymlcustomtools-0.0.6/mymlcustomtools/
+-rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.6/mymlcustomtools/__init__.py
+-rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.6/mymlcustomtools/imports.py
+-rw-rw-rw-   0        0        0     2065 2023-04-17 15:23:44.000000 mymlcustomtools-0.0.6/mymlcustomtools/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/
+-rw-rw-rw-   0        0        0      321 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-04-17 15:23:49.000000 mymlcustomtools-0.0.6/setup.py
```

### Comparing `mymlcustomtools-0.0.5/mymlcustomtools/imports.py` & `mymlcustomtools-0.0.6/mymlcustomtools/imports.py`

 * *Files identical despite different names*

### Comparing `mymlcustomtools-0.0.5/mymlcustomtools/main.py` & `mymlcustomtools-0.0.6/mymlcustomtools/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 	filepath = os.path.join(DIR_PATH, f"{__fit_model_counter}.model")
 	with open(filepath, "wb") as f:
 		print(f"Saving {filepath}...")
 		pickle.dump(model, f)
 
 def load_models(model_number=None):
 	global DIR_PATH
-	DIR_PATH = os.path.dirname(os.path.abspath(inspect.currentframe().f_back.f_globals.get("__file__", None)))
+	exec_filename = inspect.currentframe().f_back.f_globals.get('__file__', None)
+	if exec_filename is None: DIR_PATH = "/content/"
+	else: DIR_PATH = os.path.dirname(os.path.abspath(exec_filename))
 	existing_models = [fn[:-6] for fn in os.listdir(DIR_PATH) if fn[-6:]==".model"]
 
 	if model_number is None:
 		if existing_models:
 			print("Existing models:\n"+"\n".join([model_name+".model" for model_name in existing_models]))
 		else:
 			print("No model saved")
```

### Comparing `mymlcustomtools-0.0.5/setup.py` & `mymlcustomtools-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name = "mymlcustomtools",
-	version = "0.0.5",
+	version = "0.0.6",
 	description = """
 	A package with frequently and useful functions for machine learning
 	""",
 	author = "Gustavo Exel",
 	author_email = "gustavoexelgpe@gmail.com",
 	url = "https://pypi.org/project/mymlcustomtools/",
 	packages = ["mymlcustomtools"],
```

