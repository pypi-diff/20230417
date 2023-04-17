# Comparing `tmp/ravendb-5.2.2.tar.gz` & `tmp/ravendb-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ravendb-5.2.2.tar", last modified: Fri Mar  3 14:30:02 2023, max compression
+gzip compressed data, was "ravendb-5.2.3.tar", last modified: Mon Apr 17 08:22:24 2023, max compression
```

## Comparing `ravendb-5.2.2.tar` & `ravendb-5.2.3.tar`

### file list

```diff
@@ -1,243 +1,242 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.825767 ravendb-5.2.2/
--rw-rw-rw-   0        0        0     1100 2022-05-26 12:42:03.000000 ravendb-5.2.2/LICENSE
--rw-rw-rw-   0        0        0       22 2023-02-08 09:25:35.000000 ravendb-5.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4129 2023-03-03 14:30:02.824767 ravendb-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    40404 2023-03-03 14:09:38.000000 ravendb-5.2.2/README.md
--rw-rw-rw-   0        0        0     3762 2023-03-03 14:09:38.000000 ravendb-5.2.2/README_pypi.md
--rw-rw-rw-   0        0        0       81 2022-05-26 12:42:03.000000 ravendb-5.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.644644 ravendb-5.2.2/ravendb/
--rw-rw-rw-   0        0        0    19779 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.653645 ravendb-5.2.2/ravendb/changes/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/changes/__init__.py
--rw-rw-rw-   0        0        0    16419 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/changes/database_changes.py
--rw-rw-rw-   0        0        0     4356 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/changes/observers.py
--rw-rw-rw-   0        0        0     4938 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/changes/types.py
--rw-rw-rw-   0        0        0     2118 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.657645 ravendb-5.2.2/ravendb/data/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/data/__init__.py
--rw-rw-rw-   0        0        0      163 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/data/operation.py
--rw-rw-rw-   0        0        0     9796 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/data/query.py
--rw-rw-rw-   0        0        0     2466 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/data/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.660645 ravendb-5.2.2/ravendb/documents/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/__init__.py
--rw-rw-rw-   0        0        0    18788 2023-02-15 14:10:24.000000 ravendb-5.2.2/ravendb/documents/bulk_insert_operation.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.668645 ravendb-5.2.2/ravendb/documents/commands/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/__init__.py
--rw-rw-rw-   0        0        0    24381 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/commands/batches.py
--rw-rw-rw-   0        0        0     1290 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/bulkinsert.py
--rw-rw-rw-   0        0        0    17155 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/crud.py
--rw-rw-rw-   0        0        0    10527 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/multi_get.py
--rw-rw-rw-   0        0        0     2263 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/query.py
--rw-rw-rw-   0        0        0     1577 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/results.py
--rw-rw-rw-   0        0        0     8523 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/commands/subscriptions.py
--rw-rw-rw-   0        0        0    19605 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/conventions.py
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/documents.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.670645 ravendb-5.2.2/ravendb/documents/identity/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/identity/__init__.py
--rw-rw-rw-   0        0        0     9366 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/identity/hilo.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.673645 ravendb-5.2.2/ravendb/documents/indexes/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.675643 ravendb-5.2.2/ravendb/documents/indexes/analysis/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/analysis/__init__.py
--rw-rw-rw-   0        0        0      193 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/analysis/definitions.py
--rw-rw-rw-   0        0        0    19199 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/definitions.py
--rw-rw-rw-   0        0        0    19756 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/index_creation.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.676646 ravendb-5.2.2/ravendb/documents/indexes/spatial/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/spatial/__init__.py
--rw-rw-rw-   0        0        0     7985 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/indexes/spatial/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.688644 ravendb-5.2.2/ravendb/documents/operations/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.689644 ravendb-5.2.2/ravendb/documents/operations/attachments/
--rw-rw-rw-   0        0        0    11297 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/operations/attachments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.691643 ravendb-5.2.2/ravendb/documents/operations/backups/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/backups/__init__.py
--rw-rw-rw-   0        0        0      566 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/backups/settings.py
--rw-rw-rw-   0        0        0    20287 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/batch.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.695644 ravendb-5.2.2/ravendb/documents/operations/compare_exchange/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/compare_exchange/__init__.py
--rw-rw-rw-   0        0        0     9566 2023-03-03 14:25:22.000000 ravendb-5.2.2/ravendb/documents/operations/compare_exchange/compare_exchange.py
--rw-rw-rw-   0        0        0     4300 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/compare_exchange/compare_exchange_value_result_parser.py
--rw-rw-rw-   0        0        0    11066 2023-03-03 14:25:22.000000 ravendb-5.2.2/ravendb/documents/operations/compare_exchange/operations.py
--rw-rw-rw-   0        0        0     8089 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/configuration.py
--rw-rw-rw-   0        0        0      185 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/connection_strings.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.696643 ravendb-5.2.2/ravendb/documents/operations/counters/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/counters/__init__.py
--rw-rw-rw-   0        0        0     2229 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/counters/operation.py
--rw-rw-rw-   0        0        0     1666 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/definitions.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.698645 ravendb-5.2.2/ravendb/documents/operations/etl/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/etl/__init__.py
--rw-rw-rw-   0        0        0      763 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/etl/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.699643 ravendb-5.2.2/ravendb/documents/operations/etl/olap/
--rw-rw-rw-   0        0        0     1383 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/etl/olap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.700644 ravendb-5.2.2/ravendb/documents/operations/etl/sql/
--rw-rw-rw-   0        0        0      704 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/etl/sql/__init__.py
--rw-rw-rw-   0        0        0     5830 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/operations/executor.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.702643 ravendb-5.2.2/ravendb/documents/operations/expiration/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/expiration/__init__.py
--rw-rw-rw-   0        0        0      268 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/expiration/configuration.py
--rw-rw-rw-   0        0        0    25958 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/indexes.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.703643 ravendb-5.2.2/ravendb/documents/operations/lazy/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/lazy/__init__.py
--rw-rw-rw-   0        0        0      752 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/lazy/lazy_operation.py
--rw-rw-rw-   0        0        0     4369 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/misc.py
--rw-rw-rw-   0        0        0     3393 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/ongoing_tasks.py
--rw-rw-rw-   0        0        0     2543 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/operation.py
--rw-rw-rw-   0        0        0     9869 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/patch.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.705643 ravendb-5.2.2/ravendb/documents/operations/refresh/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/refresh/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/refresh/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.707644 ravendb-5.2.2/ravendb/documents/operations/replication/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/replication/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/replication/definitions.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.709644 ravendb-5.2.2/ravendb/documents/operations/revisions/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/revisions/__init__.py
--rw-rw-rw-   0        0        0      115 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/revisions/configuration.py
--rw-rw-rw-   0        0        0    11772 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/statistics.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.710643 ravendb-5.2.2/ravendb/documents/operations/time_series/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/time_series/__init__.py
--rw-rw-rw-   0        0        0       65 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/operations/time_series/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.721644 ravendb-5.2.2/ravendb/documents/queries/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/__init__.py
--rw-rw-rw-   0        0        0      666 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/explanation.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.726645 ravendb-5.2.2/ravendb/documents/queries/facets/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/facets/__init__.py
--rw-rw-rw-   0        0        0     9043 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/facets/builders.py
--rw-rw-rw-   0        0        0     5529 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/facets/definitions.py
--rw-rw-rw-   0        0        0     3425 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/queries/facets/misc.py
--rw-rw-rw-   0        0        0     4746 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/facets/queries.py
--rw-rw-rw-   0        0        0      521 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/group_by.py
--rw-rw-rw-   0        0        0     1809 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/highlighting.py
--rw-rw-rw-   0        0        0     5853 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/queries/index_query.py
--rw-rw-rw-   0        0        0     1312 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/misc.py
--rw-rw-rw-   0        0        0     5956 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/queries/more_like_this.py
--rw-rw-rw-   0        0        0     8404 2023-02-09 15:28:38.000000 ravendb-5.2.2/ravendb/documents/queries/query.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.726645 ravendb-5.2.2/ravendb/documents/queries/sorting/
--rw-rw-rw-   0        0        0      191 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/sorting/__init__.py
--rw-rw-rw-   0        0        0     6687 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/spatial.py
--rw-rw-rw-   0        0        0     7845 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/suggestions.py
--rw-rw-rw-   0        0        0     4749 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/queries/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.743926 ravendb-5.2.2/ravendb/documents/session/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/__init__.py
--rw-rw-rw-   0        0        0    13971 2023-03-03 14:25:22.000000 ravendb-5.2.2/ravendb/documents/session/cluster_transaction_operation.py
--rw-rw-rw-   0        0        0      184 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/concurrency_check_mode.py
--rw-rw-rw-   0        0        0      687 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/conditional_load.py
--rw-rw-rw-   0        0        0     1858 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/document_info.py
--rw-rw-rw-   0        0        0    63429 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/session/document_session.py
--rw-rw-rw-   0        0        0    11282 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/session/entity_to_json.py
--rw-rw-rw-   0        0        0     7891 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/event_args.py
--rw-rw-rw-   0        0        0    78949 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/in_memory_document_session_operations.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.746041 ravendb-5.2.2/ravendb/documents/session/loaders/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/loaders/__init__.py
--rw-rw-rw-   0        0        0     8174 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/loaders/include.py
--rw-rw-rw-   0        0        0     1471 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/loaders/loaders.py
--rw-rw-rw-   0        0        0     8749 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.750760 ravendb-5.2.2/ravendb/documents/session/operations/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/operations/__init__.py
--rw-rw-rw-   0        0        0    26895 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/session/operations/lazy.py
--rw-rw-rw-   0        0        0     7726 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/session/operations/load_operation.py
--rw-rw-rw-   0        0        0     3842 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/operations/operations.py
--rw-rw-rw-   0        0        0    10665 2023-03-03 14:25:22.000000 ravendb-5.2.2/ravendb/documents/session/operations/query.py
--rw-rw-rw-   0        0        0    95648 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/documents/session/query.py
--rw-rw-rw-   0        0        0     1376 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/query_group_by.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.752767 ravendb-5.2.2/ravendb/documents/session/time_series/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/time_series/__init__.py
--rw-rw-rw-   0        0        0      706 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/time_series/time_series.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.753767 ravendb-5.2.2/ravendb/documents/session/tokens/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/__init__.py
--rw-rw-rw-   0        0        0      645 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.757768 ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/__init__.py
--rw-rw-rw-   0        0        0    32819 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/definitions.py
--rw-rw-rw-   0        0        0     9277 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/facets.py
--rw-rw-rw-   0        0        0      558 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/query_token.py
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/transaction_mode.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.760769 ravendb-5.2.2/ravendb/documents/session/utils/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/utils/__init__.py
--rw-rw-rw-   0        0        0      635 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/utils/document_query.py
--rw-rw-rw-   0        0        0      509 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/session/utils/includes_util.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.764768 ravendb-5.2.2/ravendb/documents/store/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/store/__init__.py
--rw-rw-rw-   0        0        0    21198 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/documents/store/definition.py
--rw-rw-rw-   0        0        0      883 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/store/lazy.py
--rw-rw-rw-   0        0        0     1043 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/store/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.770769 ravendb-5.2.2/ravendb/documents/subscriptions/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/__init__.py
--rw-rw-rw-   0        0        0    10476 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/document_subscriptions.py
--rw-rw-rw-   0        0        0     3837 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/options.py
--rw-rw-rw-   0        0        0      255 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/revision.py
--rw-rw-rw-   0        0        0     1724 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/state.py
--rw-rw-rw-   0        0        0    45032 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/documents/subscriptions/worker.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.775768 ravendb-5.2.2/ravendb/exceptions/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/__init__.py
--rw-rw-rw-   0        0        0      181 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/cluster.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.777767 ravendb-5.2.2/ravendb/exceptions/documents/
--rw-rw-rw-   0        0        0     1028 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/documents/__init__.py
--rw-rw-rw-   0        0        0      521 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/documents/bulkinsert.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.778768 ravendb-5.2.2/ravendb/exceptions/documents/indexes/
--rw-rw-rw-   0        0        0      129 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/documents/indexes/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/exception_dispatcher.py
--rw-rw-rw-   0        0        0     2294 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/exceptions.py
--rw-rw-rw-   0        0        0     1093 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/exceptions/raven_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.782767 ravendb-5.2.2/ravendb/extensions/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/extensions/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/extensions/http_extensions.py
--rw-rw-rw-   0        0        0     4433 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/extensions/json_extensions.py
--rw-rw-rw-   0        0        0      880 2023-03-01 13:55:07.000000 ravendb-5.2.2/ravendb/extensions/string_extensions.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.789768 ravendb-5.2.2/ravendb/http/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/http/__init__.py
--rw-rw-rw-   0        0        0     4318 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/http/http_cache.py
--rw-rw-rw-   0        0        0     1862 2023-02-15 09:14:12.000000 ravendb-5.2.2/ravendb/http/misc.py
--rw-rw-rw-   0        0        0     6716 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/http/raven_command.py
--rw-rw-rw-   0        0        0    56214 2023-03-03 14:09:38.000000 ravendb-5.2.2/ravendb/http/request_executor.py
--rw-rw-rw-   0        0        0     1938 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/http/server_node.py
--rw-rw-rw-   0        0        0    11207 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/http/topology.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.795766 ravendb-5.2.2/ravendb/infrastructure/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/infrastructure/__init__.py
--rw-rw-rw-   0        0        0      953 2023-02-09 15:28:38.000000 ravendb-5.2.2/ravendb/infrastructure/entities.py
--rw-rw-rw-   0        0        0     1426 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/infrastructure/faceted.py
--rw-rw-rw-   0        0        0      520 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/infrastructure/graph.py
--rw-rw-rw-   0        0        0     1240 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/infrastructure/operations.py
--rw-rw-rw-   0        0        0     4590 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/infrastructure/orders.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.799766 ravendb-5.2.2/ravendb/json/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/json/__init__.py
--rw-rw-rw-   0        0        0    10611 2023-02-15 07:56:55.000000 ravendb-5.2.2/ravendb/json/json_operation.py
--rw-rw-rw-   0        0        0     2593 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/json/metadata_as_dictionary.py
--rw-rw-rw-   0        0        0      191 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/json/result.py
--rw-rw-rw-   0        0        0      333 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.802766 ravendb-5.2.2/ravendb/primitives/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/primitives/__init__.py
--rw-rw-rw-   0        0        0      148 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/primitives/exceptions.py
--rw-rw-rw-   0        0        0     1188 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/primitives/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.809768 ravendb-5.2.2/ravendb/serverwide/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/__init__.py
--rw-rw-rw-   0        0        0     3820 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/commands.py
--rw-rw-rw-   0        0        0    10363 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/database_record.py
--rw-rw-rw-   0        0        0     3541 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.812767 ravendb-5.2.2/ravendb/serverwide/operations/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/operations/__init__.py
--rw-rw-rw-   0        0        0    20576 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/operations/certificates.py
--rw-rw-rw-   0        0        0    14210 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/operations/common.py
--rw-rw-rw-   0        0        0     4444 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/server_operation_executor.py
--rw-rw-rw-   0        0        0    14566 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/serverwide/tcp.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.820767 ravendb-5.2.2/ravendb/tools/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/__init__.py
--rw-rw-rw-   0        0        0      399 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/concurrentset.py
--rw-rw-rw-   0        0        0     2207 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/custom_decoder.py
--rw-rw-rw-   0        0        0      642 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/generate_id.py
--rw-rw-rw-   0        0        0     2197 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/indexqueue.py
--rw-rw-rw-   0        0        0     9023 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/tools/parsers.py
--rw-rw-rw-   0        0        0     1952 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/tools/projection.py
--rw-rw-rw-   0        0        0    33546 2023-03-03 14:09:28.000000 ravendb-5.2.2/ravendb/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.823768 ravendb-5.2.2/ravendb/util/
--rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/util/__init__.py
--rw-rw-rw-   0        0        0     2167 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/util/tcp_utils.py
--rw-rw-rw-   0        0        0      501 2023-02-08 09:25:35.000000 ravendb-5.2.2/ravendb/util/util.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:30:02.650643 ravendb-5.2.2/ravendb.egg-info/
--rw-rw-rw-   0        0        0     4129 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7558 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-03 14:30:02.000000 ravendb-5.2.2/ravendb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 14:30:02.825767 ravendb-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-03-03 14:09:38.000000 ravendb-5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.685902 ravendb-5.2.3/
+-rw-rw-rw-   0        0        0     1100 2022-05-26 12:42:03.000000 ravendb-5.2.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-02-08 09:25:35.000000 ravendb-5.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4413 2023-04-17 08:22:24.685902 ravendb-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    40688 2023-04-17 08:21:27.000000 ravendb-5.2.3/README.md
+-rw-rw-rw-   0        0        0     4046 2023-04-17 08:21:27.000000 ravendb-5.2.3/README_pypi.md
+-rw-rw-rw-   0        0        0       81 2022-05-26 12:42:03.000000 ravendb-5.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.497902 ravendb-5.2.3/ravendb/
+-rw-rw-rw-   0        0        0    19779 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.506904 ravendb-5.2.3/ravendb/changes/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/changes/__init__.py
+-rw-rw-rw-   0        0        0    16419 2023-04-04 11:25:12.000000 ravendb-5.2.3/ravendb/changes/database_changes.py
+-rw-rw-rw-   0        0        0     4356 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/changes/observers.py
+-rw-rw-rw-   0        0        0     4938 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/changes/types.py
+-rw-rw-rw-   0        0        0     2118 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.509903 ravendb-5.2.3/ravendb/data/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/data/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/data/operation.py
+-rw-rw-rw-   0        0        0     9796 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/data/query.py
+-rw-rw-rw-   0        0        0     2466 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/data/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.513901 ravendb-5.2.3/ravendb/documents/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/__init__.py
+-rw-rw-rw-   0        0        0    18788 2023-02-15 14:10:24.000000 ravendb-5.2.3/ravendb/documents/bulk_insert_operation.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.521902 ravendb-5.2.3/ravendb/documents/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/__init__.py
+-rw-rw-rw-   0        0        0    24378 2023-03-13 12:54:59.000000 ravendb-5.2.3/ravendb/documents/commands/batches.py
+-rw-rw-rw-   0        0        0     1290 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/bulkinsert.py
+-rw-rw-rw-   0        0        0    17155 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/crud.py
+-rw-rw-rw-   0        0        0    10527 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/multi_get.py
+-rw-rw-rw-   0        0        0     2263 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/query.py
+-rw-rw-rw-   0        0        0     1577 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/results.py
+-rw-rw-rw-   0        0        0     8523 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/commands/subscriptions.py
+-rw-rw-rw-   0        0        0    19605 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/conventions.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/documents.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.523902 ravendb-5.2.3/ravendb/documents/identity/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/identity/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-04-11 12:57:39.000000 ravendb-5.2.3/ravendb/documents/identity/hilo.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.526901 ravendb-5.2.3/ravendb/documents/indexes/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.528901 ravendb-5.2.3/ravendb/documents/indexes/analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/analysis/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/analysis/definitions.py
+-rw-rw-rw-   0        0        0     8494 2023-04-14 14:12:28.000000 ravendb-5.2.3/ravendb/documents/indexes/counters.py
+-rw-rw-rw-   0        0        0    19199 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/definitions.py
+-rw-rw-rw-   0        0        0    19756 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/index_creation.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.531903 ravendb-5.2.3/ravendb/documents/indexes/spatial/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/spatial/__init__.py
+-rw-rw-rw-   0        0        0     7985 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/indexes/spatial/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.544902 ravendb-5.2.3/ravendb/documents/operations/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.545903 ravendb-5.2.3/ravendb/documents/operations/attachments/
+-rw-rw-rw-   0        0        0    11297 2023-02-15 09:14:12.000000 ravendb-5.2.3/ravendb/documents/operations/attachments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.546902 ravendb-5.2.3/ravendb/documents/operations/backups/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/backups/__init__.py
+-rw-rw-rw-   0        0        0      566 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/backups/settings.py
+-rw-rw-rw-   0        0        0    20313 2023-03-13 14:28:31.000000 ravendb-5.2.3/ravendb/documents/operations/batch.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.550902 ravendb-5.2.3/ravendb/documents/operations/compare_exchange/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/compare_exchange/__init__.py
+-rw-rw-rw-   0        0        0     9566 2023-03-03 14:25:22.000000 ravendb-5.2.3/ravendb/documents/operations/compare_exchange/compare_exchange.py
+-rw-rw-rw-   0        0        0     4300 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/compare_exchange/compare_exchange_value_result_parser.py
+-rw-rw-rw-   0        0        0    11066 2023-03-03 14:25:22.000000 ravendb-5.2.3/ravendb/documents/operations/compare_exchange/operations.py
+-rw-rw-rw-   0        0        0     8089 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/configuration.py
+-rw-rw-rw-   0        0        0      185 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/connection_strings.py
+-rw-rw-rw-   0        0        0    10292 2023-03-13 12:54:46.000000 ravendb-5.2.3/ravendb/documents/operations/counters.py
+-rw-rw-rw-   0        0        0     1666 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/definitions.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.552902 ravendb-5.2.3/ravendb/documents/operations/etl/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/etl/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/etl/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.553905 ravendb-5.2.3/ravendb/documents/operations/etl/olap/
+-rw-rw-rw-   0        0        0     1383 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/etl/olap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.554905 ravendb-5.2.3/ravendb/documents/operations/etl/sql/
+-rw-rw-rw-   0        0        0      704 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/etl/sql/__init__.py
+-rw-rw-rw-   0        0        0     5838 2023-03-10 13:20:06.000000 ravendb-5.2.3/ravendb/documents/operations/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.556903 ravendb-5.2.3/ravendb/documents/operations/expiration/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/expiration/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/expiration/configuration.py
+-rw-rw-rw-   0        0        0    25958 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/indexes.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.557903 ravendb-5.2.3/ravendb/documents/operations/lazy/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/lazy/__init__.py
+-rw-rw-rw-   0        0        0      752 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/lazy/lazy_operation.py
+-rw-rw-rw-   0        0        0     4369 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/misc.py
+-rw-rw-rw-   0        0        0     3393 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/ongoing_tasks.py
+-rw-rw-rw-   0        0        0     2543 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/operation.py
+-rw-rw-rw-   0        0        0     9869 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.559904 ravendb-5.2.3/ravendb/documents/operations/refresh/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/refresh/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/refresh/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.561902 ravendb-5.2.3/ravendb/documents/operations/replication/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/replication/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/replication/definitions.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.563902 ravendb-5.2.3/ravendb/documents/operations/revisions/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/revisions/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/revisions/configuration.py
+-rw-rw-rw-   0        0        0    11772 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/statistics.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.565902 ravendb-5.2.3/ravendb/documents/operations/time_series/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/time_series/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/operations/time_series/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.577901 ravendb-5.2.3/ravendb/documents/queries/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/explanation.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.583902 ravendb-5.2.3/ravendb/documents/queries/facets/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/facets/__init__.py
+-rw-rw-rw-   0        0        0     9043 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/facets/builders.py
+-rw-rw-rw-   0        0        0     5529 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/facets/definitions.py
+-rw-rw-rw-   0        0        0     3425 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/documents/queries/facets/misc.py
+-rw-rw-rw-   0        0        0     4746 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/facets/queries.py
+-rw-rw-rw-   0        0        0      521 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/group_by.py
+-rw-rw-rw-   0        0        0     1809 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/highlighting.py
+-rw-rw-rw-   0        0        0     5853 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/documents/queries/index_query.py
+-rw-rw-rw-   0        0        0     1312 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/misc.py
+-rw-rw-rw-   0        0        0     5956 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/documents/queries/more_like_this.py
+-rw-rw-rw-   0        0        0     8404 2023-02-09 15:28:38.000000 ravendb-5.2.3/ravendb/documents/queries/query.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.584904 ravendb-5.2.3/ravendb/documents/queries/sorting/
+-rw-rw-rw-   0        0        0      191 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/sorting/__init__.py
+-rw-rw-rw-   0        0        0     6687 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/spatial.py
+-rw-rw-rw-   0        0        0     7845 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/suggestions.py
+-rw-rw-rw-   0        0        0     4749 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/queries/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.598903 ravendb-5.2.3/ravendb/documents/session/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/__init__.py
+-rw-rw-rw-   0        0        0    13971 2023-03-03 14:25:22.000000 ravendb-5.2.3/ravendb/documents/session/cluster_transaction_operation.py
+-rw-rw-rw-   0        0        0      184 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/concurrency_check_mode.py
+-rw-rw-rw-   0        0        0      687 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/conditional_load.py
+-rw-rw-rw-   0        0        0     1858 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/document_info.py
+-rw-rw-rw-   0        0        0    73288 2023-04-14 14:12:28.000000 ravendb-5.2.3/ravendb/documents/session/document_session.py
+-rw-rw-rw-   0        0        0    11282 2023-02-15 09:14:12.000000 ravendb-5.2.3/ravendb/documents/session/entity_to_json.py
+-rw-rw-rw-   0        0        0     7891 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/event_args.py
+-rw-rw-rw-   0        0        0    78980 2023-03-29 09:06:14.000000 ravendb-5.2.3/ravendb/documents/session/in_memory_document_session_operations.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.602905 ravendb-5.2.3/ravendb/documents/session/loaders/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/loaders/__init__.py
+-rw-rw-rw-   0        0        0     8458 2023-03-30 10:08:29.000000 ravendb-5.2.3/ravendb/documents/session/loaders/include.py
+-rw-rw-rw-   0        0        0     1471 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/loaders/loaders.py
+-rw-rw-rw-   0        0        0     8749 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.607903 ravendb-5.2.3/ravendb/documents/session/operations/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/operations/__init__.py
+-rw-rw-rw-   0        0        0    26905 2023-04-14 14:12:28.000000 ravendb-5.2.3/ravendb/documents/session/operations/lazy.py
+-rw-rw-rw-   0        0        0     7735 2023-03-28 14:59:53.000000 ravendb-5.2.3/ravendb/documents/session/operations/load_operation.py
+-rw-rw-rw-   0        0        0     3842 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/operations/operations.py
+-rw-rw-rw-   0        0        0    10725 2023-03-29 13:00:30.000000 ravendb-5.2.3/ravendb/documents/session/operations/query.py
+-rw-rw-rw-   0        0        0    96349 2023-03-30 09:09:15.000000 ravendb-5.2.3/ravendb/documents/session/query.py
+-rw-rw-rw-   0        0        0     1376 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/query_group_by.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.609902 ravendb-5.2.3/ravendb/documents/session/time_series/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/time_series/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/time_series/time_series.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.611902 ravendb-5.2.3/ravendb/documents/session/tokens/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.615902 ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/__init__.py
+-rw-rw-rw-   0        0        0    32819 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/definitions.py
+-rw-rw-rw-   0        0        0     9277 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/facets.py
+-rw-rw-rw-   0        0        0      558 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/query_token.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/transaction_mode.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.618902 ravendb-5.2.3/ravendb/documents/session/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/utils/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/utils/document_query.py
+-rw-rw-rw-   0        0        0      509 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/session/utils/includes_util.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.622902 ravendb-5.2.3/ravendb/documents/store/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/store/__init__.py
+-rw-rw-rw-   0        0        0    21297 2023-04-11 12:57:39.000000 ravendb-5.2.3/ravendb/documents/store/definition.py
+-rw-rw-rw-   0        0        0      883 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/store/lazy.py
+-rw-rw-rw-   0        0        0     1043 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/store/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.630902 ravendb-5.2.3/ravendb/documents/subscriptions/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/subscriptions/__init__.py
+-rw-rw-rw-   0        0        0    10476 2023-04-05 11:32:12.000000 ravendb-5.2.3/ravendb/documents/subscriptions/document_subscriptions.py
+-rw-rw-rw-   0        0        0     3837 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/subscriptions/options.py
+-rw-rw-rw-   0        0        0      255 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/subscriptions/revision.py
+-rw-rw-rw-   0        0        0     1724 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/documents/subscriptions/state.py
+-rw-rw-rw-   0        0        0    45032 2023-04-04 09:21:08.000000 ravendb-5.2.3/ravendb/documents/subscriptions/worker.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.635902 ravendb-5.2.3/ravendb/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      181 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/cluster.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.637902 ravendb-5.2.3/ravendb/exceptions/documents/
+-rw-rw-rw-   0        0        0     1028 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/documents/__init__.py
+-rw-rw-rw-   0        0        0      521 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/documents/bulkinsert.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.638902 ravendb-5.2.3/ravendb/exceptions/documents/indexes/
+-rw-rw-rw-   0        0        0      129 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/documents/indexes/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/exception_dispatcher.py
+-rw-rw-rw-   0        0        0     2294 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/exceptions.py
+-rw-rw-rw-   0        0        0     1093 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/exceptions/raven_exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.642904 ravendb-5.2.3/ravendb/extensions/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/extensions/http_extensions.py
+-rw-rw-rw-   0        0        0     4433 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/extensions/json_extensions.py
+-rw-rw-rw-   0        0        0      880 2023-03-01 13:55:07.000000 ravendb-5.2.3/ravendb/extensions/string_extensions.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.650903 ravendb-5.2.3/ravendb/http/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/http/__init__.py
+-rw-rw-rw-   0        0        0     4344 2023-04-11 12:57:39.000000 ravendb-5.2.3/ravendb/http/http_cache.py
+-rw-rw-rw-   0        0        0     1862 2023-02-15 09:14:12.000000 ravendb-5.2.3/ravendb/http/misc.py
+-rw-rw-rw-   0        0        0     6716 2023-04-05 07:32:49.000000 ravendb-5.2.3/ravendb/http/raven_command.py
+-rw-rw-rw-   0        0        0    56251 2023-04-17 08:21:27.000000 ravendb-5.2.3/ravendb/http/request_executor.py
+-rw-rw-rw-   0        0        0     1938 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/http/server_node.py
+-rw-rw-rw-   0        0        0    11207 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/http/topology.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.655902 ravendb-5.2.3/ravendb/infrastructure/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/infrastructure/__init__.py
+-rw-rw-rw-   0        0        0      953 2023-02-09 15:28:38.000000 ravendb-5.2.3/ravendb/infrastructure/entities.py
+-rw-rw-rw-   0        0        0     1426 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/infrastructure/faceted.py
+-rw-rw-rw-   0        0        0      520 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/infrastructure/graph.py
+-rw-rw-rw-   0        0        0     1240 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/infrastructure/operations.py
+-rw-rw-rw-   0        0        0     4590 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/infrastructure/orders.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.659903 ravendb-5.2.3/ravendb/json/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/json/__init__.py
+-rw-rw-rw-   0        0        0    10611 2023-02-15 07:56:55.000000 ravendb-5.2.3/ravendb/json/json_operation.py
+-rw-rw-rw-   0        0        0     2593 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/json/metadata_as_dictionary.py
+-rw-rw-rw-   0        0        0      191 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/json/result.py
+-rw-rw-rw-   0        0        0      333 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.662902 ravendb-5.2.3/ravendb/primitives/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/primitives/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/primitives/exceptions.py
+-rw-rw-rw-   0        0        0     1188 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/primitives/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.668902 ravendb-5.2.3/ravendb/serverwide/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/__init__.py
+-rw-rw-rw-   0        0        0     3820 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/commands.py
+-rw-rw-rw-   0        0        0    10363 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/database_record.py
+-rw-rw-rw-   0        0        0     3541 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.672904 ravendb-5.2.3/ravendb/serverwide/operations/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/operations/__init__.py
+-rw-rw-rw-   0        0        0    20576 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/operations/certificates.py
+-rw-rw-rw-   0        0        0    14208 2023-04-11 12:57:39.000000 ravendb-5.2.3/ravendb/serverwide/operations/common.py
+-rw-rw-rw-   0        0        0     4467 2023-04-11 12:57:39.000000 ravendb-5.2.3/ravendb/serverwide/server_operation_executor.py
+-rw-rw-rw-   0        0        0    14566 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/serverwide/tcp.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.681902 ravendb-5.2.3/ravendb/tools/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/concurrentset.py
+-rw-rw-rw-   0        0        0     2207 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/custom_decoder.py
+-rw-rw-rw-   0        0        0      642 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/generate_id.py
+-rw-rw-rw-   0        0        0     2197 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/indexqueue.py
+-rw-rw-rw-   0        0        0     9023 2023-03-03 14:09:28.000000 ravendb-5.2.3/ravendb/tools/parsers.py
+-rw-rw-rw-   0        0        0     1952 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/tools/projection.py
+-rw-rw-rw-   0        0        0    34146 2023-04-05 07:54:04.000000 ravendb-5.2.3/ravendb/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.684902 ravendb-5.2.3/ravendb/util/
+-rw-rw-rw-   0        0        0        0 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/util/__init__.py
+-rw-rw-rw-   0        0        0     2167 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/util/tcp_utils.py
+-rw-rw-rw-   0        0        0      501 2023-02-08 09:25:35.000000 ravendb-5.2.3/ravendb/util/util.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:22:24.502902 ravendb-5.2.3/ravendb.egg-info/
+-rw-rw-rw-   0        0        0     4413 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7536 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 08:22:24.000000 ravendb-5.2.3/ravendb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:22:24.686903 ravendb-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-04-17 08:21:27.000000 ravendb-5.2.3/setup.py
```

### Comparing `ravendb-5.2.2/LICENSE` & `ravendb-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/PKG-INFO` & `ravendb-5.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravendb
-Version: 5.2.2
+Version: 5.2.3
 Summary: Python client for RavenDB NoSQL Database
 Home-page: https://github.com/ravendb/ravendb-python-client
 Author: RavenDB
 Author-email: support@ravendb.net
 License: MIT
 Keywords: ravendb,nosql,databasepyravendb
 Requires-Python: ~=3.7
