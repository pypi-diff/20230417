# Comparing `tmp/trawler-on-lake-1.0.8.tar.gz` & `tmp/trawler-on-lake-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trawler-on-lake-1.0.8.tar", last modified: Thu Feb  2 12:31:11 2023, max compression
+gzip compressed data, was "trawler-on-lake-1.0.9.tar", last modified: Sun Feb  5 13:47:58 2023, max compression
```

## Comparing `trawler-on-lake-1.0.8.tar` & `trawler-on-lake-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-02 12:31:11.580824 trawler-on-lake-1.0.8/
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/LICENSE
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/MANIFEST.in
--rw-r--r--   0 pierre     (501) staff       (20)      208 2023-02-02 12:31:11.580474 trawler-on-lake-1.0.8/PKG-INFO
--rw-r--r--   0 pierre     (501) staff       (20)       62 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/README.md
--rw-r--r--   0 pierre     (501) staff       (20)      824 2023-02-02 12:30:57.000000 trawler-on-lake-1.0.8/pyproject.toml
--rw-r--r--   0 pierre     (501) staff       (20)       38 2023-02-02 12:31:11.580940 trawler-on-lake-1.0.8/setup.cfg
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-02 12:31:11.575901 trawler-on-lake-1.0.8/src/
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-02 12:31:11.578579 trawler-on-lake-1.0.8/src/common/
--rw-r--r--   0 pierre     (501) staff       (20)      183 2023-02-02 12:30:57.000000 trawler-on-lake-1.0.8/src/common/__init__.py
--rw-r--r--   0 pierre     (501) staff       (20)    12462 2023-02-02 12:30:46.000000 trawler-on-lake-1.0.8/src/common/common.py
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/src/common/common_udfs.py
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/src/common/datalake_helper.py
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.8/src/common/datamart_helper.py
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-02 12:31:11.580113 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/
--rw-r--r--   0 pierre     (501) staff       (20)      208 2023-02-02 12:31:11.000000 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/PKG-INFO
--rw-r--r--   0 pierre     (501) staff       (20)      388 2023-02-02 12:31:11.000000 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/SOURCES.txt
--rw-r--r--   0 pierre     (501) staff       (20)        1 2023-02-02 12:31:11.000000 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/dependency_links.txt
--rw-r--r--   0 pierre     (501) staff       (20)       86 2023-02-02 12:31:11.000000 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/requires.txt
--rw-r--r--   0 pierre     (501) staff       (20)        7 2023-02-02 12:31:11.000000 trawler-on-lake-1.0.8/src/trawler_on_lake.egg-info/top_level.txt
+drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-05 13:47:58.950759 trawler-on-lake-1.0.9/
+-rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/LICENSE
+-rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/MANIFEST.in
+-rw-r--r--   0 pierre     (501) staff       (20)      208 2023-02-05 13:47:58.950386 trawler-on-lake-1.0.9/PKG-INFO
+-rw-r--r--   0 pierre     (501) staff       (20)       62 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/README.md
+-rw-r--r--   0 pierre     (501) staff       (20)      824 2023-02-05 13:47:44.000000 trawler-on-lake-1.0.9/pyproject.toml
+-rw-r--r--   0 pierre     (501) staff       (20)       38 2023-02-05 13:47:58.950886 trawler-on-lake-1.0.9/setup.cfg
+drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-05 13:47:58.946155 trawler-on-lake-1.0.9/src/
+drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-05 13:47:58.948557 trawler-on-lake-1.0.9/src/common/
+-rw-r--r--   0 pierre     (501) staff       (20)      183 2023-02-05 13:47:44.000000 trawler-on-lake-1.0.9/src/common/__init__.py
+-rw-r--r--   0 pierre     (501) staff       (20)    12699 2023-02-05 13:43:57.000000 trawler-on-lake-1.0.9/src/common/common.py
+-rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/src/common/common_udfs.py
+-rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/src/common/datalake_helper.py
+-rw-r--r--   0 pierre     (501) staff       (20)        0 2023-02-01 16:39:21.000000 trawler-on-lake-1.0.9/src/common/datamart_helper.py
+drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-02-05 13:47:58.950012 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/
+-rw-r--r--   0 pierre     (501) staff       (20)      208 2023-02-05 13:47:58.000000 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/PKG-INFO
+-rw-r--r--   0 pierre     (501) staff       (20)      388 2023-02-05 13:47:58.000000 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre     (501) staff       (20)        1 2023-02-05 13:47:58.000000 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre     (501) staff       (20)       86 2023-02-05 13:47:58.000000 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/requires.txt
+-rw-r--r--   0 pierre     (501) staff       (20)        7 2023-02-05 13:47:58.000000 trawler-on-lake-1.0.9/src/trawler_on_lake.egg-info/top_level.txt
```

### Comparing `trawler-on-lake-1.0.8/pyproject.toml` & `trawler-on-lake-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trawler-on-lake"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
     "pyspark",
     "confluent-kafka",
     "requests",
     "delta-spark==2.1.1",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.7"
 
 [tool.bumpver]
-current_version = "1.0.8"
+current_version = "1.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `trawler-on-lake-1.0.8/src/common/common.py` & `trawler-on-lake-1.0.9/src/common/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,24 +73,30 @@
     if output_conf.get('processing_time') is not None:
         stream \
             .writeStream \
             .format("kafka") \
             .options(**output_conf['kafka_options']) \
             .trigger(processingTime=output_conf['processing_time']) \
             .outputMode("append") \
-            .start() \
-            .awaitTermination()
+            .start()
+    elif output_conf.get('availableNow') is not None:
+        stream \
+            .writeStream \
+            .format("kafka") \
+            .options(**output_conf['kafka_options']) \
+            .trigger(availableNow=output_conf['availableNow']) \
+            .outputMode("append") \
+            .start()
     else:
         stream \
             .writeStream \
             .format("kafka") \
             .options(**output_conf['kafka_options']) \
             .outputMode("append") \
-            .start() \
-            .awaitTermination()
+            .start()
 
 
 ######
 # S3 #
 ######
 def read_s3_xxx(spark_session: SparkSession, spark_job_conf: dict, source_path: str):
     source_conf = get_spark_conf(source_path, spark_job_conf['sources'])
@@ -153,15 +159,14 @@
         .format("delta")
         .mode(output_conf['delta_options']['mode'])
         .partitionBy(output_conf['delta_options']['partition_columns'])
         .option("checkpointLocation", output_conf['delta_options']['checkpoint_location'])
         .save(output_conf['delta_options']['location'])
     )
 
-
 def write_delta_no_partitioning(spark_job_conf: dict, output_name: str, df: DataFrame):
     output_conf = get_spark_conf(output_name, spark_job_conf['outputs'])
     create_delta_tables_if_not_exists(output_conf, output_conf['delta_options']['schema'])
     (
         df
         .write
         .format("delta")
```

