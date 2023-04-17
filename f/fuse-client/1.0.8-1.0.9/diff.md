# Comparing `tmp/fuse-client-1.0.8.tar.gz` & `tmp/fuse-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuse-client-1.0.8.tar", last modified: Tue Apr 11 12:12:53 2023, max compression
+gzip compressed data, was "fuse-client-1.0.9.tar", last modified: Tue Apr 11 12:29:16 2023, max compression
```

## Comparing `fuse-client-1.0.8.tar` & `fuse-client-1.0.9.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327831 fuse-client-1.0.8/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.8/LICENSE
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:12:53.327918 fuse-client-1.0.8/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.8/README.md
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.285382 fuse-client-1.0.8/fuse_client/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      755 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    58516 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/api_client.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.286831 fuse-client-1.0.8/fuse_client/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      214 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5677 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/path_to_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.289858 fuse-client-1.0.8/fuse_client/apis/paths/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      238 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      113 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      126 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report_create.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      128 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_asset_report_refresh.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      121 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_entities_entity_id.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_accounts.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      163 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_accounts_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      173 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_financial_connection_id.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      200 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_financial_connection_id_to_delete.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      181 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_institutions_institution_id.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      171 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_investments_holdings.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      179 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_investments_transactions.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      154 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_liabilities.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      146 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_migrate.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      144 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_owners.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      172 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_public_token_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      140 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_sync.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      156 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_financial_connections_transactions.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      109 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_link_token.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      104 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/paths/v1_session.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      296 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tag_to_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.290106 fuse-client-1.0.8/fuse_client/apis/tags/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      302 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tags/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2958 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/apis/tags/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    20767 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/configuration.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4542 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/exceptions.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303387 fuse-client-1.0.8/fuse_client/model/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    20979 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1731 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1316 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1065 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4096 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3792 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5853 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10013 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3128 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8645 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3744 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2909 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3960 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3365 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2577 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3988 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3064 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    16866 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8918 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5102 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4394 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     7342 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14140 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5892 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9498 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10325 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    31683 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11085 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    15913 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    17374 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    33113 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8247 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3437 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2630 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5197 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5016 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6638 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4222 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2614 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9445 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5285 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4863 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3402 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6620 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5739 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9233 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     7099 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2584 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4186 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8943 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8395 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5129 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1669 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     4432 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3049 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10548 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)   164458 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     5400 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6464 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1425 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1673 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/model/webhook_type.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303516 fuse-client-1.0.8/fuse_client/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     6216 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/models/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.303648 fuse-client-1.0.8/fuse_client/paths/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1863 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304012 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      311 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304322 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      325 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11981 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304607 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      327 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11999 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.304926 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      323 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.305340 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12002 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.305808 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      363 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12151 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306281 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11994 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306658 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      377 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9986 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.306994 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      397 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10107 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/delete.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.307370 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      385 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     9935 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.307985 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      371 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308283 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      379 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308569 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      353 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11951 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.308898 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12259 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309370 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      343 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11966 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309649 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      373 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12475 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.309963 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      339 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12200 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310335 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      355 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    12090 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310620 fuse-client-1.0.8/fuse_client/paths/v1_link_token/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      307 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_link_token/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11939 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_link_token/post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.310883 fuse-client-1.0.8/fuse_client/paths/v1_session/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      301 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_session/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    11881 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/paths/v1_session/post.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    10567 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/rest.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    97672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/fuse_client/schemas.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.286416 fuse-client-1.0.8/fuse_client.egg-info/
--rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    14209 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/SOURCES.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/dependency_links.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)      118 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/requires.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       17 2023-04-11 12:12:53.000000 fuse-client-1.0.8/fuse_client.egg-info/top_level.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 12:12:53.328200 fuse-client-1.0.8/setup.cfg
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 12:12:22.000000 fuse-client-1.0.8/setup.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.281176 fuse-client-1.0.8/test/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321352 fuse-client-1.0.8/test/test_models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      581 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      564 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      623 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      619 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      556 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      548 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      713 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      717 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      630 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      671 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      679 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      691 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      626 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      605 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      574 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      582 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      611 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      594 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      647 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      705 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      709 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      696 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      700 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      651 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      639 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      643 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      655 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      614 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      733 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      552 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      622 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      568 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_models/test_webhook_type.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321545 fuse-client-1.0.8/test/test_paths/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1995 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.321833 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      772 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322113 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      791 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322444 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      794 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.322799 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/test_get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.323288 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.323656 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324013 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324308 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/test_get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324634 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.324930 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      924 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325221 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325505 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      922 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325744 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      873 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.325990 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      872 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326300 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326571 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      859 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.326819 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      868 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327074 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      877 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327376 fuse-client-1.0.8/test/test_paths/test_v1_link_token/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_link_token/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      766 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_link_token/test_post.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:53.327660 fuse-client-1.0.8/test/test_paths/test_v1_session/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_session/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      759 2023-04-11 12:12:22.000000 fuse-client-1.0.8/test/test_paths/test_v1_session/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.174131 fuse-client-1.0.9/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse-client-1.0.9/LICENSE
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:29:16.174200 fuse-client-1.0.9/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    19269 2023-04-11 09:24:51.000000 fuse-client-1.0.9/README.md
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.143124 fuse-client-1.0.9/fuse_client/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      755 2023-04-11 12:29:09.000000 fuse-client-1.0.9/fuse_client/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    58516 2023-04-11 12:29:09.000000 fuse-client-1.0.9/fuse_client/api_client.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.144071 fuse-client-1.0.9/fuse_client/apis/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      214 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5677 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/path_to_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.146470 fuse-client-1.0.9/fuse_client/apis/paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      238 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      113 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_asset_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      126 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_asset_report_create.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      128 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_asset_report_refresh.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      121 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_entities_entity_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_accounts.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      163 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_accounts_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      148 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      173 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_financial_connection_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      200 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_financial_connection_id_to_delete.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      181 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_institutions_institution_id.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      171 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_investments_holdings.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      179 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_investments_transactions.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      154 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_liabilities.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      146 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_migrate.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      144 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_owners.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      172 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_public_token_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      140 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_sync.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      156 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_financial_connections_transactions.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      109 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_link_token.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      104 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/paths/v1_session.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      296 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/tag_to_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.146678 fuse-client-1.0.9/fuse_client/apis/tags/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      302 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/tags/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2958 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/apis/tags/fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    20767 2023-04-11 12:29:09.000000 fuse-client-1.0.9/fuse_client/configuration.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4542 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/exceptions.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.155516 fuse-client-1.0.9/fuse_client/model/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    20979 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1731 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1316 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1065 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4096 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3792 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5853 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10013 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3128 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8645 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3744 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2909 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3960 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3365 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2577 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3988 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3064 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    16866 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8918 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5102 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4394 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     7342 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14140 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5892 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9498 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10325 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    31683 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11085 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    15913 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    17374 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2680 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    33113 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8247 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3437 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2630 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5197 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2618 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5016 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6638 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4222 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2614 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9445 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5285 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4863 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3402 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6620 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5739 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9233 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     7099 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2584 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4186 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8943 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8395 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5129 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1669 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     4432 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3049 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3602 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10548 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)   164458 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     5400 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6412 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6464 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1425 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1673 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/model/webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.155618 fuse-client-1.0.9/fuse_client/models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6216 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/models/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.155724 fuse-client-1.0.9/fuse_client/paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1863 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.155941 fuse-client-1.0.9/fuse_client/paths/v1_asset_report/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      311 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11918 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.156151 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_create/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      325 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_create/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11981 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_create/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.156361 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_refresh/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      327 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_refresh/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11999 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_asset_report_refresh/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.156576 fuse-client-1.0.9/fuse_client/paths/v1_entities_entity_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      323 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_entities_entity_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9676 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_entities_entity_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.156794 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12002 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.157001 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts_details/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      363 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts_details/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12151 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts_details/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.157208 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_balances/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      347 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_balances/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11994 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_balances/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.157423 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      377 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9986 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.157642 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      397 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10107 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/delete.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.157851 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_institutions_institution_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      385 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_institutions_institution_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     9935 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_institutions_institution_id/get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.158066 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_holdings/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      371 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_holdings/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11787 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_holdings/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.158281 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      379 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11875 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_transactions/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.158499 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_liabilities/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      353 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_liabilities/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11951 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_liabilities/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.158709 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_migrate/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      345 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_migrate/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12259 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_migrate/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.158915 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_owners/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      343 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_owners/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11966 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_owners/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.159121 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_public_token_exchange/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      373 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_public_token_exchange/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12475 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_public_token_exchange/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.159324 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_sync/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      339 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_sync/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12200 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_sync/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.159534 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      355 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    12090 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_transactions/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.159732 fuse-client-1.0.9/fuse_client/paths/v1_link_token/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      307 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_link_token/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11939 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_link_token/post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.159939 fuse-client-1.0.9/fuse_client/paths/v1_session/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      301 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_session/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    11881 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/paths/v1_session/post.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    10567 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/rest.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    97672 2023-04-11 12:12:22.000000 fuse-client-1.0.9/fuse_client/schemas.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.143753 fuse-client-1.0.9/fuse_client.egg-info/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      370 2023-04-11 12:29:16.000000 fuse-client-1.0.9/fuse_client.egg-info/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    14209 2023-04-11 12:29:16.000000 fuse-client-1.0.9/fuse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-11 12:29:16.000000 fuse-client-1.0.9/fuse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      118 2023-04-11 12:29:16.000000 fuse-client-1.0.9/fuse_client.egg-info/requires.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       17 2023-04-11 12:29:16.000000 fuse-client-1.0.9/fuse_client.egg-info/top_level.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       69 2023-04-11 12:29:16.174453 fuse-client-1.0.9/setup.cfg
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1212 2023-04-11 12:29:09.000000 fuse-client-1.0.9/setup.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.140058 fuse-client-1.0.9/test/
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.168855 fuse-client-1.0.9/test/test_models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      581 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      564 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      623 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      619 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      556 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      548 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      713 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      717 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      630 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      663 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      671 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      634 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      679 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      691 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      626 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      605 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      574 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      582 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      611 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      615 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      594 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      647 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      705 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      709 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      680 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      676 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      696 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      700 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      651 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      639 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      643 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      655 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      659 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      610 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      614 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      733 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      684 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      688 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      552 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      627 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      618 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      622 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      568 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      602 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      606 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      569 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_models/test_webhook_type.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.168981 fuse-client-1.0.9/test/test_paths/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1995 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/__init__.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.169249 fuse-client-1.0.9/test/test_paths/test_v1_asset_report/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      772 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.169460 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_create/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_create/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      791 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_create/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.169704 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_refresh/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_refresh/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      794 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_asset_report_refresh/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.169935 fuse-client-1.0.9/test/test_paths/test_v1_entities_entity_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_entities_entity_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_entities_entity_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.170170 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.170410 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts_details/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts_details/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts_details/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.170662 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_balances/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_balances/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_balances/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.170963 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.171231 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      949 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.171487 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_institutions_institution_id/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_institutions_institution_id/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      924 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.171747 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_holdings/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_holdings/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      906 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.172007 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      922 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_transactions/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.172297 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_liabilities/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_liabilities/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      873 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_liabilities/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.172493 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_migrate/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_migrate/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      872 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_migrate/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.172712 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_owners/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_owners/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      861 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_owners/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.172972 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_public_token_exchange/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_public_token_exchange/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      859 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_public_token_exchange/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.173215 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_sync/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_sync/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      868 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_sync/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.173507 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_transactions/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_transactions/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      877 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_transactions/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.173733 fuse-client-1.0.9/test/test_paths/test_v1_link_token/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_link_token/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      766 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_link_token/test_post.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:29:16.173982 fuse-client-1.0.9/test/test_paths/test_v1_session/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_session/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      759 2023-04-11 12:12:22.000000 fuse-client-1.0.9/test/test_paths/test_v1_session/test_post.py
```

### Comparing `fuse-client-1.0.8/LICENSE` & `fuse-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/README.md` & `fuse-client-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/__init__.py` & `fuse-client-1.0.9/fuse_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # import ApiClient
 from fuse_client.api_client import ApiClient
 
 # import Configuration
 from fuse_client.configuration import Configuration
