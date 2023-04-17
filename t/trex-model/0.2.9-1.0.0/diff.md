# Comparing `tmp/trex-model-0.2.9.tar.gz` & `tmp/trex-model-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-0.2.9.tar", last modified: Mon Feb 13 06:21:53 2023, max compression
+gzip compressed data, was "trex-model-1.0.0.tar", last modified: Mon Apr 17 03:29:44 2023, max compression
```

## Comparing `trex-model-0.2.9.tar` & `trex-model-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.669288 trex-model-0.2.9/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-0.2.9/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-0.2.9/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-02-13 06:21:53.669438 trex-model-0.2.9/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-0.2.9/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-02-13 06:21:53.670018 trex-model-0.2.9/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-02-13 06:19:24.000000 trex-model-0.2.9/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.630526 trex-model-0.2.9/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.632822 trex-model-0.2.9/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-0.2.9/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-0.2.9/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.635959 trex-model-0.2.9/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-0.2.9/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.664366 trex-model-0.2.9/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-0.2.9/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-0.2.9/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2978 2022-09-23 06:10:25.000000 trex-model-0.2.9/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-0.2.9/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13794 2023-02-01 14:24:54.000000 trex-model-0.2.9/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    18975 2023-01-18 15:57:20.000000 trex-model-0.2.9/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-0.2.9/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-0.2.9/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5815 2022-12-30 07:12:43.000000 trex-model-0.2.9/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9846 2021-04-16 08:20:02.000000 trex-model-0.2.9/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    55368 2023-01-31 03:16:23.000000 trex-model-0.2.9/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-0.2.9/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-0.2.9/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-0.2.9/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    18586 2023-02-11 04:49:58.000000 trex-model-0.2.9/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38931 2022-09-23 07:11:28.000000 trex-model-0.2.9/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    46571 2022-03-11 05:24:52.000000 trex-model-0.2.9/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24359 2023-02-10 09:00:56.000000 trex-model-0.2.9/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    29487 2023-02-08 09:23:02.000000 trex-model-0.2.9/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-0.2.9/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-0.2.9/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-0.2.9/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-0.2.9/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    25826 2023-02-12 05:38:38.000000 trex-model-0.2.9/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-0.2.9/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-0.2.9/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6173 2023-02-07 02:42:49.000000 trex-model-0.2.9/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-0.2.9/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-0.2.9/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-0.2.9/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16152 2023-01-27 07:27:16.000000 trex-model-0.2.9/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.666310 trex-model-0.2.9/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.666924 trex-model-0.2.9/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.668277 trex-model-0.2.9/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-0.2.9/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.462242 trex-model-1.0.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.0/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.0/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-17 03:29:44.462462 trex-model-1.0.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-17 03:29:44.463124 trex-model-1.0.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-04-17 03:26:40.000000 trex-model-1.0.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.430424 trex-model-1.0.0/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.432308 trex-model-1.0.0/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.0/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.0/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.434164 trex-model-1.0.0/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.0/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.456400 trex-model-1.0.0/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.0/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.0/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.0/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.0/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.0/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47628 2023-04-13 05:33:49.000000 trex-model-1.0.0/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.0/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.0/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5816 2023-03-02 14:42:44.000000 trex-model-1.0.0/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.0/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    57095 2023-04-13 02:21:06.000000 trex-model-1.0.0/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.0/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.0/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-1.0.0/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.0/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.0/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.0/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.0/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.0/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.0/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.0/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.0/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.0/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    33133 2023-04-11 02:45:33.000000 trex-model-1.0.0/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.0/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.0/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.0/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.0/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.0/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.0/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.0/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.458294 trex-model-1.0.0/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.459091 trex-model-1.0.0/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.461629 trex-model-1.0.0/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.0/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-0.2.9/LICENSE` & `trex-model-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/setup.py` & `trex-model-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='0.2.9',
+     version='1.0.0',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-0.2.9/trex_model.egg-info/SOURCES.txt` & `trex-model-1.0.0/trex_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/conf.py` & `trex-model-1.0.0/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/admin_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/analytic_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 @author: jacklok
 '''
 from trexmodel import conf as model_conf
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from datetime import timedelta
+from trexmodel.models.datastore.merchant_models import MerchantAcct
 
 class UpstreamData(BaseNModel, DictModel):
+    merchant_acct           = ndb.KeyProperty(name="merchant_acct", kind=MerchantAcct)
     table_template_name     = ndb.StringProperty(required=True)
     dataset_name            = ndb.StringProperty(required=True)
     table_name              = ndb.StringProperty(required=True)
     stream_content          = ndb.JsonProperty(required=True)
     is_sent                 = ndb.BooleanProperty(required=True, default=False)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     
@@ -47,16 +49,17 @@
         
         return UpstreamData.query(ndb.AND(
                                     UpstreamData.created_datetime>=datetime_start,
                                     UpstreamData.created_datetime<datetime_end,
                                 )).count(limit = limit)
     
     @staticmethod
-    def create(dataset_name, table_name, table_template_name, stream_content):
+    def create(merchant_acct, dataset_name, table_name, table_template_name, stream_content):
         UpstreamData(
+                    merchant_acct       = merchant_acct.create_ndb_key(), 
                     table_template_name = table_template_name,
                     dataset_name        = dataset_name,
                     table_name          = table_name,
                     stream_content      = stream_content,
                     ).put()
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.0.0/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             existing_latest_expiry_date = reward_summary_by_reward_format.get('latest_expiry_date')
             existing_latest_expiry_date = datetime.strptime(existing_latest_expiry_date, '%d-%m-%Y').date()
             
             final_reward_amount                         = reward_summary_by_reward_format['amount'] - reward_amount
             reward_summary_by_reward_format['amount']   = final_reward_amount
             reward_summary[reward_format]               = reward_summary_by_reward_format
             
-            if final_reward_amount==0:
+            if final_reward_amount<=0:
                 del reward_summary[reward_format]
         
     return reward_summary
 
 ''' --------------- End: Update reward summary for point and stamp--------------'''
 
 '''
@@ -242,43 +242,38 @@
 ''' --------------- End: Update reward summary for voucher--------------'''
 
 ''' --------------- Start: Update reward summary for prepaid--------------'''
 
 def update_prepaid_summary_with_new_prepaid(existing_prepaid_summary, new_prepaid_summary):
     prepaid_amount              = new_prepaid_summary.get('amount')
     used_prepaid_amount         = new_prepaid_summary.get('used_amount')
+    prepaid_balance             = prepaid_amount - used_prepaid_amount
     
-    if is_empty(existing_prepaid_summary):
-        prepaid_balance         = prepaid_amount - used_prepaid_amount
-        existing_prepaid_summary = {
-                                    'amount'  : prepaid_balance,
-                                    }
-        
-    else:
-        prepaid_balance = existing_prepaid_summary.get('amount') + (prepaid_amount-used_prepaid_amount)
-        existing_prepaid_summary = {
-                                    'amount'  : prepaid_balance,
-                                    }        
+    if is_not_empty(existing_prepaid_summary):
+        prepaid_balance = existing_prepaid_summary.get('amount') + prepaid_balance
                 
+    existing_prepaid_summary = {
+                                    'amount'  : prepaid_balance,
+                                    }            
     return existing_prepaid_summary
 
 def update_prepaid_summary_with_reverted_prepaid(existing_prepaid_summary, reverted_prepaid_summary):
     prepaid_amount              = reverted_prepaid_summary.get('amount')
-    used_prepaid_amount         = reverted_prepaid_summary.get('used_amount')
+    
     
     if is_empty(existing_prepaid_summary):
         existing_prepaid_summary = {
-                                    'amount'  : .0,
+                                    'amount'  : prepaid_amount,
                                     }
         
     else:
-        prepaid_balance = existing_prepaid_summary.get('amount') - (prepaid_amount-used_prepaid_amount)
+        prepaid_balance = existing_prepaid_summary.get('amount') - prepaid_amount
         if prepaid_balance<0:
             prepaid_balance = .0
-        
+            
         existing_prepaid_summary = {
                                     'amount'  : prepaid_balance,
                                     }        
                 
     return existing_prepaid_summary
 
 ''' --------------- End: Update reward summary for prepaid--------------'''
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/customer_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/ndb_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,400 +1,460 @@
 '''
-Created on 5 Jan 2021
+Created on 13 Apr 2020
 
 @author: jacklok
 '''
 from google.cloud import ndb
-from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel, FullTextSearchable
-from trexmodel.models.datastore.user_models import User
-from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
-import trexmodel.conf as model_conf
-from trexlib.utils.string_util import is_not_empty, is_empty
+from trexlib.utils.common.float_util import format_float
+from datetime import datetime, date, time
+from trexlib.utils.string_util import is_not_empty 
+from trexlib.utils.log_util import get_tracelog
+from six import string_types 
+from trexlib.utils.common.date_util import increase_date 
 import logging
-from trexlib.utils.common.cache_util import cache
-from trexlib.utils.common.date_util import convert_date_to_datetime,\
-    to_day_of_year
-from trexmodel import conf
-from six import string_types
-from datetime import datetime, timedelta
-from trexmodel.models.datastore.customer_model_helpers import update_reward_summary_with_new_reward
-from trexmodel.models.datastore.membership_models import MerchantTierMembership
+#from google.cloud.ndb._datastore_query import Cursor
+from google.cloud.ndb import Cursor
+from trexlib import conf as lib_conf 
+from trexmodel import conf as model_conf
+from google.cloud.datastore.helpers import GeoPoint
+ 
+logger = logging.getLogger('model') 
 
-logger = logging.getLogger('model')
+def convert_to_serializable_value(val, none_as_empty_string=False, gmt=0, 
+                                  datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
+                                  date_format=lib_conf.DEFAULT_DATE_FORMAT, 
+                                  time_format=lib_conf.DEFAULT_TIME_FORMAT,
+                                  excluded_dict_properties=None
+                                  ):
+    
+    if isinstance(val, (list, tuple)):
+        _list = []
+        for item in val:
+            _list.append(convert_to_serializable_value(item, excluded_dict_properties=excluded_dict_properties))
+        value = _list
+    elif isinstance(val, float):
+        value = format_float(val)
+    elif isinstance(val, (dict, int, bool)):
+        #logger.debug('>>>>found dict, int, float, bool value=%s', val)
+        value = val
+    elif isinstance(val, datetime):
+        gmt_datetime = increase_date(val, hour=gmt)
+        value = gmt_datetime.strftime(datetime_format)
+    elif isinstance(val, date):
+        value = val.strftime(date_format)
+    elif isinstance(val, time):
+        #gmt_datetime = increase_date(val, hours=gmt)
+        value = val.strftime(time_format)
+    elif isinstance(val, GeoPoint):
+        value = '%s,%s' % (val.latitude, val.longitude)    
+    else:
+        if none_as_empty_string:
+            if val:
+                value = str(val)
+            else:
+                value = ''
+        else:
+            if val is None:
+                value = None
+            else:
+                value = str(val)
+    #logger.debug('convert_to_serializable_value: value=%s', value)
+    return value
 
+def render_dict_value(val, full=False, show_key=True, gmt=0, 
+                      datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
+                      date_format=lib_conf.DEFAULT_DATE_FORMAT, 
+                      time_format=lib_conf.DEFAULT_TIME_FORMAT,
+                      excluded_dict_properties=None,
+                      ):
+    #logger.debug('---render_dict_value---')
+    value = None
+    if isinstance(val, DictModel):
+        value = val.to_dict(full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties)
 
-class Customer(BaseNModel, DictModel, FullTextSearchable):
-    '''
-    parent is User
-    '''
-    
-    merchant_acct               = ndb.KeyProperty(name="merchant_acct", kind=MerchantAcct)
-    outlet                      = ndb.KeyProperty(name="outlet", kind=Outlet)
-    merchant_reference_code     = ndb.StringProperty(name="merchant_reference_code", required=False)
-    registered_datetime         = ndb.DateTimeProperty(required=False, auto_now_add=True)
-    modified_datetime           = ndb.DateTimeProperty(required=False, auto_now=True)
-    
-    #---------------------------------------------------------------------------
-    # User denormalize fields
-    #---------------------------------------------------------------------------
-    name                        = ndb.StringProperty(required=False)
-    mobile_phone                = ndb.StringProperty(required=False)
-    email                       = ndb.StringProperty(required=False)
-    
-    birth_date                  = ndb.DateProperty(required=False, indexed=False)
-    birth_date_date_str         = ndb.StringProperty(required=False) 
-    birth_day_in_year           = ndb.IntegerProperty(required=False)
-    gender                      = ndb.StringProperty(required=False)
-    reference_code              = ndb.StringProperty(required=True)
-    
-    mobile_app_installed        = ndb.BooleanProperty(required=False, default=False)
-    
-    tags_list                   = ndb.StringProperty(repeated=True, write_empty_list=True)
-    
-    memberships_list            = ndb.StringProperty(repeated=True, write_empty_list=True)
-    
-    last_transact_datetime      = ndb.DateTimeProperty(required=False)
-    previous_transact_datetime  = ndb.DateTimeProperty(required=False)
-    
-    last_redeemed_datetime      = ndb.DateTimeProperty(required=False)
-    
-    tier_membership             = ndb.KeyProperty(name="tier_membership", kind=MerchantTierMembership)
-    previous_tier_membership    = ndb.KeyProperty(name="previous_tier_membership", kind=MerchantTierMembership)
-    
-    reward_summary                      = ndb.JsonProperty()
-    prepaid_summary                     = ndb.JsonProperty()
-    entitled_voucher_summary            = ndb.JsonProperty()
-    entitled_birthday_reward_summary    = ndb.JsonProperty()
-    
-    kpi_summary                         = ndb.JsonProperty()
-    
-    fulltextsearch_field_name           = 'name'
-    
-    dict_properties     = ['name', 'mobile_phone', 'email', 'gender', 'birth_date', 'reference_code', 'merchant_reference_code',  
-                           'tags_list', 'memberships_list', 'registered_merchant_acct', 
-                           'reward_summary', 'entitled_voucher_summary', 'prepaid_summary', 'kpi_summary', 'entitled_birthday_reward_summary',
-                           'registered_outlet_key', 'registered_merchant_acct_key', 'registered_datetime', 'modified_datetime']
-    
-    @property
-    def registered_user_acct_key(self):
-        return self.key.parent().urlsafe().decode('utf-8')
-    
-    @property
-    def registered_user_acct(self):
-        return User.fetch(self.key.parent().urlsafe())
-    
-    @property
-    def registered_merchant_acct(self):
-        return MerchantAcct.fetch(self.merchant_acct.urlsafe())
+    elif isinstance(val, ndb.Model):
+        value = val.key.urlsafe()
+
+    elif isinstance(val, (list, tuple)):
+        _list = []
+        for item in val:
+            _list.append(render_dict_value(item, full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties))
+        value = _list
+
+    elif isinstance(val, DictObject):
+        value = val.to_dict(gmt=gmt, excluded_dict_properties=excluded_dict_properties)
+    else:
+        value = convert_to_serializable_value(val, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties)
+    return value
+
+class DictObject(object):
+    dict_properties = None
     
-    @property
-    def registered_merchant_acct_key(self):
-        if self.merchant_acct:
-            return self.merchant_acct.urlsafe().decode("utf-8")
+    def get_class_members(self, klass):
+        ret = dir(klass)
+        if hasattr(klass,'__bases__'):
+            for base in klass.__bases__:
+                ret = ret + self.get_class_members(base)
+        return ret
     
-    @property
-    def registered_outlet(self):
-        if self.outlet:
-            return Outlet.fetch(self.outlet.urlsafe())
+    def uniq(self, seq ): 
+        return list(set(seq))
     
