# Comparing `tmp/sparrow-order-lib-0.1.82.tar.gz` & `tmp/sparrow-order-lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hbshun/coder/hg/sparrow-order-lib/dist/.tmp-qcszmu21/sparrow-order-lib-0.1.82.tar", last modified: Mon Apr 17 06:56:30 2023, max compression
+gzip compressed data, was "/Users/hbshun/hg/sparrow-order-lib/dist/tmp6d8iuth3/sparrow-order-lib-0.1.9.tar", last modified: Thu Sep  1 08:11:13 2022, max compression
```

## Comparing `sparrow-order-lib-0.1.82.tar` & `sparrow-order-lib-0.1.9.tar`

### file list

```diff
@@ -1,122 +1,103 @@
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/
--rw-r--r--   0 hbshun     (501) staff       (20)     1073 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/LICENSE
--rw-r--r--   0 hbshun     (501) staff       (20)     8426 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/PKG-INFO
--rw-r--r--   0 hbshun     (501) staff       (20)     7888 2023-04-16 05:52:08.000000 sparrow-order-lib-0.1.82/README.md
--rw-r--r--   0 hbshun     (501) staff       (20)      103 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/pyproject.toml
--rw-r--r--   0 hbshun     (501) staff       (20)      724 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/setup.cfg
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/
--rw-r--r--   0 hbshun     (501) staff       (20)       76 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/__init__.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2014 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/base_models.py
--rw-r--r--   0 hbshun     (501) staff       (20)      517 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/common_utils.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5614 2022-12-27 05:47:04.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1592 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/datastructures.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1353 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/decorators.py
--rw-r--r--   0 hbshun     (501) staff       (20)    12853 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/dt_utils.py
--rw-r--r--   0 hbshun     (501) staff       (20)       90 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/formats.py
--rw-r--r--   0 hbshun     (501) staff       (20)      714 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/model_function.py
--rw-r--r--   0 hbshun     (501) staff       (20)      251 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/numbers.py
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/text.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1415 2022-11-04 01:55:42.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/xls_util.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/db_tool/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/db_tool/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)      848 2022-11-04 01:55:42.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/db_tool/query.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/
--rw-r--r--   0 hbshun     (501) staff       (20)     1359 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)      422 2022-08-16 14:34:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/constants.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/
--rw-r--r--   0 hbshun     (501) staff       (20)       56 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7841 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/base.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1092 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/client.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1228 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3661 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_builder.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3091 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_door.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5145 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3620 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_query_util.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1223 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/exceptions.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2207 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/field.py
--rw-r--r--   0 hbshun     (501) staff       (20)      381 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/in_query_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)      163 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/index.py
--rw-r--r--   0 hbshun     (501) staff       (20)      241 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/mock.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3137 2022-08-16 14:34:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/operators.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/
--rw-r--r--   0 hbshun     (501) staff       (20)     1619 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1782 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_base.py
--rw-r--r--   0 hbshun     (501) staff       (20)       64 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_client.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2455 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3294 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3947 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2500 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2310 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_field.py
--rw-r--r--   0 hbshun     (501) staff       (20)      515 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
--rw-r--r--   0 hbshun     (501) staff       (20)      373 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_mock.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2203 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_operators.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7542 2022-08-16 14:34:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/mapping_constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3086 2022-08-16 14:34:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/query_mapping_constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3490 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/test_order_doc_type.py
--rw-r--r--   0 hbshun     (501) staff       (20)       42 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/example.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/
--rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1406 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_api_path.py
--rw-r--r--   0 hbshun     (501) staff       (20)      815 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_core.py
--rw-r--r--   0 hbshun     (501) staff       (20)     5271 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_core_go.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2778 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
--rw-r--r--   0 hbshun     (501) staff       (20)     4706 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_product.py
--rw-r--r--   0 hbshun     (501) staff       (20)      383 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/svc_config.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/
--rw-r--r--   0 hbshun     (501) staff       (20)       31 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3239 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     2974 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/models.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1164 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
--rw-r--r--   0 hbshun     (501) staff       (20)      539 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_afsplus/utils.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/
--rw-r--r--   0 hbshun     (501) staff       (20)       33 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     8626 2023-01-17 07:33:44.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    17814 2023-04-07 09:21:03.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    71783 2023-02-27 08:08:35.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7206 2023-02-21 10:06:52.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1892 2023-01-12 02:23:41.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/disstorage.py
--rw-r--r--   0 hbshun     (501) staff       (20)    15398 2023-02-21 10:06:52.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/models.py
--rw-r--r--   0 hbshun     (501) staff       (20)      550 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
--rw-r--r--   0 hbshun     (501) staff       (20)      390 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/serializers.py
--rw-r--r--   0 hbshun     (501) staff       (20)      514 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/utils.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    56765 2023-04-17 06:55:14.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    32810 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/models.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7952 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/serializer_data.py
--rw-r--r--   0 hbshun     (501) staff       (20)     4095 2023-02-01 10:05:34.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/serializers.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/
--rw-r--r--   0 hbshun     (501) staff       (20)      155 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    15287 2023-01-17 07:33:44.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    17612 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_inparcel/
--rw-r--r--   0 hbshun     (501) staff       (20)       32 2023-01-17 07:52:01.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_inparcel/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     8197 2023-01-17 07:41:20.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_inparcel/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)    11201 2023-02-21 10:11:18.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_inparcel/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_orders/
--rw-r--r--   0 hbshun     (501) staff       (20)       68 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_orders/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)    10215 2022-12-27 05:47:04.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_orders/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)   108809 2022-12-27 08:57:01.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_orders/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/
--rw-r--r--   0 hbshun     (501) staff       (20)       30 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     4434 2023-01-17 07:42:01.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)      455 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/exceptions.py
--rw-r--r--   0 hbshun     (501) staff       (20)     7599 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_promotions/
--rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_promotions/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     1979 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_promotions/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/
--rw-r--r--   0 hbshun     (501) staff       (20)       32 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/__init__.py
--rw-r--r--   0 hbshun     (501) staff       (20)     3236 2023-02-27 08:08:54.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/constants.py
--rw-r--r--   0 hbshun     (501) staff       (20)     9065 2022-06-26 00:49:25.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/models.py
-drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/
--rw-r--r--   0 hbshun     (501) staff       (20)     8426 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/PKG-INFO
--rw-r--r--   0 hbshun     (501) staff       (20)     4741 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/SOURCES.txt
--rw-r--r--   0 hbshun     (501) staff       (20)        1 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/dependency_links.txt
--rw-r--r--   0 hbshun     (501) staff       (20)       39 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/requires.txt
--rw-r--r--   0 hbshun     (501) staff       (20)       18 2023-04-17 06:56:30.000000 sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/top_level.txt
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1073 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/LICENSE
+-rw-r--r--   0 hbshun     (501) staff       (20)     5961 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/PKG-INFO
+-rw-r--r--   0 hbshun     (501) staff       (20)     5424 2022-09-01 08:08:40.000000 sparrow-order-lib-0.1.9/README.md
+-rw-r--r--   0 hbshun     (501) staff       (20)      103 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/pyproject.toml
+-rw-r--r--   0 hbshun     (501) staff       (20)      662 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/setup.cfg
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/
+-rw-r--r--   0 hbshun     (501) staff       (20)       76 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/__init__.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2014 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/base_models.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      517 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/common_utils.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3745 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1592 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/datastructures.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1353 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/decorators.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    12853 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/dt_utils.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       90 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/formats.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      714 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/model_function.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      251 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/numbers.py
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/text.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      842 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/query.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1359 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      422 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/constants.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/
+-rw-r--r--   0 hbshun     (501) staff       (20)       56 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7841 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/base.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1092 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/client.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1228 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3661 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_builder.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3091 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_door.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5145 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3620 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_query_util.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1223 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/exceptions.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2207 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/field.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      381 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/in_query_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      163 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/index.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      241 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/mock.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3137 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/operators.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/
+-rw-r--r--   0 hbshun     (501) staff       (20)     1619 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1782 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_base.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       64 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_client.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2455 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3294 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3947 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2500 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2310 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_field.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      515 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      373 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_mock.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2203 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_operators.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7542 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/mapping_constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3086 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/query_mapping_constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3490 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/test_order_doc_type.py
+-rw-r--r--   0 hbshun     (501) staff       (20)       42 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/example.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/
+-rw-r--r--   0 hbshun     (501) staff       (20)        0 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1406 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_api_path.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      815 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5271 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core_go.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2778 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     4706 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_product.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      383 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/svc_config.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/
+-rw-r--r--   0 hbshun     (501) staff       (20)       33 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     3427 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    65289 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     5826 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    13289 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    48594 2022-09-01 08:01:19.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    29654 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/
+-rw-r--r--   0 hbshun     (501) staff       (20)      155 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    13431 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    17612 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/
+-rw-r--r--   0 hbshun     (501) staff       (20)       68 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)    23984 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)   108751 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/
+-rw-r--r--   0 hbshun     (501) staff       (20)       30 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     4285 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)      455 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/exceptions.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     7599 2022-04-22 04:00:29.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/
+-rw-r--r--   0 hbshun     (501) staff       (20)       34 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     1979 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/
+-rw-r--r--   0 hbshun     (501) staff       (20)       32 2022-08-16 06:45:36.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/__init__.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     2788 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/constants.py
+-rw-r--r--   0 hbshun     (501) staff       (20)     9065 2022-04-21 06:32:48.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/models.py
+drwxr-xr-x   0 hbshun     (501) staff       (20)        0 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/
+-rw-r--r--   0 hbshun     (501) staff       (20)     5961 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/PKG-INFO
+-rw-r--r--   0 hbshun     (501) staff       (20)     3855 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 hbshun     (501) staff       (20)        1 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 hbshun     (501) staff       (20)       18 2022-09-01 08:11:13.000000 sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/top_level.txt
```

### Comparing `sparrow-order-lib-0.1.82/LICENSE` & `sparrow-order-lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/setup.cfg` & `sparrow-order-lib-0.1.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-order-lib
-version = 0.1.82
+version = 0.1.9
 author = Jessica Liao
 author_email = 18610193367@sina.cn
 description = This is a lib for sparrow order projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/sparrow614/sparrow-order-lib
 project_urls = 
@@ -15,17 +15,14 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
-install_requires = 
-	XlsxWriter~=3.0.3
-	elasticsearch==7.8.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/base_models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/base_models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/common_utils.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/datastructures.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/decorators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/dt_utils.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/dt_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/core/model_function.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/core/model_function.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/db_tool/query.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/db_tool/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from collections import namedtuple
 from django.db import connection
 import logging
-
 logger = logging.getLogger(__name__)
 
-
 def namedtuplefetchall(cursor):
     "Return all rows from a cursor as a namedtuple"
     desc = cursor.description
     nt_result = namedtuple('Result', [col[0] for col in desc])
     return [nt_result(*row) for row in cursor.fetchall()]
 
-
 def query_data_by_sql(sql_str, params):
     db_return = []
     err_msg = ""
     try:
         with connection.cursor() as c:
             if not params:
                 c.execute(sql_str)
             else:
                 c.execute(sql_str, params)
             db_return = namedtuplefetchall(c.cursor)
     except BaseException as be:
         db_return = []
-        err_msg = "查询失败,原因: {be_str}".format(be_str=str(be))
+        err_msg="查询失败,原因: {be_str}".format(be_str=str(be))
         logger.error(err_msg)
-    return db_return, err_msg
+    return db_return, err_msg
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/__init__.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/base.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/client.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/client.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_builder.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_door.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/es_query_util.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/exceptions.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/field.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/operators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/__init__.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_base.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_door.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_field.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/es_util/tests/test_operators.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/es_util/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/mapping_constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/query_mapping_constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/query_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/es/test_order_doc_type.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/es/test_order_doc_type.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_api_path.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_api_path.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_core.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_core_go.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_core_go.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_lanyue.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_lanyue.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/remote_call/sparrow_product.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/remote_call/sparrow_product.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,58 @@
-from ..core.datastructures import ImmutableList
+# 这些常量会在其他地方被用到，用作某些判断
 
 
-class AfsLineStatus:
-    ''' 退款单表体状态 '''
-    # 导购收货
-    # GUIDE_RECEIVED = "GuideReceived"
-    GUIDE_RECEIVED = "guide_received"
-
-    CHOICES = (
-        (GUIDE_RECEIVED, "导购收货"),
-    )
-
-
-class Aftersale_Number_Refund_Status(object):
-    # 退单子退款状态(init初始/doing进行中/done已完成)
+class ReversedStockStatus(object):
+    # 默认状态
     INIT = "init"
-    DOING = "doing"
-    DONE = "done"
-    FAILED = "failed"
-    AFTERSALE_NUMBER_REFUND_STATUS_CHOICES = (
-        (INIT, '初始'),
-        (DOING, '进行中'),
-        (DONE, "已完成"),
-        (FAILED, "失败"),
-
-    )
-    AFTERSALE_NUMBER_REFUND_STATUS_DICT = dict(AFTERSALE_NUMBER_REFUND_STATUS_CHOICES)
-
-
-class WechatDeliveryReturnStatus:
-    """ 用户寄回时的方式 """
-    INIT = 0  # 用户未填写退货信息
-    APPLY = 1  # 在线预约
-    SELF = 2  # 自主填写
-
-
-class WechatDeliveryReturnOrderStatus:
-    """ 退单状态 """
-    INIT = 0  # 已下单, 待揽收
-    PACKAGED = 1  # 已揽件
-    TRANSIT = 2  # 运输中
-    DELIVERING = 3  # 派件中
-    SELF_SIGNED = 4  # 已签收
-    ABNORMAL = 5  # 异常
-    PRE_SIGNED = 6  # 代签收
-    FAIL_PACKAGED = 7  # 揽件失败
-    FAIL_SIGNED = 8  # 签收失败(拒签、超区)
-    CANCEL = 11  # 已取消
-    RETURNING = 13  # 退件中
-    RETURNED = 14  # 已退件
-    UNHEARD = 99  # 未知
-
-    # 非终态退单状态
-    UNTERMINATE_ORDER_TYPE_LIST = ImmutableList(
-        [INIT, PACKAGED, TRANSIT, DELIVERING, RETURNING, UNHEARD]
-    )
-
-
-######### 以下内容来自 constant_event.py ##########
-class EventMapKey(object):
-
-    TO_STATUS_KEY = "to_status"
-    USER_ROLES_KEY = "user_roles"
-
-
-class AfsNumberRefundEventConst(object):
-    ### 子退单事件 ###
-    # 子退单开始申请退
-    START = "start"
-    # 子退单完成
-    SUCCESS = "success"
-    # 子退单失败
-    FAIL = "fail"
-
-    EVENT_2_BUTTONNAME_MAP = {
-        START: "子退单开始申请退",
-        SUCCESS: "子退单完成",
-        FAIL: "子退单失败"
-    }
-
-    FROM_TO_MAP = {
-        START: {  # 子退单开始申请退
-            Aftersale_Number_Refund_Status.INIT: {
-                EventMapKey.TO_STATUS_KEY: Aftersale_Number_Refund_Status.DOING,
-                EventMapKey.USER_ROLES_KEY: None
-            }
-        },
-        SUCCESS: {  # 子退单完成
-            Aftersale_Number_Refund_Status.DOING: {
-                EventMapKey.TO_STATUS_KEY: Aftersale_Number_Refund_Status.DONE,
-                EventMapKey.USER_ROLES_KEY: None
-            },
-            Aftersale_Number_Refund_Status.FAILED: {
-                EventMapKey.TO_STATUS_KEY: Aftersale_Number_Refund_Status.DONE,
-                EventMapKey.USER_ROLES_KEY: None
-            },
-        },
-        FAIL: {  # 子退单失败
-            Aftersale_Number_Refund_Status.DOING: {
-                EventMapKey.TO_STATUS_KEY: Aftersale_Number_Refund_Status.FAILED,
-                EventMapKey.USER_ROLES_KEY: None
-            },
-            Aftersale_Number_Refund_Status.FAILED: {
-                EventMapKey.TO_STATUS_KEY: Aftersale_Number_Refund_Status.FAILED,
-                EventMapKey.USER_ROLES_KEY: None
-            }
-        }
-    }
-
-
-class AfsLineGenerateFrom:
-    SELECT = 'select'  # 创建售后时选中的
-    VIRTUAL = 'virtual'  # 虚拟订单数据
-    ORIGIN = 'origin'  # 创建售后前的订单(或虚拟订单)数据
-
-    CHOICES = (
-        (SELECT, "创建售后时选择的商品"),
-        (VIRTUAL, "虚拟订单数据"),
-        (ORIGIN, "创建售后前的订单(或虚拟订单)数据"),
-    )
-
-
-class AfsVersionConst:
-    V2 = "V2"
-    V3 = "V3"
+    # 缺货
+    SHORTAGE = "shortage"
+    # 无货需要下架
+    OFF = "off"
+    # 备好货
+    PREPARED = "prepared"
+
+
+class ReversedStockType(object):
+    PRODUCT = "product"
+    GIFT = "gift"
+
+
+class ReversedStockActions(object):
+    # 导购标记货品
+    GUIDE_MARK = "guide_mark"
+    # 客服取货
+    PICK_UP = "pick_up"
+    # 客服还货
+    RETURN = "return"
+
+
+class ReversedStockNoteMessage(object):
+    GUIDE_MARK = '标记货品状态为{0}'
+    PICK_UP = '客服提货'
+    RETURN = '客服还货'
+
+
+class RequiredCountStock(object):
+    IS_STOCK = "is_stock"
+    IS_REQUIRED_COUNT = "is_required_count"
+    IS_ANY = "is_any"
 
 
 class AftersaleActions(object):
     # 创建售后单
     CREATE = "create"
     # 修改售后单
     UPDATE = "update"
     # 关闭售后单
     REMOVE = "remove"
     # 完成售后单
     COMPLETE = "complete"
     # 客服审核通过
     OPERATOR_APPROVE = "operator_approve"
-    # 客服审核拒绝- 消费抖店拒绝售后消息
-    OPERATOR_REFUSED = "operator_refused"
     # 财务审核通过
     FINANCE_APPROVE_1ST = "finance_approve_1st"
     # 财务审核通过
     FINANCE_APPROVE = "finance_approve"
     # 财务驳回
     FINANCE_REJECT = "finance_reject"
     # 店内系统驳回
@@ -167,221 +77,238 @@
     CONFIRM_RETURNED = "confirm_returned"
     # 客户回填运单信息
     CUSTOMER_WRITEBACK_EXPRESS = "customer_writeback_express"
     # 拦截失败
     BLOCK_FAILED = "block_failed"
     # 客服修改运单信息
     CUSSERVICE_MODIFY_EXPRESS = "cusservice_modify_express"
