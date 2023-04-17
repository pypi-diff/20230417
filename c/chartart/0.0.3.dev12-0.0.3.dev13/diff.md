# Comparing `tmp/chartart-0.0.3.dev12.tar.gz` & `tmp/chartart-0.0.3.dev13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev12.tar", last modified: Thu Feb  9 19:50:02 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev13.tar", last modified: Mon Apr 17 16:26:34 2023, max compression
```

## Comparing `chartart-0.0.3.dev12.tar` & `chartart-0.0.3.dev13.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.185815 chartart-0.0.3.dev12/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     1639 2023-02-09 19:50:02.186070 chartart-0.0.3.dev12/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1117 2022-09-29 12:39:34.000000 chartart-0.0.3.dev12/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-02-09 19:50:02.187498 chartart-0.0.3.dev12/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.157734 chartart-0.0.3.dev12/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.171801 chartart-0.0.3.dev12/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    78534 2023-02-09 19:36:07.000000 chartart-0.0.3.dev12/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.182853 chartart-0.0.3.dev12/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.181010 chartart-0.0.3.dev12/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1639 2023-02-09 19:50:02.000000 chartart-0.0.3.dev12/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-02-09 19:50:02.000000 chartart-0.0.3.dev12/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-02-09 19:50:02.000000 chartart-0.0.3.dev12/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-02-09 19:50:02.000000 chartart-0.0.3.dev12/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-02-09 19:50:02.000000 chartart-0.0.3.dev12/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-02-09 19:50:02.184890 chartart-0.0.3.dev12/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2022-09-13 20:00:53.000000 chartart-0.0.3.dev12/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.770334 chartart-0.0.3.dev13/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2028 2023-04-17 16:26:34.770618 chartart-0.0.3.dev13/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1506 2023-04-17 16:25:20.000000 chartart-0.0.3.dev13/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-04-17 16:26:34.771817 chartart-0.0.3.dev13/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.747812 chartart-0.0.3.dev13/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.758934 chartart-0.0.3.dev13/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    79147 2023-04-17 16:12:16.000000 chartart-0.0.3.dev13/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.767892 chartart-0.0.3.dev13/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.765736 chartart-0.0.3.dev13/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2028 2023-04-17 16:26:34.000000 chartart-0.0.3.dev13/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-04-17 16:26:34.000000 chartart-0.0.3.dev13/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-04-17 16:26:34.000000 chartart-0.0.3.dev13/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-04-17 16:26:34.000000 chartart-0.0.3.dev13/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-04-17 16:26:34.000000 chartart-0.0.3.dev13/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 16:26:34.768889 chartart-0.0.3.dev13/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev13/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev12/LICENSE` & `chartart-0.0.3.dev13/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/PKG-INFO` & `chartart-0.0.3.dev13/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev12
+Version: 0.0.3.dev13
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -58,7 +58,13 @@
 -Added Exception handling code if response is not in json format
 
 0.0.3.dev7 => 0.0.3.dev8
 -Added code to retry 5xx error code 
 
 0.0.3.dev7 => 0.0.3.dev10
 -Resolved unauthorized error and changed sleep time
+
+0.0.3.dev12 => 0.0.3.dev13
+- Added line/bar/scatter chart subtypes
+- line type : line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
+- bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
+- scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
```

### Comparing `chartart-0.0.3.dev12/README.md` & `chartart-0.0.3.dev13/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -41,8 +41,14 @@
 0.0.3.dev6 => 0.0.3.dev7
 -Added Exception handling code if response is not in json format
 
 0.0.3.dev7 => 0.0.3.dev8
 -Added code to retry 5xx error code 
 
 0.0.3.dev7 => 0.0.3.dev10
