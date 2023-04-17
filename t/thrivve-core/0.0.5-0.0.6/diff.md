# Comparing `tmp/thrivve_core-0.0.5.tar.gz` & `tmp/thrivve_core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-227opmol/thrivve_core-0.0.5.tar", last modified: Tue Apr 11 12:56:35 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-f538kz9k/thrivve_core-0.0.6.tar", last modified: Sun Apr 16 14:01:16 2023, max compression
```

## Comparing `thrivve_core-0.0.5.tar` & `thrivve_core-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-11 12:56:12.000000 thrivve_core-0.0.5/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 12:56:35.000000 thrivve_core-0.0.5/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-16 14:01:08.000000 thrivve_core-0.0.6/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-16 14:01:16.000000 thrivve_core-0.0.6/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.0.5/PKG-INFO` & `thrivve_core-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.0.5
+Version: 0.0.6
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.5/setup.py` & `thrivve_core-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.0.5",
+    version="0.0.6",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
     packages=find_namespace_packages(
         include=["thrivve_core", "thrivve_core.*"]
-    ),  # ['thrivve_core'],
+    ),
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
 )
```

### Comparing `thrivve_core-0.0.5/thrivve_core/__init__.py` & `thrivve_core-0.0.6/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.0.6/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.0.6/thrivve_core/app_decorators/handle_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,27 @@
 
             user = verify_user_token(token=token, pre_login=pre_login, allowed_permissions=allowed_permissions)
 
             if append_auth_args and isinstance(append_auth_args, list):
                 for arg in append_auth_args:
                     if not kws.get('appended_kws'):
                         kws['appended_kws'] = dict()
+                    if '.' in arg:
 
-                    kws['appended_kws'][arg] = user.get(arg)
+                        if 'as' in arg:
+                            arg, as_arg = arg.split(' as ')
+                        else:
+                            as_arg = arg.replace('.', '_')
+
+                        obj, key = arg.split('.')
+                        value = user.get(obj, {}).get(key)
+
+                        kws['appended_kws'][as_arg] = value
+                    else:
+                        value = user.get(arg)
+                        kws['appended_kws'][arg] = value
 
             return func(*args, **kws)
 
         return inner_function
 
     return factory
```

### Comparing `thrivve_core-0.0.5/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.0.6/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.0.6/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.0.6/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/base.py` & `thrivve_core-0.0.6/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.0.6/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.0.6/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.0.6/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.0.6/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.0.6/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/auth.py` & `thrivve_core-0.0.6/thrivve_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/config.py` & `thrivve_core-0.0.6/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.0.6/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.0.6/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/enums.py` & `thrivve_core-0.0.6/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.0.6/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.0.6/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/filters.py` & `thrivve_core-0.0.6/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.0.6/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.0.6/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.0.6/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/log_config.py` & `thrivve_core-0.0.6/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.0.6/thrivve_core/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/notification_center.py` & `thrivve_core-0.0.6/thrivve_core/helpers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/search_function.py` & `thrivve_core-0.0.6/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/service_config.py` & `thrivve_core-0.0.6/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/sql.py` & `thrivve_core-0.0.6/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/time.py` & `thrivve_core-0.0.6/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/topics.py` & `thrivve_core-0.0.6/thrivve_core/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.0.6/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.0.6/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.5/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.0.6/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.5/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.0.6/thrivve_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,12 +41,13 @@
 thrivve_core/helpers/validate_mobile_number.py
 thrivve_core/helpers/validate_parameters.py
 thrivve_core/helpers/amazon/__init__.py
 thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
 thrivve_core/helpers/amazon/get_file_url.py
 thrivve_core/helpers/amazon/get_plain_url.py
 thrivve_core/helpers/amazon/get_s3_client.py
+thrivve_core/helpers/amazon/upload_file.py
 thrivve_core/helpers/database/__init__.py
 thrivve_core/helpers/database/base_model.py
 thrivve_core/helpers/database/log_model.py
 thrivve_core/helpers/kafka_producers/__init__.py
 thrivve_core/helpers/kafka_producers/log_model_changes.py
```