-    # 强制确收退货
-    FORCE_CONFIRM_RETURNED = "force_confirm_returned"
-    # 同步线下-总退单
-    SYNC_OFFLINE = "sync_offline"
-    # 同步线下-退款
-    SYNC_OFFLINE_AFS = "sync_offline_afs"
-    # 同步线下-营业外收入
-    SYNC_OFFLINE_HGINCOME = "sync_offline_hgincome"
-    # 打印退款单
-    PRINT_AFTERSALE_SUB = "print"
-    # 自动
-    AUTO_REFUND = "auto_refund"
 
 
+class AssignmentActions(object):
+    # 创建配货
+    CREATE = "create"
+    # 关闭配货
+    REMOVE = "remove"
+    # 完成配货
+    COMPLETE = "complete"
+    # 已打印
+    PRINTED = "printed"
 
-class AfterSaleType(object):
-    # 正常售后单
-    NORMAL = "normal"
-    # 换货
-    EXCHANGE= "exchange"
-    # 投诉
-    COMPLAINT = "complaint"
-    # 催货
-    REMINDER = "reminder"
-    # 仅退运费
-    ONLY_REFUND_POSTAGE = "only_refund_postage"
+
+class OrderActions(object):
+    # 售后单独有一个Note表
+    # 负库存相关单独有一个Note表
+    # 修改
+    MODIFY_ADDRESS = "modify_address"
+    # 修改客服备注
+    MODIFY_OPERATOR_NOTE = "modify_operator_note"
+    # 关闭订单
+    CLOSE = "close"
+    # 发起支付
+    PAY = "pay"
+    # 完成支付订单
+    COMPLETE_PAYMENT = "complete_payment"
+    # 发货
+    SEND = "send"
+    # 用户提货
+    TAKE = "take"
     # 其他
