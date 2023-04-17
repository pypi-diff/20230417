# Comparing `tmp/pheno-utils-0.0.8.tar.gz` & `tmp/pheno-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.0.8.tar", last modified: Tue Apr 11 12:31:04 2023, max compression
+gzip compressed data, was "pheno-utils-0.0.9.tar", last modified: Wed Apr 12 09:26:19 2023, max compression
```

## Comparing `pheno-utils-0.0.8.tar` & `pheno-utils-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.813919 pheno-utils-0.0.8/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.8/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.8/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-11 12:31:04.813310 pheno-utils-0.0.8/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.8/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.809364 pheno-utils-0.0.8/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    12655 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/dates_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.812771 pheno-utils-0.0.8/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.8/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-11 12:25:58.000000 pheno-utils-0.0.8/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-11 12:31:04.814034 pheno-utils-0.0.8/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.8/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-12 09:26:19.619724 pheno-utils-0.0.9/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.9/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.9/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-12 09:26:19.619252 pheno-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.9/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-12 09:26:19.614669 pheno-utils-0.0.9/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     9879 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    14190 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-12 09:22:13.000000 pheno-utils-0.0.9/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-12 09:26:19.618550 pheno-utils-0.0.9/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      542 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.9/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-12 09:26:19.000000 pheno-utils-0.0.9/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-12 09:18:58.000000 pheno-utils-0.0.9/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-12 09:26:19.619908 pheno-utils-0.0.9/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.9/setup.py
```

### Comparing `pheno-utils-0.0.8/LICENSE` & `pheno-utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/PKG-INFO` & `pheno-utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.8/pheno_utils/_modidx.py` & `pheno-utils-0.0.9/pheno_utils/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,14 @@
                                                                                                            'pheno_utils/blandaltman_plots.py')},
             'pheno_utils.config': { 'pheno_utils.config.generate_synthetic_data': ( 'config.html#generate_synthetic_data',
                                                                                     'pheno_utils/config.py'),
                                     'pheno_utils.config.generate_synthetic_data_like': ( 'config.html#generate_synthetic_data_like',
                                                                                          'pheno_utils/config.py')},
             'pheno_utils.data_loader': { 'pheno_utils.data_loader.DataLoader': ( 'data_loader.html#dataloader',
                                                                                  'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__get_data__': ( 'data_loader.html#dataloader.__get_data__',
-                                                                                              'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__get_file_path__': ( 'data_loader.html#dataloader.__get_file_path__',
                                                                                                    'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__getitem__': ( 'data_loader.html#dataloader.__getitem__',
                                                                                              'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__init__': ( 'data_loader.html#dataloader.__init__',
                                                                                           'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__load_age_sex__': ( 'data_loader.html#dataloader.__load_age_sex__',
@@ -57,11 +55,23 @@
                                                                                                      'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__load_one_dataframe__': ( 'data_loader.html#dataloader.__load_one_dataframe__',
                                                                                                         'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__repr__': ( 'data_loader.html#dataloader.__repr__',
                                                                                           'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__str__': ( 'data_loader.html#dataloader.__str__',
                                                                                          'pheno_utils/data_loader.py'),
+                                         'pheno_utils.data_loader.DataLoader.get': ( 'data_loader.html#dataloader.get',
+                                                                                     'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.load_sample_data': ( 'data_loader.html#dataloader.load_sample_data',
                                                                                                   'pheno_utils/data_loader.py')},
             'pheno_utils.dates_plots': { 'pheno_utils.dates_plots.dates_dist_plot': ( 'date_plots.html#dates_dist_plot',
-                                                                                      'pheno_utils/dates_plots.py')}}}
+                                                                                      'pheno_utils/dates_plots.py')},
+            'pheno_utils.sleep_plots': { 'pheno_utils.sleep_plots.format_xticks': ( 'sleep_plots.html#format_xticks',
+                                                                                    'pheno_utils/sleep_plots.py'),
+                                         'pheno_utils.sleep_plots.get_legend_colors': ( 'sleep_plots.html#get_legend_colors',
+                                                                                        'pheno_utils/sleep_plots.py'),
+                                         'pheno_utils.sleep_plots.plot_channels': ( 'sleep_plots.html#plot_channels',
+                                                                                    'pheno_utils/sleep_plots.py'),
+                                         'pheno_utils.sleep_plots.plot_events': ( 'sleep_plots.html#plot_events',
+                                                                                  'pheno_utils/sleep_plots.py'),
+                                         'pheno_utils.sleep_plots.plot_sleep': ( 'sleep_plots.html#plot_sleep',
+                                                                                 'pheno_utils/sleep_plots.py')}}}
```

### Comparing `pheno-utils-0.0.8/pheno_utils/age_reference_plots.py` & `pheno-utils-0.0.9/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/pheno_utils/basic_plots.py` & `pheno-utils-0.0.9/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.0.9/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/pheno_utils/config.py` & `pheno-utils-0.0.9/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/pheno_utils/data_loader.py` & `pheno-utils-0.0.9/pheno_utils/data_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # %% auto 0
 __all__ = ['DataLoader']
 
 # %% ../nbs/05_data_loader.ipynb 3
 from glob import glob
 import os
+import re
 from typing import List, Union
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from .config import *
@@ -26,14 +27,15 @@
         cohort (str, optional): The name of the cohort within the dataset. Defaults to '10k'.
         base_path (str, optional): The base path where the data is stored. Defaults to '/home/ec2-user/studies'.
         age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to 'Population_Characteristics'.
         skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
+        flexible_field_search (bool, optional): Whether to allow regex field search. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
             Possible values are 'raise' and 'warn'. Defaults to 'raise'.
 
     Attributes:
     
         dict (pd.DataFrame): The data dictionary for the dataset, containing information about each field.
         dfs (dict): A dictionary of dataframes, one for each table in the dataset.
@@ -42,63 +44,68 @@
         cohort (str): The name of the cohort being used.
         base_path (str): The base path where the data is stored.
         age_sex_dataset (str): The name of the dataset being used to compute age and sex.
         skip_dfs (list): A list of tables to skip when loading the data.
         unique_index (bool): Whether to ensure the index of the data is unique.
         valid_dates (bool): Whether to ensure that all timestamps in the data are valid dates.
         valid_stage (bool): Whether to ensure that all research stages in the data are valid.
+        flexible_field_search (bool): Whether to allow regex field search.
         errors (str): Whether to raise an error or issue a warning if missing data is encountered.
     """
 
     def __init__(
         self,
         dataset: str,
         cohort: str = '10k',
         base_path: str = DATASETS_PATH,
         age_sex_dataset: str = POPULATION_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
+        flexible_field_search: bool = False,
         errors: str = 'raise'
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.age_sex_dataset = age_sex_dataset
         self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
+        self.flexible_field_search = flexible_field_search
         self.errors = errors
 
         self.__load_dictionary__()
         self.__load_dataframes__()
         if self.age_sex_dataset is not None:
             self.__load_age_sex__()
 
     def load_sample_data(
         self,
         field_name: str,
         participant_id: Union[int, List[int]],
         research_stage: Union[None, str, List[str]] = None,
         array_index: Union[None, int, List[int]] = None,
         load_func: callable = pd.read_parquet,
-        concat: bool = True
+        concat: bool = True,
+        pivot=None, **kwargs
     ) -> Union[pd.DataFrame, None]:
         """
         Load time series or bulk data for sample(s).
 
         Args:
             field_name (str): The name of the field to load.
             participant_id (str or list): The participant ID or IDs to load data for.
             research_stage (str or list, optional): The research stage or stages to load data for.
             array_index (int or list, optional): The array index or indices to load data for.
             load_func (callable, optional): The function to use to load the data. Defaults to pd.read
-            concat (bool, optional): Whether to concatenate the data into a single DataFrame. Defaults to True.
+            concat (bool, optional): Whether to concatenate the data into a single DataFrame. Automatically ignored if data is not a DataFrame. Defaults to True.
+            pivot (str, optional): The name of the field to pivot the data on (if DataFrame). Defaults to None.
         """
         query_str = 'participant_id in @participant_id'
         if not isinstance(participant_id, list):
             participant_id = [participant_id]
         if research_stage is not None:
             if not isinstance(research_stage, list):
                 research_stage = [research_stage]
@@ -119,27 +126,35 @@
             if self.errors == 'raise':
                 raise ValueError(f'Missing samples: {missing_participants}')
             elif self.errors == 'warn':
                 warnings.warn(f'Missing samples: {missing_participants}')
             if len(sample) == 0:
                 return None
 
+        # Load data
         data = []
         for p in sample.unique():
             try:
-                data.append(load_func(p))
+                data.append(load_func(p, **kwargs))
                 if isinstance(data[-1], pd.DataFrame):
                     data[-1].sort_index(inplace=True)
             except Exception as e:
                 if self.errors == 'raise':
                     raise e
                 elif self.errors == 'warn':
                     warnings.warn(f'Error loading {p}: {e}')
-        if concat:
+
+        # Format the final result
+        if concat and isinstance(data[0], pd.DataFrame):
             data = pd.concat(data, axis=0)
+        if pivot is not None and isinstance(data, pd.DataFrame):
+            if pivot in data.index.names:
+                data = data.reset_index(pivot)
+            data = data.pivot(columns=pivot)
+
         return data
 
     def __repr__(self):
         """
         Return string representation of object
 
         Returns:
@@ -153,56 +168,70 @@
 
         Returns:
             str: String representation of object
         """
         return f'DataLoader for {self.dataset} with' +\
             f'\n{len(self.fields)} fields\n{len(self.dfs)} tables: {list(self.dfs.keys())}'
 
-    def __getitem__(self, fields):
+    def __getitem__(self, fields: Union[str,List[str]]):
         """
         Return data for the specified fields from all tables
 
         Args:
             fields (Union[str, List[str]]): Fields to return
 
         Returns:
             pd.DataFrame: Data for the specified fields from all tables
         """
-        if isinstance(fields, str):
-            fields = [fields]
-        return self.__get_data__(fields)
+        return self.get(fields)
 
-    def __get_data__(self, fields):
+    def get(self, fields: Union[str,List[str]], flexible: bool=None):
         """
         Return data for the specified fields from all tables
 
         Args:
             fields (List[str]): Fields to return
+            flexible (bool, optional): Whether to use fuzzy matching to find fields. Defaults to None, which uses the DataLoader's flexible_field_search attribute.
 
         Returns:
             pd.DataFrame: Data for the specified fields from all tables
         """
+        if flexible is None:
+            flexible = self.flexible_field_search
+        if isinstance(fields, str):
+            fields = [fields]
+
         data = []
         for df in self.dfs.values():
-            fields_in_df = df.columns.intersection(fields)
-            if len(fields_in_df):
-                data.append(df[fields_in_df])
-        data = pd.concat(data, axis=1)
-        data = data.loc[:, ~data.columns.duplicated()]
-
-        fields_in_index = np.intersect1d(fields, data.index.names)
-        for field in fields_in_index:
-            data[field] = data.index.get_level_values(field)
+            if flexible:
+                # use fuzzy matching including regex to find fields
+                fields_in_col = [col for f in fields for col in df.columns if re.search(f, col)]
+            else:
+                fields_in_col = df.columns.intersection(fields)
+            if len(fields_in_col):
+                data.append(df[fields_in_col])
+
+            fields_in_index = np.intersect1d(df.index.names, fields)
+            if len(fields_in_index):
+                data.append(pd.DataFrame(
+                    df.index.get_level_values(fields_in_index),
+                    index=df.index))
+
+        if len(data):
+            data = pd.concat(data, axis=1)
+            data = data.loc[:, ~data.columns.duplicated()]
+        else:
+            data = pd.DataFrame()
 
         not_found = np.setdiff1d(fields, data.columns)
-        if len(not_found):
+        if len(not_found) and not flexible:
             if self.errors == 'raise':
                 raise KeyError(f'Fields not found: {not_found}')
             elif self.errors == 'warn':
-                warnings.warn(f'Fileds not found: {not_found}')
+                warnings.warn(f'Fields not found: {not_found}')
 
         return data
 
     def __load_age_sex__(self) -> None:
         """
         Add sex and compute age from birth date.
         """
@@ -245,15 +274,18 @@
         """
         self.dfs = {}
         self.fields = set()
         for relative_location in self.dict['relative_location'].dropna().unique():
             if any([pattern in relative_location for pattern in self.skip_dfs]):
                 print(f'Skipping {relative_location}')
                 continue
-            self.dfs[relative_location.split('.')[0]] = self.__load_one_dataframe__(relative_location)
+            df = self.__load_one_dataframe__(relative_location)
+            if df is None:
+                continue
+            self.dfs[relative_location.split('.')[0]] = df
             self.fields |= set(self.dfs[relative_location.split('.')[0]].columns.tolist())
         self.fields = list(self.fields)
 
     def __load_one_dataframe__(self, relative_location: str) -> pd.DataFrame:
         """
         Load one dataframe.
 
@@ -271,15 +303,15 @@
         try:
             data =  pd.read_parquet(df_path)
         except Exception as err:
             if self.errors == 'raise':
                 raise err
             if self.errors == 'warn':
                 warnings.warn(f'Error loading {df_path}:\n{err}')
-            return pd.DataFrame()
+            return None
 
         # set the order of columns according to the dictionary
         dict_columns = self.dict.index.intersection(data.columns)
         other_columns = data.columns.difference(self.dict.index)
         assert (len(dict_columns) + len(other_columns)) == len(data.columns), "something isn't right"
         data = data[dict_columns.tolist() + other_columns.tolist()]
```

### Comparing `pheno-utils-0.0.8/pheno_utils/dates_plots.py` & `pheno-utils-0.0.9/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.8/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.0.9/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.8/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.0.9/pheno_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pheno_utils/_modidx.py
 pheno_utils/age_reference_plots.py
 pheno_utils/basic_plots.py
 pheno_utils/blandaltman_plots.py
 pheno_utils/config.py
 pheno_utils/data_loader.py
 pheno_utils/dates_plots.py
+pheno_utils/sleep_plots.py
 pheno_utils.egg-info/PKG-INFO
 pheno_utils.egg-info/SOURCES.txt
 pheno_utils.egg-info/dependency_links.txt
 pheno_utils.egg-info/entry_points.txt
 pheno_utils.egg-info/not-zip-safe
 pheno_utils.egg-info/requires.txt
 pheno_utils.egg-info/top_level.txt
```

### Comparing `pheno-utils-0.0.8/settings.ini` & `pheno-utils-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.0.8/setup.py` & `pheno-utils-0.0.9/setup.py`

 * *Files identical despite different names*

