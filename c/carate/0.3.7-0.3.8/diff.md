# Comparing `tmp/carate-0.3.7.tar.gz` & `tmp/carate-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carate-0.3.7.tar", last modified: Sun Apr 16 13:12:09 2023, max compression
+gzip compressed data, was "carate-0.3.8.tar", last modified: Mon Apr 17 16:40:20 2023, max compression
```

## Comparing `carate-0.3.7.tar` & `carate-0.3.8.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/
--rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.7/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-16 13:12:09.148313 carate-0.3.7/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.7/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.144980 carate-0.3.7/carate/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-15 18:59:22.000000 carate-0.3.7/carate/automate.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-15 18:59:22.000000 carate-0.3.7/carate/config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1944 2023-04-15 18:59:22.000000 carate-0.3.7/carate/default_interface.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/evaluation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/base.py
--rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)    11480 2023-04-16 12:42:34.000000 carate-0.3.7/carate/evaluation/regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-15 18:59:22.000000 carate-0.3.7/carate/load_data.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/models/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/base_model.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/cgc_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/cgc_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-15 18:59:22.000000 carate-0.3.7/carate/optimizer.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/plotting/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    12834 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/base_plots.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1263 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/plot_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/plot_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-15 18:59:22.000000 carate-0.3.7/carate/run.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/utils/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/convert_to_json.py
--rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/model_files.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/training_result_parser.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     1065 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/top_level.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-16 13:12:03.000000 carate-0.3.7/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-16 13:12:09.148313 carate-0.3.7/setup.cfg
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.7/tests/test_cli.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.7/tests/test_data_loader.py
--rw-r--r--   0 developer  (1001) developer  (1001)      902 2023-04-13 19:42:15.000000 carate-0.3.7/tests/test_plotting.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2828 2023-04-16 12:44:17.000000 carate-0.3.7/tests/test_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.7/tests/test_runner.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_utils_convert_py_to_json.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/
+-rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.8/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-17 16:40:20.799767 carate-0.3.8/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.8/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-15 18:59:22.000000 carate-0.3.8/carate/automate.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-15 18:59:22.000000 carate-0.3.8/carate/config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1968 2023-04-17 16:22:52.000000 carate-0.3.8/carate/default_interface.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/evaluation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/base.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    11467 2023-04-17 16:22:52.000000 carate-0.3.8/carate/evaluation/regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-15 18:59:22.000000 carate-0.3.8/carate/load_data.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/models/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/base_model.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/cgc_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/cgc_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-15 18:59:22.000000 carate-0.3.8/carate/optimizer.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/carate/plotting/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/plotting/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    12892 2023-04-17 16:22:52.000000 carate-0.3.8/carate/plotting/base_plots.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1369 2023-04-17 16:21:54.000000 carate-0.3.8/carate/plotting/plot_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-15 18:59:22.000000 carate-0.3.8/carate/run.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/carate/utils/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/convert_to_json.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/model_files.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/training_result_parser.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     1030 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/top_level.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-17 16:40:12.000000 carate-0.3.8/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-17 16:40:20.803100 carate-0.3.8/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.8/tests/test_cli.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.8/tests/test_data_loader.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      978 2023-04-17 16:23:39.000000 carate-0.3.8/tests/test_plotting.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2827 2023-04-17 16:22:52.000000 carate-0.3.8/tests/test_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.8/tests/test_runner.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_utils_convert_py_to_json.py
```

### Comparing `carate-0.3.7/LICENSE` & `carate-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/PKG-INFO` & `carate-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.7
+Version: 0.3.8
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.7/README.md` & `carate-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/automate.py` & `carate-0.3.8/carate/automate.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/config.py` & `carate-0.3.8/carate/config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/default_interface.py` & `carate-0.3.8/carate/default_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,19 +22,22 @@
     The default object provides methods every class needs on top of the standard
     Python functionality.
     """
 
     def _get_defaults(self, method_arguments: Dict[Any, Any]) -> List[Any]:
         """
         The _get_defaults function takes a dictionary of arguments and returns a list of values.