-    OTHER = "other"
-    # 退定金
-    REFUND_DEPOIST = "refund_deposit"
-    # 退海淘
-    REFUND_HAITAO = "refund_haitao"
-    # 仅退差价
-    ONLY_REFUND = "onlyrefund"
-
-    # 特殊售后单快递转自提退运费
-    AFSPLUS_REFUND_POSTAGE = "afsplus_refund_postage"
-    # 抖音生活退券售后
-    TIKAL = "tikal"
-
-    CHOICES = (
-        (NORMAL, "退货退款"),
-        (EXCHANGE, "换货"),
-        (COMPLAINT, "投诉"),
-        (REMINDER, "提醒发货"),
-        (ONLY_REFUND_POSTAGE, "仅退运费"),
-        (REFUND_DEPOIST, "退定金"),
-        (REFUND_HAITAO, "退海淘"),
-        (OTHER, "其他"),
-        (ONLY_REFUND, "仅退差价"),
-        (AFSPLUS_REFUND_POSTAGE, "退运费"),
-        (TIKAL, "抖音生活退券"),
+    OTHERS = "others"
+    # 创建订单
+    CREATE = "create"
+    # 生成发货单
+    GENERATE_DISTRIBUTE = "generate_distribute"
+    # 给客户发短信
+    SEND_SMS_MESSAGE = "send_sms_message"
+
+
+class OrderTypes(object):
+    # 线上订单
+    ONLINE = "online"
+    # 闪购
+    FLASHSALE = "flashsale"
+    # 贩卖机类型，现场直接出货
+    VENDING = "vending"
+    # 贩卖机类型，现场直接出货： 样机种草
+    VENDING_MACHINE_HR = "vending_machine_hr"
+    # 互动触摸屏类型，提货需要到专柜
+    SCREEN = "screen"
+    # rfid 订单类型
+    RFID = "rfid"
+    # 拼团订单
+    GROUP = "group"
+    # 积分商城
+    POINTS_MALL = "points_mall"
+    # 汉光贩售机
+    HGVENDING = "hgvending"
+    # 海淘
+    HAITAO = "haitao"
+
+    ORDER_TYPES_CHOICES = (
+        (ONLINE, "线上订单"),
+        (FLASHSALE, "闪购订单"),
+        (VENDING, "售货机自提"),
+        (VENDING_MACHINE_HR, "样机种草"),
+        (SCREEN, "互动触摸屏"),
+        (RFID, "RFID"),
+        (GROUP, "拼团订单"),
+        (HGVENDING, "汉光贩售机"),
+        (HAITAO, "海淘"),
     )
 
-class AfterSaleReasons(object):
-    """
-    用户售后原因
-    """
-    # 催单
-    REMINDER = "reminder"
-    # 退运费
-    RETURN_POST = "return_post"
-    # 不喜欢/不想要了
-    NOT_LIKE_OR_NOT_WANT = "not_like_or_not_want"
-    # 快递太慢了不想等了
-    SHIPPING_TOO_SLOW_AND_NO_WAIT= "shipping_too_slow_and_no_wait"
-    # 快递太慢，帮我催一下
-    SHIPPING_TOO_SLOW_AND_REMINDER= "shipping_too_slow_reminder"
-    # 换货：质量问题
-    EXCHANGE_PRODUCT_QUALITY_ISSUE = "exchange_product_quality_issue"
-    # 退货：质量问题
-    RETURN_PRODUCT_QUALITY_ISSUE = "return_product_quality_issue"
-    # 退货：不喜欢，不想要了
-    RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT = "return_product_not_like_or_not_want"
-    # 退货：穿着不合适需退货
-    RETURN_PRODUCT_INAPPROPRIATE = "return_product_inappropriate"
-    # 换货：大小/款式不合适
-    EXCHANGE_PRODUCT_INAPPROPRIATE = "exchange_inappropriate"
-    # 退货：商品与描述不符
-    RETURN_PRODUCT_DESCRIPTION_MISMATCH = "return_product_description_mismatch"
-    # 其他
-    OTHER = "other"
-    ##其他前缀，用来做过滤查询
-    OTHER_PREFIX = "其他-"
-    ###############
-    # 客人不想要了
-    CUSTOMER_NOT_WANT = "customer_not_want"
-    # 商品缺货，不想等了
-    PRODUCT_LACK_NO_WAIT = "product_lack_no_wait"
-    # 订单不能按预计时间送达
-    ORDER_CANNOT_SHIPPING_ONTIME = "order_cannot_shipping_ontime"
-    # 操作有误（商品、地址等选错）
-    OPERATE_ERROR = "operate_error"
-    # 重复下单/误下单
-    ORDER_DUPLICATE = "order_duplicate"
-    # 其他渠道价格更低
-    CHIPPER_ON_OTHER_CHANNEL = "chipper_on_other_channel"
-    # 该商品降价了
-    CHIPPER_NOW = "chipper_now"
-    # 重新下单买（商品/数量拍错了）
-    ORDER_DUPLICATE2 = "order_duplicate2"
-    # 不想买了
-    NOT_WANT_ANYMORE = "not_want_anymore"
-    # 用户整单退
-    USER_ENTIRE_RETURN = "user_entire_return"
-    # 整单退
-    ENTIRE_RETURN = "entire_return"
-    # 买多了/买错了
-    BOUGHT_TOO_MUCH = "bought_too_much"
-    # 计划有变，暂时不需要了
-    PLAN_CHANGED = "plan_changed"
-    #信息填错
-    INFORMATION_ERROR = "information_error"
-    #无法绑卡
-    CAN_NOT_BIND_CARD = "can_not_bind_card"
-    #发票问题
-    INVOICE_ISSUE = "invoice_issue"
 
-AFTERSALE_ALL_REASON_DICT = {
-    AfterSaleReasons.REMINDER: "提醒发货",
-    AfterSaleReasons.RETURN_POST: "退运费",
-    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT: "不喜欢/不想要了",
-    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT: "快递太慢了不想等了",
-    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_REMINDER: '快递太慢，帮我催一下',
-    AfterSaleReasons.EXCHANGE_PRODUCT_INAPPROPRIATE: '换货：大小/款式不合适',
-    AfterSaleReasons.EXCHANGE_PRODUCT_QUALITY_ISSUE:'换货：质量问题',
-    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE: '退货：质量问题',
-    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE: '退货：穿着不合适需退货',
-    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT: '商品缺货',
-    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH: '退货：商品与描述不符',
-    AfterSaleReasons.CUSTOMER_NOT_WANT:"客人不想要了",
-    AfterSaleReasons.PRODUCT_LACK_NO_WAIT: "商品缺货，不想等了",
-    AfterSaleReasons.ORDER_CANNOT_SHIPPING_ONTIME: "订单不能按预计时间送达",
-    AfterSaleReasons.OPERATE_ERROR: "操作有误（商品、地址等选错）",
-    AfterSaleReasons.ORDER_DUPLICATE: "重复下单/误下单",
-    AfterSaleReasons.CHIPPER_ON_OTHER_CHANNEL:"其他渠道价格更低",
-    AfterSaleReasons.CHIPPER_NOW:"该商品降价了",
-    AfterSaleReasons.ORDER_DUPLICATE2: "重新下单买（商品/数量拍错了）",
-    AfterSaleReasons.NOT_WANT_ANYMORE: "不想买了",
-    AfterSaleReasons.USER_ENTIRE_RETURN: "用户整单退",
-    AfterSaleReasons.ENTIRE_RETURN: "整单退",
-    AfterSaleReasons.OTHER: "其他",
-    # 买多了/买错了
-    AfterSaleReasons.BOUGHT_TOO_MUCH: "买多了/买错了",
-    # 计划有变，暂时不需要了
-    AfterSaleReasons.PLAN_CHANGED: "计划有变，暂时不需要了",
-    # 信息填错
-    AfterSaleReasons.INFORMATION_ERROR: "信息填错",
-    # 无法绑卡
-    AfterSaleReasons.CAN_NOT_BIND_CARD: "无法绑卡",
-    # 发票问题
-    AfterSaleReasons.INVOICE_ISSUE: "发票问题",
-}
+class OrderShippingMethods(object):
 
-# 用户售后原因list
-AFTERSALE_USER_REASON_LIST = [
-    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT,
-    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT,
-    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT,
-    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE,
-    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE,
-    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH,
-    AfterSaleReasons.RETURN_POST,
-    AfterSaleReasons.OTHER,
-]
-# 用户售后原因dict
-AFTERSALE_USER_REASON_DICT = { item: AFTERSALE_ALL_REASON_DICT[item] for item in AFTERSALE_USER_REASON_LIST }
-
-# E卡售后原因list
-AFTERSALE_USER_REASON_HG_ECARD_LIST = [
-    # 买多了/买错了
-    AfterSaleReasons.BOUGHT_TOO_MUCH,
-    # 计划有变，暂时不需要了
-    AfterSaleReasons.PLAN_CHANGED,
-    # 信息填错
-    AfterSaleReasons.INFORMATION_ERROR,
-    # 无法绑卡
-    AfterSaleReasons.CAN_NOT_BIND_CARD,
-    # 发票问题
-    AfterSaleReasons.INVOICE_ISSUE,
-]
-# E卡售后原因dict
-AFTERSALE_USER_REASON_HG_ECARD_DICT = { item: AFTERSALE_ALL_REASON_DICT[item] for item in AFTERSALE_USER_REASON_HG_ECARD_LIST }
+    SELF_SERVICE = "self_service"
+    EXPRESS = "express"
 
 
+class OrderStatus(object):
+    """订单对外展示状态"""
+    # 2018-02-08 确定新的四个统一订单对外状态
+    # 待付款
+    UNPAID = "unpaid"
+    # 准备中
+    PREPARING = "preparing"
+    # 可提货，待发货
+    TO_DELIVER = "to_deliver"
+    # 已发货，已完成
+    COMPLETED = "completed"
+    # 已关闭/取消
+    CLOSED = "closed"
+    # 订单不再筛选售后状态！
+
+    # 售后
+    AFTERSALE = "after_sale"
+    # 待发货
+    TO_SHIP = "to_ship"
+    # 可自提
+    TO_PICKUP = "to_pickup"
+
+    # 待付款
+    # UNPAID = "unpaid"
+    # # 备货中
+    # IN_PREPARING = "in_preparing"
+    # # 待发货
+    # TO_SEND = "to_send"
+    # # 待提货
+    # TO_TAKE = "to_take"
+    # # 部分发货
+    # PARTIALLY_SENT = "partially_sent"
+    # # 已发货
+    # SENT = "sent"
+    # # 部分提货
+    # PARTIALLY_TAKEN = "partially_taken"
+    # # 已提货
+    # TAKEN = "taken"
+    # # 退换/售后
+    # IN_AFTERSALE = "in_aftersale"
+    # # 已关闭/取消
+    # CLOSED = "closed"
+
+
+class OrderPayStatus(object):
+    # 订单支付状态
+    UNPAID = "unpaid"
+    PAY_FINISHED = "pay_finished"
+    CLOSED = "closed"
+    # ------------- 分阶段支付 --------------
+    # 定金待支付
+    TO_DEPOSITPAY = "to_depositpay"
+    # 尾款待支付
+    TO_TAILPAY = "to_tailpay"
+    # 尾款超时
+    TAILPAY_OVERTIME = "tailpay_overtime"
+
+    ORDER_PAY_STATUS_CHOICE = (
+        (UNPAID, "未支付"),
+        (PAY_FINISHED, "支付完成"),
+        (CLOSED, "已关闭"),
+        (TO_DEPOSITPAY, "待支付定金"),
+        (TO_TAILPAY, "待支付尾款"),
+        (TAILPAY_OVERTIME, "尾款超时"),
+    )
+    ORDER_PAY_STATUS_DICT = dict(ORDER_PAY_STATUS_CHOICE)
+
+
+class OrderGroupStatus(object):
+    # 拼团中
+    PROGRESS = "progress"
+    # 已成团
+    SUCCESS = "success"
+    # 拼团失败
+    FAIL = "fail"
+
+
+class OrderAssignStatus(object):
+    '''订单配货状态'''
+    # 无配货 - 没有ready或completed的发货单，或者说没有发货单或发货单只有closed的
+    INIT = "init"
+    # 部分配货 - 有ready的发货单，但是ready的发货单里的line的总数总量不全
+    PARTIAL = "partial"
+    # 全部配货 - 有不是closed的发货单，全部发货单里全部line数量总量和订单一致
+    COMPLETED = "completed"
+
+
+class OrderShippingStatus(object):
+    '''订单发货状态'''
+    # 未发货 - 没有completed的发货单
+    INIT = "init"
+    # 部分发货 - 有completed的发货单，里面的line总量不全
+    PARTIAL = "partial"
+    # 全部发货 - completed的发货单里面的line总量和订单一致
+    COMPLETED = "completed"
+
+
+class OrderAftersaleStatus(object):
+    # 订单售后状态
+    # 有待处理售后
+    OPEN = "open"
+    # 无售后
+    NONE = "none"
+    # 售后都完成（因为同时open的售后单只会有一单）
+    DONE = "done"
+
+
+class OrderExchangeStatus(object):
+    '''### 订单换货状态###'''
+    # 有待处理售后
+    OPEN = "open"
+    # 无售后
+    NONE = "none"
+    # 换货都完成（因为同时open的换货单只会有一单）
+    DONE = "done"
+    # 配货状态
+    EXCHANGE_STATUS = (
+        (OPEN, "有在进行的换货"),
+        (NONE, "无换货"),
+        (DONE, "换货已完成"),
+    )
 
 
 class AftersaleStatus(object):
 
     # 财务待审
     IN_FINANCE = "in_finance"
     # 财务一审通过，待二审
     IN_FINANCE_2ND = "in_finance_2nd"
-    # 财务驳回, 目前这个状态仅在抖店售后在抖店平台拒绝时使用
+    # 财务驳回
     REJECTED = "rejected"
     # 店内通过的售后单状态们
     # AFTER_APPROVES = [ALL_APPROVED, REFUND_FAILED, COMPLETED]
     # IN_OPENS = [OPEN, IN_FINANCE, IN_FINANCE_2ND, REJECTED, INSTORE_REJECTED]
-    ######以上为需求v190611之前的状态，现在不用了,但必须保留做兼容#########
+    ######  以上为需求v190611之前的状态，现在不用了,但必须保留做兼容#########
 
     # 待审核/审核中
     OPEN = "open"
     # 待退货
-    PENDING_RETURN = "pending_return" 
-    PENDING_RETURN_0 = "pending_return_0" # For C端， 待客服退货，此状态，在数据库中并不存在
-    PENDING_RETURN_1 = "pending_return_1" # For C端， 待客人退货，此状态，在数据库中并不存在
-    PENDING_RETURN_2 = "pending_return_2" # For C端， 待外仓退货，此状态，在数据库中并不存在
+    PENDING_RETURN = "pending_return"
+    PENDING_RETURN_0 = "pending_return_0"  # For C端， 待客服退货，此状态，在数据库中并不存在
+    PENDING_RETURN_1 = "pending_return_1"  # For C端， 待客人退货，此状态，在数据库中并不存在
+    PENDING_RETURN_2 = "pending_return_2"  # For C端， 待外仓退货，此状态，在数据库中并不存在
     # 待退款
     PENDING_REFUND = "pending_refund"
     # 店内系统通过
     INSTORE_APPROVED = "instore_approved"
     # 店内系统驳回
     INSTORE_REJECTED = "instore_rejected"
     # 已完成主流程，不涉及退款 —— 这是一个中间状态，退款的时候用来校验
@@ -392,41 +319,33 @@
     # 退款失败
     REFUND_FAILED = "refund_failed"
     # 已完成
     COMPLETED = "completed"
     # 已取消，已关闭
     CLOSED = "closed"
 
-    # 2022.07 售后单和发货单解耦新增中间状态
-    OPENING = 'opening'  # 申请中
-    CLOSING = 'closing'  # 关闭中
-    COMPLETING = 'completing'  # 完成中
-    OPEN_FAILED = 'open_failed'  # 申请售后失败
-    CLOSE_FAILED = 'close_failed'  # 关闭售后失败
-    COMPLETE_FAILED = 'complete_failed'  # 完成售后失败
-
     AFTERSALE_STATUS_CHOICES = (
         (OPEN, "待审核"),
         # (IN_FINANCE, "财务待审"),
         # (IN_FINANCE_2ND, "财务一审通过"),
-        (REJECTED, "客服驳回"),
+        # (REJECTED, "财务驳回"),
         (PENDING_RETURN, "待退货"),
         (PENDING_REFUND, "待退款"),
         (INSTORE_APPROVED, "店内系统通过"),
         (INSTORE_REJECTED, "店内系统驳回"),
         (ALL_APPROVED, "店内系统通过"),
         (REFUND_FAILED, "退款失败"),
         (COMPLETED, "已完成"),
         (CLOSED, "已取消"),
     )
     AFTERSALE_STATUS_CHOICES_FOR_C = (
         (OPEN, "待审核"),
-        (PENDING_RETURN_0, "待审核"), # 待客服退货
-        (PENDING_RETURN_1, "待退货"), # 待客人退货
-        (PENDING_RETURN_2, "待退货"), # 发货拦截中
+        (PENDING_RETURN_0, "待审核"),  # 待客服退货
+        (PENDING_RETURN_1, "待退货"),  # 待客人退货
+        (PENDING_RETURN_2, "待退货"),  # 发货拦截中
         (PENDING_REFUND, "待退款"),
         (INSTORE_APPROVED, "待退款"),
         (INSTORE_REJECTED, "待退款"),
         (ALL_APPROVED, "待退款"),
         (REFUND_FAILED, "待退款"),
         (COMPLETED, "已完成"),
         (CLOSED, "已关闭"),
@@ -470,36 +389,350 @@
 class AftersaleFinanceType(object):
     '''一期有一些需要财务手动调账的'''
     # 普普通通的售后单
     AUTO = "auto"
     # 需要财务手动调账的售后单，微信不能自动退款
     MANUAL = "manual"
 
-class AftersaleSource(object):
-    """
-    售后来源
-    """
-    # 客人发起
-    GUEST_INITIATED = "guest_initiated"
-    # 客服发起
-    SERVICE_INITIATED = "service_initiated"
 
-class AftersaleCancelSource(object):
+class CancelSource(object):
     """
     售后取消来源
     """
     # 客人取消
     GUEST_CANCEL = "guest_cancel"
     # 客服取消
     SERVICE_CANCEL = "service_cancel"
     # 高级客服取消
     SUPER_SERVICE_CANCEL = "super_service_cancel"
     # 超时自动取消
     TIMEOUT_CANCEL = "timeout_cancel"
 
-class AftersaleRefundStatus(object):
+
+class RefundStatus(object):
     # 未退款，初始状态
     INIT = "init"
     # 退款成功
     SUCCEEDED = "succeeded"
     # 退款失败
     FAILED = "failed"
+
+
+class CouponSource(object):
+    # 线上发的券
+    ONLINE = "online"
+    # 店内发的券
+    IN_STORE = "store"
+
+
+class ProductSaleType(object):
+    # 实物类型
+    REAL = "REAL"
+
+    # 虚拟商品
+    VIRTUAL = "VIRTUAL"
+
+
+class SettingsLabel(object):
+    """
+    系统配置
+    """
+    # 客服主管拦截
+    SUPERVISOR_INTERCEPTION = "supervisor_interception"
+
+
+class InnerApiUri(object):
+    ALIPAY = "/api/sparrow_alipay/i/alipay_aftersale_returned/"
+    REFUND_QUERY = "/api/sparrow_alipay/i/alipay_aftersale_returned_query/"
+    PRODUCT = "/api/sparrow_products_i/pure_products/{}/"
+
+
+class ErrorCode(object):
+    SUCCESS = 0  # 成功
+    FLASH_HAS_PICKUP = 201001  # 闪购订单已提货，不能发起退单。
+    HAS_VALID_AFTERSALE = 201002  # 此订单已发起售后
+    HAS_VALID_ASSIGNMENT = 201003  # 此订单已配货，请点击申请售后
+    REFUND_ERROR = 201004  # 退款失败
+
+
+class BatchAssignType(object):
+    '''订单配货类型'''
+    # 全部配货
+    WHOLE = "whole"
+    # 部分配货
+    PARTIAL = "partial"
+    # 按商品部分配货
+    PRODUCT = "product"
+    # 按专柜部分配货
+    SHOP = "shop"
+
+
+class BatchAssignTaskStatus(object):
+    '''订单配货任务执行状态'''
+    # 正在进行中
+    IN_PROGRESS = "in_progress"
+    # 已经完成
+    COMPLETED = "completed"
+    # 执行出错
+    ERROR = "error"
+
+
+class AfterSaleType(object):
+    # 正常售后单
+    NORMAL = "normal"
+    # 换货
+    EXCHANGE = "exchange"
+    # 投诉
+    COMPLAINT = "complaint"
+    # 催货
+    REMINDER = "reminder"
+    # 仅退运费
+    ONLY_REFUND_POSTAGE = "only_refund_postage"
+    # 其他
+    OTHER = "other"
+
+
+class AfterSaleReasons(object):
+    # 催单
+    REMINDER = "reminder"
+    # 退运费
+    RETURN_POST = "return_post"
+    # 不喜欢/不想要了
+    NOT_LIKE_OR_NOT_WANT = "not_like_or_not_want"
+    # 快递太慢了不想等了
+    SHIPPING_TOO_SLOW_AND_NO_WAIT = "shipping_too_slow_and_no_wait"
+    # 快递太慢，帮我催一下
+    SHIPPING_TOO_SLOW_AND_REMINDER = "shipping_too_slow_reminder"
+    # 换货：质量问题
+    EXCHANGE_PRODUCT_QUALITY_ISSUE = "exchange_product_quality_issue"
+    # 退货：质量问题
+    RETURN_PRODUCT_QUALITY_ISSUE = "return_product_quality_issue"
+    # 退货：不喜欢，不想要了
+    RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT = "return_product_not_like_or_not_want"
+    # 退货：穿着不合适需退货
+    RETURN_PRODUCT_INAPPROPRIATE = "return_product_inappropriate"
+    # 换货：大小/款式不合适
+    EXCHANGE_PRODUCT_INAPPROPRIATE = "exchange_inappropriate"
+    # 退货：商品与描述不符
+    RETURN_PRODUCT_DESCRIPTION_MISMATCH = "return_product_description_mismatch"
+    # 其他
+    OTHER = "other"
+    ##  其他前缀，用来做过滤查询
+    OTHER_PREFIX = "其他-"
+    ###############
+    # '客人不想要了',
+    CUSTOMER_NOT_WANT = "customer_not_want"
+    # '商品缺货，不想等了',
+    PRODUCT_LACK_NO_WAIT = "product_lack_no_wait"
+    # '订单不能按预计时间送达',
+    ORDER_CANNOT_SHIPPING_ONTIME = "order_cannot_shipping_ontime"
+    # '操作有误（商品、地址等选错）',
+    OPERATE_ERROR = "operate_error"
+    # '重复下单/误下单',
+    ORDER_DUPLICATE = "order_duplicate"
+    # '其他渠道价格更低',
+    CHIPPER_ON_OTHER_CHANNEL = "chipper_on_other_channel"
+    # '该商品降价了',
+    CHIPPER_NOW = "chipper_now"
+    # 重新下单买（商品/数量拍错了）
+    ORDER_DUPLICATE2 = "order_duplicate2"
+    # 不想买了
+    NOT_WANT_ANYMORE = "not_want_anymore"
+    # 用户整单退
+    USER_ENTIRE_RETURN = "user_entire_return"
+    # 整单退
+    ENTIRE_RETURN = "entire_return"
+
+
+AFTERSALE_USER_REASON_DICT = {
+    AfterSaleReasons.REMINDER: "提醒发货",
+    AfterSaleReasons.RETURN_POST: "退运费",
+    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT: "不喜欢/不想要了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT: "快递太慢了不想等了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_REMINDER: '快递太慢，帮我催一下',
+    # AfterSaleReasons.EXCHANGE_PRODUCT_INAPPROPRIATE: '换货：大小/款式不合适',
+    # AfterSaleReasons.EXCHANGE_PRODUCT_QUALITY_ISSUE:'换货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE: '退货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE: '退货：穿着不合适需退货',
+    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT: '退货：不喜欢，不想要了',
+    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH: '退货：商品与描述不符',
+    AfterSaleReasons.OTHER: "其他",
+
+}
+
+AFTERSALE_ALL_REASON_DICT = {
+    AfterSaleReasons.REMINDER: "提醒发货",
+    AfterSaleReasons.RETURN_POST: "退运费",
+    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT: "不喜欢/不想要了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT: "快递太慢了不想等了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_REMINDER: '快递太慢，帮我催一下',
+    AfterSaleReasons.EXCHANGE_PRODUCT_INAPPROPRIATE: '换货：大小/款式不合适',
+    AfterSaleReasons.EXCHANGE_PRODUCT_QUALITY_ISSUE: '换货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE: '退货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE: '退货：穿着不合适需退货',
+    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT: '退货：不喜欢，不想要了',
+    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH: '退货：商品与描述不符',
+    AfterSaleReasons.CUSTOMER_NOT_WANT: "客人不想要了",
+    AfterSaleReasons.PRODUCT_LACK_NO_WAIT: "商品缺货，不想等了",
+    AfterSaleReasons.ORDER_CANNOT_SHIPPING_ONTIME: "订单不能按预计时间送达",
+    AfterSaleReasons.OPERATE_ERROR: "操作有误（商品、地址等选错）",
+    AfterSaleReasons.ORDER_DUPLICATE: "重复下单/误下单",
+    AfterSaleReasons.CHIPPER_ON_OTHER_CHANNEL: "其他渠道价格更低",
+    AfterSaleReasons.CHIPPER_NOW: "该商品降价了",
+    AfterSaleReasons.ORDER_DUPLICATE2: "重新下单买（商品/数量拍错了）",
+    AfterSaleReasons.NOT_WANT_ANYMORE: "不想买了",
+    AfterSaleReasons.USER_ENTIRE_RETURN: "用户整单退",
+    AfterSaleReasons.ENTIRE_RETURN: "整单退",
+    AfterSaleReasons.OTHER: "其他"
+
+}
+
+
+class HGVendingStatus(object):
+    # 初始态
+    INIT = "init"
+    # 已取货
+    PICKED_UP = "picked_up"
+    # 已售后
+    REFUND = "refund"
+    # 超时未支付关闭
+    CLOSED = "closed"
+
+    HGVENDING_STATUS_CHOICES = (
+        (INIT, "初始态"),
+        (PICKED_UP, "已取货"),
+        (REFUND, "已售后"),
+        (CLOSED, "已关闭")
+    )
+
+
+# 贩售机取货码过期检测定时任务运行间隔
+HGVENDING_BULK_TASK_INTERVAL = 15 * 60
+
+
+class DeliverTimeType(object):
+    '''
+    发货时间类型(fixed_time 固定时间/pay_relative_time 支付相对时间)
+    '''
+    FIXED_TIME = "fixed_time"
+    PAY_RELATIVE_TIME = "pay_relative_time"
+    DELIVERTIME_TYPE_CHOICES = (
+        (FIXED_TIME, "固定时间"),
+        (PAY_RELATIVE_TIME, "支付相对时间")
+    )
+
+
+class PayMethod(object):
+    '''支付方法（once 一次支付/twice两次支付）'''
+    ONCE = "once"
+    TWICE = "twice"
+    PAY_METHOD_CHOICES = (
+        (ONCE, "一次支付"),
+        (TWICE, "两次支付")
+    )
+
+
+class DeliverTimeStatus(object):
+    '''发货时间配置状态(none无需配置/to_configure待配置/configured已配置)'''
+    NONE = "none"
+    TO_CONFIGURE = "to_configure"
+    CONFIGURED = "configured"
+    DELIVERTIME_STATUS_CHOICES = (
+        (NONE, "无需配置"),
+        (TO_CONFIGURE, "待配置"),
+        (CONFIGURED, "已配置")
+    )
+
+
+class PayStepType(object):
+    '''支付阶段类型(all全款/deposit定金/tailpay尾款)'''
+    ONCE = "once"
+    DEPOSIT = "deposit"
+    TAIL = "tail"
+    PAY_STEP_TYPE_CHOICES = (
+        (ONCE, "全款"),
+        (DEPOSIT, "定金"),
+        (TAIL, "尾款")
+    )
+
+
+STEP_CHAR = "&"
+
+
+class AssignmentStatus(object):
+    '''发货单邮寄状态'''
+    # 只要创建了发货单就认为是配货了
+    # 已配货，待发货（无快递单号）或待提货
+    READY = "ready"
+    # 已完成-有快递单号了，或者用户来自提了
+    COMPLETED = "completed"
+    # 已取消
+    # 发货单不能删除，只能关闭取消
+    CLOSED = "closed"
+
+
+class AftersaleSource(object):
+    """
+    售后来源
+    """
+    # 客人发起
+    GUEST_INITIATED = "guest_initiated"
+    # 客服发起
+    SERVICE_INITIATED = "service_initiated"
+
+
+AFTERSALE_USER_REASON_DICT = {
+    AfterSaleReasons.REMINDER: "提醒发货",
+    AfterSaleReasons.RETURN_POST: "退运费",
+    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT: "不喜欢/不想要了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT: "快递太慢了不想等了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_REMINDER: '快递太慢，帮我催一下',
+    # AfterSaleReasons.EXCHANGE_PRODUCT_INAPPROPRIATE: '换货：大小/款式不合适',
+    # AfterSaleReasons.EXCHANGE_PRODUCT_QUALITY_ISSUE:'换货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE: '退货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE: '退货：穿着不合适需退货',
+    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT: '退货：不喜欢，不想要了',
+    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH: '退货：商品与描述不符',
+    AfterSaleReasons.OTHER: "其他",
+}
+
+AFTERSALE_ALL_REASON_DICT = {
+    AfterSaleReasons.REMINDER: "提醒发货",
+    AfterSaleReasons.RETURN_POST: "退运费",
+    AfterSaleReasons.NOT_LIKE_OR_NOT_WANT: "不喜欢/不想要了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_NO_WAIT: "快递太慢了不想等了",
+    AfterSaleReasons.SHIPPING_TOO_SLOW_AND_REMINDER: '快递太慢，帮我催一下',
+    AfterSaleReasons.EXCHANGE_PRODUCT_INAPPROPRIATE: '换货：大小/款式不合适',
+    AfterSaleReasons.EXCHANGE_PRODUCT_QUALITY_ISSUE: '换货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_QUALITY_ISSUE: '退货：质量问题',
+    AfterSaleReasons.RETURN_PRODUCT_INAPPROPRIATE: '退货：穿着不合适需退货',
+    AfterSaleReasons.RETURN_PRODUCT_NOT_LIKE_OR_NOT_WANT: '退货：不喜欢，不想要了',
+    AfterSaleReasons.RETURN_PRODUCT_DESCRIPTION_MISMATCH: '退货：商品与描述不符',
+    AfterSaleReasons.CUSTOMER_NOT_WANT: "客人不想要了",
+    AfterSaleReasons.PRODUCT_LACK_NO_WAIT: "商品缺货，不想等了",
+    AfterSaleReasons.ORDER_CANNOT_SHIPPING_ONTIME: "订单不能按预计时间送达",
+    AfterSaleReasons.OPERATE_ERROR: "操作有误（商品、地址等选错）",
+    AfterSaleReasons.ORDER_DUPLICATE: "重复下单/误下单",
+    AfterSaleReasons.CHIPPER_ON_OTHER_CHANNEL: "其他渠道价格更低",
+    AfterSaleReasons.CHIPPER_NOW: "该商品降价了",
+    AfterSaleReasons.ORDER_DUPLICATE2: "重新下单买（商品/数量拍错了）",
+    AfterSaleReasons.NOT_WANT_ANYMORE: "不想买了",
+    AfterSaleReasons.USER_ENTIRE_RETURN: "用户整单退",
+    AfterSaleReasons.ENTIRE_RETURN: "整单退",
+    AfterSaleReasons.OTHER: "其他",
+}
+
+
+class Order_Number_Pay_Status(object):
+    # 子支付单状态(init初始/doing进行中/done已完成)
+    INIT = "init"
+    DOING = "doing"
+    DONE = "done"
+    FAILED = "failed"
+    ORDER_NUMBER_PAY_STATUS_CHOICES = (
+        (INIT, '初始'),
+        (DOING, '进行中'),
+        (DONE, "已完成"),
+        (FAILED, "失败"),
+
+    )
+    ORDER_NUMBER_PAY_STATUS_DICT = dict(ORDER_NUMBER_PAY_STATUS_CHOICES)
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_aftersale/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_aftersale/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 from django.db import models
 from django.db.models import Sum
 from django.core import validators
 from django.contrib.auth import get_user_model
 from django.utils.functional import cached_property
 
 from ..core.constants import PayType
-from ..core.constants import ReturnQuantityType
-from ..sparrow_shipping.constants import ShippingPartnerCodes
+from ..core.constants import ShippingPartnerCodes_DICT
 from ..core.base_models import BaseModelTimeAndDeleted
 from ..core.model_function import get_object_or_None
 from ..core.common_utils import get_uuid4_hex
-from ..sparrow_aftersale.constants import AftersaleFinanceStatus
-from ..sparrow_aftersale.constants import AftersaleRefundStatus
-from ..sparrow_aftersale.constants import AftersaleStatus
-from ..sparrow_aftersale.constants import AftersaleFinanceType
-from ..sparrow_aftersale.constants import AftersaleSource
-from ..sparrow_aftersale.constants import AftersaleCancelSource
-from ..sparrow_aftersale.constants import AftersaleActions
-from ..sparrow_aftersale.constants import AfterSaleType
-from ..sparrow_aftersale.constants import AfsLineStatus
+from ..sparrow_orders.constants import AftersaleFinanceStatus
+from ..sparrow_orders.constants import RefundStatus
+from ..sparrow_orders.constants import AftersaleStatus
+from ..sparrow_orders.constants import AftersaleFinanceType
+from ..sparrow_orders.constants import AftersaleSource
+from ..sparrow_orders.constants import CancelSource
+from ..sparrow_orders.constants import AftersaleActions
 from ..sparrow_orders.constants import CouponSource
+from ..sparrow_orders.constants import AfterSaleType
 from ..sparrow_orders.constants import PayStepType
 from ..sparrow_orders.constants import PayMethod
 from ..sparrow_orders.models import generate_aftersale_number
 from ..sparrow_orders.models import OrderPayment
 from ..sparrow_orders.models import Order
 from ..sparrow_orders.models import Line
 from ..sparrow_orders.models import LineOrderPromotion
@@ -56,17 +54,14 @@
     'AfsAlipayRefund',
     'DeliveryReturn',
     'AfsHgIncome',
     'AfsHgIncomeDivide',
     'VLines',
     'VLinePayment',
     'VLinePromotion',
-    'QueryResult',
-    'QueryResultTicket',
-    'QueryResultDetail',
 ]
 
 
 class Afs(BaseModelTimeAndDeleted):
     '''
     售后单
     和 Line 是多对多的关系
@@ -78,30 +73,30 @@
     AFTERSALE_FINANCE_STATUS_CHOICES = (
         (AftersaleFinanceStatus.INIT, "财务未审"),
         (AftersaleFinanceStatus.APPROVED_1ST, "财务一审通过，待二审"),
         (AftersaleFinanceStatus.APPROVED, "财务二审通过"),
         (AftersaleFinanceStatus.REJECTED, "财务驳回")
     )
     REFUND_STATUS_CHOICES = (
-        (AftersaleRefundStatus.INIT, "未退款"),
-        (AftersaleRefundStatus.SUCCEEDED, "退款成功"),
-        (AftersaleRefundStatus.FAILED, "退款失败")
+        (RefundStatus.INIT, "未退款"),
+        (RefundStatus.SUCCEEDED, "退款成功"),
+        (RefundStatus.FAILED, "退款失败")
     )
     AFTERSALE_FINANCE_TYPE_CHOICES = (
         (AftersaleFinanceType.AUTO, "正常退单"),
         (AftersaleFinanceType.MANUAL, "需要财务手动调账退款"),
     )
     AFTERSALE_SOURCE_CHOICES = (
         (AftersaleSource.GUEST_INITIATED, "客人发起"),
         (AftersaleSource.SERVICE_INITIATED, "客服发起"),
     )
     CANCEL_SOURCE_CHOICES = (
-        (AftersaleCancelSource.GUEST_CANCEL, "客人取消"),
-        (AftersaleCancelSource.SERVICE_CANCEL, "客服取消"),
-        (AftersaleCancelSource.TIMEOUT_CANCEL, "超时自动取消"),
+        (CancelSource.GUEST_CANCEL, "客人取消"),
+        (CancelSource.SERVICE_CANCEL, "客服取消"),
+        (CancelSource.TIMEOUT_CANCEL, "超时自动取消"),
     )
     AFTERSALE_TYPE_CHOICES = (
         (AfterSaleType.NORMAL, "正常退款"),
         (AfterSaleType.EXCHANGE, "换货"),
         (AfterSaleType.COMPLAINT, "投诉"),
         (AfterSaleType.REMINDER, "提醒发货"),
         (AfterSaleType.ONLY_REFUND_POSTAGE, "仅退运费"),
@@ -148,15 +143,15 @@
     # 退款状态
     refund_status = models.CharField(
         "退款状态",
         max_length=128,
         choices=REFUND_STATUS_CHOICES,
         blank=True,
         null=True,
-        default=AftersaleRefundStatus.INIT)
+        default=RefundStatus.INIT)
     # 财务要的退款时间，找财务确认是要发起微信退款的时间还是微信退款到账的时间
     # 应该是调起微信退款接口的时间
     refund_time = models.DateTimeField("发起退款的时间", blank=True, null=True, db_index=True)
     # 收到推送退款成功的时间，一期就是收到微信通知成功的时间
     refund_notified_time = models.DateTimeField("退款收到推送的时间", blank=True, null=True, db_index=True)
     # 售后单同步信息
     sync_status = models.BooleanField('同步状态', default=False)
@@ -230,26 +225,14 @@
 
     # 支付方法（once 一次支付/twice两次支付）
     pay_method = models.CharField("支付方法", max_length=24, choices=PayMethod.PAY_METHOD_CHOICES, blank=True, null=True, default=PayMethod.ONCE)
 
     # 退货重算-售后单版本号
     afs_version = models.CharField("售后版本号", max_length=12, blank=True, null=True, db_index=True, default=AfsVersionConst.V2)
 
-    # V3售后是否重新计算
-    if_recomputed_v3 = models.BooleanField("V3售后是否重新计算", null=True, default=None)
-
-    # 2022.08 售后单表头冗余商品总数量、退款总金额
-    total_quantity = models.IntegerField('商品总数量', null=True, blank=True, default=0)
-    # refund_amount 退款总金额, 包含各种支付别, 不包含 postage
-    refund_amount = models.DecimalField("refund_amount", decimal_places=2, max_digits=12, blank=True, null=True)
-
-    # 2022.10.17 售后单表头冗余订单商品总数量 & 退货数量类型
-    order_total_quantity = models.IntegerField('商品总数量', null=True, blank=True, default=0)
-    return_quantity_type = models.CharField("退货数量类型", max_length=24, choices=ReturnQuantityType.RETURN_QUANTITY_TYPE_CHOICES, blank=True, null=True, default=ReturnQuantityType.NONE)
-
     class Meta:
         app_label = APP_LABEL
         verbose_name = "Order After Sale"
         verbose_name_plural = "Order After Sale"
 
     @cached_property
     def coupons_to_charge(self):
@@ -550,15 +533,15 @@
             for afs_line in afs_lines:
                 distribute_status = afs_line.distribute_status
                 if_returned = afs_line.if_returned
                 # if if_returned:
                 #     continue
                 customer_express_code = afs_line.customer_express_code
                 afs_line_customer_express_name = afs_line.customer_express_name or ""
-                customer_express_name = ShippingPartnerCodes.CODE_2_NAME_MAP.get(customer_express_code, afs_line_customer_express_name)
+                customer_express_name = ShippingPartnerCodes_DICT.get(customer_express_code, afs_line_customer_express_name)
                 customer_shipping_number = afs_line.customer_shipping_number
 
                 if distribute_status in [DistributeStatus.PACKAGED,
                                         DistributeStatus.CUS_CONFIRM,
                                         DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                                         DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
                                         DistributeStatus.OUTSTORAGE_PACKAGED]:
@@ -692,34 +675,14 @@
     # 退货重算-售后版本号
     afs_version = models.CharField("售后版本号", max_length=12, blank=True, null=True, db_index=True, default=AfsVersionConst.V2)
     # 售后数据来源
     generate_from = models.CharField(
         "数据来源", max_length=12, blank=True, null=True, 
         db_index=True, choices=AfsLineGenerateFrom.CHOICES, default=AfsLineGenerateFrom.SELECT)
 
-    # refund_amount 退款总金额, 包含各种支付别
-    refund_amount = models.DecimalField("refund_amount", decimal_places=2, max_digits=12, blank=True, null=True)
-
-    # 2022.08 订单冗余sell_type
-    sell_type = models.CharField("sell_type", max_length=32, blank=True, null=True, db_index=True)
-
-    # 2022.09 冗余确收人
-    afs_sub_num_shop = models.CharField("退款单小票票号", max_length=64, blank=True, null=True)
-
-    # 2022.11 发货仓需求
-    retstorage_id = models.CharField("退货仓ID", max_length=40, blank=True, null=True, db_index=True)
-    # 2022.10 新增售后单行状态
-    afsline_status = models.CharField("afsline_status", max_length=32, choices=AfsLineStatus.CHOICES, blank=True, null=True)
-    # 客服还货时, 导购收货人信息
-    guide_receiver = models.CharField("导购收货人", max_length=40, blank=True, null=True, db_index=True)
-    guide_receiver_username = models.CharField("导购收货人手机号", max_length=20, blank=True, null=True, db_index=True)
-    guide_receiver_displayname = models.CharField("导购收货人姓名", max_length=40, blank=True, null=True)
-    # guide_receiver_time (导购收货时间)
-    guide_receiver_time = models.DateTimeField("导购收货时间", blank=True, null=True)
-
     class Meta:
         # 同一个售后单里不应该创建两个相同发货单行的售后
         # unique_together = ('aftersale_id', 'line_id', 'distribute_line_id')
         app_label = APP_LABEL
 
     @cached_property
     def line(self):
@@ -1447,91 +1410,7 @@
     # 由退货重算生成的原始积分
     calc_points = models.PositiveIntegerField("calc_points")
     # 由客服编辑后的积分
     edit_points = models.PositiveIntegerField("edit_points")
 
     class Meta:
         app_label = 'sparrow_aftersale'
-
-
-# 打印退款单小票的二维码
-# 一个二维码 属于同一个售后单
-# 如果同时勾选了多个专柜的商品，会打印多张小票
-class QueryResult(BaseModelTimeAndDeleted):
-    # id(主键uuid)
-    id = models.CharField(max_length=100, primary_key=True, default=get_uuid4_hex, editable=False)
-    # user_id 操作员ID
-    query_user_id = models.CharField('User ID', max_length=40, db_index=True, null=True)
-    # username 操作员手机号
-    query_username = models.CharField('操作员手机号', max_length=15, help_text=u'操作员手机号', blank=True, null=True)
-    # displayname 操作员姓名
-    query_displayname = models.CharField("操作员姓名", max_length=10, blank=True, null=True)
-    # 售后单ID
-    aftersale_id = models.IntegerField("售后单ID", blank=True, null=True, db_index=True)
-    # 售后小票单号
-    afs_sub_num = models.CharField("售后小票单号", max_length=64, blank=True, null=True, db_index=True)
-
-    class Meta:
-        app_label = 'sparrow_aftersale'
-        ordering = ['-created_time']
-
-
-# 退款单小票，所属某个专柜
-class QueryResultTicket(BaseModelTimeAndDeleted):
-    # user_id 操作员ID
-    query_user_id = models.CharField('User ID', max_length=40, db_index=True, null=True)
-    # username 操作员手机号
-    query_username = models.CharField('操作员手机号', max_length=15, help_text=u'操作员手机号', blank=True, null=True)
-    # displayname 操作员姓名
-    query_displayname = models.CharField("操作员姓名", max_length=10, blank=True, null=True)
-    # 二维码ID
-    query_result_id = models.CharField(max_length=40, blank=True, null=True, db_index=True)
-    # 售后单ID
-    aftersale_id = models.IntegerField("售后单ID", blank=True, null=True, db_index=True)
-    # 售后小票单号
-    afs_sub_num_shop = models.CharField("售后小票单号", max_length=64, blank=True, null=True, unique=True, db_index=True)
-    # shop_id(专柜id)
-    shop_id = models.PositiveIntegerField('Shop ID', blank=True, null=True)
-    # shop_num(专柜号)
-    shop_num = models.CharField("Shop number", max_length=128, blank=True)
-    # 专柜名
-    shop_name = models.CharField("Shop Name", max_length=128, blank=True, null=True)
-    # 小票包含的商品数量
-    quantity = models.IntegerField("退货数量", default=1)
-
-    class Meta:
-        app_label = 'sparrow_aftersale'
-        ordering = ['-created_time']
-
-
-# 退款单小票line
-class QueryResultDetail(BaseModelTimeAndDeleted):
-    # id(主键uuid)
-    id = models.CharField(max_length=40, primary_key=True, default=get_uuid4_hex, editable=False)
-    query_result_id = models.CharField(max_length=40, blank=True, null=True, db_index=True)
-    aftersale_id = models.IntegerField("售后单ID", blank=True, null=True, db_index=True)
-    afsline_id = models.IntegerField("售后单表体ID", blank=True, null=True, db_index=True)
-
-    # 以下字段是上线后做优化新增
-    # 退款单小票票号, 每个专柜一张
-    afs_sub_num_shop = models.CharField("退款单小票票号", max_length=64, null=True)
-
-    # shop_id(专柜id)
-    shop_id = models.PositiveIntegerField('Shop ID', blank=True, null=True)
-    # shop_num(专柜号)
-    shop_num = models.CharField("Shop number", max_length=128, blank=True)
-    # 专柜名
-    shop_name = models.CharField("Shop Name", max_length=128, blank=True, null=True)
-    # title(商品名称)
-    title = models.CharField("Product title", max_length=255, blank=True, null=True)
-    shop_sku = models.CharField("Shop SKU", max_length=128, blank=True, null=True)
-    brand_name = models.CharField("Brand Name", max_length=128, blank=True, null=True)
-    sku_attr = models.CharField("Product SKU Attr", max_length=255, blank=True, null=True)
-    # 商品汉光码
-    hg_code = models.CharField("Product HG Code", max_length=255, blank=True, null=True)
-
-    # 退商品数量
-    quantity = models.IntegerField('退货数量', default=1)
-
-    class Meta:
-        app_label = 'sparrow_aftersale'
-        ordering = ['-created_time']
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,86 +2,38 @@
     常量
 """
 from ..core.datastructures import ImmutableList
 from ..core.datastructures import ImmutableDict
 from ..sparrow_distribute.constants import DistributeStatus
 
 
-class StorageRecordBusiType:
-    ''' 入库时, 单据类型 '''
-    REFUND = 'refund'  # 退款单小票
-    EXCHANGE = 'exchange'  # 换货单小票
-    DISTRIBUTE = 'distribute'  # 发货单小票
-
-    CHOICES = ImmutableDict(
-        {
-            REFUND: "退款单小票",
-            EXCHANGE: "换货单小票",
-            DISTRIBUTE: "发货单小票"
-        }
-    )
-
-
 class StoreNumberInfo(object):
     """ 仓库信息及对应发货单状态 """
     SERVICE_STORE_NUMBER = "B3"
     SERVICE_STORE_NAME = "B3仓库"
     SERVICE_DESK_NUMBER = "ZT"
     SERVICE_DESK_NAME = "自提点"
-    SERVICE_STOP_NUMBER = "STOP"
-    SERVICE_STOP_NAME = "滞留仓"
-    AFTERSALE_WH_NUMBER = "AFS"
-    AFTERSALE_WH_CODE = "AFS"
-    AFTERSALE_WH_NAME = "退换货仓"
 
     DISTRIBUTE_STATUS_STORE_INFO_MAP = {
         DistributeStatus.SERVICE_DESK: {
             'name': SERVICE_DESK_NAME,
             'number': SERVICE_DESK_NUMBER,
             'code': DistributeStatus.SERVICE_DESK
         },
         DistributeStatus.SERVICE_STORE: {
             'name': SERVICE_STORE_NAME,
             'number': SERVICE_STORE_NUMBER,
             'code': DistributeStatus.SERVICE_STORE
-        },
-        DistributeStatus.SERVICE_STOP: {
-            'name': SERVICE_STOP_NAME,
-            'number': SERVICE_STOP_NUMBER,
-            'code': DistributeStatus.SERVICE_STOP
-        }
-    }
-
-    STORE_INFO_MAP = {
-        SERVICE_STORE_NUMBER: {
-            'name': SERVICE_STORE_NAME,
-            'number': SERVICE_STORE_NUMBER,
-            'code': DistributeStatus.SERVICE_STORE
-        },
-        SERVICE_DESK_NUMBER: {
-            'name': SERVICE_DESK_NAME,
-            'number': SERVICE_DESK_NUMBER,
-            'code': DistributeStatus.SERVICE_DESK
-        },
-        SERVICE_STOP_NUMBER: {
-            'name': SERVICE_STOP_NAME,
-            'number': SERVICE_STOP_NUMBER,
-            'code': DistributeStatus.SERVICE_STOP
-        },
-        AFTERSALE_WH_NUMBER: {
-            'name': AFTERSALE_WH_NAME,
-            'number': AFTERSALE_WH_NUMBER,
-            'code': AFTERSALE_WH_CODE,
         }
     }
 
-    STORE_NUMBER_TO_NAME_MAP = {d['number']: d['name'] for d in STORE_INFO_MAP.values()}
-    STORE_NUMBER_TO_CODE_MAP = {d['number']: d['code'] for d in STORE_INFO_MAP.values()}
-    STORE_CODE_TO_NAME_MAP = {d['code']: d['name'] for d in STORE_INFO_MAP.values()}
-    STORE_CODE_TO_NUMBER_MAP = {d['code']: d['number'] for d in STORE_INFO_MAP.values()}
+    STORE_NUMBER_TO_NAME_MAP = {d['number']: d['name'] for d in DISTRIBUTE_STATUS_STORE_INFO_MAP.values()}
+    STORE_NUMBER_TO_CODE_MAP = {d['number']: d['code'] for d in DISTRIBUTE_STATUS_STORE_INFO_MAP.values()}
+    STORE_CODE_TO_NAME_MAP = {d['code']: d['name'] for d in DISTRIBUTE_STATUS_STORE_INFO_MAP.values()}
+    STORE_CODE_TO_NUMBER_MAP = {d['code']: d['number'] for d in DISTRIBUTE_STATUS_STORE_INFO_MAP.values()}
 
 
 class InventoryDetailResult(object):
     """
         发货单盘点结果
     """
     # 盘盈
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_disstorage/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_disstorage/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-from django.db.models import CharField, DateTimeField, BooleanField, PositiveIntegerField, Count, IntegerField
+from django.db.models import CharField, DateTimeField, BooleanField, PositiveIntegerField, Count
 
 from ..core.common_utils import get_uuid4_hex
 from ..core.base_models import BaseModelTimeAndDeleted
-from .constants import StorageRecordBusiType
 from .constants import InventoryDetailResult
 from .constants import InventoryHelpStatus
 from .constants import InventoryMainStatus
 from . import APP_LABEL
 
 
-__all__ = [
-    'InventoryMain',
-    'InventoryDetail',
-    'InventoryHelp',
-    'InventoryNote',
-    'Shelf',
-    'Seat',
-    'StorageRecord',
-]
-
-
 class InventoryMain(BaseModelTimeAndDeleted):
     """
         库存盘点主表
     """
     id = CharField("id", primary_key=True, default=get_uuid4_hex, blank=True, max_length=128)
     number = CharField("盘点序列号", max_length=128, db_index=True, unique=True)
-    distribute_status = CharField("盘点位置", max_length=128, blank=True, null=True)
-    distribute_status_name = CharField("盘点位置名称", max_length=128, blank=True, null=True)
+    distribute_status = CharField("盘点位置", max_length=128, blank=True)
+    distribute_status_name = CharField("盘点位置名称", max_length=128, blank=True)
     inventory_user_id = CharField("盘点人 id", max_length=128, blank=True)
     inventory_username = CharField("盘点人姓名", max_length=128, blank=True)
     inventory_user_displayname = CharField("盘点人昵称", max_length=128, blank=True)
     initial_num = PositiveIntegerField("期初数", blank=True)  # 盘点开始时, 由系统判断在库房内的发货单数量
     actual_num = PositiveIntegerField("实核数", default=0, blank=True)  # 盘平的发货单数量
     profit_num = PositiveIntegerField("盘盈发货单数量", default=0, blank=True, null=True)
     loss_num = PositiveIntegerField("盘亏发货单数量", default=0, blank=True, null=True)
@@ -39,18 +27,14 @@
     loss_dealed_num = PositiveIntegerField("已核销的盘亏发货单数量", default=0, blank=True, null=True)
     if_balance = BooleanField("是否持平", default=False, blank=True, null=True)
     inventory_start_time = DateTimeField("盘点开始时间", blank=True, auto_now_add=True)
     inventory_end_time = DateTimeField("盘点结束时间", blank=True, null=True)
     if_help = BooleanField("是否是多人盘点", null=True, default=0, db_index=True)
     status = CharField("盘点状态", max_length=16, default=InventoryMainStatus.INIT, db_index=True)
 
-    store_code = CharField("货架位置编码", max_length=128, null=True, db_index=True)
-    store_number = CharField("货架位置", max_length=128, null=True)
-    store_name = CharField("货架位置名称", max_length=128, null=True)
-
     @property
     def helps(self):
         return InventoryHelp.objects.filter(main_id=self.id).order_by('-help_start_time', 'shelf_number')
 
     @property
     def details(self):
         ''' 所有盘点列表 '''
@@ -64,17 +48,17 @@
 class InventoryDetail(BaseModelTimeAndDeleted):
     """
         盘点明细表
     """
     id = CharField("id", primary_key=True, default=get_uuid4_hex, blank=True, max_length=128)
     main_id = CharField("盘点主表 id", db_index=True, blank=True, max_length=128)
     main_number = CharField("盘点序列号", max_length=128, blank=True)
-    distribute_id = CharField("发货单 id", max_length=100, blank=True, db_index=True, null=True)
-    distribute_number = CharField("发货单号", max_length=100, blank=True, null=True)
-    distribute_name = CharField("发货单名称", max_length=100, blank=True, null=True)
+    distribute_id = CharField("发货单 id", max_length=100, blank=True, db_index=True)
+    distribute_number = CharField("发货单号", max_length=100, blank=True)
+    distribute_name = CharField("发货单名称", max_length=100, blank=True)
     order_id = PositiveIntegerField("订单 id", blank=True, db_index=True)
     order_number = CharField("订单号", max_length=128, blank=True)
     shop_id = PositiveIntegerField("专柜 id", blank=True)
     shop_num = CharField("专柜号", max_length=128, blank=True)
     shop_name = CharField("专柜名称", max_length=128, blank=True)
     aftersale_status = BooleanField("是否售后", blank=True)
     store_in_time = DateTimeField("入库时间", blank=True, null=True)
@@ -93,35 +77,22 @@
     shelf_id = CharField("shelf_id", max_length=32, null=True)
     shelf_number = CharField("shelf_number", max_length=32, null=True)
     seat_id = CharField("seat_id", max_length=32, null=True)
     seat_number = CharField("seat_number", max_length=32, null=True)
     checked_user_id = CharField("实际盘点人", max_length=64, null=True)
     checked_shelf_number = CharField("实际盘点位置", max_length=64, null=True)
 
-    # shipping_method(发货方式：自提、快递、闪送)
-    shipping_method = CharField('发货方式', max_length=24, blank=True, null=True)
-
-    busi_id = CharField("业务单ID", max_length=40, db_index=True, null=True)
-    busi_number = CharField("业务单number", max_length=64, db_index=True, null=True)
-    # busi_name 目前只有发货单有 distribute_name
-    busi_name = CharField("业务单Name", max_length=64, null=True)
-    busi_type = CharField("业务单类型", max_length=16, db_index=True, null=True)
-
     @property
     def notes(self):
         return InventoryNote.objects.filter(detail_id=self.id).order_by('-created_time')
 
     @property
     def checked_result_show(self):
         return InventoryDetailResult.CHECKED_RESULT_MAP.get(self.checked_result)
 
-    @property
-    def busi_type_name(self):
-        return StorageRecordBusiType.CHOICES.get(self.busi_type)
-
     class Meta:
         verbose_name = '盘点明细表'
         app_label = APP_LABEL
 
 
 class InventoryHelp(BaseModelTimeAndDeleted):
     id = CharField("id", primary_key=True, default=get_uuid4_hex, blank=True, max_length=32)
@@ -152,34 +123,24 @@
         盘点结果备注表, 存储对盘盈/盘亏发货单的核销意见
     """
     id = CharField("id", primary_key=True, default=get_uuid4_hex, blank=True, max_length=128)
     detail_id = CharField("盘点明细表 id", db_index=True, max_length=128)
 
     main_id = CharField("盘点主表 id", db_index=True, blank=True, max_length=128)
     main_number = CharField("盘点序列号", max_length=128, blank=True)
-    distribute_id = CharField("发货单 id", max_length=100, blank=True, db_index=True, null=True)
-    distribute_number = CharField("发货单号", max_length=100, blank=True, null=True)
-    distribute_name = CharField("发货单名称", max_length=100, blank=True, null=True)
+    distribute_id = CharField("发货单 id", max_length=100, blank=True, db_index=True)
+    distribute_number = CharField("发货单号", max_length=100, blank=True)
+    distribute_name = CharField("发货单名称", max_length=100, blank=True)
 
     note_user_id = CharField("备注人 id", max_length=128, blank=True)
     note_username = CharField("备注人姓名", max_length=128, blank=True)
     note_user_displayname = CharField("备注人昵称", max_length=128, blank=True)
     note_time = DateTimeField("处理时间")
     message = CharField("处理意见", max_length=512, blank=True)
 
-    busi_id = CharField("业务单ID", max_length=40, db_index=True, null=True)
-    busi_number = CharField("业务单number", max_length=64, db_index=True, null=True)
-    # busi_name 目前只有发货单有 distribute_name
-    busi_name = CharField("业务单Name", max_length=64, null=True)
-    busi_type = CharField("业务单类型", max_length=16, db_index=True, null=True)
-
-    @property
-    def busi_type_name(self):
-        return StorageRecordBusiType.CHOICES.get(self.busi_type)
-
     class Meta:
         verbose_name = '盘点备注表'
         app_label = APP_LABEL
 
 
 class Shelf(BaseModelTimeAndDeleted):
     """
@@ -227,15 +188,15 @@
                     ... ...
                 ],
             },
             ... ...
         ]
         '''
         storage_record_count_distribute_number_by_seat = StorageRecord.objects.filter(shelf_id=self.id, if_out=False).\
-            values('seat_number').annotate(count=Count('busi_number', distinct=True)).values('count', 'seat_number').all()
+            values('seat_number').annotate(count=Count('distribute_number', distinct=True)).values('count', 'seat_number').all()
         count_dict = {row['seat_number']: row['count'] or 0 for row in storage_record_count_distribute_number_by_seat}
 
         seat_objs = Seat.objects.filter(shelf_id=self.id).all()
 
         seats = {}
 
         for seat in seat_objs:
@@ -280,16 +241,16 @@
 
 class StorageRecord(BaseModelTimeAndDeleted):
     """
     库存表
     """
     id = CharField("库存 id", primary_key=True, default=get_uuid4_hex, max_length=128, blank=True)
 
-    distribute_id = CharField("发货单id", max_length=128, db_index=True, null=True)
-    distribute_number = CharField("发货单号", max_length=128, db_index=True, null=True)
+    distribute_id = CharField("发货单id", max_length=128, db_index=True)
+    distribute_number = CharField("发货单号", max_length=128, db_index=True)
 
     order_id = CharField("订单 id ", max_length=128, db_index=True)
     order_number = CharField("订单号", max_length=128, db_index=True)
     shop_id = CharField("专柜id", max_length=128)
     shop_num = CharField("专柜号", max_length=128)
     shop_name = CharField("专柜名称", max_length=128, db_index=True)
 
@@ -309,18 +270,9 @@
     store_out_time = DateTimeField("出库时间", db_index=True, null=True)
     store_out_event = CharField("出库原因", max_length=128, null=True)
     store_out_user_id = CharField("出库人 id ", max_length=128, null=True)
     store_out_user_name = CharField("出库人姓名", max_length=128, null=True)
     store_out_user_displayname = CharField("出库人昵称", max_length=128, null=True)
     if_out = BooleanField("是否已提走", default=False, db_index=False, blank=False)
 
-    busi_id = CharField("业务单ID", max_length=40, db_index=True, null=True)
-    busi_number = CharField("业务单number", max_length=64, db_index=True, null=True)
-    busi_type = CharField("业务单类型", max_length=16, db_index=True, null=True)
-    quantity = IntegerField("包含商品数量", default=1)
-
-    @property
-    def busi_type_name(self):
-        return StorageRecordBusiType.CHOICES.get(self.busi_type)
-
     class Meta:
         app_label = APP_LABEL
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-import logging
-
 from ..core.constants import MemberLevel
 from enum import Enum, unique
 
-logger = logging.getLogger(__name__)
-
-
 DISTRIBUTE_ERROR_CODE_PREFIX = 246000
 BASE_DISTRIBUTE_API_CODE = 20103000
 
 
 class DistributeStatusOwner(object):
     GUIDE = 'guide'
     CUSSERVICE = 'cusservice'
@@ -97,22 +92,14 @@
 
     # 2022.08 虚拟商品
     # 虚拟商品INIT
     VIRTUAL_INIT = "virtual_init"
     # 虚拟已确收
     CUS_CONFIRM_AT_VIRTUAL = "cus_confirm_at_virtual"
 
-    # 2022.09 特需售后单自提转快递支付运费订单的发货单
-    MAKEUP_POSTAGE_PAID = "paid"
-    
-    # 2023.4 退款单与发货单联动
-    # 退款单 售后仓已收 <> 售后仓已收
-    # event 售后仓入库
-    AFTERSALE_WH = "AftersaleWH"
-
     NO_SPLIT_STATUS_LIST = [
         INIT,
         HGVENDING_INIT,
         VIRTUAL_INIT,
         PRINTED,
         CUSSERVICE_PICKED_UP,
         GUIDE_PICKED_UP,
@@ -135,15 +122,14 @@
         TAILPAY_OVERTIME,
         DEPOSITPAY_RETURN,
         HAITAO_INIT,
         HAITAO_BAISHI,
         HAITAO_PACKAGED,
         HAITAO_RETURN,
         SERVICE_STOP,
-        MAKEUP_POSTAGE_PAID,
     ]
     
 
     # 可以被售后集合
     CAN_AFTERSALE_STATUS_LIST = [
         INIT,
         PRINTED,
@@ -155,15 +141,14 @@
         CUS_CONFIRM_AT_VIRTUAL,
         PACKAGED,
         SERVICE_DESK,
         SERVICE_STORE,
         OUTSTORAGE_WAIT_PACKAGE,
         OUTSTORAGE_PACKAGED,
         SERVICE_STOP,
-        MAKEUP_POSTAGE_PAID,
     ]
 
     ## 初始态集合
     INIT_STATUS_LIST = [
         INIT,
         HGVENDING_INIT,
         VIRTUAL_INIT,
@@ -173,17 +158,15 @@
     ## 可以整单退的发货单状态集合
     ENTIRE_AFTERSALE_STATUS_LIST = [
         INIT,
         HGVENDING_INIT,
         PRINTED,
         GUIDE_PICKED_UP,
         SPLIT,
-        HGVENDING_WAIT_PICKUP,
-        # 补缴运费的商品可以整单退
-        MAKEUP_POSTAGE_PAID,
+        HGVENDING_WAIT_PICKUP
     ]
 
     BEFORE_cuservice_pick_up = [
         INIT,
         PRINTED,
         NO_PICKUP_RETURN,
         SPLIT,
@@ -228,16 +211,14 @@
         DEPOSITPAY_RETURN: "定金已退",
         TAILPAY_OVERTIME: "尾款超时",
         HAITAO_INIT: "备货中",
         HAITAO_BAISHI: "备货中",
         HAITAO_PACKAGED: "已发货",
         HAITAO_RETURN: "售后",
         SERVICE_STOP: "待发货",
-        MAKEUP_POSTAGE_PAID: "运费已支付",
-        AFTERSALE_WH: "售后仓已收",
     }
     # For B端 查询
     DISTRIBUTE_STATUS_CHOICES_FOR_B_QUERY = {
         INIT: '未打印',
         HGVENDING_INIT: '贩售机初始态',
         PRINTED: "已打印",
         CUSSERVICE_PICKED_UP: "客服已提",
@@ -261,17 +242,15 @@
         DEPOSITPAY: "定金已付",
         DEPOSITPAY_RETURN: "定金已退",
         TAILPAY_OVERTIME: "尾款超时",
         HAITAO_INIT: "海淘备货中",
         HAITAO_BAISHI: "海淘已推百世",
         HAITAO_PACKAGED: "海淘已发货",
         HAITAO_RETURN: "海淘已退",
-        SERVICE_STOP: "滞留仓已收",
-        MAKEUP_POSTAGE_PAID: "运费已支付",
-        AFTERSALE_WH: "售后仓已收",
+        SERVICE_STOP: "滞留仓已收"
     }
 
     DISTRIBUTE_MESSAGE_DICT_FOR_C = {
         INIT: "专柜已收到您的订单，正在为您备货。",
         SERVICE_STORE: "商品已从专柜提货，正在为您准备邮寄。",
         SERVICE_DESK: "商品已备好，您可至【汉光百货顾客服务中心（一层北客梯旁）】领取。",
         CUSSERVICE_PICKED_UP: "商品已经出库。",
@@ -291,15 +270,14 @@
         DEPOSITPAY_RETURN: "您的商品已退还定金",
         TAILPAY_OVERTIME: "未按时支付尾款，您的订单已关闭",
         HAITAO_INIT: "海淘备货中。",
         HAITAO_BAISHI: "海淘备货中。",
         HAITAO_PACKAGED: "海淘已发货。",
         HAITAO_RETURN: "海淘已售后。",
         SERVICE_STOP: "暂时无法发货，商品滞留。",
-        MAKEUP_POSTAGE_PAID: "订单自提转快递运费已支付。",
     }
 
     DISTRIBUTE_STATUS_CHOICES = (
         (INIT, '未打印'),
         (HGVENDING_INIT, '贩售机初始态'),
         (PRINTED, "已打印"),
         (CUSSERVICE_PICKED_UP, "客服已提"),
@@ -325,16 +303,14 @@
         (HAITAO_INIT, "海淘备货中"),
         (HAITAO_BAISHI, "海淘已推百世"),
         (HAITAO_PACKAGED, "海淘已发货"),
         (HAITAO_RETURN, "海淘已退"),
         (SERVICE_STOP, "滞留仓已收"),
         (VIRTUAL_INIT, "虚拟商品初始态"),
         (CUS_CONFIRM_AT_VIRTUAL, "虚拟商品已提货"),
-        (MAKEUP_POSTAGE_PAID, "运费已支付"),
-        (AFTERSALE_WH, "售后仓已收"),
     )
 
     DISTRIBUTE_STATUS_OWNER_DICT = {
         INIT: DistributeStatusOwner.GUIDE,
         VIRTUAL_INIT: DistributeStatusOwner.CUSTOMER,
         HGVENDING_INIT: DistributeStatusOwner.HGVENDING,
         PRINTED: DistributeStatusOwner.GUIDE,
@@ -359,15 +335,14 @@
         DEPOSITPAY_RETURN: DistributeStatusOwner.GUIDE,
         TAILPAY_OVERTIME: DistributeStatusOwner.GUIDE,
         HAITAO_INIT: DistributeStatusOwner.HAITAO,
         HAITAO_BAISHI: DistributeStatusOwner.HAITAO,
         HAITAO_PACKAGED: DistributeStatusOwner.HAITAO,
         HAITAO_RETURN: DistributeStatusOwner.HAITAO,
         SERVICE_STOP: DistributeStatusOwner.CUSSERVICE,
-        MAKEUP_POSTAGE_PAID: DistributeStatusOwner.CUSTOMER,
     }
 
     DISTRIBUTE_STATUS_DIRECTION_DICT = {
         INIT: DistributeDirection.GUIDE,
         HGVENDING_INIT: DistributeDirection.HGVENDING,
         PRINTED: DistributeDirection.GUIDE,
         GUIDE_PICKED_UP: DistributeDirection.GUIDE,
@@ -391,16 +366,14 @@
         TAILPAY_OVERTIME: DistributeDirection.GUIDE,
 
         HAITAO_INIT: DistributeDirection.HAITAO,
         HAITAO_BAISHI: DistributeDirection.HAITAO,
         HAITAO_PACKAGED: DistributeDirection.HAITAO,
         HAITAO_RETURN: DistributeDirection.HAITAO,
         SERVICE_STOP: DistributeDirection.CUSSERVICE,
-
-        MAKEUP_POSTAGE_PAID: DistributeDirection.CUSSERVICE,
     }
 
     # 终结状态列表
     TERMINATE_STATUS_LIST = [
         PACKAGED,
         CUSSERVICE_HOLD,
         CUS_CONFIRM,
@@ -415,16 +388,15 @@
         OUTSTORAGE_PACKAGED,
         OUTSTORAGE_RETURN,
         # 分阶段支付
         DEPOSITPAY_RETURN,
         TAILPAY_OVERTIME,
         # 海淘
         HAITAO_PACKAGED,
-        HAITAO_RETURN,
-        MAKEUP_POSTAGE_PAID,
+        HAITAO_RETURN
     ]
 
     # 非最终状态
     UN_TERMINATE_STATUS_LIST = [
         SERVICE_DESK,
         SERVICE_STORE,
         PRINTED,
@@ -447,74 +419,25 @@
 
     # 可换货发货单状态
     EXCHANGE_TERMINATE_STATUS_LIST = [
         PACKAGED,
         CUS_CONFIRM,
         CUS_CONFIRM_AT_GUIDE,
         CUS_CONFIRM_AT_CUSSERVICE,
-        OUTSTORAGE_PACKAGED,
-    ]
-
-    # 未售后的不支持修改配送方式的发货单状态
-    CAN_NOT_MODY_SHIPPING_METHOD_DISTRIBUTE_STATUS_LIST = [
-        CUS_CONFIRM_AT_GUIDE,
-        CUS_CONFIRM_AT_CUSSERVICE,
-        PACKAGED,
-        OUTSTORAGE_PACKAGED,
-        OUTSTORAGE_WAIT_PACKAGE,
-        SPLIT,
-    ]
-
-    # 未出汉光的发货单状态
-    DISTRIBUTE_STATUS_IN_HG_LIST = [
-        INIT,
-        PRINTED,
-        CUSSERVICE_PICKED_UP,
-        SERVICE_DESK,
-        SERVICE_STORE,
-        SPLIT,
-        OUTSTORAGE_WAIT_PACKAGE,
-        HGVENDING_INIT,
-        HGVENDING_WAIT_PICKUP,
-        TAILPAY_OVERTIME,
-        HAITAO_INIT,
-        HAITAO_BAISHI,
-        SERVICE_STOP,
-    ]
-
-    # 未出专柜
-    DISTRIBUTE_STATUS_IN_SHOP_LIST = [
-        INIT,
-        PRINTED,
-        OUTSTORAGE_WAIT_PACKAGE,
     ]
 
 
-class __ShippingMethod(object):
+class ShippingMethod(object):
     # 普通快递
     EXPRESS = 'express'
     # 自提
     SELF_SERVICE = 'self_service'
     # 闪送
     FLASH_DELIVERY = 'flash_delivery'
 
-    CHOICES = (
-        (EXPRESS, "快递发货"),
-        (SELF_SERVICE, "到店自提"),
-        (FLASH_DELIVERY, "闪送"),
-    )
-
-    def __getattribute__(self, name: str):
-        value = super().__getattribute__(name)
-        logger.warning("sparrow_distribute.constants.ShippingMethod 已废弃, 请使用 sparrow_order_lib.core.constants.ShippingMethod 替换")
-        return value
-
-
-ShippingMethod = __ShippingMethod()
-
 
 class DistributeEventConstKey(object):
     FROM_STATUS_LIST_KEY = "from_status_list"
     TO_STATUS_KEY = "to_status"
     TO_STATE_MAP_KEY = "to_state_map"
 
 
@@ -615,132 +538,91 @@
     # 合单催配送提醒
     PUSH_GUIDE_ASSIGN = "push_guide_assign"
 
     # 2022.08 特殊售后单需求
     AFSPLUS_OPEN = "afsplus_open"
     AFSPLUS_CLOSE = "afsplus_close"
     AFSPLUS_COMPLETE = "afsplus_complete"
-    AFSPLUS_S2E = "afsplus_s2e"  # 自提转快递
-    AFSPLUS_E2S = "afsplus_e2s"  # 快递转自提
-    AFSPLUS_TO_EXPRESS = "afsplus_2e"  # 转快递
-    AFSPLUS_TO_SELF_SERVICE = "afsplus_2s"
 
     # 2022.08 虚拟商品确收
     CUS_CONFIRM_AT_VIRTUAL = "cus_confirm_at_virtual"
-    
-    CLOUDPRINT_SHIPPING_NUMBER = "cloudprint_shipping_number"
-    
-    # 2023.4 售后仓入库
-    ENTER_AFTERSALE_WH = 'enter_aftersale_wh'
-    # 2023.4 手动拆单
-    MANUAL_SPLIT = "manual_split"
 
     FROM_TO_MAP = {
         PRINT: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.GUIDE_PICKED_UP,
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.SERVICE_STORE,
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.PACKAGED,
-                DistributeStatus.CUSSERVICE_HOLD,
+            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.INIT, DistributeStatus.PRINTED,
+                DistributeStatus.GUIDE_PICKED_UP, DistributeStatus.CUSSERVICE_PICKED_UP,
+                DistributeStatus.SERVICE_STORE, DistributeStatus.SERVICE_DESK,
+                DistributeStatus.PACKAGED, DistributeStatus.CUSSERVICE_HOLD,
                 DistributeStatus.CUS_CONFIRM,
                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
-                DistributeStatus.OUTSTORAGE_PACKAGED,
-                DistributeStatus.OUTSTORAGE_WAIT_PACKAGE,
+                DistributeStatus.OUTSTORAGE_PACKAGED, DistributeStatus.OUTSTORAGE_WAIT_PACKAGE,
                 DistributeStatus.SERVICE_STOP,
-            ],
+                ],
             DistributeEventConstKey.TO_STATE_MAP_KEY: {
-                DistributeStatus.INIT: DistributeStatus.PRINTED,
-            },
+                    DistributeStatus.INIT: DistributeStatus.PRINTED,
+                    },
         },
         GUIDE_PRINT: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.GUIDE_PICKED_UP
