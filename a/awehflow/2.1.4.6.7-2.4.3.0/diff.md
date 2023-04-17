# Comparing `tmp/awehflow-2.1.4.6.7.tar.gz` & `tmp/awehflow-2.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awehflow-2.1.4.6.7.tar", last modified: Mon Apr 17 09:08:31 2023, max compression
+gzip compressed data, was "dist/awehflow-2.4.3.0.tar", last modified: Fri Mar 10 09:10:01 2023, max compression
```

## Comparing `awehflow-2.1.4.6.7.tar` & `awehflow-2.4.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8474 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8027 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow/alerts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/alerts/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/alerts/googlechat.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/alerts/slack.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/config.py
--rw-rw-rw-   0 root         (0) root         (0)    12283 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/events/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/events/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/events/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow/operators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5996 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/etl.py
--rw-rw-rw-   0 root         (0) root         (0)     3049 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/flow.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)    10526 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/gcs.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7053 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/operators/taxonomy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/sensors/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/sensors/sql_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/awehflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8474 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/awehflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 09:08:31.000000 awehflow-2.1.4.6.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-17 09:07:34.000000 awehflow-2.1.4.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/googlechat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/alerts/slack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/events/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/operators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/etl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8454 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/gcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7215 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/operators/taxonomy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/sensors/sql_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/awehflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      778 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/awehflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 09:10:01.000000 awehflow-2.4.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2023-03-10 09:09:43.000000 awehflow-2.4.3.0/setup.py
```

### Comparing `awehflow-2.1.4.6.7/LICENSE` & `awehflow-2.4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/PKG-INFO` & `awehflow-2.4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awehflow
-Version: 2.1.4.6.7
+Version: 2.4.3.0
 Summary: Configuration based Apache Airflow
 Home-page: UNKNOWN
 Author: Philip Perold
 Author-email: philip@spatialedge.co.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `awehflow-2.1.4.6.7/README.md` & `awehflow-2.4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/alerts/googlechat.py` & `awehflow-2.4.3.0/awehflow/alerts/googlechat.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/alerts/slack.py` & `awehflow-2.4.3.0/awehflow/alerts/slack.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/config.py` & `awehflow-2.4.3.0/awehflow/config.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/core.py` & `awehflow-2.4.3.0/awehflow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,20 @@
             'email_on_retry': False,
             'retries': 0,
             'on_failure_callback': self.generate_on_failure_callback(config, event_handlers)
         }, config.get('default_dag_args'))
 
         dag = DAG(dag_id=config.get('dag_id'), # type: ignore
             description=config.get('description'),
-            schedule_interval=config.get('schedule'),
+            schedule=config.get('schedule'),
             catchup=config.get('catchup', False),
             template_searchpath=self.configs_path,
             user_defined_macros=self.generate_user_defined_macros(config),
             default_args=default_dag_args,
-            concurrency=config.get('dag_concurrency', airflow_config.getint('core', 'dag_concurrency')),
+            max_active_tasks=config.get('max_active_tasks_per_dag', airflow_config.getint('core', 'max_active_tasks_per_dag')),
             max_active_runs=config.get('max_active_runs_per_dag', airflow_config.getint('core', 'max_active_runs_per_dag')),
             dagrun_timeout=config.get('dagrun_timeout', None),
             doc_md=config.get('doc_md', None),
             access_control=config.get('access_control', None),
             is_paused_upon_creation=config.get('is_paused_upon_creation', None),
             tags=config.get('tags', None))
```

### Comparing `awehflow-2.1.4.6.7/awehflow/events/base.py` & `awehflow-2.4.3.0/awehflow/events/base.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/events/gcp.py` & `awehflow-2.4.3.0/awehflow/events/gcp.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/events/postgres.py` & `awehflow-2.4.3.0/awehflow/events/postgres.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/etl.py` & `awehflow-2.4.3.0/awehflow/operators/etl.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/flow.py` & `awehflow-2.4.3.0/awehflow/operators/flow.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/gcp.py` & `awehflow-2.4.3.0/awehflow/operators/gcp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 from airflow.providers.google.cloud.operators.bigquery import BigQueryExecuteQueryOperator
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
 from airflow.models.skipmixin import SkipMixin
 from airflow.utils.decorators import apply_defaults
 