-    @property
-    def registered_outlet_key(self):
-        if self.outlet:
-            return self.outlet.urlsafe().decode("utf-8")
-    
-    @property
-    def tier_membership_key(self):
-        if self.tier_membership:
-            return self.tier_membership.urlsafe().decode("utf-8")
-        
-    @staticmethod    
-    def update_KPI(customer_acct, tags_list=None, memberships_list=None, tier_membership_key=None):
-        if isinstance(tags_list, string_types):
-            if is_not_empty(tags_list):
-                tags_list = tags_list.split(',')
-            else:
-                tags_list = []
-                
-        if isinstance(memberships_list, string_types):
-            if is_not_empty(memberships_list):
-                memberships_list = memberships_list.split(',')
-            else:
-                memberships_list = []
+    def properties(self):
+        return self.__dict__
+
+    def to_dict(self, full=True, show_key=True, dict_properties=None, excluded_dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
+                        datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
+                        date_format=lib_conf.DEFAULT_DATE_FORMAT, 
+                        time_format=lib_conf.DEFAULT_TIME_FORMAT):
+        logger.info('calling DictObject.to_dict')
+        result = {}
+        #logger.debug('properties = %s, object = %s', self.properties(), self)
+
+        _dict_properties = dict_properties or self.dict_properties
+
+        if _dict_properties:
+            for p in _dict_properties:
+
+                val = getattr(self, p)
+                if val is not None:
+                    #logger.debug('attribute=%s', p)
+                    result[p] = render_dict_value(val, full=full, show_key=show_key, gmt=gmt, 
+                                                  datetime_format=datetime_format, 
+                                                  date_format=datetime_format, 
+                                                  time_format=time_format,
+                                                  excluded_dict_properties=excluded_dict_properties,
+                                                  )
+        return result
+    
+class DictModel(ndb.Model):
+    
+    dict_properties             = None
+    dict_full_properties        = None
+    show_key_in_dict            = True
+
+    def __get_attr_value(self, obj, attr_name):
+        val = getattr(obj, attr_name)
+        if isinstance(val, GeoPoint):
+            return '%s,%s' % (val.latitude, val.longitude)
         
-        tier_membership = None
+        return val
+
+    def put(self, **kwargs):
+        super(DictModel, self).put(**kwargs)
+
+    def to_dict(self, full=False, show_key=True, dict_properties=None, excluded_dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
+                        datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
+                        date_format=lib_conf.DEFAULT_DATE_FORMAT, 
+                        time_format=lib_conf.DEFAULT_TIME_FORMAT):
+        result = {}
+        logger.debug('DictModel: full=%s', full)
+        logger.debug('DictModel: show_key=%s', show_key)
+        
+        #if self.show_key_in_dict or show_key:
+        if show_key:
+            try:
+                result['key'] = self.key.urlsafe().decode("utf-8")
+            except:
+                pass 
         
-        if tier_membership_key:
-            tier_membership = MerchantTierMembership.fetch(tier_membership_key)        
+        _dict_properties = dict_properties or self.dict_properties
+
+        if full and self.dict_full_properties:
+            _dict_properties = self.dict_full_properties
+
+        if _dict_properties:
+            for p in _dict_properties:
+                if excluded_dict_properties is not None:
+                    if p in excluded_dict_properties:
+                        continue
+                    
+                if p=='key':
+                    if result.get('key'):
+                        continue
+                    
+                _p = p.split('.')
+
+                if len(_p)>1:
+                    ref_array   = _p[:-1]
+                    ref_obj     = self
+                    for _a in ref_array:
+                        ref_obj = self.__get_attr_value(ref_obj, _a)
+
+                    if ref_obj:
+                        ref_value = self.__get_attr_value(ref_obj, _p[-1])
+                else:
+                    ref_value = self.__get_attr_value(self, p)
+
+                if is_not_empty(ref_value):
+                #if ref_value:
+                    p = p.replace('.', '_')
+                    result[p] = render_dict_value(ref_value, full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format)
+                                        
+        #logger.debug('DictModel: result=%s', result)
         
-        customer_acct.tags_list         = tags_list
-        customer_acct.memberships_list  = memberships_list
-        customer_acct.tier_membership   = tier_membership
-        customer_acct.put()
-    
+        return result    
+
+class NDBModel(object):
     @classmethod
-    def get_by_reference_code(cls, reference_code, merchant_acct):
-        return cls.query(ndb.AND(cls.reference_code==reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
+    def get_by_ndb_id(cls, ndb_id):
+        if isinstance(ndb_id, string_types):
+            return cls.get_by_key_name(ndb_id)
+        else:
+            return cls.get_by_id(ndb_id)
+
+    def ndb_id(self):
+        return self.key().id()
+
+    def create_ndb_key(self):
+        return ndb.Key(flat=self.key.flat())
     
+class BaseNModel(DictModel, NDBModel):
+
+    saved = False
+
+    def is_saved(self):
+        return self.saved
+
     @classmethod
-    def get_by_merchant_reference_code(cls, merchant_reference_code, merchant_acct):
-        return cls.query(ndb.AND(cls.merchant_reference_code==merchant_reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
+    def _post_get_hook(cls, key, future):
+        obj = future.get_result()
+        if obj is not None:
+            # test needed because post_get_hook is called even if get() fails!
+            obj.saved = True
+
+    def _post_put_hook(self, future):
+        self.saved = True
+        
+    @property
+    def parent_key(self):
+        return self.key.parent().urlsafe().decode('utf-8')
+
+    @property
+    def key_in_str(self):
+        return self.key.urlsafe().decode('utf-8')
+
+    @property
+    def key_name(self):
+        return self.key.id()
+
+    def equal(self, another_instance):
+        if another_instance:
+            return self.key_in_str == another_instance.key_in_str
+        else:
+            return False
+
+    def not_equal(self, another_instance):
+        if another_instance:
+            return self.key_in_str != another_instance.key_in_str
+        else:
+            return True
     
-    @classmethod
-    def get_by_email(cls, email):
-        return cls.query(cls.email==email).get()
+    def delete(self):
+        self.key.delete()
     
     @classmethod
-    def get_by_mobile_phone(cls, mobile_phone):
-        return cls.query(cls.mobile_phone==mobile_phone).get()
+    def fetch(cls, model_key):
+        try:
+            if model_key:
+                return ndb.Key(urlsafe=model_key).get()
+
+        except:
+            logger.error('Failed to fetch entity due to %s', get_tracelog())
+
+        return None
     
     @classmethod
-    def create(cls, outlet=None, name=None, email=None, mobile_phone=None, merchant_reference_code=None, gender=None, birth_date=None,
-               password=None):
+    def count(cls, limit=model_conf.MAX_FETCH_RECORD): 
+        query = cls.query()
         
-        created_user = User.create(name=name, email=email, mobile_phone=mobile_phone, gender=gender, birth_date=birth_date, 
-                           password=password)
+        return cls.count_with_condition_query(query, limit=limit)
+    
+    @classmethod
+    def count_with_condition_query(cls, query, limit=model_conf.MAX_FETCH_RECORD):    
         
-        created_user.put()
-        created_customer = cls.create_from_user(outlet, created_user)
-        created_customer.merchant_reference_code = merchant_reference_code
-        created_customer.put()
         
-        return created_customer
+        return query.count(limit=limit, keys_only=True)
     
     @classmethod
-    def update(cls, customer=None, outlet=None, **kwargs):
-        if outlet:
-            customer.outlet = outlet.create_ndb_key()
+    def list_all(cls, offset=0,  start_cursor=None, return_with_cursor=False, keys_only=False, 
+                 limit=model_conf.MAX_FETCH_RECORD):
         
-        logger.debug('**kwargs=%s', kwargs)
+        query = cls.query()
         
-        mobile_phone    = kwargs.get('mobile_phone')
+        return cls.list_all_with_condition_query(query, 
+                                                 offset=offset, start_cursor=start_cursor,
+                                                 return_with_cursor = return_with_cursor,
+                                                 keys_only = keys_only, limit=limit
+                                                 )
+    
+    @classmethod
+    def list_all_with_condition_query(cls, query, offset=0,  start_cursor=None, return_with_cursor=False, keys_only=False, 
+                 limit=model_conf.MAX_FETCH_RECORD):
         
-        if mobile_phone:
-            mobile_phone = mobile_phone.replace(" ", "")
         
-        kwargs['mobile_phone'] = mobile_phone
         
-        for key, value in kwargs.items():
-            setattr(customer, key, value)
+        if start_cursor or return_with_cursor:
+            if is_not_empty(start_cursor):
+                if isinstance(start_cursor, string_types):
+                    start_cursor = ndb.Cursor(urlsafe = start_cursor) if start_cursor else ndb.Cursor()
+            else:
+                start_cursor = ndb.Cursor()
             
-        user_acct = customer.registered_user_acct
-        
-        User.update(user_acct=user_acct, **kwargs)
-        '''
-        user_acct.name                   = customer.name
-        user_acct.email                  = customer.email
-        user_acct.mobile_phone           = customer.mobile_phone
-        user_acct.birth_date             = customer.birth_date
-        user_acct.birth_date_date_str    = customer.birth_date_date_str
-        user_acct.gender                 = customer.gender
-        
-        user_acct.put()
-        '''
-        customer.put()
-        
-    @classmethod
-    def create_from_user(cls, outlet, user_acct, merchant_reference_code=None):
-        merchant_acct       = outlet.merchant_acct_entity
-        created_customer    = cls(parent=user_acct.create_ndb_key(), 
-                               outlet                   = outlet.create_ndb_key(), 
-                               name                     = user_acct.name, 
-                               email                    = user_acct.email, 
-                               mobile_phone             = user_acct.mobile_phone, 
-                               gender                   = user_acct.gender, 
-                               reference_code           = user_acct.reference_code, 
-                               birth_date               = user_acct.birth_date, 
-                               birth_date_date_str      = user_acct.birth_date_date_str, 
-                               birth_day_in_year        = user_acct.birth_day_in_year,
-                               merchant_reference_code  = merchant_reference_code,
-                               merchant_acct            = merchant_acct.create_ndb_key()
-                           )
-        
-        created_customer.put()
+            (search_results, next_cursor, more)       = query.fetch_page(page_size=limit, start_cursor=start_cursor, keys_only=keys_only)
+            logger.debug('##########################################')
+            
+            logger.debug('list_all: results=%s', search_results)
+            logger.debug('list_all: next_cursor=%s', next_cursor)
+            logger.debug('list_all: more=%s', more) 
+            
+            logger.debug('##########################################')
+            
+            if more:
+                return search_results, next_cursor.to_websafe_string().decode('utf-8')  
+            else:    
+                return search_results, 'None'
+            
+        else:
+            search_results = query.fetch(limit=limit, offset=offset)
+            
+            return search_results
         
-        return created_customer
+    def before_put(self):
+        pass
     
-    @classmethod
-    def list_merchant_customer_by_date_of_birth(cls, merchant_acct, date_of_birth, offset=0, limit=conf.MAX_FETCH_RECORD, start_cursor=None, return_with_cursor=False, keys_only=False):
-        query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key(), cls.birth_date_date_str==date_of_birth))
-        
-        return cls.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor, keys_only=keys_only)
+    def after_put(self):
+        pass
     
-    @classmethod
-    def list_merchant_customer_by_date_of_birth_thru_date_range(cls, merchant_acct, date_range_start=None, date_range_end=None, offset=0, limit=conf.MAX_FETCH_RECORD, start_cursor=None, return_with_cursor=False, keys_only=False):
-        date_range_start_day_in_year    = to_day_of_year(date_range_start)
-        date_range_end_day_in_year      = to_day_of_year(date_range_end)
+    def put(self, **kwargs):
+        self.before_put()
+        super(BaseNModel, self).put(**kwargs)
+        self.after_put()
+    
+    
+class FullTextSearchable(ndb.Model):
+    full_text_search_field      = ndb.StringProperty(repeated=True)
+    
+    fulltextsearch_field_name   = None
+    
+    def _pre_put_hook(self):
+        """before save, parse searchable field into strings"""
         
-        query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key(), cls.birth_day_in_year>=date_range_start_day_in_year, cls.birth_day_in_year<=date_range_end_day_in_year))
         
-        return cls.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor, keys_only=keys_only)
-    
-    @classmethod
-    def count_merchant_customer_by_date_of_birth(cls, merchant_acct, date_of_birth, limit=conf.MAX_FETCH_RECORD):
-        query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key(), cls.birth_date_date_str==date_of_birth))
         
-        return cls.count_with_condition_query(query, limit=limit)
-    
-    @classmethod
-    def list_merchant_customer(cls, merchant_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
-        query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key()))
+        _searchable_field_name = self.fulltextsearch_field_name
         
-        return cls.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+        logger.debug('_searchable_field_name=%s', _searchable_field_name)
+        if _searchable_field_name:
+            searchable_field_value = getattr(self, _searchable_field_name)
+            logger.debug('searchable_field_value=%s', searchable_field_value)
+            if is_not_empty(searchable_field_value):
+                splitted_words = searchable_field_value.lower().split(' ')
+                
+                logger.debug('splitted_words=%s', splitted_words)
+                
+                searchable_words_list = [x for x in splitted_words if x and len(x) >= 2]
+                logger.debug('searchable_words_list=%s', searchable_words_list)
+                
+                self.full_text_search_field = searchable_words_list
     
-    @classmethod
-    def list_by_user_account(cls, user_acct):
-        return cls.query(ancestor=user_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
     
-    @classmethod
-    def count_merchant_customer(cls, merchant_acct):
-        if merchant_acct:
-            query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key()))
-        else:
-            query = cls.query()
-        
-        return cls.count_with_condition_query(query)
     
     @classmethod
-    def search_merchant_customer(cls, merchant_acct, name=None, email=None, mobile_phone=None, 
-                                 reference_code=None, merchant_reference_code=None, merchant_tagging=None,
-                                 registered_date_start=None, registered_date_end=None,
-                                 offset=0, start_cursor=None, limit=model_conf.MAX_FETCH_RECORD):
+    def full_text_count(cls, search_text_list, query=None, limit=model_conf.MAX_FETCH_RECORD_FULL_TEXT_SEARCH_PER_PAGE):
         
-        search_text_list = None
-        query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key()))
+        logger.debug('full_text_count: search_text_list=%s', search_text_list)
         
-        if is_not_empty(email):
-            query = query.filter(cls.email==email)
-            
-        elif is_not_empty(mobile_phone):
-            query = query.filter(cls.mobile_phone==mobile_phone)
-            
-        elif is_not_empty(reference_code):
-            query = query.filter(cls.reference_code==reference_code)
-            
-        elif is_not_empty(merchant_reference_code):
-            query = query.filter(cls.merchant_reference_code==merchant_reference_code)
-                    
-        elif is_not_empty(merchant_tagging):
-            query = query.filter(cls.tags_list==merchant_tagging)
+        lowercase_words_list = []
         
-        elif is_not_empty(name):
-            search_text_list = name.split(' ')
+        if is_not_empty(search_text_list):
+            lowercase_words_list = [x.lower() for x in search_text_list]
         
-        elif is_not_empty(registered_date_start) or is_not_empty(registered_date_end):
+            logger.debug('full_text_search: lowercase_words_list=%s', lowercase_words_list)
             
-            if is_not_empty(registered_date_start):
-                registered_datetime_start = convert_date_to_datetime(registered_date_start)
-                
-                query = query.filter(cls.registered_datetime>=registered_datetime_start)
-            
-            if is_not_empty(registered_date_end):
-                registered_datetime_end = convert_date_to_datetime(registered_date_end)
+        if query is None:
+            query = cls.query()
             
-                query = query.filter(cls.registered_datetime<registered_datetime_end)
-        
-        total_count                         = cls.full_text_count(search_text_list, query, conf.MAX_FETCH_RECORD_FULL_TEXT_SEARCH)
-        
-        (search_results, next_cursor)       = cls.full_text_search(search_text_list, query, offset=offset, 
-                                                                   start_cursor=start_cursor, return_with_cursor=True, 
-                                                                   limit=limit)
-        
-        return (search_results, total_count, next_cursor)
-    
-    def update_from_user_acct(self, user_acct):
-        
-        self.name                   = user_acct.name
-        self.email                  = user_acct.email
-        self.mobile_phone           = user_acct.mobile_phone
-        self.birth_date             = user_acct.birth_date
-        self.birth_date_date_str    = user_acct.birth_date_date_str
-        self.birth_day_in_year      = user_acct.birth_day_in_year
-        self.gender                 = user_acct.gender
-        self.put()
-    
-    @staticmethod
-    def count_by_last_transact_date(merchant_acct, last_transact_in_day=7):
-        checking_date = datetime.now().date() - timedelta(days=last_transact_in_day)
-        
-        logger.debug('count_by_last_transact_date: checking_date=%s', checking_date)
         
-        query = Customer.query(ndb.AND(
-                                                    Customer.merchant_acct==merchant_acct.create_ndb_key(),
-                                                    Customer.last_transact_date >= checking_date   
-                                        ))
-        
-        return Customer.count_with_condition_query(query)
-    
-    @staticmethod
-    def update_customer_entitled_birthday_reward_summary(customer_acct, merchant_program_key, transact_datetime=None):
+        for word in lowercase_words_list:
+            query = query.filter(cls.full_text_search_field == word)
+            
+        logger.debug('query=%s', query)
         
