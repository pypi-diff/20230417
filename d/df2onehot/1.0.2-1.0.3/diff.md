# Comparing `tmp/df2onehot-1.0.2.tar.gz` & `tmp/df2onehot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df2onehot-1.0.2.tar", last modified: Fri Dec  2 15:19:57 2022, max compression
+gzip compressed data, was "df2onehot-1.0.3.tar", last modified: Mon Apr 17 21:34:03 2023, max compression
```

## Comparing `df2onehot-1.0.2.tar` & `df2onehot-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 15:19:57.040893 df2onehot-1.0.2/
--rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       58 2021-02-09 21:19:52.000000 df2onehot-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3229 2022-12-02 15:19:57.040893 df2onehot-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-02 15:19:57.018966 df2onehot-1.0.2/df2onehot/
--rw-rw-rw-   0        0        0      692 2022-12-02 15:19:07.000000 df2onehot-1.0.2/df2onehot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-02 15:19:57.037901 df2onehot-1.0.2/df2onehot/data/
--rw-rw-rw-   0        0        0     3928 2022-03-13 12:30:44.000000 df2onehot-1.0.2/df2onehot/data/FIFA_2018.zip
--rw-rw-rw-   0        0        0   147068 2022-03-13 12:31:34.000000 df2onehot-1.0.2/df2onehot/data/cancer_dataset.zip
--rw-rw-rw-   0        0        0    14904 2022-03-13 12:31:04.000000 df2onehot-1.0.2/df2onehot/data/marketing_data_online_retail_small.zip
--rw-rw-rw-   0        0        0     1049 2022-03-13 13:39:12.000000 df2onehot-1.0.2/df2onehot/data/sprinkler.zip
--rw-rw-rw-   0        0        0    11296 2022-03-13 12:30:27.000000 df2onehot-1.0.2/df2onehot/data/student_train.zip
--rw-rw-rw-   0        0        0    22510 2022-03-12 19:40:15.000000 df2onehot-1.0.2/df2onehot/data/titanic_train.zip
--rw-rw-rw-   0        0        0    20592 2022-03-18 12:10:46.000000 df2onehot-1.0.2/df2onehot/df2onehot.py
--rw-rw-rw-   0        0        0      968 2022-03-13 13:31:26.000000 df2onehot-1.0.2/df2onehot/examples.py
-drwxrwxrwx   0        0        0        0 2022-12-02 15:19:57.040047 df2onehot-1.0.2/df2onehot/tests/
--rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.2/df2onehot/tests/__init__.py
--rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.2/df2onehot/tests/test_df2onehot.py
--rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.2/df2onehot/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-02 15:19:57.024915 df2onehot-1.0.2/df2onehot.egg-info/
--rw-rw-rw-   0        0        0     3229 2022-12-02 15:19:56.000000 df2onehot-1.0.2/df2onehot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2022-12-02 15:19:56.000000 df2onehot-1.0.2/df2onehot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 15:19:56.000000 df2onehot-1.0.2/df2onehot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2022-12-02 15:19:56.000000 df2onehot-1.0.2/df2onehot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-02 15:19:56.000000 df2onehot-1.0.2/df2onehot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-02 15:19:57.041858 df2onehot-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1420 2022-12-02 15:05:15.000000 df2onehot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.460909 df2onehot-1.0.3/
+-rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-17 21:33:01.000000 df2onehot-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3188 2023-04-17 21:34:03.458043 df2onehot-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.375160 df2onehot-1.0.3/df2onehot/
+-rw-rw-rw-   0        0        0      692 2023-04-17 21:29:35.000000 df2onehot-1.0.3/df2onehot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.432181 df2onehot-1.0.3/df2onehot/data/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.3/df2onehot/data/__init__.py
+-rw-rw-rw-   0        0        0    21315 2023-04-17 21:24:53.000000 df2onehot-1.0.3/df2onehot/df2onehot.py
+-rw-rw-rw-   0        0        0      968 2023-04-17 19:45:54.000000 df2onehot-1.0.3/df2onehot/examples.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.453915 df2onehot-1.0.3/df2onehot/tests/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.3/df2onehot/tests/__init__.py
+-rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.3/df2onehot/tests/test_df2onehot.py
+-rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.3/df2onehot/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.429718 df2onehot-1.0.3/df2onehot.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-17 21:34:03.000000 df2onehot-1.0.3/df2onehot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 21:34:03.000000 df2onehot-1.0.3/df2onehot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:34:03.460909 df2onehot-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2022-12-02 15:05:15.000000 df2onehot-1.0.3/setup.py
```

### Comparing `df2onehot-1.0.2/LICENSE` & `df2onehot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.2/PKG-INFO` & `df2onehot-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.2.tar.gz
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,9 +83,7 @@
 
 <hr>
 
 #### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.3 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
 page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.2.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # df2onehot [!
