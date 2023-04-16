# Comparing `tmp/export_ease-0.0.2.tar.gz` & `tmp/export_ease-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ease-0.0.2.tar", last modified: Sun Apr 16 21:55:50 2023, max compression
+gzip compressed data, was "export_ease-0.0.3.tar", last modified: Sun Apr 16 22:11:25 2023, max compression
```

## Comparing `export_ease-0.0.2.tar` & `export_ease-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.875713 export_ease-0.0.2/
--rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.2/LICENSE
--rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-04-16 21:55:50.875571 export_ease-0.0.2/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)     4332 2023-04-16 21:36:49.000000 export_ease-0.0.2/README.md
--rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 21:49:41.000000 export_ease-0.0.2/pyproject.toml
--rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 21:55:50.875767 export_ease-0.0.2/setup.cfg
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.874031 export_ease-0.0.2/src/
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.874843 export_ease-0.0.2/src/export_ease/
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.2/src/export_ease/__init__.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.2/src/export_ease/comtrade.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 21:48:39.000000 export_ease-0.0.2/src/export_ease/imf.py
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.875366 export_ease-0.0.2/src/export_ease.egg-info/
--rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/SOURCES.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/dependency_links.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/top_level.txt
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.321915 export_ease-0.0.3/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.3/LICENSE
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 22:11:25.321711 export_ease-0.0.3/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.3/README.md
+-rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 22:09:17.000000 export_ease-0.0.3/pyproject.toml
+-rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 22:11:25.321975 export_ease-0.0.3/setup.cfg
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.320034 export_ease-0.0.3/src/
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.320827 export_ease-0.0.3/src/export_ease/
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.3/src/export_ease/__init__.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.3/src/export_ease/comtrade.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 21:48:39.000000 export_ease-0.0.3/src/export_ease/imf.py
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 22:11:25.321358 export_ease-0.0.3/src/export_ease.egg-info/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 22:11:25.000000 export_ease-0.0.3/src/export_ease.egg-info/top_level.txt
```

### Comparing `export_ease-0.0.2/LICENSE` & `export_ease-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.2/PKG-INFO` & `export_ease-0.0.3/src/export_ease.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: export_ease
-Version: 0.0.2
+Name: export-ease
+Version: 0.0.3
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,37 +15,33 @@
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
   * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
-* When you run these functions, you'll need to enter the parameters for your query in the console. The program will ask you for the input that the query requires. Once the program's finished running, it'll output the names of the files that were just created.
+* When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
-* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the input required to make the query, but there's no need to worry about accidentally typing the wrong input, as the program will both prompt you for the type of input and ensure the input is valid before making the API call.
-  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
+* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
+  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 ### Other Notes
 * This program assumes that the source code is contained in a subdirectory within the project (e.g., ```src```) and that the files generated will be written to another subdirectory titled ```data``` (i.e., both your source code's and ```data```'s parent directory must be the root directory for your project). Be sure that your project adheres to this structure, as this package will throw errors if it can't find ```data```.
-* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities.
-* All methods defined in this package don't require any arguments, but they will prompt you for input through the console/terminal.
+* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities. In addition, no data from either source are seasonally or inflation adjusted.
 * Comtrade functions will retrieve data for the given year only, while IMF functions will retrieve data starting at the given year and ending with the most recently published data.
 * The ```get_reporter_exports``` function for IMF has a quirk that occurs when the user requests a query for annual data starting at a year within 3 years of the current year. In this case, the function will "override" the user's indicated year and instead make the starting year 3 years less than the current year--I had to add this padding in order to work around the varying structures of the JSON file returned by the IMF API. This has no serious implications, as it still gets all the data you requested (and then some).
 ## Example Python Script
 ```
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
-comtrade_obj = Comtrade()     # creating a Comtrade object so that we can use the methods of the class we imported
-imf_obj = IMF()     # creating an IMF object so that we can use the methods of the class we imported
-
 # see above documentation
-comtrade_obj.get_all_exports()
-comtrade_obj.get_total_exports()
+Comtrade.get_all_exports("B", 2021)
+Comtrade.get_total_exports("B", 2021)
 
-imf_obj.get_reporter_exports()
-imf_obj.get_total_exports()
+IMF.get_reporter_exports("France", "B", 2021)
+IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

### Comparing `export_ease-0.0.2/README.md` & `export_ease-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
   * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
