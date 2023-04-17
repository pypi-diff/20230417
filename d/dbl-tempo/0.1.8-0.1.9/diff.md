# Comparing `tmp/dbl_tempo-0.1.8-py3-none-any.whl.zip` & `tmp/dbl_tempo-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 24044 bytes, number of entries: 10
--rw-r--r--  2.0 unx       59 b- defN 22-Feb-25 14:19 tempo/__init__.py
--rw-r--r--  2.0 unx    14107 b- defN 22-Feb-25 14:19 tempo/interpol.py
--rw-r--r--  2.0 unx     1611 b- defN 22-Feb-25 14:19 tempo/io.py
--rw-r--r--  2.0 unx     6380 b- defN 22-Feb-25 14:19 tempo/resample.py
--rw-r--r--  2.0 unx    42147 b- defN 22-Feb-25 14:19 tempo/tsdf.py
--rw-r--r--  2.0 unx     3129 b- defN 22-Feb-25 14:19 tempo/utils.py
--rw-r--r--  2.0 unx    10974 b- defN 22-Feb-25 14:20 dbl_tempo-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-25 14:20 dbl_tempo-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 22-Feb-25 14:20 dbl_tempo-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      737 b- defN 22-Feb-25 14:20 dbl_tempo-0.1.8.dist-info/RECORD
-10 files, 79242 bytes uncompressed, 22812 bytes compressed:  71.2%
+Zip file size: 24280 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       59 b- defN 22-Feb-25 20:29 tempo/__init__.py
+-rw-r--r--  2.0 unx    14107 b- defN 22-Feb-25 20:29 tempo/interpol.py
+-rw-r--r--  2.0 unx     1611 b- defN 22-Feb-25 20:29 tempo/io.py
+-rw-r--r--  2.0 unx     6380 b- defN 22-Feb-25 20:29 tempo/resample.py
+-rw-r--r--  2.0 unx    42110 b- defN 22-Feb-25 20:29 tempo/tsdf.py
+-rw-r--r--  2.0 unx     3129 b- defN 22-Feb-25 20:29 tempo/utils.py
+-rw-r--r--  2.0 unx    11656 b- defN 22-Feb-25 20:29 dbl_tempo-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Feb-25 20:29 dbl_tempo-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 22-Feb-25 20:29 dbl_tempo-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      737 b- defN 22-Feb-25 20:29 dbl_tempo-0.1.9.dist-info/RECORD
+10 files, 79887 bytes uncompressed, 23048 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tempo/tsdf.py
 Comment: 
 
 Filename: tempo/utils.py
 Comment: 
 
-Filename: dbl_tempo-0.1.8.dist-info/METADATA
+Filename: dbl_tempo-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dbl_tempo-0.1.8.dist-info/WHEEL
+Filename: dbl_tempo-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dbl_tempo-0.1.8.dist-info/top_level.txt
+Filename: dbl_tempo-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dbl_tempo-0.1.8.dist-info/RECORD
+Filename: dbl_tempo-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tempo/tsdf.py

```diff
@@ -619,16 +619,16 @@
 
       # build window
       parsed_freq = rs.checkAllowableFreq(self, freq)
       agg_window = f.window(f.col(self.ts_col), "{} {}".format(parsed_freq[0], rs.freq_dict[parsed_freq[1]]))
 
       # compute column summaries
       selectedCols = []
-      reduce(lambda selectedCols, metric:
-          selectedCols.extend([f.mean(f.col(metric)).alias('mean_' + metric), f.count(f.col(metric)).alias('count_' + metric), f.min(f.col(metric)).alias('min_' + metric), f.max(f.col(metric)).alias('max_' + metric), f.sum(f.col(metric)).alias('sum_' + metric), f.stddev(f.col(metric)).alias('stddev_' + metric)]), metricCols, selectedCols)
+      for metric in metricCols:
+          selectedCols.extend([f.mean(f.col(metric)).alias('mean_' + metric), f.count(f.col(metric)).alias('count_' + metric), f.min(f.col(metric)).alias('min_' + metric), f.max(f.col(metric)).alias('max_' + metric), f.sum(f.col(metric)).alias('sum_' + metric), f.stddev(f.col(metric)).alias('stddev_' + metric)])
 
       selected_df = self.df.groupBy(self.partitionCols + [agg_window]).agg(*selectedCols)
       summary_df = selected_df.select(*selected_df.columns).withColumn(self.ts_col, f.col('window').start).drop('window')
 
       return TSDF(summary_df, self.ts_col, self.partitionCols)
 
   def write(self, spark, tabName, optimizationCols = None):
```