-        logger.debug('---update_customer_entitled_birthday_reward_summary---')
+        return query.count(limit=limit, keys_only=True)
+            
+           
         
-        if transact_datetime is None:
-            today       = datetime.today().date()
-            this_year   = today.year
-        else:
-            today       = transact_datetime.date()
-            this_year   = transact_datetime.year
+    @classmethod
+    def full_text_search(cls, text_search = None, query=None, offset=0,  start_cursor=None, return_with_cursor=False, keys_only=False, 
+                         limit=model_conf.MAX_FETCH_RECORD_FULL_TEXT_SEARCH_PER_PAGE):
+        if query is None:
+            query = cls.query()
         
-        year_str = str(this_year)
-        entitled_birthday_reward_summary            = customer_acct.entitled_birthday_reward_summary
-        this_year_entitled_birthday_reward_summary  = None    
+        logger.debug('##########################################')
+        logger.debug('full_text_search: text_search=%s', text_search)
+        logger.debug('full_text_search: query=%s', query)
+        logger.debug('full_text_search: start_cursor=%s', start_cursor)
+        logger.debug('full_text_search: offset=%s', offset)
+        logger.debug('full_text_search: return_with_cursor=%s', return_with_cursor)
         
-        if entitled_birthday_reward_summary:
-            this_year_entitled_birthday_reward_summary  = entitled_birthday_reward_summary.get(year_str)
-        else:
-            entitled_birthday_reward_summary = {}
+        logger.debug('##########################################')
         
-        if this_year_entitled_birthday_reward_summary is None:
-            this_year_entitled_birthday_reward_summary = {}
             
+        if is_not_empty(text_search):
+            lowercase_words_list = [x.lower() for x in text_search]
+            
+            logger.debug('full_text_search: lowercase_words_list=%s', lowercase_words_list)
+            
+            for word in lowercase_words_list:
+                query = query.filter(cls.full_text_search_field == word)
         
-        is_birthday_reward_has_been_given = False
-        if this_year_entitled_birthday_reward_summary.get('programs'):
-            if merchant_program_key in this_year_entitled_birthday_reward_summary.get('programs'):
-                is_birthday_reward_has_been_given = True
-                logger.debug('Found %s in programs list', merchant_program_key)
+        if start_cursor or return_with_cursor:
+            if is_not_empty(start_cursor):
+                if isinstance(start_cursor, string_types):
+                    start_cursor = ndb.Cursor(urlsafe = start_cursor) if start_cursor else ndb.Cursor()
+            #else:
+            #    start_cursor = ndb.Cursor()
+            '''
+            if is_not_empty(start_cursor):
+                if isinstance(start_cursor, string_types):
+                    start_cursor = Cursor.from_websafe_string(start_cursor)
             else:
-                logger.debug('going to add entitled program(%s)', merchant_program_key)
-                this_year_entitled_birthday_reward_summary['programs'].append(merchant_program_key)
-                is_birthday_reward_has_been_given = False
-                
+                start_cursor = None
+            '''
+            if is_not_empty(start_cursor):
+                logger.debug('start_cursor is empty or none')
+                (search_results, next_cursor, more)       = query.fetch_page(page_size=limit, 
+                                                                         start_cursor=start_cursor, 
+                                                                         keys_only=keys_only)
+            else:
+                (search_results, next_cursor, more)       = query.fetch_page(page_size=limit, offset=offset, 
+                                                                         keys_only=keys_only)
+            
+            logger.debug('==========================================')
+            logger.debug('full_text_search: query=%s', query)
+            logger.debug('full_text_search: offset=%s', offset)
+            logger.debug('full_text_search: search_results count =%s', len(search_results))
+            logger.debug('full_text_search: next_cursor=%s', next_cursor)
+            logger.debug('full_text_search: more=%s', more) 
+            
+            logger.debug('==========================================')
+            
+            if more:
+                return search_results, next_cursor.to_websafe_string().decode('utf-8')  
+            else:    
+                return search_results, 'None'
+            
         else:
-            this_year_entitled_birthday_reward_summary = {'programs': [merchant_program_key]}
-            is_birthday_reward_has_been_given = False
+            search_results = query.fetch(limit=limit, offset=offset)
             
-        if is_birthday_reward_has_been_given==False:
-            entitled_birthday_reward_summary[year_str]     = this_year_entitled_birthday_reward_summary
-            customer_acct.entitled_birthday_reward_summary  = entitled_birthday_reward_summary
-            customer_acct.put()
-                
+            logger.debug('==========================================')
+            logger.debug('full_text_search: query=%s', query)
+            logger.debug('full_text_search: offset=%s', offset)
+            logger.debug('full_text_search: search_results count =%s', len(search_results))
+            
+            logger.debug('==========================================')
+            
+            return search_results        
+            
+
     
-    @staticmethod
-    def check_birthday_reward_have_entitled_before(customer_acct, year, program_key):
-        entitled_birthday_reward_summary = customer_acct.entitled_birthday_reward_summary
-        year_str = str(year)
-        logger.info('entitled_birthday_reward_summary=%s', entitled_birthday_reward_summary)
-        
-        if is_not_empty(entitled_birthday_reward_summary):
-            if is_not_empty(entitled_birthday_reward_summary.get(year_str)):
-                this_year_entitled_birthday_programs_list = entitled_birthday_reward_summary.get(year_str).get('programs')
-                
-                logger.debug('this_year_entitled_birthday_programs_list=%s', this_year_entitled_birthday_programs_list)
-                is_entitled_before = False
-                if is_not_empty(this_year_entitled_birthday_programs_list):
-                    for k in this_year_entitled_birthday_programs_list:
-                        if k == program_key:
-                            is_entitled_before =  True
-                            break
-                    
-                    logger.debug('is_entitled_before=%s', is_entitled_before)
-                    return is_entitled_before
-                else:
-                    logger.debug('Program list is empty')
-            else:
-                logger.debug('Not found for year (%s)', year)
-        else:
-            logger.debug('entitled_birthday_reward_summary is empty')            
-        
-        return False
-
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.0.0/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/loyalty_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                         LoyaltyDeviceSetting.assigned_outlet==assigned_outlet.create_ndb_key()
                         ),ancestor=merchant_acct.create_ndb_key())
         
         return LoyaltyDeviceSetting.count_with_condition_query(query)
         
     def activate(self, device_id):
         self.device_id          = device_id
-        self.activated          = True
+        #self.activated          = True
         self.activated_datetime = datetime.utcnow()
         self.put()
         
         
     @staticmethod
     def remove_by_activation_code(activation_code):
         checking_device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/membership_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/membership_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 import trexmodel.conf as model_conf
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.merchant_models import MerchantAcct, \
-    MerchantUser
+    MerchantUser, Outlet
 import logging
+from dateutil.relativedelta import relativedelta
+from datetime import timedelta
 
 from datetime import datetime
