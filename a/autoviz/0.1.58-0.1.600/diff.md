# Comparing `tmp/autoviz-0.1.58.tar.gz` & `tmp/autoviz-0.1.600.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.58.tar", last modified: Mon Oct  3 01:41:05 2022, max compression
+gzip compressed data, was "autoviz-0.1.600.tar", last modified: Mon Apr 17 00:33:02 2023, max compression
```

## Comparing `autoviz-0.1.58.tar` & `autoviz-0.1.600.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2022-10-03 01:41:05.310674 autoviz-0.1.58/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12961 2022-10-03 01:41:05.293705 autoviz-0.1.58/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11213 2022-10-02 14:24:31.000000 autoviz-0.1.58/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2022-10-03 01:41:05.172535 autoviz-0.1.58/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    28343 2022-10-02 14:52:48.000000 autoviz-0.1.58/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-04-27 11:12:34.000000 autoviz-0.1.58/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-09-06 21:52:25.000000 autoviz-0.1.58/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   106325 2022-10-02 16:56:26.000000 autoviz-0.1.58/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.58/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      403 2022-10-03 01:39:04.000000 autoviz-0.1.58/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24238 2022-10-02 22:52:36.000000 autoviz-0.1.58/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2022-10-03 01:41:05.274462 autoviz-0.1.58/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12961 2022-10-03 01:41:04.000000 autoviz-0.1.58/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2022-10-03 01:41:04.000000 autoviz-0.1.58/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2022-10-03 01:41:04.000000 autoviz-0.1.58/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2022-10-03 01:41:04.000000 autoviz-0.1.58/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2022-10-03 01:41:04.000000 autoviz-0.1.58/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2022-10-03 01:41:05.311688 autoviz-0.1.58/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1204 2022-10-02 22:53:29.000000 autoviz-0.1.58/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.204645 autoviz-0.1.600/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14022 2023-04-17 00:33:02.204645 autoviz-0.1.600/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12210 2023-04-17 00:30:21.000000 autoviz-0.1.600/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.064021 autoviz-0.1.600/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    29545 2023-04-17 00:09:26.000000 autoviz-0.1.600/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   116997 2023-04-17 00:20:44.000000 autoviz-0.1.600/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-04-17 00:23:53.000000 autoviz-0.1.600/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24238 2022-10-02 22:52:36.000000 autoviz-0.1.600/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.173395 autoviz-0.1.600/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14022 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-17 00:33:02.204645 autoviz-0.1.600/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-04-17 00:22:39.000000 autoviz-0.1.600/setup.py
```

### Comparing `autoviz-0.1.58/PKG-INFO` & `autoviz-0.1.600/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,18 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.58
+Version: 0.1.600
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz
         
         Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
         