-            ],
+            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.INIT, DistributeStatus.PRINTED,
+                DistributeStatus.GUIDE_PICKED_UP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.SPLIT
         },
         PRINT_AND_OVERWRITE_EXPRESS: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.GUIDE_PICKED_UP,
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.SERVICE_STORE,
-                DistributeStatus.SERVICE_DESK,
+            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.INIT, DistributeStatus.PRINTED,
+                DistributeStatus.GUIDE_PICKED_UP, DistributeStatus.CUSSERVICE_PICKED_UP,
+                DistributeStatus.SERVICE_STORE, DistributeStatus.SERVICE_DESK,
                 DistributeStatus.CUSSERVICE_HOLD,
                 DistributeStatus.CUS_CONFIRM,
                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
                 DistributeStatus.SERVICE_STOP,
                 DistributeStatus.PACKAGED,
                 ],
             DistributeEventConstKey.TO_STATE_MAP_KEY: {
-                DistributeStatus.INIT: DistributeStatus.PRINTED,
-                },
+                    DistributeStatus.INIT: DistributeStatus.PRINTED,
+                    },
         },
         CANCEL_PRINT: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.PRINTED],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.INIT,
         },
         CUSSERVICE_PICK_UP: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.SERVICE_STORE,
-                DistributeStatus.SERVICE_STOP,
-                DistributeStatus.AFTERSALE_WH,
-                ],
+            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.INIT, DistributeStatus.PRINTED,
+                                DistributeStatus.SERVICE_DESK, DistributeStatus.SERVICE_STORE,
+                                DistributeStatus.SERVICE_STOP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.CUSSERVICE_PICKED_UP,
         },
         GUIDE_PICK_UP: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.INIT, DistributeStatus.PRINTED],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.GUIDE_PICKED_UP,
         },
         HGVENDING_PICKED_UP: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [DistributeStatus.HGVENDING_INIT],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.HGVENDING_WAIT_PICKUP,
         },
         SERVICESTORE_PICK_UP: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT, 
