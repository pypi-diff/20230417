# Comparing `tmp/evadb-0.1.6.tar.gz` & `tmp/evadb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.1.6.tar", last modified: Wed Apr  5 07:30:29 2023, max compression
+gzip compressed data, was "evadb-0.2.0.tar", last modified: Mon Apr 17 14:50:18 2023, max compression
```

## Comparing `evadb-0.1.6.tar` & `evadb-0.2.0.tar`

### file list

```diff
@@ -1,446 +1,461 @@
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2022-08-11 16:20:33.000000 evadb-0.1.6/LICENSE.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11457 2023-04-05 07:30:29.890987 evadb-0.1.6/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10710 2023-03-28 02:19:14.000000 evadb-0.1.6/README.md
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.838986 evadb-0.1.6/eva/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      645 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.842986 evadb-0.1.6/eva/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4937 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/binder/binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11763 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/binder/statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8000 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.842986 evadb-0.1.6/eva/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17810 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/catalog/catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3076 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/catalog/catalog_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5695 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.842986 evadb-0.1.6/eva/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      886 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/models/association_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3752 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/models/base_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5110 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/models/column_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3274 2023-01-13 02:28:13.000000 evadb-0.1.6/eva/catalog/models/index_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2997 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/catalog/models/table_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3532 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4066 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2262 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4722 2023-01-07 04:09:45.000000 evadb-0.1.6/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2668 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2127 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/schema_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.846986 evadb-0.1.6/eva/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1167 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/base_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2873 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2887 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4571 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3669 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3078 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2826 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2476 2023-03-26 03:53:07.000000 evadb-0.1.6/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1936 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2688 2023-04-03 04:45:07.000000 evadb-0.1.6/eva/catalog/sql_config.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.846986 evadb-0.1.6/eva/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4025 2023-04-02 16:42:28.000000 evadb-0.1.6/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3599 2023-04-03 04:45:07.000000 evadb-0.1.6/eva/configuration/configuration_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1402 2023-04-02 16:31:36.000000 evadb-0.1.6/eva/configuration/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      840 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      767 2023-04-04 00:35:22.000000 evadb-0.1.6/eva/eva.yml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1553 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2399 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2137 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2214 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1418 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/create_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5728 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3866 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3433 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4738 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2504 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2010 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/drop_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3081 2023-01-15 20:48:47.000000 evadb-0.1.6/eva/executor/execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3071 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/executor/executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1523 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3499 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/faiss_index_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1580 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/function_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1751 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/groupby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1800 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/hash_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2255 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/join_build_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1661 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/lateral_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1575 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3086 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/load_csv_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1579 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4944 2023-04-02 15:22:00.000000 evadb-0.1.6/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1472 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4175 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/executor/orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7879 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/executor/plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1644 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1284 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/predicate_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1272 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/project_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1186 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1413 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1812 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2274 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/executor/storage_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1264 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/executor/union_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      619 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/ray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      610 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/ray/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      619 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3271 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/experimental/ray/executor/exchange_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1220 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/executor/ray_stage.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/ray/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/optimizer/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/ray/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      626 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3846 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/experimental/ray/optimizer/rules/rules.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.850986 evadb-0.1.6/eva/experimental/ray/planner/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/experimental/ray/planner/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1380 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/experimental/ray/planner/exchange_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.854986 evadb-0.1.6/eva/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5469 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/expression/abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3974 2023-01-07 04:09:45.000000 evadb-0.1.6/eva/expression/aggregation_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1618 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/expression/arithmetic_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4351 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/expression/comparison_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2613 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/expression/constant_value_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10440 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/expression/expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10151 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/expression/function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3081 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/expression/logical_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4756 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.854986 evadb-0.1.6/eva/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      633 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.854986 evadb-0.1.6/eva/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1332 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/catalog/frame_info.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      857 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/catalog/properties.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.854986 evadb-0.1.6/eva/models/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1809 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/models/server/response.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.854986 evadb-0.1.6/eva/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14831 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/models/storage/batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.858986 evadb-0.1.6/eva/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/optimizer/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3260 2023-01-27 02:16:54.000000 evadb-0.1.6/eva/optimizer/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2129 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/optimizer/cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3450 2022-11-11 01:28:51.000000 evadb-0.1.6/eva/optimizer/group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2669 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/optimizer/group_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4335 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/optimizer/memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35842 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/optimizer/operators.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3838 2023-01-15 21:02:15.000000 evadb-0.1.6/eva/optimizer/optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      982 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11919 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10128 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3552 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/optimizer/plan_generator.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1169 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/optimizer/property.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.858986 evadb-0.1.6/eva/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1016 2022-11-11 01:28:51.000000 evadb-0.1.6/eva/optimizer/rules/pattern.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    41963 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/optimizer/rules/rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6840 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7008 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13132 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/optimizer/statement_to_opr_convertor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.858986 evadb-0.1.6/eva/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-25 05:50:43.000000 evadb-0.1.6/eva/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1360 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/parser/alias.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2672 2023-01-13 02:28:13.000000 evadb-0.1.6/eva/parser/create_index_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2788 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4838 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/parser/create_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4859 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/create_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2048 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1767 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1793 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/parser/drop_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19163 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/parser/eva.lark
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1384 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/parser/explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2922 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/insert_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1717 2023-01-15 20:48:47.000000 evadb-0.1.6/eva/parser/lark_parser.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.862986 evadb-0.1.6/eva/parser/lark_visitor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2655 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2150 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10304 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1404 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1202 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1006 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4672 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5959 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2465 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2057 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      932 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2121 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1091 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9468 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3214 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1228 2023-01-15 20:48:47.000000 evadb-0.1.6/eva/parser/parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5921 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/parser/select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1460 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/parser/show_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1052 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/parser/statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8639 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/parser/table_ref.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1679 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/parser/types.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.866987 evadb-0.1.6/eva/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1689 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3302 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1455 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1930 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2401 2023-01-13 02:28:13.000000 evadb-0.1.6/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2076 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/plan_nodes/create_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3603 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1660 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1532 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1033 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2355 2023-01-27 02:16:54.000000 evadb-0.1.6/eva/plan_nodes/faiss_index_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1755 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1712 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2179 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2023 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1468 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2710 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1510 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1564 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1177 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1249 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/project_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1469 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1760 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1201 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4419 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1420 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/plan_nodes/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/plan_nodes/union_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.866987 evadb-0.1.6/eva/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2320 2023-04-02 15:22:17.000000 evadb-0.1.6/eva/readers/abstract_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2651 2023-03-20 03:12:11.000000 evadb-0.1.6/eva/readers/csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5617 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/readers/decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.866987 evadb-0.1.6/eva/readers/image/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/readers/image/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1007 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/readers/image/opencv_image_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.866987 evadb-0.1.6/eva/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      623 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3284 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/server/command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3502 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/server/db_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3276 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/server/interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2866 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/server/server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.870987 evadb-0.1.6/eva/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5659 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2385 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1694 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/storage/image_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8881 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-01-07 03:29:08.000000 evadb-0.1.6/eva/storage/storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2243 2023-04-04 00:35:29.000000 evadb-0.1.6/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.870987 evadb-0.1.6/eva/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.870987 evadb-0.1.6/eva/udfs/abstract/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/udfs/abstract/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2441 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3843 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3464 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/asl_action_recognition.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.870987 evadb-0.1.6/eva/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2185 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.870987 evadb-0.1.6/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2754 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3375 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1437 2023-04-04 03:25:14.000000 evadb-0.1.6/eva/udfs/decorators/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5675 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/decorators/yolo_object_detection_decorators.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5478 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2539 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/udfs/face_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5110 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1822 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/udfs/feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1028 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/udfs/gpu_compatible.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.874987 evadb-0.1.6/eva/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2568 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1647 2022-11-12 17:07:12.000000 evadb-0.1.6/eva/udfs/ndarray/crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1179 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1557 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/udfs/ndarray/open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1782 2023-01-02 23:54:50.000000 evadb-0.1.6/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2750 2023-01-02 23:54:53.000000 evadb-0.1.6/eva/udfs/ocr_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2471 2023-04-04 03:25:28.000000 evadb-0.1.6/eva/udfs/toxicity_classifier.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6764 2023-04-05 07:05:40.000000 evadb-0.1.6/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5043 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.874987 evadb-0.1.6/eva/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      611 2022-11-11 01:28:18.000000 evadb-0.1.6/eva/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      909 2023-04-02 15:22:43.000000 evadb-0.1.6/eva/utils/errors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6421 2023-04-03 04:45:07.000000 evadb-0.1.6/eva/utils/generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1837 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/utils/kv_cache.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      985 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/utils/logging_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1562 2023-03-28 02:19:14.000000 evadb-0.1.6/eva/utils/s3_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-04-01 16:09:26.000000 evadb-0.1.6/eva/utils/stats.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      711 2023-04-05 07:10:19.000000 evadb-0.1.6/eva/version.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.874987 evadb-0.1.6/evadb.egg-info/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11457 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13082 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       88 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/entry_points.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1037 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/requires.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       21 2023-04-05 07:30:29.000000 evadb-0.1.6/evadb.egg-info/top_level.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2022-06-26 17:11:46.000000 evadb-0.1.6/pyproject.toml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-04-05 07:30:29.894988 evadb-0.1.6/setup.cfg
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4011 2023-04-05 07:05:40.000000 evadb-0.1.6/setup.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.874987 evadb-0.1.6/test/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-09-30 14:20:49.000000 evadb-0.1.6/test/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.874987 evadb-0.1.6/test/benchmark_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:53.000000 evadb-0.1.6/test/benchmark_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1172 2023-04-01 16:09:26.000000 evadb-0.1.6/test/benchmark_tests/conftest.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3294 2023-04-01 16:09:26.000000 evadb-0.1.6/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.878987 evadb-0.1.6/test/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2032 2023-01-02 23:54:53.000000 evadb-0.1.6/test/binder/test_binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14016 2023-04-01 16:09:26.000000 evadb-0.1.6/test/binder/test_statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7961 2023-03-28 02:19:14.000000 evadb-0.1.6/test/binder/test_statement_binder_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1796 2022-12-13 23:02:13.000000 evadb-0.1.6/test/binder/test_statement_binder_python37.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.878987 evadb-0.1.6/test/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/catalog/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.878987 evadb-0.1.6/test/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7234 2023-03-28 02:19:14.000000 evadb-0.1.6/test/catalog/models/test_models.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.878987 evadb-0.1.6/test/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-01-07 03:29:08.000000 evadb-0.1.6/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4657 2023-04-02 20:13:44.000000 evadb-0.1.6/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-03-28 02:19:14.000000 evadb-0.1.6/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-04-01 16:09:26.000000 evadb-0.1.6/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3210 2023-03-28 02:19:14.000000 evadb-0.1.6/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3035 2023-04-02 20:13:44.000000 evadb-0.1.6/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7560 2023-04-04 00:35:29.000000 evadb-0.1.6/test/catalog/test_catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1402 2022-12-13 23:02:13.000000 evadb-0.1.6/test/catalog/test_column_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-04-01 16:09:26.000000 evadb-0.1.6/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.878987 evadb-0.1.6/test/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1490 2022-09-30 14:24:37.000000 evadb-0.1.6/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1690 2022-09-30 14:24:37.000000 evadb-0.1.6/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.882987 evadb-0.1.6/test/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1106 2023-03-28 02:19:14.000000 evadb-0.1.6/test/executor/test_abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2441 2023-01-02 23:54:50.000000 evadb-0.1.6/test/executor/test_create_mat_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3987 2023-03-28 02:19:14.000000 evadb-0.1.6/test/executor/test_create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5590 2022-08-08 22:30:00.000000 evadb-0.1.6/test/executor/test_execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1275 2022-12-13 23:02:13.000000 evadb-0.1.6/test/executor/test_executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4650 2023-01-02 23:54:50.000000 evadb-0.1.6/test/executor/test_limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3890 2023-03-28 02:19:14.000000 evadb-0.1.6/test/executor/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2884 2023-01-02 23:54:50.000000 evadb-0.1.6/test/executor/test_orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10986 2023-03-28 02:19:14.000000 evadb-0.1.6/test/executor/test_plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1397 2022-08-08 22:30:00.000000 evadb-0.1.6/test/executor/test_pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1817 2023-01-02 23:54:50.000000 evadb-0.1.6/test/executor/test_sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2775 2022-08-08 22:30:00.000000 evadb-0.1.6/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      847 2022-08-08 22:30:00.000000 evadb-0.1.6/test/executor/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.882987 evadb-0.1.6/test/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3722 2023-03-28 02:19:14.000000 evadb-0.1.6/test/expression/test_abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5149 2023-03-19 05:07:03.000000 evadb-0.1.6/test/expression/test_aggregation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2975 2023-01-02 23:54:50.000000 evadb-0.1.6/test/expression/test_arithmetic.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5578 2023-01-02 23:54:53.000000 evadb-0.1.6/test/expression/test_comparison.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2867 2022-08-08 22:30:00.000000 evadb-0.1.6/test/expression/test_expression_tree.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7555 2023-04-01 16:09:26.000000 evadb-0.1.6/test/expression/test_expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2022-11-12 17:07:12.000000 evadb-0.1.6/test/expression/test_function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6806 2023-03-19 05:07:03.000000 evadb-0.1.6/test/expression/test_logical.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1816 2023-03-19 05:07:03.000000 evadb-0.1.6/test/expression/test_tuple_value.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/integration_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/integration_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3546 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7647 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1091 2023-03-28 02:19:14.000000 evadb-0.1.6/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5123 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4839 2023-04-04 00:35:29.000000 evadb-0.1.6/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4510 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3145 2023-03-28 02:19:14.000000 evadb-0.1.6/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3838 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2898 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_like.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19220 2023-04-04 00:35:29.000000 evadb-0.1.6/test/integration_tests/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5192 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2601 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9954 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12046 2023-04-04 03:25:14.000000 evadb-0.1.6/test/integration_tests/test_pytorch.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2953 2023-03-28 02:19:14.000000 evadb-0.1.6/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7543 2023-04-05 07:05:40.000000 evadb-0.1.6/test/integration_tests/test_reuse.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5151 2023-03-28 02:19:14.000000 evadb-0.1.6/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    28346 2023-04-04 00:35:29.000000 evadb-0.1.6/test/integration_tests/test_select_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3873 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12251 2023-04-01 16:09:26.000000 evadb-0.1.6/test/integration_tests/test_similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12021 2023-03-28 02:19:14.000000 evadb-0.1.6/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      852 2023-03-28 02:19:14.000000 evadb-0.1.6/test/markers.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2022-10-16 04:44:32.000000 evadb-0.1.6/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5919 2023-04-05 07:05:40.000000 evadb-0.1.6/test/models/storage/test_batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/optimizer/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.1.6/test/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11281 2023-04-01 16:09:26.000000 evadb-0.1.6/test/optimizer/rules/test_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4195 2023-03-16 05:59:55.000000 evadb-0.1.6/test/optimizer/test_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2196 2023-03-28 02:19:14.000000 evadb-0.1.6/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4406 2022-08-08 22:30:00.000000 evadb-0.1.6/test/optimizer/test_cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2689 2022-08-08 22:30:00.000000 evadb-0.1.6/test/optimizer/test_group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1996 2022-08-08 22:30:00.000000 evadb-0.1.6/test/optimizer/test_memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1034 2022-08-08 22:30:00.000000 evadb-0.1.6/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10171 2023-03-28 02:19:14.000000 evadb-0.1.6/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2000 2023-01-07 03:29:08.000000 evadb-0.1.6/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13335 2023-03-28 02:19:14.000000 evadb-0.1.6/test/optimizer/test_statement_to_opr_convertor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36051 2023-03-28 02:19:14.000000 evadb-0.1.6/test/parser/test_parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4843 2023-03-28 02:19:14.000000 evadb-0.1.6/test/parser/test_parser_statements.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.886987 evadb-0.1.6/test/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.1.6/test/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6292 2023-03-28 02:19:14.000000 evadb-0.1.6/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-04-01 16:09:26.000000 evadb-0.1.6/test/readers/test_csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7288 2023-04-04 00:35:29.000000 evadb-0.1.6/test/readers/test_decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-12 17:07:12.000000 evadb-0.1.6/test/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1268 2023-01-02 23:54:53.000000 evadb-0.1.6/test/server/test_command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5057 2023-03-28 02:19:14.000000 evadb-0.1.6/test/server/test_db_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2581 2023-03-28 02:19:14.000000 evadb-0.1.6/test/server/test_interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-03-28 02:19:14.000000 evadb-0.1.6/test/server/test_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4001 2023-03-28 02:19:14.000000 evadb-0.1.6/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4023 2023-03-28 02:19:14.000000 evadb-0.1.6/test/storage/test_video_storage.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1801 2023-03-28 02:19:14.000000 evadb-0.1.6/test/test_eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1294 2022-12-13 23:02:13.000000 evadb-0.1.6/test/test_eva_imports.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1810 2023-03-28 02:19:14.000000 evadb-0.1.6/test/test_eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-08-08 22:30:00.000000 evadb-0.1.6/test/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7430 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2134 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      648 2022-10-16 04:44:32.000000 evadb-0.1.6/test/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      849 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2410 2022-10-16 04:44:32.000000 evadb-0.1.6/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2353 2023-04-04 03:44:38.000000 evadb-0.1.6/test/udfs/ndarray/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4154 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/test_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2154 2022-09-30 14:24:37.000000 evadb-0.1.6/test/udfs/test_emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3345 2023-03-28 02:19:14.000000 evadb-0.1.6/test/udfs/test_facenet_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2548 2022-10-30 19:28:39.000000 evadb-0.1.6/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2689 2022-12-13 23:02:13.000000 evadb-0.1.6/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15308 2023-04-04 03:25:28.000000 evadb-0.1.6/test/util.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/test/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.1.6/test/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4269 2023-04-03 04:45:07.000000 evadb-0.1.6/test/utils/test_generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2256 2023-03-28 02:19:14.000000 evadb-0.1.6/test/utils/test_timer.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-04-05 07:30:29.890987 evadb-0.1.6/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2022-06-26 17:11:46.000000 evadb-0.1.6/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-04-02 17:27:27.000000 evadb-0.2.0/LICENSE.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12958 2023-04-17 14:50:18.503700 evadb-0.2.0/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10710 2023-04-02 17:27:27.000000 evadb-0.2.0/README.md
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.459699 evadb-0.2.0/eva/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4937 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/binder/binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12003 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/binder/statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8000 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17810 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3076 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5695 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/association_models.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3752 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/base_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3274 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/schema_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/base_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2887 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2857 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/catalog/sql_config.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4025 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4374 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/configuration/configuration_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      840 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      756 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/eva.yml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1553 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2399 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2214 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1418 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5728 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4777 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/executor/create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2504 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3013 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3043 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1523 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3507 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/faiss_index_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/function_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/groupby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/hash_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/join_build_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_csv_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4944 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8071 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/predicate_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/project_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/executor/storage_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/union_executor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3521 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/executor/exchange_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/executor/ray_stage.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/optimizer/rules/rules.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/experimental/ray/planner/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/planner/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/planner/exchange_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5469 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/expression/abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/aggregation_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/comparison_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-04-13 06:13:25.000000 evadb-0.2.0/eva/expression/constant_value_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10440 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10151 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-04-17 01:45:56.000000 evadb-0.2.0/eva/expression/logical_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-04-13 06:13:17.000000 evadb-0.2.0/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/frame_info.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/properties.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1809 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/models/server/response.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14837 2023-04-06 16:06:01.000000 evadb-0.2.0/eva/models/storage/batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3260 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/group_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    35842 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/operators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3838 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12579 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10128 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5700 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/optimizer/plan_generator.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/property.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1016 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    41137 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7023 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7573 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13132 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/alias.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2672 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_index_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/parser/create_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19228 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/parser/eva.lark
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/parser/evaql/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    65109 2022-12-14 06:32:03.000000 evadb-0.2.0/eva/parser/evaql/evaql_lexer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)   408798 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    44890 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parserListener.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    26541 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parserVisitor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/insert_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_parser.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.479699 evadb-0.2.0/eva/parser/lark_visitor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2150 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10304 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5959 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2121 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/show_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/parser/table_ref.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1679 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/parser/types.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2401 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2355 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/faiss_index_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-04-05 18:07:02.000000 evadb-0.2.0/eva/plan_nodes/types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/union_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/abstract_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2651 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5617 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/readers/decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/readers/image/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/image/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1007 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/image/opencv_image_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-04-03 16:26:49.000000 evadb-0.2.0/eva/server/command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3276 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2866 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/server/server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5659 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2385 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1694 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/image_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8881 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2243 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/third_party/huggingface/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1506 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5776 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/create.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1453 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/abstract/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3096 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/asl_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2185 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2754 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3375 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1437 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/udfs/decorators/utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5675 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/yolo_object_detection_decorators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/face_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/feature_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2471 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/udfs/toxicity_classifier.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6764 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5043 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/errors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6957 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/utils/generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1837 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/kv_cache.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/logging_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/s3_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/stats.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      711 2023-04-17 02:39:30.000000 evadb-0.2.0/eva/version.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/evadb.egg-info/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12958 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13538 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1087 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/requires.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/top_level.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-04-02 17:27:27.000000 evadb-0.2.0/pyproject.toml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-04-17 14:50:18.503700 evadb-0.2.0/setup.cfg
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4093 2023-04-13 06:12:12.000000 evadb-0.2.0/setup.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/benchmark_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1172 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/conftest.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3294 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14016 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7961 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1796 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder_python37.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/models/test_models.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4745 2023-04-13 06:12:12.000000 evadb-0.2.0/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7560 2023-04-05 15:01:02.000000 evadb-0.2.0/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/test_column_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1690 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_create_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3987 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-04-06 05:12:11.000000 evadb-0.2.0/test/executor/test_execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10986 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-04-06 17:08:11.000000 evadb-0.2.0/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_aggregation.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_arithmetic.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_comparison.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_expression_tree.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-04-13 06:25:00.000000 evadb-0.2.0/test/expression/test_logical.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/integration_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3587 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7647 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5160 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-04-05 15:01:02.000000 evadb-0.2.0/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2454 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4088 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7790 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3896 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2956 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_like.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19262 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5233 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2660 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10184 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12724 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7580 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_reuse.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    29003 2023-04-06 17:08:11.000000 evadb-0.2.0/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3873 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12289 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      852 2023-04-02 17:27:27.000000 evadb-0.2.0/test/markers.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-04-05 15:01:02.000000 evadb-0.2.0/test/models/storage/test_batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11728 2023-04-12 18:47:51.000000 evadb-0.2.0/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-04-06 05:12:11.000000 evadb-0.2.0/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-04-13 06:12:12.000000 evadb-0.2.0/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13335 2023-04-12 18:47:51.000000 evadb-0.2.0/test/optimizer/test_statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36051 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/test_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4843 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/test_parser_statements.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-04-02 17:27:27.000000 evadb-0.2.0/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.0/test/readers/test_csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7288 2023-04-05 15:01:02.000000 evadb-0.2.0/test/readers/test_decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4001 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/test_video_storage.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1801 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_imports.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1810 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7430 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2134 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-04-13 06:12:12.000000 evadb-0.2.0/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4330 2023-04-13 06:12:12.000000 evadb-0.2.0/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16108 2023-04-13 06:12:12.000000 evadb-0.2.0/test/util.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-04-13 06:12:12.000000 evadb-0.2.0/test/utils/test_generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-04-02 17:27:27.000000 evadb-0.2.0/test/utils/test_timer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2181 2023-04-13 06:12:12.000000 evadb-0.2.0/test/utils/test_xdist.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.0/third_party/__init__.py
```

### Comparing `evadb-0.1.6/LICENSE.txt` & `evadb-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/PKG-INFO` & `evadb-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: evadb
-Version: 0.1.6
-Summary: EVA Video Database System (Think MySQL for videos).
-Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group
-Author-email: georgia.tech.db@gmail.com
-License: Apache License 2.0
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 <div >
   <a href="https://evadb.readthedocs.io/">
     <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
   </a>
   <div>
         <h3>Try It Out!</h3>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.1.6 Summary: EVA Video Database
