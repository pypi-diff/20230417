# Comparing `tmp/ynab-sdk-0.4.0.tar.gz` & `tmp/ynab-sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab-sdk-0.4.0.tar", last modified: Wed Feb 22 14:56:04 2023, max compression
+gzip compressed data, was "ynab-sdk-0.5.0.tar", last modified: Sun Apr 16 23:44:09 2023, max compression
```

## Comparing `ynab-sdk-0.4.0.tar` & `ynab-sdk-0.5.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.371619 ynab-sdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-02-22 14:56:04.371619 ynab-sdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-22 14:56:04.371619 ynab-sdk-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/dummy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/support/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/payees.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/fixtures/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/support/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/test_budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/test_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/test_payees.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_api/test_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/test/test_utils/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_utils/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_utils/clients/test_cached_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_utils/clients/test_default_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/test/test_ynab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/ynab_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/ynab_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/categories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/ynab_sdk/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/ynab_sdk/api/models/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/requests/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/requests/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.367619 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/payee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/payees.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/models/responses/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/payees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/api/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.367619 ynab-sdk-0.4.0/ynab_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.367619 ynab-sdk-0.4.0/ynab_sdk/utils/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/clients/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/clients/cached_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/clients/default_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.371619 ynab-sdk-0.4.0/ynab_sdk/utils/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/configurations/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/configurations/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/utils/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-22 14:55:54.000000 ynab-sdk-0.4.0/ynab_sdk/ynab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:56:04.363619 ynab-sdk-0.4.0/ynab_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-02-22 14:56:04.000000 ynab-sdk-0.4.0/ynab_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-02-22 14:56:04.000000 ynab-sdk-0.4.0/ynab_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 14:56:04.000000 ynab-sdk-0.4.0/ynab_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-22 14:56:04.000000 ynab-sdk-0.4.0/ynab_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 14:56:04.000000 ynab-sdk-0.4.0/ynab_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/dummy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/support/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/payees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/fixtures/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/support/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/test_budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/test_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/test_payees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_api/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.814678 ynab-sdk-0.5.0/test/test_utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_utils/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_utils/clients/test_cached_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_utils/clients/test_default_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/test/test_ynab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.818678 ynab-sdk-0.5.0/ynab_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.818678 ynab-sdk-0.5.0/ynab_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/categories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.818678 ynab-sdk-0.5.0/ynab_sdk/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.818678 ynab-sdk-0.5.0/ynab_sdk/api/models/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/requests/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/requests/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/payee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/payees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/models/responses/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/payees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/api/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/ynab_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/ynab_sdk/utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/clients/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/clients/cached_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/clients/default_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.822678 ynab-sdk-0.5.0/ynab_sdk/utils/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/configurations/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/configurations/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/utils/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-16 23:43:59.000000 ynab-sdk-0.5.0/ynab_sdk/ynab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:44:09.818678 ynab-sdk-0.5.0/ynab_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-04-16 23:44:09.000000 ynab-sdk-0.5.0/ynab_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-16 23:44:09.000000 ynab-sdk-0.5.0/ynab_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:44:09.000000 ynab-sdk-0.5.0/ynab_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 23:44:09.000000 ynab-sdk-0.5.0/ynab_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 23:44:09.000000 ynab-sdk-0.5.0/ynab_sdk.egg-info/top_level.txt
```

### Comparing `ynab-sdk-0.4.0/LICENSE` & `ynab-sdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/PKG-INFO` & `ynab-sdk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: ynab-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: YNAB API Endpoints
 Home-page: https://github.com/andreroggeri/ynab-sdk-python
 Author-email: a.roggeri.c@gmail.com
 Keywords: YNAB,YNAB API Endpoints,
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ynab-sdk-python
 
 [![PyPI version](https://badge.fury.io/py/ynab-sdk.svg)](https://badge.fury.io/py/ynab-sdk)
 [![Maintainability](https://api.codeclimate.com/v1/badges/b6042768d805939000c2/maintainability)](https://codeclimate.com/github/andreroggeri/ynab-sdk-python/maintainability)
-[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
+[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/main/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python implementation of the YNAB API ([https://api.youneedabudget.com/](https://api.youneedabudget.com/))
 
-## Warning
-
-This is pretty much a work in progress, the basic stuff is working, but nothing is guaranteed.
-See below whats implemented and whats not
-
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install `ynab-sdk-python`
 
 ```bash
 pip install ynab-sdk
 ```
```

### Comparing `ynab-sdk-0.4.0/README.md` & `ynab-sdk-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # ynab-sdk-python
 
 [![PyPI version](https://badge.fury.io/py/ynab-sdk.svg)](https://badge.fury.io/py/ynab-sdk)
 [![Maintainability](https://api.codeclimate.com/v1/badges/b6042768d805939000c2/maintainability)](https://codeclimate.com/github/andreroggeri/ynab-sdk-python/maintainability)
-[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
+[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/main/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python implementation of the YNAB API ([https://api.youneedabudget.com/](https://api.youneedabudget.com/))
 
-## Warning
-
-This is pretty much a work in progress, the basic stuff is working, but nothing is guaranteed.
-See below whats implemented and whats not
-
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install `ynab-sdk-python`
 
 ```bash
 pip install ynab-sdk
 ```
```

### Comparing `ynab-sdk-0.4.0/setup.py` & `ynab-sdk-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_packages, setup
 
 NAME = "ynab-sdk"
-VERSION = "0.4.0"
+VERSION = "0.5.0"
 REQUIRES = ["requests", "python-dateutil", "redis"]
 
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
```

### Comparing `ynab-sdk-0.4.0/test/support/dummy_client.py` & `ynab-sdk-0.5.0/test/support/dummy_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/support/fixtures/accounts.py` & `ynab-sdk-0.5.0/test/support/fixtures/accounts.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/support/fixtures/budgets.py` & `ynab-sdk-0.5.0/test/support/fixtures/budgets.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/support/fixtures/categories.py` & `ynab-sdk-0.5.0/test/support/fixtures/categories.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_api/test_accounts.py` & `ynab-sdk-0.5.0/test/test_api/test_accounts.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_api/test_budgets.py` & `ynab-sdk-0.5.0/test/test_api/test_budgets.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_api/test_categories.py` & `ynab-sdk-0.5.0/test/test_api/test_categories.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_api/test_payees.py` & `ynab-sdk-0.5.0/test/test_api/test_payees.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_api/test_transactions.py` & `ynab-sdk-0.5.0/test/test_api/test_transactions.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,18 @@
         self.assertTrue(
             spy.called_with("/budgets/some-budget/accounts/some-account/transactions")
         )
         self.assertIsNotNone(transactions)
         self.assertIsInstance(transactions, TransactionsResponse)
 
     def test_create_transactions_with_success(self):
-        spy = self.spy_on(self.client.post, call_fake=build_post_mock())
+        spy = self.spy_on(
+            self.client.post,
+            call_fake=build_post_mock(transaction_fixtures.CREATED_TRANSACTIONS),
+        )
         transactions = [TransactionRequest("some-account", "some-date", 123123)]
         response = self.ynab.transactions.create_transactions(
             "some-budget", transactions
         )
 
         payload = {"transactions": [dataclasses.asdict(t) for t in transactions]}
```

### Comparing `ynab-sdk-0.4.0/test/test_utils/clients/test_cached_client.py` & `ynab-sdk-0.5.0/test/test_utils/clients/test_cached_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/test/test_utils/clients/test_default_client.py` & `ynab-sdk-0.5.0/test/test_utils/clients/test_default_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/accounts.py` & `ynab-sdk-0.5.0/ynab_sdk/api/accounts.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/budgets.py` & `ynab-sdk-0.5.0/ynab_sdk/api/budgets.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/categories.py` & `ynab-sdk-0.5.0/ynab_sdk/api/categories.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/account.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/account.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/accounts.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/accounts.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_detail.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_settings.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_settings.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/budget_summary.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/budget_summary.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/categories.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/categories.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/category.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/category.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/payee.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/payee.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/payees.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/payees.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/models/responses/transactions.py` & `ynab-sdk-0.5.0/ynab_sdk/api/models/responses/transactions.py`

 * *Files 17% similar despite different names*

```diff
@@ -129,7 +129,32 @@
     data: Data
 
     @staticmethod
     def from_dict(obj: Any) -> "TransactionsResponse":
         assert isinstance(obj, dict)
         data = Data.from_dict(obj.get("data"))
         return TransactionsResponse(data)
+
+
+@dataclass
+class CreateTransactionResponse:
+    transaction_ids: List[str]
+    transactions: List[Transaction]
+    duplicate_import_ids: List[str]
+
+    @staticmethod
+    def from_dict(obj: Any) -> "CreateTransactionResponse":
+        assert isinstance(obj, dict)
+        data = obj.get("data")
+        transaction_ids = parsers.from_list(
+            parsers.from_str, data.get("transaction_ids")
+        )
+        transactions = parsers.from_list(
+            Transaction.from_dict, data.get("transactions")
+        )
+        duplicate_import_ids = parsers.from_list(
+            parsers.from_str, data.get("duplicate_import_ids")
+        )
+
+        return CreateTransactionResponse(
+            transaction_ids, transactions, duplicate_import_ids
+        )
```

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/payees.py` & `ynab-sdk-0.5.0/ynab_sdk/api/payees.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/api/transactions.py` & `ynab-sdk-0.5.0/ynab_sdk/api/transactions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import dataclasses
 from typing import List
 
 from ynab_sdk.api.models.requests.transaction import TransactionRequest
-from ynab_sdk.api.models.responses.transactions import TransactionsResponse
+from ynab_sdk.api.models.responses.transactions import (
+    TransactionsResponse,
+    CreateTransactionResponse,
+)
 from ynab_sdk.utils.clients.base_client import BaseClient
 
 
 class TransactionsApi:
     def __init__(self, client: BaseClient):
         self.client = client
 
@@ -22,15 +25,17 @@
         )
         return TransactionsResponse.from_dict(response)
 
     def create_transactions(
         self, budget_id: str, transactions: List[TransactionRequest]
     ):
         payload = {"transactions": [dataclasses.asdict(t) for t in transactions]}
-        return self.client.post(f"/budgets/{budget_id}/transactions", payload)
+        response = self.client.post(f"/budgets/{budget_id}/transactions", payload)
+
+        return CreateTransactionResponse.from_dict(response)
 
     def update_transaction(
         self, budget_id: str, transaction_id: str, transaction: TransactionRequest
     ):
         payload = {"transaction": dataclasses.asdict(transaction)}
         return self.client.put(
             f"/budgets/{budget_id}/transactions/{transaction_id}", payload
```

### Comparing `ynab-sdk-0.4.0/ynab_sdk/utils/clients/base_client.py` & `ynab-sdk-0.5.0/ynab_sdk/utils/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/utils/clients/cached_client.py` & `ynab-sdk-0.5.0/ynab_sdk/utils/clients/cached_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/utils/clients/default_client.py` & `ynab-sdk-0.5.0/ynab_sdk/utils/clients/default_client.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/utils/configurations/cached.py` & `ynab-sdk-0.5.0/ynab_sdk/utils/configurations/cached.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/utils/parsers.py` & `ynab-sdk-0.5.0/ynab_sdk/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk/ynab.py` & `ynab-sdk-0.5.0/ynab_sdk/ynab.py`

 * *Files identical despite different names*

### Comparing `ynab-sdk-0.4.0/ynab_sdk.egg-info/PKG-INFO` & `ynab-sdk-0.5.0/ynab_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: ynab-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: YNAB API Endpoints
 Home-page: https://github.com/andreroggeri/ynab-sdk-python
 Author-email: a.roggeri.c@gmail.com
 Keywords: YNAB,YNAB API Endpoints,
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ynab-sdk-python
 
 [![PyPI version](https://badge.fury.io/py/ynab-sdk.svg)](https://badge.fury.io/py/ynab-sdk)
 [![Maintainability](https://api.codeclimate.com/v1/badges/b6042768d805939000c2/maintainability)](https://codeclimate.com/github/andreroggeri/ynab-sdk-python/maintainability)
-[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
+[![codecov](https://codecov.io/gh/andreroggeri/ynab-sdk-python/branch/main/graph/badge.svg)](https://codecov.io/gh/andreroggeri/ynab-sdk-python)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python implementation of the YNAB API ([https://api.youneedabudget.com/](https://api.youneedabudget.com/))
 
-## Warning
-
-This is pretty much a work in progress, the basic stuff is working, but nothing is guaranteed.
-See below whats implemented and whats not
-
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install `ynab-sdk-python`
 
 ```bash
 pip install ynab-sdk
 ```
```

### Comparing `ynab-sdk-0.4.0/ynab_sdk.egg-info/SOURCES.txt` & `ynab-sdk-0.5.0/ynab_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