-                DistributeStatus.PRINTED,
-                DistributeStatus.CUSSERVICE_PICKED_UP, 
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.SERVICE_STOP,
-                DistributeStatus.AFTERSALE_WH,
-                ],
+                DistributeStatus.INIT, DistributeStatus.PRINTED,
+                DistributeStatus.CUSSERVICE_PICKED_UP, DistributeStatus.SERVICE_DESK],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.SERVICE_STORE,
         },
         SERVICEDESK_PICK_UP: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.SERVICE_STORE,
-                DistributeStatus.GUIDE_PICKED_UP,
-                DistributeStatus.AFTERSALE_WH,
-                ],
+                DistributeStatus.INIT, DistributeStatus.PRINTED,
+                DistributeStatus.CUSSERVICE_PICKED_UP, DistributeStatus.SERVICE_STORE, DistributeStatus.GUIDE_PICKED_UP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.SERVICE_DESK,
         },
         PACKAGE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                    DistributeStatus.INIT,
-                    DistributeStatus.PRINTED,
+                    DistributeStatus.INIT, DistributeStatus.PRINTED,
                     DistributeStatus.CUSSERVICE_PICKED_UP,
                     DistributeStatus.SERVICE_DESK,
                     DistributeStatus.SERVICE_STORE,
-                    DistributeStatus.SERVICE_STOP,
-                    ],
+                    DistributeStatus.SERVICE_STOP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.PACKAGED,
         },
         CANCEL_PACKAGE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                 DistributeStatus.PACKAGED
                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,