-        The function checks if the value is None, if it is none then it checks to see if that key exists in the instance variables.
-        If so, then it will return the instance variable associated with that key. If not, then nothing happens and None gets returned.
+        The function checks if the value is None, if it is none then it checks to see if that key
+        exists in the instance variables.
+        If so, then it will return the instance variable associated with that key.
+        If not, then nothing happens and None gets returned.
 
         :param method_arguments:dict: Used to pass in the arguments that are passed into the method.
-        :return: A list of values that are either none or the value provided in the method_arguments dictionary.
+        :return: A list of values that are either none or the value provided in the method_arguments
+        dictionary.
 
         :doc-author: Trelent
         """
 
         result = []
         instance_variables = vars(self)  # dictionary with instance variables
         instance_attributes = instance_variables.keys()
```

### Comparing `carate-0.3.7/carate/evaluation/base.py` & `carate-0.3.8/carate/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/evaluation/regression.py` & `carate-0.3.8/carate/evaluation/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
         ) = self._get_defaults(locals())
 
         # data container
         result = {}
 
         save_model_parameters(model_net=model_net, save_dir=result_save_dir)
         for i in range(num_cv):
-            
             tmp = {}
             test_mse = []
             train_mae = []
             train_mse = []
 
             loaded_dataset: torch.utils.data.Dataset
             (
```

### Comparing `carate-0.3.7/carate/load_data.py` & `carate-0.3.8/carate/load_data.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/models/cgc_classification.py` & `carate-0.3.8/carate/models/cgc_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/models/cgc_regression.py` & `carate-0.3.8/carate/models/cgc_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/optimizer.py` & `carate-0.3.8/carate/optimizer.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/plotting/base_plots.py` & `carate-0.3.8/carate/plotting/base_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 
 def plot_range_band_single(
     result: List[Dict[str, List[float]]],
     key_val: str,
     file_name: str,
     alpha: float = 0.5,
+    fixed_y_lim=(0.0, 1.01),
     save_dir: Optional[str] = None,
     legend_text: Optional[str] = None,
 ) -> None:
     """
     The plot_range_band function takes in a list of dictionaries, each dictionary containing the
     results from one run.
     It then plots the average value for each key_val (e.g., 'accuracy') and also plots a
@@ -100,15 +101,15 @@
     fig, axis = plt.subplots()
     if legend_text is not None:
         axis.plot(avg_val, "-", label=legend_text)
     else:
         axis.plot(avg_val, "-", label=legend_text)
     plot_range_fill(max_val, min_val, alpha, axis)
 
-    axis.set_ylim(0.0, 1.01)
+    axis.set_ylim(*fixed_y_lim)
     axis.set_ylabel(key_val)
     if legend_text is not None:
         axis.legend()
 
     axis.set_xlabel("Training step")
 
     save_publication_graphic(fig_object=fig, file_name=file_name, prefix=save_dir)
@@ -225,15 +226,17 @@
         )
         results.append(result)
         logging.info(f"parsed results for CV {i}")
 
     return results
 
 
-def parse_old_file_format_for_plot(path_to_json: str) -> List[List[float]]:
+def parse_old_file_format_for_plot(
+    path_to_json: str,
+) -> List[List[float]]:  # pragma no-cover
     """
     The parse_old_file_format_for_plot function takes in a path to a json file and returns the
     following:
 
     :param path_to_json:str: Used to Specify the path to the json file that we want to parse.
     :return: A list of dictionaries.
```

### Comparing `carate-0.3.7/carate/plotting/plot_classification.py` & `carate-0.3.8/carate/plotting/plot_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Plotting function for the CARATE paper designed for classification algorithms
 
 :author: Julian M. Kleber
 """
 
 from typing import Optional
 
+from amarium.utils import append_slash
+
 from carate.plotting.base_plots import (
     plot_range_band_single,
     plot_range_band_multi,
     get_stacked_list,
 )
 
 