--Resolved unauthorized error and changed sleep time
+-Resolved unauthorized error and changed sleep time
+
+0.0.3.dev12 => 0.0.3.dev13
+- Added line/bar/scatter chart subtypes
+- line type : line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
+- bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
+- scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
```

### Comparing `chartart-0.0.3.dev12/setup.cfg` & `chartart-0.0.3.dev13/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev12
+version = 0.0.3.dev13
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev12/src/chartart/__init__.py` & `chartart-0.0.3.dev13/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/src/chartart/conftest.py` & `chartart-0.0.3.dev13/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/src/chartart/helpers.py` & `chartart-0.0.3.dev13/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/src/chartart/plot.py` & `chartart-0.0.3.dev13/src/chartart/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,27 +377,28 @@
 
     def get_chartIds(self):
         return [{'type':'chart','id':self.chart_id}]
 
 
     def line(self, x: Union[str, list, np.ndarray, pd.Series], y: Union[str, list, np.ndarray, pd.Series],
              data: Optional[pd.DataFrame] = None, c: Optional[str] = None, ls: str = '-', lw: float = 1.0,
-             labels: Union[Optional[str], Optional[list]] = None, animationDelay: Optional[float] = None, 
+             type:Optional[str]='line', labels: Union[Optional[str], Optional[list]] = None, animationDelay: Optional[float] = None, 
              animationDuration: Optional[float]=None, animationType: Optional[str]='parallel'):
         """
         Constructs a line plot.
 
         :param x: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param y: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
         ['g', 'green', 'b', 'blue', 'r', 'red', 'c', 'cyan', 'm', 'magenta', 'y', 'yellow', 'k', 'black',
         'w', 'white'] to be used to colour the line(s).
         :param ls: A string specifying line style which can be one of ['-', '--', '.-'].
         :param lw: A float specifying line width.
+        :param type: type of line chart possible values are line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
         :param labels: A string or list of strings specifying labels of each line.
         :return:
         """
         self.check_input_data_validity(x, y, data)
         self.axes_type = 'line'
         if animationType == 'sequential':
             current_fig_type: str = 'lineRace'
@@ -432,15 +433,15 @@
             # - Line types
             # - Line widths
             line_colour: str = line_colours[i % self.len_default_colour_map]
             line_label: str = self.get_ax_label('line', str(grp_id), labels[i])
             self.modify_axis_labels(x, y)
 
             line_info: dict = {
-                'type': 'line',
+                'type': type,
                 'xData': x_data,
                 'yData': y_data,
                 'color': line_colour,
                 'lineStyle': ls,
                 'lineWidth': lw,
                 'name': line_label,
             }
@@ -717,27 +718,27 @@
                 'start': x,
                 'end': x,
                 'text': label
             }
         })
 
     def scatter(self, x: Union[str, list, np.ndarray, pd.Series], y: Union[str, list, np.ndarray, pd.Series],
-                data: Optional[pd.DataFrame] = None, c: Optional[str] = None, size: float = 1.0, marker: str = 'o',
+                data: Optional[pd.DataFrame] = None, c: Optional[str] = None, size: Union[float, list] = 1.0, marker: str = 'o',
                 alpha: float = 1.0, labels: Union[Optional[str], Optional[list]] = None,animationDelay: Optional[float] = None, 
                 animationDuration: Optional[float]=None, animationType: Optional[str]='parallel'):
         """
         Constructs a scatter plot.
 
         :param x: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param y: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
         ['g', 'green', 'b', 'blue', 'r', 'red', 'c', 'cyan', 'm', 'magenta', 'y', 'yellow', 'k', 'black',
         'w', 'white'] to be used to colour the points.
-        :param size: A float specifying the point size.
+        :param size: A float specifying the point size. if not specified its 1.0. If list of size specified it will be ploted as bubble chart
         :param marker: A string specifying the point shape which can be one of ['o', '*'].
         :param alpha: A float between 0 and 1 denoting opacity of points.
         :param labels: A string or list of strings specifying labels of each point.
         :return:
         """
         self.check_input_data_validity(x, y, data)
         self.axes_type = 'scatter'