-[Python](https://img.shields.io/pypi/pyversions/df2onehot)](https://
-img.shields.io/pypi/pyversions/df2onehot) [![PyPI Version](https://
-img.shields.io/pypi/v/df2onehot)](https://pypi.org/project/df2onehot/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/df2onehot/blob/master/LICENSE) [![Downloads](https://
-pepy.tech/badge/df2onehot/month)](https://pepy.tech/project/df2onehot/month) [!
-[Downloads](https://pepy.tech/badge/df2onehot)](https://pepy.tech/project/
-df2onehot) [![DOI](https://zenodo.org/badge/245003302.svg)](https://zenodo.org/
-badge/latestdoi/245003302) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-
-Green)](https://erdogant.github.io/df2onehot/)   ``df2onehot`` is a Python
-package to convert unstructured DataFrames into structured dataframes, such as
-one-hot dense arrays. # **â­ï¸ Star this repo if you like it â­ï¸** # ####
-Install df2onehot from PyPI ```bash pip install df2onehot ``` #### Import
-df2onehot package ```python from df2onehot import df2onehot ``` # ###
-[Documentation pages](https://erdogant.github.io/df2onehot/) On the
-[documentation pages](https://erdogant.github.io/df2onehot/) you can find
-detailed information about the working of the ``df2onehot`` with many examples.
+erdogant/df2onehot/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
+pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
+[PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
+project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/df2onehot/blob/master/LICENSE) [!
+[Downloads](https://pepy.tech/badge/df2onehot/month)](https://pepy.tech/
+project/df2onehot/month) [![Downloads](https://pepy.tech/badge/df2onehot)]
+(https://pepy.tech/project/df2onehot) [![DOI](https://zenodo.org/badge/
+245003302.svg)](https://zenodo.org/badge/latestdoi/245003302) [![Sphinx](https:
+//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+df2onehot/)   ``df2onehot`` is a Python package to convert unstructured
+DataFrames into structured dataframes, such as one-hot dense arrays. # **â­ï¸
+Star this repo if you like it â­ï¸** # #### Install df2onehot from PyPI
+```bash pip install df2onehot ``` #### Import df2onehot package ```python from
+df2onehot import df2onehot ``` # ### [Documentation pages](https://
+erdogant.github.io/df2onehot/) On the [documentation pages](https://
+erdogant.github.io/df2onehot/) you can find detailed information about the
+working of the ``df2onehot`` with many examples.
 ===============================================================================
 ### Examples ```python results = df2onehot(df) ``` ```python # Force features
 (int or float) to be numeric if unique non-zero values are above percentage.
 out = df2onehot(df, perc_min_num=0.8) ``` ```python # Remove categorical
 features for which less then 2 values exists. out = df2onehot(df, y_min=2) ```
 ```python # Combine two rules above. out = df2onehot(df, y_min=2,
 perc_min_num=0.8) ``` # * [Example: Process Mixed dataset](https://
```

### Comparing `df2onehot-1.0.2/README.md` & `df2onehot-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.2/df2onehot/__init__.py` & `df2onehot-1.0.3/df2onehot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  	set_dtypes,
  	is_DataFrame,
     set_y,
 )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 # module level doc-string
 __doc__ = """
 df2onehot is an Python package to convert a pandas dataframe into a stuctured dataframe.
 =============================================================================================
 
 Description
```

### Comparing `df2onehot-1.0.2/df2onehot/df2onehot.py` & `df2onehot-1.0.3/df2onehot/df2onehot.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from df2onehot.utils import set_dtypes
 # from set_dtypes import set_dtypes
 label_encoder = LabelEncoder()
 onehot_encoder = OneHotEncoder(sparse=False, categories='auto')
 warnings.filterwarnings('ignore')
 
 # %% Dataframe to one-hot
-def df2onehot(df, dtypes='pandas', y_min=None, perc_min_num=None, hot_only=True, deep_extract=False, excl_background=None, verbose=3):
+def df2onehot(df, dtypes='pandas', y_min=None, perc_min_num=None, hot_only=True, deep_extract=False, excl_background=None, remove_mutual_exclusive=False, verbose=3):
     """Convert dataframe to one-hot matrix.
 
     Parameters
     ----------
     df : pd.DataFrame()
         Input dataframe for which the rows are the features, and colums are the samples.
     dtypes : list of str or 'pandas', optional
@@ -37,14 +37,17 @@
     perc_min_num : float [None, 0..1], optional
         This parameters can be used to force variables into numeric ones if unique non-zero values are above the percentage. The default is None. Alternative can be 0.8
     hot_only : bool [True, False], optional
         When True; the output of the onehot matrix exclusively contains categorical values that are transformed to one-hot. The default is True.
     deep_extract : bool [False, True] (default : False)
         True: Extract information from a vector that contains a list/array/dict.
         False: converted to a string and treated as catagorical ['cat'].
+    remove_mutual_exclusive : bool [False, True] (default : False)
+        True: Remove the mutual exclusive groups. In binairy features; False and 0 are excluded.
+        False: Do nothing
     excl_background : list or None, [0], [0, '0.0', 'unknown', 'nan', 'None' ...], optional
         Remove values/strings that labeled in the list. As an example, the following column: ['yes', 'no', 'yes', 'yes','no','unknown', ...], is split into 'column_yes', 'column_no' and 'column_unknown'. If unknown listed, then 'column_unknown' is not transformed into a new one-hot column.
         The default is None (every possible name is converted into a one-hot column)
     verbose : int, optional
         Print message to screen. The default is 3.
         0: (default), 1: ERROR, 2: WARN, 3: INFO, 4: DEBUG, 5: TRACE
 
@@ -112,16 +115,26 @@
             # If all values are the same, the encoder will return 0 (=False). We set values at 1 (by +1) and make them True. Otherwise it can be mis interpreted the the value was not present in the datset.
             if np.all(np.unique(integer_encoded)==0): integer_encoded=integer_encoded + 1
             # integer_encoded = set_y(integer_encoded, y_min=y_min, numeric=True, verbose=0)
             out_numeric[df.columns[i]] = integer_encoded
             out_numeric[df.columns[i]] = out_numeric[df.columns[i]].astype('category')
             if verbose>=4: print('[df2onehot] >Processing: %s%s [%.0f]' %(df.columns[i][0:maxstring], makespaces, len(np.unique(integer_encoded)) ))
 
+            # Remove mutual exclusive values
+            status_bool=False
+            if remove_mutual_exclusive and len(np.unique(integer_encoded))==2:
+                if np.isin(np.unique(integer_encoded), [0, 1]).sum()>=2:
+                    status_bool=True
+
             # Contains a single value or is bool
-            if (len(np.unique(integer_encoded))<=1) or (str(df.dtypes[i])=='bool'):
+            if status_bool:
+                label = df.columns[i] + '_' + str(df.iloc[integer_encoded==1, i].values[0])
+                out_onehot[label] = integer_encoded.astype('bool')
+                labx.append(label)
+            elif (len(np.unique(integer_encoded))<=1) or (str(df.dtypes[i])=='bool'):
                 out_onehot[df.columns[i]] = integer_encoded.astype('bool')
                 labx.append(df.columns[i])
             else:
                 # binary encode
                 onehot_encoded = onehot_encoder.fit_transform(integer_encoded.reshape(-1, 1))
                 # Remove columns if it does not fullfill minimum nr. of samples (>=y_min)
                 if y_min is not None:
```

### Comparing `df2onehot-1.0.2/df2onehot/examples.py` & `df2onehot-1.0.3/df2onehot/examples.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.2/df2onehot/tests/test_df2onehot.py` & `df2onehot-1.0.3/df2onehot/tests/test_df2onehot.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.2/df2onehot/utils.py` & `df2onehot-1.0.3/df2onehot/utils.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.2/df2onehot.egg-info/PKG-INFO` & `df2onehot-1.0.3/df2onehot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.2.tar.gz
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,9 +83,7 @@
 
 <hr>
 
 #### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.3 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
 page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.2.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # df2onehot [!
-[Python](https://img.shields.io/pypi/pyversions/df2onehot)](https://
-img.shields.io/pypi/pyversions/df2onehot) [![PyPI Version](https://
-img.shields.io/pypi/v/df2onehot)](https://pypi.org/project/df2onehot/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/df2onehot/blob/master/LICENSE) [![Downloads](https://
-pepy.tech/badge/df2onehot/month)](https://pepy.tech/project/df2onehot/month) [!
-[Downloads](https://pepy.tech/badge/df2onehot)](https://pepy.tech/project/
-df2onehot) [![DOI](https://zenodo.org/badge/245003302.svg)](https://zenodo.org/
-badge/latestdoi/245003302) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-
-Green)](https://erdogant.github.io/df2onehot/)   ``df2onehot`` is a Python
-package to convert unstructured DataFrames into structured dataframes, such as
-one-hot dense arrays. # **â­ï¸ Star this repo if you like it â­ï¸** # ####
-Install df2onehot from PyPI ```bash pip install df2onehot ``` #### Import
-df2onehot package ```python from df2onehot import df2onehot ``` # ###
-[Documentation pages](https://erdogant.github.io/df2onehot/) On the
-[documentation pages](https://erdogant.github.io/df2onehot/) you can find
-detailed information about the working of the ``df2onehot`` with many examples.
+erdogant/df2onehot/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
+pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
+[PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
+project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/df2onehot/blob/master/LICENSE) [!
+[Downloads](https://pepy.tech/badge/df2onehot/month)](https://pepy.tech/
+project/df2onehot/month) [![Downloads](https://pepy.tech/badge/df2onehot)]
+(https://pepy.tech/project/df2onehot) [![DOI](https://zenodo.org/badge/
+245003302.svg)](https://zenodo.org/badge/latestdoi/245003302) [![Sphinx](https:
+//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+df2onehot/)   ``df2onehot`` is a Python package to convert unstructured
+DataFrames into structured dataframes, such as one-hot dense arrays. # **â­ï¸
+Star this repo if you like it â­ï¸** # #### Install df2onehot from PyPI
+```bash pip install df2onehot ``` #### Import df2onehot package ```python from
+df2onehot import df2onehot ``` # ### [Documentation pages](https://
+erdogant.github.io/df2onehot/) On the [documentation pages](https://
+erdogant.github.io/df2onehot/) you can find detailed information about the
+working of the ``df2onehot`` with many examples.
 ===============================================================================
 ### Examples ```python results = df2onehot(df) ``` ```python # Force features
 (int or float) to be numeric if unique non-zero values are above percentage.
 out = df2onehot(df, perc_min_num=0.8) ``` ```python # Remove categorical
 features for which less then 2 values exists. out = df2onehot(df, y_min=2) ```
 ```python # Combine two rules above. out = df2onehot(df, y_min=2,
 perc_min_num=0.8) ``` # * [Example: Process Mixed dataset](https://
```

### Comparing `df2onehot-1.0.2/setup.py` & `df2onehot-1.0.3/setup.py`

 * *Files identical despite different names*

