# Comparing `tmp/apache-airflow-providers-fastetl-0.0.7.tar.gz` & `tmp/apache-airflow-providers-fastetl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-fastetl-0.0.7.tar", last modified: Mon Apr 17 19:37:26 2023, max compression
+gzip compressed data, was "apache-airflow-providers-fastetl-0.0.8.tar", last modified: Mon Apr 17 20:32:38 2023, max compression
```

## Comparing `apache-airflow-providers-fastetl-0.0.7.tar` & `apache-airflow-providers-fastetl-0.0.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.296119 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 19:37:26.000000 apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.296119 apache-airflow-providers-fastetl-0.0.7/fastetl/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/copy_db_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/fast_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/patchwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/samba_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/encode_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/get_table_cols_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/load_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/load_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/string_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/table_comments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/bacen_STA_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/ckan_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/dadosgovbr_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/db_to_db_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/dou_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/gsheet_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/osrm_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/datapackage_to_datadictionary_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/db_to_csv_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/gsheet_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/fastetl/operators/osrm_distance_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:37:26.304118 apache-airflow-providers-fastetl-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:37:26.300119 apache-airflow-providers-fastetl-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/tests/test_db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/tests/test_odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 19:37:08.000000 apache-airflow-providers-fastetl-0.0.7/tests/test_osrm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/fastetl/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/copy_db_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/fast_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/patchwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/samba_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/encode_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/get_table_cols_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/string_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/table_comments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/bacen_STA_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/ckan_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dadosgovbr_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/db_to_db_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dou_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/gsheet_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/osrm_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/datapackage_to_datadictionary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_csv_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/gsheet_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/osrm_distance_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_osrm.py
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/LICENSE` & `apache-airflow-providers-fastetl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.7
+Version: 0.0.8
 Summary: FastETL custom package Apache Airflow provider.
