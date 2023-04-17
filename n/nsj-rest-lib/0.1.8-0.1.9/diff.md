# Comparing `tmp/nsj_rest_lib-0.1.8.tar.gz` & `tmp/nsj_rest_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-0.1.8.tar", last modified: Wed Feb  1 15:28:33 2023, max compression
+gzip compressed data, was "nsj_rest_lib-0.1.9.tar", last modified: Wed Feb 15 09:59:06 2023, max compression
```

## Comparing `nsj_rest_lib-0.1.8.tar` & `nsj_rest_lib-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.414602 nsj_rest_lib-0.1.8/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-01 15:28:33.414602 nsj_rest_lib-0.1.8/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      130 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/README.md
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/pyproject.toml
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      888 2023-02-01 15:28:33.426602 nsj_rest_lib-0.1.8/setup.cfg
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.182602 nsj_rest_lib-0.1.8/src/
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.258602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.334602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       75 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3985 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      944 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4555 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5359 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4886 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5199 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4921 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.342602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dao/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    17853 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1223 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.362602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3987 2023-02-01 14:54:52.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.386602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     8871 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7563 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5408 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      195 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2295 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.394602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dto/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7218 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.402602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/entity/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      544 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      322 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      483 2022-12-09 11:46:59.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2856 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      825 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.406602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/service/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    22343 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      580 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.414602 nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4196 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      527 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-01 15:28:33.262602 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-01 15:28:33.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1609 2023-02-01 15:28:33.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2023-02-01 15:28:33.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      113 2023-02-01 15:28:33.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       13 2023-02-01 15:28:33.000000 nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/PKG-INFO
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      130 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/README.md
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/pyproject.toml
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      888 2023-02-15 09:59:06.381179 nsj_rest_lib-0.1.9/setup.cfg
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.197179 nsj_rest_lib-0.1.9/src/
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.229179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.289179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       75 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3985 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      944 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4555 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5359 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4886 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5199 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4921 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.301179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    17853 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1223 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.313179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3987 2023-02-01 14:54:52.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.337179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     8871 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7563 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5408 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      195 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2295 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.349179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7218 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.357179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      544 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      322 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      483 2022-12-09 11:46:59.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2856 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      825 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.369179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    22894 2023-02-15 09:54:51.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      580 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4196 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      527 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.253179 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1609 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      113 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       13 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-0.1.8/PKG-INFO` & `nsj_rest_lib-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.1.8/setup.cfg` & `nsj_rest_lib-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 0.1.8
+version = 0.1.9
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/service_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,21 +461,26 @@
 
                 relation_filter = {
                     list_field.related_entity_field: [relation_condiction]
                 }
 
                 # Recuperando do BD
                 old_detail_ids = detail_dao.list_ids(relation_filter)
+            
+            # Lista de DTOs detalhes a criar ou atualizar
+            detail_upsert_list = []
 
             # Salvando cada DTO detalhe
             for detail_dto in detail_list:
 
                 # Recuperando o ID da entidade relacionada
                 detail_pk_field = detail_dto.__class__.pk_field
                 detail_pk = getattr(detail_dto, detail_pk_field)
+                if isinstance(detail_pk, uuid.UUID):
+                    detail_pk = str(detail_pk)
 
                 # Verificando se é um update ou insert
                 is_detail_insert = True
                 if old_detail_ids is not None and detail_pk in old_detail_ids:
                     is_detail_insert = False
                     old_detail_ids.remove(detail_pk)
 
@@ -484,27 +489,35 @@
                     raise DTOListFieldConfigException(
                         f"PK field not found in class: {self._dto_class}")
 
                 if not (self._dto_class.pk_field in dto.__dict__):
                     raise DTOListFieldConfigException(
                         f"PK field not found in DTO: {self._dto_class}")
 
-                # Salvando o dto dependende (detalhe)
-                respose_detail_dto = detail_service._save(
-                    is_detail_insert, detail_dto, False, partial_update, relation_field_map, detail_pk)
-
-                # Guardando o DTO na lista de retorno
-                response_list.append(respose_detail_dto)
+                # Salvando o dto dependende (detalhe) na lista
+                detail_upsert_list.append({
+                    'is_detail_insert': is_detail_insert,
+                    'detail_dto': detail_dto,
+                    'detail_pk': detail_pk
+                })
 
             # Verificando se sobraram relacionamentos anteriores para remover
             if not partial_update and old_detail_ids is not None and len(old_detail_ids) > 0:
 
                 for old_id in old_detail_ids:
                     # Apagando cada relacionamento removido
-                    detail_service.delete(old_id, aditional_filters)
+                    detail_service.delete(old_id, **aditional_filters)
+            
+            # Salvando cada DTO detalhe
+            for item in detail_upsert_list:
+                response_detail_dto = detail_service._save(
+                    item["is_detail_insert"], item["detail_dto"], False, partial_update, relation_field_map, item["detail_pk"])
+
+                # Guardando o DTO na lista de retorno
+                response_list.append(response_detail_dto)
 
             # Setting dto property
             if response_dto is not None and master_dto_field in response_dto.list_fields_map and list_field.dto_post_response_type is not None:
                 setattr(response_dto, master_dto_field, response_list)
 
     def delete(
         self,
```

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.1.8/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