@@ -26,15 +28,16 @@
 
     :param path_to_directory:str: Used to specify the directory where the results are stored.
     :return: None.
 
     :doc-author: Julian M. Kleber
     """
 
-    legend_text = path_to_directory.split("/")[-1]
+    path_to_directory = append_slash(path_to_directory) + "data/"
+    legend_text = path_to_directory.split("/")[-3]
 
     if data_name is None:
         data_name = f"{legend_text}.json"
 
     result = get_stacked_list(
         path_to_directory=path_to_directory,
         num_cv=5,
```

### Comparing `carate-0.3.7/carate/run.py` & `carate-0.3.8/carate/run.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/utils/convert_to_json.py` & `carate-0.3.8/carate/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/utils/model_files.py` & `carate-0.3.8/carate/utils/model_files.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate/utils/training_result_parser.py` & `carate-0.3.8/carate/utils/training_result_parser.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/carate.egg-info/PKG-INFO` & `carate-0.3.8/carate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.7
+Version: 0.3.8
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.7/carate.egg-info/SOURCES.txt` & `carate-0.3.8/carate.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 carate/models/__init__.py
 carate/models/base_model.py
 carate/models/cgc_classification.py
 carate/models/cgc_regression.py
 carate/plotting/__init__.py
 carate/plotting/base_plots.py
 carate/plotting/plot_classification.py
-carate/plotting/plot_regression.py
 carate/utils/__init__.py
 carate/utils/convert_to_json.py
 carate/utils/model_files.py
 carate/utils/training_result_parser.py
 tests/test_classification.py
 tests/test_cli.py
 tests/test_config.py
```

### Comparing `carate-0.3.7/pyproject.toml` & `carate-0.3.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carate"
-version = "0.3.7"
+version = "0.3.8"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Providing reproducible modeling"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `carate-0.3.7/tests/test_classification.py` & `carate-0.3.8/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/tests/test_cli.py` & `carate-0.3.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/tests/test_config.py` & `carate-0.3.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/tests/test_data_loader.py` & `carate-0.3.8/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/tests/test_plotting.py` & `carate-0.3.8/tests/test_plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     )
     assert os.path.isdir("./plots")
     assert os.path.isfile(f"./plots/ENZYMES_{parameter}.png")
 
 
 def test_regression_plot_run():
     check_plotting_dir()
-    path_to_directory = "./notebooks/data/ALCHEMY_20"
+    path_to_directory = "./notebooks/data/ALCHEMY_20_test_training_length_no_norm/"
     parameter = "MAE Train"
     data_name = "alchemy_full.json"
 
     plot_classification_algorithm(
         path_to_directory=path_to_directory, parameter=parameter, data_name=data_name
     )
     assert os.path.isdir("./plots")
-    assert os.path.isfile(f"./plots/ENZYMES_{parameter}.png")
+    assert os.path.isfile(
+        f"./plots/ALCHEMY_20_test_training_length_no_norm_{parameter}.png"
+    )
```

### Comparing `carate-0.3.7/tests/test_regression.py` & `carate-0.3.8/tests/test_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     filename="train.log",
     encoding="utf-8",
     level=logging.DEBUG,
     format="%(asctime)s %(message)s",
 )
 
 
-
 def test_regression_override():
     check_dir_paths()
     config_filepath = "tests/config/regression_test_config_override.py"
     run_title = "ZINC_test"
     data_set_name = "ZINC_test"
     runner = RunInitializer.from_file(config_filepath=config_filepath)
     result_dir = f"tests/results/{run_title}"
@@ -80,13 +79,12 @@
         data_set_name=data_set_name,
         run_title=run_title,
         override=True,
     )
 
     verify_len_json(result_dir, dataset_name="alchemy_full")
 
-def verify_len_json(result_dir:str, dataset_name:str)->None:
 
-    
+def verify_len_json(result_dir: str, dataset_name: str) -> None:
     result_file = append_slash(result_dir) + f"data/CV_1/{dataset_name}.json"
     result = load_json_from_file(result_file)
-    assert len(result["MAE Train"]) == 2
+    assert len(result["MAE Train"]) == 2
```

### Comparing `carate-0.3.7/tests/test_runner.py` & `carate-0.3.8/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.7/tests/test_utils_convert_py_to_json.py` & `carate-0.3.8/tests/test_utils_convert_py_to_json.py`

 * *Files identical despite different names*

