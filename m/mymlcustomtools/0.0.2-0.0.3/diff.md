# Comparing `tmp/mymlcustomtools-0.0.2.tar.gz` & `tmp/mymlcustomtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mymlcustomtools-0.0.2.tar", last modified: Mon Apr 17 14:47:42 2023, max compression
+gzip compressed data, was "dist\mymlcustomtools-0.0.3.tar", last modified: Mon Apr 17 15:03:42 2023, max compression
```

## Comparing `mymlcustomtools-0.0.2.tar` & `mymlcustomtools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:47:42.758480 mymlcustomtools-0.0.2/
--rw-rw-rw-   0        0        0      321 2023-04-17 14:47:42.742803 mymlcustomtools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 14:47:42.720647 mymlcustomtools-0.0.2/mymlcustomtools/
--rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.2/mymlcustomtools/__init__.py
--rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.2/mymlcustomtools/imports.py
--rw-rw-rw-   0        0        0     1928 2023-04-17 14:43:43.000000 mymlcustomtools-0.0.2/mymlcustomtools/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:47:42.736264 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/
--rw-rw-rw-   0        0        0      321 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.2/mymlcustomtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:47:42.758480 mymlcustomtools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-04-17 14:47:36.000000 mymlcustomtools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:42.648380 mymlcustomtools-0.0.3/
+-rw-rw-rw-   0        0        0      321 2023-04-17 15:03:42.648380 mymlcustomtools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:42.616497 mymlcustomtools-0.0.3/mymlcustomtools/
+-rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.3/mymlcustomtools/__init__.py
+-rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.3/mymlcustomtools/imports.py
+-rw-rw-rw-   0        0        0     3277 2023-04-17 15:02:45.000000 mymlcustomtools-0.0.3/mymlcustomtools/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:42.648380 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/
+-rw-rw-rw-   0        0        0      321 2023-04-17 15:03:42.000000 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-17 15:03:42.000000 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:03:42.000000 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-04-17 15:03:42.000000 mymlcustomtools-0.0.3/mymlcustomtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:03:42.648380 mymlcustomtools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-04-17 15:03:21.000000 mymlcustomtools-0.0.3/setup.py
```

### Comparing `mymlcustomtools-0.0.2/mymlcustomtools/imports.py` & `mymlcustomtools-0.0.3/mymlcustomtools/imports.py`

 * *Files identical despite different names*

### Comparing `mymlcustomtools-0.0.2/mymlcustomtools/main.py` & `mymlcustomtools-0.0.3/mymlcustomtools/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import time
 import inspect
 import os
 import pickle
 
 __fit_model_counter = 0
 def fit(model, X, y, debug=False):
-	def pprint(text):
-		if debug: print(text)
 	global DIR_PATH
 	# Fit and time it ------------------------------------------------------------
 	initial_time = time.time()
 	model.fit(X, y)
 	final_time   = time.time()
 	elapsed_time = final_time - initial_time
 	print("Elapsed time: " + ("{:.1f} s".format(elapsed_time)) if elapsed_time < 60 else ("{:.0f} min {:.0f} s".format(round(elapsed_time,0)//60,round(elapsed_time,0)%60)) )
 
 	# Save the model -------------------------------------------------------------
+	print("-------------------------------------------------------------------------------------")
+	print(f"{ inspect = }")
+	print("-------------------------------------------------------------------------------------")
+	print(f"{ inspect.currentframe() = }")
+	print("-------------------------------------------------------------------------------------")
+	print(f"{ inspect.currentframe().f_back = }")
+	print("-------------------------------------------------------------------------------------")
+	print(f"{'__file__' in inspect.currentframe().f_back.f_globals = }")
+	if '__file__' in inspect.currentframe().f_back.f_globals:
+		print(f"{inspect.currentframe().f_back.f_globals['__file__'] = }")
+	print(f"{ inspect.currentframe().f_back.f_globals.get('__file__', None) = }")
+	filename = inspect.currentframe().f_back.f_globals.get('__file__', None)
+	print("-------------------------------------------------------------------------------------")
+	print(f"os.path.abspath(\"{filename}\") = \"{os.path.abspath(filename)}\"")
+	print("-------------------------------------------------------------------------------------")
+	print(f"os.path.dirname(os.path.abspath(\"{filename}\")) = \"{ os.path.dirname(os.path.abspath(inspect.currentframe().f_back.f_globals.get('__file__', None)))}\"")
+	print("-------------------------------------------------------------------------------------")
+
 	DIR_PATH = os.path.dirname(os.path.abspath(inspect.currentframe().f_back.f_globals.get("__file__", None)))
-	pprint(DIR_PATH)
+	print(DIR_PATH)
 	existing_models = [fn[:-6] for fn in os.listdir(DIR_PATH) if fn[-6:]==".model"]
-	pprint(existing_models)
+	print(existing_models)
 	global __fit_model_counter
 	__fit_model_counter = 1 + max(__fit_model_counter, *[int(model_name) if model_name.isnumeric() else 0 for model_name in existing_models], -1)
 
 	filepath = os.path.join(DIR_PATH, f"{__fit_model_counter}.model")
 	with open(filepath, "wb") as f:
 		print(f"Saving {filepath}...")
 		pickle.dump(model, f)
```

### Comparing `mymlcustomtools-0.0.2/setup.py` & `mymlcustomtools-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup
 
 setup(
 	name = "mymlcustomtools",
-	version = "0.0.2",
+	version = "0.0.3",
 	description = """
 	A package with frequently and useful functions for machine learning
 	""",
 	author = "Gustavo Exel",
 	author_email = "gustavoexelgpe@gmail.com",
 	url = "https://pypi.org/project/mymlcustomtools/",
 	packages = ["mymlcustomtools"],
 	zip_safe = False,
 )
 
 # py setup.py sdist 		# compiles/builds the package
 # pip install .				# locally installs the package for testing
 # twine upload dist/* 		# uploads package to PyPI
 # ---
-# py setup.py sdist && pip install . && twine upload dist/*
+# rm -r dist build && py setup.py sdist && pip install . && twine upload dist/*
+
+# cls && cd "Aprendizado de Maquina"/mymlcustomtools/ && pip install . && cd ../.. && cls && py a.py
```