@@ -31,43 +33,17 @@
                 location=self.location,
                 impersonation_chain=self.impersonation_chain,
             )
             credential_email = self.hook._get_credentials_email()
             self.log.info(f"Created BigQueryHook with account: {credential_email}")
 
         if self.cleanup_query:
-            if self.destination_dataset_table == None:
-                raise ValueError('No destination_dataset_table was given, set a destination_dataset_table in the following format: project_id.dataset_id.table_id')
-            
-            replaced_destination_dataset_table = self.destination_dataset_table.replace(':', '.')
-            split_destination_dataset_table = replaced_destination_dataset_table.split(".")
-
-            if len(split_destination_dataset_table) != 3:
-                raise ValueError('Please set a destination_dataset_table in the following format: project_id.dataset_id.table_id')
-        
-            project_id = split_destination_dataset_table[0]
-            dataset_id = split_destination_dataset_table[1]
-            table_id = split_destination_dataset_table[2]
-            
-            self.log.info('Checking if table exist: {}.{}.{}'.format(project_id, dataset_id, table_id))
-            
-            if self.hook.table_exists(project_id=project_id, dataset_id=dataset_id, table_id=table_id):
-                self.log.info('Table exists')
-
-                self.log.info('Executing cleanup query: {}'.format(self.cleanup_query))
-                cleanup_job_id = self.hook.run_query(sql=self.cleanup_query)
-            
-                qj = self.hook.get_job(job_id=cleanup_job_id)
-                while not qj.done():
-                    self.log.info(f'Waiting for job [{cleanup_job_id}] to complete...')
-                    time.sleep(1)
-
-                self.log.info('Completed execution of cleanup query')   
-            else:
-                self.log.info('Table does not exist, cleanup query was not executed') 
+            self.log.info('Executing cleanup query: {}'.format(self.cleanup_query))
+            self.hook.run(sql=self.cleanup_query)
+            self.log.info('Completed execution of cleanup query')
 
         if isinstance(self.sql, str):
             self.sql = [self.sql]
         
         job_id = []
         if isinstance(self.sql, Iterable):
             for s in self.sql:
@@ -109,29 +85,29 @@
     """
 
     @apply_defaults
     def __init__(
             self,
             task_ids: list=[],
             xcom_key: str='return_value',
-            bigquery_conn_id: str='bigquery_default',
-            gcp_conn_id: str=None, # type: ignore
+            bigquery_conn_id: str=None,
+            gcp_conn_id: str='google_cloud_default',
             *args, **kwargs):
         """
         :param task_ids: List of task_ids saying which tasks to sink their job_metrics for
         :param xcom_key: XCOM key used to pull the bigquery job id from the specified tasks
         """
         self.task_ids = task_ids
         self.xcom_key = xcom_key
-        self.gcp_conn_id = bigquery_conn_id
-        if gcp_conn_id:
-            self.gcp_conn_id = gcp_conn_id
+        self.gcp_conn_id = gcp_conn_id
+        if bigquery_conn_id:
+            self.gcp_conn_id = bigquery_conn_id
 
         super(BigQueryJobTaskMetricOperator, self).__init__(*args, **kwargs)
-        
+
 
     def execute(self, context):
         hook = BigQueryHook(
             gcp_conn_id=self.gcp_conn_id
         )
         credential_email = hook._get_credentials_email()
         self.log.info(f"Created BigQueryHook with account: {credential_email}")
@@ -173,25 +149,25 @@
     template_fields = ('sql',)
     template_ext = ('.sql',)
 
     @apply_defaults
     def __init__(
             self,
             sql: str,
-            bigquery_conn_id: str='bigquery_default',
-            gcp_conn_id: str=None, # type: ignore
+            gcp_conn_id: str='google_cloud_default',
+            bigquery_conn_id: str=None,
             use_legacy_sql: bool=True,
             *args, **kwargs):
         
         self.sql = sql
-        self.gcp_conn_id = bigquery_conn_id
-        if gcp_conn_id:
-            self.gcp_conn_id = gcp_conn_id
-
+        self.gcp_conn_id = gcp_conn_id
+        if bigquery_conn_id:
+            self.gcp_conn_id = bigquery_conn_id
         self.use_legacy_sql = use_legacy_sql
+
         super(BigQueryShortCircuitOperator, self).__init__(*args, **kwargs)
 
 
     def execute(self, context):
         records = self.db_hook.get_first(self.sql)
         success = records and all([bool(r) for r in records])
 
@@ -210,7 +186,38 @@
 
     @property
     def db_hook(self):
         hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id, use_legacy_sql=self.use_legacy_sql)
         credential_email = hook._get_credentials_email()
         self.log.info(f"Created BigQueryHook with account: {credential_email}")
         return hook
+
+
+class BigQueryPushFirstResultToXComOperator(BaseOperator):
+    template_fields = ('sql',)
+
+    @apply_defaults
+    def __init__(
+            self,
+            sql,
+            gcp_conn_id: str='gcp_default',
+            bigquery_conn_id: Optional[str] = None,
+            use_legacy_sql=True,
+            *args, **kwargs):
+        """
+        :param sql: Source table name that has been materialized (:project_id.:dataset_id.:table_name)
+        :param use_legacy_sql: Whether to execute the query in legacy SQL mode or not
+        """
+        if bigquery_conn_id:
+            gcp_conn_id = bigquery_conn_id
+
+        super(BigQueryPushFirstResultToXComOperator, self).__init__(*args, **kwargs)
+        self.sql = sql
+        self.use_legacy_sql = use_legacy_sql
+        self.gcp_conn_id = gcp_conn_id
+
+    def execute(self, context):
+        hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id, use_legacy_sql=self.use_legacy_sql)
+        result = hook.get_first(self.sql)
+        if not result:
+            raise Exception("No materialized date found")
+        return result
```

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/gcs.py` & `awehflow-2.4.3.0/awehflow/operators/gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                  temp_dataset_name: str,
                  print_header: bool = True,
                  field_delimiter: str = ',',
                  bigquery_conn_id: str = 'bigquery_default',
                  gcp_conn_id: str = 'gcp_conn_id',
                  location=None,
                  *args, **kwargs) -> None:
+
         """
         Create an instance of the BigQueryCSVExtractAndComposeOperator
         :param source_dataset_table: The source BigQuery table to extract, including the data set and table name ie. dev_temp.some_table_to_extract
         :param destination_object_name: The destination filename as a bucket URI ie gs://dev_extract_data/some_sub_folder/my_extract.csv
         :param temp_bucket_name: The temporary bucket area where files can be extracted and composed
         :param temp_dataset_name: A temp dataset where temporary tables can be created and saved, while processing
         :param print_header: Whether or not the extracted data should contain a header or not