@@ -804,67 +686,56 @@
                 DistributeStatus.OUTSTORAGE_WAIT_PACKAGE,
                 DistributeStatus.PACKAGED, DistributeStatus.SERVICE_STOP,
                 DistributeStatus.OUTSTORAGE_PACKAGED,
                 DistributeStatus.HGVENDING_INIT, DistributeStatus.HGVENDING_WAIT_PICKUP, DistributeStatus.CUS_CONFIRM_AT_HGVENDING,
                 DistributeStatus.HAITAO_INIT,
                 DistributeStatus.DEPOSITPAY,
                 DistributeStatus.TAILPAY_OVERTIME,
-                DistributeStatus.MAKEUP_POSTAGE_PAID,
             ],
 
             DistributeEventConstKey.TO_STATE_MAP_KEY: {
                 DistributeStatus.INIT: DistributeStatus.SPLIT,
                 DistributeStatus.PRINTED: DistributeStatus.SPLIT,
-                DistributeStatus.CUSSERVICE_PICKED_UP: None,
+                DistributeStatus.CUSSERVICE_PICKED_UP: DistributeStatus.SPLIT,
                 DistributeStatus.GUIDE_PICKED_UP: DistributeStatus.SPLIT,
-                DistributeStatus.SERVICE_STORE: None,
-                DistributeStatus.SERVICE_DESK: None,
+                DistributeStatus.SERVICE_STORE: DistributeStatus.SPLIT,
+                DistributeStatus.SERVICE_DESK: DistributeStatus.SPLIT,
                 DistributeStatus.PACKAGED: None,
                 DistributeStatus.CUS_CONFIRM: None,
                 DistributeStatus.CUS_CONFIRM_AT_GUIDE: None,
                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE: None,
                 DistributeStatus.CUS_CONFIRM_AT_VIRTUAL: None,
                 DistributeStatus.OUTSTORAGE_WAIT_PACKAGE: DistributeStatus.SPLIT,
                 DistributeStatus.PACKAGED: None,
                 DistributeStatus.OUTSTORAGE_PACKAGED: None,
                 DistributeStatus.HGVENDING_INIT: None,
                 DistributeStatus.HGVENDING_WAIT_PICKUP: None,
                 DistributeStatus.CUS_CONFIRM_AT_HGVENDING: None,
                 DistributeStatus.HAITAO_INIT: None,
                 DistributeStatus.DEPOSITPAY: None,
-                DistributeStatus.SERVICE_STOP: None,
-                # DistributeStatus.HAITAO_INIT: None,
+                DistributeStatus.SERVICE_STOP: DistributeStatus.SPLIT,
+            #    DistributeStatus.HAITAO_INIT: None,
                 DistributeStatus.TAILPAY_OVERTIME: None,
-                DistributeStatus.MAKEUP_POSTAGE_PAID: None,
             },
         },
         CLOSE_AFTERSALE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
+                DistributeStatus.CUSSERVICE_HOLD, DistributeStatus.PACKAGED,
                 DistributeStatus.CUS_CONFIRM,
                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
                 DistributeStatus.CUS_CONFIRM_AT_VIRTUAL,
-                DistributeStatus.CUSSERVICE_HOLD,
-                DistributeStatus.PACKAGED,
-                DistributeStatus.OUTSTORAGE_PACKAGED,
-                DistributeStatus.OUTSTORAGE_WAIT_PACKAGE,
-                DistributeStatus.OUTSTORAGE_RETURN,
-                DistributeStatus.INIT,
-                DistributeStatus.PRINTED,
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.GUIDE_PICKED_UP,
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.SERVICE_STORE,
-                DistributeStatus.HGVENDING_INIT,
-                DistributeStatus.HGVENDING_WAIT_PICKUP,
+                DistributeStatus.CUSSERVICE_HOLD, DistributeStatus.PACKAGED, DistributeStatus.OUTSTORAGE_PACKAGED,
+                DistributeStatus.OUTSTORAGE_WAIT_PACKAGE, DistributeStatus.OUTSTORAGE_RETURN,
+                DistributeStatus.INIT, DistributeStatus.PRINTED, DistributeStatus.CUSSERVICE_PICKED_UP,
+                DistributeStatus.GUIDE_PICKED_UP, DistributeStatus.SERVICE_DESK, DistributeStatus.SERVICE_STORE,
+                DistributeStatus.HGVENDING_INIT, DistributeStatus.HGVENDING_WAIT_PICKUP,
                 DistributeStatus.SERVICE_STOP,
                 DistributeStatus.DEPOSITPAY,
                 DistributeStatus.TAILPAY_OVERTIME,
-                DistributeStatus.MAKEUP_POSTAGE_PAID,
-                DistributeStatus.AFTERSALE_WH,
                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,
         },
         COMPLETE_AFTERSALE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                 DistributeStatus.INIT,
                 DistributeStatus.PRINTED,
@@ -872,17 +743,14 @@
                 DistributeStatus.OUTSTORAGE_WAIT_PACKAGE,
                 DistributeStatus.HGVENDING_INIT,
                 DistributeStatus.HGVENDING_WAIT_PICKUP,
                 DistributeStatus.CUS_CONFIRM_AT_VIRTUAL,
                 DistributeStatus.HAITAO_INIT,
                 DistributeStatus.DEPOSITPAY,
                 DistributeStatus.TAILPAY_OVERTIME,
-                DistributeStatus.MAKEUP_POSTAGE_PAID,
-                DistributeStatus.PACKAGED,
-                DistributeStatus.AFTERSALE_WH,
                 ],
             DistributeEventConstKey.TO_STATE_MAP_KEY: {
                 DistributeStatus.INIT: DistributeStatus.NO_PICKUP_RETURN,
                 DistributeStatus.PRINTED: DistributeStatus.NO_PICKUP_RETURN,
                 DistributeStatus.GUIDE_PICKED_UP: DistributeStatus.NO_PICKUP_RETURN,
                 DistributeStatus.HGVENDING_INIT: DistributeStatus.HGVENDING_NO_PICKUP_RETURN,
                 DistributeStatus.HGVENDING_WAIT_PICKUP: DistributeStatus.HGVENDING_NO_PICKUP_RETURN,
@@ -890,16 +758,14 @@
                 # DistributeStatus.OUTSTORAGE_WAIT_PACKAGE: DistributeStatus.OUTSTORAGE_RETURN
                 # DistributeStatus.CUSSERVICE_PICKED_UP:DistributeStatus.CUSSERVICE_HOLD,
                 # DistributeStatus.SERVICE_DESK:DistributeStatus.CUSSERVICE_HOLD,
                 # DistributeStatus.SERVICE_STORE:DistributeStatus.CUSSERVICE_HOLD,
                 DistributeStatus.DEPOSITPAY: DistributeStatus.DEPOSITPAY_RETURN,
                 DistributeStatus.TAILPAY_OVERTIME: DistributeStatus.DEPOSITPAY_RETURN,
                 DistributeStatus.CUS_CONFIRM_AT_VIRTUAL: None,
-                DistributeStatus.MAKEUP_POSTAGE_PAID: None,
-                DistributeStatus.PACKAGED: None,
             }
         },
         CREATE_EXPRESS: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                                 DistributeStatus.INIT,
                                 DistributeStatus.PRINTED,
                                 DistributeStatus.CUSSERVICE_PICKED_UP,
@@ -937,17 +803,15 @@
             DistributeEventConstKey.TO_STATUS_KEY: None,
         },
         CUSSERVICE_RETURN: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                                 DistributeStatus.CUSSERVICE_PICKED_UP,
                                 DistributeStatus.SERVICE_DESK,
                                 DistributeStatus.SERVICE_STORE,
-                                DistributeStatus.SERVICE_STOP,
-                                DistributeStatus.AFTERSALE_WH,
-                                ],
+                                DistributeStatus.SERVICE_STOP],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.CUSSERVICE_HOLD,  # 客服已退
         },
         OUTSTORAGE_RETURN: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                                 DistributeStatus.OUTSTORAGE_WAIT_PACKAGE],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.OUTSTORAGE_RETURN,  # 外仓已退
         },
@@ -968,33 +832,30 @@
             DistributeEventConstKey.TO_STATUS_KEY: None,
         },
         EXCHANGE_OPEN: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [  # 仅支持发货单邮寄或者自提后进行换货申请，外仓不支持换货
                                 DistributeStatus.PACKAGED,
                                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
-                                DistributeStatus.OUTSTORAGE_PACKAGED,
                                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,  # 发货单状态不变更
         },
         EXCHANGE_CANCEL: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [  # 仅支持发货单邮寄或者自提后进行换货申请，外仓不支持换货
                                 DistributeStatus.PACKAGED,
                                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
-                                DistributeStatus.OUTSTORAGE_PACKAGED,
                                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,  # 发货单状态不变更
         },
         EXCHANGE_DONE: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [  # 仅支持发货单邮寄或者自提后进行换货申请，外仓不支持换货
                                 DistributeStatus.PACKAGED,
                                 DistributeStatus.CUS_CONFIRM_AT_GUIDE,
                                 DistributeStatus.CUS_CONFIRM_AT_CUSSERVICE,
-                                DistributeStatus.OUTSTORAGE_PACKAGED,
                                 ],
             DistributeEventConstKey.TO_STATUS_KEY: None,  # 发货单状态不变更
         },
         RETURN_DEPOSIT: {  # 分阶段支付--退定金
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                 DistributeStatus.DEPOSITPAY,
                 DistributeStatus.TAILPAY_OVERTIME,
@@ -1066,91 +927,21 @@
                                 DistributeStatus.GUIDE_PICKED_UP,
                                 DistributeStatus.SERVICE_DESK,
                                 DistributeStatus.SERVICE_STORE,
                                 DistributeStatus.SERVICE_STOP,
             ],
             DistributeEventConstKey.TO_STATUS_KEY: None
         },
-        AFSPLUS_S2E: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT, DistributeStatus.PRINTED,
-                                DistributeStatus.CUSSERVICE_PICKED_UP,
-                                DistributeStatus.GUIDE_PICKED_UP,
-                                DistributeStatus.SERVICE_DESK,
-                                DistributeStatus.SERVICE_STORE,
-                                DistributeStatus.SERVICE_STOP,
-            ],
-            DistributeEventConstKey.TO_STATUS_KEY: None
-        },
-        AFSPLUS_E2S: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT, DistributeStatus.PRINTED,
-                                DistributeStatus.CUSSERVICE_PICKED_UP,
-                                DistributeStatus.GUIDE_PICKED_UP,
-                                DistributeStatus.SERVICE_DESK,
-                                DistributeStatus.SERVICE_STORE,
-                                DistributeStatus.SERVICE_STOP,
-            ],
-            DistributeEventConstKey.TO_STATUS_KEY: None
-        },
-        AFSPLUS_TO_EXPRESS: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT, DistributeStatus.PRINTED,
-                                DistributeStatus.CUSSERVICE_PICKED_UP,
-                                DistributeStatus.GUIDE_PICKED_UP,
-                                DistributeStatus.SERVICE_DESK,
-                                DistributeStatus.SERVICE_STORE,
-                                DistributeStatus.SERVICE_STOP,
-            ],
-            DistributeEventConstKey.TO_STATUS_KEY: None
-        },
-        AFSPLUS_TO_SELF_SERVICE: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.INIT, DistributeStatus.PRINTED,
-                                DistributeStatus.CUSSERVICE_PICKED_UP,
-                                DistributeStatus.GUIDE_PICKED_UP,
-                                DistributeStatus.SERVICE_DESK,
-                                DistributeStatus.SERVICE_STORE,
-                                DistributeStatus.SERVICE_STOP,
-            ],
-            DistributeEventConstKey.TO_STATUS_KEY: None
-        },
-
         # 2022.08 虚拟商品确收事件
         CUS_CONFIRM_AT_VIRTUAL: {
             DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
                 DistributeStatus.VIRTUAL_INIT],
             DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.CUS_CONFIRM_AT_VIRTUAL,
         },