@@ -18,23 +18,32 @@
 Install from [PyPi](https://pypi.python.org/pypi), as [ravendb](https://pypi.org/project/ravendb/).
 ```bash
 pip install ravendb
 ````
 ## Introduction
 Python client API (v5.2) for [RavenDB](https://ravendb.net/) , a NoSQL document database.
 
-
 Although new API isn't compatible with the previous one, it comes with **many improvements and new features**.
 
 **Package has been reworked to match Java and other RavenDB clients**
 
 **Type-hinted entire project and API results** - using the API is now much more comfortable with IntelliSense
 
+
+## Releases
+
+* All client versions 5.2.x are fully compatible with and support RavenDB server releases 5.4 and 6.0.
+
+* [Click here](https://github.com/ravendb/ravendb-python-client/releases) to view all Releases and Changelog.
+
 ## What's new?
 
+###### 5.2.3
+- **Counters**
+- Counters indexes
 
 ###### 5.2.2
 - New feature - **[Bulk insert](https://github.com/ravendb/ravendb-python-client/pull/161)**
 - Bugfixes - Cluster-wide operations ([here](https://github.com/ravendb/ravendb-python-client/pull/166))
 
 ###### 5.2.1
 - Bugfixes - Serialization while loading/querying ([here](https://github.com/ravendb/ravendb-python-client/pull/163))
```

### Comparing `ravendb-5.2.2/README.md` & `ravendb-5.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,37 @@
 Install from [PyPi](https://pypi.python.org/pypi), as [ravendb](https://pypi.org/project/ravendb).
 ```bash
 pip install ravendb
 ````
 ## Introduction and changelog
 Python client API (v5.2) for [RavenDB](https://ravendb.net/) , a NoSQL document database.
 
-
 Although new API isn't compatible with the previous one, it comes with **many improvements and new features**.
 
 **Package has been reworked to match Java and other RavenDB clients**
 
 **Type-hinted entire project and API results** - using the API is now much more comfortable with IntelliSense
 
+## Releases
+
+* All client versions 5.2.x are fully compatible with and support RavenDB server releases 5.4 and 6.0.
+
+* [Click here](https://github.com/ravendb/ravendb-python-client/releases) to view all Releases and Changelog.
+
 ---
 ![](.github/readme_content/typehints.gif)
 
 ---
 
 ## What's new?
 
+###### 5.2.3
+- **Counters**
+- Counters indexes
+
 ###### 5.2.2
 - New feature - **[Bulk insert](https://github.com/ravendb/ravendb-python-client/pull/161)**
 - Bugfixes - Cluster-wide operations ([here](https://github.com/ravendb/ravendb-python-client/pull/166))
 
 ###### 5.2.1
 - Bugfixes - Serialization while loading/querying ([here](https://github.com/ravendb/ravendb-python-client/pull/163))
```

### Comparing `ravendb-5.2.2/README_pypi.md` & `ravendb-5.2.3/README_pypi.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,32 @@
 Install from [PyPi](https://pypi.python.org/pypi), as [ravendb](https://pypi.org/project/ravendb/).
 ```bash
 pip install ravendb
 ````
 ## Introduction
 Python client API (v5.2) for [RavenDB](https://ravendb.net/) , a NoSQL document database.
 
-
 Although new API isn't compatible with the previous one, it comes with **many improvements and new features**.
 
 **Package has been reworked to match Java and other RavenDB clients**
 
 **Type-hinted entire project and API results** - using the API is now much more comfortable with IntelliSense
 
+
+## Releases
+
+* All client versions 5.2.x are fully compatible with and support RavenDB server releases 5.4 and 6.0.
+
+* [Click here](https://github.com/ravendb/ravendb-python-client/releases) to view all Releases and Changelog.
+
 ## What's new?
 
+###### 5.2.3
+- **Counters**
+- Counters indexes
 
 ###### 5.2.2
 - New feature - **[Bulk insert](https://github.com/ravendb/ravendb-python-client/pull/161)**
 - Bugfixes - Cluster-wide operations ([here](https://github.com/ravendb/ravendb-python-client/pull/166))
 
 ###### 5.2.1
 - Bugfixes - Serialization while loading/querying ([here](https://github.com/ravendb/ravendb-python-client/pull/163))
```

### Comparing `ravendb-5.2.2/ravendb/__init__.py` & `ravendb-5.2.3/ravendb/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/changes/database_changes.py` & `ravendb-5.2.3/ravendb/changes/database_changes.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/changes/observers.py` & `ravendb-5.2.3/ravendb/changes/observers.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/changes/types.py` & `ravendb-5.2.3/ravendb/changes/types.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/constants.py` & `ravendb-5.2.3/ravendb/constants.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/data/query.py` & `ravendb-5.2.3/ravendb/data/query.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/data/timeseries.py` & `ravendb-5.2.3/ravendb/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/bulk_insert_operation.py` & `ravendb-5.2.3/ravendb/documents/bulk_insert_operation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/batches.py` & `ravendb-5.2.3/ravendb/documents/commands/batches.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 from abc import abstractmethod
 from enum import Enum
 from typing import Callable, Union, Optional, TYPE_CHECKING, List, Set, Dict
 
 import requests
 
-from ravendb.documents.operations.counters.operation import (
+from ravendb.documents.operations.counters import (
     CounterOperation,
     DocumentCountersOperation,
     CounterOperationType,
 )
 from ravendb.documents.session.misc import TransactionMode, ForceRevisionStrategy
 from ravendb.http.raven_command import RavenCommand
 from ravendb.http.server_node import ServerNode
@@ -488,15 +488,15 @@
         if not counter_operations:
             raise ValueError("invalid counter_operations")
         if not isinstance(counter_operations, list):
             counter_operations = [counter_operations]
 
         super().__init__(key=document_id, command_type=CommandType.COUNTERS, change_vector=change_vector)
         self._from_etl = from_etl
-        self._counters = DocumentCountersOperation(self.key, *counter_operations)
+        self._counters = DocumentCountersOperation(self.key, counter_operations)
 
     def has_increment(self, counter_name):
         self.has_operation_of_type(CounterOperationType.INCREMENT, counter_name)
 
     def has_delete(self, counter_name):
         self.has_operation_of_type(CounterOperationType.DELETE, counter_name)
 
@@ -513,15 +513,15 @@
     def counters(self):
         return self._counters
 
     def serialize(self, conventions: DocumentConventions) -> Dict:
         json_dict = {
             "Id": self.key,
             "Counters": self.counters.to_json(),
-            "Type": self.type,
+            "Type": self.command_type,
         }
         if self._from_etl:
             json_dict["FromEtl"] = self._from_etl
         return json_dict
 
 
 class PutAttachmentCommandData(CommandData):
```

### Comparing `ravendb-5.2.2/ravendb/documents/commands/bulkinsert.py` & `ravendb-5.2.3/ravendb/documents/commands/bulkinsert.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/crud.py` & `ravendb-5.2.3/ravendb/documents/commands/crud.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/multi_get.py` & `ravendb-5.2.3/ravendb/documents/commands/multi_get.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/query.py` & `ravendb-5.2.3/ravendb/documents/commands/query.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/results.py` & `ravendb-5.2.3/ravendb/documents/commands/results.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/commands/subscriptions.py` & `ravendb-5.2.3/ravendb/documents/commands/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/conventions.py` & `ravendb-5.2.3/ravendb/documents/conventions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/identity/hilo.py` & `ravendb-5.2.3/ravendb/documents/identity/hilo.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 class GenerateEntityIdOnTheClient:
     def __init__(self, conventions: "DocumentConventions", generate_id: Callable[[Any], str]):
         self.__conventions = conventions
         self.__generate_id = generate_id
 
-    def try_get_id_from_instance(self, entity: object) -> Tuple[bool, Union[str, None]]:
+    def try_get_id_from_instance(self, entity: Union[object, dict]) -> Tuple[bool, Union[str, None]]:
         if not entity:
             raise ValueError("Entity cannot be None")
         identity_property = "Id"  # todo: make sure it's ok, create get_identity_property within conventions if not
-        value = entity.__dict__.get(identity_property, None)
+        value = (entity if isinstance(entity, dict) else entity.__dict__).get(identity_property, None)
         if isinstance(value, str):
             return True, value
         return False, None
 
     def get_or_generate_document_id(self, entity) -> str:
         key = self.try_get_id_from_instance(entity)[1]
         if key is None:
```

### Comparing `ravendb-5.2.2/ravendb/documents/indexes/definitions.py` & `ravendb-5.2.3/ravendb/documents/indexes/definitions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/indexes/index_creation.py` & `ravendb-5.2.3/ravendb/documents/indexes/index_creation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/indexes/spatial/configuration.py` & `ravendb-5.2.3/ravendb/documents/indexes/spatial/configuration.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/attachments/__init__.py` & `ravendb-5.2.3/ravendb/documents/operations/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/backups/settings.py` & `ravendb-5.2.3/ravendb/documents/operations/backups/settings.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/batch.py` & `ravendb-5.2.3/ravendb/documents/operations/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,18 @@
                 self.__handle_attachment_put(batch_result)
             elif command_type == CommandType.ATTACHMENT_DELETE:
                 self.__handle_attachment_delete(batch_result)
             elif command_type == CommandType.ATTACHMENT_MOVE:
                 self.__handle_attachment_move(batch_result)
             elif command_type == CommandType.ATTACHMENT_COPY:
                 self.__handle_attachment_copy(batch_result)
-            elif (
-                command_type == CommandType.COMPARE_EXCHANGE_PUT
-                or CommandType.COMPARE_EXCHANGE_DELETE
-                or CommandType.FORCE_REVISION_CREATION
+            elif command_type in (
+                CommandType.COMPARE_EXCHANGE_PUT,
+                CommandType.COMPARE_EXCHANGE_DELETE,
+                CommandType.FORCE_REVISION_CREATION,
             ):
                 pass
             elif command_type == CommandType.COUNTERS:
                 self.__handle_counters(batch_result)
             elif command_type == CommandType.TIME_SERIES_COPY or command_type == CommandType.BATCH_PATCH:
                 break
             else:
@@ -297,39 +297,38 @@
         document_info.key = key
         document_info.change_vector = change_vector
 
         self.__apply_metadata_modifications(key, document_info)
 
     def __handle_counters(self, batch_result: dict) -> None:
         doc_id = self.__get_string_field(batch_result, CommandType.COUNTERS, "Id")
-        counters_detail: dict = batch_result.get("CountersDetail")
+        counters_detail: dict = batch_result.get("CountersDetail", None)
         if counters_detail is None:
             self.__throw_missing_field(CommandType.COUNTERS, "CountersDetail")
 
-        counters = counters_detail.get("Counters")
+        counters = counters_detail.get("Counters", None)
         if counters is None:
             self.__throw_missing_field(CommandType.COUNTERS, "Counters")
 
-        cache = self.__session.counters_by_doc_id[doc_id]
+        cache = self.__session.counters_by_doc_id.get(doc_id, None)
         if cache is None:
             cache = [False, CaseInsensitiveDict()]
             self.__session.counters_by_doc_id[doc_id] = cache
 
         change_vector = self.__get_string_field(batch_result, CommandType.COUNTERS, "DocumentChangeVector", False)
         if change_vector is not None:
-            document_info = self.__session._documents_by_id.get(doc_id)
+            document_info = self.__session._documents_by_id.get(doc_id, None)
             if document_info is not None:
                 document_info.change_vector = change_vector
 
         for counter in counters:
-            counter: dict
-            name = counter.get("CounterName")
-            value = counter.get("TotalValue")
+            name = counter.get("CounterName", None)
+            value = counter.get("TotalValue", None)
 
-            if not name and not value:
+            if name is not None and value is not None:
                 cache[1][name] = value
 
     def __handle_attachment_put(self, batch_result: dict) -> None:
         self.__handle_attachment_put_internal(
             batch_result, CommandType.ATTACHMENT_PUT, "Id", "Name", "DocumentChangeVector"
         )
```

### Comparing `ravendb-5.2.2/ravendb/documents/operations/compare_exchange/compare_exchange.py` & `ravendb-5.2.3/ravendb/documents/operations/compare_exchange/compare_exchange.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/compare_exchange/compare_exchange_value_result_parser.py` & `ravendb-5.2.3/ravendb/documents/operations/compare_exchange/compare_exchange_value_result_parser.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/compare_exchange/operations.py` & `ravendb-5.2.3/ravendb/documents/operations/compare_exchange/operations.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/configuration.py` & `ravendb-5.2.3/ravendb/documents/operations/configuration.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/definitions.py` & `ravendb-5.2.3/ravendb/documents/operations/definitions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/etl/configuration.py` & `ravendb-5.2.3/ravendb/documents/operations/etl/configuration.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/etl/olap/__init__.py` & `ravendb-5.2.3/ravendb/documents/operations/etl/olap/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/etl/sql/__init__.py` & `ravendb-5.2.3/ravendb/documents/operations/etl/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/executor.py` & `ravendb-5.2.3/ravendb/documents/operations/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             raise ValueError("Cannot use operations without a database defined, did you forget to call 'for_database'?")
 
     def for_database(self, database_name: str) -> OperationExecutor:
         if self.__database_name.lower() == database_name.lower():
             return self
         return OperationExecutor(self.__store, database_name)
 
-    def send(self, operation: Union[IOperation, VoidOperation], session_info: SessionInfo = None):
+    def send(self, operation: IOperation[_Operation_T], session_info: SessionInfo = None) -> _Operation_T:
         command = operation.get_command(
             self.__store, self.__request_executor.conventions, self.__request_executor.cache
         )
         self.__request_executor.execute_command(command, session_info)
         return None if isinstance(operation, VoidOperation) else command.result
 
     def send_async(self, operation: IOperation[OperationIdResult]) -> Operation:
```

### Comparing `ravendb-5.2.2/ravendb/documents/operations/indexes.py` & `ravendb-5.2.3/ravendb/documents/operations/indexes.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/lazy/lazy_operation.py` & `ravendb-5.2.3/ravendb/documents/operations/lazy/lazy_operation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/misc.py` & `ravendb-5.2.3/ravendb/documents/operations/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/ongoing_tasks.py` & `ravendb-5.2.3/ravendb/documents/operations/ongoing_tasks.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/operation.py` & `ravendb-5.2.3/ravendb/documents/operations/operation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/patch.py` & `ravendb-5.2.3/ravendb/documents/operations/patch.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/refresh/configuration.py` & `ravendb-5.2.3/ravendb/documents/operations/refresh/configuration.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/replication/definitions.py` & `ravendb-5.2.3/ravendb/documents/operations/replication/definitions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/operations/statistics.py` & `ravendb-5.2.3/ravendb/documents/operations/statistics.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/explanation.py` & `ravendb-5.2.3/ravendb/documents/queries/explanation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/facets/builders.py` & `ravendb-5.2.3/ravendb/documents/queries/facets/builders.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/facets/definitions.py` & `ravendb-5.2.3/ravendb/documents/queries/facets/definitions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/facets/misc.py` & `ravendb-5.2.3/ravendb/documents/queries/facets/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/facets/queries.py` & `ravendb-5.2.3/ravendb/documents/queries/facets/queries.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/group_by.py` & `ravendb-5.2.3/ravendb/documents/queries/group_by.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/highlighting.py` & `ravendb-5.2.3/ravendb/documents/queries/highlighting.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/index_query.py` & `ravendb-5.2.3/ravendb/documents/queries/index_query.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/misc.py` & `ravendb-5.2.3/ravendb/documents/queries/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/more_like_this.py` & `ravendb-5.2.3/ravendb/documents/queries/more_like_this.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/query.py` & `ravendb-5.2.3/ravendb/documents/queries/query.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/spatial.py` & `ravendb-5.2.3/ravendb/documents/queries/spatial.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/suggestions.py` & `ravendb-5.2.3/ravendb/documents/queries/suggestions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/queries/utils.py` & `ravendb-5.2.3/ravendb/documents/queries/utils.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/cluster_transaction_operation.py` & `ravendb-5.2.3/ravendb/documents/session/cluster_transaction_operation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/conditional_load.py` & `ravendb-5.2.3/ravendb/documents/session/conditional_load.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/document_info.py` & `ravendb-5.2.3/ravendb/documents/session/document_info.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/document_session.py` & `ravendb-5.2.3/ravendb/documents/session/document_session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+import copy
 import datetime
 import http
 import json
 import os
 import time
 import uuid
 from typing import Union, Callable, TYPE_CHECKING, Optional, Dict, List, Type, TypeVar
 
 from ravendb import constants
+from ravendb.documents.operations.counters import CounterOperation, CounterOperationType, GetCountersOperation
 from ravendb.documents.session.conditional_load import ConditionalLoadResult
 from ravendb.exceptions import exceptions
 from ravendb.exceptions.exceptions import InvalidOperationException
 from ravendb.data.operation import AttachmentType
 from ravendb.data.timeseries import TimeSeriesRange
 import ravendb.documents
 from ravendb.documents.indexes.definitions import AbstractCommonApiForIndexes
@@ -42,26 +44,27 @@
     DocumentsChanges,
     SessionInfo,
     TransactionMode,
 )
 from ravendb.documents.session.query import DocumentQuery, RawDocumentQuery
 from ravendb.json.metadata_as_dictionary import MetadataAsDictionary
 from ravendb.documents.session.operations.load_operation import LoadOperation
-from ravendb.tools.utils import Utils, Stopwatch
+from ravendb.tools.utils import Utils, Stopwatch, CaseInsensitiveDict
 from ravendb.documents.commands.batches import (
     PatchCommandData,
     CommandType,
     DeleteCommandData,
     PutAttachmentCommandData,
     DeleteAttachmentCommandData,
     CopyAttachmentCommandData,
     MoveAttachmentCommandData,
     CommandData,
     IndexBatchOptions,
     ReplicationBatchOptions,
+    CountersBatchCommandData,
 )
 from ravendb.documents.commands.crud import (
     HeadDocumentCommand,
     GetDocumentsCommand,
     HeadAttachmentCommand,
     ConditionalGetDocumentsCommand,
 )
@@ -339,16 +342,16 @@
                 except IOError as e:
                     raise RuntimeError(f"Unable to serialize returned value into stream {e.args[0]}", e)
             else:
                 operation.set_result(command.result)
 
     def load_starting_with(
         self,
-        object_type: Type[_T],
         id_prefix: str,
+        object_type: Optional[Type[_T]] = None,
         matches: Optional[str] = None,
         start: Optional[int] = None,
         page_size: Optional[int] = None,
         exclude: Optional[str] = None,
         start_after: Optional[str] = None,
     ) -> List[_T]:
         load_starting_with_operation = LoadStartingWithOperation(self)
@@ -422,14 +425,20 @@
             return self.query(Query.from_index_name(index_name), object_type)
         raise ValueError("index_name cannot be None or whitespace")
 
     def query_index_type(self, index_type: Type[_TIndex], object_type: Optional[Type[_T]] = None) -> DocumentQuery[_T]:
         if index_type is None or not isinstance(index_type, AbstractCommonApiForIndexes):
             return self.query(Query.from_index_type(index_type), object_type)
 
+    def counters_for(self, document_id: str) -> SessionDocumentCounters:
+        return SessionDocumentCounters(self, document_id)
+
+    def counters_for_entity(self, entity: object) -> SessionDocumentCounters:
+        return SessionDocumentCounters(self, entity)
+
     class _EagerSessionOperations:
         def __init__(self, session: DocumentSession):
             self.__session = session
 
         def execute_all_pending_lazy_operations(self) -> ResponseTimeInformation:
             operations_to_remove = []
 
@@ -464,232 +473,232 @@
 
             self.__session._pending_lazy_operations.clear()
 
             return response_time_duration
 
     class _Advanced:
         def __init__(self, session: DocumentSession):
-            self.__session = session
+            self._session = session
             self.__vals_count = 0
             self.__custom_count = 0
             self.__attachment = None
 
             self.eagerly = DocumentSession._EagerSessionOperations(session)
 
         @property
         def request_executor(self) -> RequestExecutor:
-            return self.__session._request_executor
+            return self._session._request_executor
 
         @property
         def document_store(self) -> DocumentStore:
-            return self.__session._document_store
+            return self._session._document_store
 
         @property
         def session_info(self) -> SessionInfo:
-            return self.__session.session_info
+            return self._session.session_info
 
         @property
         def attachments(self):
             if not self.__attachment:
-                self.__attachment = self._Attachment(self.__session)
+                self.__attachment = self._Attachment(self._session)
             return self.__attachment
 
         @property
         def cluster_transaction(self) -> IClusterTransactionOperations:
-            return self.__session.cluster_transaction
+            return self._session.cluster_transaction
 
         @property
         def number_of_requests(self) -> int:
-            return self.__session.number_of_requests
+            return self._session.number_of_requests
 
         @property
         def store_identifier(self) -> str:
-            return self.__session._store_identifier
+            return self._session._store_identifier
 
         @property
         def transaction_mode(self) -> TransactionMode:
-            return self.__session.transaction_mode
+            return self._session.transaction_mode
 
         @transaction_mode.setter
         def transaction_mode(self, value: TransactionMode):
-            self.__session.transaction_mode = value
+            self._session.transaction_mode = value
 
         def is_loaded(self, key: str) -> bool:
-            return self.__session.is_loaded_or_deleted(key)
+            return self._session.is_loaded_or_deleted(key)
 
         def has_changed(self, entity: object) -> bool:
-            document_info = self.__session._documents_by_entity.get(entity)
+            document_info = self._session._documents_by_entity.get(entity)
 
             if document_info is None:
                 return False
 
-            document = self.__session.entity_to_json.convert_entity_to_json(entity, document_info)
-            return self.__session._entity_changed(document, document_info, None)
+            document = self._session.entity_to_json.convert_entity_to_json(entity, document_info)
+            return self._session._entity_changed(document, document_info, None)
 
         def get_metadata_for(self, entity: object) -> MetadataAsDictionary:
             if entity is None:
                 raise ValueError("Entity cannot be None")
-            document_info = self.__session._get_document_info(entity)
+            document_info = self._session._get_document_info(entity)
             if document_info.metadata_instance:
                 return document_info.metadata_instance
             metadata_as_json = document_info.metadata
             metadata = MetadataAsDictionary(metadata=metadata_as_json)
             document_info.metadata_instance = metadata
             return metadata
 
         def get_counters_for(self, entity: object) -> List[str]:
             if entity is None:
                 raise ValueError("Entity cannot be None")
-            document_info = self.__session._get_document_info(entity)
+            document_info = self._session._get_document_info(entity)
 
             counters_array = document_info.metadata.get(constants.Documents.Metadata.COUNTERS)
             return counters_array if counters_array else None
 
         def get_time_series_for(self, entity: object) -> List[str]:
             if not entity:
                 raise ValueError("Instance cannot be None")
-            document_info = self.__session._get_document_info(entity)
+            document_info = self._session._get_document_info(entity)
             array = document_info.metadata.get(constants.Documents.Metadata.TIME_SERIES)
             return list(map(str, array)) if array else []
 
         def get_change_vector_for(self, entity: object) -> str:
             if not entity:
                 raise ValueError("Entity cannot be None")
-            return self.__session._get_document_info(entity).metadata.get(constants.Documents.Metadata.CHANGE_VECTOR)
+            return self._session._get_document_info(entity).metadata.get(constants.Documents.Metadata.CHANGE_VECTOR)
 
         def get_last_modified_for(self, entity: object) -> datetime.datetime:
             if entity is None:
                 raise ValueError("Entity cannot be None")
-            document_info = self.__session._get_document_info(entity)
+            document_info = self._session._get_document_info(entity)
             last_modified = document_info.metadata.get(constants.Documents.Metadata.LAST_MODIFIED)
             if last_modified is not None and last_modified is not None:
                 return Utils.string_to_datetime(last_modified)
 
         def get_document_id(self, entity: object) -> Union[None, str]:
             if entity is None:
                 return None
 
-            value = self.__session._documents_by_entity.get(entity)
+            value = self._session._documents_by_entity.get(entity)
             return value.key if value is not None else None
 
         def evict(self, entity: object) -> None:
-            document_info = self.__session._documents_by_entity.get(entity)
+            document_info = self._session._documents_by_entity.get(entity)
             if document_info is not None:
-                self.__session._documents_by_entity.evict(entity)
-                self.__session._documents_by_id.pop(document_info.key, None)
+                self._session._documents_by_entity.evict(entity)
+                self._session._documents_by_id.pop(document_info.key, None)
 
-                if self.__session._counters_by_doc_id:
-                    self.__session._counters_by_doc_id.pop(document_info.key, None)
-                if self.__session._time_series_by_doc_id:
-                    self.__session._time_series_by_doc_id.pop(document_info.key, None)
+                if self._session._counters_by_doc_id:
+                    self._session._counters_by_doc_id.pop(document_info.key, None)
+                if self._session._time_series_by_doc_id:
+                    self._session._time_series_by_doc_id.pop(document_info.key, None)
 
-            self.__session._deleted_entities.evict(entity)
-            self.__session.entity_to_json.remove_from_missing(entity)
+            self._session._deleted_entities.evict(entity)
+            self._session.entity_to_json.remove_from_missing(entity)
 
         def defer(self, *commands: CommandData) -> None:
-            self.__session._defer(*commands)
+            self._session.defer(*commands)
 
         def clear(self) -> None:
-            self.__session._documents_by_entity.clear()
-            self.__session._deleted_entities.clear()
-            self.__session._documents_by_id.clear()
-            self.__session._known_missing_ids.clear()
-            if self.__session._counters_by_doc_id:
-                self.__session._counters_by_doc_id.clear()
-            self.__session._deferred_commands.clear()
-            self.__session._deferred_commands_map.clear()
-            self.__session._clear_cluster_session()
-            self.__session._pending_lazy_operations.clear()
-            self.__session.entity_to_json.clear()
+            self._session._documents_by_entity.clear()
+            self._session._deleted_entities.clear()
+            self._session._documents_by_id.clear()
+            self._session._known_missing_ids.clear()
+            if self._session._counters_by_doc_id:
+                self._session._counters_by_doc_id.clear()
+            self._session._deferred_commands.clear()
+            self._session._deferred_commands_map.clear()
+            self._session._clear_cluster_session()
+            self._session._pending_lazy_operations.clear()
+            self._session.entity_to_json.clear()
 
         def document_query(
             self,
             index_name: str = None,
             collection_name: str = None,
             object_type: Type[_T] = None,
             is_map_reduce: bool = False,
         ) -> DocumentQuery[_T]:
-            return self.__session.document_query(index_name, collection_name, object_type, is_map_reduce)
+            return self._session.document_query(index_name, collection_name, object_type, is_map_reduce)
 
         def document_query_from_index_type(self, index_type: Type[_TIndex], object_type: Type[_T]) -> DocumentQuery[_T]:
-            return self.__session.document_query_from_index_type(index_type, object_type)
+            return self._session.document_query_from_index_type(index_type, object_type)
 
         def refresh(self, entity: object) -> object:
-            document_info = self.__session._documents_by_entity.get(entity)
+            document_info = self._session._documents_by_entity.get(entity)
             if document_info is None:
                 raise ValueError("Cannot refresh a transient instance")
-            self.__session.increment_requests_count()
+            self._session.increment_requests_count()
 
             command = GetDocumentsCommand.from_single_id(document_info.key, None, False)
-            self.__session._request_executor.execute_command(command, self.__session.session_info)
-            entity = self.__session._refresh_internal(entity, command, document_info)
+            self._session._request_executor.execute_command(command, self._session.session_info)
+            entity = self._session._refresh_internal(entity, command, document_info)
             return entity
 
         def raw_query(self, query: str, object_type: Optional[Type[_T]] = None) -> RawDocumentQuery[_T]:
-            return RawDocumentQuery(object_type, self.__session, query)
+            return RawDocumentQuery(object_type, self._session, query)
 
         @property
         def lazily(self) -> LazySessionOperations:
-            return self.__session._lazily
+            return self._session._lazily
 
         def graph_query(self, object_type: type, query: str):  # -> GraphDocumentQuery:
             pass
 
         def what_changed(self) -> Dict[str, List[DocumentsChanges]]:
-            return self.__session._what_changed()
+            return self._session._what_changed()
 
         def exists(self, key: str) -> bool:
             if key is None:
                 raise ValueError("Key cannot be None")
-            if key in self.__session._known_missing_ids:
+            if key in self._session._known_missing_ids:
                 return False
 
-            if self.__session._documents_by_id.get(key) is not None:
+            if self._session._documents_by_id.get(key) is not None:
                 return True
 
             command = HeadDocumentCommand(key, None)
-            self.__session._request_executor.execute_command(command, self.__session.session_info)
+            self._session._request_executor.execute_command(command, self._session.session_info)
             return command.result is not None
 
         def wait_for_replication_after_save_changes(
             self,
             options: Callable[
                 [InMemoryDocumentSessionOperations.ReplicationWaitOptsBuilder], None
             ] = lambda options: None,
         ) -> None:
-            builder = self.__session.ReplicationWaitOptsBuilder(self.__session)
+            builder = self._session.ReplicationWaitOptsBuilder(self._session)
             options(builder)
 
             builder_options = builder.get_options()
             replication_options = builder_options.replication_options
             if replication_options is None:
                 builder_options.replication_options = ReplicationBatchOptions()
 
             if replication_options.wait_for_replicas_timeout is None:
                 replication_options.wait_for_replicas_timeout = (
-                    self.__session.conventions.wait_for_replication_after_save_changes_timeout
+                    self._session.conventions.wait_for_replication_after_save_changes_timeout
                 )
             replication_options.wait_for_replicas = True
 
         def wait_for_indexes_after_save_changes(
             self,
             options: Callable[[InMemoryDocumentSessionOperations.IndexesWaitOptsBuilder], None] = lambda options: None,
         ):
-            builder = InMemoryDocumentSessionOperations.IndexesWaitOptsBuilder(self.__session)
+            builder = InMemoryDocumentSessionOperations.IndexesWaitOptsBuilder(self._session)
             options(builder)
 
             builder_options = builder.get_options()
             index_options = builder_options.index_options
 
             if index_options is None:
                 builder_options.index_options = IndexBatchOptions()
 
             if index_options.wait_for_indexes_timeout is None:
                 index_options.wait_for_indexes_timeout = (
-                    self.__session.conventions.wait_for_indexes_after_save_changes_timeout
+                    self._session.conventions.wait_for_indexes_after_save_changes_timeout
                 )
 
             index_options.wait_for_indexes = True
 
         def __load_starting_with_internal(
             self,
             id_prefix: str,
@@ -700,39 +709,38 @@
             page_size: int,
             exclude: str,
             start_after: str,
         ) -> GetDocumentsCommand:
             operation.with_start_with(id_prefix, matches, start, page_size, exclude, start_after)
             command = operation.create_request()
             if command is not None:
-                self.__session._request_executor.execute(command, self.__session.session_info)
+                self._session._request_executor.execute(command, self._session.session_info)
                 if stream:
                     try:
                         result = command.result
                         stream_to_dict = json.loads(stream.decode("utf-8"))
                         result.__dict__.update(stream_to_dict)
                     except IOError as e:
                         raise RuntimeError(f"Unable to serialize returned value into stream {e.args[0]}", e)
                 else:
                     operation.set_result(command.result)
             return command
 
         def load_starting_with(
             self,
-            object_type: type,
             id_prefix: str,
-            matches: str,
-            start: int,
-            page_size: int,
-            exclude: str,
-            start_after: str,
-        ) -> object:
-            load_starting_with_operation = LoadStartingWithOperation(self.__session)
-            self.__load_starting_with_internal(
-                id_prefix, load_starting_with_operation, None, matches, start, page_size, exclude, start_after
+            object_type: Optional[Type[_T]] = None,
+            matches: Optional[str] = None,
+            start: Optional[int] = None,
+            page_size: Optional[int] = None,
+            exclude: Optional[str] = None,
+            start_after: Optional[str] = None,
+        ) -> List[_T]:
+            return self._session.load_starting_with(
+                id_prefix, object_type, matches, start, page_size, exclude, start_after
             )
 
         def load_starting_with_into_stream(
             self,
             id_prefix: str,
             output: bytes,
             matches: str = None,
@@ -743,37 +751,37 @@
         ):
             if not output:
                 raise ValueError("Output cannot be None")
             if not id_prefix:
                 raise ValueError("Id prefix cannot be None")
             self.__load_starting_with_internal(
                 id_prefix,
-                LoadStartingWithOperation(self.__session),
+                LoadStartingWithOperation(self._session),
                 output,
                 matches,
                 start,
                 page_size,
                 exclude,
                 start_after,
             )
 
         def load_into_stream(self, keys: List[str], output: bytes) -> None:
             if keys is None:
                 raise ValueError("Keys cannot be None")
 
-            self.__session.__load_internal_stream(keys, LoadOperation(self.__session), output)
+            self._session.__load_internal_stream(keys, LoadOperation(self._session), output)
 
         def __try_merge_patches(self, document_key: str, patch_request: PatchRequest) -> bool:
-            command = self.__session._deferred_commands_map.get(
+            command = self._session._deferred_commands_map.get(
                 IdTypeAndName.create(document_key, CommandType.PATCH, None)
             )
             if command is None:
                 return False
 
-            self.__session._deferred_commands.remove(command)
+            self._session._deferred_commands.remove(command)
             # We'll overwrite the deferredCommandsMap when calling Defer
             # No need to call deferredCommandsMap.remove((id, CommandType.PATCH, null));
 
             old_patch: PatchCommandData = command
             new_script = old_patch.patch.script + "\n" + patch_request.script
             new_vals = dict(old_patch.patch.values)
 
@@ -851,24 +859,24 @@
                 self.defer(PatchCommandData(key_or_entity, None, patch_request, None))
 
         def add_or_patch(self, key: str, entity: object, path_to_object: str, value: object) -> None:
             patch_request = PatchRequest()
             patch_request.script = f"this.{path_to_object} = args.val_{self.__vals_count}"
             patch_request.values = {f"val_{self.__vals_count}": value}
 
-            collection_name = self.__session._request_executor.conventions.get_collection_name(entity)
-            python_type = self.__session._request_executor.conventions.get_python_class_name(type(entity))
+            collection_name = self._session._request_executor.conventions.get_collection_name(entity)
+            python_type = self._session._request_executor.conventions.get_python_class_name(type(entity))
 
             metadata_as_dictionary = MetadataAsDictionary()
             metadata_as_dictionary[constants.Documents.Metadata.COLLECTION] = collection_name
             metadata_as_dictionary[constants.Documents.Metadata.RAVEN_PYTHON_TYPE] = python_type
 
             document_info = DocumentInfo(key, collection=collection_name, metadata_instance=metadata_as_dictionary)
 
-            new_instance = self.__session.entity_to_json.convert_entity_to_json(entity, document_info)
+            new_instance = self._session.entity_to_json.convert_entity_to_json(entity, document_info)
 
             self.__vals_count += 1
 
             patch_command_data = PatchCommandData(key, None, patch_request)
             patch_command_data.create_if_missing = new_instance
             self.defer(patch_command_data)
 
@@ -880,24 +888,24 @@
 
             list_adder(script_array)
 
             patch_request = PatchRequest()
             patch_request.script = script_array.script
             patch_request.values = script_array.parameters
 
-            collection_name = self.__session._request_executor.conventions.get_collection_name(entity)
-            python_type = self.__session._request_executor.conventions.get_python_class_name(type(entity))
+            collection_name = self._session._request_executor.conventions.get_collection_name(entity)
+            python_type = self._session._request_executor.conventions.get_python_class_name(type(entity))
 
             metadata_as_dictionary = MetadataAsDictionary()
             metadata_as_dictionary[constants.Documents.Metadata.COLLECTION] = collection_name
             metadata_as_dictionary[constants.Documents.Metadata.RAVEN_PYTHON_TYPE] = python_type
 
             document_info = DocumentInfo(key, collection=collection_name, metadata_instance=metadata_as_dictionary)
 
-            new_instance = self.__session.entity_to_json.convert_entity_to_json(entity, document_info)
+            new_instance = self._session.entity_to_json.convert_entity_to_json(entity, document_info)
 
             self.__vals_count += 1
 
             patch_command_data = PatchCommandData(key, None, patch_request)
             patch_command_data.create_if_missing = new_instance
             self.defer(patch_command_data)
 
@@ -905,24 +913,24 @@
             variable = f"this.{path_to_object}"
             value = f"args.val_{self.__vals_count}"
 
             patch_request = PatchRequest()
             patch_request.script = f"{variable} = {variable} ? {variable} + {value} : {value}"
             patch_request.values = {f"val_{self.__vals_count}": val_to_add}
 
-            collection_name = self.__session._request_executor.conventions.get_collection_name(entity)
-            python_type = self.__session._request_executor.conventions.find_python_class_name(entity.__class__)
+            collection_name = self._session._request_executor.conventions.get_collection_name(entity)
+            python_type = self._session._request_executor.conventions.find_python_class_name(entity.__class__)
 
             metadata_as_dictionary = MetadataAsDictionary()
             metadata_as_dictionary[constants.Documents.Metadata.COLLECTION] = collection_name
             metadata_as_dictionary[constants.Documents.Metadata.RAVEN_PYTHON_TYPE] = python_type
 
             document_info = DocumentInfo(key, collection=collection_name, metadata_instance=metadata_as_dictionary)
 
-            new_instance = self.__session.entity_to_json.convert_entity_to_json(entity, document_info)
+            new_instance = self._session.entity_to_json.convert_entity_to_json(entity, document_info)
 
             self.__vals_count += 1
 
             patch_command_data = PatchCommandData(key, None, patch_request)
             patch_command_data.create_if_missing = new_instance
             self.defer(patch_command_data)
 
@@ -950,41 +958,41 @@
         def conditional_load(
             self, key: str, change_vector: str, object_type: Type[_T] = None
         ) -> ConditionalLoadResult[_T]:
             if key is None or key.isspace():
                 raise ValueError("Key cannot be None")
 
             if self.is_loaded(key):
-                entity = self.__session.load(key, object_type)
+                entity = self._session.load(key, object_type)
                 if entity is None:
                     return ConditionalLoadResult.create(None, None)
 
                 cv = self.get_change_vector_for(entity)
                 return ConditionalLoadResult.create(entity, cv)
 
             if change_vector is None or change_vector.isspace():
                 raise ValueError(
                     f"The requested document with id '{key}' is not loaded into the session "
                     f"and could not conditional load when change_vector is None or empty."
                 )
 
-            self.__session.increment_requests_count()
+            self._session.increment_requests_count()
 
             cmd = ConditionalGetDocumentsCommand(key, change_vector)
-            self.__session._request_executor.execute_command(cmd)
+            self._session._request_executor.execute_command(cmd)
 
             if cmd.status_code == http.HTTPStatus.NOT_MODIFIED:
                 return ConditionalLoadResult.create(None, change_vector)  # value not changed
 
             elif cmd.status_code == http.HTTPStatus.NOT_FOUND:
-                self.__session.register_missing(key)
+                self._session.register_missing(key)
                 return ConditionalLoadResult.create(None, None)  # value is missing
 
             document_info = DocumentInfo.get_new_document_info(cmd.result.results[0])
-            r = self.__session.track_entity_document_info(object_type, document_info)
+            r = self._session.track_entity_document_info(object_type, document_info)
             return ConditionalLoadResult.create(r, cmd.result.change_vector)
 
             # todo: stream, query and fors like timeseriesrollupfor, conditional load
 
         class _Attachment:
             def __init__(self, session: DocumentSession):
                 self.__session = session
@@ -1059,15 +1067,15 @@
                         "Can't store attachment "
                         + name
                         + " of document"
                         + entity_or_document_id
                         + ", the document was already deleted in this session."
                     )
 
-                self.__session._defer(
+                self.__session.defer(
                     PutAttachmentCommandData(entity_or_document_id, name, stream, content_type, change_vector)
                 )
 
             def delete(self, entity_or_document_id, name):
                 if not isinstance(entity_or_document_id, str):
                     entity = self.__session._documents_by_entity.get(entity_or_document_id, None)
                     if not entity:
@@ -1099,15 +1107,15 @@
 
                 if (
                     IdTypeAndName.create(entity_or_document_id, CommandType.ATTACHMENT_MOVE, name)
                     in self.__session._deferred_commands_map
                 ):
                     self.__throw_other_deferred_command_exception(entity_or_document_id, name, "delete", "rename")
 
-                self.__session._defer(DeleteAttachmentCommandData(entity_or_document_id, name, None))
+                self.__session.defer(DeleteAttachmentCommandData(entity_or_document_id, name, None))
 
             def get(
                 self,
                 entity_or_document_id: str = None,
                 name: str = None,
                 # att_requests: Optional[List[AttachmentRequest]] = None,
                 # todo: fetching multiple attachments with single command
@@ -1204,15 +1212,15 @@
                     IdTypeAndName.create(
                         destination_entity_or_document_id, CommandType.ATTACHMENT_MOVE, destination_name
                     )
                     in self.__session._deferred_commands_map
                 ):
                     self.__throw_other_deferred_command_exception(entity_or_document_id, source_name, "copy", "rename")
 
-                self.__session._defer(
+                self.__session.defer(
                     CopyAttachmentCommandData(
                         entity_or_document_id, source_name, destination_entity_or_document_id, destination_name, None
                     )
                 )
 
             def rename(self, entity_or_document_id: Union[str, object], name: str, new_name: str) -> None:
                 self.move(entity_or_document_id, name, entity_or_document_id, new_name)
@@ -1303,15 +1311,15 @@
                     )
                     in self.__session._deferred_commands_map
                 ):
                     self.__throw_other_deferred_command_exception(
                         source_entity_or_document_id, destination_name, "rename", "rename"
                     )
 
-                self.__session._defer(
+                self.__session.defer(
                     MoveAttachmentCommandData(
                         source_entity_or_document_id,
                         source_name,
                         destination_entity_or_document_id,
                         destination_name,
                         None,
                     )
@@ -1395,7 +1403,235 @@
                 )
                 index_class_or_name = index_class_or_name.index_name
             index_name_and_collection = self.session._process_query_parameters(
                 object_type, index_class_or_name, collection_name, self.session.conventions
             )
             index_name = index_name_and_collection[0]
             collection_name = index_name_and_collection[1]
+
+
+class SessionCountersBase:
+    def __init__(self, session: InMemoryDocumentSessionOperations, document_id_or_entity: Union[str, object]):
+        if isinstance(document_id_or_entity, str):
+            if not document_id_or_entity or document_id_or_entity.isspace():
+                raise ValueError("Document id cannot be empty")
+
+            self.doc_id = document_id_or_entity
+            self.session = session
+        else:
+            document = session._documents_by_entity.get(document_id_or_entity)
+            if document is None:
+                self._throw_entity_not_in_session(document_id_or_entity)
+                return
+            self.doc_id = document.key
+            self.session = session
+
+    def increment(self, counter: str, delta: int = 1) -> None:
+        if not counter or counter.isspace():
+            raise ValueError("Counter name cannot be empty")
+
+        counter_op = CounterOperation(counter, CounterOperationType.INCREMENT, delta)
+        document_info = self.session._documents_by_id.get_value(self.doc_id)
+        if document_info is not None and document_info.entity in self.session._deleted_entities:
+            self._throw_document_already_deleted_in_session(self.doc_id, counter)
+
+        command = self.session._deferred_commands_map.get(
+            IdTypeAndName.create(self.doc_id, CommandType.COUNTERS, None), None
+        )
+        if command is not None:
+            counters_batch_command_data: CountersBatchCommandData = command
+            if counters_batch_command_data.has_delete(counter):
+                self._throw_increment_counter_after_delete_attempt(self.doc_id, counter)
+
+            counters_batch_command_data.counters.operations.append(counter_op)
+        else:
+            self.session.defer(CountersBatchCommandData(self.doc_id, counter_op))
+
+    def delete(self, counter: str) -> None:
+        if not counter or counter.isspace():
+            raise ValueError("Counter name is required")
+
+        if IdTypeAndName.create(self.doc_id, CommandType.DELETE, None) in self.session._deferred_commands_map:
+            return  # no-op
+
+        document_info = self.session._documents_by_id.get_value(self.doc_id)
+        if document_info is not None and document_info.entity in self.session._deleted_entities:
+            return  # no-op
+
+        counter_op = CounterOperation(counter, CounterOperationType.DELETE)
+
+        command = self.session._deferred_commands_map.get(
+            IdTypeAndName.create(self.doc_id, CommandType.COUNTERS, None), None
+        )
+        if command is not None:
+            counters_batch_command_data: CountersBatchCommandData = command
+            if counters_batch_command_data.has_increment(counter):
+                self._throw_delete_counter_after_increment_attempt(self.doc_id, counter)
+
+            counters_batch_command_data.counters.operations.append(counter_op)
+        else:
+            self.session.defer(CountersBatchCommandData(self.doc_id, counter_op))
+
+        cache = self.session.counters_by_doc_id.get(self.doc_id, None)
+        if cache is not None:
+            del cache[1][counter]
+
+    def _throw_entity_not_in_session(self, entity) -> None:
+        raise ValueError(
+            "Entity is not associated with the session, cannot add counter to it. "
+            "Use document_id instead of track the entity in the session."
+        )
+
+    @staticmethod
+    def _throw_increment_counter_after_delete_attempt(document_id: str, counter: str) -> None:
+        raise ValueError(
+            f"Can't increment counter {counter} of document {document_id}, "
+            f"there is a deferred command registered to delete a counter with the same name."
+        )
+
+    @staticmethod
+    def _throw_delete_counter_after_increment_attempt(document_id: str, counter: str) -> None:
+        raise ValueError(
+            f"Can't delete counter {counter} of document {document_id}, "
+            f"there is a deferred command registered to increment a counter with the same name."
+        )
+
+    @staticmethod
+    def _throw_document_already_deleted_in_session(document_id: str, counter: str) -> None:
+        raise ValueError(
+            f"Can't increment counter {counter} of document {document_id}, "
+            f"the document was already deleted in this session"
+        )
+
+
+class SessionDocumentCounters(SessionCountersBase):
+    def get_all(self) -> Dict[str, int]:
+        cache = self.session.counters_by_doc_id.get(self.doc_id, None)
+
+        if cache is None:
+            cache = [False, CaseInsensitiveDict()]
+
+        missing_counters = not cache[0]
+
+        document = self.session._documents_by_id.get_value(self.doc_id)
+        if document is not None:
+            metadata_counters: Dict = document.metadata.get(constants.Documents.Metadata.COUNTERS, None)
+            if metadata_counters is None:
+                missing_counters = False
+            elif len(cache[1]) >= len(metadata_counters):
+                missing_counters = False
+
+                for c in metadata_counters:
+                    if c in cache[1]:
+                        continue
+                    missing_counters = True
+                    break
+
+        if missing_counters:
+            # we either don't have the document in session and got_all = False,
+            # or we do and cache doesn't contain all metadata counters
+
+            self.session.increment_requests_count()
+
+            details = self.session.operations.send(GetCountersOperation(self.doc_id), self.session.session_info)
+            cache[1].clear()
+
+            for counter_detail in details.counters:
+                cache[1][counter_detail.counter_name] = counter_detail.total_value
+
+        cache[0] = True
+
+        if not self.session.no_tracking:
+            self.session.counters_by_doc_id[self.doc_id] = cache
+
+        return cache[1]
+
+    def get(self, counter) -> int:
+        value = None
+
+        cache = self.session.counters_by_doc_id.get(self.doc_id, None)
+        if cache is not None:
+            value = cache[1].get(counter, None)
+            if counter in cache[1]:
+                return value
+        else:
+            cache = [False, CaseInsensitiveDict()]
+
+        document = self.session._documents_by_id.get_value(self.doc_id)
+        metadata_has_counter_name = False
+        if document is not None:
+            metadata_counters = document.metadata.get(constants.Documents.Metadata.COUNTERS, None)
+            if metadata_counters is not None:
+                for node in metadata_counters:
+                    if node.lower() == counter.lower():
+                        metadata_has_counter_name = True
+
+        if (document is None and not cache[0]) or metadata_has_counter_name:
+            # we either don't have the document in session and got_all = False,
+            # or we do and it's metadata contains the counter name
+
+            self.session.increment_requests_count()
+
+            details = self.session.operations.send(
+                GetCountersOperation(self.doc_id, counter), self.session.session_info
+            )
+            if details.counters:
+                counter_detail = details.counters[0]
+                value = counter_detail.total_value if counter_detail is not None else None
+
+        cache[1][counter] = value
+        if not self.session.no_tracking:
+            self.session.counters_by_doc_id[self.doc_id] = cache
+
+        return value
+
+    def get_many(self, counters: List[str]) -> Dict[str, int]:
+        cache = self.session.counters_by_doc_id.get(self.doc_id, None)
+        if cache is None:
+            cache = [False, CaseInsensitiveDict()]
+
+        metadata_counters = None
+        document = self.session._documents_by_id.get_value(self.doc_id)
+        if document is not None:
+            metadata_counters = document.metadata.get(constants.Documents.Metadata.COUNTERS, None)
+
+        result = {}
+
+        for counter in counters:
+            has_counter = counter in cache[1]
+            val = cache[1].get(counter, None)
+            not_in_metadata = True
+
+            if document is not None and metadata_counters is not None:
+                for metadata_counter in metadata_counters:
+                    if metadata_counter.lower() == counter.lower():
+                        not_in_metadata = False
+
+            if has_counter or cache[0] or (document is not None and not_in_metadata):
+                # we either have value in cache
+                # or we have the metadata and the counter is not there,
+                # or got_all
+
+                result[counter] = val
+                continue
+
+            result.clear()
+
+            self.session.increment_requests_count()
+
+            details = self.session.operations.send(
+                GetCountersOperation(self.doc_id, copy.deepcopy(counters), self.session.session_info)
+            )
+
+            for counter_detail in details.counters:
+                if counter_detail is None:
+                    continue
+
+                cache[1][counter_detail.counter_name] = counter_detail.total_value
+                result[counter_detail.counter_name] = counter_detail.total_value
+
+            break
+
+        if self.session.no_tracking:
+            self.session.counters_by_doc_id[self.doc_id] = cache
+
+        return result
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/entity_to_json.py` & `ravendb-5.2.3/ravendb/documents/session/entity_to_json.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/event_args.py` & `ravendb-5.2.3/ravendb/documents/session/event_args.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/in_memory_document_session_operations.py` & `ravendb-5.2.3/ravendb/documents/session/in_memory_document_session_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         self.__deleted_entities.clear()
         if self.__on_before_deleted_entities:
             self.__on_before_deleted_entities.clear()
 
     def evict(self, entity) -> None:
         if self.__prepare_entities_deleted:
             raise RuntimeError("Cannot evict entity during OnBeforeDelete")
-        self.__deleted_entities.remove(RefEq(entity))
+        self.__deleted_entities.discard(RefEq(entity))
 
     class DeletedEntitiesEnumeratorResult:
         def __init__(self, entity: object, execute_on_before_delete: bool):
             self.__entity = entity
             self.__execute_on_before_delete = execute_on_before_delete
 
         @property
@@ -455,15 +455,15 @@
         )
 
         self._known_missing_ids = CaseInsensitiveSet()
         self._documents_by_id = DocumentsByIdHolder()
         self._included_documents_by_id = CaseInsensitiveDict()
         self._documents_by_entity: DocumentsByEntityHolder = DocumentsByEntityHolder()
 
-        self._counters_by_doc_id: Dict[str, List[bool, Dict[str, int]]] = {}
+        self._counters_by_doc_id: Dict[str, List[Dict[str, int]]] = CaseInsensitiveDict()
         self._time_series_by_doc_id: Dict[str, Dict[str, List[TimeSeriesRangeResult]]] = {}
 
         self._deleted_entities: Union[
             Set[DeletedEntitiesHolder.DeletedEntitiesEnumeratorResult], DeletedEntitiesHolder
         ] = DeletedEntitiesHolder()
         self._deferred_commands: List[CommandData] = []
         self._deferred_commands_map: Dict[IdTypeAndName, CommandData] = {}
@@ -588,15 +588,15 @@
             event(before_delete_event_args)
 
     def before_query_invoke(self, before_query_event_args: BeforeQueryEventArgs):
         for event in self.__before_query:
             event(before_query_event_args)
 
     @property
-    def operation_executor(self) -> OperationExecutor:
+    def operations(self) -> OperationExecutor:
         return self._operation_executor
 
     @property
     def conventions(self) -> DocumentConventions:
         return self._request_executor.conventions
 
     @property
@@ -797,15 +797,15 @@
                 self._documents_by_id.pop(key, None)
                 change_vector = document_info.change_vector
 
             self._known_missing_ids.add(key)
             change_vector = change_vector if self.__use_optimistic_concurrency else None
             if self._counters_by_doc_id:
                 self._counters_by_doc_id.pop(key, None)
-            self._defer(DeleteCommandData(key, expected_change_vector if expected_change_vector else change_vector))
+            self.defer(DeleteCommandData(key, expected_change_vector if expected_change_vector else change_vector))
             return
 
         entity = key_or_entity
         if entity is None:
             raise ValueError("Entity cannot be None")
 
         value = self._documents_by_entity.get(entity)
@@ -1149,20 +1149,20 @@
             self.__update_metadata_modifications(value)
             new_obj = self.entity_to_json.convert_entity_to_json(value.entity, value)
             self._entity_changed(new_obj, value, changes)
 
     def ignore_changes_for(self, entity: object) -> None:
         self._get_document_info(entity).ignore_changes = True
 
-    def _defer(self, *commands: CommandData) -> None:
+    def defer(self, *commands: CommandData) -> None:
         self._deferred_commands.extend(commands)
         for command in commands:
-            self.__defer_internal(command)
+            self._defer_internal(command)
 
-    def __defer_internal(self, command: CommandData) -> None:
+    def _defer_internal(self, command: CommandData) -> None:
         if command.command_type is CommandType.BATCH_PATCH:
             command: BatchPatchCommandData
             for kvp in command.ids:
                 self.__add_command(command, kvp.key, CommandType.PATCH, command.name)
             return
         self.__add_command(command, command.key, command.command_type, command.name)
 
@@ -1240,46 +1240,52 @@
 
         for result in results:
             for include in include_paths:
                 if constants.Documents.Indexing.Fields.DOCUMENT_ID_FIELD_NAME == include:
                     continue
                 IncludesUtil.include(result, include, __include)
 
+    def register_counters_ids_list(
+        self, result_counters: dict, keys: List[str], counters_to_include: List[str], got_all: bool
+    ) -> None:
+        if self.no_tracking:
+            return
+
+        if not result_counters:
+            if got_all:
+                for key in keys:
+                    self.__set_got_all_counters_for_document(key)
+
+                return
+        else:
+            self._register_counters_internal(result_counters, None, False, got_all)
+
+        self.__register_missing_counters_for_keys(keys, counters_to_include)
+
     def register_counters(
         self,
         result_counters: dict,
-        counters_to_include: Union[Dict[str, List[str]], List[str]],
-        keys: List[str] = None,
-        got_all: bool = None,
-    ):
-        keys_case = keys is not None and got_all is not None
+        counters_to_include: Dict[str, List[str]],
+    ) -> None:
         if self.no_tracking:
             return
+
         if not result_counters:
-            if keys_case:
-                if got_all:
-                    for key in keys:
-                        self.__set_got_all_counters_for_document(key)
-                    return
-            else:
-                self.__set_got_all_in_cache_if_needed(counters_to_include)
+            self.__set_got_all_in_cache_if_needed(counters_to_include)
         else:
-            self._register_counters_internal(
-                result_counters,
-                {} if keys_case else counters_to_include,
-                not keys_case,
-                got_all if keys_case else False,
-            )
+            self._register_counters_internal(result_counters, counters_to_include, True, False)
 
-        self.__register_missing_counters_for_keys(
-            keys, counters_to_include
-        ) if keys_case else self.__register_missing_counters(counters_to_include)
+        self.__register_missing_counters(counters_to_include)
 
     def _register_counters_internal(
-        self, result_counters: dict, counters_to_include: Dict[str, List[str]], from_query_result: bool, got_all: bool
+        self,
+        result_counters: dict,
+        counters_to_include: Optional[Dict[str, List[str]]],
+        from_query_result: bool,
+        got_all: bool,
     ):
         for key, result_counters in result_counters.items():
             if not result_counters:
                 continue
             counters = []
             if from_query_result:
                 counters = counters_to_include.get(key, None)
@@ -1357,16 +1363,16 @@
 
     def __register_missing_counters_for_keys(self, keys: List[str], counters_to_include: List[str]):
         if not counters_to_include:
             return
 
         for counter in counters_to_include:
             for key in keys:
-                cache = self._counters_by_doc_id.get(key)
-                if not cache:
+                cache = self._counters_by_doc_id.get(key, None)
+                if cache is None:
                     cache = [False, CaseInsensitiveDict()]
                     self._counters_by_doc_id[key] = cache
 
                 if counter in cache[1]:
                     continue
 
                 cache[1][counter] = None
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/loaders/include.py` & `ravendb-5.2.3/ravendb/documents/session/loaders/include.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import datetime
-from typing import Set, Tuple, Dict, Union, Optional
+from typing import Set, Tuple, Dict, Union, Optional, List
 from ravendb.documents.conventions import DocumentConventions
 from ravendb.data.timeseries import TimeSeriesRange
 from ravendb.tools.utils import CaseInsensitiveDict, CaseInsensitiveSet
 
 
 class IncludeBuilderBase:
     def __init__(self, conventions: DocumentConventions):
@@ -39,51 +39,48 @@
     def _include_compare_exchange_value(self, path: str) -> None:
         if self._compare_exchange_values_to_include is None:
             self._compare_exchange_values_to_include = {}
         self._compare_exchange_values_to_include.add(path)
 
     def _include_counter_with_alias(self, path: str, *names: str) -> None:
         self._with_alias()
-        self._include_counters(path, *names)
+        self._include_counters(path, list(names) if isinstance(names, tuple) else [names])
 
     def _include_documents(self, path: str):
         if not self._documents_to_include:
             self._documents_to_include = set()
         self._documents_to_include.add(path)
 
-    def _include_counters(self, path: str, *names: str):
+    def _include_counters(self, path: str, names: List[str]):
         if not names:
             raise ValueError("Expected at least one name")
 
         self._assert_not_all_and_add_new_entry_if_needed(path)
         for name in names:
             if name.isspace():
                 raise ValueError("Counters(names): 'names' should not contain null or whitespace elements")
-            if isinstance(name, list):
-                self._include_counters(path, *name)
-                continue
             self._counters_to_include_by_source_path.get(path)[1].add(name)
 
     def _include_all_counters_with_alias(self, path: str):
         self._with_alias()
         self._include_all_counters(path)
 
     def _include_all_counters(self, source_path: str):
         if self._counters_to_include_by_source_path is None:
             self._counters_to_include_by_source_path = CaseInsensitiveDict()
         val = self._counters_to_include_by_source_path.get(source_path)
         if val is not None and val[1] is not None:
-            raise ValueError("You cannot use all_counters() after using counters(*names)")
+            raise RuntimeError("You cannot use all_counters() after using counters(*names)")
         self._counters_to_include_by_source_path[source_path] = (True, None)
 
     def _assert_not_all_and_add_new_entry_if_needed(self, path: str):
         if self._counters_to_include_by_source_path is not None:
             val = self._counters_to_include_by_source_path.get(path, None)
             if val is not None and val[0]:
-                raise ValueError("You cannot use counters(*names) after using all_counters()")
+                raise RuntimeError("You cannot use counters(*names) after using all_counters()")
 
         if self._counters_to_include_by_source_path is None:
             self._counters_to_include_by_source_path = CaseInsensitiveDict()
 
         if path not in self._counters_to_include_by_source_path:
             self._counters_to_include_by_source_path[path] = (False, CaseInsensitiveSet())
 
@@ -112,16 +109,21 @@
     def __init__(self, conventions: DocumentConventions):
         super(IncludeBuilder, self).__init__(conventions)
 
     def include_documents(self, path: str) -> IncludeBuilderBase:
         self._include_documents(path)
         return self
 
-    def include_counter(self, *names: str) -> IncludeBuilderBase:
-        self._include_counters("", *names)
+    def include_counter(self, name: str) -> IncludeBuilderBase:
+        self._include_counters("", [name])
+        return self
+
+    def include_counters(self, *names: str) -> IncludeBuilderBase:
+        for name in names:
+            self.include_counter(name)
         return self
 
     def include_all_counters(self) -> IncludeBuilderBase:
         self._include_all_counters("")
         return self
 
     def include_time_series(
@@ -136,16 +138,20 @@
 
     def include_compare_exchange_value(self, path: str) -> IncludeBuilderBase:
         super(IncludeBuilder, self)._include_compare_exchange_value(path)
         return self
 
 
 class QueryIncludeBuilder(IncludeBuilderBase):
+    def include_counter(self, name: str, path: Optional[str] = ""):
+        self._include_counter_with_alias(path, name)
+        return self
+
     def include_counters(self, *names: str, path: Optional[str] = ""):
-        self._include_counter_with_alias(path, *names)
+        self._include_counter_with_alias(path, *names if isinstance(names, tuple) else names)
         return self
 
     def include_all_counters(self, path: Optional[str] = ""):
         self._include_all_counters_with_alias(path)
         return self
 
     def include_documents(self, path: str):
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/loaders/loaders.py` & `ravendb-5.2.3/ravendb/documents/session/loaders/loaders.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/misc.py` & `ravendb-5.2.3/ravendb/documents/session/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/operations/lazy.py` & `ravendb-5.2.3/ravendb/documents/session/operations/lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,16 @@
         elif isinstance(ids, list):
             return self._delegate.lazy_load_internal(object_type, ids, [], on_eval)
 
         raise TypeError("Expected 'ids' as 'str' or 'list[str]'")
 
     def load_starting_with(
         self,
-        object_type: Type[_T],
         id_prefix: str,
+        object_type: Optional[Type[_T]],
         matches: str = None,
         start: int = 0,
         page_size: int = 25,
         exclude: str = None,
         start_after: str = None,
     ) -> Lazy[Dict[str, _T]]:
         operation = LazyStartsWithOperation(
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/operations/load_operation.py` & `ravendb-5.2.3/ravendb/documents/session/operations/load_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         if not result:
             self._session.register_missing(*self._keys)
             return
 
         self._session.register_includes(result.includes)
 
         if self._include_all_counters or self._counters_to_include:
-            self._session.register_counters(
+            self._session.register_counters_ids_list(
                 result.counter_includes, self._keys, self._counters_to_include, self._include_all_counters
             )
 
         if self._time_series_to_include:
             self._session.register_time_series(result.time_series_includes)
 
         if self._compare_exchange_values_to_include:
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/operations/operations.py` & `ravendb-5.2.3/ravendb/documents/session/operations/operations.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/operations/query.py` & `ravendb-5.2.3/ravendb/documents/session/operations/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,18 @@
                 ),
             )
         if not self.__no_tracking:
             self.__session.register_missing_includes(
                 query_result.results, query_result.includes, query_result.included_paths
             )
 
-            # todo: counters and timeseries
             if query_result.counter_includes is not None:
-                raise NotImplementedError()
+                self.__session.register_counters(query_result.counter_includes, query_result.included_counter_names)
 
+            # todo: timeseries
             if query_result.time_series_includes is not None:
                 raise NotImplementedError()
 
             if query_result.compare_exchange_value_includes is not None:
                 self.__session.cluster_transaction.register_compare_exchange_values(
                     query_result.compare_exchange_value_includes
                 )
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/query.py` & `ravendb-5.2.3/ravendb/documents/session/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     HighlightingToken,
     ExplanationToken,
     TimingsToken,
     IntersectMarkerToken,
     DistinctToken,
     ShapeToken,
     SuggestToken,
+    CounterIncludesToken,
 )
 from ravendb.documents.session.utils.document_query import DocumentQueryHelper
 from ravendb.documents.session.utils.includes_util import IncludesUtil
 from ravendb.tools.utils import Utils
 
 _T = TypeVar("_T")
 _TResult = TypeVar("_TResult")
@@ -97,19 +98,19 @@
 
 
 class AbstractDocumentQuery(Generic[_T]):
     def __init__(
         self,
         object_type: Type[_T],
         session: "InMemoryDocumentSessionOperations",
-        index_name: Union[None, str],
-        collection_name: Union[None, str],
+        index_name: Optional[str],
+        collection_name: Optional[str],
         is_group_by: bool,
-        declare_tokens: Union[None, List[DeclareToken]],
-        load_tokens: Union[None, List[LoadToken]],
+        declare_tokens: Optional[List[DeclareToken]],
+        load_tokens: Optional[List[LoadToken]],
         from_alias: Optional[str] = None,
         is_project_into: Optional[bool] = False,
     ):
         self._object_type = object_type
         self._root_types = {object_type}
         self._is_group_by = is_group_by
         self.__index_name = index_name
@@ -117,56 +118,57 @@
         self._from_token = FromToken.create(index_name, collection_name, from_alias)
         self._declare_tokens = declare_tokens
         self._load_tokens = load_tokens
         self._the_session = session
         self.__conventions = DocumentConventions() if session is None else session.conventions
         self.is_project_into = is_project_into if is_project_into is not None else False
 
-        self._is_intersect: Union[None, bool] = None
-        self.__is_in_more_like_this: Union[None, bool] = None
-        self._includes_alias: Union[None, str] = None
-        self._negate: Union[None, bool] = None
-        self._query_raw: Union[None, str] = None
+        self._is_intersect: Optional[bool] = None
+        self.__is_in_more_like_this: Optional[bool] = None
+        self._includes_alias: Optional[str] = None
+        self._negate: Optional[bool] = None
+        self._query_raw: Optional[str] = None
         self._query_parameters: Dict[str, object] = {}
         self.__alias_to_group_by_field_name: Dict[str, str] = {}
 
         self._document_includes: Set[str] = set()
-        self._page_size: Union[None, int] = None
-        self._start: Union[None, int] = None
+        self._page_size: Optional[int] = None
+        self._start: Optional[int] = None
         self.__current_clause_depth: int = 0
 
         self._select_tokens: List[QueryToken] = []
-        self._fields_to_fetch_token: Union[None, FieldsToFetchToken] = None
+        self._fields_to_fetch_token: Optional[FieldsToFetchToken] = None
         self._where_tokens: List[QueryToken] = []
         self._group_by_tokens: List[QueryToken] = []
         self._order_by_tokens: List[QueryToken] = []
         self._with_tokens: List[QueryToken] = []
         self._compare_exchange_includes_tokens: List[CompareExchangeValueIncludesToken] = []
         self._highlighting_tokens: List[HighlightingToken] = []
         self._query_highlightings: QueryHighlightings = QueryHighlightings()
-        self._explanation_token: Union[None, ExplanationToken] = None
-        self._explanations: Union[None, Explanations] = None
+        self._explanation_token: Optional[ExplanationToken] = None
+        self._explanations: Optional[Explanations] = None
+        self._counter_includes_tokens: Optional[List[CounterIncludesToken]] = None
 
         self._before_query_executed_callback: List[Callable[[IndexQuery], None]] = []
         self._after_query_executed_callback: List[Callable[[QueryResult], None]] = [
             self.__update_stats_highlightings_and_explanations
         ]
         self._after_stream_executed_callback: List[Callable[[Dict], None]] = []
 
         self._query_stats = QueryStatistics()
-        self._disable_entities_tracking: Union[None, bool] = None
-        self._disable_caching: Union[None, bool] = None
-        self._projection_behavior: Union[None, ProjectionBehavior] = None
+        self._disable_entities_tracking: Optional[bool] = None
+        self._disable_caching: Optional[bool] = None
+        self._projection_behavior: Optional[ProjectionBehavior] = None
         self.parameter_prefix = "p"
-        self._query_timings: Union[None, QueryTimings] = None
+        self._query_timings: Optional[QueryTimings] = None
         self._default_operator = QueryOperator.AND
-        self._the_wait_for_non_stale_results: Union[None, bool] = None
-        self._timeout: Union[None, datetime.timedelta] = None
+        self._the_wait_for_non_stale_results: Optional[bool] = None
+        self._timeout: Optional[datetime.timedelta] = None
 
-        self._query_operation: Union[None, QueryOperation] = None
+        self._query_operation: Optional[QueryOperation] = None
 
     @property
     def conventions(self) -> DocumentConventions:
         return self.__conventions
 
     @property
     def query_operation(self) -> QueryOperation:
@@ -207,15 +209,15 @@
 
     def _using_default_operator(self, operator: QueryOperator) -> None:
         if not self._where_tokens:
             raise RuntimeError("Default operator can only be set before any where clause is added")
 
         self._default_operator = operator
 
-    def _wait_for_non_stale_results(self, wait_timeout: Union[None, datetime.timedelta]) -> None:
+    def _wait_for_non_stale_results(self, wait_timeout: Optional[datetime.timedelta]) -> None:
         # Graph queries may set this property multiple times
         if self._the_wait_for_non_stale_results:
             if self._timeout is None or (wait_timeout is not None and self._timeout.seconds < wait_timeout.seconds):
                 self._timeout = wait_timeout
             return
 
         self._the_wait_for_non_stale_results = True
@@ -363,15 +365,15 @@
             includes = path_or_include_builder
             if includes is None:
                 return
             if includes._documents_to_include is not None:
                 self._document_includes.update(includes._documents_to_include)
 
             # todo: counters and time series includes
-            # self._include_counters(includes.alias, includes.counters_to_include_by_source_path)
+            self._include_counters(includes._alias, includes._counters_to_include_by_source_path)
             # if includes.time_series_to_include_by_source_alias is not None:
             #     self._include_time_series(includes.alias, includes.time_series_to_include_by_source_alias)
             if includes._compare_exchange_values_to_include is not None:
                 for compare_exchange_value in includes._compare_exchange_values_to_include:
                     self._compare_exchange_includes_tokens.append(
                         CompareExchangeValueIncludesToken.create(compare_exchange_value)
                     )
@@ -457,15 +459,15 @@
         if isinstance(where_params.value, MethodCall):
             mc = where_params.value
 
             args = []
             for arg in mc.args:
                 args.append(self.__add_query_parameter(arg))
 
-            token: Union[None, WhereToken] = None
+            token: Optional[WhereToken] = None
             object_type = type(mc)
             if object_type == CmpXchg:
                 token = WhereToken.create(
                     op,
                     where_params.field_name,
                     None,
                     WhereToken.WhereOptions(
@@ -914,15 +916,15 @@
     def __build_include(self, query_text: List[str]) -> None:
         if (
             not self._document_includes
             and not self._highlighting_tokens
             and self._explanation_token is None
             and self._query_timings is None
             and not self._compare_exchange_includes_tokens
-            # todo: and self._counter_includes_tokens is None
+            and self._counter_includes_tokens is None
             # todo: and self._time_series_includes_tokens is None
         ):
             return
 
         query_text.append(" include ")
         first = True
         for include in self._document_includes:
@@ -935,15 +937,15 @@
                 query_text.append("'")
                 query_text.append(escaped_include)
                 query_text.append("'")
             else:
                 query_text.append(include)
 
         # todo: counters & time series
-        # first = self.__write_include_tokens(self._counter_includes_tokens, first, query_text)
+        first = self.__write_include_tokens(self._counter_includes_tokens, first, query_text)
         # first = self.__write_include_tokens(self._time_series_includes_tokens, first, query_text)
         first = self.__write_include_tokens(self._compare_exchange_includes_tokens, first, query_text)
         first = self.__write_include_tokens(self._highlighting_tokens, first, query_text)
 
         if self._explanation_token is not None:
             if not first:
                 query_text.append(",")
@@ -1163,15 +1165,15 @@
                 nested_where_params.allow_wildcards = True
                 nested_where_params.field_name = field_name
                 nested_where_params.value = value
 
                 result.append(self.__transform_value(nested_where_params))
         return result
 
-    def __negate_if_needed(self, tokens: List[QueryToken], field_name: Union[None, str]) -> None:
+    def __negate_if_needed(self, tokens: List[QueryToken], field_name: Optional[str]) -> None:
         if not self._negate:
             return
 
         self._negate = False
 
         if not tokens or isinstance(tokens[-1], OpenSubclauseToken):
             if field_name is not None:
@@ -1256,20 +1258,23 @@
         if self._includes_alias is None:
             return from_alias
 
         if from_alias is None:
             from_alias = self._includes_alias
             self.add_from_alias_to_where_tokens(from_alias)
 
-        # todo: counter and time series tokens
+        if self._counter_includes_tokens is not None:
+            for counter_includes_token in self._counter_includes_tokens:
+                counter_includes_token.add_alias_to_path(from_alias)
+        # todo: time series tokens
 
         return from_alias
 
     @staticmethod
-    def _get_source_alias_if_exists(object_type: type, query_data: QueryData, fields: List[str]) -> Union[None, str]:
+    def _get_source_alias_if_exists(object_type: type, query_data: QueryData, fields: List[str]) -> Optional[str]:
         if len(fields) != 1 or fields[0] is None:
             return None
         try:
             index_of = fields[0].index(".")
         except ValueError:
             return None
 
@@ -1552,15 +1557,15 @@
         self._the_session.advanced.request_executor.execute_command(command, self._the_session.session_info)
         self._query_operation.set_result(command.result)
         self.invoke_after_query_executed(self._query_operation.current_query_results)
 
     def __iter__(self) -> Iterator[_T]:
         return self.__execute_query_operation(None).__iter__()
 
-    def __execute_query_operation(self, take: Union[None, int]) -> List[_T]:
+    def __execute_query_operation(self, take: Optional[int]) -> List[_T]:
         self.__execute_query_operation_internal(take)
 
         return self._query_operation.complete(self._object_type)
 
     def __execute_query_operation_internal(self, take: int) -> None:
         if take is not None and (self._page_size is None or self._page_size > take):
             self._take(take)
@@ -1599,15 +1604,15 @@
 
         lazy_query_operation = LazyQueryOperation(
             self._object_type, self._the_session, self._query_operation, self._after_query_executed_callback
         )
         self._the_session: "DocumentSession"
         return self._the_session.add_lazy_count_operation(self.lazy_query_operation)
 
-    def _suggest_using(self, suggestion: Union[None, SuggestionBase]) -> None:
+    def _suggest_using(self, suggestion: Optional[SuggestionBase]) -> None:
         if suggestion is None:
             raise ValueError("suggestion cannot be None")
 
         self.__assert_can_suggest(suggestion)
 
         if isinstance(suggestion, SuggestionWithTerm):
             term = suggestion
@@ -1660,17 +1665,33 @@
             raise RuntimeError("Duplicate IncludeExplanations method calls are forbidden.")
 
         options_parameter_name = self.__add_query_parameter(options) if options is not None else None
         self._explanation_token = ExplanationToken.create(options_parameter_name)
         self._explanations = Explanations()
         explanations_callback(self._explanations)
 
-    # todo: counters
-    def _include_counters(self, alias: str, counter_to_include_by_doc_id: Dict[str, Tuple[bool, Set[str]]]) -> None:
-        raise NotImplementedError()
+    def _include_counters(
+        self, alias: str, counter_to_include_by_doc_id: Optional[Dict[str, Tuple[bool, Set[str]]]]
+    ) -> None:
+        if not counter_to_include_by_doc_id:
+            return
+
+        self._counter_includes_tokens = []
+        self._includes_alias = alias
+
+        for key, value in counter_to_include_by_doc_id.items():
+            if value[0]:
+                self._counter_includes_tokens.append(CounterIncludesToken.all(key))
+                continue
+
+            if not value[1]:
+                continue
+
+            for name in value[1]:
+                self._counter_includes_tokens.append(CounterIncludesToken.create(key, name))
 
     # todo: time series
     # def _include_time_series(self, alias:str, time_series_to_include:Dict[str,Set[AbstractTimeSeriesRange]]) -> None:
     # pass
 
 
 class DocumentQuery(Generic[_T], AbstractDocumentQuery[_T]):
@@ -2037,15 +2058,15 @@
         query._query_parameters = Parameters(self._query_parameters)
         query._start = self._start
         query._timeout = self._timeout
         query._query_stats = self._query_stats
         query._the_wait_for_non_stale_results = self._the_wait_for_non_stale_results
         query._negate = self._negate
         query._document_includes = self._document_includes
-        # todo: self._counter_includes_tokens = self._counter_includes_tokens
+        query._counter_includes_tokens = self._counter_includes_tokens
         # todo: self._time_series_includes_tokens = self._time_series_includes_tokens
         query._compare_exchange_includes_tokens = self._compare_exchange_includes_tokens
         query._root_types = {self._object_type}
         query._before_query_executed_callback = self._before_query_executed_callback
         query._after_query_executed_callback = self._after_query_executed_callback
         query._after_stream_executed_callback = self._after_stream_executed_callback
         query._highlighting_tokens = self._highlighting_tokens
@@ -2342,17 +2363,17 @@
 
 
 class WhereParams:
     def __init__(self):
         self.nested_path = False
         self.allow_wildcards = False
 
-        self.field_name: Union[None, str] = None
-        self.value: Union[None, object] = None
-        self.exact: Union[None, bool] = None
+        self.field_name: Optional[str] = None
+        self.value: Optional[object] = None
+        self.exact: Optional[bool] = None
 
 
 class QueryStatistics:
     def __init__(
         self,
         is_stale: bool = None,
         duration_in_ms: float = None,
```

### Comparing `ravendb-5.2.2/ravendb/documents/session/query_group_by.py` & `ravendb-5.2.3/ravendb/documents/session/query_group_by.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/time_series/time_series.py` & `ravendb-5.2.3/ravendb/documents/session/time_series/time_series.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/tokens/misc.py` & `ravendb-5.2.3/ravendb/documents/session/tokens/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/definitions.py` & `ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/definitions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/facets.py` & `ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/facets.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/tokens/query_tokens/query_token.py` & `ravendb-5.2.3/ravendb/documents/session/tokens/query_tokens/query_token.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/session/utils/document_query.py` & `ravendb-5.2.3/ravendb/documents/session/utils/document_query.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/store/definition.py` & `ravendb-5.2.3/ravendb/documents/store/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,39 +360,44 @@
     def add_before_close(self, event: Callable[[], None]):
         self.__before_close.append(event)
 
     def remove_before_close(self, event: Callable[[], None]):
         self.__before_close.remove(event)
 
     def close(self):
+        if self._disposed:
+            return
         for event in self.__before_close:
             event()
 
         # todo: evict items from cache based on changes
 
         while len(self.__database_changes) > 0:
             self.__database_changes.popitem()[1].close()
 
         if self.__multi_db_hilo is not None:
             try:
                 self.__multi_db_hilo.return_unused_range()
             except Exception:
                 pass  # ignore
-        # todo: clear subscriptions
-        self._disposed = True
+
+        if self.subscriptions is not None:
+            self.subscriptions.close()
+
         for event in self.__after_close:
             event()
 
         for key, lazy in self.__request_executors.items():
             if not lazy.is_value_created:
                 continue
 
             lazy.value.close()
 
         self.__thread_pool_executor.shutdown()
+        self._disposed = True
 
     def open_session(
         self, database: Optional[str] = None, session_options: Optional[SessionOptions] = None
     ) -> DocumentSession:
         if not database and not session_options:
             session_options = SessionOptions()
         if not ((session_options is not None) ^ (database is not None)):
```

### Comparing `ravendb-5.2.2/ravendb/documents/store/lazy.py` & `ravendb-5.2.3/ravendb/documents/store/lazy.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/store/misc.py` & `ravendb-5.2.3/ravendb/documents/store/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/subscriptions/document_subscriptions.py` & `ravendb-5.2.3/ravendb/documents/subscriptions/document_subscriptions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/subscriptions/options.py` & `ravendb-5.2.3/ravendb/documents/subscriptions/options.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/subscriptions/state.py` & `ravendb-5.2.3/ravendb/documents/subscriptions/state.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/documents/subscriptions/worker.py` & `ravendb-5.2.3/ravendb/documents/subscriptions/worker.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/exceptions/documents/__init__.py` & `ravendb-5.2.3/ravendb/exceptions/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/exceptions/documents/bulkinsert.py` & `ravendb-5.2.3/ravendb/exceptions/documents/bulkinsert.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/exceptions/exception_dispatcher.py` & `ravendb-5.2.3/ravendb/exceptions/exception_dispatcher.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/exceptions/exceptions.py` & `ravendb-5.2.3/ravendb/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/exceptions/raven_exceptions.py` & `ravendb-5.2.3/ravendb/exceptions/raven_exceptions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/extensions/http_extensions.py` & `ravendb-5.2.3/ravendb/extensions/http_extensions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/extensions/json_extensions.py` & `ravendb-5.2.3/ravendb/extensions/json_extensions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/extensions/string_extensions.py` & `ravendb-5.2.3/ravendb/extensions/string_extensions.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/http/http_cache.py` & `ravendb-5.2.3/ravendb/http/http_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         http_cache_item.change_vector = change_vector
         http_cache_item.payload = result
         http_cache_item.cache = self
         http_cache_item.generation = self.generation
         self.__items[url] = http_cache_item
 
     def get(self, url: str) -> (ReleaseCacheItem, str, str):
-        item = self.__items.get(url, None)
+        item = self.__items.get(url, None) if self.__items else None
         if item is not None:
             change_vector = item.change_vector
             response = item.payload
             return ReleaseCacheItem(item), change_vector, response
 
         return ReleaseCacheItem(), None, None
```

### Comparing `ravendb-5.2.2/ravendb/http/misc.py` & `ravendb-5.2.3/ravendb/http/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/http/raven_command.py` & `ravendb-5.2.3/ravendb/http/raven_command.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/http/request_executor.py` & `ravendb-5.2.3/ravendb/http/request_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from ravendb.documents.conventions import DocumentConventions
     from typing import Union, Callable, Any, Optional
 
 
 class RequestExecutor:
     __INITIAL_TOPOLOGY_ETAG = -2
     __GLOBAL_APPLICATION_IDENTIFIER = uuid.uuid4()
-    CLIENT_VERSION = "5.2.2"
+    CLIENT_VERSION = "5.2.3"
     logger = logging.getLogger("request_executor")
 
     # todo: initializer should take also cryptography certificates
     def __init__(
         self,
         database_name: str,
         conventions: DocumentConventions,
@@ -124,14 +124,15 @@
         self._disposed = True
         self.__cache.close()
 
         if self.__update_topology_timer:
             self.__update_topology_timer.cancel()
 
         self._dispose_all_failed_nodes_timers()
+        self.__http_session.close()
 
     @property
     def certificate_path(self) -> str:
         return self.__certificate_path
 
     @property
     def trust_store_path(self) -> str:
```

### Comparing `ravendb-5.2.2/ravendb/http/server_node.py` & `ravendb-5.2.3/ravendb/http/server_node.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/http/topology.py` & `ravendb-5.2.3/ravendb/http/topology.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/infrastructure/entities.py` & `ravendb-5.2.3/ravendb/infrastructure/entities.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/infrastructure/faceted.py` & `ravendb-5.2.3/ravendb/infrastructure/faceted.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/infrastructure/graph.py` & `ravendb-5.2.3/ravendb/infrastructure/graph.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/infrastructure/operations.py` & `ravendb-5.2.3/ravendb/infrastructure/operations.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/infrastructure/orders.py` & `ravendb-5.2.3/ravendb/infrastructure/orders.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/json/json_operation.py` & `ravendb-5.2.3/ravendb/json/json_operation.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/json/metadata_as_dictionary.py` & `ravendb-5.2.3/ravendb/json/metadata_as_dictionary.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/primitives/misc.py` & `ravendb-5.2.3/ravendb/primitives/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/serverwide/commands.py` & `ravendb-5.2.3/ravendb/serverwide/commands.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/serverwide/database_record.py` & `ravendb-5.2.3/ravendb/serverwide/database_record.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/serverwide/misc.py` & `ravendb-5.2.3/ravendb/serverwide/misc.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/serverwide/operations/certificates.py` & `ravendb-5.2.3/ravendb/serverwide/operations/certificates.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/serverwide/operations/common.py` & `ravendb-5.2.3/ravendb/serverwide/operations/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,17 +218,17 @@
             if parameters
             else DeleteDatabaseOperation.Parameters(
                 [database_name], hard_delete, [from_node] if from_node else None, time_to_wait_for_confirmation
             )
         )
 
     def get_command(self, conventions: "DocumentConventions") -> RavenCommand[DeleteDatabaseResult]:
-        return self.__DeleteDatabaseCommand(conventions, self.__parameters)
+        return self._DeleteDatabaseCommand(conventions, self.__parameters)
 
-    class __DeleteDatabaseCommand(RavenCommand[DeleteDatabaseResult], RaftCommand):
+    class _DeleteDatabaseCommand(RavenCommand[DeleteDatabaseResult], RaftCommand):
         def __init__(self, conventions: DocumentConventions, parameters: DeleteDatabaseOperation.Parameters):
             super().__init__(DeleteDatabaseResult)
 
             if conventions is None:
                 raise ValueError("Conventions cannot be None")
 
             if parameters is None:
```

### Comparing `ravendb-5.2.2/ravendb/serverwide/server_operation_executor.py` & `ravendb-5.2.3/ravendb/serverwide/server_operation_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,16 @@
             raise ValueError("Request Executor cannot be None")
         self.__store = store
         self.__request_executor = request_executor
         self.__initial_request_executor = None
         self.__node_tag = None
         self.__cache = CaseInsensitiveDict()
 
-        # todo: register events
-
-        # todo: if node tag is null add after_close_listener
+        store.register_events_for_request_executor(self.__request_executor)
+        store.add_after_close(self.close)
 
     def send(self, operation: ServerOperation[_T_OperationResult]) -> Optional[None, _T_OperationResult]:
         command = operation.get_command(self.__request_executor.conventions)
         self.__request_executor.execute_command(command)
 
         if isinstance(operation, ServerOperation):
             return command.result
```

### Comparing `ravendb-5.2.2/ravendb/serverwide/tcp.py` & `ravendb-5.2.3/ravendb/serverwide/tcp.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/custom_decoder.py` & `ravendb-5.2.3/ravendb/tools/custom_decoder.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/generate_id.py` & `ravendb-5.2.3/ravendb/tools/generate_id.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/indexqueue.py` & `ravendb-5.2.3/ravendb/tools/indexqueue.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/parsers.py` & `ravendb-5.2.3/ravendb/tools/parsers.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/projection.py` & `ravendb-5.2.3/ravendb/tools/projection.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb/tools/utils.py` & `ravendb-5.2.3/ravendb/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,56 +153,69 @@
         self.human_size = human_size
 
     @classmethod
     def from_json(cls, json_dict: Dict) -> Size:
         return cls(json_dict["SizeInBytes"], json_dict["HumaneSize"])
 
 
+# todo: https://issues.hibernatingrhinos.com/issue/RDBC-686
 class CaseInsensitiveDict(dict, Generic[_TKey, _TVal]):
     @classmethod
-    def _k(cls, key):
+    def _lower_if_str(cls, key):
         return key.lower() if isinstance(key, str) else key
 
     def __init__(self, *args, **kwargs):
         super(CaseInsensitiveDict, self).__init__(*args, **kwargs)
+        self._original_values: Dict[_TKey, _TKey] = {}
         self._convert_keys()
 
-    def __getitem__(self, key) -> Tuple[_TKey, _TVal]:
-        return super(CaseInsensitiveDict, self).__getitem__(self.__class__._k(key))
+    def _convert_key_back(self, lowered_key: _TKey) -> _TKey:
+        return self._original_values[lowered_key]
+
+    def _convert_item_back(self, item: Tuple[_TKey, _TVal]) -> Tuple[_TKey, _TVal]:
+        return self._convert_key_back(item[0]), item[1]
+
+    def __getitem__(self, key) -> _TVal:
+        return super(CaseInsensitiveDict, self).__getitem__(self.__class__._lower_if_str(key))
 
     def __setitem__(self, key, value):
-        super(CaseInsensitiveDict, self).__setitem__(self.__class__._k(key), value)
+        adjusted_key = self.__class__._lower_if_str(key)
+        self._original_values[adjusted_key] = key
+        super(CaseInsensitiveDict, self).__setitem__(adjusted_key, value)
 
     def __delitem__(self, key):
-        return super(CaseInsensitiveDict, self).__delitem__(self.__class__._k(key))
+        return super(CaseInsensitiveDict, self).__delitem__(self.__class__._lower_if_str(key))
 
     def __contains__(self, key):
-        return super(CaseInsensitiveDict, self).__contains__(self.__class__._k(key))
+        return super(CaseInsensitiveDict, self).__contains__(self.__class__._lower_if_str(key))
 
-    def pop(self, key, *args, **kwargs) -> Tuple[_TKey, _TVal]:
-        return super(CaseInsensitiveDict, self).pop(self.__class__._k(key), *args, **kwargs)
+    def pop(self, key, *args, **kwargs) -> _TVal:
+        return super(CaseInsensitiveDict, self).pop(self.__class__._lower_if_str(key), *args, **kwargs)
 
     def remove(self, key, *args, **kwargs) -> Optional[_TVal]:
         return self.pop(key, *args, **kwargs) if key in self else None
 
     def get(self, key, *args, **kwargs) -> _TVal:
-        return super(CaseInsensitiveDict, self).get(self.__class__._k(key), *args, **kwargs)
+        return super(CaseInsensitiveDict, self).get(self.__class__._lower_if_str(key), *args, **kwargs)
 
     def setdefault(self, key, *args, **kwargs):
-        return super(CaseInsensitiveDict, self).setdefault(self.__class__._k(key), *args, **kwargs)
+        return super(CaseInsensitiveDict, self).setdefault(self.__class__._lower_if_str(key), *args, **kwargs)
 
     def update(self, e=None, **f):
         super(CaseInsensitiveDict, self).update(self.__class__(e))
         super(CaseInsensitiveDict, self).update(self.__class__(**f))
 
     def _convert_keys(self):
         for k in list(self):
             v = super(CaseInsensitiveDict, self).pop(k)
             self.__setitem__(k, v)
 
+    def keys(self) -> List[_TKey]:
+        return list(self._original_values.values())
+
 
 class CaseInsensitiveSet(set):
     @classmethod
     def _v(cls, value):
         return value.lower() if isinstance(value, str) else value
 
     def __init__(self, *args, **kwargs):
@@ -337,15 +350,15 @@
                 continue
             results.append(item)
 
         return results
 
     @staticmethod
     def quote_key(key, reserved_slash=False, reserved_at=False) -> str:
-        reserved = "%:=&?~#+!$,;'*[]"
+        reserved = ""
         if reserved_slash:
             reserved += "/"
         if reserved_at:
             reserved += "@"
         if key:
             return urllib.parse.quote(key, safe=reserved)
         else:
```

### Comparing `ravendb-5.2.2/ravendb/util/tcp_utils.py` & `ravendb-5.2.3/ravendb/util/tcp_utils.py`

 * *Files identical despite different names*

### Comparing `ravendb-5.2.2/ravendb.egg-info/PKG-INFO` & `ravendb-5.2.3/ravendb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravendb
-Version: 5.2.2
+Version: 5.2.3
 Summary: Python client for RavenDB NoSQL Database
 Home-page: https://github.com/ravendb/ravendb-python-client
 Author: RavenDB
 Author-email: support@ravendb.net
 License: MIT
 Keywords: ravendb,nosql,databasepyravendb
 Requires-Python: ~=3.7
@@ -18,23 +18,32 @@
 Install from [PyPi](https://pypi.python.org/pypi), as [ravendb](https://pypi.org/project/ravendb/).
 ```bash
 pip install ravendb
 ````
 ## Introduction
 Python client API (v5.2) for [RavenDB](https://ravendb.net/) , a NoSQL document database.
 
-
 Although new API isn't compatible with the previous one, it comes with **many improvements and new features**.
 
 **Package has been reworked to match Java and other RavenDB clients**
 
 **Type-hinted entire project and API results** - using the API is now much more comfortable with IntelliSense
 
+
+## Releases
+
+* All client versions 5.2.x are fully compatible with and support RavenDB server releases 5.4 and 6.0.
+
+* [Click here](https://github.com/ravendb/ravendb-python-client/releases) to view all Releases and Changelog.
+
 ## What's new?
 
+###### 5.2.3
+- **Counters**
+- Counters indexes
 
 ###### 5.2.2
 - New feature - **[Bulk insert](https://github.com/ravendb/ravendb-python-client/pull/161)**
 - Bugfixes - Cluster-wide operations ([here](https://github.com/ravendb/ravendb-python-client/pull/166))
 
 ###### 5.2.1
 - Bugfixes - Serialization while loading/querying ([here](https://github.com/ravendb/ravendb-python-client/pull/163))
```

### Comparing `ravendb-5.2.2/ravendb.egg-info/SOURCES.txt` & `ravendb-5.2.3/ravendb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,24 +32,26 @@
 ravendb/documents/commands/multi_get.py
 ravendb/documents/commands/query.py
 ravendb/documents/commands/results.py
 ravendb/documents/commands/subscriptions.py
 ravendb/documents/identity/__init__.py
 ravendb/documents/identity/hilo.py
 ravendb/documents/indexes/__init__.py
+ravendb/documents/indexes/counters.py
 ravendb/documents/indexes/definitions.py
 ravendb/documents/indexes/index_creation.py
 ravendb/documents/indexes/analysis/__init__.py
 ravendb/documents/indexes/analysis/definitions.py
 ravendb/documents/indexes/spatial/__init__.py
 ravendb/documents/indexes/spatial/configuration.py
 ravendb/documents/operations/__init__.py
 ravendb/documents/operations/batch.py
 ravendb/documents/operations/configuration.py
 ravendb/documents/operations/connection_strings.py
+ravendb/documents/operations/counters.py
 ravendb/documents/operations/definitions.py
 ravendb/documents/operations/executor.py
 ravendb/documents/operations/indexes.py
 ravendb/documents/operations/misc.py
 ravendb/documents/operations/ongoing_tasks.py
 ravendb/documents/operations/operation.py
 ravendb/documents/operations/patch.py
@@ -57,16 +59,14 @@
 ravendb/documents/operations/attachments/__init__.py
 ravendb/documents/operations/backups/__init__.py
 ravendb/documents/operations/backups/settings.py
 ravendb/documents/operations/compare_exchange/__init__.py
 ravendb/documents/operations/compare_exchange/compare_exchange.py
 ravendb/documents/operations/compare_exchange/compare_exchange_value_result_parser.py
 ravendb/documents/operations/compare_exchange/operations.py
-ravendb/documents/operations/counters/__init__.py
-ravendb/documents/operations/counters/operation.py
 ravendb/documents/operations/etl/__init__.py
 ravendb/documents/operations/etl/configuration.py
 ravendb/documents/operations/etl/olap/__init__.py
 ravendb/documents/operations/etl/sql/__init__.py
 ravendb/documents/operations/expiration/__init__.py
 ravendb/documents/operations/expiration/configuration.py
 ravendb/documents/operations/lazy/__init__.py
```

### Comparing `ravendb-5.2.2/setup.py` & `ravendb-5.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ravendb",
     packages=find_packages(exclude=["*.tests.*", "tests", "*.tests", "tests.*"]),
-    version="5.2.2",
+    version="5.2.3",
     long_description_content_type="text/markdown",
     long_description=open("README_pypi.md").read(),
     description="Python client for RavenDB NoSQL Database",
     author="RavenDB",
     author_email="support@ravendb.net",
     url="https://github.com/ravendb/ravendb-python-client",
     license="MIT",
```