```

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/metrics.py` & `awehflow-2.4.3.0/awehflow/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/operators/taxonomy.py` & `awehflow-2.4.3.0/awehflow/operators/taxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
 from airflow.utils.decorators import apply_defaults
 from airflow.operators.python import PythonVirtualenvOperator
 
-def set_policy_tag(project_id, dataset_id, table_names, policy_tags, bigquery_conn_id, testing=False):
+def set_policy_tag(project_id, dataset_id, table_names, policy_tags, gcp_conn_id, testing=False):
     from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 
     from google.api_core.exceptions import NotFound
     from google.cloud import bigquery
     from google.cloud.bigquery import schema
 
     import logging
@@ -79,23 +80,23 @@
                                                     policy_tags=schema.PolicyTagList((get_pii_tag(column, policy_tags),))))
             else:
                 logging.debug(f'Not modifying column: {column.name}')
                 new_schema.append(column)
 
         return new_schema
 
-    def update_policy_tag(project_id: str, dataset_id: str, table_names: list, policy_tags: dict, bigquery_conn_id: str): #pragma: no cover
+    def update_policy_tag(project_id: str, dataset_id: str, table_names: list, policy_tags: dict, gcp_conn_id: str): #pragma: no cover
         hook = BigQueryHook(
-            gcp_conn_id=bigquery_conn_id,
+            gcp_conn_id=gcp_conn_id,
             use_legacy_sql=False
         )
         credential_email = hook._get_credentials_email()
         logging.info(f"Created BigQueryHook with account: {credential_email}")
 
-        client = bigquery.Client(project=project_id, credentials=hook._get_credentials())
+        client = hook.get_client()
 
         if isinstance(table_names, str):
             table_names = [table_names]
 
         if not isinstance(table_names, list):
             raise ValueError(f'table_names should be of type str or list, not of type {type(table_names)}')
 
@@ -119,15 +120,15 @@
             'get_pii_tag': get_pii_tag,
             'get_pii_description': get_pii_description,
             '_schema_builder': _schema_builder,
             'update_policy_tag': update_policy_tag
             
         }
 
-    update_policy_tag(project_id, dataset_id, table_names, policy_tags, bigquery_conn_id) #pragma: no cover
+    update_policy_tag(project_id, dataset_id, table_names, policy_tags, gcp_conn_id) #pragma: no cover
     
 class ApplyTaxonomyOperator(PythonVirtualenvOperator): #pragma: no cover
     # """
     # Adds policy tags to columns in a BigQuery Table.
 
     # param project_id: The name of the project that the BigQuery table is in.
     # type project_id: str
@@ -136,28 +137,38 @@
     # param table_name: The table name that the policy tags should be applied to.
     # type table_name: str
     # param policy_tags: The policy tags that needs to be applied to the table.
     # type policy_tags: dict
     
     # """
     @apply_defaults
-    def __init__(self, task_id: str, project_id: str, dataset_id: str, table_names: list, 
+    def __init__(
+            self, 
+            task_id: str, 
+            project_id: str, 
+            dataset_id: str, 
+            table_names: list, 
             policy_tags: dict,
-            bigquery_conn_id: str, *args, **kwargs):
+            gcp_conn_id: str='gcp_default',
+            bigquery_conn_id: Optional[str] = None,
+            *args, **kwargs):
+        
+        if bigquery_conn_id:
+            gcp_conn_id = bigquery_conn_id
 
         super(ApplyTaxonomyOperator, self).__init__(
             task_id=task_id,
             python_callable=set_policy_tag,
             requirements=["google-cloud-bigquery==2.13.1"],
             system_site_packages=True,
             op_kwargs={
                 'project_id': project_id,
                 'dataset_id': dataset_id,
                 'table_names': table_names,
                 'policy_tags': policy_tags,
-                'bigquery_conn_id': bigquery_conn_id,
+                'gcp_conn_id': gcp_conn_id,
             },
             *args, **kwargs
         )
 
 class TaxonomyException(Exception):
     pass
```

### Comparing `awehflow-2.1.4.6.7/awehflow/sensors/http.py` & `awehflow-2.4.3.0/awehflow/sensors/http.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow/sensors/sql_sensor.py` & `awehflow-2.4.3.0/awehflow/sensors/sql_sensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import sleep
 from datetime import timedelta
 from airflow.utils import timezone
 
 from airflow.models.taskreschedule import TaskReschedule
 from airflow.exceptions import AirflowSensorTimeout, AirflowSkipException, AirflowRescheduleException
-from airflow.sensors.sql import SqlSensor
+from airflow.providers.common.sql.sensors.sql import SqlSensor
 
 class SqlSensor(SqlSensor):
     """
     Override of the default SqlSensor with modified 'execute' logic.  Sensor now fails quitely in soft_fail mode
     """
     def execute(self, context):
         started_at = timezone.utcnow()
```

### Comparing `awehflow-2.1.4.6.7/awehflow/utils.py` & `awehflow-2.4.3.0/awehflow/utils.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/awehflow.egg-info/PKG-INFO` & `awehflow-2.4.3.0/awehflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awehflow
-Version: 2.1.4.6.7
+Version: 2.4.3.0
 Summary: Configuration based Apache Airflow
 Home-page: UNKNOWN
 Author: Philip Perold
 Author-email: philip@spatialedge.co.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `awehflow-2.1.4.6.7/awehflow.egg-info/SOURCES.txt` & `awehflow-2.4.3.0/awehflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awehflow-2.1.4.6.7/setup.py` & `awehflow-2.4.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 with open('requirements.txt') as req:
     requirements = list(filter(None, [x if 'github.com' not in x else None for x in req.read().split('\n')]))
 
 EXCLUDE_FROM_PACKAGES = ['docs', 'tests*']
 
 EXTRAS_REQUIREMENTS = {
     'default': [
-        'apache-airflow==2.1.4'
+        'apache-airflow==1.10.9'
     ],
     'composer': [
-        'apache-airflow==2.1.4+composer'
+        'apache-airflow==1.10.9-composer'
     ]
 }
 
 setuptools.setup(
     name="awehflow",
     version=version.strip('v'),
     author="Philip Perold",
```