+from trexmodel import program_conf
 
 logger = logging.getLogger('model')
 
 class MembershipBase(BaseNModel, DictModel):
     '''
     Merchant Acct as ancestor
     
@@ -46,76 +49,108 @@
     def merchant_acct(self):
         return MerchantAcct.fetch(self.key.parent().urlsafe())
     
     @classmethod
     def list_by_merchant_acct(cls, merchant_acct, is_archived=False):
         return cls.query(ndb.AND(MerchantMembership.archived == is_archived), ancestor=merchant_acct.create_ndb_key()).fetch(limit=model_conf.MAX_FETCH_RECORD)
     
-    @classmethod
-    def create(cls, merchant_acct, label, desc=None, expiration_type=None, expiration_value=None, 
+    
+    
+        
+    def calc_expiry_date(self, start_date=None):
+        
+        if start_date is None:
+            start_date = datetime.utcnow()
+        
+        logger.debug('start_date=%s', start_date)
+        logger.debug('self.expiration_type=%s', self.expiration_type)
+            
+        if self.expiration_type == program_conf.MEMBERSHIP_EXPIRATION_TYPE_AFTER_YEAR:
+            return start_date + relativedelta(years=self.expiration_value)
+         
+        elif self.expiration_type == program_conf.MEMBERSHIP_EXPIRATION_TYPE_AFTER_MONTH:
+            return start_date + relativedelta(months=self.expiration_value)
+        
+        elif self.expiration_type == program_conf.MEMBERSHIP_EXPIRATION_TYPE_AFTER_WEEK:
+            return start_date + relativedelta(weeks=self.expiration_value)
+        
+        elif self.expiration_type == program_conf.MEMBERSHIP_EXPIRATION_TYPE_AFTER_DAY:
+            return start_date + relativedelta(days=self.expiration_value)
+        
+        else:
+            #for no expiration
+            return datetime.max    
+
+class MerchantMembership(MembershipBase):
+    
+    
+    def to_configuration(self):
+        membership_configuration = {
+                                    'membership_key'                : self.key_in_str,
+                                    'label'                         : self.label,
+                                    'expiration_type'               : self.expiration_type,
+                                    'expiration_value'              : self.expiration_value,
+                                    }
+        
+        return membership_configuration
+    
+        
+    @staticmethod
+    def create(merchant_acct, label, desc=None, expiration_type=None, expiration_value=None, 
                created_by=None):
         
         created_by_username = None
         if is_not_empty(created_by):
             if isinstance(created_by, MerchantUser):
                 created_by_username = created_by.username
         
-        merchant_membership = cls(
+        merchant_membership = MerchantMembership(
                                                 parent                  = merchant_acct.create_ndb_key(),
                                                 label                   = label,
                                                 desc                    = desc,
                                                 expiration_type         = expiration_type,
                                                 expiration_value        = expiration_value,
                                                 created_by              = created_by.create_ndb_key(),
                                                 created_by_username     = created_by_username,
                                                 )
         
         merchant_membership.put()
         
+        merchant_acct.add_membership(merchant_membership.to_configuration())
+        
         return merchant_membership
     
-    @classmethod
-    def update(cls, merchant_membership, label, desc=None, expiration_type=None, expiration_value=None, 
+    @staticmethod
+    def update(merchant_membership, label, desc=None, expiration_type=None, expiration_value=None, 
                modified_by=None):
         modified_by_username = None
         if is_not_empty(modified_by):
             if isinstance(modified_by, MerchantUser):
                 modified_by_username = modified_by.username
         
         merchant_membership.label                   = label
         merchant_membership.desc                    = desc
         merchant_membership.expiration_type         = expiration_type
         merchant_membership.expiration_value        = expiration_value
         merchant_membership.modified_by             = modified_by.create_ndb_key()
         merchant_membership.modified_by_username    = modified_by_username
         
         merchant_membership.put()
-
-class MerchantMembership(MembershipBase):
-    
-    
-    def to_configuration(self):
-        membership_configuration = {
-                                    'membership_key'                : self.key_in_str,
-                                    'label'                         : self.label,
-                                    'expiration_type'               : self.expiration_type,
-                                    'expiration_value'              : self.expiration_value,
-                                    }
         
-        return membership_configuration
+        merchant_acct = merchant_membership.merchant_acct
+        merchant_acct.update_membership(merchant_membership.to_configuration())
     
-    @staticmethod
-    def archive_membership(membership):
+    @classmethod
+    def archive_membership(cls, membership):
         membership.archived = True
         membership.archived_datetime = datetime.now()
         membership.put()
         
         merchant_acct = membership.merchant_acct
         merchant_acct.remove_archieve_basic_membership(membership.key_in_str)    
-        
     
 
 
 class MerchantTierMembership(MembershipBase):        
     entitle_qualification_type          = ndb.StringProperty(required=True)
     entitle_qualification_value         = ndb.FloatProperty(required=False)
     upgrade_expiry_type                 = ndb.StringProperty(required=True)
@@ -203,8 +238,10 @@
     def archive_membership(membership):
         membership.archived = True
         membership.archived_datetime = datetime.now()
         membership.put()
         
         merchant_acct = membership.merchant_acct
         merchant_acct.remove_archieve_tier_membership(membership.key_in_str)   
-            
+
+
+
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/merchant_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,32 +69,69 @@
     
     reward_naming_configuration             = ndb.JsonProperty()
     
     prepaid_configuration                   = ndb.JsonProperty()
     
     product_modifier_configuration          = ndb.JsonProperty()
     
+    program_settings                        = ndb.JsonProperty()
+    
     stat_figure_update_interval_in_minutes  = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
     stat_figure_update_datetime_format      = '%d-%m-%Y %H:%M:%S'
     
     dict_properties = ['company_name', 'brand_name', 'contact_name', 'business_reg_no', 'mobile_phone', 'office_phone', 'fax_phone', 'email', 'account_code', 'country',
                        'registered_datetime', 'modified_datetime', 'plan_start_date', 'plan_end_date', 'currency_code', 
                        'published_program_configuration', 'published_voucher_configuration', 'membership_configuration', 
-                       'tier_membership_configuration', 'prepaid_configuration', 'product_modifier_configuration']
+                       'tier_membership_configuration', 'prepaid_configuration', 'product_modifier_configuration',
+                       'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured',
+                       ]
     
     
     def to_login_dict(self):
         return {
                 'account_code'      : self.account_code,
                 'plan_end_date'     : self.plan_end_date,
                 'currency_code'     : self.currency_code,
                 'country'           : self.country,
                 }
     
-       
+    @property
+    def program_configuration_list(self):
+        return self.published_program_configuration.get('programs')
+    
+    
+    @property
+    def is_tier_membership_configured(self):
+        return is_not_empty(self.tier_membership_configuration)
+    
+    
+    @property
+    def days_of_return_policy(self):
+        return self.program_settings.get('days_of_return_policy') or MerchantAcct.default_program_settings().get('days_of_return_policy')
+    
+    @property
+    def days_of_repeat_purchase_measurement(self):
+        return self.program_settings.get('days_of_repeat_purchase_measurement') or MerchantAcct.default_program_settings().get('days_of_repeat_purchase_measurement')
+    
+    @property
+    def membership_renew_advance_day(self):
+        return self.program_settings.get('membership_renew_advance_day') or MerchantAcct.default_program_settings().get('membership_renew_advance_day')
+    
+    @property
+    def membership_renew_late_day(self):
+        return self.program_settings.get('membership_renew_late_day') or MerchantAcct.default_program_settings().get('membership_renew_late_day')
+    
+    @staticmethod
+    def default_program_settings():
+        return {
+                'days_of_return_policy'                 : 3,
+                'days_of_repeat_purchase_measurement'   : 7,
+                'membership_renew_advance_day'          : 7,
+                'membership_renew_late_day'             : 30,
+                }   
     
     
     @staticmethod
     def update_details(merchant_acct, company_name=None, brand_name=None, business_reg_no=None, contact_name=None, email=None, mobile_phone=None, office_phone=None, currency_code=None, country=None):
         merchant_acct.company_name      = company_name
         merchant_acct.brand_name        = brand_name
         merchant_acct.business_reg_no   = business_reg_no
@@ -624,14 +661,15 @@
                                        mobile_phone     = mobile_phone,
                                        office_phone     = office_phone,
                                        plan_start_date  = plan_start_date, 
                                        plan_end_date    = plan_end_date,
                                        currency_code    = currency_code,
                                        country          = country,    
                                        api_key          = random_string(24),
+                                       program_settings = MerchantAcct.default_program_settings(),
                                        )
         
         logging.debug('account_code=%s', account_code)
         
         merchant_acct.account_code = account_code
         
         merchant_acct.put()
@@ -1098,30 +1136,31 @@
     receipt_footer_settings = ndb.JsonProperty()
     modified_datetime       = ndb.DateTimeProperty(auto_now=True)
     
     
     dict_properties = ['receipt_header_settings', 'receipt_footer_settings']
     
     @staticmethod
-    def update(merchant_acct, receipt_header_settings={}, receipt_footer_settings={}):
-        receipt_setup = ReceiptSetup.get_by_merchant_acct(merchant_acct)
-        
-        if receipt_setup:
-        
-            receipt_setup.receipt_header_settings      = receipt_header_settings
-            receipt_setup.receipt_footer_settings      = receipt_footer_settings
-            
-        else:
-            receipt_setup = ReceiptSetup(
+    def create(merchant_acct, receipt_header_settings={}):
+        receipt_setup = ReceiptSetup(
                                         parent                  = merchant_acct.create_ndb_key(),
                                         receipt_header_settings = receipt_header_settings,    
-                                        receipt_footer_settings = receipt_footer_settings,
+                                        receipt_footer_settings = {},
                                         )
         receipt_setup.put() 
         
+        return receipt_setup
+    
+    @staticmethod
+    def update(receipt_setup, receipt_header_settings={}, receipt_footer_settings={}):
+        receipt_setup.receipt_header_settings      = receipt_header_settings
+        receipt_setup.receipt_footer_settings      = receipt_footer_settings
+            
+        receipt_setup.put() 
+        
         return receipt_setup   
     
     @staticmethod    
     def remove(receipt_setup):
         receipt_setup.delete()
         
     @staticmethod
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.0.0/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/pos_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/pos_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/prepaid_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging, json
 from trexmodel import conf, program_conf
 from trexlib.utils.string_util import random_string
 from datetime import datetime, timedelta
 import trexmodel.conf as model_conf
 from trexlib.utils.common.common_util import sort_dict_list
 from trexmodel.utils.model.model_util import generate_transaction_id
+from dateutil.relativedelta import relativedelta
 
 logger = logging.getLogger('debug')
 
 class PrepaidSettings(BaseNModel,DictModel):
     '''
     Merchant acct as ancestor
     '''
@@ -203,20 +204,27 @@
     transaction_id                      = ndb.StringProperty(required=True)
     invoice_id                          = ndb.StringProperty(required=False)
     
     #store prepaid program key, topup_amount, prepaid_amount scheme
     prepaid_scheme_details              = ndb.JsonProperty(required=False)
     
     topup_datetime                      = ndb.DateTimeProperty(required=True, auto_now_add=True)
-    topup_by                            = ndb.KeyProperty(name="created_by", kind=MerchantUser)
+    topup_by                            = ndb.KeyProperty(name="topup_by", kind=MerchantUser)
+    topup_by_username                   = ndb.StringProperty(required=False)
     
     reverted_datetime                   = ndb.DateTimeProperty(required=False)
     reverted_by                         = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
     reverted_by_username                = ndb.StringProperty(required=False)
     
+    dict_properties         = ['transaction_id', 'invoice_id', 'topup_amount', 'topup_unit', 'topup_prepaid_rate',
+                               'prepaid_amount', 'used_prepaid_amount', 'status', 'prepaid_scheme_details',
+                               'topup_datetime', 'topup_by', 'reverted_datetime', 'reverted_by_username',
+                               'status'
+                               ]
+    
     @property
     def is_valid(self):
         return self.status == program_conf.REWARD_STATUS_VALID
     
     @property
     def is_redeemed(self):
         return self.status == program_conf.REWARD_STATUS_REDEEMED
@@ -225,126 +233,167 @@
     def is_used(self):
         return self.used_prepaid_amount>0
     
     @property
     def prepaid_balance(self):
         return self.prepaid_amount - self.used_prepaid_amount
     
+    @property
+    def expiry_date(self):
+        return (self.topup_datetime + relativedelta(years=100)).date()
+    
+    @property
+    def reward_format_key(self):
+        return None
+    
+    @property
+    def rewarded_datetime(self):
+        return self.topup_datetime
+    
+    @property
+    def reward_amount(self):
+        return self.prepaid_amount
+    
     def update_used_reward_amount(self, used_prepaid_amount):
         self.used_prepaid_amount    += used_prepaid_amount
         prepaid_balance              = self.prepaid_balance
         
+        if prepaid_balance<0:
+            prepaid_balance = 0
+        
         logger.debug('CustomerCountableReward: prepaid_balance=%s', prepaid_balance)
         
         if prepaid_balance ==0:
             self.status = program_conf.REWARD_STATUS_REDEEMED
-        
+        else:
+            self.status = program_conf.REWARD_STATUS_VALID
+            
         self.put()
     
+    @property
+    def reward_format(self):
+        return program_conf.REWARD_FORMAT_PREPAID
+    
     @staticmethod
     def __calculate_topup_unit(topup_amount, prepaid_scheme_details):
         return int(topup_amount/prepaid_scheme_details.get('topup_amount'))
     
     @staticmethod
     def __calculate_prepaid_amount(topup_unit, prepaid_scheme_details):
         return topup_unit * prepaid_scheme_details.get('prepaid_amount')
     
     @staticmethod
     def __calculate_topup_prepaid_rate(prepaid_scheme_details):
         return float(prepaid_scheme_details.get('topup_amount')/prepaid_scheme_details.get('prepaid_amount'))
     
     def to_prepaid_summary(self):
         prepaid_summary =  {
-                            'amount'            : self.prepaid_amount,
-                            'used_amount'       : self.used_prepaid_amount,    
+                            'amount'                : self.prepaid_amount,
+                            'used_amount'           : self.used_prepaid_amount,  
+                               
                             }
         
         return prepaid_summary
     
+    def to_reward_summary(self):
+        return self.to_prepaid_summary()
+    
     @property
     def is_reach_reward_limit(self):
         return self.status == program_conf.REWARD_STATUS_REACH_LIMIT
     
     @property
     def reward_balance(self):
         return self.prepaid_amount - self.used_prepaid_amount
     
+    @property
+    def reward_format_label(self):
+        return 'prepaid'
+    
+    @property
+    def reward_brief(self):
+        return 'Entitle {reward_amount} {reward_format}'.format(reward_amount=self.prepaid_amount, reward_format=self.reward_format_label)
+    
     @classmethod
     def list_by_valid_with_cursor(cls, customer, limit=50, start_cursor=None):
         query = cls.query(ndb.AND(cls.status==program_conf.REWARD_STATUS_VALID
             ), ancestor=customer.create_ndb_key()).order(cls.topup_datetime)
             
         (result, next_cursor) = cls.list_all_with_condition_query(query, start_cursor=start_cursor, return_with_cursor=True, limit=limit)
         
         return (result, next_cursor) 
     
     @staticmethod
     def list_by_customer(customer, status=program_conf.REWARD_STATUS_VALID, limit = conf.MAX_FETCH_RECORD):
         return CustomerPrepaidReward.query(ndb.AND(CustomerPrepaidReward.status==status), ancestor=customer.create_ndb_key()).fetch(limit=limit)
     
     @staticmethod
-    def list_all_by_customer(customer, limit = conf.MAX_FETCH_RECORD):
-        return CustomerPrepaidReward.query(ancestor=customer.create_ndb_key()).fetch(limit=limit)
+    def list_all_by_customer(customer, limit = conf.MAX_FETCH_RECORD, offset=0):
+        return CustomerPrepaidReward.query(ancestor=customer.create_ndb_key()).fetch(offset=offset, limit=limit)
     
     @staticmethod
     def list_by_transaction_id(transaction_id):
         return CustomerPrepaidReward.query(CustomerPrepaidReward.transaction_id==transaction_id).fetch(limit=conf.MAX_FETCH_RECORD)
     
     @staticmethod
     def list_by_customer_acct(customer_acct):
         return CustomerPrepaidReward.query(ndb.AND(CustomerPrepaidReward.status==program_conf.REDEEM_STATUS_VALID),ancestor=customer_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
         
     @staticmethod
-    def topup(customer_acct, topup_amount, prepaid_program, invoice_id=None, topup_outlet=None, topup_by=None, transaction_id=None):
-        
-        is_lump_sum_prepaid     = prepaid_program.is_lump_sum_prepaid
-        is_multi_tier_prepaid   = prepaid_program.is_multi_tier_prepaid
-        
-        sorted_tier_scheme      = None
-        
-        prepaid_scheme_details  = {
-                                    'program_key'   : prepaid_program.key_in_str
-                                    }
-        
-        tier_prepaid_scheme      = None
-        found_match_scheme       = None
-        
-        logger.debug('is_multi_tier_prepaid=%s', is_multi_tier_prepaid)
-        
-        if is_multi_tier_prepaid:
-            sorted_tier_scheme = sort_dict_list(prepaid_program.multitier_settings.values(), 'min_topup_amount')
+    def topup(customer_acct, topup_amount, prepaid_program, invoice_id=None, topup_outlet=None, topup_by=None, transaction_id=None, topup_datetime=None):
+        prepaid_scheme_details      = {
+                                        }
+        found_match_scheme          = None
+        
+        if prepaid_program:
+            is_lump_sum_prepaid     = prepaid_program.is_lump_sum_prepaid
+            is_multi_tier_prepaid   = prepaid_program.is_multi_tier_prepaid
             
-            logger.debug('Get topup scheme from topup amount(%s)', topup_amount)
+            sorted_tier_scheme      = None
             
-            #look for higheest min topup amount scheme
-            for scheme in sorted_tier_scheme:
-                if topup_amount>= scheme.get('min_topup_amount'):
-                    tier_prepaid_scheme = {
-                                            'topup_amount'  : scheme.get('topup_amount'),
-                                            'prepaid_amount': scheme.get('prepaid_amount'),
-                                            'prepaid_rate'  : scheme.get('prepaid_amount')/scheme.get('topup_amount'),
-                                            'scheme_type'   : 'tier',
-                                            }
-                    logger.debug('Found topup scheme for min topup amount(%s)', scheme.get('min_topup_amount'))
-        
-        logger.debug('tier_prepaid_scheme=%s', tier_prepaid_scheme)
-        
-        #if topup amount is less than smallest prepaid tier minimum topup amount, thus goto lump sum scheme    
-        if tier_prepaid_scheme is None and is_lump_sum_prepaid:
-            logger.debug('going to create scheme from lump sum setting')
-            prepaid_scheme = prepaid_program.lump_sum_settings
-            found_match_scheme = {
-                                            'topup_amount'  : prepaid_scheme.get('topup_amount'),
-                                            'prepaid_amount': prepaid_scheme.get('prepaid_amount'),
-                                            'prepaid_rate'  : prepaid_scheme.get('prepaid_amount')/prepaid_scheme.get('topup_amount'),
-                                            'scheme_type'   : 'lump_sum',
-                                            }  
-        
-        else:
-            found_match_scheme = tier_prepaid_scheme
+            prepaid_scheme_details  = {
+                                        'program_key'   : prepaid_program.key_in_str
+                                        }
+            
+            tier_prepaid_scheme      = None
+            
+            
+            logger.debug('is_multi_tier_prepaid=%s', is_multi_tier_prepaid)
+            
+            if is_multi_tier_prepaid:
+                sorted_tier_scheme = sort_dict_list(prepaid_program.multitier_settings.values(), 'min_topup_amount')
+                
+                logger.debug('Get topup scheme from topup amount(%s)', topup_amount)
+                
+                #look for higheest min topup amount scheme
+                for scheme in sorted_tier_scheme:
+                    if topup_amount>= scheme.get('min_topup_amount'):
+                        tier_prepaid_scheme = {
+                                                'topup_amount'  : scheme.get('topup_amount'),
+                                                'prepaid_amount': scheme.get('prepaid_amount'),
+                                                'prepaid_rate'  : scheme.get('prepaid_amount')/scheme.get('topup_amount'),
+                                                'scheme_type'   : 'tier',
+                                                }
+                        logger.debug('Found topup scheme for min topup amount(%s)', scheme.get('min_topup_amount'))
+            
+            logger.debug('tier_prepaid_scheme=%s', tier_prepaid_scheme)
+            
+            #if topup amount is less than smallest prepaid tier minimum topup amount, thus goto lump sum scheme    
+            if tier_prepaid_scheme is None and is_lump_sum_prepaid:
+                logger.debug('going to create scheme from lump sum setting')
+                prepaid_scheme = prepaid_program.lump_sum_settings
+                found_match_scheme = {
+                                                'topup_amount'  : prepaid_scheme.get('topup_amount'),
+                                                'prepaid_amount': prepaid_scheme.get('prepaid_amount'),
+                                                'prepaid_rate'  : prepaid_scheme.get('prepaid_amount')/prepaid_scheme.get('topup_amount'),
+                                                'scheme_type'   : 'lump_sum',
+                                                }  
+            
+            else:
+                found_match_scheme = tier_prepaid_scheme
              
         if found_match_scheme is None:
             logger.debug('going to create scheme default scheme')
             
             found_match_scheme = {
                                             'topup_amount'  : 1,
                                             'prepaid_amount': 1,
@@ -363,30 +412,37 @@
         topup_prepaid_rate  = CustomerPrepaidReward.__calculate_topup_prepaid_rate(prepaid_scheme_details)
         
         topup_by_key = None
         
         if topup_by:
             topup_by_key = topup_by.create_ndb_key()
             
+        if topup_datetime is None:
+            topup_datetime = datetime.utcnow()
+            
         merchant_acct               = customer_acct.registered_merchant_acct
         prepaid_topup_reward        = CustomerPrepaidReward(
                                                             parent                  = customer_acct.create_ndb_key(),
                                                             merchant_acct           = merchant_acct.create_ndb_key(),
-                                                            topup_outlet            = topup_outlet.create_ndb_key(),
+                                                            topup_outlet            = topup_outlet.create_ndb_key() if topup_outlet else None,
                                                             topup_amount            = topup_amount,
                                                             topup_unit              = topup_unit,
                                                             prepaid_amount          = prepaid_amount,
                                                             topup_prepaid_rate      = topup_prepaid_rate,
                                                             used_prepaid_amount     = .0,
                                                             prepaid_scheme_details  = prepaid_scheme_details,
                                                             
                                                             transaction_id          = transaction_id,
                                                             invoice_id              = invoice_id,
                                                             
                                                             topup_by                = topup_by_key,
+                                                            
+                                                            topup_datetime          = topup_datetime,    
                                                             )
         
         prepaid_topup_reward.put()
         
         return prepaid_topup_reward
     
     
+    
+
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/product_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/product_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,14 +754,16 @@
     merchant_acct as ancestor
     '''
     catalogue_name              = ndb.StringProperty(required=True)
     desc                        = ndb.StringProperty(required=False) 
     menu_settings               = ndb.JsonProperty()  
     published_menu_settings     = ndb.JsonProperty()
     
+    
+    
     is_publish                  = ndb.BooleanProperty(default=False)
     
     created_datetime            = ndb.DateTimeProperty(required=True, auto_now_add=True)
     modified_datetime           = ndb.DateTimeProperty(required=True, auto_now=True)  
     
     created_by                  = ndb.KeyProperty(name="created_by", kind=MerchantUser)
     modified_by                 = ndb.KeyProperty(name="modified_by", kind=MerchantUser)
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/program_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/program_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,17 +105,22 @@
     
     @property
     def is_recurring_scheme(self):
         if self.program_settings and self.program_settings.get('scheme'):
             return self.program_settings.get('scheme').get('is_recurring_scheme') or True
         
     @property
+    def giveaway_system_condition(self):
+        if self.program_settings and self.program_settings.get('giveaway_system_settings'):
+            return self.program_settings.get('giveaway_system_settings').get('giveaway_system_condition')
+        
+    @property
     def expiration_type(self):
         if self.program_settings and self.program_settings.get('scheme'):
-            return self.program_settings.get('scheme').get('expiration_type')
+            return self.program_settings.get('scheme').get('expiration_type')    
         
     @property
     def is_expiration_date_type(self):
         if self.program_settings and self.program_settings.get('scheme'):
             return self.program_settings.get('scheme').get('expiration_type') == program_conf.REWARD_EXPIRATION_TYPE_SPECIFIC_DATE    
         
     @property
@@ -159,19 +164,26 @@
         program.put()
         
         return program
     
     @classmethod
     def __create_schedule_program(cls, merchant_acct, program):
         if program.reward_base in (program_conf.SCHEDULE_BASED_PROGRAM):
+            
             if program.reward_base == program_conf.REWARD_BASE_ON_BIRTHDAY:
                 if program.giveaway_reward_when == program_conf.PROGRAM_SCHEDULE_TYPE_MONTH_START:
                     MerchantScheduleProgram.create_first_day_of_month_schedule_program(merchant_acct, program)
+                
                 elif program.giveaway_reward_when == program_conf.ADVANCE_IN_DAY:
                     MerchantScheduleProgram.create_daily_schedule_program(merchant_acct, program)
+                    
+            elif program.reward_base == program_conf.REWARD_BASE_ON_GIVEAWAY:
+                if program.giveaway_system_condition == program_conf.GIVEAWAY_SYSTEM_CONDITION_MEMBERSHIP_YEAR:
+                    MerchantScheduleProgram.create_daily_schedule_program(merchant_acct, program)
+                        
     
     @classmethod
     def __remove_schedule_program(cls, program):
         if program.reward_base in (program_conf.SCHEDULE_BASED_PROGRAM):
             MerchantScheduleProgram.remove_by_merchant_program(program)
         
     @classmethod
