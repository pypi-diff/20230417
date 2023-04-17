# Comparing `tmp/gmltools-0.0.59.tar.gz` & `tmp/gmltools-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.59.tar", last modified: Fri Apr 14 10:52:53 2023, max compression
+gzip compressed data, was "gmltools-0.0.60.tar", last modified: Mon Apr 17 07:51:02 2023, max compression
```

## Comparing `gmltools-0.0.59.tar` & `gmltools-0.0.60.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.855181 gmltools-0.0.59/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.59/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.59/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-14 10:52:53.855181 gmltools-0.0.59/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.59/README.md
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.59/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.59/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-14 10:44:20.000000 gmltools-0.0.59/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 10:52:53.855181 gmltools-0.0.59/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-14 10:44:12.000000 gmltools-0.0.59/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.809669 gmltools-0.0.59/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.820596 gmltools-0.0.59/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.59/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.59/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.836231 gmltools-0.0.59/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.59/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.59/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.844144 gmltools-0.0.59/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.59/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.59/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.59/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5137 2023-04-14 09:39:40.000000 gmltools-0.0.59/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119078 2023-04-14 10:28:24.000000 gmltools-0.0.59/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.59/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    12799 2023-04-14 10:43:53.000000 gmltools-0.0.59/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.848174 gmltools-0.0.59/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.59/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.59/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.59/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.853162 gmltools-0.0.59/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.59/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.59/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.59/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.59/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:53.834228 gmltools-0.0.59/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-14 10:52:53.000000 gmltools-0.0.59/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2023-04-14 10:52:53.000000 gmltools-0.0.59/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:52:53.000000 gmltools-0.0.59/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-14 10:52:53.000000 gmltools-0.0.59/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 10:52:53.000000 gmltools-0.0.59/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.715516 gmltools-0.0.60/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.60/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.60/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-17 07:51:02.714539 gmltools-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.60/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.558811 gmltools-0.0.60/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.60/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.60/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.60/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-17 07:50:11.000000 gmltools-0.0.60/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:51:02.715516 gmltools-0.0.60/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-17 07:49:54.000000 gmltools-0.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.501195 gmltools-0.0.60/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.574332 gmltools-0.0.60/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.60/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.60/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.612204 gmltools-0.0.60/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.60/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.60/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.656108 gmltools-0.0.60/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.60/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.60/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.60/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.60/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119078 2023-04-14 10:28:24.000000 gmltools-0.0.60/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.60/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    12799 2023-04-14 10:43:53.000000 gmltools-0.0.60/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.677594 gmltools-0.0.60/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.60/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.60/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.60/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.712541 gmltools-0.0.60/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.60/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.60/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.60/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.60/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.608283 gmltools-0.0.60/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.59/LICENSE` & `gmltools-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/Models.ipynb` & `gmltools-0.0.60/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/PKG-INFO` & `gmltools-0.0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.59
+Version: 0.0.60
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.59/README.md` & `gmltools-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/gmltools.yml` & `gmltools-0.0.60/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/mltools.yml` & `gmltools-0.0.60/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/pyproject.toml` & `gmltools-0.0.60/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.59"
+version = "0.0.60"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.59/setup.py` & `gmltools-0.0.60/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.59',
+    'version': '0.0.60',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.59/src/gmltools/To_Do.txt` & `gmltools-0.0.60/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/eda/eda.py` & `gmltools-0.0.60/src/gmltools/eda/eda.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 import itertools
 from scipy.stats import pearsonr
 import math
 import seaborn as sns
 import matplotlib.pyplot as plt
 warnings.filterwarnings("ignore")
 # from src.decomposition.seasonal import BaseDecomposition
+import stumpy
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+import seaborn as sns
+#import Rectanmgle
+from matplotlib.patches import Rectangle
+import plotly.graph_objects as go
+import plotly.graph_objs as go
+from plotly.subplots import make_subplots
 
 # OUTLIERMANAGER
 # EXPLOREMANAGER
 
 
 # -------------------------------------------------------------------------------------------------OUTLIERS------------------------------------------------------------------------------------------------------------------------------
 class OutlierManager:
@@ -716,7 +726,122 @@
                     sns.pairplot(data=df2, y_vars=y_var, x_vars=x_var, hue=hue,diag_kws=dict(alpha=alpha), plot_kws=dict(alpha=alpha),size=size,aspect=aspect)
 
         else:
              sns.pairplot(data=df2, y_vars=y_var, x_vars=x_var,diag_kws=dict(alpha=alpha), plot_kws=dict(alpha=alpha),size=size,aspect=aspect)
 
         plt.show()
 