+Home-page: https://github.com/economiagovbr/FastETL
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -66,14 +67,17 @@
 ```
 
 To see an example of an Apache Airflow container that uses FastETL,
 check out the
 [airflow2-docker](https://github.com/economiagovbr/airflow2-docker)
 repository.
 
+To ensure appropriate results, please make sure to install the
+`msodbcsql17` and `unixodbc-dev` libraries on your Apache Airflow workers.
+
 # Tests
 
 The test suite uses Docker containers to simulate a complete use
 environment, including Airflow and the databases. For that reason, to
 execute the tests, you first need to install Docker and docker-compose.
 
 For people using Ubuntu 20.04, you can just type on the terminal:
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/README.md` & `apache-airflow-providers-fastetl-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 ```
 
 To see an example of an Apache Airflow container that uses FastETL,
 check out the
 [airflow2-docker](https://github.com/economiagovbr/airflow2-docker)
 repository.
 
+To ensure appropriate results, please make sure to install the
+`msodbcsql17` and `unixodbc-dev` libraries on your Apache Airflow workers.
+
 # Tests
 
 The test suite uses Docker containers to simulate a complete use
 environment, including Airflow and the databases. For that reason, to
 execute the tests, you first need to install Docker and docker-compose.
 
 For people using Ubuntu 20.04, you can just type on the terminal:
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.7
+Version: 0.0.8
 Summary: FastETL custom package Apache Airflow provider.
+Home-page: https://github.com/economiagovbr/FastETL
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -66,14 +67,17 @@
 ```
 
 To see an example of an Apache Airflow container that uses FastETL,
 check out the
 [airflow2-docker](https://github.com/economiagovbr/airflow2-docker)
 repository.
 
+To ensure appropriate results, please make sure to install the
+`msodbcsql17` and `unixodbc-dev` libraries on your Apache Airflow workers.
+
 # Tests
 
 The test suite uses Docker containers to simulate a complete use
 environment, including Airflow and the databases. For that reason, to
 execute the tests, you first need to install Docker and docker-compose.
 
 For people using Ubuntu 20.04, you can just type on the terminal:
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/apache_airflow_providers_fastetl.egg-info/SOURCES.txt` & `apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/__init__.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/copy_db_extensions.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/copy_db_extensions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/fast_etl.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/fast_etl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Thanks to Jedi Wash! *.*
 """
-Módulo cópia de dados entre Postgres e MsSql e outras coisas
+Copy tabular data between Postgres, MSSQL and MySQL.
 """
 
 import time
 from datetime import datetime, date
 import re
 from typing import Union, Tuple, Dict
 import logging
@@ -30,27 +30,29 @@
 from fastetl.custom_functions.utils.table_comments import TableComments
 from fastetl.custom_functions.utils.get_table_cols_name import (
     get_table_cols_name,
 )
 
 
 class SourceConnection:
-    """
-    Represents a source connection to a database, encapsulating the connection details
-    (e.g., connection ID, schema, table, query) required to read data from a database.
+    """Represents a source connection to a database, encapsulating the
+    connection details (e.g., connection ID, schema, table, query)
+    required to read data from a database.
 
     Args:
         conn_id (str): The unique identifier of the connection to use.
-        schema (str, optional): The name of the schema to use. Default is None.
-        table (str, optional): The name of the table to use. Default is None.
+        schema (str, optional): The name of the schema to use.
+            Default is None.
+        table (str, optional): The name of the table to use.
+            Default is None.
         query (str, optional): The SQL query to use. Default is None.
 
     Raises:
-        ValueError: If `conn_id` is empty or if neither `query` nor (`schema` and `table`)
-            is provided.
+        ValueError: If `conn_id` is empty or if neither `query` nor
+            (`schema` and `table`) is provided.
 
     Attributes:
         conn_id (str): The unique identifier of the connection.
         schema (str): The name of the schema.
         table (str): The name of the table.
         query (str): The SQL query.
     """
@@ -67,17 +69,17 @@
         self.conn_id = conn_id
         self.schema = schema
         self.table = table
         self.query = query
 
 
 class DestinationConnection:
-    """
-    Represents a destination connection to a database, encapsulating the connection details
-    (e.g., connection ID, schema, table) required to write data to a database.
+    """Represents a destination connection to a database, encapsulating
+    the connection details (e.g., connection ID, schema, table) required
+    to write data to a database.
 
     Args:
         conn_id (str): The unique identifier of the connection to use.
         schema (str): The name of the schema to use.
         table (str): The name of the table to use.
 
     Attributes:
@@ -90,31 +92,38 @@
 
         self.conn_id = conn_id
         self.schema = schema
         self.table = table
 
 
 def build_select_sql(schema: str, table: str, column_list: str) -> str:
-    """
-    Monta a string do select da origem
-    """
+    """Generates sql `select` query based on schema, table and columns."""
 
     columns = ", ".join(f'"{col}"' for col in column_list)
 
     return f"SELECT {columns} FROM {schema}.{table}"
 
 
 def build_dest_sqls(
     destination: DestinationConnection, column_list: str, wildcard_symbol: str
-) -> Union[str, str, str]:
-    """
-    Monta a string do insert do destino
-    Monta a string de truncate do destino
+) -> Union[str, str]:
+    """Generates sql `insert` and `truncate` queries.
+
+    Args:
+        destination (DestinationConnection): Object with connection
+            details as schema and table.
+        column_list (str): Columns names to be inserted on destination.
+        wildcard_symbol (str): Db symbol for insert statement.
+            E.g.: ? for mssql or %s to postgres
+
+    Returns:
+        Union[str, str]: `insert` and `truncate` sql queries.
     """
 
+
     columns = ", ".join(f'"{col}"' for col in column_list)
 
     values = ", ".join([wildcard_symbol for i in range(len(column_list))])
     insert = (
         f"INSERT INTO {destination.schema}.{destination.table} ({columns}) "
         f"VALUES ({values})"
     )
@@ -127,20 +136,20 @@
 def insert_df_to_db(
     df: pd.DataFrame,
     conn_id: str,
     schema: str,
     table: str,
     reflect_col_table: bool = True,
 ):
-    """
-    Insere os registros do DataFrame df na tabela especificada. Insere
-    apenas as colunas que existem na tabela.
+    """Inserts the records from the DataFrame df into the specified
+    table. Inserts only the columns that exist in the table.
 
-    TODO: Implementar aqui o registro no LOG CONTROLE
+    TODO: Register operation on `log control`.
     """
+
     if reflect_col_table:
         # Filter existing table columns
         cols = get_table_cols_name(conn_id=conn_id, schema=schema, table=table)
         cols = [col.lower() for col in cols]
         df.columns = df.columns.str.lower()
         df = df[cols]
 
@@ -154,16 +163,15 @@
 
 
 def create_table_if_not_exists(
     source: SourceConnection,
     destination: DestinationConnection,
     copy_table_comments: bool,
 ) -> None:
-    """
-    Creates a destination table if it does not already exist and copies
+    """Creates a destination table if it does not already exist and copies
     data from a source table to the destination.
 
     Args:
         source (SourceConnection): A `SourceConnection` object containing
             the connection details for the source database.
         destination (DestinationConnection): A `DestinationConnection`
             object containing the connection details for the destination
@@ -224,19 +232,18 @@
     except (DatabaseError, OperationalError, NoSuchModuleError) as db_error:
         if not ERROR_TABLE_DOES_NOT_EXIST[destination_provider] in str(db_error):
             raise db_error
         # Table does not exist so we create it
         source_eng.echo = True
         try:
             insp = reflection.Inspector.from_engine(source_eng)
-        except AssertionError as e:
+        except AssertionError as e: # pylint: disable=invalid-name
             logging.error(
-                "Não é possível criar tabela automaticamente "
-                "a partir deste banco de dados. Crie a tabela "
-                "manualmente para executar a cópia dos dados. "
+                "Cannot create the table automatically from this database."
+                "Please create the table manually to execute data copying."
             )
             raise e
 
         generic_columns = insp.get_columns(source.table, source.schema)
         dest_columns = [
             _convert_column(c, destination_provider) for c in generic_columns
         ]
@@ -257,16 +264,15 @@
             destination=destination,
         )
 
 
 def _copy_table_comments(
     source: SourceConnection, destination: DestinationConnection
 ) -> None:
-    """
-    Copy table and column comments/descriptions between databases.
+    """Copy table and column comments/descriptions between databases.
 
     Args:
         source (SourceConnection): Connection object containing the
             source database information.
         destination (DestinationConnection): Connection object
             containing the destination database information.
 
@@ -289,16 +295,15 @@
 
 def save_load_info(
     source: SourceConnection,
     destination: DestinationConnection,
     load_type: str,
     rows_loaded: int,
 ):
-    """
-    Inserts metadata information into a database about a data ingestion
+    """Inserts metadata information into a database about a data ingestion
     process, including the origin of the data, the type of ingestion
     (full or incremental), the destination database, the schema where
     the control data will be stored, and the number of rows loaded.
 
     Args:
         source (SourceConnection): Object with connection info to the
             source database (conn_id, schema, table).
@@ -319,62 +324,65 @@
         dest_conn_id=destination.conn_id,
         log_schema_name=destination.schema,
     )
 
     load_info.save(rows_loaded)
 
 
-def get_schema_table_from_query(query: str) -> str:
-    """Returns schema.table from a query statement.
+def get_schema_table_from_query(query: str) -> Union[str, str]:
+    """Returns schema and table from a sql query string statement.
 
     Args:
         query (str): sql query statement.
 
     Returns:
-        schema_table (str): table string in format `schema.table`
+        schema, table (Union[str, str]): schema and table strings.
     """
 
     # search pattern "from schema.table" on query
     sintax_from = re.search(
         r"from\s+\"?\'?\[?[\w|\.|\"|\'|\]|\]]*\"?\'?\]?", query, re.IGNORECASE
     ).group()
-    # split "from " from "schema.table" and get schema.table [-1]
+    # split "from " from "schema.table" and get schema.table[-1]
     db_schema_table = sintax_from.split()[-1]
-    # clean [, ], ", '
+    # clean `[`, `]`, `"`, `'`
     db_schema_table = re.sub(r"\[|\]|\"|\'", "", db_schema_table)
-    # clean "dbo." if exists on dbo.schema.table
+    # clean "dbo." if exists as dbo.schema.table
     schema, table = db_schema_table.split(".")[-2:]
 
     return schema, table
 
 
 def copy_db_to_db(
     source: Dict[str, str],
     destination: Dict[str, str],
     columns_to_ignore: list = None,
     destination_truncate: bool = True,
     chunksize: int = 1000,
     copy_table_comments: bool = False,
     load_type: str = "full",
 ) -> None:
-    """
-    Carrega dado do Postgres/MSSQL/MySQL para Postgres/MSSQL com psycopg2 e pyodbc
-    copiando todas as colunas e linhas já existentes na tabela de destino.
-    Tabela de destino deve ter a mesma estrutura e nome de tabela e colunas
-    que a tabela de origem, ou passar um select_sql que tenha as colunas de
-    destino.
-
-    Alguns tipos de dados utilizados na tabela destino podem gerar
-    problemas na cópia. Esta lista consolida os casos conhecidos:
-    * **float**: mude para **numeric(x,y)** ou **decimal(x,y)**
-    * **text**: mude para **varchar(max)** ou **nvarchar**
-    * para datas: utilize **date** para apenas datas, **datetime** para
-    data com hora, e **datetime2** para timestamp
+    """Load data from Postgres/MSSQL/MySQL to Postgres/MSSQL using psycopg2
+    and pyodbc copying all existing columns and rows in the destination
+    table.
+
+    The destination table:
+        * can be created if not exists
+        * must have matching `ddl` with source table column names
+        * can be loaded with provided query on the source table
+
+    Some data types used in the destination table may cause problems
+    in copying.
+    This list consolidates known cases:
+    * **float**: change to **numeric(x,y)** or **decimal(x,y)**
+    * **text**: change to **varchar(max)** or **nvarchar**
+    * for dates: use **date** for only dates, **datetime** for
+    date with time, and **datetime2** for timestamp
 
-    Exemplo:
+    Example:
         copy_db_to_db(
             {"conn_id": "conn_id", "schema": "schema", "table: "table"},
             {"conn_id": "conn_id", "schema": "schema", "table: "table"}
         )
 
     Args:
         source (Dict[str, str]): A dictionary containing connection
@@ -409,21 +417,14 @@
             source table will be copied to the destination table.
             Defaults to False.
         load_type (str, optional): The type of load to perform. Can be
             "full" or "incremental". Defaults to "full".
 
     Return:
         None
-
-    Todo:
-        * Transformar em Classe ou em Airflow Operator
-        * Criar tabela no destino quando não existente
-        * Alterar conexão do Postgres para pyodbc
-        * Possibilitar inserir data da carga na tabela de destino
-        * Criar testes
     """
 
     # validate connections
     source = SourceConnection(**source)
     destination = DestinationConnection(**destination)
 
     # create table if not exists in destination db
@@ -445,15 +446,15 @@
                     if destination_provider == "mssql":
                         destination_conn.autocommit = False
                         destination_cur.fast_executemany = True
                         wildcard_symbol = "?"
                     else:
                         wildcard_symbol = "%s"
 
-                    # gera queries
+                    # generate queries
                     col_list = get_table_cols_name(
                         conn_id=destination.conn_id,
                         schema=destination.schema,
                         table=destination.table,
                         columns_to_ignore=columns_to_ignore,
                     )
 
@@ -465,40 +466,40 @@
                     else:
                         select_sql = build_select_sql(
                             schema=source.schema,
                             table=source.table,
                             column_list=col_list,
                         )
 
-                    # Remove as aspas na query para compatibilidade com o MYSQL
+                    # remove quotes for mysql compatibility
                     if source_provider == "mysql":
                         select_sql = select_sql.replace('"', "")
 
-                    # truncate stg
+                    # truncate stage
                     if destination_truncate:
                         destination_cur.execute(truncate)
                         if destination_provider == "mssql":
                             destination_cur.commit()
 
                     # download data
                     start_time = time.perf_counter()
                     source_cur.execute(select_sql)
                     rows = source_cur.fetchmany(chunksize)
                     rows_inserted = 0
 
                     logging.info(
-                        "Inserindo linhas na tabela [%s].[%s]",
+                        "Loading rows on table [%s].[%s]",
                         destination.schema,
                         destination.table,
                     )
                     while rows:
                         destination_cur.executemany(insert, rows)
                         rows_inserted += len(rows)
                         rows = source_cur.fetchmany(chunksize)
-                        logging.info("%d linhas inseridas!!", rows_inserted)
+                        logging.info("%d rows loaded!!", rows_inserted)
 
                     destination_conn.commit()
 
                     delta_time = time.perf_counter() - start_time
 
                     if source.query:
                         source.schema, source.table = get_schema_table_from_query(
@@ -508,23 +509,22 @@
                     save_load_info(
                         source=source,
                         destination=destination,
                         load_type=load_type,
                         rows_loaded=rows_inserted,
                     )
 
-                    logging.info("Tempo load: %f segundos", delta_time)
-                    logging.info("Linhas inseridas: %d", rows_inserted)
-                    logging.info("linhas/segundo: %f", rows_inserted / delta_time)
+                    logging.info("Load time: %f seconds", delta_time)
+                    logging.info("Rows insertes: %d", rows_inserted)
+                    logging.info("lines by second: %f", rows_inserted / delta_time)
 
 
 def _table_rows_count(db_hook, table: str, where_condition: str = None):
-    """
-    Calcula a quantidade de linhas na tabela (table) e utiliza a
-    condição (where_condition) caso seja passada como parâmetro.
+    """Calculates the number of rows in the table and uses the condition
+    (where_condition) if passed as a parameter.
     """
 
     sql = f"SELECT COUNT(*) FROM {table}"
     sql += f" WHERE {where_condition};" if where_condition is not None else ";"
 
     return db_hook.get_first(sql)[0]
 
@@ -532,56 +532,54 @@
 def _build_filter_condition(
     dest_hook: MsSqlHook,
     table: str,
     date_column: str,
     key_column: str,
     since_datetime: datetime = None,
 ) -> Tuple[str, str]:
-    """
-    Monta o filtro (where) obtenção o valor max() da tabela,
-    distinguindo se a coluna é a "data ou data/hora de atualização"
-    (date_column) ou outro número sequencial (key_column), por exemplo
-    id, pk, etc. Se o parâmetro "since_datetime" for recebido, será
-    considerado em vez do valor max() da tabela.
+    """Builds the filter (where) by obtaining the max() value from the table,
+    distinguishing whether the column is the "date or update datetime"
+    (date_column) or another sequential number (key_column). For example,
+    id, pk, etc. If the "since_datetime" parameter is provided, it will
+    be considered instead of the max() value from the table.
 
-    Exemplo:
-        _build_filter_condition(dest_hook: hook,
+    Example:
+        _build_filter_condition(dest_hook=dest_hook,
                         table=table,
                         date_column=date_column,
                         key_column=key_column)
 
     Args:
-        dest_hook (str): hook de conexão do DB de destino
-        table (str): tabela a ser sincronizada
-        date_column (str): nome da coluna a ser utilizado para
-            identificação dos registros atualizados.
-        key_column (str): nome da coluna a ser utilizado como chave na
-            etapa de atualização dos registros antigos que sofreram
-            atualizações na origem.
-        since_datetime (datetime): data/hora a partir do qual o filtro será
-            montado, em vez de usar o max() da tabela.
-
-        Returns:
-                Tuple[str, str]: Tupla contendo o valor máximo e a condição
-                        where da query sql.
+        dest_hook (str): destination database connection hook.
+        table (str): table to be synchronized.
+        date_column (str): name of the column to be used for
+            identification of updated records.
+        key_column (str): name of the column to be used as a key in the
+            step of updating old records that have been updated on
+            source.
+        since_datetime (datetime): date/time from which the filter will be
+            built, instead of using the max() value from the table.
 
+    Returns:
+        Tuple[str, str]: Tuple containing the maximum value and the where
+            condition of the SQL query.
     """
 
     if since_datetime:
         max_value = since_datetime
     else:
         if date_column:
             sql = f"SELECT MAX({date_column}) FROM {table}"
         else:
             sql = f"SELECT MAX({key_column}) FROM {table}"
 
         max_value = dest_hook.get_first(sql)[0]
 
     if date_column:
-        # Verifica se o formato do campo max_value é date ou datetime
+        # Checks if the format of the max_value field is date or datetime
         if isinstance(max_value, date):
             max_value = max_value.strftime("%Y-%m-%d")
         elif isinstance(max_value, datetime):
             max_value = max_value.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
 
         where_condition = f"{date_column} > '{max_value}'"
     else:
@@ -590,18 +588,16 @@
 
     return max_value, where_condition
 
 
 def _build_incremental_sqls(
     dest_table: str, source_table: str, key_column: str, column_list: str
 ):
-    """
-    Constrói as queries SQLs que realizam os Updates dos registros
-    atualizados desde a última sincronização e os Inserts das novas
-    linhas.
+    """Builds the SQL queries that perform the updates of the source updated
+    records since the last synchronization and the inserts of new records.
     """
 
     cols = ", ".join(f"{col} = orig.{col}" for col in column_list)
     updates_sql = f"""
             UPDATE {dest_table} SET {cols}
             FROM {source_table} orig
             WHERE orig.{key_column} = {dest_table}.{key_column}
@@ -631,74 +627,68 @@
     sync_exclusions: bool = False,
     source_exc_schema: str = None,
     source_exc_table: str = None,
     source_exc_column: str = None,
     chunksize: int = 1000,
     copy_table_comments: bool = False,
 ) -> None:
-    """
-    Realiza a atualização incremental de uma tabela. A sincronização
-    é realizada em 3 etapas. 1-Envia as alterações necessárias para uma
-    tabela intermediária localizada no esquema `increment_schema`.
-    2-Realiza os Updates. 3-Realiza os Inserts. Apenas as colunas que
-    existam na tabela no BD destino serão sincronizadas. Funciona com
-    Postgres na origem e MsSql no destino. O algoritmo também realiza,
-    opcionalmente, sincronização de exclusões.
+    """Performs incremental update on a table. The synchronization is
+    performed in 3 steps.
+        1 - Sends the necessary changes to an intermediate table
+        located in the `increment_schema` schema.
+        2 - Performs Updates.
+        3 - Performs Inserts. Only columns that exists at destination
+        table will be synchronized.
 
-    Exemplo:
+    Works with Postgres as source and MsSql as destination. `sync_db_2_db`
+    also optionally performs synchronization of deletions.
+
+    Example:
         sync_db_2_db(source_conn_id=SOURCE_CONN_ID,
                      destination_conn_id=DEST_CONN_ID,
                      table=table,
                      date_column=date_column,
                      key_column=key_column,
                      source_schema=SOURCE_SCHEMA,
                      destination_schema=STG_SCHEMA,
                      chunksize=CHUNK_SIZE)
 
     Args:
-        source_conn_id (str): string de conexão airflow do DB origem
-        destination_conn_id (str): string de conexão airflow do DB destino
-        table (str): tabela a ser sincronizada
-        date_column (str): nome da coluna a ser utilizado para
-            identificação dos registros atualizados na origem.
-        key_column (str): nome da coluna a ser utilizado como chave na
-            etapa de atualização dos registros antigos que sofreram
-            atualizações na origem.
-        source_eschema (str): esquema do BD na origem
-        destination_schema (str): esquema do BD no destino
-        increment_schema (str): Esquema no banco utilizado para tabelas
-            temporárias. Caso esta variável seja None, esta tabela será
-            criada no mesmo schema com sufixo '_alteracoes'
-        select_sql (str): select customizado para utilizar na carga ao invés
-            de replicar as colunas da tabela origem. Não deve ser utilizado com
-            JOINS, apenas para uma única tabela.
-        since_datetime (datetime): data/hora a partir da qual o incremento
-            será realizado, sobrepondo-se à data/hora máxima da tabela destino
-        sync_exclusions (bool): opção de sincronizar exclusões.
+        source_conn_id (str): Airflow connection string of the source DB.
+        destination_conn_id (str): Airflow connection string of the
+            destination DB.
+        table (str): Table to be synchronized
+        date_column (str): Name of the column to be used for
+            identifying updated records in the source.
+        key_column (str): Name of the column to be used as a key in
+            the update step of old records that have been updated in the source.
+        source_schema (str): Schema of the DB in the source.
+        destination_schema (str): schema of the DB in the destination.
+        increment_schema (str): Schema in the database used for temporary
+            tables. If this variable is None, the table will be created
+            at the same destiny schema with the suffix '_alteracoes'
+        select_sql (str): customized select to use in the load instead of
+            replicating the columns of the source table. Should not be used with
+            JOINS, only for a single table.
+        since_datetime (datetime): date/time from which the increment
+            will be performed, overriding the maximum date/time of the destination table.
+        sync_exclusions (bool): option to synchronize exclusions.
             Default = False.
-        source_exc_schema (str): esquema da tabela na origem onde estão
-            registradas exclusões
-        source_exc_table (str): tabela na origem onde estão registradas
-            exclusões
-        source_exc_column (str): coluna na tabela na origem onde estão
-            registradas exclusões
-        chunksize (int): tamanho do bloco de leitura na origem.
-        Default = 1000 linhas
+        source_exc_schema (str): schema of the table in the source where
+            exclusions are registered
+        source_exc_table (str): table in the source where exclusions are registered
+        source_exc_column (str): column in the table in the source where
+            exclusions are registered
+        chunksize (int): read block size in the source.
+        Default = 1000 rows
         copy_table_comments (bool): flag if includes on the execution the
             copy of table comments/descriptions. Default to False.
 
     Return:
         None
-
-    Todo:
-        * Automatizar a criação da tabela gêmea e remoção ao final
-        * Transformar em Airflow Operator
-        * Possibilitar ler de MsSql e escrever em Postgres
-        * Possibilitar inserir data da carga na tabela de destino
-        * Criar testes
     """
 
     def _divide_chunks(l, n):
         """Split list into a new list with n lists"""
         # looping till length l
         for i in range(0, len(l), n):
             yield l[i : i + n]
@@ -712,32 +702,32 @@
 
     source_hook = PostgresHook(postgres_conn_id=source_conn_id, autocommit=True)
     dest_hook, _ = get_hook_and_engine_by_provider(destination_conn_id)
 
     col_list = get_table_cols_name(destination_conn_id, destination_schema, table)
 
     dest_rows_count = _table_rows_count(dest_hook, dest_table_name)
-    logging.info("Total de linhas atualmente na tabela destino: %d.", dest_rows_count)
-    # If de tabela vazia separado para evitar erro na _build_filter_condition()
+    logging.info("Total rows at destination table: %d.", dest_rows_count)
+    # If empty table, to avoid error on _build_filter_condition()
     if dest_rows_count == 0:
-        raise Exception("Tabela destino vazia! Utilize carga full!")
+        raise Exception("Destination table empty. Use full load option.")
 
     ref_value, where_condition = _build_filter_condition(
         dest_hook, dest_table_name, date_column, key_column, since_datetime
     )
     new_rows_count = _table_rows_count(source_hook, source_table_name, where_condition)
-    logging.info("Total de linhas novas ou modificadas: %d.", new_rows_count)
+    logging.info("New or modified rows total: %d.", new_rows_count)
 
-    # Guarda as alterações e inclusões necessárias
+    # store updates and inserts
     if not select_sql:
         select_sql = build_select_sql(
             schema=source_schema, table=table, column_list=col_list
         )
     select_diff = f"{select_sql} WHERE {where_condition}"
-    logging.info("SELECT para espelhamento: %s", select_diff)
+    logging.info("SQL Query to mirror tables: %s", select_diff)
 
     copy_db_to_db(
         source={
             "conn_id": source_conn_id,
             "query": select_diff,
             "schema": source_table_name.split(".")[0],
             "table": source_table_name.split(".")[1],
@@ -748,36 +738,35 @@
             "table": inc_table_name.split(".")[1],
         },
         destination_truncate=True,
         chunksize=chunksize,
         load_type="incremental",
     )
 
-    # Reconstrói índices
+    # rebuild index
     destination_conn_type = get_conn_type(destination_conn_id)
     if destination_conn_type == "mssql":
         sql = f"ALTER INDEX ALL ON {inc_table_name} REBUILD"
     elif destination_conn_type == "postgres":
         sql = f"REINDEX TABLE {inc_table_name}"
 
     dest_hook.run(sql)
 
-    logging.info("Iniciando carga incremental na tabela %s.", dest_table_name)
+    logging.info("Starting incremental load on table %s.", dest_table_name)
     updates_sql, inserts_sql = _build_incremental_sqls(
         dest_table=f"{dest_table_name}",
         source_table=f"{inc_table_name}",
         key_column=key_column,
         column_list=col_list,
     )
-    # Realiza updates
+
     dest_hook.run(updates_sql)
-    # Realiza inserts de novas linhas
     dest_hook.run(inserts_sql)
 
-    # Se precisar aplicar as exclusões da origem no destino:
+    # if needed to delete rows at destination
     if sync_exclusions:
         source_exc_sql = f"""SELECT {key_column}
                              FROM {source_exc_schema}.{source_exc_table}
                              WHERE {source_exc_column} > '{ref_value}'
                           """
         rows = source_hook.get_records(source_exc_sql)
         ids_to_del = [row[0] for row in rows]
@@ -789,18 +778,18 @@
                 sql = f"""
                     DELETE FROM {dest_table_name}
                     WHERE {key_column} IN ({ids})
                 """
                 dest_hook.run(sql)
 
         logging.info(
-            "Quantidade de linhas possivelmente excluídas: %d", len(ids_to_del)
+            "Approximated number of rows deleted: %d", len(ids_to_del)
         )
 
-    # atualiza comentários da tabela
+    # update table descriptions/comments
     if copy_table_comments:
         _copy_table_comments(
             source=SourceConnection(
                 conn_id=source_conn_id,
                 schema=source_table_name.split(".")[0],
                 table=source_table_name.split(".")[1],
             ),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/patchwork.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/patchwork.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/samba_services.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/samba_services.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/date.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,64 @@
-""" Funções de uso comum para manipular datas e horas.
+"""Common use functions for manipulating dates and times.
 """
+
 import os
 from datetime import datetime, timedelta, date
 from dateutil.relativedelta import relativedelta
 
 AIRFLOW_TIMEZONE = os.getenv("AIRFLOW__CORE__DEFAULT_TIMEZONE")
 
 def remove_template_indentation(text: str) -> str:
-    """Remove a indentação em strings de templates.
+    """Remove indentation in template strings.
     """
+
     return ''.join(line.strip() for line in text.splitlines())
 
 def get_reference_date(context: dict) -> datetime:
-    """ Calcula a data de referência execução da DAG.
+    """Calculates the reference date of the DAG execution.
+
+    If it is a scheduled execution, it will be the logical_date, which
+    in Airflow is the start date of the execution interval for the DAG.
+
+    If it is triggered manually (trigger DAG), the reference_date
+    parameter can be passed in the configuration JSON. In this case,
+    it will be used instead of logical_date. The parameter must be
+    passed in ISO format (e.g., 2021-01-02T12:00):
+
+    {
+        "reference_date": "2021-01-02T12:00"
+    }
+
+    If manual activation (trigger DAG) is done without passing this
+    parameter, an exception will be raised.
+
+    Args:
+        context (dict): Airflow information about current task.
 
-        Caso seja uma execução agendada, será logical_date,
-        que no Airflow é a data do início do intervalo de execução da
-        DAG.
-
-        Caso seja feita ativação manual (trigger DAG), poderá ser
-        passado o parâmetro reference_date no JSON de configuração.
-        Nesse caso, valerá esta. O parâmetro deve ser passado no
-        formato ISO (ex.: 2021-01-02T12:00):
-
-        {
-            "reference_date": "2021-01-02T12:00"
-        }
+    Raises:
+        ValueError: Manual trigger without reference_date parameter
 
-        Caso seja feita a ativação manual (trigger DAG) sem passar
-        esse parâmetro, será levantada uma exceção.
+    Returns:
+        datetime: reference date based on how dag was triggered
     """
 
-    # trigger manual, sem especificar a variavel reference_date
+    # trigger manual, without variable reference_date defined
     if context["dag_run"].external_trigger and \
         context["dag_run"].conf is not None and \
         "reference_date" not in context["dag_run"].conf:
         raise ValueError(
             'Para executar esta DAG manualmente é necessário incluir o '
             'parâmetro reference_date no JSON das configurações.')
 
     reference_date: datetime = (
         datetime.fromisoformat(
             context["dag_run"].conf["reference_date"]
         )
     ) if context["dag_run"].conf \
-        else context["logical_date"] # execução agendada da dag
+        else context["logical_date"] # dag run scheduled
 
     return reference_date
 
 def get_trigger_date(context: dict, local_time: bool = False) -> datetime:
     """ Calcula a data de disparo da execução da DAG.
 
         Caso seja uma execução agendada, será data_interval_end,
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/db_connection.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/db_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/encode_html.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/encode_html.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/get_table_cols_name.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/get_table_cols_name.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/load_env_var.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_env_var.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/load_info.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/odf_tables.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/string_formatting.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/string_formatting.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/custom_functions/utils/table_comments.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/table_comments.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/bacen_STA_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/bacen_STA_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/ckan_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/ckan_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/dadosgovbr_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dadosgovbr_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/db_to_db_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/db_to_db_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/dou_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dou_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/gsheet_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/gsheet_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/hooks/osrm_hook.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/osrm_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/operators/datapackage_to_datadictionary_operator.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/datapackage_to_datadictionary_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/operators/db_to_csv_operator.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_csv_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/operators/db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_db_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
-Operador que realiza a cópia de dados seguindo uma estratégia completa
-(full) ou incremental de um banco de dados para outro. Os BDs podem ser
-Postgres ou SQL Server. Internamente são utilizadas as bibliotecas psycopg2 e
-pyodbc. Os dados copiados podem ser oriundos de uma tabela ou de um
-Select SQL.
+Airflow operator that performs data copying between DBs with complete
+or incremental strategy. The DBs can be Postgres, SQL Server or MySQL.
+It uses psycopg2 and pyodbc libraries. The copied data can
+come from a table or an SQL Query.
 
 Args:
-    is_incremental (bool, optional): Whether to perform an incremental copy
-        based on a datetime or key column. Defaults to False.
+    is_incremental (bool, optional): Whether to perform an incremental
+        copy based on a datetime or key column. Defaults to False.
 
     (when full copy)
     columns_to_ignore (List[str], optional): A list of column names to
         ignore during the copy operation. Defaults to None.
     destination_truncate (bool, optional): Whether to truncate the
         destination table before copying data to it. Defaults to True.
 
@@ -42,15 +41,15 @@
 
         (incremental copy)
         source incremental copy dict expects these keys:
         * conn_id -> required
         * schema -> required
         * query -> optional
         * source_exc_schema -> optional
-            Table `scheme` name at the source where exclusions are recorded.
+            Table `schema` name at the source where exclusions are recorded.
         * source_exc_table -> optional
             Table `table` name at the source where exclusions are recorded.
         * source_exc_column -> optional
             Table `column` name at the source where exclusions are recorded.
 
     destination (Dict[str, str]): A dictionary containing the connection
         details of the destination database.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/operators/gsheet_operator.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/gsheet_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/fastetl/operators/osrm_distance_operator.py` & `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/osrm_distance_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/setup.py` & `apache-airflow-providers-fastetl-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 """Perform the package apache-airflow-providers-fastetl setup."""
 setup(
     name="apache-airflow-providers-fastetl",
     version=__version__,
     description="FastETL custom package Apache Airflow provider.",
     long_description=long_description,
@@ -40,13 +40,14 @@
         "pytz>=2022.6",
         "requests>=2.28.1",
         "SQLAlchemy>=1.4.44"
     ],
     setup_requires=["setuptools", "wheel"],
     author="Time de Dados CGINF",
     author_email="seges.cginf@economia.gov.br",
+    url="https://github.com/economiagovbr/FastETL",
     classifiers=[
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
     ],
     python_requires="~=3.8",
 )
```

### Comparing `apache-airflow-providers-fastetl-0.0.7/tests/test_dag.py` & `apache-airflow-providers-fastetl-0.0.8/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/tests/test_db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.8/tests/test_db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/tests/test_odf_tables.py` & `apache-airflow-providers-fastetl-0.0.8/tests/test_odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.7/tests/test_osrm.py` & `apache-airflow-providers-fastetl-0.0.8/tests/test_osrm.py`

 * *Files identical despite different names*