-System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
-eva Download-URL: https://github.com/georgia-tech-db/eva Author: Georgia Tech
-Database Group Author-email: georgia.tech.db@gmail.com License: Apache License
-2.0 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3 Classifier: Development Status :: 3 - Alpha Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE.txt
 [EVA]
 **** Try It Out! ****
 [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
 Versions]
 # EVA AI-Relational Database System EVA is an open-source **AI-relational
 database with first-class support for deep learning models**. It aims to
 support AI-powered database applications that operate on both structured
```

### Comparing `evadb-0.1.6/README.md` & `evadb-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,187 +1,207 @@
-<div >
-  <a href="https://evadb.readthedocs.io/">
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-  </a>
-  <div>
-        <h3>Try It Out!</h3>
-        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+Metadata-Version: 2.1
+Name: evadb
+Version: 0.2.0
+Summary: EVA Video Database System (Think MySQL for videos).
+Home-page: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group
+Author-email: georgia.tech.db@gmail.com
+License: Apache License 2.0
+Download-URL: https://github.com/georgia-tech-db/eva
+Description: <div >
+          <a href="https://evadb.readthedocs.io/">
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
+          </a>
+          <div>
+                <h3>Try It Out!</h3>
+                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+                </a>
+                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+                </a>    
+                <a href="https://github.com/georgia-tech-db/eva/discussions">
+                    <img alt="Discuss on Github!" src="https://img.shields.io/badge/-Discuss%20on%20Github!-blueviolet">
+                </a>
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
+            </div>
+        </div>
+        
+        # EVA AI-Relational Database System
+        
+        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
+        
+        EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
+        
+        EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
+        
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
+         * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+         
+        If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
+        
+        The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
+        
+        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
+        
+        ## Why EVA? ##
+        
+        <details>
+          <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
+          Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
+        </details>
+        
+        <details>
+          <summary><b>Speed up queries and save money spent on model inference</b></summary>
+          EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
+        </details>
+        
+        <details>
+          <summary><b>Extensible by design to support custom deep learning models </b></summary>
+          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
+        </details>
+        
+        ## Links
+        * [Documentation](https://evadb.readthedocs.io/)
+        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        * [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+        * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
+        
+        ## Quick Start
+        
+        1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
+        
+        ```shell
+        pip install evadb
+        ```
+        
+        2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
+        ```shell
+        eva_server &   # launch server
+        eva_client     # launch client
+        ```
+        
+        3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
+        
+        ```mysql
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
+        ```
+        
+        4. That's it! You can now run queries over the loaded video:
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE id < 5;
+        ```
+        
+        5. Search for frames in the video that contain a car
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
+        ```
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        6. Search for frames in the video that contain a pedestrian and a car
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
+        ```
+        
+        7. Search for frames in the video with more than 3 cars
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
+        ```
+        
+        8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
+        ```mysql
+        CREATE UDF IF NOT EXISTS MyUDF
+        INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
+        OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
+                scores NDARRAY FLOAT32(ANYDIM))
+        TYPE  Classification
+        IMPL  'eva/udfs/fastrcnn_object_detector.py';
+        ```
+        
+        9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
+        ```mysql
+           -- Analyse emotions of faces in a video
+           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+           FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+           WHERE id < 15;
+        ```
+        
+        ## Illustrative EVA Applications 
+        
+        ### Traffic Analysis (Object Detection Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        ### MNIST Digit Recognition (Image Classification Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+        
+        ### Movie Analysis (Face Detection + Emotion Classfication Models)
+        
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+        
+        ### [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+        
+        ### [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
+        
+        ## Community
+        
+        Join the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for improving EVA.
+        
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
         </a>
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-        </a>    
-        <a href="https://github.com/georgia-tech-db/eva/discussions">
-            <img alt="Discuss on Github!" src="https://img.shields.io/badge/-Discuss%20on%20Github!-blueviolet">
-        </a>
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
-    </div>
-</div>
-
-# EVA AI-Relational Database System
-
-EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
-
-EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
-
-EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
-
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
- * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
- 
-If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
-
-The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
-
-The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
-
-## Why EVA? ##
-
-<details>
-  <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
-  Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
-</details>
-
-<details>
-  <summary><b>Speed up queries and save money spent on model inference</b></summary>
-  EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
-</details>
-
-<details>
-  <summary><b>Extensible by design to support custom deep learning models </b></summary>
-  EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
-</details>
-
-## Links
-* [Documentation](https://evadb.readthedocs.io/)
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-* [Demo](https://ada-00.cc.gatech.edu/eva/playground)
-
-## Quick Start
-
-1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
-
-```shell
-pip install evadb
-```
-
-2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
-```shell
-eva_server &   # launch server
-eva_client     # launch client
-```
-
-3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
-
-```mysql
-LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
-```
-
-4. That's it! You can now run queries over the loaded video:
-
-```mysql
-SELECT id, data FROM MyVideo WHERE id < 5;
-```
-
-5. Search for frames in the video that contain a car
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
-```
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-6. Search for frames in the video that contain a pedestrian and a car
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
-```
-
-7. Search for frames in the video with more than 3 cars
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
-```
-
-8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
-```mysql
-CREATE UDF IF NOT EXISTS MyUDF
-INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
-OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
-        scores NDARRAY FLOAT32(ANYDIM))
-TYPE  Classification
-IMPL  'eva/udfs/fastrcnn_object_detector.py';
-```
-
-9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
-```mysql
-   -- Analyse emotions of faces in a video
-   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-   FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-   WHERE id < 15;
-```
-
-## Illustrative EVA Applications 
-
-### Traffic Analysis (Object Detection Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-### MNIST Digit Recognition (Image Classification Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-
-### Movie Analysis (Face Detection + Emotion Classfication Models)
-
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-
-### [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-
-### [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-
-## Community
-
-Join the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for improving EVA.
-
-<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
-</a>
-
-### Architecture Diagram of EVA
-
-<img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-arch.png" alt="EVA Architecture Diagram" width="500">
-
-## Contributing to EVA
-
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-[![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-
-We welcome all kinds of contributions to EVA.
-To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-
-For more information on contributing to EVA, see our
-[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-
-## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
-Licensed under [Apache License](LICENSE).
+        
+        ### Architecture Diagram of EVA
+        
+        <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-arch.png" alt="EVA Architecture Diagram" width="500">
+        
+        ## Contributing to EVA
+        
+        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+        [![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
+        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
+        
+        We welcome all kinds of contributions to EVA.
+        To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        
+        For more information on contributing to EVA, see our
+        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+        
+        ## License
+        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
+        Licensed under [Apache License](LICENSE).
+        
+Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1 Name: evadb Version: 0.2.0 Summary: EVA Video Database
+System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
+eva Author: Georgia Tech Database Group Author-email: georgia.tech.db@gmail.com
+License: Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/
+eva Description:
 [EVA]
 **** Try It Out! ****
 [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
 Versions]
 # EVA AI-Relational Database System EVA is an open-source **AI-relational
 database with first-class support for deep learning models**. It aims to
 support AI-powered database applications that operate on both structured
@@ -89,8 +94,14 @@
 eva?branch=master) [![Documentation Status](https://readthedocs.org/projects/
 evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
 index.html) We welcome all kinds of contributions to EVA. To file a bug or
 request a feature, please use GitHub_issues. Pull_requests are welcome. For
 more information on contributing to EVA, see our [contribution guide](https://
 evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
 Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/
-) Licensed under [Apache License](LICENSE).
+) Licensed under [Apache License](LICENSE). Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Information Analysis Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `evadb-0.1.6/eva/__init__.py` & `evadb-0.2.0/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/binder/__init__.py` & `evadb-0.2.0/eva/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/binder/binder_utils.py` & `evadb-0.2.0/eva/binder/binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/binder/statement_binder.py` & `evadb-0.2.0/eva/binder/statement_binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from eva.parser.create_mat_view_statement import CreateMaterializedViewStatement
 from eva.parser.delete_statement import DeleteTableStatement
 from eva.parser.explain_statement import ExplainStatement
 from eva.parser.rename_statement import RenameTableStatement
 from eva.parser.select_statement import SelectStatement
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableRef
+from eva.third_party.huggingface.binder import assign_hf_udf
 from eva.utils.generic_utils import get_file_checksum, load_udf_class_from_file
 from eva.utils.logging_manager import logger
 
 if sys.version_info >= (3, 8):
     from functools import singledispatchmethod
 else:
     # https://stackoverflow.com/questions/24601722/how-can-i-use-functools-singledispatch-with-instance-methods
@@ -239,33 +240,36 @@
             err_msg = (
                 f"UDF with name {node.name} does not exist in the catalog. "
                 "Please create the UDF using CREATE UDF command."
             )
             logger.error(err_msg)
             raise BinderError(err_msg)
 
-        # Verify the consistency of the UDF. If the checksum of the UDF does not match
-        # the one stored in the catalog, an error will be thrown and the user will be
-        # asked to register the UDF again.
-        assert (
-            get_file_checksum(udf_obj.impl_file_path) == udf_obj.checksum
-        ), f"""UDF file {udf_obj.impl_file_path} has been modified from the
-            registration. Please create a new UDF using the CREATE UDF command or UPDATE the existing one."""
-
-        try:
-            node.function = load_udf_class_from_file(
-                udf_obj.impl_file_path, udf_obj.name
-            )
-        except Exception as e:
-            err_msg = (
-                f"{str(e)}. Please verify that the UDF class name in the"
-                "implementation file matches the UDF name."
-            )
-            logger.error(err_msg)
-            raise BinderError(err_msg)
+        if udf_obj.type == "HuggingFace":
+            node.function = assign_hf_udf(udf_obj)
+        else:
+            # Verify the consistency of the UDF. If the checksum of the UDF does not match
+            # the one stored in the catalog, an error will be thrown and the user will be
+            # asked to register the UDF again.
+            assert (
+                get_file_checksum(udf_obj.impl_file_path) == udf_obj.checksum
+            ), f"""UDF file {udf_obj.impl_file_path} has been modified from the
+                registration. Please create a new UDF using the CREATE UDF command or UPDATE the existing one."""
+
+            try:
+                node.function = load_udf_class_from_file(
+                    udf_obj.impl_file_path, udf_obj.name
+                )
+            except Exception as e:
+                err_msg = (
+                    f"{str(e)}. Please verify that the UDF class name in the"
+                    "implementation file matches the UDF name."
+                )
+                logger.error(err_msg)
+                raise BinderError(err_msg)
 
         node.udf_obj = udf_obj
         output_objs = self._catalog.get_udf_io_catalog_output_entries(udf_obj)
         if node.output:
             for obj in output_objs:
                 if obj.name.lower() == node.output:
                     node.output_objs = [obj]
```

### Comparing `evadb-0.1.6/eva/binder/statement_binder_context.py` & `evadb-0.2.0/eva/binder/statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/__init__.py` & `evadb-0.2.0/eva/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/catalog_manager.py` & `evadb-0.2.0/eva/catalog/catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/catalog_type.py` & `evadb-0.2.0/eva/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/catalog_utils.py` & `evadb-0.2.0/eva/catalog/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/__init__.py` & `evadb-0.2.0/eva/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/association_models.py` & `evadb-0.2.0/eva/catalog/models/association_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/base_model.py` & `evadb-0.2.0/eva/catalog/models/base_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/column_catalog.py` & `evadb-0.2.0/eva/catalog/models/column_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/index_catalog.py` & `evadb-0.2.0/eva/catalog/models/index_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/table_catalog.py` & `evadb-0.2.0/eva/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.0/eva/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/udf_catalog.py` & `evadb-0.2.0/eva/catalog/models/udf_catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from sqlalchemy import Column, String
 from sqlalchemy.orm import relationship
 
 from eva.catalog.models.association_models import depend_udf_and_udf_cache
 from eva.catalog.models.base_model import BaseModel
 from eva.catalog.models.udf_io_catalog import UdfIOCatalogEntry
+from eva.catalog.models.udf_metadata_catalog import UdfMetadataCatalogEntry
 
 
 class UdfCatalog(BaseModel):
     """The `UdfCatalog` catalog stores information about the user-defined functions (UDFs) in the system. It maintains the following information for each UDF
     `_row_id:` an autogenerated identifier
     `_impl_file_path: ` the path to the implementation script for the UDF
     `_type:` an optional tag associated with the UDF (useful for grouping similar UDFs, such as multiple object detection UDFs)
@@ -67,22 +68,27 @@
         outputs = []
         for attribute in self._attributes:
             if attribute._is_input:
                 args.append(attribute.as_dataclass())
             else:
                 outputs.append(attribute.as_dataclass())
 
+        metadata = []
+        for meta_key_value in self._metadata:
+            metadata.append(meta_key_value.as_dataclass())
+
         return UdfCatalogEntry(
             row_id=self._row_id,
             name=self._name,
             impl_file_path=self._impl_file_path,
             type=self._type,
             checksum=self._checksum,
             args=args,
             outputs=outputs,
+            metadata=metadata,
             dep_caches=[entry.as_dataclass() for entry in self._dep_caches],
         )
 
 
 @dataclass(unsafe_hash=True)
 class UdfCatalogEntry:
     """Dataclass representing an entry in the `UdfCatalog`.
@@ -92,21 +98,23 @@
     name: str
     impl_file_path: str
     type: str
     checksum: str
     row_id: int = None
     args: List[UdfIOCatalogEntry] = field(compare=False, default_factory=list)
     outputs: List[UdfIOCatalogEntry] = field(compare=False, default_factory=list)
+    metadata: List[UdfMetadataCatalogEntry] = field(compare=False, default_factory=list)
     dep_caches: List[UdfIOCatalogEntry] = field(compare=False, default_factory=list)
 
     def display_format(self):
         def _to_str(col):
             col_display = col.display_format()
             return f"{col_display['name']} {col_display['data_type']}"
 
         return {
             "name": self.name,
             "inputs": [_to_str(col) for col in self.args],
             "outputs": [_to_str(col) for col in self.outputs],
             "type": self.type,
             "impl": self.impl_file_path,
+            "metadata": self.metadata,
         }
```

### Comparing `evadb-0.1.6/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.0/eva/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.0/eva/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.0/eva/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/schema_utils.py` & `evadb-0.2.0/eva/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/__init__.py` & `evadb-0.2.0/eva/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/base_service.py` & `evadb-0.2.0/eva/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.0/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/catalog/sql_config.py` & `evadb-0.2.0/eva/catalog/sql_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,23 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
 
 from sqlalchemy import create_engine, event
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from eva.configuration.configuration_manager import ConfigurationManager
 
 IDENTIFIER_COLUMN = "_row_id"
 
-# import os
-# def prefix_worker_id(uri: str):
-#    try:
-#        worker_id = os.environ["PYTEST_XDIST_WORKER"]
-#        base = "eva_catalog.db"
-#        uri = uri.replace(base, str(worker_id) + "_" + base)
-#    except KeyError:
-#        # Single threaded mode
-#        pass
-#    return uri
-
 
 class SQLConfig:
     """Singleton class for configuring connection to the database.
 
     Attributes:
         _instance: stores the singleton instance of the class.
     """
@@ -54,18 +44,29 @@
 
     def __init__(self):
         """Initializes the engine and session for database operations
 
         Retrieves the database uri for connection from ConfigurationManager.
         """
         uri = ConfigurationManager().get_value("core", "catalog_database_uri")
-        # parallelize using xdist
-        # worker_uri = prefix_worker_id(str(uri))
+
+        # to parallelize tests using pytest-xdist
+        def prefix_worker_id_to_uri(uri: str):
+            try:
+                worker_id = os.environ["PYTEST_XDIST_WORKER"]
+                base = "eva_catalog.db"
+                # eva_catalog.db -> test_gw1_eva_catalog.db
+                uri = uri.replace(base, "test_" + str(worker_id) + "_" + base)
+            except KeyError:
+                pass
+            return uri
+
+        self.worker_uri = prefix_worker_id_to_uri(str(uri))
         # set echo=True to log SQL
-        self.engine = create_engine(uri)
+        self.engine = create_engine(self.worker_uri, isolation_level="SERIALIZABLE")
 
         if self.engine.url.get_backend_name() == "sqlite":
             # enforce foreign key constraint and wal logging for sqlite
             # https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#foreign-key-support
 
             def _enable_sqlite_pragma(dbapi_con, con_record):
                 dbapi_con.execute("pragma foreign_keys=ON")
```

### Comparing `evadb-0.1.6/eva/configuration/__init__.py` & `evadb-0.2.0/eva/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/configuration/bootstrap_environment.py` & `evadb-0.2.0/eva/configuration/bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/configuration/configuration_manager.py` & `evadb-0.2.0/eva/configuration/configuration_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
+from pathlib import Path
 from typing import Any
 
 import yaml
 
 from eva.configuration.bootstrap_environment import bootstrap_environment
 from eva.configuration.constants import (
     EVA_CONFIG_FILE,
@@ -31,18 +33,37 @@
         if not hasattr(cls, "_instance"):
             cls._instance = super(ConfigurationManager, cls).__new__(cls)
             cls._create_if_not_exists()
 
         return cls._instance
 
     @classmethod
+    def suffix_pytest_xdist_worker_id_to_dir(cls, path: Path):
+        try:
+            worker_id = os.environ["PYTEST_XDIST_WORKER"]
+            path = path / str(worker_id)
+        except KeyError:
+            pass
+        return path
+
+    @classmethod
     def _create_if_not_exists(cls):
         if not cls._yml_path.exists():
+            initial_eva_config_dir = Path(EVA_DEFAULT_DIR)
+
+            # parallelize tests using pytest-xdist
+            # activated only under pytest-xdist
+            # Changes config dir From EVA_DEFAULT_DIR To EVA_DEFAULT_DIR / gw1
+            # (where gw1 is worker id)
+            updated_eva_config_dir = cls.suffix_pytest_xdist_worker_id_to_dir(
+                initial_eva_config_dir
+            )
+            cls._yml_path = updated_eva_config_dir / EVA_CONFIG_FILE
             bootstrap_environment(
-                eva_config_dir=EVA_DEFAULT_DIR,
+                eva_config_dir=updated_eva_config_dir,
                 eva_installation_dir=EVA_INSTALLATION_DIR,
             )
 
     @classmethod
     def _get(cls, category: str, key: str) -> Any:
         with cls._yml_path.open("r") as yml_file:
             config_obj = yaml.load(yml_file, Loader=yaml.FullLoader)
```

### Comparing `evadb-0.1.6/eva/configuration/constants.py` & `evadb-0.2.0/eva/configuration/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/constants.py` & `evadb-0.2.0/eva/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/eva.yml` & `evadb-0.2.0/eva/eva.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 00000110: 5f73 697a 6520 2f20 6261 7463 685f 6d65  _size / batch_me
 00000120: 6d5f 7369 7a65 290a 2020 6261 7463 685f  m_size).  batch_
 00000130: 6d65 6d5f 7369 7a65 3a20 3330 3030 3030  mem_size: 300000
 00000140: 3030 0a0a 2020 2320 6261 7463 6820 7369  00..  # batch si
 00000150: 7a65 2075 7365 6420 666f 7220 6770 755f  ze used for gpu_
 00000160: 6f70 6572 6174 696f 6e73 0a20 2067 7075  operations.  gpu
 00000170: 5f62 6174 6368 5f73 697a 653a 2031 0a0a  _batch_size: 1..
-00000180: 2020 6770 7573 3a20 7b20 2231 3237 2e30    gpus: { "127.0
-00000190: 2e30 2e31 223a 205b 305d 207d 0a0a 7374  .0.1": [0] }..st
-000001a0: 6f72 6167 653a 0a20 2074 6d70 5f64 6972  orage:.  tmp_dir
-000001b0: 3a20 2222 0a20 2073 335f 646f 776e 6c6f  : "".  s3_downlo
-000001c0: 6164 5f64 6972 3a20 2222 0a20 2073 7472  ad_dir: "".  str
-000001d0: 7563 7475 7265 645f 6461 7461 5f65 6e67  uctured_data_eng
-000001e0: 696e 653a 2022 6576 612e 7374 6f72 6167  ine: "eva.storag
-000001f0: 652e 7371 6c69 7465 5f73 746f 7261 6765  e.sqlite_storage
-00000200: 5f65 6e67 696e 652e 5351 4c53 746f 7261  _engine.SQLStora
-00000210: 6765 456e 6769 6e65 220a 2020 7669 6465  geEngine".  vide
-00000220: 6f5f 656e 6769 6e65 3a20 2265 7661 2e73  o_engine: "eva.s
-00000230: 746f 7261 6765 2e76 6964 656f 5f73 746f  torage.video_sto
-00000240: 7261 6765 5f65 6e67 696e 652e 4465 636f  rage_engine.Deco
-00000250: 7264 5374 6f72 6167 6545 6e67 696e 6522  rdStorageEngine"
-00000260: 0a20 2069 6d61 6765 5f65 6e67 696e 653a  .  image_engine:
-00000270: 2022 6576 612e 7374 6f72 6167 652e 696d   "eva.storage.im
-00000280: 6167 655f 7374 6f72 6167 655f 656e 6769  age_storage_engi
-00000290: 6e65 2e49 6d61 6765 5374 6f72 6167 6545  ne.ImageStorageE
-000002a0: 6e67 696e 6522 0a73 6572 7665 723a 0a20  ngine".server:. 
-000002b0: 2068 6f73 743a 2022 302e 302e 302e 3022   host: "0.0.0.0"
-000002c0: 0a20 2070 6f72 743a 2035 3433 320a 2020  .  port: 5432.  
-000002d0: 736f 636b 6574 5f74 696d 656f 7574 3a20  socket_timeout: 
-000002e0: 3630 0a0a 6578 7065 7269 6d65 6e74 616c  60..experimental
-000002f0: 3a0a 2020 7261 793a 2046 616c 7365 0a    :.  ray: False.
+00000180: 2020 6770 755f 6964 733a 205b 302c 2031    gpu_ids: [0, 1
+00000190: 5d0a 0a73 746f 7261 6765 3a0a 2020 746d  ]..storage:.  tm
+000001a0: 705f 6469 723a 2022 220a 2020 7333 5f64  p_dir: "".  s3_d
+000001b0: 6f77 6e6c 6f61 645f 6469 723a 2022 220a  ownload_dir: "".
+000001c0: 2020 7374 7275 6374 7572 6564 5f64 6174    structured_dat
+000001d0: 615f 656e 6769 6e65 3a20 2265 7661 2e73  a_engine: "eva.s
+000001e0: 746f 7261 6765 2e73 716c 6974 655f 7374  torage.sqlite_st
+000001f0: 6f72 6167 655f 656e 6769 6e65 2e53 514c  orage_engine.SQL
+00000200: 5374 6f72 6167 6545 6e67 696e 6522 0a20  StorageEngine". 
+00000210: 2076 6964 656f 5f65 6e67 696e 653a 2022   video_engine: "
+00000220: 6576 612e 7374 6f72 6167 652e 7669 6465  eva.storage.vide
+00000230: 6f5f 7374 6f72 6167 655f 656e 6769 6e65  o_storage_engine
+00000240: 2e44 6563 6f72 6453 746f 7261 6765 456e  .DecordStorageEn
+00000250: 6769 6e65 220a 2020 696d 6167 655f 656e  gine".  image_en
+00000260: 6769 6e65 3a20 2265 7661 2e73 746f 7261  gine: "eva.stora
+00000270: 6765 2e69 6d61 6765 5f73 746f 7261 6765  ge.image_storage
+00000280: 5f65 6e67 696e 652e 496d 6167 6553 746f  _engine.ImageSto
+00000290: 7261 6765 456e 6769 6e65 220a 7365 7276  rageEngine".serv
+000002a0: 6572 3a0a 2020 686f 7374 3a20 2230 2e30  er:.  host: "0.0
+000002b0: 2e30 2e30 220a 2020 706f 7274 3a20 3534  .0.0".  port: 54
+000002c0: 3332 0a20 2073 6f63 6b65 745f 7469 6d65  32.  socket_time
+000002d0: 6f75 743a 2036 300a 0a65 7870 6572 696d  out: 60..experim
+000002e0: 656e 7461 6c3a 0a20 2072 6179 3a20 4661  ental:.  ray: Fa
+000002f0: 6c73 650a                                lse.
```

### Comparing `evadb-0.1.6/eva/eva_cmd_client.py` & `evadb-0.2.0/eva/eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/eva_server.py` & `evadb-0.2.0/eva/eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/__init__.py` & `evadb-0.2.0/eva/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/abstract_executor.py` & `evadb-0.2.0/eva/executor/abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.0/eva/executor/apply_and_merge_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/create_executor.py` & `evadb-0.2.0/eva/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/create_index_executor.py` & `evadb-0.2.0/eva/executor/create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/create_mat_view_executor.py` & `evadb-0.2.0/eva/executor/create_mat_view_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/create_udf_executor.py` & `evadb-0.2.0/eva/executor/create_udf_executor.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,45 +11,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 
 from eva.catalog.catalog_manager import CatalogManager
+from eva.configuration.constants import EVA_DEFAULT_DIR
 from eva.executor.abstract_executor import AbstractExecutor
 from eva.models.storage.batch import Batch
 from eva.plan_nodes.create_udf_plan import CreateUDFPlan
+from eva.third_party.huggingface.create import gen_hf_io_catalog_entries
 from eva.udfs.decorators.utils import load_io_from_udf_decorators
 from eva.utils.errors import UDFIODefinitionError
 from eva.utils.generic_utils import load_udf_class_from_file
 from eva.utils.logging_manager import logger
 
 
 class CreateUDFExecutor(AbstractExecutor):
     def __init__(self, node: CreateUDFPlan):
         super().__init__(node)
 
-    def exec(self, *args, **kwargs):
-        """Create udf executor
+    def handle_huggingface_udf(self):
+        """Handle HuggingFace UDFs
 
-        Calls the catalog to insert a udf catalog entry.
+        HuggingFace UDFs are special UDFs that are not loaded from a file.
+        So we do not need to call the setup method on them like we do for other UDFs.
         """
-        catalog_manager = CatalogManager()
-        # check catalog if it already has this udf entry
-        if catalog_manager.get_udf_catalog_entry_by_name(self.node.name):
-            if self.node.if_not_exists:
-                msg = f"UDF {self.node.name} already exists, nothing added."
-                logger.warn(msg)
-                yield Batch(pd.DataFrame([msg]))
-                return
-            else:
-                msg = f"UDF {self.node.name} already exists."
-                logger.error(msg)
-                raise RuntimeError(msg)
+        impl_path = f"{EVA_DEFAULT_DIR}/udfs/abstract/hf_abstract_udf.py"
+        io_list = gen_hf_io_catalog_entries(self.node.name, self.node.metadata)
+        return (
+            self.node.name,
+            impl_path,
+            self.node.udf_type,
+            io_list,
+            self.node.metadata,
+        )
+
+    def handle_generic_udf(self):
+        """Handle generic UDFs
 
+        Generic UDFs are loaded from a file. We check for inputs passed by the user during CREATE or try to load io from decorators.
+        """
         # load the udf class from the file
         impl_path = self.node.impl_path.absolute().as_posix()
         try:
             # loading the udf class from the file
             udf = load_udf_class_from_file(impl_path, self.node.name)
             # initializing the udf class calls the setup method internally
             udf()
@@ -71,14 +76,45 @@
             else:
                 # try to load the outputs from decorators, the outputs from CREATE statement take precedence
                 io_list.extend(load_io_from_udf_decorators(udf, is_input=False))
         except UDFIODefinitionError as e:
             err_msg = f"Error creating UDF, input/output definition incorrect: {str(e)}"
             logger.error(err_msg)
             raise RuntimeError(err_msg)
+        return (
+            self.node.name,
+            impl_path,
+            self.node.udf_type,
+            io_list,
+            self.node.metadata,
+        )
+
+    def exec(self, *args, **kwargs):
+        """Create udf executor
+
+        Calls the catalog to insert a udf catalog entry.
+        """
+        catalog_manager = CatalogManager()
+        # check catalog if it already has this udf entry
+        if catalog_manager.get_udf_catalog_entry_by_name(self.node.name):
+            if self.node.if_not_exists:
+                msg = f"UDF {self.node.name} already exists, nothing added."
+                logger.warn(msg)
+                yield Batch(pd.DataFrame([msg]))
+                return
+            else:
+                msg = f"UDF {self.node.name} already exists."
+                logger.error(msg)
+                raise RuntimeError(msg)
+
+        # if it's a type of HuggingFaceModel, override the impl_path
+        if self.node.udf_type == "HuggingFace":
+            name, impl_path, udf_type, io_list, metadata = self.handle_huggingface_udf()
+        else:
+            name, impl_path, udf_type, io_list, metadata = self.handle_generic_udf()
 
         catalog_manager.insert_udf_catalog_entry(
-            self.node.name, impl_path, self.node.udf_type, io_list, self.node.metadata
+            name, impl_path, udf_type, io_list, metadata
         )
         yield Batch(
             pd.DataFrame([f"UDF {self.node.name} successfully added to the database."])
         )
```

### Comparing `evadb-0.1.6/eva/executor/delete_executor.py` & `evadb-0.2.0/eva/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/drop_executor.py` & `evadb-0.2.0/eva/executor/drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/drop_udf_executor.py` & `evadb-0.2.0/eva/executor/drop_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/execution_context.py` & `evadb-0.2.0/eva/executor/execution_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import random
-import socket
-from typing import List, Set
+from typing import List
 
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.constants import NO_GPU
-from eva.utils.generic_utils import is_gpu_available
+from eva.utils.generic_utils import get_gpu_count, is_gpu_available
 
 
 class Context:
     """
     Stores the context information of the executor, i.e.,
     if using spark, name of the application, current spark executors,
     if using horovod: current rank etc.
@@ -38,38 +37,34 @@
         self._config_manager = ConfigurationManager()
         self._gpus = self._populate_gpu_ids()
 
     @property
     def gpus(self):
         return self._gpus
 
-    def _possible_addresses(self) -> Set:
-        host = socket.gethostname()
-        result_address = {host}
-        true_host, aliases, address = socket.gethostbyaddr(host)
-        result_address.add(true_host)
-        result_address.update(set(aliases).union(set(address)))
-        return result_address
-
     def _populate_gpu_from_config(self) -> List:
-        gpu_conf = self._config_manager.get_value("executor", "gpus")
-        gpu_conf = gpu_conf if gpu_conf else {}
-        this_address = self._possible_addresses()
-        intersection_addresses = this_address.intersection(gpu_conf.keys())
-        if len(intersection_addresses) != 0:
-            return [str(gpu) for gpu in gpu_conf.get(intersection_addresses.pop())]
-        return []
+        # Populate GPU IDs from yaml config file.
+        gpu_conf = self._config_manager.get_value("executor", "gpu_ids")
+        availble_gpus = [i for i in range(get_gpu_count())]
+        return list(set(availble_gpus) & set(gpu_conf))
 
     def _populate_gpu_from_env(self) -> List:
-        gpus = map(
-            lambda x: x.strip(), os.environ.get("GPU_DEVICES", "").strip().split(",")
+        # Populate GPU IDs from env variable.
+        gpu_conf = map(
+            lambda x: x.strip(),
+            os.environ.get("CUDA_VISIBLE_DEVICES", "").strip().split(","),
         )
-        return list(filter(lambda x: x, gpus))
+        gpu_conf = list(filter(lambda x: x, gpu_conf))
+        gpu_conf = [int(gpu_id) for gpu_id in gpu_conf]
+        availble_gpus = [i for i in range(get_gpu_count())]
+        return list(set(availble_gpus) & set(gpu_conf))
 
     def _populate_gpu_ids(self) -> List:
+        # Populate available GPU IDs from Torch library. Then, select subset of GPUs
+        # from available GPUs based on user configuration.
         if not is_gpu_available():
             return []
         gpus = self._populate_gpu_from_config()
         if len(gpus) == 0:
             gpus = self._populate_gpu_from_env()
         return gpus
```

### Comparing `evadb-0.1.6/eva/executor/executor_utils.py` & `evadb-0.2.0/eva/executor/executor_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     return batch
 
 
 def apply_predicate(batch: Batch, predicate: AbstractExpression) -> Batch:
     if not batch.empty() and predicate is not None:
         outcomes = predicate.evaluate(batch)
         batch.drop_zero(outcomes)
-        batch.reset_index()
     return batch
 
 
 def handle_if_not_exists(table_info: TableInfo, if_not_exist=False):
     if CatalogManager().check_table_exists(
         table_info.table_name,
         table_info.database_name,
```

### Comparing `evadb-0.1.6/eva/executor/explain_executor.py` & `evadb-0.2.0/eva/executor/explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/faiss_index_scan_executor.py` & `evadb-0.2.0/eva/executor/faiss_index_scan_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         for dis, row_id in zip(dis_np[0], row_id_np[0]):
             distance_list.append(dis)
             row_id_list.append(row_id)
 
         # Load projected columns from disk and join with search results.
         row_id_col_name = None
         res_row_list = [None for _ in range(self.limit_count.value)]
-        for batch in self.children[0].exec():
+        for batch in self.children[0].exec(**kwargs):
             column_list = batch.columns
             if not row_id_col_name:
                 row_id_alias = get_row_id_column_alias(column_list)
                 row_id_col_name = "{}.{}".format(row_id_alias, IDENTIFIER_COLUMN)
 
             # Nested join.
             for _, row in batch.frames.iterrows():
```

### Comparing `evadb-0.1.6/eva/executor/function_scan_executor.py` & `evadb-0.2.0/eva/executor/function_scan_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,10 +37,10 @@
             "lateral_input" in kwargs
         ), "Key lateral_input not passed to the FunctionScan"
         lateral_input = kwargs.get("lateral_input")
         if not lateral_input.empty():
             res = self.func_expr.evaluate(lateral_input)
             if not res.empty():
                 if self.do_unnest:
-                    res.unnest()
+                    res.unnest(res.columns)
 
                 yield res
```

### Comparing `evadb-0.1.6/eva/executor/groupby_executor.py` & `evadb-0.2.0/eva/executor/groupby_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         super().__init__(node)
         self._segment_length = int(node.groupby_clause.value[:-1])
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
 
         buffer = Batch(pd.DataFrame())
-        for batch in child_executor.exec():
+        for batch in child_executor.exec(**kwargs):
             new_batch = buffer + batch
             # We assume that all the segments exactly of segment_length size
             # and discard any dangling frames in the end.
             while len(new_batch) >= self._segment_length:
                 yield new_batch[: self._segment_length]
                 new_batch = new_batch[self._segment_length :]
             buffer = new_batch
```

### Comparing `evadb-0.1.6/eva/executor/hash_join_executor.py` & `evadb-0.2.0/eva/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/insert_executor.py` & `evadb-0.2.0/eva/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/join_build_executor.py` & `evadb-0.2.0/eva/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/lateral_join_executor.py` & `evadb-0.2.0/eva/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/limit_executor.py` & `evadb-0.2.0/eva/executor/limit_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         super().__init__(node)
         self._limit_count = node.limit_value
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         remaining_tuples = self._limit_count
         # aggregates the batches into one large batch
-        for batch in child_executor.exec():
+        for batch in child_executor.exec(**kwargs):
             if len(batch) > remaining_tuples:
                 yield batch[:remaining_tuples]
                 return
 
             remaining_tuples -= len(batch)
             yield batch
```

### Comparing `evadb-0.1.6/eva/executor/load_csv_executor.py` & `evadb-0.2.0/eva/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/load_executor.py` & `evadb-0.2.0/eva/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/load_multimedia_executor.py` & `evadb-0.2.0/eva/executor/load_multimedia_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.0/eva/executor/nested_loop_join_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     def __init__(self, node: NestedLoopJoinPlan):
         super().__init__(node)
         self.predicate = node.join_predicate
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         outer = self.children[0]
         inner = self.children[1]
-        for row1 in outer.exec():
-            for row2 in inner.exec():
+        for row1 in outer.exec(**kwargs):
+            for row2 in inner.exec(**kwargs):
                 result_batch = Batch.join(row1, row2)
                 result_batch.reset_index()
                 result_batch = apply_predicate(result_batch, self.predicate)
                 if not result_batch.empty():
                     yield result_batch
```

### Comparing `evadb-0.1.6/eva/executor/orderby_executor.py` & `evadb-0.2.0/eva/executor/orderby_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         return sort_type_bools
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         aggregated_batch_list = []
 
         # aggregates the batches into one large batch
-        for batch in child_executor.exec():
+        for batch in child_executor.exec(**kwargs):
             self.batch_sizes.append(len(batch))
             aggregated_batch_list.append(batch)
         aggregated_batch = Batch.concat(aggregated_batch_list, copy=False)
 
         # nothing to order by
         if not len(aggregated_batch):
             return
```

### Comparing `evadb-0.1.6/eva/executor/plan_executor.py` & `evadb-0.2.0/eva/executor/plan_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         elif plan_opr_type == PlanOprType.LIMIT:
             executor_node = LimitExecutor(node=plan)
         elif plan_opr_type == PlanOprType.SAMPLE:
             executor_node = SampleExecutor(node=plan)
         elif plan_opr_type == PlanOprType.NESTED_LOOP_JOIN:
             executor_node = NestedLoopJoinExecutor(node=plan)
         elif plan_opr_type == PlanOprType.LATERAL_JOIN:
+            logger.warn(
+                "LateralJoin Executor should not be part of the execution plan."
+                "Please raise an issue with the current query. Thanks!"
+            )
             executor_node = LateralJoinExecutor(node=plan)
         elif plan_opr_type == PlanOprType.HASH_JOIN:
             executor_node = HashJoinExecutor(node=plan)
         elif plan_opr_type == PlanOprType.HASH_BUILD:
             executor_node = BuildJoinExecutor(node=plan)
         elif plan_opr_type == PlanOprType.FUNCTION_SCAN:
             executor_node = FunctionScanExecutor(node=plan)
```

### Comparing `evadb-0.1.6/eva/executor/pp_executor.py` & `evadb-0.2.0/eva/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/predicate_executor.py` & `evadb-0.2.0/eva/executor/predicate_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
     def __init__(self, node: PredicatePlan):
         super().__init__(node)
         self.predicate = node.predicate
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
-        for batch in child_executor.exec(*args, **kwargs):
+        for batch in child_executor.exec(**kwargs):
             batch = apply_predicate(batch, self.predicate)
             if not batch.empty():
                 yield batch
```

### Comparing `evadb-0.1.6/eva/executor/project_executor.py` & `evadb-0.2.0/eva/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/rename_executor.py` & `evadb-0.2.0/eva/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/sample_executor.py` & `evadb-0.2.0/eva/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/seq_scan_executor.py` & `evadb-0.2.0/eva/executor/seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/show_info_executor.py` & `evadb-0.2.0/eva/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/storage_executor.py` & `evadb-0.2.0/eva/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/executor/union_executor.py` & `evadb-0.2.0/eva/executor/union_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/__init__.py` & `evadb-0.2.0/eva/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/__init__.py` & `evadb-0.2.0/eva/experimental/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/executor/__init__.py` & `evadb-0.2.0/eva/experimental/ray/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/executor/exchange_executor.py` & `evadb-0.2.0/eva/experimental/ray/executor/exchange_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 from ray.util.queue import Queue
 
 from eva.executor.abstract_executor import AbstractExecutor
+from eva.executor.executor_utils import ExecutorError
 from eva.experimental.ray.executor.ray_stage import (
     StageCompleteSignal,
     ray_stage,
     ray_stage_wait_and_alert,
 )
 from eva.experimental.ray.planner.exchange_plan import ExchangePlan
 from eva.models.storage.batch import Batch
@@ -39,14 +40,17 @@
         iq = input_queues[0]
 
         while True:
             next_item = iq.get(block=True)
             if next_item is StageCompleteSignal:
                 iq.put(StageCompleteSignal)
                 break
+            elif isinstance(next_item, ExecutorError):
+                iq.put(next_item)
+                raise next_item
             else:
                 yield next_item
 
 
 class ExchangeExecutor(AbstractExecutor):
     """
     Applies predicates to filter the frames which satisfy the condition
@@ -89,11 +93,13 @@
                 )
             )
         ray_stage_wait_and_alert.remote(ray_task, [output_queue])
         while is_top:
             res = output_queue.get(block=True)
             if res is StageCompleteSignal:
                 break
+            elif isinstance(res, ExecutorError):
+                raise res
             else:
                 yield res
         else:
             return output_queue
```

### Comparing `evadb-0.1.6/eva/experimental/ray/executor/ray_stage.py` & `evadb-0.2.0/eva/experimental/ray/executor/ray_stage.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Callable, List
 
 import ray
+from ray.exceptions import RayError
 from ray.util.queue import Queue
 
+from eva.executor.executor_utils import ExecutorError
+
 
 class StageCompleteSignal:
     pass
 
 
 @ray.remote(num_cpus=0)
 def ray_stage_wait_and_alert(tasks: ray.ObjectRef, output_queue: Queue):
-    ray.get(tasks)
-    for q in output_queue:
-        q.put(StageCompleteSignal)
+    try:
+        ray.get(tasks)
+        for q in output_queue:
+            q.put(StageCompleteSignal)
+    except RayError as e:
+        for q in output_queue:
+            q.put(ExecutorError(e.cause))
 
 
 @ray.remote
 def ray_stage(
-    exectuor: Callable, input_queues: List[Queue], output_queues: List[Queue]
+    executor: Callable, input_queues: List[Queue], output_queues: List[Queue]
 ):
     if len(input_queues) > 1 or len(output_queues) > 1:
         raise NotImplementedError
 
-    gen = exectuor(input_queues=input_queues)
+    gen = executor(input_queues=input_queues)
     for next_item in gen:
         for oq in output_queues:
             oq.put(next_item)
```

### Comparing `evadb-0.1.6/eva/experimental/ray/optimizer/__init__.py` & `evadb-0.2.0/eva/experimental/ray/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/optimizer/rules/__init__.py` & `evadb-0.2.0/eva/experimental/ray/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/optimizer/rules/rules.py` & `evadb-0.2.0/eva/experimental/ray/optimizer/rules/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import TYPE_CHECKING
 
 from eva.optimizer.rules.pattern import Pattern
 
 if TYPE_CHECKING:
     from eva.optimizer.optimizer_context import OptimizerContext
 
+from eva.executor.execution_context import Context
 from eva.experimental.ray.planner.exchange_plan import ExchangePlan
 from eva.expression.function_expression import FunctionExpression
 from eva.optimizer.operators import (
     LogicalExchange,
     LogicalGet,
     LogicalProject,
     OperatorType,
@@ -66,15 +67,18 @@
     def check(self, grp_id: int, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalProject, context: OptimizerContext):
         after = ProjectPlan(before.target_list)
         for child in before.children:
             after.append_child(child)
-        upper = ExchangePlan(parallelism=1)
+        upper = ExchangePlan(
+            parallelism=1,
+            ray_conf={"num_gpus": 1} if Context().gpus else {"num_cpus": 1},
+        )
         upper.append_child(after)
         yield upper
 
 
 class LogicalGetToSeqScan(Rule):
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICALGET)
@@ -101,11 +105,17 @@
             )
         )
         scan.append_child(lower)
         # Check whether the projection contains a UDF
         if before.target_list is None or not any(
             [isinstance(expr, FunctionExpression) for expr in before.target_list]
         ):
-            return scan
-        upper = ExchangePlan(parallelism=2)
-        upper.append_child(scan)
-        yield upper
+            yield scan
+        else:
+            upper = ExchangePlan(
+                parallelism=2,
+                ray_conf={"num_gpus": 1}
+                if len(Context().gpus) >= 2
+                else {"num_cpus": 1},
+            )
+            upper.append_child(scan)
+            yield upper
```

### Comparing `evadb-0.1.6/eva/experimental/ray/planner/__init__.py` & `evadb-0.2.0/eva/experimental/ray/planner/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/experimental/ray/planner/exchange_plan.py` & `evadb-0.2.0/eva/experimental/ray/planner/exchange_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     Arguments:
         all: Bool
             UNION (deduplication) vs UNION ALL (non-deduplication)
     """
 
     def __init__(
-        self, parallelism: int = 1, ray_conf: Dict[str, Any] = {"num_gpus": 1}
+        self, parallelism: int = 1, ray_conf: Dict[str, Any] = {"num_cpus": 1}
     ):
         self.parallelism = parallelism
         self.ray_conf = ray_conf
         super().__init__(PlanOprType.EXCHANGE)
 
     def __str__(self) -> str:
         return "ExchangePlan"
```

### Comparing `evadb-0.1.6/eva/expression/__init__.py` & `evadb-0.2.0/eva/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/abstract_expression.py` & `evadb-0.2.0/eva/expression/abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/aggregation_expression.py` & `evadb-0.2.0/eva/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/arithmetic_expression.py` & `evadb-0.2.0/eva/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/comparison_expression.py` & `evadb-0.2.0/eva/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/constant_value_expression.py` & `evadb-0.2.0/eva/expression/constant_value_expression.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,14 @@
     def __init__(self, value: Any, v_type: ColumnType = ColumnType.INTEGER):
         super().__init__(ExpressionType.CONSTANT_VALUE)
         self._value = value
         self._v_type = v_type
 
     def evaluate(self, batch: Batch, **kwargs):
         batch = Batch(pd.DataFrame({0: [self._value] * len(batch)}))
-        if "mask" in kwargs:
-            batch = batch[kwargs["mask"]]
         return batch
 
     def signature(self) -> str:
         return str(self)
 
     @property
     def value(self):
```

### Comparing `evadb-0.1.6/eva/expression/expression_utils.py` & `evadb-0.2.0/eva/expression/expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/function_expression.py` & `evadb-0.2.0/eva/expression/function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/expression/logical_expression.py` & `evadb-0.2.0/eva/expression/logical_expression.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,45 +31,43 @@
             children.append(left)
         if right is not None:
             children.append(right)
         super().__init__(
             exp_type, rtype=ExpressionReturnType.BOOLEAN, children=children
         )
 
-    def evaluate(self, *args, **kwargs):
+    def evaluate(self, batch, **kwargs):
         if self.get_children_count() == 2:
-
-            left_batch = self.get_child(0).evaluate(*args, **kwargs)
+            left_batch = self.get_child(0).evaluate(batch, **kwargs)
             if self.etype == ExpressionType.LOGICAL_AND:
-
                 if left_batch.all_false():  # check if all are false
                     return left_batch
-                kwargs["mask"] = left_batch.create_mask()
+                mask = left_batch.create_mask()
             elif self.etype == ExpressionType.LOGICAL_OR:
                 if left_batch.all_true():  # check if all are true
                     return left_batch
-                kwargs["mask"] = left_batch.create_inverted_mask()
-            right_batch = self.get_child(1).evaluate(*args, **kwargs)
-            left_batch.update_indices(kwargs["mask"], right_batch)
+                mask = left_batch.create_inverted_mask()
+
+            right_batch = self.get_child(1).evaluate(batch[mask], **kwargs)
+            left_batch.update_indices(mask, right_batch)
 
             return left_batch
         else:
-            batch = self.get_child(0).evaluate(*args, **kwargs)
+            batch = self.get_child(0).evaluate(batch, **kwargs)
             if self.etype == ExpressionType.LOGICAL_NOT:
                 batch.invert()
                 return batch
 
     def __eq__(self, other):
         is_subtree_equal = super().__eq__(other)
         if not isinstance(other, LogicalExpression):
             return False
         return is_subtree_equal and self.etype == other.etype
 
     def get_symbol(self) -> str:
-
         if self.etype == ExpressionType.LOGICAL_AND:
             return "AND"
         elif self.etype == ExpressionType.LOGICAL_OR:
             return "OR"
         elif self.etype == ExpressionType.LOGICAL_NOT:
             return "NOT"
         else:
```

### Comparing `evadb-0.1.6/eva/expression/tuple_value_expression.py` & `evadb-0.2.0/eva/expression/tuple_value_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,16 +71,14 @@
         return self._col_alias
 
     @col_alias.setter
     def col_alias(self, value: str):
         self._col_alias = value
 
     def evaluate(self, batch: Batch, *args, **kwargs):
-        if "mask" in kwargs:
-            batch = batch[kwargs["mask"]]
         return batch.project([self.col_alias])
 
     def signature(self):
         """It constructs the signature of the tuple value expression.
         It assumes the col_object attribute is populated by the binder with the catalog
         entries. For a standard column in the table, it returns `table_name.col_name`,
         and for UDF output columns it returns `udf_name.col_name`
```

### Comparing `evadb-0.1.6/eva/models/__init__.py` & `evadb-0.2.0/eva/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/catalog/__init__.py` & `evadb-0.2.0/eva/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/catalog/frame_info.py` & `evadb-0.2.0/eva/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/catalog/properties.py` & `evadb-0.2.0/eva/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/server/__init__.py` & `evadb-0.2.0/eva/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/server/response.py` & `evadb-0.2.0/eva/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/storage/__init__.py` & `evadb-0.2.0/eva/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/models/storage/batch.py` & `evadb-0.2.0/eva/models/storage/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return self._frames
 
     def __len__(self):
         return len(self._frames)
 
     @property
     def columns(self):
-        return self._frames.columns
+        return list(self._frames.columns)
 
     def column_as_numpy_array(self, column_name: str) -> np.ndarray:
         """Return a column as numpy array
 
         Args:
             column_name (str): the name of the required column
```

### Comparing `evadb-0.1.6/eva/optimizer/__init__.py` & `evadb-0.2.0/eva/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/binder.py` & `evadb-0.2.0/eva/optimizer/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/cost_model.py` & `evadb-0.2.0/eva/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/group.py` & `evadb-0.2.0/eva/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/group_expression.py` & `evadb-0.2.0/eva/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/memo.py` & `evadb-0.2.0/eva/optimizer/memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/operators.py` & `evadb-0.2.0/eva/optimizer/operators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/optimizer_context.py` & `evadb-0.2.0/eva/optimizer/optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.0/eva/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.0/eva/optimizer/optimizer_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,21 +80,28 @@
         valid_rules = sorted(valid_rules, key=lambda x: x.promise())
         for rule in valid_rules:
             binder = Binder(self.root_expr, rule.pattern, self.optimizer_context.memo)
             for match in iter(binder):
                 if not rule.check(match, self.optimizer_context):
                     continue
                 after = rule.apply(match, self.optimizer_context)
-                for plan in after:
+                plans = list(after)
+                assert (
+                    len(plans) <= 1
+                ), "Rewrite rule cannot generate more than oen alternate plan."
+                for plan in plans:
                     new_expr = self.optimizer_context.replace_expression(
                         plan, self.root_expr.group_id
                     )
                     self.optimizer_context.task_stack.push(
                         TopDownRewrite(new_expr, self.rule_set, self.optimizer_context)
                     )
+                    # The root has changed so we cannot apply more rules to the same
+                    # root, hence return
+                    return
 
                 self.root_expr.mark_rule_explored(rule.rule_type)
         for child in self.root_expr.children:
             child_expr = self.optimizer_context.memo.groups[child].logical_exprs[0]
             self.optimizer_context.task_stack.push(
                 TopDownRewrite(child_expr, self.rule_set, self.optimizer_context)
             )
@@ -140,22 +147,29 @@
             for match in iter(binder):
                 if not rule.check(match, self.optimizer_context):
                     continue
                 logger.info(
                     "In BottomUp, Rule {} matched for {}".format(rule, self.root_expr)
                 )
                 after = rule.apply(match, self.optimizer_context)
-                for plan in after:
+                plans = list(after)
+                assert (
+                    len(plans) <= 1
+                ), "Rewrite rule cannot generate more than oen alternate plan."
+                for plan in plans:
                     new_expr = self.optimizer_context.replace_expression(
                         plan, self.root_expr.group_id
                     )
                     logger.info("After rewiting {}".format(self.root_expr))
                     self.optimizer_context.task_stack.push(
                         BottomUpRewrite(new_expr, self.rule_set, self.optimizer_context)
                     )
+                    # The root has changed so we cannot apply more rules to the same
+                    # root, hence return
+                    return
             self.root_expr.mark_rule_explored(rule.rule_type)
 
 
 class OptimizeExpression(OptimizerTask):
     def __init__(
         self,
         root_expr: GroupExpression,
```

### Comparing `evadb-0.1.6/eva/optimizer/optimizer_utils.py` & `evadb-0.2.0/eva/optimizer/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/property.py` & `evadb-0.2.0/eva/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/rules/__init__.py` & `evadb-0.2.0/eva/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/rules/pattern.py` & `evadb-0.2.0/eva/optimizer/rules/pattern.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/optimizer/rules/rules.py` & `evadb-0.2.0/eva/optimizer/rules/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,44 +182,14 @@
             sampling_rate=sample_freq,
             sampling_type=sample_type,
             children=lget.children,
         )
         yield new_get_opr
 
 
-class EmbedProjectIntoGet(Rule):
-    def __init__(self):
-        pattern = Pattern(OperatorType.LOGICALPROJECT)
-        pattern.append_child(Pattern(OperatorType.LOGICALGET))
-        super().__init__(RuleType.EMBED_PROJECT_INTO_GET, pattern)
-
-    def promise(self):
-        return Promise.EMBED_PROJECT_INTO_GET
-
-    def check(self, before: Operator, context: OptimizerContext):
-        # nothing else to check if logical match found return true
-        return True
-
-    def apply(self, before: LogicalProject, context: OptimizerContext):
-        target_list = before.target_list
-        lget = before.children[0]
-        new_get_opr = LogicalGet(
-            lget.video,
-            lget.table_obj,
-            alias=lget.alias,
-            predicate=lget.predicate,
-            target_list=target_list,
-            sampling_rate=lget.sampling_rate,
-            sampling_type=lget.sampling_type,
-            children=lget.children,
-        )
-
-        yield new_get_opr
-
-
 class CacheFunctionExpressionInApply(Rule):
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICAL_APPLY_AND_MERGE)
         pattern.append_child(Pattern(OperatorType.DUMMY))
         super().__init__(RuleType.CACHE_FUNCTION_EXPRESISON_IN_APPLY, pattern)
 
     def promise(self):
@@ -383,27 +353,31 @@
         apply_and_merge: LogicalApplyAndMerge = before.children[0]
         aliases = context.memo.get_group_by_id(A.group_id).aliases
         predicate = before.predicate
         pushdown_pred, rem_pred = extract_pushdown_predicate_for_alias(
             predicate, aliases
         )
 
+        # we do not return a new plan if nothing can be pushed
+        # this ensures we do not keep applying this optimization
+        if pushdown_pred is None:
+            return
+
         # if we find a feasible pushdown predicate, add a new filter node between
         # ApplyAndMerge and Dummy
         if pushdown_pred:
             pushdown_filter = LogicalFilter(predicate=pushdown_pred)
             pushdown_filter.append_child(A)
             apply_and_merge.children = [pushdown_filter]
 
         # If we have partial predicate make it the root
         root_node = apply_and_merge
-        assert rem_pred is None
-        # if rem_pred:
-        #    root_node = LogicalFilter(predicate=rem_pred)
-        #    root_node.append_child(apply_and_merge)
+        if rem_pred:
+            root_node = LogicalFilter(predicate=rem_pred)
+            root_node.append_child(apply_and_merge)
 
         yield root_node
 
 
 class CombineSimilarityOrderByAndLimitToFaissIndexScan(Rule):
     """
     This rule currently rewrites Order By + Limit to a Faiss index scan.
```

### Comparing `evadb-0.1.6/eva/optimizer/rules/rules_base.py` & `evadb-0.2.0/eva/optimizer/rules/rules_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     """
     Manages enums for all the supported rules
     """
 
     # Don't move this enum, else will break rule exploration logic
     INVALID_RULE = 0
 
-    # REWRITE RULES(LOGICAL -> LOGICAL)
+    # REWRITE RULES TOP DOWN APPLY FIRST (LOGICAL -> LOGICAL)
+    XFORM_LATERAL_JOIN_TO_LINEAR_FLOW = auto()
+    TOP_DOWN_DELIMETER = auto()
+
+    # REWRITE RULES BOTTOM UP APPLY SECOND (LOGICAL -> LOGICAL)
     EMBED_FILTER_INTO_GET = auto()
-    EMBED_FILTER_INTO_DERIVED_GET = auto()
     EMBED_SAMPLE_INTO_GET = auto()
-    EMBED_PROJECT_INTO_DERIVED_GET = auto()
-    EMBED_PROJECT_INTO_GET = auto()
     PUSHDOWN_FILTER_THROUGH_JOIN = auto()
-    XFORM_LATERAL_JOIN_TO_LINEAR_FLOW = auto()
     PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE = auto()
     COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN = auto()
     REORDER_PREDICATES = auto()
 
     REWRITE_DELIMETER = auto()
 
     # TRANSFORMATION RULES (LOGICAL -> LOGICAL)
@@ -130,15 +130,14 @@
 
     # TRANSFORMATION RULES (LOGICAL -> LOGICAL)
     LOGICAL_INNER_JOIN_COMMUTATIVITY = auto()
     CACHE_FUNCTION_EXPRESISON_IN_APPLY = auto()
 
     # REWRITE RULES
     EMBED_FILTER_INTO_GET = auto()
-    EMBED_PROJECT_INTO_GET = auto()
     EMBED_SAMPLE_INTO_GET = auto()
     XFORM_LATERAL_JOIN_TO_LINEAR_FLOW = auto()
     PUSHDOWN_FILTER_THROUGH_JOIN = auto()
     PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE = auto()
     COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN = auto()
     REORDER_PREDICATES = auto()
 
@@ -172,16 +171,22 @@
 
     def is_logical_rule(self):
         return (
             self.rule_type.value > RuleType.REWRITE_DELIMETER.value
             and self.rule_type.value < RuleType.TRANSFORMATION_DELIMETER.value
         )
 
-    def is_rewrite_rule(self):
-        return self.rule_type.value < RuleType.REWRITE_DELIMETER.value
+    def is_stage_two_rewrite_rules(self):
+        return (
+            self.rule_type.value > RuleType.TOP_DOWN_DELIMETER.value
+            and self.rule_type.value < RuleType.REWRITE_DELIMETER.value
+        )
+
+    def is_stage_one_rewrite_rules(self):
+        return self.rule_type.value < RuleType.TOP_DOWN_DELIMETER.value
 
     @abstractmethod
     def promise(self) -> int:
         raise NotImplementedError
 
     @abstractmethod
     def check(self, before: Operator, context: OptimizerContext) -> bool:
```

### Comparing `evadb-0.1.6/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.0/eva/optimizer/rules/rules_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from eva.experimental.ray.optimizer.rules.rules import (
     LogicalProjectToPhysical as DistributedLogicalProjectToPhysical,
 )
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CombineSimilarityOrderByAndLimitToFaissIndexScan,
     EmbedFilterIntoGet,
-    EmbedProjectIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
     LogicalCreateIndexToFaiss,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
@@ -77,23 +76,24 @@
 class RulesManager:
     def __init__(self):
         self._logical_rules = [
             LogicalInnerJoinCommutativity(),
             CacheFunctionExpressionInApply(),
         ]
 
-        self._rewrite_rules = [
+        self._stage_one_rewrite_rules = [
+            XformLateralJoinToLinearFlow(),
+        ]
+
+        self._stage_two_rewrite_rules = [
             EmbedFilterIntoGet(),
             # EmbedFilterIntoDerivedGet(),
-            EmbedProjectIntoGet(),
-            # EmbedProjectIntoDerivedGet(),
             EmbedSampleIntoGet(),
             PushDownFilterThroughJoin(),
             PushDownFilterThroughApplyAndMerge(),
-            XformLateralJoinToLinearFlow(),
             CombineSimilarityOrderByAndLimitToFaissIndexScan(),
             ReorderPredicates(),
         ]
 
         ray_enabled = ConfigurationManager().get_value("experimental", "ray")
 
         self._implementation_rules = [
@@ -128,20 +128,27 @@
             LogicalApplyAndMergeToPhysical(),
             LogicalFaissIndexScanToPhysical(),
         ]
 
         if ray_enabled:
             self._implementation_rules.append(LogicalExchangeToPhysical())
         self._all_rules = (
-            self._rewrite_rules + self._logical_rules + self._implementation_rules
+            self._stage_one_rewrite_rules
+            + self._stage_two_rewrite_rules
+            + self._logical_rules
+            + self._implementation_rules
         )
 
     @property
-    def rewrite_rules(self):
-        return self._rewrite_rules
+    def stage_one_rewrite_rules(self):
+        return self._stage_one_rewrite_rules
+
+    @property
+    def stage_two_rewrite_rules(self):
+        return self._stage_two_rewrite_rules
 
     @property
     def implementation_rules(self):
         return self._implementation_rules
 
     @property
     def logical_rules(self):
@@ -152,41 +159,47 @@
             for rule in rule_list:
                 if rule.rule_type == rule_to_remove.rule_type:
                     rule_list.remove(rule)
 
         for rule in rules:
             assert (
                 rule.is_implementation_rule()
-                or rule.is_rewrite_rule()
+                or rule.is_stage_one_rewrite_rules()
+                or rule.is_stage_two_rewrite_rules()
                 or rule.is_logical_rule()
             ), f"Provided Invalid rule {rule}"
 
             if rule.is_implementation_rule():
                 _remove_from_list(self.implementation_rules, rule)
-            elif rule.is_rewrite_rule():
-                _remove_from_list(self.rewrite_rules, rule)
+            elif rule.is_stage_one_rewrite_rules():
+                _remove_from_list(self.stage_one_rewrite_rules, rule)
+            elif rule.is_stage_two_rewrite_rules():
+                _remove_from_list(self.stage_two_rewrite_rules, rule)
             elif rule.is_logical_rule():
                 _remove_from_list(self.logical_rules, rule)
 
     def add_rules(self, rules: List[Rule]):
         def _add_to_list(rule_list, rule_to_remove):
             if any([rule.rule_type != rule_to_remove.rule_type for rule in rule_list]):
                 rule_list.append(rule)
 
         for rule in rules:
             assert (
                 rule.is_implementation_rule()
-                or rule.is_rewrite_rule()
+                or rule.is_stage_one_rewrite_rules()
+                or rule.is_stage_two_rewrite_rules()
                 or rule.is_logical_rule()
             ), f"Provided Invalid rule {rule}"
 
             if rule.is_implementation_rule():
                 _add_to_list(self.implementation_rules, rule)
-            elif rule.is_rewrite_rule():
-                _add_to_list(self.rewrite_rules, rule)
+            elif rule.is_stage_one_rewrite_rules():
+                _add_to_list(self.stage_one_rewrite_rules, rule)
+            elif rule.is_stage_two_rewrite_rules():
+                _add_to_list(self.stage_two_rewrite_rules, rule)
             elif rule.is_logical_rule():
                 _add_to_list(self.logical_rules, rule)
 
 
 @contextmanager
 def disable_rules(rules: List[Rule]):
     """Use this function to temporarily drop rules.
```

### Comparing `evadb-0.1.6/eva/optimizer/statement_to_opr_convertor.py` & `evadb-0.2.0/eva/optimizer/statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/__init__.py` & `evadb-0.2.0/eva/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/alias.py` & `evadb-0.2.0/eva/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/create_index_statement.py` & `evadb-0.2.0/eva/parser/create_index_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/create_mat_view_statement.py` & `evadb-0.2.0/eva/parser/create_mat_view_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/create_statement.py` & `evadb-0.2.0/eva/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/create_udf_statement.py` & `evadb-0.2.0/eva/parser/create_udf_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         metadata: List[Tuple[str, str]] = None,
     ):
         super().__init__(StatementType.CREATE_UDF)
         self._name = name
         self._if_not_exists = if_not_exists
         self._inputs = inputs
         self._outputs = outputs
-        self._impl_path = Path(impl_path)
+        self._impl_path = Path(impl_path) if impl_path else None
         self._udf_type = udf_type
         self._metadata = metadata
 
     def __str__(self) -> str:
         exists_str = ""
         if self._if_not_exists:
             exists_str += "IF NOT EXISTS "
```

### Comparing `evadb-0.1.6/eva/parser/delete_statement.py` & `evadb-0.2.0/eva/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/drop_statement.py` & `evadb-0.2.0/eva/parser/drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/drop_udf_statement.py` & `evadb-0.2.0/eva/parser/drop_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/eva.lark` & `evadb-0.2.0/eva/parser/eva.lark`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 create_table: CREATE TABLE if_not_exists? table_name create_definitions 
     
 // Rename statements
 
 rename_table: RENAME TABLE table_name TO table_name
     
 // Create UDFs
-create_udf: CREATE UDF if_not_exists? udf_name INPUT create_definitions OUTPUT create_definitions TYPE udf_type IMPL udf_impl udf_metadata* | CREATE UDF if_not_exists? udf_name IMPL udf_impl udf_metadata*
+create_udf: CREATE UDF if_not_exists? udf_name INPUT create_definitions OUTPUT create_definitions TYPE udf_type IMPL udf_impl udf_metadata* | CREATE UDF if_not_exists? udf_name IMPL udf_impl udf_metadata* | CREATE UDF if_not_exists? udf_name TYPE udf_type udf_metadata*
 
 // Create Materialized View
 create_materialized_view: CREATE MATERIALIZED VIEW if_not_exists? table_name ("(" uid_list ")") AS select_statement 
 
 // Details
 udf_name: uid
```

### Comparing `evadb-0.1.6/eva/parser/explain_statement.py` & `evadb-0.2.0/eva/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/insert_statement.py` & `evadb-0.2.0/eva/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_parser.py` & `evadb-0.2.0/eva/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.0/eva/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.0/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.0/eva/parser/lark_visitor/_create_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.0/eva/parser/lark_visitor/_expressions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.0/eva/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.0/eva/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.0/eva/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.0/eva/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.0/eva/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/load_statement.py` & `evadb-0.2.0/eva/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/parser.py` & `evadb-0.2.0/eva/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/rename_statement.py` & `evadb-0.2.0/eva/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/select_statement.py` & `evadb-0.2.0/eva/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/show_statement.py` & `evadb-0.2.0/eva/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/statement.py` & `evadb-0.2.0/eva/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/table_ref.py` & `evadb-0.2.0/eva/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/parser/types.py` & `evadb-0.2.0/eva/parser/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/__init__.py` & `evadb-0.2.0/eva/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.0/eva/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.0/eva/plan_nodes/abstract_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,28 +88,36 @@
         for k, v in self.__dict__.items():
             if k == "_children":
                 setattr(result, k, [])
             else:
                 setattr(result, k, v)
         return result
 
-    def bfs(self):
-        """Returns a generator which visits all nodes in plan tree in
-        breadth-first search (BFS) traversal order.
-
-        Returns:
-            the generator object.
+    def walk(self, bfs=True):
+        """
+        Returns a generator which visits all nodes in physical plan tree.
         """
+        if bfs:
+            yield from self.bfs()
+        else:
+            yield from self.dfs()
+
+    def bfs(self):
         queue = deque([self])
         while queue:
             node = queue.popleft()
             yield node
             for child in node.children:
                 queue.append(child)
 
+    def dfs(self):
+        yield self
+        for child in self.children:
+            yield from child.dfs()
+
     def find_all(self, plan_type: Any):
         """Returns a generator which visits all the nodes in plan tree and yields one
         that matches the passed `expression_type`.
 
         Args:
             plan_type (Any): plan type to match with
```

### Comparing `evadb-0.1.6/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.0/eva/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.0/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.0/eva/plan_nodes/create_index_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.0/eva/plan_nodes/create_mat_view_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/create_plan.py` & `evadb-0.2.0/eva/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.0/eva/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/delete_plan.py` & `evadb-0.2.0/eva/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/drop_plan.py` & `evadb-0.2.0/eva/plan_nodes/drop_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.0/eva/plan_nodes/drop_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/explain_plan.py` & `evadb-0.2.0/eva/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/faiss_index_scan_plan.py` & `evadb-0.2.0/eva/plan_nodes/faiss_index_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.0/eva/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.0/eva/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.0/eva/plan_nodes/hash_join_build_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.0/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/insert_plan.py` & `evadb-0.2.0/eva/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.0/eva/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/limit_plan.py` & `evadb-0.2.0/eva/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.0/eva/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.0/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.0/eva/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/pp_plan.py` & `evadb-0.2.0/eva/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.0/eva/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/project_plan.py` & `evadb-0.2.0/eva/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/rename_plan.py` & `evadb-0.2.0/eva/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/sample_plan.py` & `evadb-0.2.0/eva/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.0/eva/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.0/eva/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/storage_plan.py` & `evadb-0.2.0/eva/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/types.py` & `evadb-0.2.0/eva/plan_nodes/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/plan_nodes/union_plan.py` & `evadb-0.2.0/eva/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/__init__.py` & `evadb-0.2.0/eva/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/abstract_reader.py` & `evadb-0.2.0/eva/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/csv_reader.py` & `evadb-0.2.0/eva/readers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/decord_reader.py` & `evadb-0.2.0/eva/readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/image/__init__.py` & `evadb-0.2.0/eva/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.0/eva/readers/image/opencv_image_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/server/__init__.py` & `evadb-0.2.0/eva/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/server/command_handler.py` & `evadb-0.2.0/eva/server/command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/server/db_api.py` & `evadb-0.2.0/eva/server/db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/server/interpreter.py` & `evadb-0.2.0/eva/server/interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/server/server.py` & `evadb-0.2.0/eva/server/server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/__init__.py` & `evadb-0.2.0/eva/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.0/eva/storage/abstract_media_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/abstract_storage_engine.py` & `evadb-0.2.0/eva/storage/abstract_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/image_storage_engine.py` & `evadb-0.2.0/eva/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.0/eva/storage/sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/storage_engine.py` & `evadb-0.2.0/eva/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/storage/video_storage_engine.py` & `evadb-0.2.0/eva/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/__init__.py` & `evadb-0.2.0/eva/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/abstract/__init__.py` & `evadb-0.2.0/eva/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.0/eva/udfs/abstract/abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.0/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/asl_action_recognition.py` & `evadb-0.2.0/eva/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/__init__.py` & `evadb-0.2.0/eva/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/decorators.py` & `evadb-0.2.0/eva/udfs/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.0/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.0/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.0/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/utils.py` & `evadb-0.2.0/eva/udfs/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/decorators/yolo_object_detection_decorators.py` & `evadb-0.2.0/eva/udfs/decorators/yolo_object_detection_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/emotion_detector.py` & `evadb-0.2.0/eva/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/face_detector.py` & `evadb-0.2.0/eva/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.0/eva/udfs/fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/feature_extractor.py` & `evadb-0.2.0/eva/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/gpu_compatible.py` & `evadb-0.2.0/eva/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.0/eva/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/__init__.py` & `evadb-0.2.0/eva/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/array_count.py` & `evadb-0.2.0/eva/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/crop.py` & `evadb-0.2.0/eva/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.0/eva/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/open.py` & `evadb-0.2.0/eva/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ndarray/similarity.py` & `evadb-0.2.0/eva/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/ocr_extractor.py` & `evadb-0.2.0/eva/udfs/ocr_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/toxicity_classifier.py` & `evadb-0.2.0/eva/udfs/toxicity_classifier.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.0/eva/udfs/udf_bootstrap_queries.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/udfs/yolo_object_detector.py` & `evadb-0.2.0/eva/udfs/yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/__init__.py` & `evadb-0.2.0/eva/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/errors.py` & `evadb-0.2.0/eva/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/generic_utils.py` & `evadb-0.2.0/eva/utils/generic_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,37 @@
         import torch
 
         return torch.cuda.is_available()
     except ImportError:
         return False
 
 
+def prefix_worker_id_to_path(path: str):
+    try:
+        worker_id = os.environ["PYTEST_XDIST_WORKER"]
+        base = "eva_datasets"
+        path = "build/" + str(worker_id) + "_" + base
+    except KeyError:
+        # Single threaded mode
+        pass
+    return path
+
+
+def get_gpu_count() -> int:
+    """
+    Check number of GPUs through Torch.
+    """
+    try:
+        import torch
+
+        return torch.cuda.device_count()
+    except ImportError:
+        return 0
+
+
 def generate_file_path(name: str = "") -> Path:
     """Generates a arbitrary file_path(md5 hash) based on the a random salt
     and name
 
     Arguments:
         name (str): Input file_name.
 
@@ -118,14 +141,15 @@
 
     """
     dataset_location = ConfigurationManager().get_value("core", "datasets_dir")
     if dataset_location is None:
         logger.error("Missing dataset location key in eva.yml")
         raise KeyError("Missing datasets_dir key in eva.yml")
 
+    dataset_location = prefix_worker_id_to_path(dataset_location)
     dataset_location = Path(dataset_location)
     dataset_location.mkdir(parents=True, exist_ok=True)
 
     salt = uuid.uuid4().hex
     file_name = hashlib.md5(salt.encode() + name.encode()).hexdigest()
     path = dataset_location / file_name
     return path.resolve()
```

### Comparing `evadb-0.1.6/eva/utils/kv_cache.py` & `evadb-0.2.0/eva/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/logging_manager.py` & `evadb-0.2.0/eva/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/s3_utils.py` & `evadb-0.2.0/eva/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/utils/stats.py` & `evadb-0.2.0/eva/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/eva/version.py` & `evadb-0.2.0/eva/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 _MAJOR = "0"
-_MINOR = "1"
-_REVISION = "6"
+_MINOR = "2"
+_REVISION = "0"
 
 VERSION_SHORT = f"{_MAJOR}.{_MINOR}"
 VERSION = f"{_MAJOR}.{_MINOR}.{_REVISION}"
```

### Comparing `evadb-0.1.6/evadb.egg-info/PKG-INFO` & `evadb-0.2.0/evadb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,207 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.1.6
+Version: 0.2.0
 Summary: EVA Video Database System (Think MySQL for videos).
 Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: georgia.tech.db@gmail.com
 License: Apache License 2.0
+Download-URL: https://github.com/georgia-tech-db/eva
+Description: <div >
+          <a href="https://evadb.readthedocs.io/">
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
+          </a>
+          <div>
+                <h3>Try It Out!</h3>
+                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+                </a>
+                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+                </a>    
+                <a href="https://github.com/georgia-tech-db/eva/discussions">
+                    <img alt="Discuss on Github!" src="https://img.shields.io/badge/-Discuss%20on%20Github!-blueviolet">
+                </a>
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
+            </div>
+        </div>
+        
+        # EVA AI-Relational Database System
+        
+        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
+        
+        EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
+        
+        EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
+        
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
+         * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
+         * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+         
+        If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
+        
+        The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
+        
+        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
+        
+        ## Why EVA? ##
+        
+        <details>
+          <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
+          Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
+        </details>
+        
+        <details>
+          <summary><b>Speed up queries and save money spent on model inference</b></summary>
+          EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
+        </details>
+        
+        <details>
+          <summary><b>Extensible by design to support custom deep learning models </b></summary>
+          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
+        </details>
+        
+        ## Links
+        * [Documentation](https://evadb.readthedocs.io/)
+        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        * [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+        * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
+        
+        ## Quick Start
+        
+        1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
+        
+        ```shell
+        pip install evadb
+        ```
+        
+        2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
+        ```shell
+        eva_server &   # launch server
+        eva_client     # launch client
+        ```
+        
+        3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
+        
+        ```mysql
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
+        ```
+        
+        4. That's it! You can now run queries over the loaded video:
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE id < 5;
+        ```
+        
+        5. Search for frames in the video that contain a car
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
+        ```
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        6. Search for frames in the video that contain a pedestrian and a car
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
+        ```
+        
+        7. Search for frames in the video with more than 3 cars
+        
+        ```mysql
+        SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
+        ```
+        
+        8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
+        ```mysql
+        CREATE UDF IF NOT EXISTS MyUDF
+        INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
+        OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
+                scores NDARRAY FLOAT32(ANYDIM))
+        TYPE  Classification
+        IMPL  'eva/udfs/fastrcnn_object_detector.py';
+        ```
+        
+        9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
+        ```mysql
+           -- Analyse emotions of faces in a video
+           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+           FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+           WHERE id < 15;
+        ```
+        
+        ## Illustrative EVA Applications 
+        
+        ### Traffic Analysis (Object Detection Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        ### MNIST Digit Recognition (Image Classification Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+        
+        ### Movie Analysis (Face Detection + Emotion Classfication Models)
+        
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+        
+        ### [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+        
+        ### [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
+        
+        ## Community
+        
+        Join the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for improving EVA.
+        
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+        </a>
+        
+        ### Architecture Diagram of EVA
+        
+        <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-arch.png" alt="EVA Architecture Diagram" width="500">
+        
+        ## Contributing to EVA
+        
+        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+        [![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
+        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
+        
+        We welcome all kinds of contributions to EVA.
+        To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        
+        For more information on contributing to EVA, see our
+        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+        
+        ## License
+        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
+        Licensed under [Apache License](LICENSE).
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-<div >
-  <a href="https://evadb.readthedocs.io/">
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-  </a>
-  <div>
-        <h3>Try It Out!</h3>
-        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
-        </a>
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-        </a>    
-        <a href="https://github.com/georgia-tech-db/eva/discussions">
-            <img alt="Discuss on Github!" src="https://img.shields.io/badge/-Discuss%20on%20Github!-blueviolet">
-        </a>
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
-    </div>
-</div>
-
-# EVA AI-Relational Database System
-
-EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
-
-EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
-
-EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
-
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
- * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
- * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
- 
-If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
-
-The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
-
-The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
-
-## Why EVA? ##
-
-<details>
-  <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
-  Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
-</details>
-
-<details>
-  <summary><b>Speed up queries and save money spent on model inference</b></summary>
-  EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
-</details>
-
-<details>
-  <summary><b>Extensible by design to support custom deep learning models </b></summary>
-  EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
-</details>
-
-## Links
-* [Documentation](https://evadb.readthedocs.io/)
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-* [Demo](https://ada-00.cc.gatech.edu/eva/playground)
-
-## Quick Start
-
-1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
-
-```shell
-pip install evadb
-```
-
-2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
-```shell
-eva_server &   # launch server
-eva_client     # launch client
-```
-
-3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
-
-```mysql
-LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
-```
-
-4. That's it! You can now run queries over the loaded video:
-
-```mysql
-SELECT id, data FROM MyVideo WHERE id < 5;
-```
-
-5. Search for frames in the video that contain a car
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
-```
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-6. Search for frames in the video that contain a pedestrian and a car
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
-```
-
-7. Search for frames in the video with more than 3 cars
-
-```mysql
-SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
-```
-
-8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
-```mysql
-CREATE UDF IF NOT EXISTS MyUDF
-INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
-OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
-        scores NDARRAY FLOAT32(ANYDIM))
-TYPE  Classification
-IMPL  'eva/udfs/fastrcnn_object_detector.py';
-```
-
-9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
-```mysql
-   -- Analyse emotions of faces in a video
-   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-   FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-   WHERE id < 15;
-```
-
-## Illustrative EVA Applications 
-
-### Traffic Analysis (Object Detection Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-### MNIST Digit Recognition (Image Classification Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-
-### Movie Analysis (Face Detection + Emotion Classfication Models)
-
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-
-### [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-
-### [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-
-## Community
-
-Join the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for improving EVA.
-
-<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
-</a>
-
-### Architecture Diagram of EVA
-
-<img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-arch.png" alt="EVA Architecture Diagram" width="500">
-
-## Contributing to EVA
-
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-[![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-
-We welcome all kinds of contributions to EVA.
-To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-
-For more information on contributing to EVA, see our
-[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-
-## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
-Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,17 +1,12 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.1.6 Summary: EVA Video Database
+Metadata-Version: 2.1 Name: evadb Version: 0.2.0 Summary: EVA Video Database
 System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
-eva Download-URL: https://github.com/georgia-tech-db/eva Author: Georgia Tech
-Database Group Author-email: georgia.tech.db@gmail.com License: Apache License
-2.0 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3 Classifier: Development Status :: 3 - Alpha Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE.txt
+eva Author: Georgia Tech Database Group Author-email: georgia.tech.db@gmail.com
+License: Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/
+eva Description:
 [EVA]
 **** Try It Out! ****
 [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
 Versions]
 # EVA AI-Relational Database System EVA is an open-source **AI-relational
 database with first-class support for deep learning models**. It aims to
 support AI-powered database applications that operate on both structured
@@ -99,8 +94,14 @@
 eva?branch=master) [![Documentation Status](https://readthedocs.org/projects/
 evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
 index.html) We welcome all kinds of contributions to EVA. To file a bug or
 request a feature, please use GitHub_issues. Pull_requests are welcome. For
 more information on contributing to EVA, see our [contribution guide](https://
 evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
 Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/
-) Licensed under [Apache License](LICENSE).
+) Licensed under [Apache License](LICENSE). Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Information Analysis Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `evadb-0.1.6/evadb.egg-info/SOURCES.txt` & `evadb-0.2.0/evadb.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -143,14 +143,18 @@
 eva/parser/parser.py
 eva/parser/rename_statement.py
 eva/parser/select_statement.py
 eva/parser/show_statement.py
 eva/parser/statement.py
 eva/parser/table_ref.py
 eva/parser/types.py
+eva/parser/evaql/evaql_lexer.py
+eva/parser/evaql/evaql_parser.py
+eva/parser/evaql/evaql_parserListener.py
+eva/parser/evaql/evaql_parserVisitor.py
 eva/parser/lark_visitor/__init__.py
 eva/parser/lark_visitor/_common_clauses_ids.py
 eva/parser/lark_visitor/_create_statements.py
 eva/parser/lark_visitor/_delete_statement.py
 eva/parser/lark_visitor/_drop_statement.py
 eva/parser/lark_visitor/_explain_statement.py
 eva/parser/lark_visitor/_expressions.py
@@ -209,28 +213,34 @@
 eva/storage/__init__.py
 eva/storage/abstract_media_storage_engine.py
 eva/storage/abstract_storage_engine.py
 eva/storage/image_storage_engine.py
 eva/storage/sqlite_storage_engine.py
 eva/storage/storage_engine.py
 eva/storage/video_storage_engine.py
+eva/third_party/__init__.py
+eva/third_party/huggingface/__init__.py
+eva/third_party/huggingface/binder.py
+eva/third_party/huggingface/create.py
+eva/third_party/huggingface/model.py
 eva/udfs/__init__.py
 eva/udfs/asl_action_recognition.py
 eva/udfs/emotion_detector.py
 eva/udfs/face_detector.py
 eva/udfs/fastrcnn_object_detector.py
 eva/udfs/feature_extractor.py
 eva/udfs/gpu_compatible.py
 eva/udfs/mvit_action_recognition.py
 eva/udfs/ocr_extractor.py
 eva/udfs/toxicity_classifier.py
 eva/udfs/udf_bootstrap_queries.py
 eva/udfs/yolo_object_detector.py
 eva/udfs/abstract/__init__.py
 eva/udfs/abstract/abstract_udf.py
+eva/udfs/abstract/hf_abstract_udf.py
 eva/udfs/abstract/pytorch_abstract_udf.py
 eva/udfs/decorators/__init__.py
 eva/udfs/decorators/decorators.py
 eva/udfs/decorators/utils.py
 eva/udfs/decorators/yolo_object_detection_decorators.py
 eva/udfs/decorators/io_descriptors/__init__.py
 eva/udfs/decorators/io_descriptors/abstract_types.py
@@ -303,23 +313,24 @@
 test/expression/test_aggregation.py
 test/expression/test_arithmetic.py
 test/expression/test_comparison.py
 test/expression/test_expression_tree.py
 test/expression/test_expression_utils.py
 test/expression/test_function_expression.py
 test/expression/test_logical.py
-test/expression/test_tuple_value.py
 test/integration_tests/__init__.py
 test/integration_tests/test_array_count.py
 test/integration_tests/test_create_index_executor.py
 test/integration_tests/test_create_table_executor.py
 test/integration_tests/test_delete_executor.py
 test/integration_tests/test_drop_executor.py
+test/integration_tests/test_error_handling_with_ray.py
 test/integration_tests/test_explain_executor.py
 test/integration_tests/test_fuzzy_join.py
+test/integration_tests/test_huggingface_udfs.py
 test/integration_tests/test_insert_executor.py
 test/integration_tests/test_like.py
 test/integration_tests/test_load_executor.py
 test/integration_tests/test_mat_executor.py
 test/integration_tests/test_open.py
 test/integration_tests/test_optimizer_rules.py
 test/integration_tests/test_pytorch.py
@@ -376,8 +387,9 @@
 test/udfs/ndarray/__init__.py
 test/udfs/ndarray/test_array_count.py
 test/udfs/ndarray/test_crop.py
 test/udfs/ndarray/test_open.py
 test/utils/__init__.py
 test/utils/test_generic_utils.py
 test/utils/test_timer.py
+test/utils/test_xdist.py
 third_party/__init__.py
```

### Comparing `evadb-0.1.6/evadb.egg-info/requires.txt` & `evadb-0.2.0/evadb.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-numpy<=1.23.5,>=1.19.5
-opencv-python<4.6.0.66,>=4.5.4.60
-pandas>=1.1.5
 Pillow>=8.4.0
-sqlalchemy<2.0.0,>=1.4.0
-sqlalchemy-utils>=0.36.6
-lark>=1.0.0
-pyyaml>=5.1
-importlib-metadata<5.0
-ray>=1.13.0
 aenum>=2.2.0
+detoxify
 diskcache>=5.4.0
-decord>=0.6.0
-torch>=1.10.0
-torchvision>=0.11.1
-faiss-cpu
-facenet-pytorch>=2.5.2
 easyocr>=1.5.0
+eva-decord==0.6.0
+facenet-pytorch>=2.5.2
+faiss-cpu
+importlib-metadata<5.0
 ipython
-yolov5<=7.0.6
-detoxify
-thefuzz
-
-[dev]
+lark>=1.0.0
 numpy<=1.23.5,>=1.19.5
 opencv-python<4.6.0.66,>=4.5.4.60
 pandas>=1.1.5
-Pillow>=8.4.0
-sqlalchemy<2.0.0,>=1.4.0
-sqlalchemy-utils>=0.36.6
-lark>=1.0.0
 pyyaml>=5.1
-importlib-metadata<5.0
 ray>=1.13.0
-aenum>=2.2.0
-diskcache>=5.4.0
-decord>=0.6.0
+sqlalchemy-utils>=0.36.6
+sqlalchemy<2.0.0,>=1.4.0
+thefuzz
 torch>=1.10.0
 torchvision>=0.11.1
-faiss-cpu
-facenet-pytorch>=2.5.2
-easyocr>=1.5.0
-ipython
+transformers==4.27.4
 yolov5<=7.0.6
-detoxify
-thefuzz
+
+[dev]
+Pillow>=8.4.0
+aenum>=2.2.0
 black>=23.1.0
-isort>=5.10.1
-pytest>=6.1.2
-pytest-cov>=2.11.1
-pytest-random-order>=1.0.4
-pytest-virtualenv
-pytest-asyncio
-pytest-xdist
 coveralls>=3.0.1
+detoxify
+diskcache>=5.4.0
+easyocr>=1.5.0
+eva-decord==0.6.0
+facenet-pytorch>=2.5.2
+faiss-cpu
 flake8>=3.9.1
-moto[s3]>=4.1.1
+importlib-metadata<5.0
+ipython
 ipywidgets>=7.7.2
+isort>=5.10.1
+lark>=1.0.0
 matplotlib>=3.3.4
+moto[s3]>=4.1.1
 nbmake>=1.2.1
 nest-asyncio>=1.5.6
-pytest-benchmark
+numpy<=1.23.5,>=1.19.5
+opencv-python<4.6.0.66,>=4.5.4.60
+pandas>=1.1.5
 pymysql>=0.10.1
-wheel>=0.37.1
+pytest-asyncio
+pytest-benchmark
+pytest-cov>=2.11.1
+pytest-random-order>=1.0.4
+pytest-virtualenv
+pytest-xdist
+pytest>=6.1.2
+pyyaml>=5.1
+ray>=1.13.0
 scriv>=0.16.0
+sqlalchemy-utils>=0.36.6
+sqlalchemy<2.0.0,>=1.4.0
+thefuzz
+torch>=1.10.0
+torchvision>=0.11.1
+transformers==4.27.4
+wheel>=0.37.1
+yolov5<=7.0.6
```

### Comparing `evadb-0.1.6/setup.py` & `evadb-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "importlib-metadata<5.0",
     "ray>=1.13.0",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
-    "decord>=0.6.0",
+    "eva-decord==0.6.0"
 ]
 
 formatter_libs = ["black>=23.1.0", "isort>=5.10.1"]
 
 test_libs = [
     "pytest>=6.1.2",
     "pytest-cov>=2.11.1",
@@ -92,17 +92,18 @@
 database_libs = ["pymysql>=0.10.1"]
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
     "easyocr>=1.5.0",  # OCR EXTRACTION
     "ipython",
-    "yolov5<=7.0.6",  # OBJECT DETECTION
-    "detoxify",  # TEXT TOXICITY CLASSIFICATION
-    "thefuzz",  # FUZZY STRING MATCHINGz
+    "yolov5<=7.0.6",          # OBJECT DETECTION
+    "detoxify",               # TEXT TOXICITY CLASSIFICATION
+    "thefuzz",                # FUZZY STRING MATCHINGz
+    "transformers==4.27.4"    # HUGGINGFACE
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 experimental_libs = []
 
 INSTALL_REQUIRES = minimal_requirement + integration_test_libs + udf_libs
 DEV_REQUIRES = (
```

### Comparing `evadb-0.1.6/test/__init__.py` & `evadb-0.2.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/benchmark_tests/__init__.py` & `evadb-0.2.0/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/benchmark_tests/conftest.py` & `evadb-0.2.0/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.0/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/binder/__init__.py` & `evadb-0.2.0/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/binder/test_binder_utils.py` & `evadb-0.2.0/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/binder/test_statement_binder.py` & `evadb-0.2.0/test/binder/test_statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/binder/test_statement_binder_context.py` & `evadb-0.2.0/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/binder/test_statement_binder_python37.py` & `evadb-0.2.0/test/binder/test_statement_binder_python37.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/__init__.py` & `evadb-0.2.0/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/models/__init__.py` & `evadb-0.2.0/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/models/test_models.py` & `evadb-0.2.0/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/__init__.py` & `evadb-0.2.0/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_index_catalog_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 from unittest import TestCase
 
 import pytest
 from mock import MagicMock, patch
 from sqlalchemy.orm.exc import NoResultFound
 
+from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import ColumnType, IndexType
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 from eva.catalog.services.index_catalog_service import IndexCatalogService
 
 INDEX_NAME = "name"
 INDEX_ID = 123
 
@@ -94,14 +95,15 @@
         self.assertEqual(service.get_entry_by_name(MagicMock()), None)
 
         self.assertEqual(service.get_entry_by_id(MagicMock()), None)
 
         self.assertEqual(service.get_all_entries(), [])
 
     def test_index_get_all_entries(self):
+        CatalogManager().reset()
         INDEX_NAME = "name"
         INDEX_URL = "file1"
         INDEX_TYPE = IndexType.HNSW
         FEAT_COLUMN = ColumnCatalogEntry("abc", ColumnType.INTEGER)
 
         service = IndexCatalogService()
```

### Comparing `evadb-0.1.6/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.0/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/test_catalog_manager.py` & `evadb-0.2.0/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/test_column_type.py` & `evadb-0.2.0/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/catalog/test_sqlalchemy.py` & `evadb-0.2.0/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/configuration/__init__.py` & `evadb-0.2.0/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.0/test/configuration/test_bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/configuration/test_configuration_manager.py` & `evadb-0.2.0/test/configuration/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/__init__.py` & `evadb-0.2.0/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_abstract_executor.py` & `evadb-0.2.0/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_create_mat_executor.py` & `evadb-0.2.0/test/executor/test_create_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_create_udf_executor.py` & `evadb-0.2.0/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_execution_context.py` & `evadb-0.2.0/test/executor/test_execution_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,126 +18,89 @@
 
 from eva.constants import NO_GPU
 from eva.executor.execution_context import Context
 
 
 class ExecutionContextTest(unittest.TestCase):
     @patch("eva.executor.execution_context.ConfigurationManager")
-    @patch("eva.executor.execution_context.socket")
+    @patch("eva.executor.execution_context.get_gpu_count")
     @patch("eva.executor.execution_context.is_gpu_available")
-    def test_gpu_devices_gets_populated_from_config(self, gpu_check, socket, cfm):
+    def test_CUDA_VISIBLE_DEVICES_gets_populated_from_config(
+        self, gpu_check, get_gpu_count, cfm
+    ):
         gpu_check.return_value = True
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = {"address2": ["0", "1", "2"]}
+        get_gpu_count.return_value = 3
+        cfm.return_value.get_value.return_value = [0, 1]
         context = Context()
 
-        self.assertEqual(context.gpus, ["0", "1", "2"])
+        self.assertEqual(context.gpus, [0, 1])
 
     @patch("eva.executor.execution_context.ConfigurationManager")
     @patch("eva.executor.execution_context.os")
-    @patch("eva.executor.execution_context.socket")
+    @patch("eva.executor.execution_context.get_gpu_count")
     @patch("eva.executor.execution_context.is_gpu_available")
-    def test_gpu_devices_gets_populated_from_environment_if_no_config(
-        self, is_gpu, socket, os, cfm
+    def test_CUDA_VISIBLE_DEVICES_gets_populated_from_environment_if_no_config(
+        self, is_gpu, get_gpu_count, os, cfm
     ):
         is_gpu.return_value = True
-
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = {"address3": ["0", "1", "2"]}
-        os.environ.get.return_value = "0,1,2"
+        cfm.return_value.get_value.return_value = []
+        get_gpu_count.return_value = 3
+        os.environ.get.return_value = "0,1"
         context = Context()
-        os.environ.get.assert_called_with("GPU_DEVICES", "")
+        os.environ.get.assert_called_with("CUDA_VISIBLE_DEVICES", "")
 
-        self.assertEqual(context.gpus, ["0", "1", "2"])
+        self.assertEqual(context.gpus, [0, 1])
 
     @patch("eva.executor.execution_context.ConfigurationManager")
     @patch("eva.executor.execution_context.os")
-    @patch("eva.executor.execution_context.socket")
+    @patch("eva.executor.execution_context.get_gpu_count")
     @patch("eva.executor.execution_context.is_gpu_available")
-    def test_gpu_devices_should_be_empty_if_nothing_provided(
-        self, gpu_check, socket, os, cfm
+    def test_CUDA_VISIBLE_DEVICES_should_be_empty_if_nothing_provided(
+        self, gpu_check, get_gpu_count, os, cfm
     ):
         gpu_check.return_value = True
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = {"address3": ["0", "1", "2"]}
+        get_gpu_count.return_value = 3
+        cfm.return_value.get_value.return_value = []
         os.environ.get.return_value = ""
         context = Context()
-        os.environ.get.assert_called_with("GPU_DEVICES", "")
+        os.environ.get.assert_called_with("CUDA_VISIBLE_DEVICES", "")
 
         self.assertEqual(context.gpus, [])
 
     @patch("eva.executor.execution_context.ConfigurationManager")
     @patch("eva.executor.execution_context.os")
-    @patch("eva.executor.execution_context.socket")
     @patch("eva.executor.execution_context.is_gpu_available")
-    def test_gpus_ignores_config_if_no_gpu_available(self, gpu_check, socket, os, cfm):
+    def test_gpus_ignores_config_if_no_gpu_available(self, gpu_check, os, cfm):
         gpu_check.return_value = False
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = {"address3": ["0", "1", "2"]}
+        cfm.return_value.get_value.return_value = [0, 1, 2]
         os.environ.get.return_value = "0,1,2"
         context = Context()
 
         self.assertEqual(context.gpus, [])
 
     @patch("eva.executor.execution_context.ConfigurationManager")
     @patch("eva.executor.execution_context.os")
-    @patch("eva.executor.execution_context.socket")
     @patch("eva.executor.execution_context.is_gpu_available")
     def test_gpu_device_should_return_NO_GPU_if_GPU_not_available(
-        self, gpu_check, socket, os, cfm
+        self, gpu_check, os, cfm
     ):
         gpu_check.return_value = True
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = None
+        cfm.return_value.get_value.return_value = []
         os.environ.get.return_value = ""
         context = Context()
-        os.environ.get.assert_called_with("GPU_DEVICES", "")
+        os.environ.get.assert_called_with("CUDA_VISIBLE_DEVICES", "")
 
         self.assertEqual(context.gpu_device(), NO_GPU)
 
     @patch("eva.executor.execution_context.ConfigurationManager")
-    @patch("eva.executor.execution_context.socket")
+    @patch("eva.executor.execution_context.get_gpu_count")
     @patch("eva.executor.execution_context.is_gpu_available")
-    @patch("eva.executor.execution_context.random")
     def test_should_return_random_gpu_ID_if_available(
-        self, random, gpu_check, socket, cfm
+        self, gpu_check, get_gpu_count, cfm
     ):
-        random.choice.return_value = "2"
         gpu_check.return_value = True
-        socket.gethostname.return_value = "host"
-        socket.gethostbyaddr.return_value = (
-            "local",
-            ["another-hostname", "other-possible"],
-            ["address2"],
-        )
-        cfm.return_value.get_value.return_value = {"address2": ["0", "1", "2"]}
+        get_gpu_count.return_value = 1
+        cfm.return_value.get_value.return_value = [0, 1, 2]
         context = Context()
 
         selected_device = context.gpu_device()
-
-        random.choice.assert_called_with(context.gpus)
-        self.assertEqual(selected_device, "2")
+        self.assertEqual(selected_device, 0)
```

### Comparing `evadb-0.1.6/test/executor/test_executor_utils.py` & `evadb-0.2.0/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_limit_executor.py` & `evadb-0.2.0/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_load_executor.py` & `evadb-0.2.0/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_orderby_executor.py` & `evadb-0.2.0/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_plan_executor.py` & `evadb-0.2.0/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_pp_executor.py` & `evadb-0.2.0/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_sample_executor.py` & `evadb-0.2.0/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/executor/test_seq_scan_executor.py` & `evadb-0.2.0/test/executor/test_seq_scan_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         plan = type(
             "ScanPlan", (), {"predicate": expression, "columns": None, "alias": None}
         )
         predicate_executor = SequentialScanExecutor(plan)
         predicate_executor.append_child(DummyExecutor([batch]))
 
-        expected = Batch(batch[[2]].frames.reset_index(drop=True))
+        expected = Batch(batch[[2]].frames)
         filtered = list(predicate_executor.exec())[0]
         self.assertEqual(expected, filtered)
 
     def test_should_return_all_frames_when_no_predicate_is_applied(self):
         dataframe = create_dataframe(3)
 
         batch = Batch(frames=dataframe)
```

### Comparing `evadb-0.1.6/test/executor/utils.py` & `evadb-0.2.0/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/__init__.py` & `evadb-0.2.0/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_abstract_expression.py` & `evadb-0.2.0/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_aggregation.py` & `evadb-0.2.0/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_arithmetic.py` & `evadb-0.2.0/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_comparison.py` & `evadb-0.2.0/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_expression_tree.py` & `evadb-0.2.0/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_expression_utils.py` & `evadb-0.2.0/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_function_expression.py` & `evadb-0.2.0/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/expression/test_logical.py` & `evadb-0.2.0/test/expression/test_logical.py`

 * *Files 26% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             ExpressionType.LOGICAL_AND, comp_exp_l, comp_exp_r
         )
 
         tuples = Batch(pd.DataFrame({0: [1, 2, 3, 4], 1: [1, 2, 5, 6]}))
         self.assertEqual(
             [True, False, False, False], logical_exp.evaluate(tuples).frames[0].tolist()
         )
-        comp_exp_r.evaluate.assert_called_once_with(tuples, mask=[0, 1])
+        comp_exp_r.evaluate.assert_called_once_with(tuples[[0, 1]])
 
     def test_short_circuiting_or_partial(self):
         # tests whether right-hand side is partially executed with or
         tup_val_exp_l = TupleValueExpression(col_name=0)
         tup_val_exp_l.col_alias = 0
         tup_val_exp_r = TupleValueExpression(col_name=1)
         tup_val_exp_r.col_alias = 1
@@ -165,8 +165,88 @@
             ExpressionType.LOGICAL_OR, comp_exp_l, comp_exp_r
         )
 
         tuples = Batch(pd.DataFrame({0: [1, 2, 3, 4], 1: [5, 6, 3, 4]}))
         self.assertEqual(
             [True, False, True, True], logical_exp.evaluate(tuples).frames[0].tolist()
         )
-        comp_exp_r.evaluate.assert_called_once_with(tuples, mask=[0, 1])
+        comp_exp_r.evaluate.assert_called_once_with(tuples[[0, 1]])
+
+    def test_multiple_logical(self):
+        batch = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+
+        # col > 1
+        comp_left = ComparisonExpression(
+            ExpressionType.COMPARE_GREATER,
+            TupleValueExpression(col_alias="col"),
+            ConstantValueExpression(1),
+        )
+
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[list(range(2, 10))]
+        batch_copy.drop_zero(comp_left.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # col < 8
+        comp_right = ComparisonExpression(
+            ExpressionType.COMPARE_LESSER,
+            TupleValueExpression(col_alias="col"),
+            ConstantValueExpression(8),
+        )
+
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[list(range(0, 8))]
+        batch_copy.drop_zero(comp_right.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # col >= 5
+        comp_expr = ComparisonExpression(
+            ExpressionType.COMPARE_GEQ,
+            TupleValueExpression(col_alias="col"),
+            ConstantValueExpression(5),
+        )
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[list(range(5, 10))]
+        batch_copy.drop_zero(comp_expr.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # (col >= 5)  AND (col > 1 AND col < 8)
+        l_expr = LogicalExpression(ExpressionType.LOGICAL_AND, comp_left, comp_right)
+        root_l_expr = LogicalExpression(ExpressionType.LOGICAL_AND, comp_expr, l_expr)
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[[5, 6, 7]]
+        batch_copy.drop_zero(root_l_expr.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # (col > 1 AND col < 8) AND (col >= 5)
+        root_l_expr = LogicalExpression(ExpressionType.LOGICAL_AND, l_expr, comp_expr)
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[[5, 6, 7]]
+        batch_copy.drop_zero(root_l_expr.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # (col >=4 AND col <= 7) AND (col > 1 AND col < 8)
+        between_4_7 = LogicalExpression(
+            ExpressionType.LOGICAL_AND,
+            ComparisonExpression(
+                ExpressionType.COMPARE_GEQ,
+                TupleValueExpression(col_alias="col"),
+                ConstantValueExpression(4),
+            ),
+            ComparisonExpression(
+                ExpressionType.COMPARE_LEQ,
+                TupleValueExpression(col_alias="col"),
+                ConstantValueExpression(7),
+            ),
+        )
+        test_expr = LogicalExpression(ExpressionType.LOGICAL_AND, between_4_7, l_expr)
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[[4, 5, 6, 7]]
+        batch_copy.drop_zero(test_expr.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
+
+        # (col >=4 AND col <= 7) OR (col > 1 AND col < 8)
+        test_expr = LogicalExpression(ExpressionType.LOGICAL_OR, between_4_7, l_expr)
+        batch_copy = Batch(pd.DataFrame({"col": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}))
+        expected = batch[[2, 3, 4, 5, 6, 7]]
+        batch_copy.drop_zero(test_expr.evaluate(batch))
+        self.assertEqual(batch_copy, expected)
```

### Comparing `evadb-0.1.6/test/integration_tests/__init__.py` & `evadb-0.2.0/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/integration_tests/test_array_count.py` & `evadb-0.2.0/test/integration_tests/test_array_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 import unittest
 from test.util import (
     NUM_FRAMES,
     create_sample_video,
     file_remove,
     load_udfs_for_testing,
+    shutdown_ray,
 )
 
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.models.storage.batch import Batch
@@ -36,14 +37,15 @@
         video_file_path = create_sample_video(NUM_FRAMES)
         load_query = f"LOAD VIDEO '{video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(load_query)
         load_udfs_for_testing(mode="minimal")
 
     @classmethod
     def tearDownClass(cls):
+        shutdown_ray()
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         file_remove("dummy.avi")
 
     # integration test
 
     def test_should_load_and_select_using_udf_video(self):
         # Equality test
```

### Comparing `evadb-0.1.6/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.0/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.0/test/integration_tests/test_create_table_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/integration_tests/test_delete_executor.py` & `evadb-0.2.0/test/integration_tests/test_delete_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import file_remove, load_udfs_for_testing
+from test.util import file_remove, load_udfs_for_testing, shutdown_ray
 
 import numpy as np
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.configuration.constants import EVA_ROOT_DIR
@@ -66,14 +66,15 @@
         ####################################################
 
         path = f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4"
         query = f'LOAD VIDEO "{path}" INTO TestDeleteVideos;'
         _ = execute_query_fetch_all(query)
 
     def tearDown(self):
+        shutdown_ray()
         file_remove("dummy.avi")
 
     # integration test
     @unittest.skip("Not supported in current version")
     def test_should_delete_single_video_in_table(self):
         path = f"{EVA_ROOT_DIR}/data/sample_videos/1/2.mp4"
         delete_query = f"""DELETE FROM TestDeleteVideos WHERE name="{path}";"""
```

### Comparing `evadb-0.1.6/test/integration_tests/test_drop_executor.py` & `evadb-0.2.0/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/integration_tests/test_explain_executor.py` & `evadb-0.2.0/test/integration_tests/test_explain_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import (
-    create_sample_video,
-    create_table,
-    file_remove,
-    load_udfs_for_testing,
-)
+from test.util import create_sample_video, file_remove, load_udfs_for_testing
 
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.optimizer.plan_generator import PlanGenerator
 from eva.optimizer.rules.rules import (
@@ -41,48 +36,39 @@
     @classmethod
     def setUpClass(cls):
         CatalogManager().reset()
         video_file_path = create_sample_video(NUM_FRAMES)
         load_query = f"LOAD VIDEO '{video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(load_query)
         load_udfs_for_testing(mode="minimal")
-        cls.table1 = create_table("table1", 100, 3)
-        cls.table2 = create_table("table2", 500, 3)
-        cls.table3 = create_table("table3", 1000, 3)
 
     @classmethod
     def tearDownClass(cls):
         file_remove("dummy.avi")
-        drop_query = """DROP TABLE table1;"""
-        execute_query_fetch_all(drop_query)
-        drop_query = """DROP TABLE table2;"""
-        execute_query_fetch_all(drop_query)
-        drop_query = """DROP TABLE table3;"""
-        execute_query_fetch_all(drop_query)
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     def test_explain_simple_select(self):
         ray_enabled = ConfigurationManager().get_value("experimental", "ray")
         select_query = "EXPLAIN SELECT id, data FROM MyVideo"
         batch = execute_query_fetch_all(select_query)
         expected_output = (
-            """|__ SeqScanPlan\n    |__ ExchangePlan\n    |__ StoragePlan\n"""
+            """|__ ExchangePlan\n    |__ ProjectPlan\n        |__ SeqScanPlan\n            |__ ExchangePlan\n                |__ StoragePlan\n"""
             if ray_enabled
-            else """|__ SeqScanPlan\n    |__ StoragePlan\n"""
+            else """|__ ProjectPlan\n    |__ SeqScanPlan\n        |__ StoragePlan\n"""
         )
         self.assertEqual(batch.frames[0][0], expected_output)
 
         with disable_rules([XformLateralJoinToLinearFlow()]) as rules_manager:
             custom_plan_generator = PlanGenerator(rules_manager)
             select_query = "EXPLAIN SELECT id, data FROM MyVideo JOIN LATERAL DummyObjectDetector(data) AS T ;"
             batch = execute_query_fetch_all(
                 select_query, plan_generator=custom_plan_generator
             )
             expected_output = (
-                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n        |__ ExchangePlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
+                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
                 if ray_enabled
                 else """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
             )
             self.assertEqual(batch.frames[0][0], expected_output)
 
         # Disable more rules
         with disable_rules(
@@ -94,12 +80,12 @@
         ) as rules_manager:
             custom_plan_generator = PlanGenerator(rules_manager)
             select_query = "EXPLAIN SELECT id, data FROM MyVideo JOIN LATERAL DummyObjectDetector(data) AS T ;"
             batch = execute_query_fetch_all(
                 select_query, plan_generator=custom_plan_generator
             )
             expected_output = (
-                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n        |__ ExchangePlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
+                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
                 if ray_enabled
                 else """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
             )
             self.assertEqual(batch.frames[0][0], expected_output)
```

### Comparing `evadb-0.1.6/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.0/test/integration_tests/test_fuzzy_join.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from pathlib import Path
-from test.util import create_sample_csv, create_sample_video, file_remove
+from test.util import create_sample_csv, create_sample_video, file_remove, shutdown_ray
 
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.server.command_handler import execute_query_fetch_all
@@ -56,14 +56,16 @@
         execute_query_fetch_all(load_query)
 
         # load the video to be joined with the csv
         query = f"LOAD VIDEO '{self.video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(query)
 
     def tearDown(self):
+        shutdown_ray()
+
         file_remove("dummy.avi")
         file_remove("dummy.csv")
         # clean up
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideoCSV;")
 
     def test_fuzzyjoin(self):
```

### Comparing `evadb-0.1.6/test/integration_tests/test_insert_executor.py` & `evadb-0.2.0/test/integration_tests/test_insert_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import create_sample_video, file_remove, load_udfs_for_testing
+from test.util import (
+    create_sample_video,
+    file_remove,
+    load_udfs_for_testing,
+    shutdown_ray,
+)
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.server.command_handler import execute_query_fetch_all
@@ -36,14 +41,15 @@
                 name TEXT(100)
             );
         """
         execute_query_fetch_all(query)
         load_udfs_for_testing(mode="minimal")
 
     def tearDown(self):
+        shutdown_ray()
         file_remove("dummy.avi")
 
     # integration test
     @unittest.skip("Not supported in current version")
     def test_should_load_video_in_table(self):
         query = f"""LOAD VIDEO '{self.video_file_path}' INTO MyVideo;"""
         execute_query_fetch_all(query)
```

### Comparing `evadb-0.1.6/test/integration_tests/test_like.py` & `evadb-0.2.0/test/integration_tests/test_like.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
+from test.util import shutdown_ray
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.server.command_handler import execute_query_fetch_all
 
 
 class LikeTest(unittest.TestCase):
@@ -26,14 +27,15 @@
         meme1 = f"{EVA_ROOT_DIR}/data/detoxify/meme1.jpg"
         meme2 = f"{EVA_ROOT_DIR}/data/detoxify/meme2.jpg"
 
         execute_query_fetch_all(f"LOAD IMAGE '{meme1}' INTO MemeImages;")
         execute_query_fetch_all(f"LOAD IMAGE '{meme2}' INTO MemeImages;")
 
     def tearDown(self):
+        shutdown_ray()
         # clean up
         execute_query_fetch_all("DROP TABLE IF EXISTS MemeImages;")
 
     def test_like_with_ocr(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(10),
```

### Comparing `evadb-0.1.6/test/integration_tests/test_load_executor.py` & `evadb-0.2.0/test/integration_tests/test_load_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pathlib import Path
 from test.util import (
     create_dummy_batches,
     create_dummy_csv_batches,
     create_sample_csv,
     create_sample_video,
     file_remove,
+    shutdown_ray,
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.binder.binder_utils import BinderError
@@ -47,14 +48,16 @@
         self.video_file_path = create_sample_video()
         self.image_files_path = Path(
             f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/*.jpg"
         )
         self.csv_file_path = create_sample_csv()
 
     def tearDown(self):
+        shutdown_ray()
+
         file_remove("dummy.avi")
         file_remove("dummy.csv")
         # clean up
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideos;")
 
     # integration test for load video
     def test_should_load_video_in_table(self):
```

### Comparing `evadb-0.1.6/test/integration_tests/test_mat_executor.py` & `evadb-0.2.0/test/integration_tests/test_mat_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 import unittest
 from test.util import (
     DummyObjectDetector,
     create_sample_video,
     file_remove,
     load_udfs_for_testing,
+    shutdown_ray,
 )
 
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.constants import EVA_ROOT_DIR
@@ -42,14 +43,15 @@
         execute_query_fetch_all(load_query)
         ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(f"LOAD VIDEO '{ua_detrac}' INTO UATRAC;")
         load_udfs_for_testing()
 
     @classmethod
     def tearDownClass(cls):
+        shutdown_ray()
         file_remove("dummy.avi")
         file_remove("ua_detrac.mp4")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all("DROP TABLE UATRAC;")
 
     def test_should_mat_view_with_dummy(self):
         materialized_query = """CREATE MATERIALIZED VIEW dummy_view (id, label)
```

### Comparing `evadb-0.1.6/test/integration_tests/test_open.py` & `evadb-0.2.0/test/integration_tests/test_open.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import create_sample_image, file_remove, load_udfs_for_testing
+from test.util import (
+    create_sample_image,
+    file_remove,
+    load_udfs_for_testing,
+    shutdown_ray,
+)
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
@@ -43,14 +48,16 @@
         table_catalog_entry = CatalogManager().get_table_catalog_entry("testOpenTable")
         storage_engine = StorageEngine().factory(table_catalog_entry)
         storage_engine.write(
             table_catalog_entry, Batch(pd.DataFrame([{"num": 1}, {"num": 2}]))
         )
 
     def tearDown(self):
+        shutdown_ray()
+
         file_remove("dummy.jpg")
 
         # Drop table.
         drop_table_query = "DROP TABLE testOpenTable;"
         execute_query_fetch_all(drop_table_query)
 
     def test_open_should_open_image(self):
```

### Comparing `evadb-0.1.6/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.0/test/integration_tests/test_optimizer_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import get_physical_query_plan, load_udfs_for_testing
+from test.util import get_physical_query_plan, load_udfs_for_testing, shutdown_ray
 
 import pytest
 from mock import MagicMock, patch
 
 from eva.catalog.catalog_manager import CatalogManager
+from eva.configuration.configuration_manager import ConfigurationManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.expression.comparison_expression import ComparisonExpression
 from eva.optimizer.plan_generator import PlanGenerator
 from eva.optimizer.rules.rules import (
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
@@ -31,25 +32,30 @@
 from eva.optimizer.rules.rules_manager import disable_rules
 from eva.plan_nodes.predicate_plan import PredicatePlan
 from eva.server.command_handler import execute_query_fetch_all
 from eva.utils.stats import Timer
 
 
 @pytest.mark.notparallel
+@pytest.mark.skipif(
+    ConfigurationManager().get_value("experimental", "ray"),
+    reason="Not necessary for Ray",
+)
 class OptimizerRulesTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         CatalogManager().reset()
         ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(f"LOAD VIDEO '{ua_detrac}' INTO MyVideo;")
         execute_query_fetch_all(f"LOAD VIDEO '{ua_detrac}' INTO MyVideo2;")
         load_udfs_for_testing(mode="minimal")
 
     @classmethod
     def tearDownClass(cls):
+        shutdown_ray()
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     @patch("eva.expression.function_expression.FunctionExpression.evaluate")
     def test_should_benefit_from_pushdown(self, evaluate_mock):
         query = """SELECT id, obj.labels
                   FROM MyVideo JOIN LATERAL
                     FastRCNNObjectDetector(data) AS obj(labels, bboxes, scores)
```

### Comparing `evadb-0.1.6/test/integration_tests/test_pytorch.py` & `evadb-0.2.0/test/integration_tests/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import unittest
 from test.markers import windows_skip_marker
-from test.util import file_remove, load_udfs_for_testing
+from test.util import file_remove, load_udfs_for_testing, shutdown_ray
 
 import cv2
 import numpy as np
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
@@ -46,14 +46,16 @@
         execute_query_fetch_all(f"LOAD VIDEO '{asl_actions}' INTO Asl_actions;")
         execute_query_fetch_all(f"LOAD IMAGE '{meme1}' INTO MemeImages;")
         execute_query_fetch_all(f"LOAD IMAGE '{meme2}' INTO MemeImages;")
         load_udfs_for_testing()
 
     @classmethod
     def tearDownClass(cls):
+        shutdown_ray()
+
         file_remove("ua_detrac.mp4")
         file_remove("mnist.mp4")
         file_remove("actions.mp4")
         file_remove("computer_asl.mp4")
 
         execute_query_fetch_all("DROP TABLE IF EXISTS Actions;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MNIST;")
@@ -270,16 +272,31 @@
                   INPUT  (text NDARRAY STR(100))
                   OUTPUT (labels NDARRAY STR(10))
                   TYPE  Classification
                   IMPL  'eva/udfs/toxicity_classifier.py';
         """
         execute_query_fetch_all(create_udf_query)
 
-        select_query = """SELECT OCRExtractor(data).labels,
+        select_query = """SELECT name, OCRExtractor(data).labels,
                                  ToxicityClassifier(OCRExtractor(data).labels)
                         FROM MemeImages;"""
         actual_batch = execute_query_fetch_all(select_query)
 
         # non-trivial test case for Detoxify
         res = actual_batch.frames
-        self.assertTrue(res["toxicityclassifier.labels"][0] == "toxic")
-        self.assertTrue(res["toxicityclassifier.labels"][1] == "not toxic")
+        for i in range(2):
+            # Image can be reordered.
+            if "meme1" in res["memeimages.name"][i]:
+                self.assertTrue(res["toxicityclassifier.labels"][i] == "toxic")
+            else:
+                self.assertTrue(res["toxicityclassifier.labels"][i] == "not toxic")
+
+    def test_check_unnest_with_predicate_on_yolo(self):
+        query = """SELECT id, yolov5.label, yolov5.bbox, yolov5.score
+                  FROM MyVideo
+                  JOIN LATERAL UNNEST(YoloV5(data)) AS yolov5(label, bbox, score)
+                  WHERE yolov5.label = 'car' AND id < 10;"""
+
+        actual_batch = execute_query_fetch_all(query)
+
+        # due to unnest the number of returned tuples should be atleast > 10
+        self.assertTrue(len(actual_batch) > 10)
```

### Comparing `evadb-0.1.6/test/integration_tests/test_rename_executor.py` & `evadb-0.2.0/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/integration_tests/test_reuse.py` & `evadb-0.2.0/test/integration_tests/test_reuse.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import unittest
 from pathlib import Path
 from test.markers import windows_skip_marker
-from test.util import get_logical_query_plan, load_udfs_for_testing
+from test.util import get_logical_query_plan, load_udfs_for_testing, shutdown_ray
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.expression.function_expression import FunctionExpression
 from eva.optimizer.operators import LogicalFilter, LogicalFunctionScan
 from eva.optimizer.plan_generator import PlanGenerator
 from eva.optimizer.rules.rules import CacheFunctionExpressionInApply
@@ -33,14 +33,15 @@
     def setUp(self):
         CatalogManager().reset()
         ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(f"LOAD VIDEO '{ua_detrac}' INTO DETRAC;")
         load_udfs_for_testing()
 
     def tearDown(self):
+        shutdown_ray()
         execute_query_fetch_all("DROP TABLE IF EXISTS DETRAC;")
 
     def _verify_reuse_correctness(self, query, reuse_batch):
         with disable_rules([CacheFunctionExpressionInApply()]) as rules_manager:
             custom_plan_generator = PlanGenerator(rules_manager)
             without_reuse_batch = execute_query_fetch_all(
                 query, plan_generator=custom_plan_generator
```

### Comparing `evadb-0.1.6/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.0/test/integration_tests/test_s3_load_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import unittest
 from pathlib import Path
-from test.util import create_dummy_batches, create_sample_video, file_remove
+from test.util import (
+    create_dummy_batches,
+    create_sample_video,
+    file_remove,
+    shutdown_ray,
+)
 
 import boto3
 import pandas as pd
 import pytest
 from moto import mock_s3
 
 from eva.catalog.catalog_manager import CatalogManager
@@ -62,14 +67,16 @@
         self.s3_client.create_bucket(Bucket=bucket_name)
         video_path = self.multiple_video_file_path
 
         for file in os.listdir(video_path):
             self.s3_client.upload_file(f"{video_path}/{file}", bucket_name, file)
 
     def tearDown(self):
+        shutdown_ray()
+
         file_remove("MyVideo/dummy.avi", parent_dir=self.s3_download_dir)
 
         for file in os.listdir(self.multiple_video_file_path):
             file_remove(f"MyVideos/{file}", parent_dir=self.s3_download_dir)
 
         self.mock_s3.stop()
```

### Comparing `evadb-0.1.6/test/integration_tests/test_select_executor.py` & `evadb-0.2.0/test/integration_tests/test_select_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     create_dummy_4d_batches,
     create_dummy_batches,
     create_sample_video,
     create_table,
     file_remove,
     get_logical_query_plan,
     load_udfs_for_testing,
+    shutdown_ray,
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.binder.binder_utils import BinderError
@@ -51,14 +52,16 @@
         load_udfs_for_testing()
         cls.table1 = create_table("table1", 100, 3)
         cls.table2 = create_table("table2", 500, 3)
         cls.table3 = create_table("table3", 1000, 3)
 
     @classmethod
     def tearDownClass(cls):
+        shutdown_ray()
+
         file_remove("dummy.avi")
         drop_query = """DROP TABLE table1;"""
         execute_query_fetch_all(drop_query)
         drop_query = """DROP TABLE table2;"""
         execute_query_fetch_all(drop_query)
         drop_query = """DROP TABLE table3;"""
         execute_query_fetch_all(drop_query)
@@ -524,14 +527,30 @@
                     "myvideo.id": np.array([0, 0, 1, 1], np.intp),
                     "T.label": np.array(["person", "person", "bicycle", "bicycle"]),
                 }
             )
         )
         self.assertEqual(unnest_batch, expected)
 
+        # unnest with predicate on function expression
+        query = """SELECT id, label
+                FROM MyVideo JOIN LATERAL
+                UNNEST(DummyMultiObjectDetector(data).labels) AS T(label)
+                WHERE id < 2 AND T.label = "person" ORDER BY id;"""
+        unnest_batch = execute_query_fetch_all(query)
+        expected = Batch(
+            pd.DataFrame(
+                {
+                    "myvideo.id": np.array([0, 0], np.intp),
+                    "T.label": np.array(["person", "person"]),
+                }
+            )
+        )
+        self.assertEqual(unnest_batch, expected)
+
     def test_should_raise_error_with_missing_alias_in_lateral_join(self):
         udf_name = "DummyMultiObjectDetector"
         query = """SELECT id, labels
                   FROM MyVideo JOIN LATERAL DummyMultiObjectDetector(data).labels;"""
         with self.assertRaises(SyntaxError) as cm:
             execute_query_fetch_all(query)
         self.assertEqual(
```

### Comparing `evadb-0.1.6/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.0/test/integration_tests/test_show_info_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         execute_query_fetch_all("DROP TABLE IF EXISTS Actions;")
         execute_query_fetch_all("DROP TABLE IF EXISTS Mnist;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     # integration test
     def test_show_udfs(self):
         result = execute_query_fetch_all("SHOW UDFS;")
-        self.assertEqual(len(result.columns), 5)
+        self.assertEqual(len(result.columns), 6)
 
         expected = {
             "name": ["FastRCNNObjectDetector", "ArrayCount"],
             "inputs": [
                 ["Frame_Array NDARRAY UINT8 (3, None, None)"],
                 ["Input_Array NDARRAY ANYTYPE ()", "Search_Key ANY"],
             ],
```

### Comparing `evadb-0.1.6/test/integration_tests/test_similarity.py` & `evadb-0.2.0/test/integration_tests/test_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.util import create_sample_image, load_udfs_for_testing
+from test.util import create_sample_image, load_udfs_for_testing, shutdown_ray
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.models.storage.batch import Batch
@@ -90,14 +90,16 @@
                         ]
                     )
                 ),
             )
             base_img -= 1
 
     def tearDown(self):
+        shutdown_ray()
+
         drop_table_query = "DROP TABLE testSimilarityTable;"
         execute_query_fetch_all(drop_table_query)
         drop_table_query = "DROP TABLE testSimilarityFeatureTable;"
         execute_query_fetch_all(drop_table_query)
 
     def test_similarity_should_work_in_order(self):
         ###############################################
```

### Comparing `evadb-0.1.6/test/integration_tests/test_udf_executor.py` & `evadb-0.2.0/test/integration_tests/test_udf_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import tempfile
 import unittest
 from test.util import (
     DummyObjectDetector,
     create_dummy_batches,
     create_sample_video,
     file_remove,
+    shutdown_ray,
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.binder.binder_utils import BinderError
@@ -48,14 +49,15 @@
                   OUTPUT (label NDARRAY STR(10))
                   TYPE  Classification
                   IMPL  'test/util.py';
         """
         execute_query_fetch_all(create_udf_query)
 
     def tearDown(self):
+        shutdown_ray()
         file_remove("dummy.avi")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     # integration test
 
     def test_should_load_and_select_using_udf_video_in_table(self):
         select_query = "SELECT id,DummyObjectDetector(data) FROM MyVideo \
```

### Comparing `evadb-0.1.6/test/markers.py` & `evadb-0.2.0/test/markers.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/models/__init__.py` & `evadb-0.2.0/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/models/catalog/__init__.py` & `evadb-0.2.0/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/models/catalog/test_frame_info.py` & `evadb-0.2.0/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/models/storage/__init__.py` & `evadb-0.2.0/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/models/storage/test_batch.py` & `evadb-0.2.0/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/__init__.py` & `evadb-0.2.0/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/rules/__init__.py` & `evadb-0.2.0/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/rules/test_rules.py` & `evadb-0.2.0/test/optimizer/rules/test_rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,51 +19,63 @@
 from mock import MagicMock, patch
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import TableType
 from eva.catalog.models.table_catalog import TableCatalogEntry
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.experimental.ray.optimizer.rules.rules import LogicalExchangeToPhysical
+from eva.experimental.ray.optimizer.rules.rules import (
+    LogicalGetToSeqScan as DistributedLogicalGetToSeqScan,
+)
+from eva.experimental.ray.optimizer.rules.rules import (
+    LogicalProjectToPhysical as DistributedLogicalProjectToPhysical,
+)
 from eva.optimizer.operators import (
     LogicalFilter,
     LogicalGet,
     LogicalJoin,
-    LogicalProject,
     LogicalSample,
 )
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CombineSimilarityOrderByAndLimitToFaissIndexScan,
     EmbedFilterIntoGet,
-    EmbedProjectIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
     LogicalCreateIndexToFaiss,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
     LogicalDerivedGetToPhysical,
     LogicalDropToPhysical,
     LogicalDropUDFToPhysical,
     LogicalExplainToPhysical,
     LogicalFaissIndexScanToPhysical,
     LogicalFilterToPhysical,
     LogicalFunctionScanToPhysical,
-    LogicalGetToSeqScan,
+)
+from eva.optimizer.rules.rules import (
+    LogicalGetToSeqScan as SequentialLogicalGetToSeqScan,
+)
+from eva.optimizer.rules.rules import (
     LogicalGroupByToPhysical,
     LogicalInnerJoinCommutativity,
     LogicalInsertToPhysical,
     LogicalJoinToPhysicalHashJoin,
     LogicalJoinToPhysicalNestedLoopJoin,
     LogicalLateralJoinToPhysical,
     LogicalLimitToPhysical,
     LogicalLoadToPhysical,
     LogicalOrderByToPhysical,
-    LogicalProjectToPhysical,
+)
+from eva.optimizer.rules.rules import (
+    LogicalProjectToPhysical as SequentialLogicalProjectToPhysical,
+)
+from eva.optimizer.rules.rules import (
     LogicalRenameToPhysical,
     LogicalShowToPhysical,
     LogicalUnionToPhysical,
     Promise,
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
@@ -92,15 +104,14 @@
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     def test_rules_promises_order(self):
         # Promise of all rewrite should be greater than implementation
         rewrite_promises = [
             Promise.LOGICAL_INNER_JOIN_COMMUTATIVITY,
             Promise.EMBED_FILTER_INTO_GET,
-            Promise.EMBED_PROJECT_INTO_GET,
             Promise.EMBED_SAMPLE_INTO_GET,
             Promise.XFORM_LATERAL_JOIN_TO_LINEAR_FLOW,
             Promise.PUSHDOWN_FILTER_THROUGH_JOIN,
             Promise.PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE,
             Promise.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN,
             Promise.REORDER_PREDICATES,
         ]
@@ -151,75 +162,86 @@
         self.assertEqual(rewrite_count + implementation_count + 2, promise_count)
 
     def test_supported_rules(self):
         # adding/removing rules should update this test
         supported_rewrite_rules = [
             EmbedFilterIntoGet(),
             #    EmbedFilterIntoDerivedGet(),
-            EmbedProjectIntoGet(),
             EmbedSampleIntoGet(),
-            #    EmbedProjectIntoDerivedGet(),
             XformLateralJoinToLinearFlow(),
             PushDownFilterThroughApplyAndMerge(),
             PushDownFilterThroughJoin(),
             CombineSimilarityOrderByAndLimitToFaissIndexScan(),
             ReorderPredicates(),
         ]
+        rewrite_rules = (
+            RulesManager().stage_one_rewrite_rules
+            + RulesManager().stage_two_rewrite_rules
+        )
         self.assertEqual(
-            len(supported_rewrite_rules), len(RulesManager().rewrite_rules)
+            len(supported_rewrite_rules),
+            len(rewrite_rules),
         )
         # check all the rule instance exists
         for rule in supported_rewrite_rules:
-            self.assertTrue(
-                any(isinstance(rule, type(x)) for x in RulesManager().rewrite_rules)
-            )
+            self.assertTrue(any(isinstance(rule, type(x)) for x in rewrite_rules))
 
         supported_logical_rules = [
             LogicalInnerJoinCommutativity(),
             CacheFunctionExpressionInApply(),
         ]
         self.assertEqual(
             len(supported_logical_rules), len(RulesManager().logical_rules)
         )
 
         for rule in supported_logical_rules:
             self.assertTrue(
                 any(isinstance(rule, type(x)) for x in RulesManager().logical_rules)
             )
 
+        ray_enabled = ConfigurationManager().get_value("experimental", "ray")
+
+        # For the current version, we choose either the distributed or the
+        # sequential rule, because we do not have a logic to choose one over
+        # the other in the current optimizer. Sequential rewrite is currently
+        # embedded inside distributed rule if ray is enabled. The rule itself
+        # has some simple heuristics to choose one over the other.
         supported_implementation_rules = [
             LogicalCreateToPhysical(),
             LogicalRenameToPhysical(),
             LogicalDropToPhysical(),
             LogicalCreateUDFToPhysical(),
             LogicalDropUDFToPhysical(),
             LogicalInsertToPhysical(),
             LogicalDeleteToPhysical(),
             LogicalLoadToPhysical(),
-            LogicalGetToSeqScan(),
+            DistributedLogicalGetToSeqScan()
+            if ray_enabled
+            else SequentialLogicalGetToSeqScan(),
             LogicalDerivedGetToPhysical(),
             LogicalUnionToPhysical(),
             LogicalGroupByToPhysical(),
             LogicalOrderByToPhysical(),
             LogicalLimitToPhysical(),
             LogicalJoinToPhysicalNestedLoopJoin(),
             LogicalLateralJoinToPhysical(),
             LogicalFunctionScanToPhysical(),
             LogicalJoinToPhysicalHashJoin(),
             LogicalCreateMaterializedViewToPhysical(),
             LogicalFilterToPhysical(),
-            LogicalProjectToPhysical(),
+            DistributedLogicalProjectToPhysical()
+            if ray_enabled
+            else SequentialLogicalProjectToPhysical(),
             LogicalShowToPhysical(),
             LogicalExplainToPhysical(),
             LogicalCreateIndexToFaiss(),
             LogicalApplyAndMergeToPhysical(),
             LogicalFaissIndexScanToPhysical(),
         ]
 
-        ray_enabled = ConfigurationManager().get_value("experimental", "ray")
         if ray_enabled:
             supported_implementation_rules.append(LogicalExchangeToPhysical())
         self.assertEqual(
             len(supported_implementation_rules),
             len(RulesManager().implementation_rules),
         )
 
@@ -227,28 +249,14 @@
             self.assertTrue(
                 any(
                     isinstance(rule, type(x))
                     for x in RulesManager().implementation_rules
                 )
             )
 
-    # EmbedProjectIntoGet
-    def test_simple_project_into_get(self):
-        rule = EmbedProjectIntoGet()
-        expr1 = MagicMock()
-        expr2 = MagicMock()
-        expr3 = MagicMock()
-
-        logi_get = LogicalGet(MagicMock(), MagicMock(), MagicMock())
-        logi_project = LogicalProject([expr1, expr2, expr3], [logi_get])
-
-        rewrite_opr = next(rule.apply(logi_project, MagicMock()))
-        self.assertFalse(rewrite_opr is logi_get)
-        self.assertEqual(rewrite_opr.target_list, [expr1, expr2, expr3])
-
     # EmbedFilterIntoGet
     def test_simple_filter_into_get(self):
         rule = EmbedFilterIntoGet()
         predicate = MagicMock()
 
         logi_get = LogicalGet(MagicMock(), MagicMock(), MagicMock())
         logi_filter = LogicalFilter(predicate, [logi_get])
@@ -270,15 +278,15 @@
         self.assertFalse(rule.check(logi_sample, MagicMock()))
 
     def test_disable_rules(self):
         with disable_rules([PushDownFilterThroughApplyAndMerge()]) as rules_manager:
             self.assertFalse(
                 any(
                     isinstance(PushDownFilterThroughApplyAndMerge, type(x))
-                    for x in rules_manager.rewrite_rules
+                    for x in rules_manager.stage_two_rewrite_rules
                 )
             )
 
     def test_xform_lateral_join_does_not_work_with_other_join(self):
         rule = XformLateralJoinToLinearFlow()
         logi_join = LogicalJoin(JoinType.INNER_JOIN)
         self.assertFalse(rule.check(logi_join, MagicMock()))
```

### Comparing `evadb-0.1.6/test/optimizer/test_binder.py` & `evadb-0.2.0/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.0/test/integration_tests/test_error_handling_with_ray.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,53 +8,66 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import time
 import unittest
-from test.util import NUM_FRAMES, create_sample_video, file_remove
+from pathlib import Path
+from test.util import (
+    create_sample_image,
+    is_ray_stage_running,
+    load_udfs_for_testing,
+    shutdown_ray,
+)
 
-import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
-from eva.models.storage.batch import Batch
+from eva.configuration.configuration_manager import ConfigurationManager
+from eva.executor.executor_utils import ExecutorError
 from eva.server.command_handler import execute_query_fetch_all
 
 
-@pytest.mark.notparallel
-class CascadeOptimizer(unittest.TestCase):
+@pytest.mark.skipif(
+    not ConfigurationManager().get_value("experimental", "ray"),
+    reason="Only test for ray execution.",
+)
+class ErrorHandlingRayTests(unittest.TestCase):
     def setUp(self):
         CatalogManager().reset()
-        self.video_file_path = create_sample_video(NUM_FRAMES)
+        ConfigurationManager()
+        # Load built-in UDFs.
+        load_udfs_for_testing(mode="minimal")
+
+        # Deliberately create a faulty path.
+        img_path = create_sample_image()
+        execute_query_fetch_all(f"LOAD IMAGE '{img_path}' INTO testRayErrorHandling;")
+
+        # Forcefully remove file to cause error.
+        Path(img_path).unlink()
 
     def tearDown(self):
-        file_remove("dummy.avi")
+        shutdown_ray()
 
-    def test_logical_to_physical_udf(self):
-        load_query = f"LOAD VIDEO '{self.video_file_path}' INTO MyVideo;"
-        execute_query_fetch_all(load_query)
-
-        create_udf_query = """CREATE UDF DummyObjectDetector
-                  INPUT  (Frame_Array NDARRAY UINT8(3, 256, 256))
-                  OUTPUT (label NDARRAY STR(10))
+        # Drop table.
+        drop_table_query = "DROP TABLE testRayErrorHandling;"
+        execute_query_fetch_all(drop_table_query)
+
+    def test_ray_error_populate_to_all_stages(self):
+        create_udf_query = """CREATE UDF IF NOT EXISTS ToxicityClassifier
+                  INPUT  (text NDARRAY STR(100))
+                  OUTPUT (labels NDARRAY STR(10))
                   TYPE  Classification
-                  IMPL  'test/util.py';
+                  IMPL  'eva/udfs/toxicity_classifier.py';
         """
         execute_query_fetch_all(create_udf_query)
 
-        select_query = """SELECT id, DummyObjectDetector(data)
-                    FROM MyVideo
-                    WHERE DummyObjectDetector(data).label = ['person'];
-        """
-        actual_batch = execute_query_fetch_all(select_query)
-        actual_batch.sort()
-        expected = [
-            {"myvideo.id": i * 2, "dummyobjectdetector.label": ["person"]}
-            for i in range(NUM_FRAMES // 2)
-        ]
-        expected_batch = Batch(frames=pd.DataFrame(expected))
-        self.assertEqual(actual_batch, expected_batch)
+        select_query = """SELECT ToxicityClassifier(data) FROM testRayErrorHandling;"""
+
+        with self.assertRaises(ExecutorError):
+            _ = execute_query_fetch_all(select_query)
 
-        execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
+        time.sleep(3)
+        self.assertFalse(is_ray_stage_running())
```

### Comparing `evadb-0.1.6/test/optimizer/test_cost_model.py` & `evadb-0.2.0/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_group.py` & `evadb-0.2.0/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_memo.py` & `evadb-0.2.0/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_optimizer_context.py` & `evadb-0.2.0/test/optimizer/test_optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.0/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/optimizer/test_statement_to_opr_convertor.py` & `evadb-0.2.0/test/optimizer/test_statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/parser/__init__.py` & `evadb-0.2.0/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/parser/test_parser.py` & `evadb-0.2.0/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/parser/test_parser_statements.py` & `evadb-0.2.0/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/plan_nodes/__init__.py` & `evadb-0.2.0/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/plan_nodes/test_plan.py` & `evadb-0.2.0/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/readers/__init__.py` & `evadb-0.2.0/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/readers/test_csv_reader.py` & `evadb-0.2.0/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/readers/test_decord_reader.py` & `evadb-0.2.0/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/server/__init__.py` & `evadb-0.2.0/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/server/test_command_handler.py` & `evadb-0.2.0/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/server/test_db_api.py` & `evadb-0.2.0/test/server/test_db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/server/test_interpreter.py` & `evadb-0.2.0/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/server/test_server.py` & `evadb-0.2.0/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/storage/__init__.py` & `evadb-0.2.0/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.0/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/storage/test_video_storage.py` & `evadb-0.2.0/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/test_eva_cmd_client.py` & `evadb-0.2.0/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/test_eva_imports.py` & `evadb-0.2.0/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/test_eva_server.py` & `evadb-0.2.0/test/test_eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/__init__.py` & `evadb-0.2.0/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/decorators/__init__.py` & `evadb-0.2.0/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.0/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.0/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/decorators/test_decorators.py` & `evadb-0.2.0/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/ndarray/__init__.py` & `evadb-0.2.0/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.0/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/ndarray/test_crop.py` & `evadb-0.2.0/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/ndarray/test_open.py` & `evadb-0.2.0/test/udfs/ndarray/test_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,9 +55,9 @@
 
         # cached open
         with patch("eva.udfs.ndarray.open.cv2") as mock_cv2:
             self.open_instance(pd.DataFrame([self.image_file_path]))
             mock_cv2.imread.assert_not_called()
 
     def test_open_path_should_raise_error(self):
-        with self.assertRaises(AssertionError):
+        with self.assertRaises((AssertionError, FileNotFoundError)):
             self.open_instance(pd.DataFrame(["incorrect_path"]))
```

### Comparing `evadb-0.1.6/test/udfs/test_abstract_udf.py` & `evadb-0.2.0/test/udfs/test_abstract_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 import unittest
 from enum import Enum
 from inspect import isabstract
 from test.util import get_all_subclasses, get_mock_object
+from unittest.mock import patch
 
 import eva
 from eva.udfs.abstract.abstract_udf import AbstractUDF
 
 
 class AbstractUDFTest(unittest.TestCase):
-    def test_udf_abstract_functions(self):
+    # Need to mock the HF pipeline function to avoid downloading a model
+    @patch("eva.udfs.abstract.hf_abstract_udf.pipeline")
+    def test_udf_abstract_functions(self, mock_pipeline):
         derived_udf_classes = list(get_all_subclasses(AbstractUDF))
-
         # Go over each derived class of AbstractUDF
         for derived_udf_class in derived_udf_classes:
             if isabstract(derived_udf_class) is False:
                 class_type = derived_udf_class
                 # Check class init signature
                 # Ref: https://stackoverflow.com/a/2677263
                 sig = inspect.signature(class_type.__init__)
```

### Comparing `evadb-0.1.6/test/udfs/test_emotion_detector.py` & `evadb-0.2.0/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/test_facenet_udf.py` & `evadb-0.2.0/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.0/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.0/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/util.py` & `evadb-0.2.0/test/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import socket
 from contextlib import closing
 from pathlib import Path
 
 import cv2
 import numpy as np
 import pandas as pd
+import psutil
+import ray
 from mock import MagicMock
 
 from eva.binder.statement_binder import StatementBinder
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.catalog.catalog_type import NdArrayType
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.models.storage.batch import Batch
@@ -44,14 +46,23 @@
 tmp_dir_from_config = config.get_value("storage", "tmp_dir")
 s3_dir_from_config = config.get_value("storage", "s3_download_dir")
 
 
 EVA_TEST_DATA_DIR = Path(config.get_value("core", "eva_installation_dir")).parent
 
 
+def is_ray_stage_running():
+    return "ray::ray_stage" in (p.name() for p in psutil.process_iter())
+
+
+def shutdown_ray():
+    if ConfigurationManager().get_value("experimental", "ray"):
+        ray.shutdown()
+
+
 def prefix_worker_id(base: str):
     try:
         worker_id = os.environ["PYTEST_XDIST_WORKER"]
         prefixed_base = str(worker_id) + "_" + base
     except KeyError:
         # Single threaded mode
         prefixed_base = base
@@ -283,14 +294,31 @@
     df = pd.DataFrame(columns=columns)
     for col in columns:
         df[col] = np.random.randint(1, 100, num_rows)
     df.to_csv(csv_path, index=False)
     return df, csv_path
 
 
+def create_text_csv(num_rows=30):
+    """
+    Creates a csv with 2 columns: id and comment
+    The comment column has 2 values: "I like this" and "I don't like this" that are alternated
+    """
+    csv_path = os.path.join(tmp_dir_from_config, "dummy.csv")
+    try:
+        os.remove(csv_path)
+    except FileNotFoundError:
+        pass
+    df = pd.DataFrame(columns=["id", "comment"])
+    df["id"] = np.arange(num_rows)
+    df["comment"] = np.where(df["id"] % 2 == 0, "I like this", "I don't like this")
+    df.to_csv(csv_path, index=False)
+    return csv_path
+
+
 def create_table(table_name, num_rows, num_columns):
     # creates a table with num_rows tuples and columns = [a1, a2, a3, ...]
     columns = "".join("a{} INTEGER, ".format(i) for i in range(num_columns - 1))
     columns += "a{} INTEGER".format(num_columns - 1)
     create_table_query = "CREATE TABLE IF NOT EXISTS {} ( {} );".format(
         table_name, columns
     )
```

### Comparing `evadb-0.1.6/test/utils/__init__.py` & `evadb-0.2.0/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.1.6/test/utils/test_generic_utils.py` & `evadb-0.2.0/test/utils/test_generic_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
-from pathlib import Path
 from test.markers import windows_skip_marker
 
 from mock import MagicMock, patch
 
 from eva.readers.decord_reader import DecordReader
 from eva.utils.generic_utils import (
     generate_file_path,
@@ -88,15 +87,14 @@
 
     @windows_skip_marker
     @patch("eva.utils.generic_utils.ConfigurationManager")
     def test_should_return_a_random_full_path(self, mock_conf):
         mock_conf_inst = MagicMock()
         mock_conf.return_value = mock_conf_inst
         mock_conf_inst.get_value.return_value = "eva_datasets"
-        expected = Path("eva_datasets").resolve()
         actual = generate_file_path("test")
         self.assertTrue(actual.is_absolute())
         # Root directory must be the same, filename is random
-        self.assertTrue(expected.match(str(actual.parent)))
+        self.assertTrue("eva_datasets" in str(actual.parent))
 
         mock_conf_inst.get_value.return_value = None
         self.assertRaises(KeyError, generate_file_path)
```

### Comparing `evadb-0.1.6/test/utils/test_timer.py` & `evadb-0.2.0/test/utils/test_timer.py`

 * *Files identical despite different names*