```

### Comparing `fuse-client-1.0.8/fuse_client/api_client.py` & `fuse-client-1.0.9/fuse_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `fuse-client-1.0.8/fuse_client/apis/path_to_api.py` & `fuse-client-1.0.9/fuse_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/apis/tags/fuse_api.py` & `fuse-client-1.0.9/fuse_client/apis/tags/fuse_api.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/configuration.py` & `fuse-client-1.0.9/fuse_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.8".\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fuse-client-1.0.8/fuse_client/exceptions.py` & `fuse-client-1.0.9/fuse_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/account_subtype.py` & `fuse-client-1.0.9/fuse_client/model/account_subtype.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/account_type.py` & `fuse-client-1.0.9/fuse_client/model/account_type.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/aggregator.py` & `fuse-client-1.0.9/fuse_client/model/aggregator.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/country_code.py` & `fuse-client-1.0.9/fuse_client/model/country_code.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_asset_report_request.py` & `fuse-client-1.0.9/fuse_client/model/create_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_asset_report_response.py` & `fuse-client-1.0.9/fuse_client/model/create_asset_report_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_entity_request.py` & `fuse-client-1.0.9/fuse_client/model/create_entity_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_entity_response.py` & `fuse-client-1.0.9/fuse_client/model/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_link_token_request.py` & `fuse-client-1.0.9/fuse_client/model/create_link_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_link_token_response.py` & `fuse-client-1.0.9/fuse_client/model/create_link_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_session_request.py` & `fuse-client-1.0.9/fuse_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/create_session_response.py` & `fuse-client-1.0.9/fuse_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/currency.py` & `fuse-client-1.0.9/fuse_client/model/currency.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/delete_financial_connection_response.py` & `fuse-client-1.0.9/fuse_client/model/delete_financial_connection_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/entity.py` & `fuse-client-1.0.9/fuse_client/model/entity.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.9/fuse_client/model/exchange_financial_connections_public_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/exchange_financial_connections_public_token_response.py` & `fuse-client-1.0.9/fuse_client/model/exchange_financial_connections_public_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connection_data.py` & `fuse-client-1.0.9/fuse_client/model/financial_connection_data.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connection_details.py` & `fuse-client-1.0.9/fuse_client/model/financial_connection_details.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_account.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_account.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_account_balance.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_account_balance.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_account_cached_balance.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_account_cached_balance.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_account_details.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_account_details.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_account_liability.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_account_liability.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_holding.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_holding.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_investment_security.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_investment_security.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_investment_transaction.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_investment_transaction.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_connections_owner.py` & `fuse-client-1.0.9/fuse_client/model/financial_connections_owner.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/financial_institution.py` & `fuse-client-1.0.9/fuse_client/model/financial_institution.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/fuse_api_error.py` & `fuse-client-1.0.9/fuse_client/model/fuse_api_error.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/fuse_api_warning.py` & `fuse-client-1.0.9/fuse_client/model/fuse_api_warning.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_asset_report_request.py` & `fuse-client-1.0.9/fuse_client/model/get_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_asset_report_response.py` & `fuse-client-1.0.9/fuse_client/model/get_asset_report_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_entity_response.py` & `fuse-client-1.0.9/fuse_client/model/get_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connection_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connection_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_request.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_account_details_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_account_details_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_account_details_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_request.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_accounts_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_accounts_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_request.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_balance_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_balance_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_balance_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_request.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_owners_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_owners_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_owners_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_request.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_connections_transactions_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_connections_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_financial_institution_response.py` & `fuse-client-1.0.9/fuse_client/model/get_financial_institution_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_investment_holdings_request.py` & `fuse-client-1.0.9/fuse_client/model/get_investment_holdings_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_investment_holdings_response.py` & `fuse-client-1.0.9/fuse_client/model/get_investment_holdings_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_investment_transactions_request.py` & `fuse-client-1.0.9/fuse_client/model/get_investment_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_investment_transactions_response.py` & `fuse-client-1.0.9/fuse_client/model/get_investment_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_liabilities_request.py` & `fuse-client-1.0.9/fuse_client/model/get_liabilities_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/get_liabilities_response.py` & `fuse-client-1.0.9/fuse_client/model/get_liabilities_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py` & `fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_aggregator_connection_data.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_request.py` & `fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/migrate_financial_connections_token_response.py` & `fuse-client-1.0.9/fuse_client/model/migrate_financial_connections_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/product.py` & `fuse-client-1.0.9/fuse_client/model/product.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/refresh_asset_report_request.py` & `fuse-client-1.0.9/fuse_client/model/refresh_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/sync_financial_connections_data_response.py` & `fuse-client-1.0.9/fuse_client/model/sync_financial_connections_data_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/sync_transactions_request.py` & `fuse-client-1.0.9/fuse_client/model/sync_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/sync_transactions_response.py` & `fuse-client-1.0.9/fuse_client/model/sync_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/transaction.py` & `fuse-client-1.0.9/fuse_client/model/transaction.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/update_entity_request.py` & `fuse-client-1.0.9/fuse_client/model/update_entity_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/update_entity_response.py` & `fuse-client-1.0.9/fuse_client/model/update_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/webhook_event.py` & `fuse-client-1.0.9/fuse_client/model/webhook_event.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/webhook_source.py` & `fuse-client-1.0.9/fuse_client/model/webhook_source.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/model/webhook_type.py` & `fuse-client-1.0.9/fuse_client/model/webhook_type.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/models/__init__.py` & `fuse-client-1.0.9/fuse_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/__init__.py` & `fuse-client-1.0.9/fuse_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_asset_report/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_asset_report/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_asset_report_create/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_asset_report_create/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_asset_report_refresh/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_asset_report_refresh/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_entities_entity_id/get.py` & `fuse-client-1.0.9/fuse_client/paths/v1_entities_entity_id/get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_accounts_details/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_accounts_details/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_balances/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_balances/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id/get.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id/get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/delete.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_financial_connection_id_to_delete/delete.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_institutions_institution_id/get.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_institutions_institution_id/get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_holdings/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_holdings/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_investments_transactions/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_investments_transactions/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_liabilities/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_liabilities/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_migrate/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_migrate/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_owners/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_owners/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_public_token_exchange/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_public_token_exchange/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_sync/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_sync/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_financial_connections_transactions/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_financial_connections_transactions/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_link_token/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_link_token/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/paths/v1_session/post.py` & `fuse-client-1.0.9/fuse_client/paths/v1_session/post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/rest.py` & `fuse-client-1.0.9/fuse_client/rest.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client/schemas.py` & `fuse-client-1.0.9/fuse_client/schemas.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/fuse_client.egg-info/SOURCES.txt` & `fuse-client-1.0.9/fuse_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/setup.py` & `fuse-client-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "fuse-client"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fuse-client-1.0.8/test/test_models/test_account_subtype.py` & `fuse-client-1.0.9/test/test_models/test_account_subtype.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_account_type.py` & `fuse-client-1.0.9/test/test_models/test_account_type.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_aggregator.py` & `fuse-client-1.0.9/test/test_models/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_country_code.py` & `fuse-client-1.0.9/test/test_models/test_country_code.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_asset_report_request.py` & `fuse-client-1.0.9/test/test_models/test_create_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_asset_report_response.py` & `fuse-client-1.0.9/test/test_models/test_create_asset_report_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_entity_request.py` & `fuse-client-1.0.9/test/test_models/test_create_entity_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_entity_response.py` & `fuse-client-1.0.9/test/test_models/test_create_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_link_token_request.py` & `fuse-client-1.0.9/test/test_models/test_create_link_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_link_token_response.py` & `fuse-client-1.0.9/test/test_models/test_create_link_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_session_request.py` & `fuse-client-1.0.9/test/test_models/test_create_session_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_create_session_response.py` & `fuse-client-1.0.9/test/test_models/test_create_session_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_currency.py` & `fuse-client-1.0.9/test/test_models/test_currency.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_delete_financial_connection_response.py` & `fuse-client-1.0.9/test/test_models/test_delete_financial_connection_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_entity.py` & `fuse-client-1.0.9/test/test_models/test_entity.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_request.py` & `fuse-client-1.0.9/test/test_models/test_exchange_financial_connections_public_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_exchange_financial_connections_public_token_response.py` & `fuse-client-1.0.9/test/test_models/test_exchange_financial_connections_public_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connection_data.py` & `fuse-client-1.0.9/test/test_models/test_financial_connection_data.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connection_details.py` & `fuse-client-1.0.9/test/test_models/test_financial_connection_details.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_account.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_account.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_account_balance.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_account_balance.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_account_cached_balance.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_account_cached_balance.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_account_details.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_account_details.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_account_liability.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_account_liability.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_holding.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_holding.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_investment_security.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_investment_security.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_investment_transaction.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_investment_transaction.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_connections_owner.py` & `fuse-client-1.0.9/test/test_models/test_financial_connections_owner.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_financial_institution.py` & `fuse-client-1.0.9/test/test_models/test_financial_institution.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_fuse_api_error.py` & `fuse-client-1.0.9/test/test_models/test_fuse_api_error.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_fuse_api_warning.py` & `fuse-client-1.0.9/test/test_models/test_fuse_api_warning.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_asset_report_request.py` & `fuse-client-1.0.9/test/test_models/test_get_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_asset_report_response.py` & `fuse-client-1.0.9/test/test_models/test_get_asset_report_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_entity_response.py` & `fuse-client-1.0.9/test/test_models/test_get_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connection_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connection_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_request.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_account_details_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_account_details_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_account_details_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_request.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_accounts_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_accounts_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_request.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_balance_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_balance_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_balance_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_request.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_owners_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_owners_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_owners_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_request.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_connections_transactions_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_connections_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_financial_institution_response.py` & `fuse-client-1.0.9/test/test_models/test_get_financial_institution_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_investment_holdings_request.py` & `fuse-client-1.0.9/test/test_models/test_get_investment_holdings_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_investment_holdings_response.py` & `fuse-client-1.0.9/test/test_models/test_get_investment_holdings_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_investment_transactions_request.py` & `fuse-client-1.0.9/test/test_models/test_get_investment_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_investment_transactions_response.py` & `fuse-client-1.0.9/test/test_models/test_get_investment_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_liabilities_request.py` & `fuse-client-1.0.9/test/test_models/test_get_liabilities_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_get_liabilities_response.py` & `fuse-client-1.0.9/test/test_models/test_get_liabilities_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py` & `fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_aggregator_connection_data.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_request.py` & `fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_migrate_financial_connections_token_response.py` & `fuse-client-1.0.9/test/test_models/test_migrate_financial_connections_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_product.py` & `fuse-client-1.0.9/test/test_models/test_product.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_refresh_asset_report_request.py` & `fuse-client-1.0.9/test/test_models/test_refresh_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_sync_financial_connections_data_response.py` & `fuse-client-1.0.9/test/test_models/test_sync_financial_connections_data_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_sync_transactions_request.py` & `fuse-client-1.0.9/test/test_models/test_sync_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_sync_transactions_response.py` & `fuse-client-1.0.9/test/test_models/test_sync_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_transaction.py` & `fuse-client-1.0.9/test/test_models/test_transaction.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_update_entity_request.py` & `fuse-client-1.0.9/test/test_models/test_update_entity_request.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_update_entity_response.py` & `fuse-client-1.0.9/test/test_models/test_update_entity_response.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_webhook_event.py` & `fuse-client-1.0.9/test/test_models/test_webhook_event.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_webhook_source.py` & `fuse-client-1.0.9/test/test_models/test_webhook_source.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_models/test_webhook_type.py` & `fuse-client-1.0.9/test/test_models/test_webhook_type.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/__init__.py` & `fuse-client-1.0.9/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_asset_report/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_asset_report/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_asset_report_create/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_asset_report_create/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_asset_report_refresh/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_asset_report_refresh/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_entities_entity_id/test_get.py` & `fuse-client-1.0.9/test/test_paths/test_v1_entities_entity_id/test_get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_accounts_details/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_accounts_details/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_balances/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_balances/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id/test_get.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id/test_get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_financial_connection_id_to_delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_institutions_institution_id/test_get.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_holdings/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_investments_transactions/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_investments_transactions/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_liabilities/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_liabilities/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_migrate/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_migrate/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_owners/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_owners/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_public_token_exchange/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_public_token_exchange/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_sync/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_sync/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_financial_connections_transactions/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_financial_connections_transactions/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_link_token/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_link_token/test_post.py`

 * *Files identical despite different names*

### Comparing `fuse-client-1.0.8/test/test_paths/test_v1_session/test_post.py` & `fuse-client-1.0.9/test/test_paths/test_v1_session/test_post.py`

 * *Files identical despite different names*