-        # 2022.12.16 云打印面单
-        CLOUDPRINT_SHIPPING_NUMBER:{
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.PACKAGED,
-            ],
-            DistributeEventConstKey.TO_STATUS_KEY: None
-        },
-        # 2023.4 售后仓入库 (位于客服处的发货单，可以执行售后仓入库)
-        ENTER_AFTERSALE_WH: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.SERVICE_STOP,
-                DistributeStatus.SERVICE_STORE,
-                ],
-            DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.AFTERSALE_WH,
-        },
-        MANUAL_SPLIT: {
-            DistributeEventConstKey.FROM_STATUS_LIST_KEY: [
-                DistributeStatus.CUSSERVICE_PICKED_UP,
-                DistributeStatus.SERVICE_DESK,
-                DistributeStatus.SERVICE_STOP,
-                DistributeStatus.SERVICE_STORE,
-                ],
-            DistributeEventConstKey.TO_STATUS_KEY: DistributeStatus.SPLIT,
-        },
+
     }
 
     EVENT_TO_BUTTONNAME_MAP = {
         NEW_ADD: "新增发货单",
         PRINT: '打印',
         GUIDE_PRINT: '导购打单',
         PRINT_AND_OVERWRITE_EXPRESS: '更新运单并打印',
@@ -1222,25 +1013,17 @@
         # 合单催配货消息功能
         PUSH_GUIDE_ASSIGN: "合单催配送提醒",
 
         # 特殊售后单
         AFSPLUS_OPEN: "申请特殊售后",
         AFSPLUS_CLOSE: "取消特殊售后",
         AFSPLUS_COMPLETE: "完成特殊售后",
-        AFSPLUS_S2E: "自提转快递",  # 自提转快递
-        AFSPLUS_E2S: "快递转自提",  # 快递转自提
-        AFSPLUS_TO_EXPRESS: "转快递",
-        AFSPLUS_TO_SELF_SERVICE: "转自提",
 
         # 虚拟商品
-        CUS_CONFIRM_AT_VIRTUAL: "虚拟商品确收",
-        CLOUDPRINT_SHIPPING_NUMBER: "打印面单",
-        # 售后
-        ENTER_AFTERSALE_WH: "售后仓入库",
-        MANUAL_SPLIT: "手动拆单",
+        CUS_CONFIRM_AT_VIRTUAL: "虚拟商品确收"
     }
 
 
 def get_available_event_list(distribute_status):
     '''
     根据发货单的状态，获取可进行的操作事件列表
     '''
@@ -1261,16 +1044,15 @@
         DistributeEventConst.EXCHANGE_DONE,
         DistributeEventConst.HGVENDING_PICKED_UP,
         DistributeEventConst.CUS_CONFIRM_AT_HGVENDING,
         DistributeEventConst.PAY_TAIL,
         DistributeEventConst.RETURN_DEPOSIT,
         DistributeEventConst.OVERTIME_TAILPAY,
         DistributeEventConst.HAITAO_PACKAGE,
-        DistributeEventConst.UPDATE_DELIVER_TIME,
-        DistributeEventConst.CLOUDPRINT_SHIPPING_NUMBER
+        DistributeEventConst.UPDATE_DELIVER_TIME
     ]
     from_to_map = DistributeEventConst.FROM_TO_MAP
     for event_name, event_dict in from_to_map.items():
         if DistributeEventConstKey.FROM_STATUS_LIST_KEY not in event_dict:
             continue
         from_status_list = event_dict.get(DistributeEventConstKey.FROM_STATUS_LIST_KEY)
         if distribute_status in from_status_list and event_name not in special_event_list:
@@ -1333,45 +1115,42 @@
     "108030": "01",
     "108048": "45",
     "108063": "15"
 }
 
 class AddressGroupStatus(object):
     """
-    可合-已齐、可合-未齐、无可合、已合单、在库已合、单单、无在库、其他
+    可合-已齐、可合-未齐、无可合、已合单、单单、其他
     """
-    # 可合-已齐（多单在库、未合、无其他状态）
+    # 可合-已齐
     MERGABLE_READY = "mergable_ready"
-    # 可合-未齐（多单在库、未合、有其他状态）
+    # 可合-未齐
     MERGABLE_WAITING = "mergable_waiting"
-    # 已合单（多单在库、已合、无其他状态）
+    # 已合单
     MERGED = "merged"
-    # 在库-已合（多单在库、已合、有其他状态）
+    # 在库-已合
     MERGED_IN_STORE = "merged_in_store"
-    # 无可合（一单在库、有其他状态）
+    # 无可合
     UNMERGABLE = "unmergable"
-    # 单单（一单在库、无其他状态）
+    # 单单
     SINGLE = 'single'
-    # 无在库（0单在库、有其他状态）
-    NO_IN_STORE = 'no_in_store'
     # 其他
     OTHER = 'other'
 
     CHOICES = (
         (MERGABLE_READY, '可合-已齐'),
         (MERGABLE_WAITING, '可合-未齐'),
         (MERGED, "已合单"),
         (MERGED_IN_STORE, "在库-已合"),
         (UNMERGABLE, "无可合"),
         (SINGLE, "单单"),
-        (NO_IN_STORE, "无在库"),
         (OTHER, "其他"),
     )
     # 存在未终结发货单的分组
-    UNTERMINATE_STATUS_LIST = [MERGABLE_READY, MERGABLE_WAITING, MERGED, MERGED_IN_STORE, UNMERGABLE, NO_IN_STORE, SINGLE]
+    UNTERMINATE_STATUS_LIST = [MERGABLE_READY,MERGABLE_WAITING, MERGED, UNMERGABLE, SINGLE]
 
 """
 发货单运送变更事件 枚举
 合单、更新运单
 TODO 修改地址、修改运输方式
 """
 @unique
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_distribute/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_distribute/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import datetime
 
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
 
 from ..core.base_models import BaseModelTimeAndDeleted
 from ..core.common_utils import get_uuid4_hex
-from ..core.constants import ShippingMethod
 from ..core.numbers import getRandomNumSet
 from ..sparrow_orders.constants import PayMethod
 from ..sparrow_orders.constants import DeliverTimeType
-from .constants import DistributeStatus
+from .constants import DistributeStatus, ShippingMethod
 from . import APP_LABEL
 
 __all__ = ['Distribute', 'Distributeline', 'FootPrint', 'ExpressRela',
            'QueryResult', 'QueryResultDetail', 'OlayToken', 'EventPool',
            'EventPoolDetail', 'DeviceConfig', 'AddressGroup', 'AddressGroupRela']
 
 
@@ -27,14 +26,19 @@
     return number
 
 
 class Distribute(BaseModelTimeAndDeleted):
     '''
     配货单总表
     '''
+    SHIPPING_METHOD_CHOICES = (
+        (ShippingMethod.EXPRESS, '快递'),
+        (ShippingMethod.SELF_SERVICE, '自提'),
+        (ShippingMethod.FLASH_DELIVERY, '闪送'),
+    )
     # id(主键uuid)
     id = models.CharField(max_length=100, primary_key=True, default=get_uuid4_hex, editable=False)
     # 发货单名称（包裹1、包裹2等，这个名称并不是固定的，由于客户提货或者售后造成的拆单，可能造成这个字段值发生变化）
     name = models.CharField("Distribute Name", max_length=128, blank=True, null=True, default="")
     # number(发货单号）
     number = models.CharField("Distribute number", max_length=128, db_index=True, unique=True, default=get_sparrow_distribute_number)
     # origin_id（原始发货单id）
@@ -48,15 +52,15 @@
     # 订单下单时间
     order_created_time = models.DateTimeField("Order Created Time", blank=True, null=True, default=None)
     # distribute_status(配货单状态：初始态、已打印、导购已取货、客服已取货、已发货等等)
     distribute_status = models.CharField('配货单状态', max_length=128, blank=True, null=True, choices=DistributeStatus.DISTRIBUTE_STATUS_CHOICES, db_index=True)
     # aftersale_status(有售后，无售后)
     aftersale_status = models.BooleanField("是否有售后", default=False, db_index=True)
     # shipping_method(发货方式：自提、快递、闪送)
-    shipping_method = models.CharField('发货方式', max_length=128, blank=True, null=True, choices=ShippingMethod.CHOICES, db_index=True)
+    shipping_method = models.CharField('发货方式', max_length=128, blank=True, null=True, choices=SHIPPING_METHOD_CHOICES, db_index=True)
     # print_times打印次数
     print_times = models.IntegerField(_("打印次数"), default=0)
     # shop_id(专柜id)
     shop_id = models.PositiveIntegerField('Shop ID', blank=True, null=True, db_index=True)
     # shop_num(专柜号)
     shop_num = models.CharField("Shop number", max_length=128, blank=True, db_index=True)
     # shop_name(专柜号)
@@ -198,22 +202,14 @@
     # 商品类目
     categories = models.CharField('商品类目', max_length=128, blank=True, null=True, default=None)
 
     # deliver_time_type 发货时间类型(fixed_time 固定时间/pay_relative_time支付相对时间)
     deliver_time_type = models.CharField("发货时间类型", max_length=32, choices=DeliverTimeType.DELIVERTIME_TYPE_CHOICES, blank=True, null=True)
     # deliver_relative_time 相对时间(单位：天)
     deliver_relative_time = models.DecimalField("相对时间", decimal_places=2, max_digits=12, blank=True, null=True)
-    ecard_info = None
-
-    # 2022.08 订单冗余sell_type
-    sell_type = models.CharField("sell_type", max_length=32, blank=True, null=True, db_index=True)
-
-    # 2022.11 发货仓
-    outstorage_id = models.CharField("发货仓", max_length=40, blank=True, null=True)
-    retstorage_id = models.CharField("退货仓", max_length=40, blank=True, null=True)
 
     class Meta:
         app_label = APP_LABEL
         ordering = ['-created_time']
 
 
 class FootPrint(BaseModelTimeAndDeleted):
@@ -556,66 +552,7 @@
 
     class Meta:
         app_label = APP_LABEL
         ordering = ['-created_time']
 
     def __str__(self):
         return f'{self.opt_username}-{self.opt_displayname}-{self.event_code}-{self.event_day}-{self.shop_name}'
-
-
-class DistributelineEcard(BaseModelTimeAndDeleted):
-    # order_id (订单主键)
-    order_id = models.PositiveIntegerField('Order ID', blank=True, null=True)
-    # order_number (订单编码)
-    order_number = models.CharField('Order Number', max_length=36, blank=True)
-    # line_id(订单行id)
-    line_id = models.PositiveIntegerField('Line ID', blank=True, null=True)
-    # distribute_id(发货单id)
-    distribute_id = models.CharField('Distribute ID', max_length=40, blank=True, null=True)
-    # distribute_number(发货单号）
-    distribute_number = models.CharField("Distribute Number", max_length=40)
-    # distribute_line_id(发货单Line id)
-    distribute_line_id = models.CharField('Distribute Line ID', max_length=40, blank=True, null=True, db_index=True)
-    # E卡卡号
-    ecard_number = models.CharField("Ecard Number", max_length=40)
-    class Meta:
-        app_label = APP_LABEL
-
-
-class ExpressRelaBack(BaseModelTimeAndDeleted):
-    '''
-    发货单与运单关系历史表
-    被删除的关系表存在这里，以便查询发货单绑过的所有运单号
-    '''
-    # id(主键uuid)
-    id = models.CharField(max_length=100, primary_key=True, default=get_uuid4_hex, editable=False)
-    # distribute_id(新发货单id)
-    distribute_id = models.CharField('Distribute ID', max_length=40, default=get_uuid4_hex, db_index=True)
-    # distribute_number(新发货单id)
-    distribute_number = models.CharField('Distribute Number', max_length=40)
-    # order_id (订单主键)
-    order_id = models.PositiveIntegerField('Order ID', blank=True, null=True, db_index=True)
-    # order_number (订单编码)
-    order_number = models.CharField('Order Number', max_length=36, blank=True, null=True)
-    # newexpressorder_id(运单信息id)
-    newexpressorder_id = models.CharField(max_length=40, default=get_uuid4_hex, editable=False)
-    # if_main 是否主单（当发生合单时，将给主单与运单关联数据打上此标记，表示运单先由此发货单生成）
-    if_main = models.BooleanField("是否主单", default=True)
-    # 是否参与了合单
-    if_merge = models.BooleanField("是否合单", default=False)
-    # 运单号
-    shipping_number = models.CharField("快递单号/母单号", max_length=64, blank=True, null=True, db_index=True)
-    # 快递公司中文
-    express_name = models.CharField("快递供应商", max_length=20, blank=True, null=True)
-    # 快递公司编码
-    express_code = models.CharField("快递代码", max_length=16, blank=True, null=True)
-    # 账号名称
-    account = models.CharField("账号名称", max_length=20, blank=True, null=True, default="")
-    # 删除时间
-    deleted_time = models.DateTimeField("Date Deleted", blank=True, null=True)
-    # 删除关联的原因
-    deleted_reason = models.CharField("删除原因", max_length=20, blank=True, null=True)
-
-    class Meta:
-        app_label = APP_LABEL
-        ordering = ['-created_time']
-
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from ..core.constants import UserRole
 
-BASE_EXCHANGE_API_CODE = 20106000
-
 
 class ExchangeOrderStatus(object):
     '''
     ### 换货单总单状态 ###
     '''
     IN_PROCESS = "in_process"
     CLOSED = "closed"
@@ -39,47 +37,44 @@
     CLOSED = "closed"
     # 待客户退回商品
     PENDING_RETURN = "pending_return"
     # 待确收商品
     PENDING_CONFIRM = "pending_confirm"
     # 待换货
     PENDING_EXCHANGE = "pending_exchange"
-    # 客服收到寄回商品
-    CUSSERVICE_RECEIVED = "cusservice_received"
-    # 退换货仓
-    AFTERSALE_WH = "AftersaleWH"
     # 换货完成
     DONE = "done"
-
     EXCHANGE_LINE_STATUS_CHOICES = (
         (OPEN, "待审核"),
         (PENDING_RETURN, "待客人寄回"),
         (PENDING_CONFIRM, "待专柜确收"),
         (PENDING_EXCHANGE, "待寄出换货"),
-        (CUSSERVICE_RECEIVED, "客服收到寄回商品"),
-        (AFTERSALE_WH, "退货仓上架"),
         (DONE, "换货完成"),
         (CLOSED, "已关闭"),
     )
     EXCHANGE_LINE_STATUS_DICT = dict(EXCHANGE_LINE_STATUS_CHOICES)
 
-    EXCHANGE_LINE_STATUS_CHOICES_FOR_A = EXCHANGE_LINE_STATUS_CHOICES
-
-    EXCHANGE_LINE_STATUS_CHOICES_FOR_B = (
+    EXCHANGE_LINE_STATUS_CHOICES_FOR_C = (
         (OPEN, "待审核"),
-        (PENDING_RETURN, "待客人寄回"),
-        (PENDING_CONFIRM, "待专柜确收"),
-        (PENDING_EXCHANGE, "待寄出换货"),
-        (CUSSERVICE_RECEIVED, "客服收到寄回商品"),
-        (AFTERSALE_WH, "客服已收退货"),
+        (PENDING_RETURN, "待寄回"),
+        (PENDING_CONFIRM, "待换货"),
+        (PENDING_EXCHANGE, "待换货"),
         (DONE, "换货完成"),
-        (CLOSED, "已关闭"),
+        (CLOSED, "换货关闭"),
     )
+    EXCHANGE_LINE_STATUS_DICT_FOR_C = dict(EXCHANGE_LINE_STATUS_CHOICES_FOR_C)
 
-    EXCHANGE_LINE_STATUS_CHOICES_FOR_P = EXCHANGE_LINE_STATUS_CHOICES
+    EXCHANGE_MESSAGE_DICT_FOR_C = {
+        OPEN: "您的售后已申请成功，待售后审核中",
+        PENDING_RETURN: "您的售后审核已通过，待寄回换货商品",
+        PENDING_CONFIRM: "您的售后物流已提交，待专柜处理换货商品",
+        PENDING_EXCHANGE: "您的售后物流已提交，待专柜处理换货商品",
+        DONE: "售后服务已完成，感谢您对汉光的支持",
+        CLOSED: "售后服务已关闭，感谢您对汉光的支持"
+    }
 
 
 class EventMapKey(object):
 
     TO_STATUS_KEY = "to_status"
     USER_ROLES_KEY = "user_roles"
 
@@ -112,20 +107,14 @@
     MODIFY_CUS_SHIPPING_NUMBER = "modify_cus_shipping_number"
     # 催导购确收
     PUSH_GUIDE_CONFIRM = "push_guide_confirm"
     # 催导购审核
     PUSH_GUIDE_APPROVE = "push_guide_approve"
     # 催导购寄出
     PUSH_GUIDE_EXPRESS = "push_guide_express"
-    # 客服收货
-    CUSSERVICE_RECEIVE = "cusservice_receive"
-    # 取消客服收货
-    CANCEL_CUSSERVICE_RECEIVE = "cancel_cusservice_receive"
-    # 售后仓入库、上架
-    ENTER_AFTERSALE_WH = "enter_aftersale_wh"
 
     EVENT_2_BUTTONNAME_MAP = {
         NEW_ADD: "创建换货单",
         APPROVE: "通过",
         CANCEL: "关闭",
         CUS_SELF_SERVICE: "现换",
         CUS_WRITE_BACK: "客户回填运单信息",
@@ -134,17 +123,14 @@
         COMMENT: "备注",
         PRINT: "打印",
         MODIFY_ADDRESS: "修改换货地址",
         MODIFY_CUS_SHIPPING_NUMBER: "修改客户回填运单号",
         PUSH_GUIDE_CONFIRM: "催确收",
         PUSH_GUIDE_APPROVE: "催审核",
         PUSH_GUIDE_EXPRESS: "催寄出",
-        CUSSERVICE_RECEIVE: "客服收货",
-        CANCEL_CUSSERVICE_RECEIVE: "取消客服收货",
-        ENTER_AFTERSALE_WH: "售后仓入库",
     }
 
     EVENT_2_CNAME_MAP = {
         CUS_SELF_SERVICE: "客人现场换货",
         APPROVE: "通过审核",
         CANCEL: "关闭换货",
     }
@@ -152,144 +138,123 @@
     # 注意：
     # 1、当不存在EventMapKey.USER_ROLES_KEY的key时，说明所有角色都可以操作；
     # 2、当EventMapKey.TO_STATUS_KEY对应的value设置为None时，则说明动作不会造成状态变更；
     FROM_TO_MAP = {
         NEW_ADD: {  # 创建换货单
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSTOMER, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSTOMER]
             }
         },
         APPROVE: {  # 导购同意客户换货
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.PENDING_RETURN,
                 EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE]
             }
         },
         CANCEL: {  # 取消换货
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CLOSED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CLOSED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CLOSED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CLOSED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
         },
         CUS_SELF_SERVICE: {  # 客人自提
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.DONE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.DONE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.DONE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.DONE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
         },
         CUS_WRITE_BACK: {  # 客户回填运单信息
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.PENDING_CONFIRM,
                 EventMapKey.USER_ROLES_KEY: [UserRole.CUSTOMER]
             },
         },
         CONFIRM: {  # 确收
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.PENDING_EXCHANGE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.PENDING_EXCHANGE,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
         },
         GUIDE_EXPRESS: {  # 导购发货
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.DONE,
                 EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE]
             },
         },
         PRINT: {  # 打印
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.DONE: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
         },
         COMMENT: {
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.DONE: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.GUIDE, UserRole.CUSSERVICE]
+                EventMapKey.USER_ROLES_KEY: [UserRole.GUIDE, UserRole.CUSSERVICE]
             },
         },
         MODIFY_ADDRESS: {
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: None,
                 EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE]
             },