+
+
+
+class SimilarPattern:
+    """
+    Class to obtain the similar pattern of a given sequence. The sequence could be 2D or 1D.
+    For 2D the columns are stacked to obtain a 1D sequence, ready to be used by stumpy.
+    """
+    def __init__(self,df, subsequence):
+        if not isinstance(df, pd.DataFrame):
+            df=df.to_frame()
+            
+        self.df = df
+        self.subsequence = subsequence
+        self.y = df.stack().reset_index(drop=True)
+        self.x = df.stack().reset_index(drop=True).index
+        self.m = subsequence*df.columns.size
+        
+    def get_matrix_profile(self):
+        
+        matrix_profile = stumpy.stump(self.y, self.m)
+        self.matrix_profile_df = pd.DataFrame(matrix_profile, columns=['profile', 'profile index', 'left profile index', 'right profile index'])
+        return self.matrix_profile_df
+    
+    def _get_values(self,df,columns,remove_):
+        """
+        Obtains the different values of a dataframe selecting the columns to seek
+        
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Dataframe to obtain the values
+        columns: list
+            Columns to obtain the values
+        Returns
+        -------
+        values: list
+            List of the values of the columns
+        """
+        values=[]
+        for col in columns:
+            values.extend(df[col].unique())
+        values=np.unique(values).tolist()
+        values.remove(remove_)
+        #make an array of int
+        return np.array(values)
+
+    def get_similar_pattern(self,date):
+        """
+        Obtains the similar date pattern to the given date
+        
+        Parameters
+        ----------
+        date: str
+            Date to obtain the similar pattern
+        Returns
+        -------
+        patron: str or tuple
+            Date of the similar pattern
+        """
+        slice_index=self.df.index.get_loc(date)
+        start_index=slice_index.start
+        self.stumpy_index=start_index*self.df.columns.size
+
+        matrix_profile_df=self.get_matrix_profile()
+        matrix_profile_df_=matrix_profile_df[(matrix_profile_df['right profile index'] != -1) & (matrix_profile_df['left profile index'] != -1)]
+        self.seek_motif=matrix_profile_df[matrix_profile_df['profile index'] == self.stumpy_index]
+        close_values=self._get_values(self.seek_motif,['left profile index','right profile index'],self.stumpy_index.item())
+        self.stumpy_close_values=close_values
+        self.close_values=close_values/self.df.columns.size
+        self.close_values=self.close_values.astype(int)
+            
+
+        patron= [self.df.iloc[int(i)].to_frame().T.index[0].strftime('%Y-%m-%d') for i in self.close_values]
+
+        return patron
+    
+    def plot_similar_pattern(self,date):
+        """
+        Plot similar pattern of a given date
+        Parameters
+        ----------
+        date : str
+            Date to plot similar pattern
+        """
+        patron=self.get_similar_pattern(date)
+        self.patron=patron
+        height_adjuts= len(patron)
+        try:
+            patron_profile=[pat + ", " + str(round(self.seek_motif.reset_index().profile.iloc[i],3)) for i, pat in enumerate(patron)]
+        except:
+            
+            patron_profile=patron
+
+        fig = make_subplots(rows=len(patron), cols=1, vertical_spacing=0.1, subplot_titles= patron_profile )
+
+        for i,idx in enumerate(self.stumpy_close_values):
+            plot_y = self.y.iloc[idx:idx.item()+self.m].to_list()
+            plot_base = self.y.iloc[self.stumpy_index:self.stumpy_index+self.m].to_list()
+           
+            fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_y))))), y=plot_y, name=patron[i] ), row=i+1, col=1)
+            fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_base))))), y=plot_base, name=date, line={'color': '#000000'}), row=i+1, col=1)
+            fig.update_yaxes(title_text="Serie {}".format(i+1), row=i+1, col=1)
+
+        #indicate all int x values in the x axis
+            fig.update_xaxes(tickmode = 'array', tickvals = np.linspace(0,self.subsequence-1,self.subsequence), row=i+1, col=1)
+        fig.update_layout(title_text="Patrones similares para {}".format(date), title_x=0.5, height=800+height_adjuts*100)
+        #x name as Hour
+        fig.update_xaxes(title_text="Hour")
+        fig.update_yaxes(title_text="Valor")
+        #tight layout automatically adjusts subplot params so that the subplot(s) fits in to the figure area
+        fig.update_layout(showlegend=True, title_x=0.5, title_font_size=20, title_font_color="black", title_font_family="Arial", title_xanchor="center", title_yanchor="top",
+                          margin=dict(t=100, b=50, l=50, r=50))
+        fig.show()
+
```

### Comparing `gmltools-0.0.59/src/gmltools/models/bayes.py` & `gmltools-0.0.60/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.60/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models/dummy_model.py` & `gmltools-0.0.60/src/gmltools/models/dummy_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if continious:
             continious_preds=pd.concat(pred_list)
             #plot the true and pred col of the dataframe in one plotly
             fig = go.Figure()
             fig.add_trace(go.Scatter(x=continious_preds.index, y=continious_preds["true"], mode="lines", name="True"))
             fig.add_trace(go.Scatter(x=continious_preds.index, y=continious_preds["pred"], mode="lines", name="Predicted"))
 
-            fig.update_layout(title="True vs Predicted Values", xaxis_title="Date", yaxis_title="Value")
+            fig.update_layout(title="Naive True vs Predicted Values", xaxis_title="Date", yaxis_title="Value")
             fig.show()
 
 
         else:
             fig=make_subplots(rows=len(pred_list),cols=1,subplot_titles=self.tscv.get_test_days(self.X),)
             for i,df in enumerate(pred_list):
                 fig.add_trace(go.Scatter(x=df.index, y=df["true"], mode="lines", name="True"), row=i+1, col=1)
```

### Comparing `gmltools-0.0.59/src/gmltools/models/model.py` & `gmltools-0.0.60/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models/models_info.py` & `gmltools-0.0.60/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.60/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.60/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.60/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.60/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.60/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.60/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.59/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.60/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.59
+Version: 0.0.60
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.59/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.60/src/gmltools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Models.ipynb
 PKG-INFO
 README.md
 gmltools.yml
 mltools.yml
 pyproject.toml
 setup.py
+dist/gmltools-0.0.59.tar.gz
 src/gmltools/To_Do.txt
 src/gmltools/__init__.py
 src/gmltools.egg-info/PKG-INFO
 src/gmltools.egg-info/SOURCES.txt
 src/gmltools.egg-info/dependency_links.txt
 src/gmltools.egg-info/requires.txt
 src/gmltools.egg-info/top_level.txt
```