@@ -243,14 +255,15 @@
         
         cls.__remove_schedule_program(program)
         
     def to_program_configuration(self):
         program_configuration = {
                                 'merchant_acct_key'                 : self.parent_key,
                                 'program_key'                       : self.key_in_str,
+                                'label'                             : self.label,
                                 'desc'                              : self.desc,
                                 'reward_base'                       : self.reward_base,
                                 'reward_format'                     : self.reward_format,
                                 'giveaway_method'                   : self.giveaway_method,
                                 'start_date'                        : self.start_date.strftime('%d-%m-%Y'),
                                 'end_date'                          : self.end_date.strftime('%d-%m-%Y'),    
                                 'program_settings'                  : self.program_settings,
@@ -269,15 +282,15 @@
     
     @property
     def completed_status_index(self):
         return program_conf.get_program_completed_status_index(self.completed_status)
     
         
     @classmethod
-    def update_program_base_data(cls, program, reward_base=None, reward_format=None,  
+    def update_program_base_data(cls, program, label=None, reward_base=None, reward_format=None,  
                                  desc=None,start_date=None, end_date=None, modified_by=None):
         
         modified_by_username = None
         
         if is_not_empty(modified_by):
             if isinstance(modified_by, MerchantUser):
                 modified_by_username = modified_by.username
@@ -287,37 +300,38 @@
         exclusivity_configuration = {
                                                     'tags'              : [],
                                                     'memberships'       : [],
                                                     'tier_memberships'  : [],
                                                     }
         
         program_settings['exclusivity'] = exclusivity_configuration
-        
-        program.reward_base            = reward_base
-        program.reward_format          = reward_format
-        program.desc                   = desc
-        program.start_date             = start_date
-        program.end_date               = end_date
-        program.modified_by            = modified_by.create_ndb_key()
-        program.modified_by_username   = modified_by_username
-        program.completed_status       = program_conf.PROGRAM_STATUS_PROGRAM_BASE 
-        program.program_settings       = program_settings
+        program.label                   = label
+        program.reward_base             = reward_base
+        program.reward_format           = reward_format
+        program.desc                    = desc
+        program.start_date              = start_date
+        program.end_date                = end_date
+        program.modified_by             = modified_by.create_ndb_key()
+        program.modified_by_username    = modified_by_username
+        program.completed_status        = program_conf.PROGRAM_STATUS_PROGRAM_BASE 
+        program.program_settings        = program_settings
         
         
         
         program.put()
         
         return program
     
     @classmethod
     def update_prorgram_reward_details_data(cls, program, 
                                             giveaway_method=None,
                                             giveaway_system_condition = None, 
                                             giveaway_system_condition_membership_key=None, 
                                             giveaway_system_condition_tier_membership_key=None,
+                                            giveaway_system_condition_value=None,
                                             reward_scheme_configuration={}, modified_by=None,
                                             remarks=None):
         modified_by_username = None
         
         if is_not_empty(modified_by):
             if isinstance(modified_by, MerchantUser):
                 modified_by_username = modified_by.username
@@ -333,18 +347,20 @@
             
         if program_conf.REWARD_BASE_ON_GIVEAWAY == program.reward_base:  
             program.giveaway_method     = giveaway_method
             giveaway_system_settings    = program_settings.get('giveaway_system_settings')
             
             if giveaway_system_settings is None:        
                 giveaway_system_settings = {
-                                                    'giveaway_system_condition': giveaway_system_condition
+                                                    'giveaway_system_condition'         : giveaway_system_condition,
+                                                    'giveaway_system_condition_value'   : giveaway_system_condition_value,
                                                 }
             else:
-                giveaway_system_settings['giveaway_system_condition'] = giveaway_system_condition
+                giveaway_system_settings['giveaway_system_condition']       = giveaway_system_condition
+                giveaway_system_settings['giveaway_system_condition_value'] = giveaway_system_condition_value
                 
             if is_not_empty(giveaway_system_condition_membership_key):
                 giveaway_system_settings['giveaway_memberships'] = giveaway_system_condition_membership_key
             else:
                 if giveaway_system_settings.get('giveaway_memberships'):
                     del giveaway_system_settings['giveaway_memberships']
             
@@ -525,41 +541,36 @@
         program.modified_by                     = modified_by.create_ndb_key()
         program.modified_by_username            = modified_by_username
         program.put()    
     
     
     
 class MerchantProgram(BasicRewardProgram):
-    dict_properties                     = ['reward_base', 'giveaway_method', 'reward_format', 'completed_status', 'start_date', 'end_date', 'desc', 'program_settings', 
+    dict_properties                     = ['reward_base', 'giveaway_method', 'reward_format', 'completed_status', 'start_date', 'end_date', 'label','desc', 'program_settings', 
                                            'created_datetime', 'modified_datetime',  'enabled','completed_status','is_enabled', 'is_disabled', 'is_review_state', 
                                            'is_published', 'archived', 'is_reward_amount_required', 'completed_prograss_in_percentage', 'completed_status_index',
                                            'exclusive_tags_list', 'exclusive_memberships_list', 'exclusive_tier_memberships_list',
                                            'is_recurring_scheme', 
                                            'expiration_type', 'expiration_date', 'expiration_value', 'is_expiration_date_type',
                                            'giveaway_reward_when', 'giveaway_reward_advance_in_day',
                                            'giveaway_system_condition', 'giveaway_system_condition_memberships_list', 'giveaway_system_condition_tier_memberships_list',
                                            'created_by_username', 'modified_by_username']
     
     @property
-    def giveaway_system_condition(self):
-        if self.program_settings and self.program_settings.get('giveaway_system_settings'):
-            return self.program_settings.get('giveaway_system_settings').get('giveaway_system_condition')
-    
-    @property
     def giveaway_system_condition_memberships_list(self):
         if self.program_settings and self.program_settings.get('giveaway_system_settings'):
             return self.program_settings.get('giveaway_system_settings').get('giveaway_memberships')
     
     @property
     def giveaway_system_condition_tier_memberships_list(self):
         if self.program_settings and self.program_settings.get('giveaway_system_settings'):
             return self.program_settings.get('giveaway_system_settings').get('giveaway_tier_memberships')
     
     @staticmethod
-    def create(merchant_acct, reward_base=None, reward_format=None, 
+    def create(merchant_acct, label=None, reward_base=None, reward_format=None, 
                desc=None, start_date=None, end_date=None, created_by=None):
         
         created_by_username = None
         if is_not_empty(created_by):
             if isinstance(created_by, MerchantUser):
                 created_by_username = created_by.username
         
@@ -573,14 +584,15 @@
                             'exclusivity'               : exclusivity_configuration
                             }
         
         
         
         merchant_program =  MerchantProgram(
                                         parent                              = merchant_acct.create_ndb_key(),
+                                        label                               = label,
                                         reward_base                         = reward_base,
                                         reward_format                       = reward_format,
                                         desc                                = desc,
                                         start_date                          = start_date,
                                         end_date                            = end_date,
                                         created_by                          = created_by.create_ndb_key(),
                                         created_by_username                 = created_by_username,
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/redeem_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     CustomerStampReward, CustomerEntitledVoucher
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 
 
-logger = logging.getLogger('model')
+logger = logging.getLogger('debug')
 
 
 class CustomerRedeemedItemUpstream(DictModel):
     
     dict_properties         = ['customer_key', 'merchant_key', 'redeemed_outlet_key', 'transaction_id', 'redeemed_amount',
                                'reward_format', 'voucher_key', 'redeemed_datetime', 'reverted',
                                'reverted_datetime', 'is_revert'
@@ -71,33 +71,50 @@
     redeemed_by                 = ndb.KeyProperty(name="redeemed_by", kind=MerchantUser)
     redeemed_by_username        = ndb.StringProperty(required=False)
     
     reverted_datetime           = ndb.DateTimeProperty(required=False)
     reverted_by                 = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
     reverted_by_username        = ndb.StringProperty(required=False)
     
+    is_tier_program_redemption  = ndb.BooleanProperty(required=False, default=False) 
+    tier_program_transaction_id = ndb.StringProperty(required=False)
+    
+    
     dict_properties         = ['transaction_id', 'invoice_id', 'remarks', 'redeemed_amount', 'reward_format',
-                               'redeemed_summary', 'redeemed_customer', 'redeemed_outlet_details', 'redeemed_merchant_acct',
-                               'redeemed_datetime', 'is_revert',
-                               'redeemed_by_username'
+                               'redeemed_summary', 'redeemed_customer_acct', 'redeemed_outlet_details', 'redeemed_merchant_acct',
+                               'redeemed_datetime', 'is_revert', 'allow_to_revert', 
+                               'is_system_redemption', 'is_tier_program_redemption', 'tier_program_transaction_id',
+                               'redeemed_by_username', 'reverted_datetime', 'reverted_by_username',
                                ]
     
     @staticmethod
-    def list_by_transaction_id(cls, transaction_id):
-        return cls.query(cls.transaction_id==transaction_id).fetch(limit=conf.MAX_FETCH_RECORD)
+    def get_by_transaction_id(transaction_id):
+        return CustomerRedemption.query(CustomerRedemption.transaction_id==transaction_id).get()
     
     @property
     def is_valid(self):
         return self.status == program_conf.REDEEM_STATUS_VALID
     
     @property
+    def is_system_redemption(self):
+        return self.is_tier_program_redemption
+    
+    @property
+    def allow_to_revert(self):
+        return self.is_revert == False and self.is_tier_program_redemption==False
+    
+    @property
     def is_revert(self):
         return self.status == program_conf.REDEEM_STATUS_REVERTED
     
     @property
+    def is_voucher_redemption(self):
+        return self.redeemed_summary.get('vouchers')is not None and len(self.redeemed_summary.get('vouchers'))>0
+    
+    @property
     def redeemed_voucher_keys_list(self):
         return self.redeemed_summary.get('vouchers') 
     
     @property
     def redeemed_voucher_keys_list_in_str(self):
         vourchers =  self.redeemed_summary.get('vouchers')
         if vourchers:
@@ -122,21 +139,59 @@
         return Outlet.fetch(self.redeemed_outlet_key)
     
     @property
     def redeemed_customer_key(self):
         return self.parent_key
     
     @property
-    def redeemed_customer(self):
+    def redeemed_customer_acct(self):
         return Customer.fetch(self.parent_key)
     
     @property
     def redeem_format_label(self):
         pass
     
+    @property
+    def voucher_count(self):
+        count = 0
+        if self.reward_format == program_conf.REWARD_FORMAT_VOUCHER:
+            if self.redeemed_summary:
+                
+                for voucher_redeemed_details in  self.redeemed_summary.get(program_conf.REWARD_FORMAT_VOUCHER).get('vouchers').values():
+                    count+=voucher_redeemed_details.get('amount')
+            
+        return count
+    
+    def to_upstream_info(self):
+        return CustomerRedeemedItemUpstream(
+                                        customer_key        = self.redeemed_customer_key,
+                                        merchant_key        = self.redeemed_merchant_acct_key,
+                                        redeemed_outlet_key = self.redeemed_outlet_key,
+                                        transaction_id      = self.transaction_id,
+                                        reward_format       = self.reward_format,
+                                        redeemed_datetime   = self.redeemed_datetime,
+                                        redeemed_amount     = self.redeemed_amount,
+                                        
+                                    )
+        
+    def to_voucher_upstream_info_list(self):
+        upstream_info_list = []
+        for merchant_voucher_key, voucher_redeemed_details in  self.redeemed_summary.get(program_conf.REWARD_FORMAT_VOUCHER).get('vouchers').items():
+            upstream_info_list.append(CustomerRedeemedItemUpstream(
+                                        customer_key        = self.redeemed_customer_key,
+                                        merchant_key        = self.redeemed_merchant_acct_key,
+                                        redeemed_outlet_key = self.redeemed_outlet_key,
+                                        transaction_id      = self.transaction_id,
+                                        reward_format       = self.reward_format,
+                                        redeemed_datetime   = self.redeemed_datetime,
+                                        redeemed_amount     = voucher_redeemed_details.get('amount'),
+                                        voucher_key         = merchant_voucher_key,
+                                    ))    
+        return upstream_info_list
+    
     def revert(self, reverted_by, reverted_datetime=None):
         self.status = program_conf.REWARD_STATUS_REVERTED
         if reverted_datetime is None:
             reverted_datetime = datetime.now()
         
         self.reverted_datetime      = reverted_datetime
         self.reverted_by            = reverted_by.create_ndb_key()
@@ -150,23 +205,46 @@
     @staticmethod
     def list_customer_redemption(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
         query = CustomerRedemption.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerRedemption.redeemed_datetime)
         
         return CustomerRedemption.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
     
     @staticmethod
+    def list_by_outlet(redeemed_outlet, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
+        query = CustomerRedemption.query(ndb.AND(CustomerRedemption.redeemed_outlet==redeemed_outlet.create_ndb_key())).order(-CustomerRedemption.redeemed_datetime)
+        
+        return CustomerRedemption.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+    
+    @staticmethod
+    def list_merchant_transaction(merchant_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+        if reverse_order:
+            query = CustomerRedemption.query(ndb.AND(CustomerRedemption.merchant_acct==merchant_acct.create_ndb_key()))
+        else:
+            query = CustomerRedemption.query(ndb.AND(CustomerRedemption.merchant_acct==merchant_acct.create_ndb_key()))
+        
+        return CustomerRedemption.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+    
+    @staticmethod
     def count_customer_redemption(customer_acct, limit=conf.MAX_FETCH_RECORD):
         query = CustomerRedemption.query(ancestor = customer_acct.create_ndb_key())
         
         return CustomerRedemption.count_with_condition_query(query, limit=limit)
     
     @staticmethod
-    def create(customer, reward_format, redeemed_amount, redeemed_outlet, transaction_id=None, 
+    def count_merchant_redemption(merchant_acct, limit=conf.MAX_FETCH_RECORD):
+        query = CustomerRedemption.query(ndb.AND(CustomerRedemption.merchant_acct==merchant_acct.create_ndb_key()))
+        
+        return CustomerRedemption.count_with_condition_query(query, limit=limit)
+    
+    @staticmethod
+    def create(customer, reward_format, redeemed_outlet, transaction_id=None, 
+               redeemed_amount=1, is_tier_program_redemption=False, tier_program_transaction_id=None,
                redeemed_voucher_keys_list=None, invoice_id=None, remarks=None, redeemed_by=None, redeemed_datetime=None):
         
+        
         reward_summary              = customer.reward_summary
         prepaid_summary             = customer.prepaid_summary
         entitled_voucher_summary    = customer.entitled_voucher_summary
         
         if is_not_empty(redeemed_by):
             if isinstance(redeemed_by, MerchantUser):
                 redeemed_by_username = redeemed_by.username
@@ -175,162 +253,257 @@
         redeem_transaction_id = transaction_id or generate_transaction_id(prefix='r')
         
         if redeemed_datetime is None:
             redeemed_datetime = datetime.utcnow()
         
         redeemed_summary = {}
         
-        @model_transactional(desc='redeem reward')
+        #@model_transactional(desc='redeem reward')
         def __start_redeem(__customer, __total_redeemed_amount, cursor, reward_cls):
             (result, next_cursor) = reward_cls.list_by_valid_with_cursor(__customer, limit=50, start_cursor=cursor)
             
             if result:
+                 
                 redeemed_items_list = []
                 transaction_id_list = []
                 for r in result:
-                    reward_balance = r.reward_balance
+                    redeemed_amount                     = .0
+                    reward_balance_before_redeem        = r.reward_balance
                     
-                    logger.debug('__start_redeem: reward_balance=%s',  reward_balance)
+                    logger.debug('__start_redeem: reward_balance_before_redeem before=%s',  reward_balance_before_redeem)
+                    logger.debug('__start_redeem: __total_redeemed_amount before=%s',  __total_redeemed_amount)
                     
-                    if reward_balance<__total_redeemed_amount:
-                        logger.debug('__start_redeem: redeem full amount from reward')
+                    if reward_balance_before_redeem>0:
                         
-                        __total_redeemed_amount -=reward_balance
-                        r.update_used_reward_amount(reward_balance)
+                        if reward_balance_before_redeem<__total_redeemed_amount:
+                            logger.debug('__start_redeem: redeem partial amount from redeem amount')
+                            redeemed_amount = reward_balance_before_redeem
+                            __total_redeemed_amount -=reward_balance_before_redeem
+                            r.update_used_reward_amount(reward_balance_before_redeem)
+                            reward_balance_before_redeem = 0
+                            
+                        else:
+                            logger.debug('__start_redeem: redeem remaining balance from redeem amount')
+                            redeemed_amount = __total_redeemed_amount
+                            r.update_used_reward_amount(__total_redeemed_amount)
+                            reward_balance_before_redeem -= __total_redeemed_amount
+                            __total_redeemed_amount = 0
+                         
                         
-                    else:
-                        logger.debug('__start_redeem: redeem full amount from reward')
-                        r.update_used_reward_amount(__total_redeemed_amount)
-                        __total_redeemed_amount = 0
+                        logger.debug('__start_redeem: __total_redeemed_amount=%s',  __total_redeemed_amount)
+                        logger.debug('__start_redeem: reward_balance_before_redeem after =%s',  reward_balance_before_redeem)
                         
-                    logger.debug('__start_redeem: __total_redeemed_amount=%s',  __total_redeemed_amount)
+                        transaction_id_list.append(r.transaction_id)
                     
-                    transaction_id_list.append(r.transaction_id)
-                    
-                    #record customer CustomerPointReward/CustomerStampReward key and used_reward_amount
-                    redeemed_items_list.append({
-                                                'key'               : r.key_in_str, 
-                                                'redeemed_amount'   : reward_balance
-                                                })
-                    
-                    if __total_redeemed_amount==0:
-                        break
+                        #record customer CustomerPointReward/CustomerStampReward key and used_reward_amount
+                        redeemed_items_list.append({
+                                                    'key'      : r.key_in_str, 
+                                                    'amount'   : redeemed_amount,
+                                                    
+                                                    })
+                        
+                        if __total_redeemed_amount<=0:
+                            break
+                    else:
+                        logger.debug('__start_redeem reward balance is ZERO')
+                
+                logger.debug('after finished reading reward') 
                 
                 transaction_id_list = set(transaction_id_list) 
                 for transaction_id in transaction_id_list:
-                    CustomerTransaction.update_transaction_reward_have_been_redeemed(transaction_id)
+                    CustomerTransaction.update_transaction_reward_have_been_redeemed(transaction_id, redeem_transaction_id)
                 
                 return (__total_redeemed_amount, next_cursor,  redeemed_items_list)
             else:
                 raise Exception('Reward not found')
         
-        if reward_format == program_conf.REWARD_FORMAT_POINT or reward_format == program_conf.REWARD_FORMAT_STAMP:
-            total_redeemed_amount   = redeemed_amount
-            cursor                  = None
-            redeemed_items_list     = [] 
-            
+        if reward_format == program_conf.REWARD_FORMAT_POINT:
+            total_redeemed_amount               = redeemed_amount
+            cursor                              = None
+            redeemed_reward_details_list        = [] 
+            no_sufficient_to_redeem             = False
             while total_redeemed_amount>0:
-                (total_redeemed_amount, cursor, __redeemed_items_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
+                (total_redeemed_amount, cursor, __redeemed_reward_details_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
                                                                                         CustomerPointReward)
-                redeemed_items_list.extend(__redeemed_items_list)
+                logger.debug('after __start_redeem total_redeemed_amount= %s, cursor=%s', total_redeemed_amount, cursor)
+                logger.debug('__redeemed_reward_details_list count=%d', len(__redeemed_reward_details_list))
+                if __redeemed_reward_details_list:
+                    redeemed_reward_details_list.extend(__redeemed_reward_details_list)
+                    
+                if total_redeemed_amount>0 and cursor is None:
+                    no_sufficient_to_redeem = True
+                    break    
             
-            if reward_format == program_conf.REWARD_FORMAT_POINT:
+            if no_sufficient_to_redeem:
+                raise Exception('No sufficient balance to redeem')    
             
-                redeemed_summary = {
+            redeemed_summary = {
                                     reward_format               : {
                                         
                                                                     'amount'                    : redeemed_amount,        
-                                                                    'customer_point_rewards'    : redeemed_items_list
+                                                                    'customer_point_rewards'    : redeemed_reward_details_list
                                                                     }
                                     }
-            elif reward_format == program_conf.REWARD_FORMAT_STAMP:
-                redeemed_summary = {
-                                    reward_format               : {
-                                    
-                                                                'amount'                    : redeemed_amount,        
-                                                                'customer_stamp_rewards'    : redeemed_items_list
-                                                                }
-                                
-                                }
                 
             reward_balance = reward_summary[reward_format]['amount'] - redeemed_amount
             if reward_balance<0:
                 reward_balance = 0
                 
             reward_summary[reward_format]['amount'] = reward_balance
+        
+        elif reward_format == program_conf.REWARD_FORMAT_STAMP:
+            total_redeemed_amount           = redeemed_amount
+            cursor                          = None
+            redeemed_reward_details_list    = [] 
+            no_sufficient_to_redeem         = False
+            
+            while total_redeemed_amount>0:
+                (total_redeemed_amount, cursor, __redeemed_reward_details_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
+                                                                                        CustomerStampReward)
+                
+                logger.debug('after __start_redeem total_redeemed_amount= %s, cursor=%s', total_redeemed_amount, cursor)
+                logger.debug('__redeemed_reward_details_list count=%d', len(__redeemed_reward_details_list))
+                
+                if __redeemed_reward_details_list:
+                    redeemed_reward_details_list.extend(__redeemed_reward_details_list)
+                    
+                if total_redeemed_amount>0 and is_empty(cursor):
+                    no_sufficient_to_redeem = True
+                    logger.debug('suppose stop here')
+                    break  
+                else:
+                    logger.warn('still continue')
+                
+            if no_sufficient_to_redeem:
+                raise Exception('No sufficient balance to redeem')      
+            
+            redeemed_summary = {
+                                reward_format               : {
+                                
+                                                            'amount'                    : redeemed_amount,        
+                                                            'customer_stamp_rewards'    : redeemed_reward_details_list
+                                                            }
+                            
+                            }
+                
+            reward_balance = reward_summary[reward_format]['amount'] - redeemed_amount
+            if reward_balance<0:
+                reward_balance = 0
+                
+            reward_summary[reward_format]['amount'] = reward_balance    
             
         elif reward_format == program_conf.REWARD_FORMAT_PREPAID:
-            total_redeemed_amount   = redeemed_amount
-            cursor                  = None
-            redeemed_items_list     = [] 
+            total_redeemed_amount           = redeemed_amount
+            cursor                          = None
+            redeemed_reward_details_list    = [] 
+            no_sufficient_to_redeem         = False
             
             while total_redeemed_amount>0:
-                (total_redeemed_amount, cursor, __redeemed_items_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
+                (total_redeemed_amount, cursor, __redeemed_reward_details_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
                                                                                         CustomerPrepaidReward)
-                redeemed_items_list.extend(__redeemed_items_list)
+                
+                logger.debug('after __start_redeem total_redeemed_amount= %s, cursor=%s', total_redeemed_amount, cursor)
+                logger.debug('__redeemed_reward_details_list count=%d', len(__redeemed_reward_details_list))
+                
+                if __redeemed_reward_details_list:
+                    redeemed_reward_details_list.extend(__redeemed_reward_details_list)
+                
+                if total_redeemed_amount>0 and cursor is None:
+                    no_sufficient_to_redeem = True
+                    break 
+            
+            if no_sufficient_to_redeem:
+                raise Exception('No sufficient balance to redeem')
             
             redeemed_summary = {
-                                reward_format               : {
+                                program_conf.REWARD_FORMAT_PREPAID: {
                                     
                                                                 'amount'                    : redeemed_amount,        
-                                                                'customer_prepaid'          : redeemed_items_list
+                                                                'customer_prepaid_rewards'   : redeemed_reward_details_list
                                                                 }
                                 }
             
                 
             reward_balance = prepaid_summary['amount'] - redeemed_amount
             if reward_balance<0:
                 reward_balance = 0
                 
             prepaid_summary['amount'] = reward_balance    
                                 
             
         elif reward_format == program_conf.REWARD_FORMAT_VOUCHER:
             
-            redemption_details = {
+            redeemed_voucher_details_dict = {
                                 'vouchers': {}
                                 }
             
             voucher_redeem_codes_list           = []
             transaction_id_list                 = []
+            transaction_id_and_redeem_code_dict = {}
+            voucher_count                       = 0
             
-            for v_k in redeemed_voucher_keys_list:
-                customer_voucher            = CustomerEntitledVoucher.fetch(v_k)
-                merchant_voucher            = customer_voucher.merchant_voucher_entity
-                merchant_voucher_key        = customer_voucher.merchant_voucher_key
-                redeem_code                 = customer_voucher.redeem_code
-                redeemed_voucher_details    = redemption_details.get('vouchers').get(merchant_voucher_key)
+            for customer_entitled_voucher_key in redeemed_voucher_keys_list:
+                customer_entitled_voucher           = CustomerEntitledVoucher.fetch(customer_entitled_voucher_key)
+                merchant_voucher                    = customer_entitled_voucher.merchant_voucher_entity
+                merchant_voucher_key                = customer_entitled_voucher.merchant_voucher_key
+                redeem_code                         = customer_entitled_voucher.redeem_code
+                effective_date                      = customer_entitled_voucher.effective_date
+                expiry_date                         = customer_entitled_voucher.expiry_date
+                redeemed_voucher_details            = redeemed_voucher_details_dict.get('vouchers').get(merchant_voucher_key)
                 
                 voucher_redeem_codes_list.append(redeem_code)
+                voucher_count +=1
                 
                 if redeemed_voucher_details:
-                    redemption_details.get('vouchers')[merchant_voucher_key]['amount'] +=1
-                    redemption_details.get('vouchers')[merchant_voucher_key]['redeem_codes'].append(redeem_code)
-                    redemption_details.get('vouchers')[merchant_voucher_key]['customer_voucher_keys'].append(v_k)
+                    
+                    redeemed_voucher_details_dict.get('vouchers')[merchant_voucher_key]['amount'] +=1
+                    redeemed_voucher_details_dict.get('vouchers')[merchant_voucher_key]['customer_entitled_vouchers'].append({
+                                                                                                                            'customer_entitled_voucher_key': customer_entitled_voucher_key,
+                                                                                                                            'redeem_code': redeem_code,
+                                                                                                                            })
                 else:
-                    redemption_details.get('vouchers')[merchant_voucher_key] = {
-                                                                                    'label'                 : merchant_voucher.label,
-                                                                                    'image_url'             : merchant_voucher.image_public_url,
-                                                                                    'amount'                : 1,
-                                                                                    'redeem_codes'          : [redeem_code],
-                                                                                    'customer_voucher_keys' : [v_k]
+                    redeemed_voucher_details_dict.get('vouchers')[merchant_voucher_key] = {
+                                                                                    'label'                             : merchant_voucher.label,
+                                                                                    'image_url'                         : merchant_voucher.image_public_url,
+                                                                                    'amount'                            : 1,
+                                                                                    'customer_entitled_vouchers'    : [
+                                                                                                                        {
+                                                                                                                        'customer_entitled_voucher_key': customer_entitled_voucher_key,
+                                                                                                                        'redeem_code'   : redeem_code,
+                                                                                                                        'effective_date': effective_date.strftime('%d-%m-%Y'),
+                                                                                                                        'expired_date'  : expiry_date.strftime('%d-%m-%Y'),
+                                                                                                                        }
+                                                                                                                    ]
                                                                                 }
                 
-                customer_voucher.redeem(redeemed_by, redeemed_datetime=redeemed_datetime)
                 
-                transaction_id_list.append(customer_voucher.transaction_id)
+                customer_entitled_voucher.redeem(redeemed_by, redeemed_datetime=redeemed_datetime)
+                
+                transaction_id_list.append(customer_entitled_voucher.transaction_id)
                 
-                logger.debug('Voucher(%s) have been redeemed', customer_voucher.redeem_code)
+                if(transaction_id_and_redeem_code_dict.get(transaction_id)):
+                    if transaction_id_and_redeem_code_dict[customer_entitled_voucher.transaction_id].get(merchant_voucher_key):
+                        transaction_id_and_redeem_code_dict[customer_entitled_voucher.transaction_id][merchant_voucher_key].append(redeem_code)
+                    else:
+                        transaction_id_and_redeem_code_dict[customer_entitled_voucher.transaction_id]= {
+                                                                                            merchant_voucher_key:[redeem_code]
+                                                                                            }
+                else:
+                    transaction_id_and_redeem_code_dict[customer_entitled_voucher.transaction_id]= {
+                                                                                            merchant_voucher_key:[redeem_code]
+                                                                                            }
+                
+                logger.debug('Voucher(%s) have been redeemed', customer_entitled_voucher.redeem_code)
                 
                 
                 
             #mark customer sales/reward transaction entitled voucher have been redeem. thus transaction is not allow to revert
             transaction_id_list = set(transaction_id_list) 
-            for transaction_id in transaction_id_list:
-                CustomerTransaction.update_transaction_reward_have_been_redeemed(transaction_id)
+            for transaction_id, redeem_voucher_details_dict in transaction_id_and_redeem_code_dict.items():
+                CustomerTransaction.update_transaction_reward_have_been_redeemed(transaction_id, redeem_transaction_id, redeem_voucher_details_dict=redeem_voucher_details_dict, )
             
             #update customer entitled voucher summary
             copied_entitled_voucher_summary = entitled_voucher_summary.copy()
             
             for v_k, v_info in  copied_entitled_voucher_summary.items():
                 filtered_voucher_redeem_info_list = []
                 
@@ -339,37 +512,39 @@
                         filtered_voucher_redeem_info_list.append(redeem_info)
                 
                 if filtered_voucher_redeem_info_list:
                     entitled_voucher_summary[v_k]['redeem_info_list'] = filtered_voucher_redeem_info_list
                 else:
                     del entitled_voucher_summary[v_k]
             
-            redemption_details['customer_entitled_vouchers'] = redeemed_voucher_keys_list
-            
+            #redeemed_voucher_details_dict['customer_entitled_vouchers'] = redeemed_voucher_keys_list
+            redeemed_voucher_details_dict['amount'] = voucher_count
             redeemed_summary = {
-                                reward_format :   redemption_details
+                                reward_format :   redeemed_voucher_details_dict
                                 }
             
         customer_redemption = CustomerRedemption(
-                                                    parent                  = customer.create_ndb_key(),
-                                                    user_acct               = customer.registered_user_acct.create_ndb_key(),
-                                                    merchant_acct           = customer.registered_merchant_acct.create_ndb_key(),
-                                                    redeemed_outlet         = redeemed_outlet.create_ndb_key(),
-                                                    reward_format           = reward_format,
-                                                    redeemed_amount         = redeemed_amount,
-                                                    redeemed_summary        = redeemed_summary,
+                                                    parent                      = customer.create_ndb_key(),
+                                                    user_acct                   = customer.registered_user_acct.create_ndb_key(),
+                                                    merchant_acct               = customer.registered_merchant_acct.create_ndb_key(),
+                                                    redeemed_outlet             = redeemed_outlet.create_ndb_key(),
+                                                    reward_format               = reward_format,
+                                                    redeemed_amount             = redeemed_amount,
+                                                    redeemed_summary            = redeemed_summary,
                                                     
-                                                    transaction_id          = redeem_transaction_id,
-                                                    invoice_id              = invoice_id,
-                                                    remarks                 = remarks,
+                                                    transaction_id              = redeem_transaction_id,
+                                                    invoice_id                  = invoice_id,
+                                                    remarks                     = remarks,
                                                     
-                                                    redeemed_by             = redeemed_by.create_ndb_key(),
-                                                    redeemed_by_username    = redeemed_by_username,
+                                                    redeemed_by                 = redeemed_by.create_ndb_key(),
+                                                    redeemed_by_username        = redeemed_by_username,
                                                     
-                                                    redeemed_datetime       = redeemed_datetime,
+                                                    redeemed_datetime           = redeemed_datetime,
+                                                    is_tier_program_redemption  = is_tier_program_redemption,
+                                                    tier_program_transaction_id = tier_program_transaction_id,
                                                     
                                                     )
         
         
         customer_redemption.put()
         
         customer.reward_summary             = reward_summary
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/reward_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/reward_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,25 +111,33 @@
         self.put()
     
     @classmethod
     def list_by_customer(cls, customer, status=program_conf.REWARD_STATUS_VALID, limit = conf.MAX_FETCH_RECORD):
         return cls.query(ndb.AND(cls.status==status), ancestor=customer.create_ndb_key()).fetch(limit=limit)
         
     @classmethod
-    def list_all_by_customer(cls, customer, limit = conf.MAX_FETCH_RECORD):
-        return cls.query(ancestor=customer.create_ndb_key()).fetch(limit=limit)
+    def list_all_by_customer(cls, customer, offset=0, limit = conf.MAX_FETCH_RECORD):
+        return cls.query(ancestor=customer.create_ndb_key()).fetch(offset=offset, limit=limit)
     
     @classmethod
     def list_all_by_user_acct(cls, user_acct, limit = conf.MAX_FETCH_RECORD):
         return cls.query(ndb.AND(cls.user_acct==user_acct.create_ndb_key())).fetch(limit=limit)    
 
 class CustomerCountableReward(CustomerEntitledReward):
     reward_amount               = ndb.FloatProperty(required=True, default=0)
     used_reward_amount          = ndb.FloatProperty(required=True, default=0)
     
+    dict_properties     = [
+                            'reward_amount', 'used_reward_amount', 'transaction_id', 'rewarded_datetime', 
+                            'status',
+                           ]
+    
+    def __repr__(self):
+        return 'transaction_id=%s, rewarded_datetime=%s, reward_balance=%s'% (self.transaction_id, self.rewarded_datetime, self.reward_balance)
+    
     @property
     def is_reach_reward_limit(self):
         return self.status == program_conf.REWARD_STATUS_REACH_LIMIT
     
     @property
     def reward_balance(self):
         return self.reward_amount - self.used_reward_amount
@@ -147,15 +155,23 @@
     @classmethod
     def list_by_valid_with_cursor(cls, customer, limit=50, start_cursor=None):
         query = cls.query(ndb.AND(cls.status==program_conf.REWARD_STATUS_VALID
             ), ancestor=customer.create_ndb_key()).order(cls.expiry_date)
             
         (result, next_cursor) = cls.list_all_with_condition_query(query, start_cursor=start_cursor, return_with_cursor=True, limit=limit)
         
-        return (result, next_cursor) 
+        return (result, next_cursor)
+    
+    @classmethod
+    def list_valid(cls, customer, limit=50):
+        query = cls.query(ndb.AND(cls.status==program_conf.REWARD_STATUS_VALID
+            ), ancestor=customer.create_ndb_key()).order(cls.expiry_date)
+            
+        return cls.list_all_with_condition_query(query, limit=limit)
+         
     
     @property
     def is_used(self):
         return self.used_reward_amount>0
     
     @property
     def reward_brief(self):
@@ -292,14 +308,26 @@
     use_in_store                = ndb.BooleanProperty(required=False, default=False)
     
     dict_properties     = [
                             'redeem_code', 'configuration', 'rewarded_datetime', 'transaction_id', 
                             'status', 'is_reverted', 'is_used',
                            ]
     
+    @staticmethod
+    def list_by_transaction_id(transaction_id):
+        return CustomerEntitledVoucher.query(CustomerEntitledVoucher.transaction_id==transaction_id).fetch(limit=conf.MAX_FETCH_RECORD)
+    
+    def revert_from_redemption(self):
+        self.status = program_conf.REDEEM_STATUS_VALID
+        self.redeemed_datetime      = None
+        self.redeemed_by            = None
+        self.redeemed_by_username   = None
+        self.put()
+        
+    
     def redeem(self, redeemed_by, redeemed_datetime=None):
         self.status = program_conf.REWARD_STATUS_REDEEMED   
         
         if redeemed_datetime is None:
             redeemed_datetime = datetime.now()
         
         self.redeemed_datetime      = redeemed_datetime
@@ -404,19 +432,20 @@
     def get_by_redeem_code(redeem_code):
         return  CustomerEntitledVoucher.query(CustomerEntitledVoucher.redeem_code==redeem_code).get()
     
     @staticmethod
     def list_by_customer(customer, limit=conf.MAX_FETCH_RECORD, offset=0, voucher_status=program_conf.REWARD_STATUS_VALID):
         return CustomerEntitledVoucher.query(ndb.AND(CustomerEntitledVoucher.status==voucher_status),
                 ancestor=customer.create_ndb_key()).fetch(limit=limit, offset=offset)
-
+    
+    '''
     @staticmethod
     def list_all_by_customer(customer, limit=conf.MAX_FETCH_RECORD, offset=0):
         return CustomerEntitledVoucher.query(ancestor=customer.create_ndb_key()).fetch(limit=limit, offset=offset)
-    
+    '''
         
     @staticmethod
     def update_customer_entiteld_voucher_summary(customer, voucher_status=program_conf.REWARD_STATUS_VALID):
         customers_vouchers_list = CustomerEntitledVoucher.list_by_customer(customer, voucher_status=voucher_status)
         entitled_voucher_summary   = {}
         if customers_vouchers_list:
             
@@ -424,14 +453,15 @@
                 merchant_voucher        = customer_voucher.merchant_voucher_entity
                 merchant_voucher_key    = customer_voucher.merchant_voucher_key
                 voucher_summary         = entitled_voucher_summary.get(merchant_voucher_key)
                 new_redeem_info         = {
                                             'redeem_code'       : customer_voucher.redeem_code,
                                             'effective_date'    : customer_voucher.effective_date.strftime('%d-%m-%Y'),
                                             'expiry_date'       : customer_voucher.expiry_date.strftime('%d-%m-%Y'),
+                                            'is_redeem'         : False,
                                             }    
                 if voucher_summary:
                     entitled_voucher_summary[merchant_voucher_key]['key']=merchant_voucher_key
                     entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'].append(new_redeem_info)
                     
                 else:
                     entitled_voucher_summary[merchant_voucher_key]={
@@ -518,14 +548,18 @@
                 
                 found_incomplete_tier = True
                 
         return {
                 'label' : tier_reward_program.label,
                 'tiers' :tier_details_list
                 }
+    
+    @staticmethod
+    def list_all_by_customer(customer, limit = conf.MAX_FETCH_RECORD, offset=0):
+        return CustomerEntitledTierRewardSummary.query(ancestor=customer.create_ndb_key()).fetch(offset=offset, limit=limit)
         
     @staticmethod
     def list_tier_reward_summary_by_customer(customer_acct):
         today = datetime.utcnow().date()
         return CustomerEntitledTierRewardSummary.query(ndb.AND(
                                                             CustomerEntitledTierRewardSummary.is_valid==True, 
                                                             CustomerEntitledTierRewardSummary.program_end_date>=today
@@ -556,15 +590,19 @@
                             'tier_index'                : tier_setting.get('tier_index'),
                             'tier_label'                : tier_setting.get('tier_label'),
                             'unlock_tier_message'       : tier_setting.get('unlock_tier_message'),
                             'unlock_status'             : False,
                             'unlock_condition'          : tier_setting.get('unlock_tier_condition'),
                             'unlock_condition_value'    : tier_setting.get('unlock_tier_condition_value'), 
                             'unlock_value'              : .0,
-                            }  
+                            'unlock_source_details'     : {},
+                            }
+            
+            
+              
             tier_reward_summary_list.append(tier_summary)  
             
         
         reward_summary = CustomerEntitledTierRewardSummary(
                                             parent                  = customer_acct.create_ndb_key(),
                                             tier_reward_program     = tier_reward_program.create_ndb_key(),
                                             program_end_date        = tier_reward_program.end_date,
@@ -574,42 +612,43 @@
                                             )
         
         reward_summary.put()
         
         return reward_summary
     
     @staticmethod
-    def update(customer_tier_reward_summary, tier_summary=None, cycle_start_datetime=None, cycle_end_datetime=None):
+    def update(customer_tier_reward_summary, tier_summary_list=None, cycle_start_datetime=None):
         if cycle_start_datetime:
             customer_tier_reward_summary.cycle_start_datetime = cycle_start_datetime
         
-        if cycle_end_datetime:
-            customer_tier_reward_summary.cycle_end_datetime = cycle_end_datetime
-            
-        customer_tier_reward_summary.tier_summary = tier_summary
         if customer_tier_reward_summary.is_cycle_completed:
             customer_tier_reward_summary.cycle_end_datetime = datetime.utcnow()
         
+        
+        customer_tier_reward_summary.tier_summary = tier_summary_list
+        
+        logger.debug('update CustomerEntitledTierRewardSummary with customer_tier_reward_summary=%s', customer_tier_reward_summary)
         customer_tier_reward_summary.put()
         
     @staticmethod
     def restart_cycle(customer_tier_reward_summary, cycle_start_datetime=None):
         if cycle_start_datetime is None:
             customer_tier_reward_summary.cycle_start_datetime   = datetime.utcnow()
         else:
             customer_tier_reward_summary.cycle_start_datetime   = cycle_start_datetime
             
         customer_tier_reward_summary.cycle_end_datetime     = None
         
         tier_details_list = customer_tier_reward_summary.tier_summary.get('tiers')
         
         for tier_details in tier_details_list:
-            tier_details['unlock_status']      = False
-            tier_details['unlock_datetime']    = None
-            tier_details['unlock_value']       = .0
+            tier_details['unlock_status']           = False
+            tier_details['unlock_datetime']         = None
+            tier_details['unlock_value']            = .0
+            tier_details['unlock_source_details']   = {}
         
         logger.debug('tier_details_list=%s', tier_details_list)
             
         customer_tier_reward_summary.tier_summary['ties'] = tier_details_list
         
         customer_tier_reward_summary.put()
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.0.0/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/system_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/task_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/test_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/transaction_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 
 @author: jacklok
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.user_models import User
-from trexmodel.models.datastore.customer_models import Customer
-import trexmodel.conf as model_conf
+from trexmodel.models.datastore.customer_models import Customer,\
+    CustomerMembership
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet,\
     MerchantUser
 import logging
 from trexmodel import conf, program_conf
-from datetime import datetime,date, timedelta
-from trexmodel.models.datastore.reward_models import CustomerPointReward,\
-    CustomerStampReward, CustomerEntitledVoucher, CustomerEntitledReward
-from trexmodel.models.datastore.customer_model_helpers import update_reward_summary_with_reverted_reward,\
-    update_customer_entiteld_voucher_summary_after_reverted_voucher
+from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id
-from gettext import gettext
+from trexmodel.models.datastore.membership_models import MerchantMembership,\
+    MerchantTierMembership
+from trexmodel.program_conf import REWARD_FORMAT_POINT
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
-from trexmodel.models.datastore.program_models import MerchantTierRewardProgram
+from trexmodel.models.datastore.reward_models import CustomerPointReward,\
+    CustomerStampReward, CustomerEntitledVoucher
 
 logger = logging.getLogger('model')
 
 
 class CustomerTransaction(BaseNModel, DictModel):
     '''
     
@@ -66,48 +65,85 @@
     reverted_by                 = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
     reverted_by_username        = ndb.StringProperty(required=False)
     
     is_reward_redeemed          = ndb.BooleanProperty(required=False, default=False)
     
     is_sales_transaction        = ndb.BooleanProperty(required=False, default=True)
     
+    is_membership_purchase      = ndb.BooleanProperty(required=False, default=False)
+    is_membership_renew         = ndb.BooleanProperty(required=False, default=False)
+    
+    is_tier_membership_upgraded = ndb.BooleanProperty(required=False, default=False)
+    
+    upgraded_merchant_tier_membership   = ndb.KeyProperty(name="upgraded_merchant_tier_membership", kind=MerchantTierMembership)
+    
+    purchased_merchant_membership        = ndb.KeyProperty(name="purchased_merchant_membership", kind=MerchantMembership)
+    purchased_customer_membership        = ndb.KeyProperty(name="purchased_customer_membership", kind=CustomerMembership)
+    
     dict_properties         = ['transaction_id', 'invoice_id', 'remarks', 'system_remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
                                'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 
                                'transact_customer_acct', 'transact_outlet_details', 'transact_merchant_acct',
-                               'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime',
+                               'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime', 'reverted_by_username',
                                'transact_by', 'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
+                               'is_membership_purchase', 'purchased_merchant_membership_key', 'is_tier_membership_upgraded', 'upgraded_merchant_tier_membership_key',
                                ]
     
     def to_transaction_details_json(self):
         pass
     
     @property
+    def is_point_reward_entitled(self):
+        if is_not_empty(self.entitled_reward_summary):
+            if program_conf.REWARD_FORMAT_POINT in self.entitled_reward_summary:
+                return True
+        return False
+    
+    @property
+    def is_stamp_reward_entitled(self):
+        if is_not_empty(self.entitled_reward_summary):
+            if program_conf.REWARD_FORMAT_STAMP in self.entitled_reward_summary:
+                return True
+        return False
+    
+    @property
+    def is_voucher_reward_entitled(self):
+        if is_not_empty(self.entitled_voucher_summary):
+            return True
+        return False
+    
+    @property
+    def is_prepaid_reward_entitled(self):
+        if is_not_empty(self.entitled_prepaid_summary):
+            return True
+        return False
+    
+    @property
     def transact_customer_acct(self):
         return Customer.fetch(self.key.parent().urlsafe())
     
     @property
     def transact_user_acct_key(self):
         return Customer.fetch(self.key.parent().urlsafe()).registered_user_acct_key
     
     @property
     def transact_merchant_acct(self):
         return MerchantAcct.fetch(self.transact_merchant.urlsafe())
     
     @property
     def transact_outlet_key(self):
         if self.transact_outlet:
-            return self.transact_outlet.urlsafe()
+            return self.transact_outlet.urlsafe().decode('utf-8')
     
     @property
     def transact_merchant_acct_key(self):
-        return self.transact_merchant.urlsafe()
+        return self.transact_merchant.urlsafe().decode('utf-8')
     
     @property
     def transact_customer_key(self):
-        return self.key.parent().urlsafe()
+        return self.key.parent().urlsafe().decode('utf-8')
     
     @property
     def transact_outlet_details(self):
         if self.transact_outlet:
             return Outlet.fetch(self.transact_outlet.urlsafe())
     
     @property
@@ -118,36 +154,77 @@
     @property
     def after_deduct_tax_sales_amount(self):
         if self.tax_amount:
             return self.transact_amount - self.tax_amount
         else:
             return self.transact_amount
     
+    @property
+    def purchased_merchant_membership_key(self):
+        if self.purchased_merchant_membership:
+            return self.purchased_merchant_membership.urlsafe().decode('utf-8')
+    
+    @property
+    def purchased_customer_membership_entity(self):
+        if self.purchased_customer_membership:
+            return CustomerMembership.fetch(self.purchased_customer_membership.urlsafe())
+    
+    @property
+    def upgraded_merchant_tier_membership_key(self):
+        if self.upgraded_merchant_tier_membership:
+            return self.upgraded_merchant_tier_membership.urlsafe().decode('utf-8')
+    
     @staticmethod
-    def update_transaction_reward_have_been_redeemed(transaction_id):
+    def update_transaction_reward_have_been_redeemed(transaction_id, redeem_transaction_id, redeem_voucher_details_dict=None):
         
         logger.debug('Update customer transaction reward have been redeemed by transaction id=%s', transaction_id)
         
         if transaction_id:
             customer_transaction = CustomerTransaction.get_by_transaction_id(transaction_id)
             if customer_transaction:
                 customer_transaction.is_reward_redeemed = True
+                
+                if redeem_voucher_details_dict:
+                    # voucher key -[list of voucher redeem code]
+                    entitled_voucher_summary = customer_transaction.entitled_voucher_summary
+                    for voucher_key, redeem_code_list in redeem_voucher_details_dict.items():
+                        if entitled_voucher_summary.get(voucher_key):
+                            for redeem_info in entitled_voucher_summary.get(voucher_key).get('redeem_info_list'):
+                                if redeem_info.get('redeem_code') in redeem_code_list:
+                                    redeem_info['is_redeem'] = True
+                                    redeem_info['redeem_transaction_id'] = redeem_transaction_id
+                    
+                
                 customer_transaction.put()
     
     @staticmethod
-    def create_manual_transaction(customer, remarks=None, system_remarks=None, transact_outlet=None, transact_by=None, transact_datetime=None, is_sales_transaction=False, allow_to_revert=True): 
+    def create_membership_purchase_transaction(customer, purchased_customer_membership, 
+                                               remarks=None, system_remarks=None, transact_outlet=None, 
+                                               transact_by=None, transact_datetime=None, 
+                                               allow_to_revert=True,):
+         
         return CustomerTransaction.create_system_transaction(customer, remarks=remarks, system_remarks=system_remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
                                    transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL,
-                                   is_sales_transaction = is_sales_transaction, allow_to_revert=allow_to_revert,
+                                   is_sales_transaction = False, allow_to_revert=allow_to_revert, is_membership_purchase=True, is_membership_renew=False,
+                                   purchased_customer_membership=purchased_customer_membership, 
                                    )
+        
+    @staticmethod
+    def create_manual_transaction(customer, remarks=None, system_remarks=None, transact_outlet=None, transact_by=None, transact_datetime=None, is_sales_transaction=False, 
+                                  allow_to_revert=True, is_membership_purchase=False, is_membership_renew=False): 
+        return CustomerTransaction.create_system_transaction(customer, remarks=remarks, system_remarks=system_remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
+                                   transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL,
+                                   is_sales_transaction = is_sales_transaction, allow_to_revert=allow_to_revert, 
+                                   is_membership_purchase=is_membership_purchase, is_membership_renew=is_membership_renew,
+                                   )    
     
     @staticmethod
     def create_system_transaction(customer, transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
                transact_outlet=None, transact_by=None, transact_datetime=None, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM,
-               is_sales_transaction = False, allow_to_revert=True
+               is_sales_transaction = False, allow_to_revert=True, is_membership_purchase=False, is_membership_renew=False, purchased_customer_membership=None,
                ):
         
         transact_by_username = None
         
         if is_not_empty(transact_by):
             if isinstance(transact_by, MerchantUser):
                 transact_by_username = transact_by.username
@@ -163,42 +240,46 @@
         logger.debug('tax_amount=%s', tax_amount)
         logger.debug('transact_amount=%s', transact_amount)
         logger.debug('transact_datetime=%s', transact_datetime)
         logger.debug('transact_by_username=%s', transact_by_username)
         logger.debug('system_remarks=%s', system_remarks)
         
         customer_transaction = CustomerTransaction(
-                                                    parent                  = customer.create_ndb_key(),
+                                                    parent                          = customer.create_ndb_key(),
                                                     
-                                                    transact_merchant       = customer.registered_merchant_acct.create_ndb_key(),
-                                                    transact_outlet         = transact_outlet.create_ndb_key() if transact_outlet else None,
+                                                    transact_merchant               = customer.registered_merchant_acct.create_ndb_key(),
+                                                    transact_outlet                 = transact_outlet.create_ndb_key() if transact_outlet else None,
                                                     
-                                                    tax_amount              = tax_amount,
-                                                    transact_amount         = transact_amount,
+                                                    tax_amount                      = tax_amount,
+                                                    transact_amount                 = transact_amount,
                                                     
-                                                    transaction_id          = transaction_id,
-                                                    invoice_id              = invoice_id,
-                                                    remarks                 = remarks,
-                                                    system_remarks          = system_remarks,
+                                                    transaction_id                  = transaction_id,
+                                                    invoice_id                      = invoice_id,
+                                                    remarks                         = remarks,
+                                                    system_remarks                  = system_remarks,
                                                     
-                                                    transact_by             = transact_by.create_ndb_key() if transact_by else None,
-                                                    transact_by_username    = transact_by_username,
+                                                    transact_by                     = transact_by.create_ndb_key() if transact_by else None,
+                                                    transact_by_username            = transact_by_username,
                                                     
-                                                    transact_datetime       = transact_datetime,
-                                                    reward_giveaway_method  = reward_giveaway_method,
+                                                    transact_datetime               = transact_datetime,
+                                                    reward_giveaway_method          = reward_giveaway_method,
                                                     
-                                                    is_sales_transaction    = is_sales_transaction,
-                                                    allow_to_revert         = allow_to_revert,
+                                                    is_sales_transaction            = is_sales_transaction,
+                                                    allow_to_revert                 = allow_to_revert,
+                                                    is_membership_purchase          = is_membership_purchase,
+                                                    is_membership_renew             = is_membership_renew,
+                                                    purchased_merchant_membership   = purchased_customer_membership.merchant_membership_entity.create_ndb_key() if purchased_customer_membership else None,
+                                                    purchased_customer_membership   = purchased_customer_membership.create_ndb_key() if purchased_customer_membership else None,
                                                     )
         
         customer_transaction.put()
-        customer.put()
+        #customer.put()
         
         return customer_transaction
-    
+    '''
     def revert(self, customer_acct, reverted_by):
         transaction_id = self.transaction_id
         
         entitled_point_details_list     = CustomerPointReward.list_by_transaction_id(transaction_id)
         
         entitled_stamp_details_list     = CustomerStampReward.list_by_transaction_id(transaction_id)
         
@@ -287,51 +368,75 @@
             customer_acct.reward_summary            = customer_reward_summary
             customer_acct.entitled_voucher_summary  = updated_voucher_summary or {}
             customer_acct.put()
             
             return True
         
         else:
-            raise Exception(gettext('Transaction reward have been used'))
-    
+            raise Exception('Transaction reward have been used')
+    '''
     @staticmethod
     def list_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
         if reverse_order:
             query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerTransaction.transact_datetime)
         else:
             query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(CustomerTransaction.transact_datetime)
         
         return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
     
     @staticmethod
-    def list_valid_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+    def list(offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
         if reverse_order:
-            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerTransaction.transact_datetime)
+            query = CustomerTransaction.query().order(-CustomerTransaction.transact_datetime)
         else:
-            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(CustomerTransaction.transact_datetime)
+            query = CustomerTransaction.query().order(CustomerTransaction.transact_datetime)
         
-        result                  = None
-        next_cursor             = None
-        valid_transaction_list  = []
+        return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+    
+    @staticmethod
+    def list_outlet_transaction(transact_outlet, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+        if reverse_order:
+            query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_outlet==transact_outlet.create_ndb_key())).order(-CustomerTransaction.transact_datetime)
+        else:
+            query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_outlet==transact_outlet.create_ndb_key())).order(CustomerTransaction.transact_datetime)
         
-        if return_with_cursor:
-            (result, next_cursor) = CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+        return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+    
+    @staticmethod
+    def list_merchant_transaction(transact_merchant, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+        if reverse_order:
+            query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_merchant==transact_merchant.create_ndb_key()))
         else:
-            result =  CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+            query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_merchant==transact_merchant.create_ndb_key()))
         
+        return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+    
+    @staticmethod
+    def count_valid_customer_transaction(customer_acct, limit=conf.MAX_FETCH_RECORD):
+        query = CustomerTransaction.query(ndb.AND(CustomerTransaction.is_revert==False), ancestor = customer_acct.create_ndb_key())
+        
+        return   CustomerTransaction.count_with_condition_query(query, limit=limit)
+    
+    @staticmethod
+    def count_outlet_transaction(transact_outlet, limit=conf.MAX_FETCH_RECORD):
+        query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_outlet==transact_outlet.create_ndb_key()))
         
-        if result:
-            for r in result:
-                if r.is_revert==False:
-                    valid_transaction_list.append(r)
+        return   CustomerTransaction.count_with_condition_query(query, limit=limit)
+    
+    @staticmethod
+    def list_valid_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
+        
+        query = CustomerTransaction.query(ndb.AND(CustomerTransaction.is_revert==False), ancestor = customer_acct.create_ndb_key())
         
         if return_with_cursor:
-            return (valid_transaction_list, next_cursor)
+            return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
         else:
-            return valid_transaction_list
+            return  CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+        
+        
             
     
     @staticmethod
     def list_customer_transaction_by_transact_timestamp(customer_acct, transact_timestamp_from=None, transact_timestamp_to=None):
         return CustomerTransaction.query(ndb.AND(
                                                     CustomerTransaction.transact_timestamp>transact_timestamp_from,
                                                     CustomerTransaction.transact_timestamp<=transact_timestamp_to
@@ -400,14 +505,20 @@
     @staticmethod
     def count_customer_transaction(customer_acct, limit=conf.MAX_FETCH_RECORD):
         query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key())
         
         return CustomerTransaction.count_with_condition_query(query, limit=limit)
     
     @staticmethod
+    def count_merchant_transaction(merchant_acct, limit=conf.MAX_FETCH_RECORD):
+        query = CustomerTransaction.query(ndb.AND(CustomerTransaction.transact_merchant==merchant_acct.create_ndb_key()))
+        
+        return CustomerTransaction.count_with_condition_query(query, limit=limit)
+    
+    @staticmethod
     def count_transaction_by_date(transact_date, including_reverted_transaction=True, transact_outlet=None, limit=conf.MAX_FETCH_RECORD):
         
         transact_datetime           = datetime.combine(transact_date, datetime.min.time())
         next_day_transact_datetime  = transact_datetime + timedelta(days=1)
         
         logger.debug('transact_datetime=%s',transact_datetime)
         logger.debug('next_day_transact_datetime=%s',next_day_transact_datetime)
@@ -473,14 +584,14 @@
         self.is_revert                      = transaction_details.is_revert
         self.reverted_datetime              = transaction_details.reverted_datetime
         self.topup_amount                   = prepaid_details.topup_amount
         self.prepaid_amount                 = prepaid_details.prepaid_amount
         self.topup_datetime                 = prepaid_details.topup_datetime 
             
     
-    
+
```

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/user_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.0.0/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.9/trexmodel/models/merchant_helpers.py` & `trex-model-1.0.0/trexmodel/models/merchant_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     
     account_settings['assigned_service_charge_setup']   = outlet.service_charge_settings
     account_settings['assigned_tax_setup']              = outlet.assigned_tax_setup
     account_settings['dinning_table_list']              = outlet.assigned_dinning_table_list
     account_settings['show_dinning_table_occupied']     = outlet.show_dinning_table_occupied
     account_settings['payment_methods']                 = pos_payment_method_json
     
+    
     outlet_details = {
                     'key'                        : outlet.key_in_str,
                     'id'                         : outlet.id,
                     'outlet_name'                : outlet.name,
                     'company_name'               : outlet.company_name,
                     'brand_name'                 : merchant_acct.brand_name,
                     'business_reg_no'            : outlet.business_reg_no,
@@ -85,25 +86,28 @@
                     'email'                      : outlet.email,
                     'phone'                      : outlet.office_phone,
                     'website'                    : merchant_acct.website or '',  
                         
                     }
     
     program_configurations = {
-                            'prepaid_configuration': merchant_acct.prepaid_configuration,
+                            'prepaid_configuration' : merchant_acct.prepaid_configuration,
+                            'days_of_return_policy' : merchant_acct.program_settings.get('days_of_return_policy'),
                             }
     
     setting =  {
                 'company_name'                      : merchant_acct.company_name,
                 'website'                           : merchant_acct.website,
                 'account_id'                        : merchant_acct.key_in_str,
                 'api_key'                           : merchant_acct.api_key,
                 'logo_image_url'                    : merchant_acct.logo_public_url,
                 'account_settings'                  : account_settings,
                 'outlet_details'                    : outlet_details,
                 'program_configurations'            : program_configurations,
+                'membership_configurations'         : merchant_acct.membership_configuration, 
                 } 
     if device_setting:
         setting['activation_code']  = device_setting.activation_code
         setting['device_name']      = device_setting.device_name
+        setting['device_id']        = device_setting.device_id
         
     return setting
```

### Comparing `trex-model-0.2.9/trexmodel/program_conf.py` & `trex-model-1.0.0/trexmodel/program_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,28 @@
 REWARD_FORMAT_STAMP                     = 'stamp'
 REWARD_FORMAT_CASH                      = 'cash'
 REWARD_FORMAT_VOUCHER                   = 'voucher'
 REWARD_FORMAT_DISCOUNT                  = 'discount'
 REWARD_FORMAT_MIXED                     = 'mixed'
 REWARD_FORMAT_PREPAID                   = 'prepaid'
 
+
 SALES_AMOUNT                            = 'sales_amount'
 
 REWARD_FORMAT_SET                       = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP, REWARD_FORMAT_CASH, REWARD_FORMAT_VOUCHER, REWARD_FORMAT_MIXED, REWARD_FORMAT_PREPAID)
 BASIC_TYPE_REWARD_FORMAT                = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP)
 
 SUPPORT_TIER_REWARD_PROGRAM_CONDITION_REWARD_FORMAT = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP)
 
 ENTITLE_REWARD_CONDITION_ACCUMULATE_POINT           = 'acc_point'
 ENTITLE_REWARD_CONDITION_ACCUMULATE_STAMP           = 'acc_stamp'
 ENTITLE_REWARD_CONDITION_ACCUMULATE_SALES_AMOUNT    = 'acc_sales'
 
+ENTITLE_REWARD_CONDITION_ACCUMULATE_TYPES           = (ENTITLE_REWARD_CONDITION_ACCUMULATE_POINT, ENTITLE_REWARD_CONDITION_ACCUMULATE_STAMP, ENTITLE_REWARD_CONDITION_ACCUMULATE_SALES_AMOUNT)
+
 PROGRAM_STATUS_PROGRAM_BASE             = 'program_base'
 PROGRAM_STATUS_REWARD_SCHEME            = 'reward_scheme'
 PROGRAM_STATUS_REWARD_DETAILS           = 'reward_details'
 PROGRAM_STATUS_DEFINE_TIER              = 'define_program_tier'
 PROGRAM_STATUS_DEFINE_REWARD            = 'define_reward'
 PROGRAM_STATUS_REWARD_EXCLUSIVITY       = 'exclusivity'
 PROGRAM_STATUS_REVIEW                   = 'review'
@@ -56,14 +59,15 @@
 PROGRAM_REWARD_GIVEAWAY_METHOD_AUTO     = 'auto'
 PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL   = 'manual'
 PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM   = 'system'
 PROGRAM_REWARD_GIVEAWAY_METHOD_TIER     = 'tier'
 
 GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP        = 'new_membership'
 GIVEAWAY_SYSTEM_CONDITION_RENEW_MEMBERSHIP      = 'renew_membership'
+GIVEAWAY_SYSTEM_CONDITION_MEMBERSHIP_YEAR       = 'membership_year'
 
 GIVEAWAY_SYSTEM_CONDITION_FOR_MEMBERSHIP        = (GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP, GIVEAWAY_SYSTEM_CONDITION_RENEW_MEMBERSHIP)
 
 '''
 BASIC_REWARD_PROGRAM_STATUS                          = OrderedSet([PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_REWARD_SCHEME, 
                                                                   PROGRAM_STATUS_REWARD_EXCLUSIVITY,
@@ -173,14 +177,15 @@
 REWARD_LIMIT_TYPE_BY_MONTH                  = 'limit_by_month'
 REWARD_LIMIT_TYPE_BY_WEEK                   = 'limit_by_week'
 REWARD_LIMIT_TYPE_BY_DAY                    = 'limit_by_day'
 
 MEMBERSHIP_EXPIRATION_TYPE_AFTER_YEAR       = 'year'
 MEMBERSHIP_EXPIRATION_TYPE_AFTER_MONTH      = 'month'
 MEMBERSHIP_EXPIRATION_TYPE_AFTER_WEEK       = 'week'
+MEMBERSHIP_EXPIRATION_TYPE_AFTER_DAY        = 'day'
 MEMBERSHIP_EXPIRATION_TYPE_SPECIFIC_DATE    = 'date'
 MEMBERSHIP_EXPIRATION_TYPE_NO_EXPIRY        = 'no_expiry'
 
 MEMBERSHIP_EFFECTIVE_TYPE_IMMEDIATE         = 'immediate'
 MEMBERSHIP_EFFECTIVE_TYPE_SPECIFIC_DATE     = 'date'
 MEMBERSHIP_EFFECTIVE_TYPE_AFTER_DAY         = 'day'
 
@@ -211,14 +216,19 @@
 REWARD_STATUS_REDEEMED     = 'redeemed'
 REWARD_STATUS_REVERTED     = 'reverted'
 REWARD_STATUS_REMOVED      = 'removed'
 
 REDEEM_STATUS_VALID        = 'valid'
 REDEEM_STATUS_REVERTED     = 'reverted'
 
+TIER_MEMBERSHIP_STATUS_ACTIVE           = 'active'
+TIER_MEMBERSHIP_STATUS_UPGRADED         = 'upgraded'
+
+
+
 
 REDEEM_CODE_LENGTH                                                  = 12
 
 MAX_REWARD_AMOUNT           = 999999999
 
 def get_program_completed_status_index(completed_status):
     return BASIC_REWARD_PROGRAM_STATUS.index(completed_status)
```

### Comparing `trex-model-0.2.9/trexmodel/utils/model/model_util.py` & `trex-model-1.0.0/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