@@ -305,73 +270,47 @@
                 EventMapKey.TO_STATUS_KEY: None,
                 EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE]
             }
         },
         MODIFY_CUS_SHIPPING_NUMBER: {
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.CUSTOMER]
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE, UserRole.CUSTOMER]
             },
+            ExchangeLineStatus.PENDING_EXCHANGE: {
+                EventMapKey.TO_STATUS_KEY: None,
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE]
+            }
         },
         PUSH_GUIDE_CONFIRM: {
             ExchangeLineStatus.PENDING_CONFIRM: {
                 EventMapKey.TO_STATUS_KEY: None,
                 EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE]
             },
             ExchangeLineStatus.PENDING_RETURN: {
                 EventMapKey.TO_STATUS_KEY: None,
                 EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE]
             }
         },
         PUSH_GUIDE_APPROVE: {
             ExchangeLineStatus.OPEN: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE, UserRole.AUTO]
             },
         },
         PUSH_GUIDE_EXPRESS: {
             ExchangeLineStatus.PENDING_EXCHANGE: {
                 EventMapKey.TO_STATUS_KEY: None,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
+                EventMapKey.USER_ROLES_KEY: [UserRole.CUSSERVICE, UserRole.AUTO]
             }
-        },
-        CUSSERVICE_RECEIVE: {
-            ExchangeLineStatus.PENDING_RETURN: {
-                EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CUSSERVICE_RECEIVED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
-            },
-            ExchangeLineStatus.PENDING_CONFIRM: {
-                EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.CUSSERVICE_RECEIVED,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
-            },
-        },
-        CANCEL_CUSSERVICE_RECEIVE: {
-            ExchangeLineStatus.CUSSERVICE_RECEIVED: {
-                EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.PENDING_CONFIRM,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
-            },
-        },
-        ENTER_AFTERSALE_WH: {
-            ExchangeLineStatus.CUSSERVICE_RECEIVED: {
-                EventMapKey.TO_STATUS_KEY: ExchangeLineStatus.AFTERSALE_WH,
-                EventMapKey.USER_ROLES_KEY: [
-                    UserRole.CUSSERVICE, UserRole.AUTO]
-            },
-        },
+        }
     }
 
     # 按钮排序
     EVENT_CONST_SORT_MAP = {
         CANCEL: 0,
         COMMENT: 1,
         APPROVE: 2,
@@ -395,28 +334,25 @@
     for event_code, event_dict in from_to_map.items():
         if event_code in special_event_list:
             continue
 
         if exline_status not in event_dict:
             continue
         to_status_dict = event_dict.get(exline_status)
-        to_status_user_role_list = to_status_dict.get(
-            EventMapKey.USER_ROLES_KEY, None)
+        to_status_user_role_list = to_status_dict.get(EventMapKey.USER_ROLES_KEY, None)
 
-        event_str = event_code + "|" + \
-            ExchangeEventConst.EVENT_2_BUTTONNAME_MAP.get(event_code)
+        event_str = event_code + "|" + ExchangeEventConst.EVENT_2_BUTTONNAME_MAP.get(event_code)
 
         # 当不存在EventMapKey.USER_ROLES_KEY的key时，说明所有角色都可以操作；
         if not to_status_user_role_list:
             available_event_list.append(event_str)
         else:
             if user_role in to_status_user_role_list:
                 available_event_list.append(event_str)
-    available_event_list.sort(
-        key=lambda event_str: ExchangeEventConst.EVENT_CONST_SORT_MAP.get(event_str.split("|")[0], 0))
+    available_event_list.sort(key=lambda event_str: ExchangeEventConst.EVENT_CONST_SORT_MAP.get(event_str.split("|")[0], 0))
     return available_event_list
 
 
 EXCHANGE_USER_REASON = [
     "无理由换货",
     "尺码/颜色不合适",
     "质量问题",
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_exchange/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_exchange/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_orders/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_orders/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 from ..core.model_function import get_object_or_None
 from ..core.common_utils import get_setting_value
 from ..core.common_utils import get_uuid4_hex
 from ..core.base_models import BaseModelTimeAndDeleted
 from ..core.base_models import BaseModelNew
 from ..core.base_models import AbstractAddress
-from ..core.constants import ShippingMethod
 from ..core.constants import MemberLevel
 from ..core.constants import PayType
 from ..core.constants import LogLevel
 from ..sparrow_promotions.models import Coupon
 from .constants import OrderShippingStatus
+from .constants import OrderShippingMethods
 from .constants import OrderPayStatus
 from .constants import OrderAssignStatus
 from .constants import OrderAftersaleStatus
 from .constants import OrderGroupStatus
 from .constants import OrderTypes
 from .constants import OrderExchangeStatus
 from .constants import PayMethod
@@ -38,22 +38,22 @@
 from .constants import CouponSource
 from .constants import PayStepType
 from .constants import ReversedStockStatus
 from .constants import ReversedStockType
 from .constants import ReversedStockActions
 from .constants import AssignmentStatus
 from .constants import AssignmentActions
-from ..sparrow_aftersale.constants import AftersaleStatus
-from ..sparrow_aftersale.constants import AftersaleFinanceStatus
-from ..sparrow_aftersale.constants import AftersaleRefundStatus
-from ..sparrow_aftersale.constants import AftersaleFinanceType
-from ..sparrow_aftersale.constants import AftersaleSource
-from ..sparrow_aftersale.constants import AftersaleCancelSource
-from ..sparrow_aftersale.constants import AfterSaleType
-from ..sparrow_aftersale.constants import AftersaleActions
+from .constants import AftersaleStatus
+from .constants import AftersaleFinanceStatus
+from .constants import RefundStatus
+from .constants import AftersaleFinanceType
+from .constants import AftersaleSource
+from .constants import CancelSource
+from .constants import AfterSaleType
+from .constants import AftersaleActions
 from .constants import OrderActions
 from .constants import SettingsLabel
 from .constants import BatchAssignTaskStatus
 from .constants import BatchAssignType
 from .constants import DeliverTimeType
 from .constants import HGVendingStatus
 from .constants import Order_Number_Pay_Status
@@ -281,14 +281,18 @@
         app_label = APP_LABEL
 
 
 class Order(BaseModelTimeAndDeleted):
     '''
     订单
     '''
+    SHIPPING_METHOD = (
+        (OrderShippingMethods.SELF_SERVICE, "到店自提"),  # 客户到店自提
+        (OrderShippingMethods.EXPRESS, "快递"),   # 商品采用快递形式
+    )
     # 支付状态
     PAY_STATUS = (
         (OrderPayStatus.UNPAID, "未支付"),
         (OrderPayStatus.PAY_FINISHED, "支付已完成"),
         (OrderPayStatus.CLOSED, "订单关闭"),
     )
     # 配货状态
@@ -344,15 +348,15 @@
         db_index=True)
     flashsale_guide_id = models.CharField(
         "闪购提货导购",
         max_length=100, blank=True, null=True, db_index=True)
     # 邮寄方式
     shipping_method = models.CharField(
         "Shipping method",
-        max_length=128, choices=ShippingMethod.CHOICES,
+        max_length=128, choices=SHIPPING_METHOD,
         blank=True, null=True)
     # 邮费
     postage = models.DecimalField(
         "Postage",
         decimal_places=2, max_digits=12, default=0.00)
     # 订单支付状态
     pay_status = models.CharField(
@@ -833,30 +837,30 @@
     AFTERSALE_FINANCE_STATUS_CHOICES = (
         (AftersaleFinanceStatus.INIT, "财务未审"),
         (AftersaleFinanceStatus.APPROVED_1ST, "财务一审通过，待二审"),
         (AftersaleFinanceStatus.APPROVED, "财务二审通过"),
         (AftersaleFinanceStatus.REJECTED, "财务驳回")
     )
     REFUND_STATUS_CHOICES = (
-        (AftersaleRefundStatus.INIT, "未退款"),
-        (AftersaleRefundStatus.SUCCEEDED, "退款成功"),
-        (AftersaleRefundStatus.FAILED, "退款失败")
+        (RefundStatus.INIT, "未退款"),
+        (RefundStatus.SUCCEEDED, "退款成功"),
+        (RefundStatus.FAILED, "退款失败")
     )
     AFTERSALE_FINANCE_TYPE_CHOICES = (
         (AftersaleFinanceType.AUTO, "正常退单"),
         (AftersaleFinanceType.MANUAL, "需要财务手动调账退款"),
     )
     AFTERSALE_SOURCE_CHOICES = (
         (AftersaleSource.GUEST_INITIATED, "客人发起"),
         (AftersaleSource.SERVICE_INITIATED, "客服发起"),
     )
     CANCEL_SOURCE_CHOICES = (
-        (AftersaleCancelSource.GUEST_CANCEL, "客人取消"),
-        (AftersaleCancelSource.SERVICE_CANCEL, "客服取消"),
-        (AftersaleCancelSource.TIMEOUT_CANCEL, "超时自动取消"),
+        (CancelSource.GUEST_CANCEL, "客人取消"),
+        (CancelSource.SERVICE_CANCEL, "客服取消"),
+        (CancelSource.TIMEOUT_CANCEL, "超时自动取消"),
     )
     AFTERSALE_TYPE_CHOICES = (
         (AfterSaleType.NORMAL, "正常退款"),
         (AfterSaleType.EXCHANGE, "换货"),
         (AfterSaleType.COMPLAINT, "投诉"),
         (AfterSaleType.REMINDER, "提醒发货"),
     )
@@ -898,15 +902,15 @@
     # 退款状态
     refund_status = models.CharField(
         "退款状态",
         max_length=128,
         choices=REFUND_STATUS_CHOICES,
         blank=True,
         null=True,
-        default=AftersaleRefundStatus.INIT)
+        default=RefundStatus.INIT)
     # 财务要的退款时间，找财务确认是要发起微信退款的时间还是微信退款到账的时间
     # 应该是调起微信退款接口的时间
     refund_time = models.DateTimeField("发起退款的时间", blank=True, null=True, db_index=True)
     # 收到推送退款成功的时间，一期就是收到微信通知成功的时间
     refund_notified_time = models.DateTimeField("退款收到推送的时间", blank=True, null=True, db_index=True)
     # 售后单同步信息
     sync_status = models.BooleanField('同步状态', default=False)
@@ -1743,19 +1747,19 @@
         )
 
     # TODO: @property
     # @property
     # def product(self):
     #     return get_object_or_None(Product, id=self.product_id)
 
-    # @property
-    # def productmain_id(self):
-    #     # GIO 埋点用
-    #     product = self.product
-    #     return product.productmain_id if product else None
+    @property
+    def productmain_id(self):
+        # GIO 埋点用
+        product = self.product
+        return product.productmain_id if product else None
 
     @cached_property
     def fixed_price_product(self):
         # 有时候需要知道这个line是不是加价购
         return get_object_or_None(OrderPromotionFixedPriceProduct, line_id=self.id)
 
     @classmethod
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,28 +131,25 @@
 
 class ExpressName:
     """ 包裹管理中给前端用的快递公司 """
 
     SF = 'sf'
     YZ = 'yz'
     ZTO = 'zto'
-    JD = 'jd'
 
     CODE_2_system_codes = {
         SF: [Partner.SF, Partner.SFTCJS],
         YZ: [Partner.YZPY],
-        ZTO: [Partner.ZTO],
-        JD: [Partner.JD],
+        ZTO: [Partner.ZTO]
     }
 
     CODE_2_NAME_MAP = {
         SF: "顺丰",
         YZ: "邮政",
         ZTO: "中通",
-        JD: "京东",
     }
 
     EXPRESS_NAME_INFOS = [
         {
             "name": CODE_2_NAME_MAP[SF],
             "code": SF,
         },
@@ -160,12 +157,8 @@
             "name": CODE_2_NAME_MAP[YZ],
             "code": YZ,
         },
         {
             "name": CODE_2_NAME_MAP[ZTO],
             "code": ZTO,
         },
-        {
-            "name": CODE_2_NAME_MAP[JD],
-            "code": JD,
-        },
     ]
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_parcel/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_parcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_promotions/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_promotions/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/constants.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,34 +33,14 @@
     # 其它
     OTHERS = "others"
     # 专柜代发
     SHOP = "shop"
     # 闪送
     SS = "ss"
 
-    # code to name
-    CODE_2_NAME_MAP = {
-        SF: "顺丰",
-        SFTCJS: "顺丰同城急送",
-        YTO: "圆通",
-        ZTO: "中通",
-        STO: "申通",
-        EMS: "EMS",
-        YZPY: "邮政",
-        YD: "韵达",
-        ZJS: "宅急送",
-        JD: "京东",
-        DBL: "德邦",
-        HTKY: "百世快递",
-        HHTT: "天天",
-        OTHERS: "其它",
-        SHOP: "专柜代发",
-        SS: "闪送",
-    }
-
 
 # 快递公司代号与中文对照
 ShippingPartnerCodes_DICT = {
     ShippingPartnerCodes.SF: "顺丰",
     ShippingPartnerCodes.SFTCJS: "顺丰同城急送",
     ShippingPartnerCodes.YTO: "圆通",
     ShippingPartnerCodes.ZTO: "中通",
```

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib/sparrow_shipping/models.py` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib/sparrow_shipping/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.82/src/sparrow_order_lib.egg-info/SOURCES.txt` & `sparrow-order-lib-0.1.9/src/sparrow_order_lib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 pyproject.toml
 setup.cfg
 src/sparrow_order_lib/__init__.py
 src/sparrow_order_lib/example.py
 src/sparrow_order_lib.egg-info/PKG-INFO
 src/sparrow_order_lib.egg-info/SOURCES.txt
 src/sparrow_order_lib.egg-info/dependency_links.txt
-src/sparrow_order_lib.egg-info/requires.txt
 src/sparrow_order_lib.egg-info/top_level.txt
 src/sparrow_order_lib/core/__init__.py
 src/sparrow_order_lib/core/base_models.py
 src/sparrow_order_lib/core/common_utils.py
 src/sparrow_order_lib/core/constants.py
 src/sparrow_order_lib/core/datastructures.py
 src/sparrow_order_lib/core/decorators.py
 src/sparrow_order_lib/core/dt_utils.py
 src/sparrow_order_lib/core/formats.py
 src/sparrow_order_lib/core/model_function.py
 src/sparrow_order_lib/core/numbers.py
 src/sparrow_order_lib/core/text.py
-src/sparrow_order_lib/core/xls_util.py
 src/sparrow_order_lib/db_tool/__init__.py
 src/sparrow_order_lib/db_tool/query.py
 src/sparrow_order_lib/es/__init__.py
 src/sparrow_order_lib/es/constants.py
 src/sparrow_order_lib/es/mapping_constants.py
 src/sparrow_order_lib/es/query_mapping_constants.py
 src/sparrow_order_lib/es/test_order_doc_type.py
@@ -56,41 +54,26 @@
 src/sparrow_order_lib/remote_call/__init__.py
 src/sparrow_order_lib/remote_call/sparrow_api_path.py
 src/sparrow_order_lib/remote_call/sparrow_core.py
 src/sparrow_order_lib/remote_call/sparrow_core_go.py
 src/sparrow_order_lib/remote_call/sparrow_lanyue.py
 src/sparrow_order_lib/remote_call/sparrow_product.py
 src/sparrow_order_lib/remote_call/svc_config.py
-src/sparrow_order_lib/sparrow_afsplus/__init__.py
-src/sparrow_order_lib/sparrow_afsplus/constants.py
-src/sparrow_order_lib/sparrow_afsplus/models.py
-src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
-src/sparrow_order_lib/sparrow_afsplus/utils.py
 src/sparrow_order_lib/sparrow_aftersale/__init__.py
-src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
 src/sparrow_order_lib/sparrow_aftersale/constants.py
 src/sparrow_order_lib/sparrow_aftersale/models.py
 src/sparrow_order_lib/sparrow_disstorage/__init__.py
 src/sparrow_order_lib/sparrow_disstorage/constants.py
-src/sparrow_order_lib/sparrow_disstorage/disstorage.py
 src/sparrow_order_lib/sparrow_disstorage/models.py
-src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
-src/sparrow_order_lib/sparrow_disstorage/serializers.py
-src/sparrow_order_lib/sparrow_disstorage/utils.py
 src/sparrow_order_lib/sparrow_distribute/__init__.py
 src/sparrow_order_lib/sparrow_distribute/constants.py
 src/sparrow_order_lib/sparrow_distribute/models.py
-src/sparrow_order_lib/sparrow_distribute/serializer_data.py
-src/sparrow_order_lib/sparrow_distribute/serializers.py
 src/sparrow_order_lib/sparrow_exchange/__init__.py
 src/sparrow_order_lib/sparrow_exchange/constants.py
 src/sparrow_order_lib/sparrow_exchange/models.py
-src/sparrow_order_lib/sparrow_inparcel/__init__.py
-src/sparrow_order_lib/sparrow_inparcel/constants.py
-src/sparrow_order_lib/sparrow_inparcel/models.py
 src/sparrow_order_lib/sparrow_orders/__init__.py
 src/sparrow_order_lib/sparrow_orders/constants.py
 src/sparrow_order_lib/sparrow_orders/models.py
 src/sparrow_order_lib/sparrow_parcel/__init__.py
 src/sparrow_order_lib/sparrow_parcel/constants.py
 src/sparrow_order_lib/sparrow_parcel/exceptions.py
 src/sparrow_order_lib/sparrow_parcel/models.py
```