@@ -775,16 +776,20 @@
             # - Point types
             # - Point sizes
             point_colour: str = point_colours[i % self.len_default_colour_map]
             point_label: str = self.get_ax_label(
                 'point', str(grp_id), labels[i])
             self.modify_axis_labels(x, y)
 
+            type = 'scatter'
+            if isinstance(size, list):
+                type = 'bubble'
+
             point_info: dict = {
-                'type': 'scatter',
+                'type': type,
                 'xData': x_data,
                 'yData': y_data,
                 'color': point_colour,
                 'size': size,
                 'marker': marker,
                 'alpha': alpha,
                 'name': point_label,
@@ -797,26 +802,28 @@
 
             self.data.insert(point_info)
 
             i += 1
 
     def bar(self, x: Union[str, list, np.ndarray, pd.Series, pd.Index],
             height: Union[str, list, np.ndarray, pd.Series], data: Optional[pd.DataFrame] = None, c: str = None,
-            labels: Optional[list] = None,barType:Optional[str]='vertical' ,animationDelay: Optional[float] = None, 
+            labels: Optional[list] = None,barType:Optional[str]='vertical', type:Optional[str]='column', animationDelay: Optional[float] = None, 
              animationDuration: Optional[float] = None, animationType: Optional[str]='parallel', animationRollingWindow: Optional[int] = None):
         """
         Constructs a bar chart.
 
         :param x: A list, NumPy array, Pandas series, Pandas index, or column name of `data` to plot bars for.
         :param height: A list, NumPy array, Pandas series, or column name of `data` denoting height of each bar.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
         ['g', 'green', 'b', 'blue', 'r', 'red', 'c', 'cyan', 'm', 'magenta', 'y', 'yellow', 'k', 'black',
         'w', 'white'] to be used to colour the bars.
         :param labels: A string or list of strings specifying labels of each bar.
+        :param barType: This is legacy parameter just for matplot or plotly friendly terminology users. Use type parameter wherever possible.
+        :param type: type of chart allowed values are bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
         :param animationDelay: wait before starting animation. applicable if animationType == parallel
         :param animationDuration: total time to animate entire series
         :param animationType: parallel or sequential, dapapoints will get printed accordingly.
         :param animationRollingWindow: rolling window for animation, applicable only if animationType == sequential
         :return:
         """
         self.check_not_datetime(x[0])
@@ -852,20 +859,18 @@
                 grp_df.loc[:, _y].values, data)
             self.y_axis_type = y_axis_type
             # TODO: Add support for custom:
             # - Colour maps
             bar_colour: str = bar_colours[i]
             bar_label: str = self.get_ax_label('bar', str(grp_id), labels[i])
             self.modify_axis_labels(x, height)
-            if barType == 'vertical':
-                barType = 'column'
-            elif barType == 'horizontal':
-                barType = 'bar'
+            if barType == 'horizontal':
+                type = 'bar'
             bar_info: dict = {
-                'type': barType,
+                'type': type,
                 'xData': x_data,
                 'yData': y_data,
                 'color': bar_colour,
                 'name': bar_label,
             }
 
             if animationDelay is not None:
```

### Comparing `chartart-0.0.3.dev12/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev13/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/src/chartart/test_plot.py` & `chartart-0.0.3.dev13/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev12/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev13/src/chartart.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev12
+Version: 0.0.3.dev13
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -58,7 +58,13 @@
 -Added Exception handling code if response is not in json format
 
 0.0.3.dev7 => 0.0.3.dev8
 -Added code to retry 5xx error code 
 
 0.0.3.dev7 => 0.0.3.dev10
 -Resolved unauthorized error and changed sleep time
+
+0.0.3.dev12 => 0.0.3.dev13
+- Added line/bar/scatter chart subtypes
+- line type : line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
+- bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
+- scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
```