-* When you run these functions, you'll need to enter the parameters for your query in the console. The program will ask you for the input that the query requires. Once the program's finished running, it'll output the names of the files that were just created.
+* When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
-* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the input required to make the query, but there's no need to worry about accidentally typing the wrong input, as the program will both prompt you for the type of input and ensure the input is valid before making the API call.
-  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
+* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
+  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 ### Other Notes
 * This program assumes that the source code is contained in a subdirectory within the project (e.g., ```src```) and that the files generated will be written to another subdirectory titled ```data``` (i.e., both your source code's and ```data```'s parent directory must be the root directory for your project). Be sure that your project adheres to this structure, as this package will throw errors if it can't find ```data```.
-* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities.
-* All methods defined in this package don't require any arguments, but they will prompt you for input through the console/terminal.
+* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities. In addition, no data from either source are seasonally or inflation adjusted.
 * Comtrade functions will retrieve data for the given year only, while IMF functions will retrieve data starting at the given year and ending with the most recently published data.
 * The ```get_reporter_exports``` function for IMF has a quirk that occurs when the user requests a query for annual data starting at a year within 3 years of the current year. In this case, the function will "override" the user's indicated year and instead make the starting year 3 years less than the current year--I had to add this padding in order to work around the varying structures of the JSON file returned by the IMF API. This has no serious implications, as it still gets all the data you requested (and then some).
 ## Example Python Script
 ```
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
-comtrade_obj = Comtrade()     # creating a Comtrade object so that we can use the methods of the class we imported
-imf_obj = IMF()     # creating an IMF object so that we can use the methods of the class we imported
-
 # see above documentation
-comtrade_obj.get_all_exports()
-comtrade_obj.get_total_exports()
+Comtrade.get_all_exports("B", 2021)
+Comtrade.get_total_exports("B", 2021)
 
-imf_obj.get_reporter_exports()
-imf_obj.get_total_exports()
+IMF.get_reporter_exports("France", "B", 2021)
+IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

### Comparing `export_ease-0.0.2/pyproject.toml` & `export_ease-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "export_ease"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Paul Dilly", email="paul.dilly@duke.edu" },
 ]
 description = "A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `export_ease-0.0.2/src/export_ease/comtrade.py` & `export_ease-0.0.3/src/export_ease/comtrade.py`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.2/src/export_ease/imf.py` & `export_ease-0.0.3/src/export_ease/imf.py`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.2/src/export_ease.egg-info/PKG-INFO` & `export_ease-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: export-ease
-Version: 0.0.2
+Name: export_ease
+Version: 0.0.3
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,37 +15,33 @@
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
   * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
-* When you run these functions, you'll need to enter the parameters for your query in the console. The program will ask you for the input that the query requires. Once the program's finished running, it'll output the names of the files that were just created.
+* When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
-* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the input required to make the query, but there's no need to worry about accidentally typing the wrong input, as the program will both prompt you for the type of input and ensure the input is valid before making the API call.
-  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
+* The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
+  * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
 ### Other Notes
 * This program assumes that the source code is contained in a subdirectory within the project (e.g., ```src```) and that the files generated will be written to another subdirectory titled ```data``` (i.e., both your source code's and ```data```'s parent directory must be the root directory for your project). Be sure that your project adheres to this structure, as this package will throw errors if it can't find ```data```.
-* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities.
-* All methods defined in this package don't require any arguments, but they will prompt you for input through the console/terminal.
+* Data is expressed in USD (Comtrade in ones, IMF in millions) and is available in both monthly and annual quantities. In addition, no data from either source are seasonally or inflation adjusted.
 * Comtrade functions will retrieve data for the given year only, while IMF functions will retrieve data starting at the given year and ending with the most recently published data.
 * The ```get_reporter_exports``` function for IMF has a quirk that occurs when the user requests a query for annual data starting at a year within 3 years of the current year. In this case, the function will "override" the user's indicated year and instead make the starting year 3 years less than the current year--I had to add this padding in order to work around the varying structures of the JSON file returned by the IMF API. This has no serious implications, as it still gets all the data you requested (and then some).
 ## Example Python Script
 ```
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
-comtrade_obj = Comtrade()     # creating a Comtrade object so that we can use the methods of the class we imported
-imf_obj = IMF()     # creating an IMF object so that we can use the methods of the class we imported
-
 # see above documentation
-comtrade_obj.get_all_exports()
-comtrade_obj.get_total_exports()
+Comtrade.get_all_exports("B", 2021)
+Comtrade.get_total_exports("B", 2021)
 
-imf_obj.get_reporter_exports()
-imf_obj.get_total_exports()
+IMF.get_reporter_exports("France", "B", 2021)
+IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