-        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
-        
-        In order to get this latest function, you must upgrade autoviz to the latest version by:
-        ```
-        pip install autoviz --upgrade
-        ```
-        
-        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
-        
-        ```
-        from autoviz import data_cleaning_suggestions
-        data_cleaning_suggestions(df)
-        ```
-        
-        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
-        
-        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
-        
-        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
-        
-        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
-        
-        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
-        
-        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
-        
-        ![banner](intro2.gif)
-        
         [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
         [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
         [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
@@ -176,14 +137,62 @@
         - `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
         - `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
         - `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
         - `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
         
         ![server_charts](server_charts.JPG)
         
+        ### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
+        From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+        
+        ```
+        AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
+        You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
+        # More info about this function here:
+        # - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
+        # - https://github.com/myrthings/catscatter/blob/master/README.md
+        ```
+        
+        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
+        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
+        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+        
+        In order to get this latest function, you must upgrade autoviz to the latest version by:
+        ```
+        pip install autoviz --upgrade
+        ```
+        
+        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+        
+        ```
+        from autoviz import data_cleaning_suggestions
+        data_cleaning_suggestions(df)
+        ```
+        
+        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
+        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+        
+        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+        
+        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
+        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+        
+        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
+        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+        
+        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
+        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+        
+        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
+        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
+        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
+        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
+        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
+        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+        
         ## Maintainers
         
         * [@AutoViML](https://github.com/AutoViML)
         * [@morenoh149](https://github.com/morenoh149)
         * [@hironroy](https://github.com/hironroy)
         
         ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoviz-0.1.58/README.md` & `autoviz-0.1.600/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,11 @@
 # AutoViz
 
 Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
 
-### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-<img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
-
-In order to get this latest function, you must upgrade autoviz to the latest version by:
-```
-pip install autoviz --upgrade
-```
-
-In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
-
-```
-from autoviz import data_cleaning_suggestions
-data_cleaning_suggestions(df)
-```
-
-### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
-
-<img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
-
-### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
-
-<b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-<b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
-
-You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
-
-### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-- `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-- `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-- `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-<img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
-
-![banner](intro2.gif)
-
 [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
 [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
 [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
 [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
 [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
 [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
@@ -169,14 +130,62 @@
 - `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
 - `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
 - `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
 - `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
 
 ![server_charts](server_charts.JPG)
 
+### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
+From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+
+```
+AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
+You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
+# More info about this function here:
+# - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
+# - https://github.com/myrthings/catscatter/blob/master/README.md
+```
+
+### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
+From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
+<img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+
+In order to get this latest function, you must upgrade autoviz to the latest version by:
+```
+pip install autoviz --upgrade
+```
+
+In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+
+```
+from autoviz import data_cleaning_suggestions
+data_cleaning_suggestions(df)
+```
+
+### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
+AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+
+<img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+
+### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
+We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+
+<b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
+<b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+
+You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
+![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+
+### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
+Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
+- `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
+- `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
+- `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
+<img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+
 ## Maintainers
 
 * [@AutoViML](https://github.com/AutoViML)
 * [@morenoh149](https://github.com/morenoh149)
 * [@hironroy](https://github.com/hironroy)
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoviz-0.1.58/autoviz/AutoViz_Class.py` & `autoviz-0.1.600/autoviz/AutoViz_Class.py`

 * *Files 9% similar despite different names*

```diff
@@ -169,14 +169,21 @@
         self.wordcloud = {
         'name': 'wordcloud',
         'heading': 'Word Cloud Plots of NLP or String vars',
         'plots': [],
         'subheading':[],#"\n".join(subheading)
         'desc': [] #"\n".join(desc)
         }  ######## This is for description and images for date time plots ###
+        self.catscatter_plot = {
+        'name': 'catscatter',
+        'heading': 'Cat-Scatter  Plots of categorical vars',
+        'plots': [],
+        'subheading':[],#"\n".join(subheading)
+        'desc': [] #"\n".join(desc)
+        }  ######## This is for description and images for catscatter plots ###
 
 
     def add_plots(self,plotname,X):
         """
         This is a simple program to append the input chart to the right variable named plotname
         which is an attribute of class AV. So make sure that the plotname var matches an exact
         variable name defined in class AV. Otherwise, this will give an error.
@@ -322,16 +329,17 @@
             try:
                 svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,problem_type,
                                     depVar,classes, mk_dir)
                 self.add_plots('dist_plot',svg_data)
             except:
                 print('Could not draw Distribution Plot')
             try:
-                svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                self.add_plots('violin_plot',svg_data)
+                if len(continuous_vars) > 0:
+                    svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
+                    self.add_plots('violin_plot',svg_data)
             except:
                 print('Could not draw Violin Plot')
             try:
                 #### Since there is no depependent variable in this dataset, you can leave it as-is
                 numeric_cols = dft.select_dtypes(include='number').columns.tolist()
                 numeric_cols = list_difference(numeric_cols, date_vars)
                 svg_data = draw_heatmap(dft, numeric_cols, verbose,chart_format, date_vars, depVar,
@@ -350,15 +358,20 @@
                 try:
                     svg_data = draw_barplots(dft,cats,continuous_vars, problem_type,
                                     verbose,chart_format,depVar,classes, mk_dir)
                     self.add_plots('bar_plot',svg_data)
                 except:
                     print('Could not draw Bar Plots')
             else:
-                print ('No Continuous Variables at all in this dataset...')
+                try:
+                    svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                chart_format, mk_dir=None)
+                    self.add_plots('catscatter_plot',svg_data)
+                except:
+                    print ('Could not draw catscatter plots...')
         else:
             if problem_type=='Regression':
                 ############## This is a Regression Problem #################
                 try:
                     svg_data = draw_scatters(dft,
                                     continuous_vars,verbose,chart_format,problem_type,depVar,classes,lowess, mk_dir)
                     self.add_plots('scatter_plot',svg_data)
@@ -383,16 +396,17 @@
                                             problem_type, depVar, classes, mk_dir)
                         self.add_plots('dist_plot',svg_data)
                     else:
                         print('No continuous var in data set: hence no distribution plots')
                 except:
                     print('Could not draw some Distribution Plots')
                 try:
-                    svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                    self.add_plots('violin_plot',svg_data)
+                    if len(continuous_vars) > 0:
+                        svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
+                        self.add_plots('violin_plot',svg_data)
                 except:
                     print('Could not draw Violin Plots')
                 try:
                     numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if x not in [depVar]]
                     numeric_cols = list_difference(numeric_cols, date_vars)
                     svg_data = draw_heatmap(dft,
                                         numeric_cols, verbose,chart_format, date_vars, depVar,
@@ -404,29 +418,35 @@
                     try:
                         svg_data = draw_date_vars(
                             dft,depVar,date_vars,continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('date_plot',svg_data)
                     except:
                         print('Could not draw some Time Series plots')
                 if len(continuous_vars) > 0:
+
                     try:
-                        svg_data = draw_pivot_tables(dft,find_remove_duplicates(cats+bool_vars),
-                                    continuous_vars,problem_type,verbose,chart_format,depVar,classes, mk_dir)
+                        svg_data = draw_pivot_tables(dft, problem_type, verbose,
+                            chart_format,depVar,classes, mk_dir)
                         self.add_plots('pivot_plot',svg_data)
                     except:
                         print('Could not draw some Pivot Charts against Dependent Variable')
                     try:
-                        svg_data = draw_barplots(dft,cats,continuous_vars,problem_type,verbose,
-                                                    chart_format,depVar,classes, mk_dir)
+                        svg_data = draw_barplots(dft, find_remove_duplicates(cats+bool_vars),continuous_vars,
+                                                    problem_type, verbose,chart_format,depVar,classes, mk_dir)
                         self.add_plots('bar_plot',svg_data)
                         #self.add_plots('bar_plot',None)
                     except:
                         print('Could not draw some Bar Charts')
                 else:
-                    print ('No Continuous Variables at all in this dataset...')
+                    try:
+                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                    chart_format, mk_dir=None)
+                        self.add_plots('catscatter_plot',svg_data)
+                    except:
+                        print ('Could not draw catscatter plots...')
             else :
                 ############ This is a Classification Problem ##################
                 try:
                     svg_data = draw_scatters(dft,continuous_vars,
                                              verbose,chart_format,problem_type,depVar, classes,lowess, mk_dir)
                     self.add_plots('scatter_plot',svg_data)
                 except Exception as e:
@@ -450,16 +470,17 @@
                                                 problem_type,depVar,classes, mk_dir)
                         self.add_plots('dist_plot',svg_data)
                     else:
                         print('No continuous var in data set: hence no distribution plots')
                 except:
                     print('Could not draw some Distribution Plots')
                 try:
-                    svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                    self.add_plots('violin_plot',svg_data)
+                    if len(continuous_vars) > 0:
+                        svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
+                        self.add_plots('violin_plot',svg_data)
                 except:
                     print('Could not draw some Violin Plots')
                 try:
                     numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if x not in [depVar]]
                     numeric_cols = list_difference(numeric_cols, date_vars)
                     svg_data = draw_heatmap(dft, numeric_cols,
                                             verbose,chart_format, date_vars, depVar,problem_type,
@@ -472,30 +493,35 @@
                         svg_data = draw_date_vars(dft,depVar,date_vars,
                                                   continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('date_plot',svg_data)
                     except:
                         print('Could not draw some Time Series plots')
                 if len(continuous_vars) > 0:
                     try:
-                        svg_data = draw_pivot_tables(
-                            dft,find_remove_duplicates(cats+bool_vars),continuous_vars,problem_type,verbose,chart_format,depVar,classes, mk_dir)
+                        svg_data = draw_pivot_tables(dft, problem_type, verbose,
+                                        chart_format,depVar,classes, mk_dir)
                         self.add_plots('pivot_plot',svg_data)
                     except:
                         print('Could not draw some Pivot Charts against Dependent Variable')
                     try:
                         svg_data = draw_barplots(dft,find_remove_duplicates(cats+bool_vars),continuous_vars,problem_type,
                                         verbose,chart_format, depVar, classes, mk_dir)
                         self.add_plots('bar_plot',svg_data)
                         pass
                     except:
                         if verbose <= 1:
                             print('Could not draw some Bar Charts')
                         pass
                 else:
-                    print ('No Continuous Variables at all in this dataset...')
+                    try:
+                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                    chart_format, mk_dir=None)
+                        self.add_plots('catscatter_plot',svg_data)
+                    except:
+                        print ('Could not draw catscatter plots...')
         ###### Now you can check for NLP vars or discrete_string_vars to do wordcloud #######
         if len(discrete_string_vars) > 0:
             plotname = 'wordcloud'
             import nltk
             nltk.download('popular')
             for each_string_var in discrete_string_vars:
                 try:
```

### Comparing `autoviz-0.1.58/autoviz/AutoViz_Holo.py` & `autoviz-0.1.600/autoviz/AutoViz_Holo.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.58/autoviz/AutoViz_NLP.py` & `autoviz-0.1.600/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.58/autoviz/AutoViz_Utils.py` & `autoviz-0.1.600/autoviz/AutoViz_Utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,15 +143,107 @@
         print('''\n################ %s problem #####################''' %model_class)
     return model_class
 #################################################################################
 # Pivot Tables are generally meant for Categorical Variables on the axes
 # and a Numeric Column (typically the Dep Var) as the "Value" aggregated by Sum.
 # Let's do some pivot tables to capture some meaningful insights
 import random
-def draw_pivot_tables(dft,cats,nums,problem_type,verbose,chart_format,depVar='', classes=None, mk_dir=None):
+def draw_pivot_tables(dft, problem_type, verbose, chart_format, depVar='', classes=None, mk_dir=None):
+    #### Finally I have fixed the bugs in pivot tables due to "category" dtypes in data ##############
+    plot_name = 'Bar_Plots_Cats'
+    cats = [i for i in dft.loc[:,dft.nunique()<=15]]
+    dft = copy.deepcopy(dft)
+    cols = 2
+    cmap = plt.get_cmap('jet')
+    #### For some reason, the cmap colors are not working #########################
+    colors = cmap(np.linspace(0, 1, len(cats)))
+    colors = cycle('byrcmgkbyrcmgkbyrcmgkbyrcmgkbyr')
+    #colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
+    colormaps = ['Greys','Blues','Greens','GnBu','PuBu',
+                    'YlGnBu','PuBuGn','BuGn','YlGn']
+    #colormaps = ['Purples','Oranges','Reds','YlOrBr',
+    #                'YlOrRd','OrRd','PuRd','RdPu','BuPu',]
+    N = len(cats)
+    combos = copy.deepcopy(cats)
+    if N==0:
+        print('No categorical or boolean vars in data set. Hence no pivot plots...')
+        return None
+    noplots = copy.deepcopy(N)
+    #### You can set the number of subplots per row and the number of categories to display here cols = 2
+    displaylimit = 20
+    categorylimit = 5
+    imgdata_list = []
+    width_size = 15
+    height_size = 5
+    stringlimit = 20
+    N = len(cats)
+    sns.set_palette("Set1")
+    ###########  This works equally well for classification as well as Regression ###
+    lst=[]
+    noplots=int(len(cats))
+    dicti = {}
+    counter = 1
+    cols = 2
+    ### first make sure there are enough plots to plot #####
+    ######  we want to now figure out rows and columns ####
+    if noplots%cols <= 2:
+        if noplots == 0:
+            rows = 1
+        else:
+            rows = int((noplots/cols)+0.5)
+    else:
+        rows = int((noplots/cols)+0.5)
+    countplots  = len(cats)
+    if N > 0:
+        fig = plt.figure()
+        if cols < 2:
+            fig.set_size_inches(min(15,8),rows*height_size)
+            fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
+            fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+        else:
+            fig.set_size_inches(min(cols*10,20),rows*height_size)
+            fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
+            fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+        ### we start to draw the pivot tables here #########
+        for var1 in combos:
+            #color1 = random.choice(colormaps)
+            color1 = "Set1"
+            data = pd.DataFrame(dicti)
+            x=dft[var1]
+            ax1 = fig.add_subplot(rows,cols,counter)
+            nocats = min(categorylimit,dft[var1].nunique())
+            data = dft[var1].value_counts()
+            if problem_type != 'Binary_Classification' or problem_type != 'Multi_Classification':
+                sns.countplot(x=var1,
+                                data=dft,
+                                ax=ax1,
+                                order=dft[var1].value_counts().index,
+                                hue = depVar)
+            else:
+                sns.countplot(x=var1,
+                                data=dft,
+                                ax=ax1,
+                                order=dft[var1].value_counts().index,)
+            ax1.set_xlabel(var1)
+            ax1.set_xticklabels(dft[var1].value_counts().index, rotation=30, ha='right', fontsize=9)
+            ax1.set_title('Distribution of %s' %var1,fontsize=12)
+            counter += 1
+        fig.tight_layout()
+        fig.suptitle('Distribution of Variables (with <=15 categories)', fontsize=15,y=1.01);
+    image_count = 0
+    if verbose == 2:
+        imgdata_list.append(save_image_data(fig, chart_format,
+                            plot_name, depVar, mk_dir))
+        image_count += 1
+    if verbose <= 1:
+        plt.show();
+    ####### End of Pivot Plotting #############################
+    return imgdata_list
+
+def draw_pivot_tables_old(dft,problem_type,verbose,chart_format,depVar='', classes=None, mk_dir=None):
     #### Finally I have fixed the bugs in pivot tables due to "category" dtypes in data ##############
     plot_name = 'Bar_Plots_Pivots'
     cats = copy.deepcopy(cats)
     cats = list(set(cats))
     dft = copy.deepcopy(dft)
     cols = 2
     cmap = plt.get_cmap('jet')
@@ -341,14 +433,17 @@
         rows = int((noplots/cols)+0.99)
         ### Be very careful with the next line. we have used the singular "subplot" ##
         fig = plt.figure(figsize=(width_size,rows*height_size))
         for num, plotc, color_val in zip(nums, range(1,noplots+1),colors):
             ####Strip plots are meant for categorical plots so x axis must always be depVar ##
             plt.subplot(rows,cols,plotc)
             sns.stripplot(x=dft[dep], y=dft[num], ax=plt.gca(), jitter=jitter)
+            plt.xticks(rotation=30, ha='right', fontsize=9)
+            plt.ylabel(num)
+            plt.xlabel(dep)
         plt.suptitle('Scatter Plot of Continuous Variable vs Target (jitter=%0.2f)' %jitter, fontsize=15,y=1.01)
         fig.tight_layout();
         if verbose <= 1:
             plt.show();
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
                             plot_name, dep, mk_dir))
@@ -516,14 +611,15 @@
                 counter += 1
     if verbose <= 1:
         plt.show()
     if verbose == 2:
         return fig
 ################# The barplots module below calls the plot_fast_average_num_by_cat module above ###
 def draw_barplots(dft,cats,conti,problem_type,verbose,chart_format,dep='', classes=None, mk_dir=None):
+
     cats = cats[:]
     conti = conti[:]
     plot_name = 'Bar_Plots'
     #### Category limit within a variable ###
     #### Remove Floating Point Categorical Vars from this list since they Error when Bar Plots are drawn
     cats = [x for x in cats if dft[x].dtype != float]
     dft = dft[:]
@@ -956,34 +1052,36 @@
                 image_count += 1
     else :
         plot_name = "Box_Plots"
         ###### This is for Classification problems only ##########################
         image_count = 0
         classes = df[dep].factorize()[1].tolist()
         ######################### Add Box plots here ##################################
+        # Styling...
         numb = len(nums)
         target_vars = df[dep].unique()
+        target_len = df[dep].nunique()
         if len(othernums) >= 1:
             width_size = 15
             height_size = 7
             count = 0
             data = pd.DataFrame(index=df.index)
             cols = 2
             noplots = len(nums)
             rows = int((noplots/cols)+0.99 )
             fig = plt.figure(figsize=(width_size,rows*height_size))
             for col in nums:
                 ax = plt.subplot(rows,cols,count+1)
-                for targetvar in target_vars:
-                    data[targetvar] = np.nan
-                    mask = df[dep]==targetvar
-                    data.loc[mask,targetvar] = df.loc[mask,col]
-                ax = sns.boxplot(data=data, orient='v', fliersize=5, ax=ax,
-                        linewidth=3, notch=False, saturation=0.5, showfliers=False)
+                sns.boxplot(x=dep,
+                    y=col,
+                    data=df,
+                    ax=ax,
+                    linewidth=3, notch=False, saturation=0.5, showfliers=False)
                 ax.set_title('%s for each %s' %(col,dep))
+                ax.set_xticklabels(df[dep].value_counts().index, rotation=30, ha='right', fontsize=9)
                 count += 1
             fig.suptitle('Box Plots without Outliers shown',  fontsize=15)
             fig.tight_layout();
             if verbose <= 1:
                 plt.show();
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
@@ -1116,16 +1214,150 @@
             fig = plot_fast_average_num_by_cat(df_target, datevars, num_vars, verbose,kind="line")
         fig.suptitle('Time Series Plot by %s: Continuous Variables Pair' %ts_column, fontsize=15, y=1.01)
     if verbose == 2:
         imgdata_list.append(save_image_data(fig, chart_format,
                         plot_name, dep, mk_dir))
         image_count += 1
     return imgdata_list
-    ############# End of Date vars plotting #########################
+############# End of Date vars plotting #########################
+def catscatter(data,colx,coly, ax, ratio=10,save=False,save_name='Default'):
+    """
+    ####################################################################################
+    # The catscatter idea was conceived by: Myr Barnés in 2020 
+    # This idea is reused and modified here in AutoViz with sincere thanks to Myr Barnés.
+    ####################################################################################
+    The function draws catscatter plots for pairs of categorical variables in a data frame. 
+    A catscatter plot is a type of scatter plot that shows the frequency of each combination 
+    of categories in two variables. It can be useful for exploring the relationship between 
+    categorical variables and identifying patterns or outliers.
+    """
+    length = 7
+    # aggregate record counts by different labels of cat_x and cat_y
+    df = data.groupby([colx, coly]).size().reset_index(name='record_count')
+    top_xticks = df[colx].value_counts().index[:length]
+    top_yticks = df[coly].value_counts().index[:length]
+    df = df[(df[colx].isin(top_xticks)) & (df[coly].isin(top_yticks))].reset_index(drop=True)
+    cols = 'record_count'
+    # define the color map
+    color=['red', 'green', 'grey']
+    font_size = 7
+    font='Helvetica'
+    # Create a dict to encode the categeories into numbers (sorted)
+    xticks = df[colx].sort_values().unique().tolist()
+    yticks = df[coly].sort_values().unique().tolist()
+    
+    colx_codes=dict(zip(xticks,range(len(xticks))))
+    coly_codes=dict(zip(yticks,range(len(yticks))))
+    
+    # Apply the encoding
+    df[colx]=df[colx].apply(lambda x: colx_codes[x])
+    df[coly]=df[coly].apply(lambda x: coly_codes[x])
+    
+    # Prepare the aspect of the plot
+    #plt.rcParams['xtick.bottom'] = plt.rcParams['xtick.labelbottom'] = False
+    #plt.rcParams['xtick.top'] = plt.rcParams['xtick.labeltop'] = True
+    plt.rcParams['font.family'] = 'sans-serif'
+    plt.rcParams['font.sans-serif'] = [font] + plt.rcParams['font.sans-serif']
+    plt.rcParams['xtick.color']=color[-1]
+    plt.rcParams['ytick.color']=color[-1]
+    plt.box(False)
+
+    plt.tick_params(
+        axis='x',          # changes apply to the x-axis
+        which='both',      # both major and minor ticks are affected
+        bottom=True,      # ticks along the bottom edge are off
+        top=False,         # ticks along the top edge are off
+        labelbottom=True) # labels along the bottom edge are off
+
+    plt.tick_params(
+        axis='y',          # changes apply to the y-axis
+        which='major',      # both major and minor ticks are affected
+        left=False,      # ticks along the bottom edge are off
+        right=False,         # ticks along the top edge are off
+        ) # labels along the bottom edge are off
+
+    # Plot all the lines for the background
+    for num in range(len(top_yticks)):
+        ax.hlines(num,-1,len(top_xticks),linestyle='dashed',linewidth=1,color=color[num%2],alpha=0.5)
+    for num in range(len(top_xticks)):
+        ax.vlines(num,-1,len(top_yticks),linestyle='dashed',linewidth=1,color=color[num%2],alpha=0.5)
+        
+    
+    ax.set_xticklabels(['']+xticks[:length], rotation=15, ha='right', color=color[-1])
+    ax.set_xticks(range(-1,len(xticks)))
+    ax.set_yticklabels(['']+yticks[:length], rotation=15, ha='left', color=color[-1])
+    ax.set_yticks(range(-1,len(yticks)+1))
+
+    # Plot the scatter plot with the numbers
+    ax.scatter(df[colx],
+               df[coly],
+               s=df[cols]*ratio,
+               zorder=1,
+               color=color[-1],
+               )
+    ax.set_xlim(xmin=-1,xmax=len(colx_codes))
+    ax.set_ylim(ymin=-1,ymax=len(coly_codes))
+    return ax
+############################################################################
+def draw_catscatterplots(dft,cats, problem_type, verbose, 
+                chart_format, mk_dir=None):
+    """
+    The function draws catscatter plots for pairs of categorical variables in a data frame. 
+    A catscatter plot is a type of scatter plot that shows the frequency of each combination 
+    of categories in two variables. It can be useful for exploring the relationship between 
+    categorical variables and identifying patterns or outliers.
+    Args:
+        dft (pandas.DataFrame): The data frame containing the categorical variables.
+        cats (list): A list of column names of the categorical variables in dft.
+        problem_type (str): The type of problem to be solved, either 'classification' or 'regression'.
+        verbose (int): The level of verbosity for displaying the plots. 0 means no plots, 1 means show plots, 2 means save plots as image files.
+        chart_format (str): The format of the image files to be saved. Can be 'png', 'jpg', 'svg', etc.
+        mk_dir (str, optional): The directory where the image files will be saved. Defaults to None.
+
+    Returns:
+        list: A list of image data objects for each catscatter plot if verbose == 2, otherwise an empty list.
+    """
+    imgdata_list = list()
+    image_count = 0
+    N = len(cats)
+    chunksize = 20
+    if len(cats) == 0:
+        #### If there are no categorical variables, nothing to plot here ######
+        return imgdata_list
+    else:
+        width_size = 15
+        height_size = 5
+    #### start drawing the catscatter here ###
+    cols = 2
+    gap=0.5
+    image_count = 0
+    combos = combinations(cats, 2)
+    combs = copy.deepcopy(combos)
+    noplots = int((N**2-N)/2)
+    rows = int((noplots/cols)+0.99)
+    counter = 1
+    fig = plt.figure(figsize=(width_size,rows*height_size))
+    fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
+    for (var1,var2) in combs:
+        try:
+            plt.subplot(rows,cols,counter)
+            ax1 = plt.gca()
+            catscatter(dft, var1, var2, ax1, ratio=10)
+            ax1.set_title('Catscatter plot for '+var1 + '(X axis) vs. '+var2, fontsize=10)
+            counter += 1
+        except:
+            plt.close('all')
+    fig.suptitle('Catscatter plot of Pairs of Categorical Variables', fontsize=15, y=1.01)
+    if verbose == 2:
+        imgdata_list.append(save_image_data(fig, chart_format,
+                        plot_name, dep, mk_dir))
+        image_count += 1
+    return imgdata_list
 
+######################################################################################
 # This little function classifies columns into 4 types: categorical, continuous, boolean and
 # certain columns that have only one value repeated that they are useless and must be removed from dataset
 #Subtract RIGHT_LIST from LEFT_LIST to produce a new list
 ### This program is USED VERY HEAVILY so be careful about changing it
 def list_difference(l1,l2):
     lst = []
     for i in l1:
@@ -1451,17 +1683,17 @@
     categorical_vars = var_df['cat_vars'] + var_df['factor_vars'] + int_vars + bool_vars
     date_vars = var_df['date_vars']
     
     if len(var_df['continuous_vars'])==0 and len(int_vars)>0:
         continuous_vars = var_df['int_vars']
         categorical_vars = list_difference(categorical_vars, int_vars)
         int_vars = []
-    elif len(var_df['continuous_vars'])==0 and len(int_vars)==0:
-        print('Cannot visualize this dataset since no numeric or integer vars in data...returning')
-        return dataname
+    #elif len(var_df['continuous_vars'])==0 and len(int_vars)==0:
+    #    print('Cannot visualize this dataset since no numeric or integer vars in data...returning')
+    #    return dataname
     else:
         continuous_vars = var_df['continuous_vars']
     #### from now you can use wordclouds on discrete_string_vars ######################
     preds = [x for x in orig_preds if x not in IDcols+cols_delete]
     if len(IDcols+cols_delete) == 0:
         print('        No variables removed since no ID or low-information variables found in data set')
     else:
@@ -1525,16 +1757,16 @@
                                             preds), max_cols_analyzed))
             important_features,num_vars, _ = find_top_features_xgb(dft,preds,continuous_vars,
                                                          depVar,problem_type,corr_limit,verbose)
             if len(important_features) >= max_cols_analyzed:
                 print('    Since number of features selected is greater than max columns analyzed, limiting to %d variables' %max_cols_analyzed)
                 important_features = important_features[:max_cols_analyzed]
             dft = dft[important_features+[depVar]]
-            #### Time to  classify the important columns again ###
-            var_df = classify_columns(dft[important_features], verbose)
+            #### Time to  classify the important columns again. Set verbose to zero so you don't print it again ###
+            var_df = classify_columns(dft[important_features], verbose=0)
             IDcols = var_df['id_vars']
             discrete_string_vars = var_df['nlp_vars']+var_df['discrete_string_vars']
             cols_delete = var_df['cols_delete']
             bool_vars = var_df['string_bool_vars'] + var_df['num_bool_vars']
             int_vars = var_df['int_vars']
             categorical_vars = var_df['cat_vars'] + var_df['factor_vars'] + int_vars + bool_vars
             if len(var_df['continuous_vars'])==0 and len(int_vars)>0:
@@ -1555,18 +1787,18 @@
             dft = dft[preds+[depVar]]
         else:
             continuous_vars = continuous_vars[:max_cols_analyzed]
             print('%d numeric variables in data exceeds limit, taking top %d variables' %(len(
                                             continuous_vars), max_cols_analyzed))
             if verbose >= 1:
                 print('    List of variables selected: %s' %(continuous_vars[:max_cols_analyzed]))
-    elif len(continuous_vars) < 1:
-        print('No continuous variables in this data set. No visualization can be performed')
-        ### Return data frame as is #####
-        return dfte
+    #elif len(continuous_vars) < 1:
+    #    print('No continuous variables in this data set. No visualization can be performed')
+    #    ### Return data frame as is #####
+    #    return dfte
     else:
         #########     If above 1 but below limit, leave features as it is   ######################
         if not isinstance(depVar, list):
             if depVar != '':
                 dft = dft[preds+[depVar]]
         else:
             dft = dft[preds+depVar]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoviz-0.1.58/autoviz/__init__.py` & `autoviz-0.1.600/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.58/autoviz/classify_method.py` & `autoviz-0.1.600/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.58/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.600/autoviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,18 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.58
+Version: 0.1.600
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz
         
         Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
         
-        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
-        
-        In order to get this latest function, you must upgrade autoviz to the latest version by:
-        ```
-        pip install autoviz --upgrade
-        ```
-        
-        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
-        
-        ```
-        from autoviz import data_cleaning_suggestions
-        data_cleaning_suggestions(df)
-        ```
-        
-        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
-        
-        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
-        
-        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
-        
-        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
-        
-        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
-        
-        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
-        
-        ![banner](intro2.gif)
-        
         [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
         [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
         [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
@@ -176,14 +137,62 @@
         - `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
         - `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
         - `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
         - `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
         
         ![server_charts](server_charts.JPG)
         
+        ### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
+        From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+        
+        ```
+        AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
+        You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
+        # More info about this function here:
+        # - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
+        # - https://github.com/myrthings/catscatter/blob/master/README.md
+        ```
+        
+        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
+        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
+        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+        
+        In order to get this latest function, you must upgrade autoviz to the latest version by:
+        ```
+        pip install autoviz --upgrade
+        ```
+        
+        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+        
+        ```
+        from autoviz import data_cleaning_suggestions
+        data_cleaning_suggestions(df)
+        ```
+        
+        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
+        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+        
+        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+        
+        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
+        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+        
+        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
+        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+        
+        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
+        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+        
+        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
+        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
+        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
+        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
+        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
+        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+        
         ## Maintainers
         
         * [@AutoViML](https://github.com/AutoViML)
         * [@morenoh149](https://github.com/morenoh149)
         * [@hironroy](https://github.com/hironroy)
         
         ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoviz-0.1.58/setup.py` & `autoviz-0.1.600/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.58",
+    version="0.1.600",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
@@ -28,15 +28,15 @@
         "scikit-learn",
         "statsmodels",
         "nltk",
         "textblob",
         "holoviews>=1.14.6",
         "bokeh>=2.4.2",
         "hvplot>=0.7.3",
-        "panel~=0.12.6",
+        "panel>=0.12.6",
         "xgboost>=0.82",
         "fsspec>=0.8.3",
         "typing-extensions>=4.1.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

