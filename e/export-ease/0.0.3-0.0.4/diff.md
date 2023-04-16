# Comparing `tmp/export_ease-0.0.3.tar.gz` & `tmp/export_ease-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ease-0.0.3.tar", last modified: Sun Apr 16 22:11:25 2023, max compression
+gzip compressed data, was "export_ease-0.0.4.tar", last modified: Sun Apr 16 23:11:49 2023, max compression
```

## Comparing `export_ease-0.0.3.tar` & `export_ease-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.321915 export_ease-0.0.3/
--rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.3/LICENSE
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 22:11:25.321711 export_ease-0.0.3/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.3/README.md
--rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 22:09:17.000000 export_ease-0.0.3/pyproject.toml
--rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 22:11:25.321975 export_ease-0.0.3/setup.cfg
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.320034 export_ease-0.0.3/src/
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.320827 export_ease-0.0.3/src/export_ease/
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.3/src/export_ease/__init__.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.3/src/export_ease/comtrade.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 21:48:39.000000 export_ease-0.0.3/src/export_ease/imf.py
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.321358 export_ease-0.0.3/src/export_ease.egg-info/
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/SOURCES.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/dependency_links.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/top_level.txt
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.647182 export_ease-0.0.4/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.4/LICENSE
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 23:11:49.647056 export_ease-0.0.4/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.4/README.md
+-rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 23:10:45.000000 export_ease-0.0.4/pyproject.toml
+-rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 23:11:49.647220 export_ease-0.0.4/setup.cfg
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.645294 export_ease-0.0.4/src/
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.646323 export_ease-0.0.4/src/export_ease/
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.4/src/export_ease/__init__.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.4/src/export_ease/comtrade.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 23:10:39.000000 export_ease-0.0.4/src/export_ease/imf.py
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.646878 export_ease-0.0.4/src/export_ease.egg-info/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/top_level.txt
```

### Comparing `export_ease-0.0.3/LICENSE` & `export_ease-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.3/PKG-INFO` & `export_ease-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_ease
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `export_ease-0.0.3/README.md` & `export_ease-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.3/pyproject.toml` & `export_ease-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "export_ease"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Paul Dilly", email="paul.dilly@duke.edu" },
 ]
 description = "A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `export_ease-0.0.3/src/export_ease/comtrade.py` & `export_ease-0.0.4/src/export_ease/comtrade.py`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.3/src/export_ease/imf.py` & `export_ease-0.0.4/src/export_ease/imf.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         os.remove(IMF.json_path)
 
     # function to write export data to a csv file for a country to all its partners, starting at year designated by start
     @classmethod
     def get_reporter_exports(cls, rep, freq, start):
         IMF.make_country_dict()
         if (freq == "B"):
-            IMF.get_reporter_exports(rep, start, "A")
-            IMF.get_reporter_exports(rep, start, "M")
+            IMF.get_reporter_exports(rep, "A", start)
+            IMF.get_reporter_exports(rep, "M", start)
         else:
             reporter = IMF.country_dict[rep]
             csv_name = f'imf_{reporter}_all_exports_{start}{freq}.csv'
             year = int(datetime.date.today().year) - 3
             if int(start) > year and freq == "A":
                 start = str(year)
             csv_path = os.path.join(IMF.directory, csv_name)
```

### Comparing `export_ease-0.0.3/src/export_ease.egg-info/PKG-INFO` & `export_ease-0.0.4/src/export_ease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-ease
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