## Comparing `dbl_tempo-0.1.8.dist-info/METADATA` & `dbl_tempo-0.1.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl-tempo
-Version: 0.1.8
+Version: 0.1.9
 Summary: Spark Time Series Utility Package
 Home-page: https://github.com/databrickslabs/tempo
 Author: Ricardo Portilla, Tristan Nixon, Max Thone, Sonali Guleria
 Author-email: labs@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -247,14 +247,30 @@
     method="linear",
     target_cols= ["columnA","columnB"],
     show_interpolated=True,
 )
 
 ```
 
+#### 8 - Grouped Stats by Frequency
+
+Group by partition columns and a frequency to get the minimum, maximum, count, mean, standard deviation, and sum for all or some subset of numeric columns.
+
+###### Parameters: 
+
+`freq` = (required) Frequency at which the grouping should take place - acceptable parameters are strings of the form "1 minute", "40 seconds", etc.
+
+`metricCols` = (optional) List of columns to compute metrics for. These should be numeric columns. If this is not supplied, this method will compute stats on all numeric columns in the TSDF
+
+```python
+grouped_stats = watch_accel_tsdf.withGroupedStats(metricCols = ["y"], freq="1 minute")
+display(grouped_stats)
+```
+
+
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
 
 ## Project Setup
 After cloning the repo, it is highly advised that you create a [virtual environment](https://docs.python.org/3/library/venv.html) to isolate and manage
```

## Comparing `dbl_tempo-0.1.8.dist-info/RECORD` & `dbl_tempo-0.1.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tempo/__init__.py,sha256=FbnUA0pBdr56idOgGnelZGgAWWbF8Nf1XHNIWZ4xrM8,59
 tempo/interpol.py,sha256=hF9V0fIcmL4Zt_q7LadAiVxnf27gLvi817HxEqKu954,14107
 tempo/io.py,sha256=zQd6vSKozbB7QwZXog9UONO3rQX_Q9G4HmwPC8JKDGk,1611
 tempo/resample.py,sha256=_BaKGgX5lcHE4Chxh4hwVaWY7bZMXfcXM7i_y3OMLyU,6380
-tempo/tsdf.py,sha256=YHckrGvNFj-3QiD8tI-Etk-VA9k47eTJrZuPJiYMwqI,42147
+tempo/tsdf.py,sha256=SkkTBYY2g7JiLGWcj9W0k13nnhbv-4b9wo5T8VoVBrg,42110
 tempo/utils.py,sha256=Gn8waM80_hkPhDs4H7IB4EObJ9GOqlzGv96OJQ_dyb8,3129
-dbl_tempo-0.1.8.dist-info/METADATA,sha256=XUSKP58tX0AvdanOxfSl5HWIEKh1BDC8HiPsiFvY-dI,10974
-dbl_tempo-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dbl_tempo-0.1.8.dist-info/top_level.txt,sha256=8u_v6-1uzEEM1eHgHpGZBrZoJ53TGB5NxaOrLNpyD4M,6
-dbl_tempo-0.1.8.dist-info/RECORD,,
+dbl_tempo-0.1.9.dist-info/METADATA,sha256=hMPRkHQutZtqDQ7rnCF3H9_kuNXjcAWJGhoavXcJDmM,11656
+dbl_tempo-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dbl_tempo-0.1.9.dist-info/top_level.txt,sha256=8u_v6-1uzEEM1eHgHpGZBrZoJ53TGB5NxaOrLNpyD4M,6
+dbl_tempo-0.1.9.dist-info/RECORD,,
```

