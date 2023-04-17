# Comparing `tmp/dbt-athena-community-1.4.2.tar.gz` & `tmp/dbt-athena-community-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.4.2.tar", last modified: Fri Mar 31 11:27:02 2023, max compression
+gzip compressed data, was "dbt-athena-community-1.4.3.tar", last modified: Mon Apr 17 14:02:16 2023, max compression
```

## Comparing `dbt-athena-community-1.4.2.tar` & `dbt-athena-community-1.4.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.526540 dbt-athena-community-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-03-31 11:27:02.526540 dbt-athena-community-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29272 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.518539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.522539 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.526540 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/ddl_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:27:02.526540 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-03-31 11:27:02.000000 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-31 11:27:02.000000 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:27:02.000000 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-31 11:27:02.000000 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-31 11:27:02.000000 dbt-athena-community-1.4.2/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:27:02.526540 dbt-athena-community-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-31 11:26:50.000000 dbt-athena-community-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30215 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/ddl_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/setup.py
```

### Comparing `dbt-athena-community-1.4.2/LICENSE.txt` & `dbt-athena-community-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/PKG-INFO` & `dbt-athena-community-1.4.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,1047 +1,1224 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6462 742d  : 2.1.Name: dbt-
 00000020: 6174 6865 6e61 2d63 6f6d 6d75 6e69 7479  athena-community
-00000030: 0a56 6572 7369 6f6e 3a20 312e 342e 320a  .Version: 1.4.2.
+00000030: 0a56 6572 7369 6f6e 3a20 312e 342e 330a  .Version: 1.4.3.
 00000040: 5375 6d6d 6172 793a 2054 6865 2061 7468  Summary: The ath
 00000050: 656e 6120 6164 6170 7465 7220 706c 7567  ena adapter plug
 00000060: 696e 2066 6f72 2064 6274 2028 6461 7461  in for dbt (data
 00000070: 2062 7569 6c64 2074 6f6f 6c29 0a48 6f6d   build tool).Hom
 00000080: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000090: 6769 7468 7562 2e63 6f6d 2f64 6274 2d61  github.com/dbt-a
 000000a0: 7468 656e 612f 6462 742d 6174 6865 6e61  thena/dbt-athena
 000000b0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 000000c0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 000000d0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
 000000e0: 2d46 696c 653a 204c 4943 454e 5345 2e74  -File: LICENSE.t
-000000f0: 7874 0a0a 5b21 5b70 7970 695d 2868 7474  xt..[![pypi](htt
-00000100: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000110: 696f 2f70 792f 6462 742d 6174 6865 6e61  io/py/dbt-athena
-00000120: 2d63 6f6d 6d75 6e69 7479 2e73 7667 295d  -community.svg)]
-00000130: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000140: 672f 7072 6f6a 6563 742f 6462 742d 6174  g/project/dbt-at
-00000150: 6865 6e61 2d63 6f6d 6d75 6e69 7479 2f29  hena-community/)
-00000160: 0a5b 215b 496d 706f 7274 733a 2069 736f  .[![Imports: iso
-00000170: 7274 5d28 6874 7470 733a 2f2f 696d 672e  rt](https://img.
-00000180: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000190: 2f25 3230 696d 706f 7274 732d 6973 6f72  /%20imports-isor
-000001a0: 742d 2532 3331 3637 3462 313f 7374 796c  t-%231674b1?styl
-000001b0: 653d 666c 6174 266c 6162 656c 436f 6c6f  e=flat&labelColo
-000001c0: 723d 6566 3833 3336 295d 2868 7474 7073  r=ef8336)](https
-000001d0: 3a2f 2f70 7963 7161 2e67 6974 6875 622e  ://pycqa.github.
-000001e0: 696f 2f69 736f 7274 2f29 0a5b 215b 436f  io/isort/).[![Co
-000001f0: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
-00000200: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000210: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00000220: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-00000230: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
-00000240: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000250: 2f70 7366 2f62 6c61 636b 290a 5b21 5b53  /psf/black).[![S
-00000260: 7461 7473 3a20 7065 7079 5d28 6874 7470  tats: pepy](http
-00000270: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
-00000280: 6467 652f 6462 742d 6174 6865 6e61 2d63  dge/dbt-athena-c
-00000290: 6f6d 6d75 6e69 7479 2f6d 6f6e 7468 295d  ommunity/month)]
-000002a0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-000002b0: 6368 2f70 726f 6a65 6374 2f64 6274 2d61  ch/project/dbt-a
-000002c0: 7468 656e 612d 636f 6d6d 756e 6974 7929  thena-community)
-000002d0: 0a0a 2320 6462 742d 6174 6865 6e61 0a0a  ..# dbt-athena..
-000002e0: 2a20 5375 7070 6f72 7473 2064 6274 2076  * Supports dbt v
-000002f0: 6572 7369 6f6e 2060 312e 342e 2a60 0a2a  ersion `1.4.*`.*
-00000300: 2053 7570 706f 7274 7320 5b53 6565 6473   Supports [Seeds
-00000310: 5d5b 7365 6564 735d 0a2a 2043 6f72 7265  ][seeds].* Corre
-00000320: 6374 6c79 2064 6574 6563 7473 2076 6965  ctly detects vie
-00000330: 7773 2061 6e64 2074 6865 6972 2063 6f6c  ws and their col
-00000340: 756d 6e73 0a2a 2053 7570 706f 7274 7320  umns.* Supports 
-00000350: 5b74 6162 6c65 206d 6174 6572 6961 6c69  [table materiali
-00000360: 7a61 7469 6f6e 5d5b 7461 626c 655d 0a20  zation][table]. 
-00000370: 202a 205b 4963 6562 6572 6720 7461 626c   * [Iceberg tabl
-00000380: 6573 5d5b 6174 6865 6e61 2d69 6365 6265  es][athena-icebe
-00000390: 7267 5d20 6973 2073 7570 706f 7274 6564  rg] is supported
-000003a0: 202a 2a6f 6e6c 7920 7769 7468 2041 7468   **only with Ath
-000003b0: 656e 6120 456e 6769 6e65 2076 332a 2a20  ena Engine v3** 
-000003c0: 616e 6420 2a2a 6120 756e 6971 7565 2074  and **a unique t
-000003d0: 6162 6c65 206c 6f63 6174 696f 6e2a 2a0a  able location**.
-000003e0: 2020 2873 6565 2074 6162 6c65 206c 6f63    (see table loc
-000003f0: 6174 696f 6e20 7365 6374 696f 6e20 6265  ation section be
-00000400: 6c6f 7729 0a20 202a 2048 6976 6520 7461  low).  * Hive ta
-00000410: 626c 6573 2069 7320 7375 7070 6f72 7465  bles is supporte
-00000420: 6420 6279 2062 6f74 6820 4174 6865 6e61  d by both Athena
-00000430: 2065 6e67 696e 6573 2e0a 2a20 5375 7070   engines..* Supp
-00000440: 6f72 7473 205b 696e 6372 656d 656e 7461  orts [incrementa
-00000450: 6c20 6d6f 6465 6c73 5d5b 696e 6372 656d  l models][increm
-00000460: 656e 7461 6c5d 0a20 202a 204f 6e20 6963  ental].  * On ic
-00000470: 6562 6572 6720 7461 626c 6573 203a 0a20  eberg tables :. 
-00000480: 2020 202a 2053 7570 706f 7274 2074 6865     * Support the
-00000490: 2075 7365 206f 6620 6075 6e69 7175 655f   use of `unique_
-000004a0: 6b65 7960 206f 6e6c 7920 7769 7468 2074  key` only with t
-000004b0: 6865 2060 6d65 7267 6560 2073 7472 6174  he `merge` strat
-000004c0: 6567 790a 2020 2020 2a20 5375 7070 6f72  egy.    * Suppor
-000004d0: 7420 7468 6520 6061 7070 656e 6460 2073  t the `append` s
-000004e0: 7472 6174 6567 790a 2020 2a20 4f6e 2048  trategy.  * On H
-000004f0: 6976 6520 7461 626c 6573 203a 0a20 2020  ive tables :.   
-00000500: 202a 2053 7570 706f 7274 2074 776f 2069   * Support two i
-00000510: 6e63 7265 6d65 6e74 616c 2075 7064 6174  ncremental updat
-00000520: 6520 7374 7261 7465 6769 6573 3a20 6069  e strategies: `i
-00000530: 6e73 6572 745f 6f76 6572 7772 6974 6560  nsert_overwrite`
-00000540: 2061 6e64 2060 6170 7065 6e64 600a 2020   and `append`.  
-00000550: 2020 2a20 446f 6573 202a 2a6e 6f74 2a2a    * Does **not**
-00000560: 2073 7570 706f 7274 2074 6865 2075 7365   support the use
-00000570: 206f 6620 6075 6e69 7175 655f 6b65 7960   of `unique_key`
-00000580: 0a2a 2053 7570 706f 7274 7320 5b73 6e61  .* Supports [sna
-00000590: 7073 686f 7473 5d5b 736e 6170 7368 6f74  pshots][snapshot
-000005a0: 735d 0a2a 2044 6f65 7320 6e6f 7420 7375  s].* Does not su
-000005b0: 7070 6f72 7420 5b50 7974 686f 6e20 6d6f  pport [Python mo
-000005c0: 6465 6c73 5d5b 7079 7468 6f6e 2d6d 6f64  dels][python-mod
-000005d0: 656c 735d 0a2a 2044 6f65 7320 6e6f 7420  els].* Does not 
-000005e0: 7375 7070 6f72 7420 5b70 6572 7369 7374  support [persist
-000005f0: 2064 6f63 735d 5b70 6572 7369 7374 2d64   docs][persist-d
-00000600: 6f63 735d 2066 6f72 2076 6965 7773 0a0a  ocs] for views..
-00000610: 5b73 6565 6473 5d3a 2068 7474 7073 3a2f  [seeds]: https:/
-00000620: 2f64 6f63 732e 6765 7464 6274 2e63 6f6d  /docs.getdbt.com
-00000630: 2f64 6f63 732f 6275 696c 6469 6e67 2d61  /docs/building-a
-00000640: 2d64 6274 2d70 726f 6a65 6374 2f73 6565  -dbt-project/see
-00000650: 6473 0a5b 696e 6372 656d 656e 7461 6c5d  ds.[incremental]
-00000660: 3a20 6874 7470 733a 2f2f 646f 6373 2e67  : https://docs.g
-00000670: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
-00000680: 7569 6c64 2f69 6e63 7265 6d65 6e74 616c  uild/incremental
-00000690: 2d6d 6f64 656c 730a 5b74 6162 6c65 5d3a  -models.[table]:
-000006a0: 2068 7474 7073 3a2f 2f64 6f63 732e 6765   https://docs.ge
-000006b0: 7464 6274 2e63 6f6d 2f64 6f63 732f 6275  tdbt.com/docs/bu
-000006c0: 696c 642f 6d61 7465 7269 616c 697a 6174  ild/materializat
-000006d0: 696f 6e73 2374 6162 6c65 0a5b 7079 7468  ions#table.[pyth
-000006e0: 6f6e 2d6d 6f64 656c 735d 3a20 6874 7470  on-models]: http
-000006f0: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
-00000700: 636f 6d2f 646f 6373 2f62 7569 6c64 2f70  com/docs/build/p
-00000710: 7974 686f 6e2d 6d6f 6465 6c73 2363 6f6e  ython-models#con
-00000720: 6669 6775 7269 6e67 2d70 7974 686f 6e2d  figuring-python-
-00000730: 6d6f 6465 6c73 0a5b 6174 6865 6e61 2d69  models.[athena-i
-00000740: 6365 6265 7267 5d3a 2068 7474 7073 3a2f  ceberg]: https:/
-00000750: 2f64 6f63 732e 6177 732e 616d 617a 6f6e  /docs.aws.amazon
-00000760: 2e63 6f6d 2f61 7468 656e 612f 6c61 7465  .com/athena/late
-00000770: 7374 2f75 672f 7175 6572 7969 6e67 2d69  st/ug/querying-i
-00000780: 6365 6265 7267 2e68 746d 6c0a 5b73 6e61  ceberg.html.[sna
-00000790: 7073 686f 7473 5d3a 2068 7474 7073 3a2f  pshots]: https:/
-000007a0: 2f64 6f63 732e 6765 7464 6274 2e63 6f6d  /docs.getdbt.com
-000007b0: 2f64 6f63 732f 6275 696c 642f 736e 6170  /docs/build/snap
-000007c0: 7368 6f74 730a 5b70 6572 7369 7374 2d64  shots.[persist-d
-000007d0: 6f63 735d 3a20 6874 7470 733a 2f2f 646f  ocs]: https://do
-000007e0: 6373 2e67 6574 6462 742e 636f 6d2f 7265  cs.getdbt.com/re
-000007f0: 6665 7265 6e63 652f 7265 736f 7572 6365  ference/resource
-00000800: 2d63 6f6e 6669 6773 2f70 6572 7369 7374  -configs/persist
-00000810: 5f64 6f63 730a 0a23 2323 2049 6e73 7461  _docs..### Insta
-00000820: 6c6c 6174 696f 6e0a 0a2a 2060 7069 7020  llation..* `pip 
-00000830: 696e 7374 616c 6c20 6462 742d 6174 6865  install dbt-athe
-00000840: 6e61 2d63 6f6d 6d75 6e69 7479 600a 2a20  na-community`.* 
-00000850: 4f72 2060 7069 7020 696e 7374 616c 6c20  Or `pip install 
-00000860: 6769 742b 6874 7470 733a 2f2f 6769 7468  git+https://gith
-00000870: 7562 2e63 6f6d 2f64 6274 2d61 7468 656e  ub.com/dbt-athen
-00000880: 612f 6462 742d 6174 6865 6e61 2e67 6974  a/dbt-athena.git
-00000890: 600a 0a23 2323 2050 7265 7265 7175 6973  `..### Prerequis
-000008a0: 6974 6573 0a0a 546f 2073 7461 7274 2c20  ites..To start, 
-000008b0: 796f 7520 7769 6c6c 206e 6565 6420 616e  you will need an
-000008c0: 2053 3320 6275 636b 6574 2c20 666f 7220   S3 bucket, for 
-000008d0: 696e 7374 616e 6365 2060 6d79 2d62 7563  instance `my-buc
-000008e0: 6b65 7460 2061 6e64 2061 6e20 4174 6865  ket` and an Athe
-000008f0: 6e61 2064 6174 6162 6173 653a 0a0a 6060  na database:..``
-00000900: 6073 716c 0a43 5245 4154 4520 4441 5441  `sql.CREATE DATA
-00000910: 4241 5345 2049 4620 4e4f 5420 4558 4953  BASE IF NOT EXIS
-00000920: 5453 2061 6e61 6c79 7469 6373 5f64 6576  TS analytics_dev
-00000930: 0a43 4f4d 4d45 4e54 2027 416e 616c 7974  .COMMENT 'Analyt
-00000940: 6963 7320 6d6f 6465 6c73 2067 656e 6572  ics models gener
-00000950: 6174 6564 2062 7920 6462 7420 2864 6576  ated by dbt (dev
-00000960: 656c 6f70 6d65 6e74 2927 0a4c 4f43 4154  elopment)'.LOCAT
-00000970: 494f 4e20 2773 333a 2f2f 6d79 2d62 7563  ION 's3://my-buc
-00000980: 6b65 742f 270a 5749 5448 2044 4250 524f  ket/'.WITH DBPRO
-00000990: 5045 5254 4945 5320 2827 6372 6561 746f  PERTIES ('creato
-000009a0: 7227 3d27 466f 6f20 4261 7227 2c20 2765  r'='Foo Bar', 'e
-000009b0: 6d61 696c 273d 2766 6f6f 4062 6172 2e63  mail'='foo@bar.c
-000009c0: 6f6d 2729 3b0a 6060 600a 0a4e 6f74 6573  om');.```..Notes
-000009d0: 3a0a 2d20 5461 6b65 206e 6f74 6520 6f66  :.- Take note of
-000009e0: 2079 6f75 7220 4157 5320 7265 6769 6f6e   your AWS region
-000009f0: 2063 6f64 6520 2865 2e67 2e20 6075 732d   code (e.g. `us-
-00000a00: 7765 7374 2d32 6020 6f72 2060 6575 2d77  west-2` or `eu-w
-00000a10: 6573 742d 3260 2c20 6574 632e 292e 0a2d  est-2`, etc.)..-
-00000a20: 2059 6f75 2063 616e 2061 6c73 6f20 7573   You can also us
-00000a30: 6520 5b41 5753 2047 6c75 655d 2868 7474  e [AWS Glue](htt
-00000a40: 7073 3a2f 2f64 6f63 732e 6177 732e 616d  ps://docs.aws.am
-00000a50: 617a 6f6e 2e63 6f6d 2f61 7468 656e 612f  azon.com/athena/
-00000a60: 6c61 7465 7374 2f75 672f 676c 7565 2d61  latest/ug/glue-a
-00000a70: 7468 656e 612e 6874 6d6c 2920 746f 2063  thena.html) to c
-00000a80: 7265 6174 6520 616e 6420 6d61 6e61 6765  reate and manage
-00000a90: 2041 7468 656e 6120 6461 7461 6261 7365   Athena database
-00000aa0: 732e 0a0a 2323 2320 4372 6564 656e 7469  s...### Credenti
-00000ab0: 616c 730a 0a54 6869 7320 706c 7567 696e  als..This plugin
-00000ac0: 2064 6f65 7320 6e6f 7420 6163 6365 7074   does not accept
-00000ad0: 2061 6e79 2063 7265 6465 6e74 6961 6c73   any credentials
-00000ae0: 2064 6972 6563 746c 792e 2049 6e73 7465   directly. Inste
-00000af0: 6164 2c20 5b63 7265 6465 6e74 6961 6c73  ad, [credentials
-00000b00: 2061 7265 2064 6574 6572 6d69 6e65 6420   are determined 
-00000b10: 6175 746f 6d61 7469 6361 6c6c 795d 2868  automatically](h
-00000b20: 7474 7073 3a2f 2f62 6f74 6f33 2e61 6d61  ttps://boto3.ama
-00000b30: 7a6f 6e61 7773 2e63 6f6d 2f76 312f 646f  zonaws.com/v1/do
-00000b40: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
-00000b50: 6c61 7465 7374 2f67 7569 6465 2f63 7265  latest/guide/cre
-00000b60: 6465 6e74 6961 6c73 2e68 746d 6c29 2062  dentials.html) b
-00000b70: 6173 6564 206f 6e20 6061 7773 2063 6c69  ased on `aws cli
-00000b80: 602f 6062 6f74 6f33 6020 636f 6e76 656e  `/`boto3` conven
-00000b90: 7469 6f6e 7320 616e 640a 7374 6f72 6564  tions and.stored
-00000ba0: 206c 6f67 696e 2069 6e66 6f2e 2059 6f75   login info. You
-00000bb0: 2063 616e 2063 6f6e 6669 6775 7265 2074   can configure t
-00000bc0: 6865 2041 5753 2070 726f 6669 6c65 206e  he AWS profile n
-00000bd0: 616d 6520 746f 2075 7365 2076 6961 2060  ame to use via `
-00000be0: 6177 735f 7072 6f66 696c 655f 6e61 6d65  aws_profile_name
-00000bf0: 602e 2043 6865 636b 6f75 7420 4442 5420  `. Checkout DBT 
-00000c00: 7072 6f66 696c 6520 636f 6e66 6967 7572  profile configur
-00000c10: 6174 696f 6e20 6265 6c6f 7720 666f 7220  ation below for 
-00000c20: 6465 7461 696c 732e 0a0a 2323 2320 436f  details...### Co
-00000c30: 6e66 6967 7572 696e 6720 796f 7572 2070  nfiguring your p
-00000c40: 726f 6669 6c65 0a0a 4120 6462 7420 7072  rofile..A dbt pr
-00000c50: 6f66 696c 6520 6361 6e20 6265 2063 6f6e  ofile can be con
-00000c60: 6669 6775 7265 6420 746f 2072 756e 2061  figured to run a
-00000c70: 6761 696e 7374 2041 5753 2041 7468 656e  gainst AWS Athen
-00000c80: 6120 7573 696e 6720 7468 6520 666f 6c6c  a using the foll
-00000c90: 6f77 696e 6720 636f 6e66 6967 7572 6174  owing configurat
-00000ca0: 696f 6e3a 0a0a 7c20 4f70 7469 6f6e 2020  ion:..| Option  
-00000cb0: 2020 2020 2020 2020 207c 2044 6573 6372           | Descr
-00000cc0: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2020 2020 2020 7c20 5265 7175            | Requ
-00000d10: 6972 6564 3f20 7c20 4578 616d 706c 6520  ired? | Example 
-00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
-00000d50: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000da0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000db0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-00000de0: 7c20 7333 5f73 7461 6769 6e67 5f64 6972  | s3_staging_dir
-00000df0: 2020 207c 2053 3320 6c6f 6361 7469 6f6e     | S3 location
-00000e00: 2074 6f20 7374 6f72 6520 4174 6865 6e61   to store Athena
-00000e10: 2071 7565 7279 2072 6573 756c 7473 2061   query results a
-00000e20: 6e64 206d 6574 6164 6174 6120 2020 2020  nd metadata     
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 2020 2020 7c20 5265 7175 6972 6564 2020      | Required  
-00000e50: 7c20 6073 333a 2f2f 6275 636b 6574 2f64  | `s3://bucket/d
-00000e60: 6274 2f60 2020 2020 2020 2020 2020 2020  bt/`            
-00000e70: 2020 2020 2020 2020 2020 207c 0a7c 2073             |.| s
-00000e80: 335f 6461 7461 5f64 6972 2020 2020 2020  3_data_dir      
-00000e90: 7c20 5072 6566 6978 2066 6f72 2073 746f  | Prefix for sto
-00000ea0: 7269 6e67 2074 6162 6c65 732c 2069 6620  ring tables, if 
-00000eb0: 6469 6666 6572 656e 7420 6672 6f6d 2074  different from t
-00000ec0: 6865 2063 6f6e 6e65 6374 696f 6e27 7320  he connection's 
-00000ed0: 6073 335f 7374 6167 696e 675f 6469 7260  `s3_staging_dir`
-00000ee0: 207c 204f 7074 696f 6e61 6c20 207c 2060   | Optional  | `
-00000ef0: 7333 3a2f 2f62 7563 6b65 7432 2f64 6274  s3://bucket2/dbt
-00000f00: 2f60 2020 2020 2020 2020 2020 2020 2020  /`              
-00000f10: 2020 2020 2020 2020 7c0a 7c20 7333 5f64          |.| s3_d
-00000f20: 6174 615f 6e61 6d69 6e67 2020 207c 2048  ata_naming   | H
-00000f30: 6f77 2074 6f20 6765 6e65 7261 7465 2074  ow to generate t
-00000f40: 6162 6c65 2070 6174 6873 2069 6e20 6073  able paths in `s
-00000f50: 335f 6461 7461 5f64 6972 6020 2020 2020  3_data_dir`     
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000f80: 4f70 7469 6f6e 616c 2020 7c20 6073 6368  Optional  | `sch
-00000f90: 656d 615f 7461 626c 655f 756e 6971 7565  ema_table_unique
-00000fa0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00000fb0: 2020 2020 207c 0a7c 2072 6567 696f 6e5f       |.| region_
-00000fc0: 6e61 6d65 2020 2020 2020 7c20 4157 5320  name      | AWS 
-00000fd0: 7265 6769 6f6e 206f 6620 796f 7572 2041  region of your A
-00000fe0: 7468 656e 6120 696e 7374 616e 6365 2020  thena instance  
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 2020 2020 207c 2052 6571             | Req
-00001020: 7569 7265 6420 207c 2060 6575 2d77 6573  uired  | `eu-wes
-00001030: 742d 3160 2020 2020 2020 2020 2020 2020  t-1`            
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 7c0a 7c20 7363 6865 6d61 2020 2020    |.| schema    
-00001060: 2020 2020 2020 207c 2053 7065 6369 6679         | Specify
-00001070: 2074 6865 2073 6368 656d 6120 2841 7468   the schema (Ath
-00001080: 656e 6120 6461 7461 6261 7365 2920 746f  ena database) to
-00001090: 2062 7569 6c64 206d 6f64 656c 7320 696e   build models in
-000010a0: 746f 2028 6c6f 7765 7263 6173 6520 2a2a  to (lowercase **
-000010b0: 6f6e 6c79 2a2a 2920 7c20 5265 7175 6972  only**) | Requir
-000010c0: 6564 2020 7c20 6064 6274 6020 2020 2020  ed  | `dbt`     
+000000f0: 7874 0a0a 3c70 2061 6c69 676e 3d22 6365  xt..<p align="ce
+00000100: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
+00000110: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000120: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000130: 6e74 2e63 6f6d 2f64 6274 2d61 7468 656e  nt.com/dbt-athen
+00000140: 612f 6462 742d 6174 6865 6e61 2f6d 6169  a/dbt-athena/mai
+00000150: 6e2f 7374 6174 6963 2f69 6d61 6765 732f  n/static/images/
+00000160: 6462 742d 6174 6865 6e61 2d6c 6f6e 672e  dbt-athena-long.
+00000170: 706e 6722 202f 3e0a 2020 2020 3c61 2068  png" />.    <a h
+00000180: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000190: 692e 6f72 672f 7072 6f6a 6563 742f 6462  i.org/project/db
+000001a0: 742d 6174 6865 6e61 2d63 6f6d 6d75 6e69  t-athena-communi
+000001b0: 7479 2f22 3e3c 696d 6720 7372 633d 2268  ty/"><img src="h
+000001c0: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+000001d0: 792e 696f 2f70 792f 6462 742d 6174 6865  y.io/py/dbt-athe
+000001e0: 6e61 2d63 6f6d 6d75 6e69 7479 2e73 7667  na-community.svg
+000001f0: 2220 2f3e 3c2f 613e 0a20 2020 203c 6120  " /></a>.    <a 
+00000200: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000210: 6371 612e 6769 7468 7562 2e69 6f2f 6973  cqa.github.io/is
+00000220: 6f72 742f 223e 3c69 6d67 2073 7263 3d22  ort/"><img src="
+00000230: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000240: 6c64 732e 696f 2f62 6164 6765 2f25 3230  lds.io/badge/%20
+00000250: 696d 706f 7274 732d 6973 6f72 742d 2532  imports-isort-%2
+00000260: 3331 3637 3462 313f 7374 796c 653d 666c  31674b1?style=fl
+00000270: 6174 266c 6162 656c 436f 6c6f 723d 6566  at&labelColor=ef
+00000280: 3833 3336 2220 2f3e 3c2f 613e 0a20 2020  8336" /></a>.   
+00000290: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000002a0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+000002b0: 2f62 6c61 636b 223e 3c69 6d67 2073 7263  /black"><img src
+000002c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002d0: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
+000002e0: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
+000002f0: 6b2d 3030 3030 3030 2e73 7667 2220 2f3e  k-000000.svg" />
+00000300: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000310: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00000320: 6563 682f 7072 6f6a 6563 742f 6462 742d  ech/project/dbt-
+00000330: 6174 6865 6e61 2d63 6f6d 6d75 6e69 7479  athena-community
+00000340: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000350: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+00000360: 6467 652f 6462 742d 6174 6865 6e61 2d63  dge/dbt-athena-c
+00000370: 6f6d 6d75 6e69 7479 2f6d 6f6e 7468 2220  ommunity/month" 
+00000380: 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a23 2320  /></a>.</p>..## 
+00000390: 4665 6174 7572 6573 0a0a 2a20 5375 7070  Features..* Supp
+000003a0: 6f72 7473 2064 6274 2076 6572 7369 6f6e  orts dbt version
+000003b0: 2060 312e 342e 2a60 0a2a 2053 7570 706f   `1.4.*`.* Suppo
+000003c0: 7274 7320 5b53 6565 6473 5d5b 7365 6564  rts [Seeds][seed
+000003d0: 735d 0a2a 2043 6f72 7265 6374 6c79 2064  s].* Correctly d
+000003e0: 6574 6563 7473 2076 6965 7773 2061 6e64  etects views and
+000003f0: 2074 6865 6972 2063 6f6c 756d 6e73 0a2a   their columns.*
+00000400: 2053 7570 706f 7274 7320 5b74 6162 6c65   Supports [table
+00000410: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
+00000420: 5d5b 7461 626c 655d 0a20 202a 205b 4963  ][table].  * [Ic
+00000430: 6562 6572 6720 7461 626c 6573 5d5b 6174  eberg tables][at
+00000440: 6865 6e61 2d69 6365 6265 7267 5d20 6973  hena-iceberg] is
+00000450: 2073 7570 706f 7274 6564 202a 2a6f 6e6c   supported **onl
+00000460: 7920 7769 7468 2041 7468 656e 6120 456e  y with Athena En
+00000470: 6769 6e65 2076 332a 2a20 616e 6420 2a2a  gine v3** and **
+00000480: 6120 756e 6971 7565 2074 6162 6c65 206c  a unique table l
+00000490: 6f63 6174 696f 6e2a 2a0a 2020 2873 6565  ocation**.  (see
+000004a0: 2074 6162 6c65 206c 6f63 6174 696f 6e20   table location 
+000004b0: 7365 6374 696f 6e20 6265 6c6f 7729 0a20  section below). 
+000004c0: 202a 2048 6976 6520 7461 626c 6573 2069   * Hive tables i
+000004d0: 7320 7375 7070 6f72 7465 6420 6279 2062  s supported by b
+000004e0: 6f74 6820 4174 6865 6e61 2065 6e67 696e  oth Athena engin
+000004f0: 6573 2e0a 2a20 5375 7070 6f72 7473 205b  es..* Supports [
+00000500: 696e 6372 656d 656e 7461 6c20 6d6f 6465  incremental mode
+00000510: 6c73 5d5b 696e 6372 656d 656e 7461 6c5d  ls][incremental]
+00000520: 0a20 202a 204f 6e20 6963 6562 6572 6720  .  * On iceberg 
+00000530: 7461 626c 6573 203a 0a20 2020 202a 2053  tables :.    * S
+00000540: 7570 706f 7274 2074 6865 2075 7365 206f  upport the use o
+00000550: 6620 6075 6e69 7175 655f 6b65 7960 206f  f `unique_key` o
+00000560: 6e6c 7920 7769 7468 2074 6865 2060 6d65  nly with the `me
+00000570: 7267 6560 2073 7472 6174 6567 790a 2020  rge` strategy.  
+00000580: 2020 2a20 5375 7070 6f72 7420 7468 6520    * Support the 
+00000590: 6061 7070 656e 6460 2073 7472 6174 6567  `append` strateg
+000005a0: 790a 2020 2a20 4f6e 2048 6976 6520 7461  y.  * On Hive ta
+000005b0: 626c 6573 203a 0a20 2020 202a 2053 7570  bles :.    * Sup
+000005c0: 706f 7274 2074 776f 2069 6e63 7265 6d65  port two increme
+000005d0: 6e74 616c 2075 7064 6174 6520 7374 7261  ntal update stra
+000005e0: 7465 6769 6573 3a20 6069 6e73 6572 745f  tegies: `insert_
+000005f0: 6f76 6572 7772 6974 6560 2061 6e64 2060  overwrite` and `
+00000600: 6170 7065 6e64 600a 2020 2020 2a20 446f  append`.    * Do
+00000610: 6573 202a 2a6e 6f74 2a2a 2073 7570 706f  es **not** suppo
+00000620: 7274 2074 6865 2075 7365 206f 6620 6075  rt the use of `u
+00000630: 6e69 7175 655f 6b65 7960 0a2a 2053 7570  nique_key`.* Sup
+00000640: 706f 7274 7320 5b73 6e61 7073 686f 7473  ports [snapshots
+00000650: 5d5b 736e 6170 7368 6f74 735d 0a2a 2044  ][snapshots].* D
+00000660: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+00000670: 5b50 7974 686f 6e20 6d6f 6465 6c73 5d5b  [Python models][
+00000680: 7079 7468 6f6e 2d6d 6f64 656c 735d 0a2a  python-models].*
+00000690: 2044 6f65 7320 6e6f 7420 7375 7070 6f72   Does not suppor
+000006a0: 7420 5b70 6572 7369 7374 2064 6f63 735d  t [persist docs]
+000006b0: 5b70 6572 7369 7374 2d64 6f63 735d 2066  [persist-docs] f
+000006c0: 6f72 2076 6965 7773 0a0a 5b73 6565 6473  or views..[seeds
+000006d0: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+000006e0: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+000006f0: 6275 696c 6469 6e67 2d61 2d64 6274 2d70  building-a-dbt-p
+00000700: 726f 6a65 6374 2f73 6565 6473 0a5b 696e  roject/seeds.[in
+00000710: 6372 656d 656e 7461 6c5d 3a20 6874 7470  cremental]: http
+00000720: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
+00000730: 636f 6d2f 646f 6373 2f62 7569 6c64 2f69  com/docs/build/i
+00000740: 6e63 7265 6d65 6e74 616c 2d6d 6f64 656c  ncremental-model
+00000750: 730a 5b74 6162 6c65 5d3a 2068 7474 7073  s.[table]: https
+00000760: 3a2f 2f64 6f63 732e 6765 7464 6274 2e63  ://docs.getdbt.c
+00000770: 6f6d 2f64 6f63 732f 6275 696c 642f 6d61  om/docs/build/ma
+00000780: 7465 7269 616c 697a 6174 696f 6e73 2374  terializations#t
+00000790: 6162 6c65 0a5b 7079 7468 6f6e 2d6d 6f64  able.[python-mod
+000007a0: 656c 735d 3a20 6874 7470 733a 2f2f 646f  els]: https://do
+000007b0: 6373 2e67 6574 6462 742e 636f 6d2f 646f  cs.getdbt.com/do
+000007c0: 6373 2f62 7569 6c64 2f70 7974 686f 6e2d  cs/build/python-
+000007d0: 6d6f 6465 6c73 2363 6f6e 6669 6775 7269  models#configuri
+000007e0: 6e67 2d70 7974 686f 6e2d 6d6f 6465 6c73  ng-python-models
+000007f0: 0a5b 6174 6865 6e61 2d69 6365 6265 7267  .[athena-iceberg
+00000800: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+00000810: 6177 732e 616d 617a 6f6e 2e63 6f6d 2f61  aws.amazon.com/a
+00000820: 7468 656e 612f 6c61 7465 7374 2f75 672f  thena/latest/ug/
+00000830: 7175 6572 7969 6e67 2d69 6365 6265 7267  querying-iceberg
+00000840: 2e68 746d 6c0a 5b73 6e61 7073 686f 7473  .html.[snapshots
+00000850: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+00000860: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+00000870: 6275 696c 642f 736e 6170 7368 6f74 730a  build/snapshots.
+00000880: 5b70 6572 7369 7374 2d64 6f63 735d 3a20  [persist-docs]: 
+00000890: 6874 7470 733a 2f2f 646f 6373 2e67 6574  https://docs.get
+000008a0: 6462 742e 636f 6d2f 7265 6665 7265 6e63  dbt.com/referenc
+000008b0: 652f 7265 736f 7572 6365 2d63 6f6e 6669  e/resource-confi
+000008c0: 6773 2f70 6572 7369 7374 5f64 6f63 730a  gs/persist_docs.
+000008d0: 0a0a 2323 2051 7569 636b 2053 7461 7274  ..## Quick Start
+000008e0: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+000008f0: 6f6e 0a0a 2a20 6070 6970 2069 6e73 7461  on..* `pip insta
+00000900: 6c6c 2064 6274 2d61 7468 656e 612d 636f  ll dbt-athena-co
+00000910: 6d6d 756e 6974 7960 0a2a 204f 7220 6070  mmunity`.* Or `p
+00000920: 6970 2069 6e73 7461 6c6c 2067 6974 2b68  ip install git+h
+00000930: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000940: 6d2f 6462 742d 6174 6865 6e61 2f64 6274  m/dbt-athena/dbt
+00000950: 2d61 7468 656e 612e 6769 7460 0a0a 2323  -athena.git`..##
+00000960: 2320 5072 6572 6571 7569 7369 7465 730a  # Prerequisites.
+00000970: 0a54 6f20 7374 6172 742c 2079 6f75 2077  .To start, you w
+00000980: 696c 6c20 6e65 6564 2061 6e20 5333 2062  ill need an S3 b
+00000990: 7563 6b65 742c 2066 6f72 2069 6e73 7461  ucket, for insta
+000009a0: 6e63 6520 606d 792d 6275 636b 6574 6020  nce `my-bucket` 
+000009b0: 616e 6420 616e 2041 7468 656e 6120 6461  and an Athena da
+000009c0: 7461 6261 7365 3a0a 0a60 6060 7371 6c0a  tabase:..```sql.
+000009d0: 4352 4541 5445 2044 4154 4142 4153 4520  CREATE DATABASE 
+000009e0: 4946 204e 4f54 2045 5849 5354 5320 616e  IF NOT EXISTS an
+000009f0: 616c 7974 6963 735f 6465 760a 434f 4d4d  alytics_dev.COMM
+00000a00: 454e 5420 2741 6e61 6c79 7469 6373 206d  ENT 'Analytics m
+00000a10: 6f64 656c 7320 6765 6e65 7261 7465 6420  odels generated 
+00000a20: 6279 2064 6274 2028 6465 7665 6c6f 706d  by dbt (developm
+00000a30: 656e 7429 270a 4c4f 4341 5449 4f4e 2027  ent)'.LOCATION '
+00000a40: 7333 3a2f 2f6d 792d 6275 636b 6574 2f27  s3://my-bucket/'
+00000a50: 0a57 4954 4820 4442 5052 4f50 4552 5449  .WITH DBPROPERTI
+00000a60: 4553 2028 2763 7265 6174 6f72 273d 2746  ES ('creator'='F
+00000a70: 6f6f 2042 6172 272c 2027 656d 6169 6c27  oo Bar', 'email'
+00000a80: 3d27 666f 6f40 6261 722e 636f 6d27 293b  ='foo@bar.com');
+00000a90: 0a60 6060 0a0a 4e6f 7465 733a 0a2d 2054  .```..Notes:.- T
+00000aa0: 616b 6520 6e6f 7465 206f 6620 796f 7572  ake note of your
+00000ab0: 2041 5753 2072 6567 696f 6e20 636f 6465   AWS region code
+00000ac0: 2028 652e 672e 2060 7573 2d77 6573 742d   (e.g. `us-west-
+00000ad0: 3260 206f 7220 6065 752d 7765 7374 2d32  2` or `eu-west-2
+00000ae0: 602c 2065 7463 2e29 2e0a 2d20 596f 7520  `, etc.)..- You 
+00000af0: 6361 6e20 616c 736f 2075 7365 205b 4157  can also use [AW
+00000b00: 5320 476c 7565 5d28 6874 7470 733a 2f2f  S Glue](https://
+00000b10: 646f 6373 2e61 7773 2e61 6d61 7a6f 6e2e  docs.aws.amazon.
+00000b20: 636f 6d2f 6174 6865 6e61 2f6c 6174 6573  com/athena/lates
+00000b30: 742f 7567 2f67 6c75 652d 6174 6865 6e61  t/ug/glue-athena
+00000b40: 2e68 746d 6c29 2074 6f20 6372 6561 7465  .html) to create
+00000b50: 2061 6e64 206d 616e 6167 6520 4174 6865   and manage Athe
+00000b60: 6e61 2064 6174 6162 6173 6573 2e0a 0a23  na databases...#
+00000b70: 2323 2043 7265 6465 6e74 6961 6c73 0a0a  ## Credentials..
+00000b80: 5468 6973 2070 6c75 6769 6e20 646f 6573  This plugin does
+00000b90: 206e 6f74 2061 6363 6570 7420 616e 7920   not accept any 
+00000ba0: 6372 6564 656e 7469 616c 7320 6469 7265  credentials dire
+00000bb0: 6374 6c79 2e20 496e 7374 6561 642c 205b  ctly. Instead, [
+00000bc0: 6372 6564 656e 7469 616c 7320 6172 6520  credentials are 
+00000bd0: 6465 7465 726d 696e 6564 2061 7574 6f6d  determined autom
+00000be0: 6174 6963 616c 6c79 5d28 6874 7470 733a  atically](https:
+00000bf0: 2f2f 626f 746f 332e 616d 617a 6f6e 6177  //boto3.amazonaw
+00000c00: 732e 636f 6d2f 7631 2f64 6f63 756d 656e  s.com/v1/documen
+00000c10: 7461 7469 6f6e 2f61 7069 2f6c 6174 6573  tation/api/lates
+00000c20: 742f 6775 6964 652f 6372 6564 656e 7469  t/guide/credenti
+00000c30: 616c 732e 6874 6d6c 2920 6261 7365 6420  als.html) based 
+00000c40: 6f6e 2060 6177 7320 636c 6960 2f60 626f  on `aws cli`/`bo
+00000c50: 746f 3360 2063 6f6e 7665 6e74 696f 6e73  to3` conventions
+00000c60: 2061 6e64 0a73 746f 7265 6420 6c6f 6769   and.stored logi
+00000c70: 6e20 696e 666f 2e20 596f 7520 6361 6e20  n info. You can 
+00000c80: 636f 6e66 6967 7572 6520 7468 6520 4157  configure the AW
+00000c90: 5320 7072 6f66 696c 6520 6e61 6d65 2074  S profile name t
+00000ca0: 6f20 7573 6520 7669 6120 6061 7773 5f70  o use via `aws_p
+00000cb0: 726f 6669 6c65 5f6e 616d 6560 2e20 4368  rofile_name`. Ch
+00000cc0: 6563 6b6f 7574 2044 4254 2070 726f 6669  eckout DBT profi
+00000cd0: 6c65 2063 6f6e 6669 6775 7261 7469 6f6e  le configuration
+00000ce0: 2062 656c 6f77 2066 6f72 2064 6574 6169   below for detai
+00000cf0: 6c73 2e0a 0a23 2323 2043 6f6e 6669 6775  ls...### Configu
+00000d00: 7269 6e67 2079 6f75 7220 7072 6f66 696c  ring your profil
+00000d10: 650a 0a41 2064 6274 2070 726f 6669 6c65  e..A dbt profile
+00000d20: 2063 616e 2062 6520 636f 6e66 6967 7572   can be configur
+00000d30: 6564 2074 6f20 7275 6e20 6167 6169 6e73  ed to run agains
+00000d40: 7420 4157 5320 4174 6865 6e61 2075 7369  t AWS Athena usi
+00000d50: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
+00000d60: 2063 6f6e 6669 6775 7261 7469 6f6e 3a0a   configuration:.
+00000d70: 0a7c 204f 7074 696f 6e20 2020 2020 2020  .| Option       
+00000d80: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
+00000d90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dd0: 2020 2020 207c 2052 6571 7569 7265 643f       | Required?
+00000de0: 207c 2045 7861 6d70 6c65 2020 2020 2020   | Example      
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
+00000e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e20: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e70: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --|-----------|-
+00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ea0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2073 335f  ---------|.| s3_
+00000eb0: 7374 6167 696e 675f 6469 7220 2020 7c20  staging_dir   | 
+00000ec0: 5333 206c 6f63 6174 696f 6e20 746f 2073  S3 location to s
+00000ed0: 746f 7265 2041 7468 656e 6120 7175 6572  tore Athena quer
+00000ee0: 7920 7265 7375 6c74 7320 616e 6420 6d65  y results and me
+00000ef0: 7461 6461 7461 2020 2020 2020 2020 2020  tadata          
+00000f00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000f10: 2052 6571 7569 7265 6420 207c 2060 7333   Required  | `s3
+00000f20: 3a2f 2f62 7563 6b65 742f 6462 742f 6020  ://bucket/dbt/` 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 7c0a 7c20 7333 5f64 6174        |.| s3_dat
+00000f50: 615f 6469 7220 2020 2020 207c 2050 7265  a_dir      | Pre
+00000f60: 6669 7820 666f 7220 7374 6f72 696e 6720  fix for storing 
+00000f70: 7461 626c 6573 2c20 6966 2064 6966 6665  tables, if diffe
+00000f80: 7265 6e74 2066 726f 6d20 7468 6520 636f  rent from the co
+00000f90: 6e6e 6563 7469 6f6e 2773 2060 7333 5f73  nnection's `s3_s
+00000fa0: 7461 6769 6e67 5f64 6972 6020 7c20 4f70  taging_dir` | Op
+00000fb0: 7469 6f6e 616c 2020 7c20 6073 333a 2f2f  tional  | `s3://
+00000fc0: 6275 636b 6574 322f 6462 742f 6020 2020  bucket2/dbt/`   
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 207c 0a7c 2073 335f 6461 7461 5f6e     |.| s3_data_n
+00000ff0: 616d 696e 6720 2020 7c20 486f 7720 746f  aming   | How to
+00001000: 2067 656e 6572 6174 6520 7461 626c 6520   generate table 
+00001010: 7061 7468 7320 696e 2060 7333 5f64 6174  paths in `s3_dat
+00001020: 615f 6469 7260 2020 2020 2020 2020 2020  a_dir`          
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 207c 204f 7074 696f           | Optio
+00001050: 6e61 6c20 207c 2060 7363 6865 6d61 5f74  nal  | `schema_t
+00001060: 6162 6c65 5f75 6e69 7175 6560 2020 2020  able_unique`    
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 7c0a 7c20 7265 6769 6f6e 5f6e 616d 6520  |.| region_name 
+00001090: 2020 2020 207c 2041 5753 2072 6567 696f       | AWS regio
+000010a0: 6e20 6f66 2079 6f75 7220 4174 6865 6e61  n of your Athena
+000010b0: 2069 6e73 7461 6e63 6520 2020 2020 2020   instance       
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000010f0: 0a7c 2064 6174 6162 6173 6520 2020 2020  .| database     
-00001100: 2020 2020 7c20 5370 6563 6966 7920 7468      | Specify th
-00001110: 6520 6461 7461 6261 7365 2028 4461 7461  e database (Data
-00001120: 2063 6174 616c 6f67 2920 746f 2062 7569   catalog) to bui
-00001130: 6c64 206d 6f64 656c 7320 696e 746f 2028  ld models into (
-00001140: 6c6f 7765 7263 6173 6520 2a2a 6f6e 6c79  lowercase **only
-00001150: 2a2a 2920 207c 2052 6571 7569 7265 6420  **)  | Required 
-00001160: 207c 2060 6177 7364 6174 6163 6174 616c   | `awsdatacatal
-00001170: 6f67 6020 2020 2020 2020 2020 2020 2020  og`             
-00001180: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00001190: 706f 6c6c 5f69 6e74 6572 7661 6c20 2020  poll_interval   
-000011a0: 207c 2049 6e74 6572 7661 6c20 696e 2073   | Interval in s
-000011b0: 6563 6f6e 6473 2074 6f20 7573 6520 666f  econds to use fo
-000011c0: 7220 706f 6c6c 696e 6720 7468 6520 7374  r polling the st
-000011d0: 6174 7573 206f 6620 7175 6572 7920 7265  atus of query re
-000011e0: 7375 6c74 7320 696e 2041 7468 656e 6120  sults in Athena 
-000011f0: 2020 7c20 4f70 7469 6f6e 616c 2020 7c20    | Optional  | 
-00001200: 6035 6020 2020 2020 2020 2020 2020 2020  `5`             
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 207c 0a7c 2061 7773           |.| aws
-00001230: 5f70 726f 6669 6c65 5f6e 616d 6520 7c20  _profile_name | 
-00001240: 5072 6f66 696c 6520 746f 2075 7365 2066  Profile to use f
-00001250: 726f 6d20 796f 7572 2041 5753 2073 6861  rom your AWS sha
-00001260: 7265 6420 6372 6564 656e 7469 616c 7320  red credentials 
-00001270: 6669 6c65 2e20 2020 2020 2020 2020 2020  file.           
-00001280: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001290: 204f 7074 696f 6e61 6c20 207c 2060 6d79   Optional  | `my
-000012a0: 2d70 726f 6669 6c65 6020 2020 2020 2020  -profile`       
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 7c0a 7c20 776f 726b 5f67        |.| work_g
-000012d0: 726f 7570 2020 2020 2020 207c 2049 6465  roup       | Ide
-000012e0: 6e74 6966 6965 7220 6f66 2041 7468 656e  ntifier of Athen
-000012f0: 6120 776f 726b 6772 6f75 7020 2020 2020  a workgroup     
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 2020 2020 2020 2020 7c20 4f70              | Op
-00001330: 7469 6f6e 616c 2020 7c20 606d 792d 6375  tional  | `my-cu
-00001340: 7374 6f6d 2d77 6f72 6b67 726f 7570 6020  stom-workgroup` 
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 207c 0a7c 206e 756d 5f72 6574 7269     |.| num_retri
-00001370: 6573 2020 2020 2020 7c20 4e75 6d62 6572  es      | Number
-00001380: 206f 6620 7469 6d65 7320 746f 2072 6574   of times to ret
-00001390: 7279 2061 2066 6169 6c69 6e67 2071 7565  ry a failing que
-000013a0: 7279 2020 2020 2020 2020 2020 2020 2020  ry              
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 2020 2020 207c 204f 7074 696f           | Optio
-000013d0: 6e61 6c20 207c 2060 3360 2020 2020 2020  nal  | `3`      
+000010e0: 2020 2020 2020 7c20 5265 7175 6972 6564        | Required
+000010f0: 2020 7c20 6065 752d 7765 7374 2d31 6020    | `eu-west-1` 
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00001120: 2073 6368 656d 6120 2020 2020 2020 2020   schema         
+00001130: 2020 7c20 5370 6563 6966 7920 7468 6520    | Specify the 
+00001140: 7363 6865 6d61 2028 4174 6865 6e61 2064  schema (Athena d
+00001150: 6174 6162 6173 6529 2074 6f20 6275 696c  atabase) to buil
+00001160: 6420 6d6f 6465 6c73 2069 6e74 6f20 286c  d models into (l
+00001170: 6f77 6572 6361 7365 202a 2a6f 6e6c 792a  owercase **only*
+00001180: 2a29 207c 2052 6571 7569 7265 6420 207c  *) | Required  |
+00001190: 2060 6462 7460 2020 2020 2020 2020 2020   `dbt`          
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2020 2020 2020 2020 7c0a 7c20 6461            |.| da
+000011c0: 7461 6261 7365 2020 2020 2020 2020 207c  tabase         |
+000011d0: 2053 7065 6369 6679 2074 6865 2064 6174   Specify the dat
+000011e0: 6162 6173 6520 2844 6174 6120 6361 7461  abase (Data cata
+000011f0: 6c6f 6729 2074 6f20 6275 696c 6420 6d6f  log) to build mo
+00001200: 6465 6c73 2069 6e74 6f20 286c 6f77 6572  dels into (lower
+00001210: 6361 7365 202a 2a6f 6e6c 792a 2a29 2020  case **only**)  
+00001220: 7c20 5265 7175 6972 6564 2020 7c20 6061  | Required  | `a
+00001230: 7773 6461 7461 6361 7461 6c6f 6760 2020  wsdatacatalog`  
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 2020 2020 207c 0a7c 2070 6f6c 6c5f         |.| poll_
+00001260: 696e 7465 7276 616c 2020 2020 7c20 496e  interval    | In
+00001270: 7465 7276 616c 2069 6e20 7365 636f 6e64  terval in second
+00001280: 7320 746f 2075 7365 2066 6f72 2070 6f6c  s to use for pol
+00001290: 6c69 6e67 2074 6865 2073 7461 7475 7320  ling the status 
+000012a0: 6f66 2071 7565 7279 2072 6573 756c 7473  of query results
+000012b0: 2069 6e20 4174 6865 6e61 2020 207c 204f   in Athena   | O
+000012c0: 7074 696f 6e61 6c20 207c 2060 3560 2020  ptional  | `5`  
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 7c0a 7c20 6177 735f 7072 6f66      |.| aws_prof
+00001300: 696c 655f 6e61 6d65 207c 2050 726f 6669  ile_name | Profi
+00001310: 6c65 2074 6f20 7573 6520 6672 6f6d 2079  le to use from y
+00001320: 6f75 7220 4157 5320 7368 6172 6564 2063  our AWS shared c
+00001330: 7265 6465 6e74 6961 6c73 2066 696c 652e  redentials file.
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2020 2020 2020 7c20 4f70 7469            | Opti
+00001360: 6f6e 616c 2020 7c20 606d 792d 7072 6f66  onal  | `my-prof
+00001370: 696c 6560 2020 2020 2020 2020 2020 2020  ile`            
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 207c 0a7c 2077 6f72 6b5f 6772 6f75 7020   |.| work_group 
+000013a0: 2020 2020 2020 7c20 4964 656e 7469 6669        | Identifi
+000013b0: 6572 206f 6620 4174 6865 6e61 2077 6f72  er of Athena wor
+000013c0: 6b67 726f 7570 2020 2020 2020 2020 2020  kgroup          
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 7c0a 7c20 6c66 5f74 6167 7320 2020 2020  |.| lf_tags     
-00001410: 2020 2020 207c 2044 6566 6175 6c74 206c       | Default l
-00001420: 6620 7461 6773 2074 6f20 6170 706c 7920  f tags to apply 
-00001430: 746f 2061 6e79 2064 6174 6162 6173 6520  to any database 
-00001440: 6372 6561 7465 6420 6279 2064 6274 2020  created by dbt  
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 2020 2020 2020 7c20 4f70 7469 6f6e 616c        | Optional
-00001470: 2020 7c20 607b 226f 7269 6769 6e22 3a20    | `{"origin": 
-00001480: 2264 6274 222c 2022 7465 616d 223a 2022  "dbt", "team": "
-00001490: 616e 616c 7974 6963 7322 7d60 207c 0a0a  analytics"}` |..
-000014a0: 2a2a 4578 616d 706c 6520 7072 6f66 696c  **Example profil
-000014b0: 6573 2e79 6d6c 2065 6e74 7279 3a2a 2a0a  es.yml entry:**.
-000014c0: 6060 6079 616d 6c0a 6174 6865 6e61 3a0a  ```yaml.athena:.
-000014d0: 2020 7461 7267 6574 3a20 6465 760a 2020    target: dev.  
-000014e0: 6f75 7470 7574 733a 0a20 2020 2064 6576  outputs:.    dev
-000014f0: 3a0a 2020 2020 2020 7479 7065 3a20 6174  :.      type: at
-00001500: 6865 6e61 0a20 2020 2020 2073 335f 7374  hena.      s3_st
-00001510: 6167 696e 675f 6469 723a 2073 333a 2f2f  aging_dir: s3://
-00001520: 6174 6865 6e61 2d71 7565 7279 2d72 6573  athena-query-res
-00001530: 756c 7473 2f64 6274 2f0a 2020 2020 2020  ults/dbt/.      
-00001540: 7333 5f64 6174 615f 6469 723a 2073 333a  s3_data_dir: s3:
-00001550: 2f2f 796f 7572 5f73 335f 6275 636b 6574  //your_s3_bucket
-00001560: 2f64 6274 2f0a 2020 2020 2020 7333 5f64  /dbt/.      s3_d
-00001570: 6174 615f 6e61 6d69 6e67 3a20 7363 6865  ata_naming: sche
-00001580: 6d61 5f74 6162 6c65 0a20 2020 2020 2072  ma_table.      r
-00001590: 6567 696f 6e5f 6e61 6d65 3a20 6575 2d77  egion_name: eu-w
-000015a0: 6573 742d 310a 2020 2020 2020 7363 6865  est-1.      sche
-000015b0: 6d61 3a20 6462 740a 2020 2020 2020 6461  ma: dbt.      da
-000015c0: 7461 6261 7365 3a20 6177 7364 6174 6163  tabase: awsdatac
-000015d0: 6174 616c 6f67 0a20 2020 2020 2061 7773  atalog.      aws
-000015e0: 5f70 726f 6669 6c65 5f6e 616d 653a 206d  _profile_name: m
-000015f0: 792d 7072 6f66 696c 650a 2020 2020 2020  y-profile.      
-00001600: 776f 726b 5f67 726f 7570 3a20 6d79 2d77  work_group: my-w
-00001610: 6f72 6b67 726f 7570 0a20 2020 2020 206c  orkgroup.      l
-00001620: 665f 7461 6773 3a0a 2020 2020 2020 2020  f_tags:.        
-00001630: 6f72 6967 696e 3a20 6462 740a 2020 2020  origin: dbt.    
-00001640: 2020 2020 7465 616d 3a20 616e 616c 7974      team: analyt
-00001650: 6963 730a 6060 600a 0a5f 4164 6469 7469  ics.```.._Additi
-00001660: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
-00001670: 5f0a 2a20 6074 6872 6561 6473 6020 6973  _.* `threads` is
-00001680: 2073 7570 706f 7274 6564 0a2a 2060 6461   supported.* `da
-00001690: 7461 6261 7365 6020 616e 6420 6063 6174  tabase` and `cat
-000016a0: 616c 6f67 6020 6361 6e20 6265 2075 7365  alog` can be use
-000016b0: 6420 696e 7465 7263 6861 6e67 6561 626c  d interchangeabl
-000016c0: 790a 0a23 2323 204d 6f64 656c 730a 0a23  y..### Models..#
-000016d0: 2323 2320 5461 626c 6520 436f 6e66 6967  ### Table Config
-000016e0: 7572 6174 696f 6e0a 0a2a 2060 6578 7465  uration..* `exte
-000016f0: 726e 616c 5f6c 6f63 6174 696f 6e60 2028  rnal_location` (
-00001700: 6064 6566 6175 6c74 3d6e 6f6e 6560 290a  `default=none`).
-00001710: 2020 2a20 4966 2073 6574 2c20 7468 6520    * If set, the 
-00001720: 6675 6c6c 2053 3320 7061 7468 2069 6e20  full S3 path in 
-00001730: 7768 6963 6820 7468 6520 7461 626c 6520  which the table 
-00001740: 7769 6c6c 2062 6520 7361 7665 642e 2028  will be saved. (
-00001750: 446f 6573 206e 6f74 2077 6f72 6b20 7769  Does not work wi
-00001760: 7468 2049 6365 6265 7267 2074 6162 6c65  th Iceberg table
-00001770: 292e 0a2a 2060 7061 7274 6974 696f 6e65  )..* `partitione
-00001780: 645f 6279 6020 2860 6465 6661 756c 743d  d_by` (`default=
-00001790: 6e6f 6e65 6029 0a20 202a 2041 6e20 6172  none`).  * An ar
-000017a0: 7261 7920 6c69 7374 206f 6620 636f 6c75  ray list of colu
-000017b0: 6d6e 7320 6279 2077 6869 6368 2074 6865  mns by which the
-000017c0: 2074 6162 6c65 2077 696c 6c20 6265 2070   table will be p
-000017d0: 6172 7469 7469 6f6e 6564 0a20 202a 204c  artitioned.  * L
-000017e0: 696d 6974 6564 2074 6f20 6372 6561 7469  imited to creati
-000017f0: 6f6e 206f 6620 3130 3020 7061 7274 6974  on of 100 partit
-00001800: 696f 6e73 2028 5f63 7572 7265 6e74 6c79  ions (_currently
-00001810: 5f29 0a2a 2060 6275 636b 6574 6564 5f62  _).* `bucketed_b
-00001820: 7960 2028 6064 6566 6175 6c74 3d6e 6f6e  y` (`default=non
-00001830: 6560 290a 2020 2a20 416e 2061 7272 6179  e`).  * An array
-00001840: 206c 6973 7420 6f66 2063 6f6c 756d 6e73   list of columns
-00001850: 2074 6f20 6275 636b 6574 2064 6174 612c   to bucket data,
-00001860: 2069 676e 6f72 6564 2069 6620 7573 696e   ignored if usin
-00001870: 6720 4963 6562 6572 670a 2a20 6062 7563  g Iceberg.* `buc
-00001880: 6b65 745f 636f 756e 7460 2028 6064 6566  ket_count` (`def
-00001890: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-000018a0: 5468 6520 6e75 6d62 6572 206f 6620 6275  The number of bu
-000018b0: 636b 6574 7320 666f 7220 6275 636b 6574  ckets for bucket
-000018c0: 696e 6720 796f 7572 2064 6174 612c 2069  ing your data, i
-000018d0: 676e 6f72 6564 2069 6620 7573 696e 6720  gnored if using 
-000018e0: 4963 6562 6572 670a 2a20 6074 6162 6c65  Iceberg.* `table
-000018f0: 5f74 7970 6560 2028 6064 6566 6175 6c74  _type` (`default
-00001900: 3d27 6869 7665 2760 290a 2020 2a20 5468  ='hive'`).  * Th
-00001910: 6520 7479 7065 206f 6620 7461 626c 650a  e type of table.
-00001920: 2020 2a20 5375 7070 6f72 7473 2060 6869    * Supports `hi
-00001930: 7665 6020 6f72 2060 6963 6562 6572 6760  ve` or `iceberg`
-00001940: 0a2a 2060 666f 726d 6174 6020 2860 6465  .* `format` (`de
-00001950: 6661 756c 743d 2770 6172 7175 6574 2760  fault='parquet'`
-00001960: 290a 2020 2a20 5468 6520 6461 7461 2066  ).  * The data f
-00001970: 6f72 6d61 7420 666f 7220 7468 6520 7461  ormat for the ta
-00001980: 626c 650a 2020 2a20 5375 7070 6f72 7473  ble.  * Supports
-00001990: 2060 4f52 4360 2c20 6050 4152 5155 4554   `ORC`, `PARQUET
-000019a0: 602c 2060 4156 524f 602c 2060 4a53 4f4e  `, `AVRO`, `JSON
-000019b0: 602c 2060 5445 5854 4649 4c45 600a 2a20  `, `TEXTFILE`.* 
-000019c0: 6077 7269 7465 5f63 6f6d 7072 6573 7369  `write_compressi
-000019d0: 6f6e 6020 2860 6465 6661 756c 743d 6e6f  on` (`default=no
-000019e0: 6e65 6029 0a20 202a 2054 6865 2063 6f6d  ne`).  * The com
-000019f0: 7072 6573 7369 6f6e 2074 7970 6520 746f  pression type to
-00001a00: 2075 7365 2066 6f72 2061 6e79 2073 746f   use for any sto
-00001a10: 7261 6765 2066 6f72 6d61 7420 7468 6174  rage format that
-00001a20: 2061 6c6c 6f77 7320 636f 6d70 7265 7373   allows compress
-00001a30: 696f 6e20 746f 2062 6520 7370 6563 6966  ion to be specif
-00001a40: 6965 642e 2054 6f20 7365 6520 7768 6963  ied. To see whic
-00001a50: 6820 6f70 7469 6f6e 7320 6172 6520 6176  h options are av
-00001a60: 6169 6c61 626c 652c 2063 6865 636b 206f  ailable, check o
-00001a70: 7574 205b 4352 4541 5445 2054 4142 4c45  ut [CREATE TABLE
-00001a80: 2041 535d 5b63 7265 6174 652d 7461 626c   AS][create-tabl
-00001a90: 652d 6173 5d0a 2a20 6066 6965 6c64 5f64  e-as].* `field_d
-00001aa0: 656c 696d 6974 6572 6020 2860 6465 6661  elimiter` (`defa
-00001ab0: 756c 743d 6e6f 6e65 6029 0a20 202a 2043  ult=none`).  * C
-00001ac0: 7573 746f 6d20 6669 656c 6420 6465 6c69  ustom field deli
-00001ad0: 6d69 7465 722c 2066 6f72 2077 6865 6e20  miter, for when 
-00001ae0: 666f 726d 6174 2069 7320 7365 7420 746f  format is set to
-00001af0: 2060 5445 5854 4649 4c45 600a 2a20 6074   `TEXTFILE`.* `t
-00001b00: 6162 6c65 5f70 726f 7065 7274 6965 7360  able_properties`
-00001b10: 3a20 7461 626c 6520 7072 6f70 6572 7469  : table properti
-00001b20: 6573 2074 6f20 6164 6420 746f 2074 6865  es to add to the
-00001b30: 2074 6162 6c65 2c20 7661 6c69 6420 666f   table, valid fo
-00001b40: 7220 4963 6562 6572 6720 6f6e 6c79 0a2a  r Iceberg only.*
-00001b50: 2060 6c66 5f74 6167 7360 2028 6064 6566   `lf_tags` (`def
-00001b60: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-00001b70: 6c66 2074 6167 7320 746f 2061 7373 6f63  lf tags to assoc
-00001b80: 6961 7465 2077 6974 6820 7468 6520 7461  iate with the ta
-00001b90: 626c 650a 2020 2a20 666f 726d 6174 3a20  ble.  * format: 
-00001ba0: 607b 2274 6167 3122 3a20 2276 616c 7565  `{"tag1": "value
-00001bb0: 3122 2c20 2274 6167 3222 3a20 2276 616c  1", "tag2": "val
-00001bc0: 7565 3222 7d60 0a2a 2060 6c66 5f74 6167  ue2"}`.* `lf_tag
-00001bd0: 735f 636f 6c75 6d6e 7360 2028 6064 6566  s_columns` (`def
-00001be0: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-00001bf0: 6c66 2074 6167 7320 746f 2061 7373 6f63  lf tags to assoc
-00001c00: 6961 7465 2077 6974 6820 7468 6520 7461  iate with the ta
-00001c10: 626c 6520 636f 6c75 6d6e 730a 2020 2a20  ble columns.  * 
-00001c20: 666f 726d 6174 3a20 607b 2274 6167 3122  format: `{"tag1"
-00001c30: 3a20 7b22 7661 6c75 6531 223a 205b 2263  : {"value1": ["c
-00001c40: 6f6c 756d 6e31 223a 2022 636f 6c75 6d6e  olumn1": "column
-00001c50: 3222 5d7d 7d60 0a0a 2323 2323 2054 6162  2"]}}`..#### Tab
-00001c60: 6c65 206c 6f63 6174 696f 6e0a 0a54 6865  le location..The
-00001c70: 206c 6f63 6174 696f 6e20 696e 2077 6869   location in whi
-00001c80: 6368 2061 2074 6162 6c65 2069 7320 7361  ch a table is sa
-00001c90: 7665 6420 6973 2064 6574 6572 6d69 6e65  ved is determine
-00001ca0: 6420 6279 3a0a 0a31 2e20 4966 2060 6578  d by:..1. If `ex
-00001cb0: 7465 726e 616c 5f6c 6f63 6174 696f 6e60  ternal_location`
-00001cc0: 2069 7320 6465 6669 6e65 642c 2074 6861   is defined, tha
-00001cd0: 7420 7661 6c75 6520 6973 2075 7365 642e  t value is used.
-00001ce0: 0a32 2e20 4966 2060 7333 5f64 6174 615f  .2. If `s3_data_
-00001cf0: 6469 7260 2069 7320 6465 6669 6e65 642c  dir` is defined,
-00001d00: 2074 6865 2070 6174 6820 6973 2064 6574   the path is det
-00001d10: 6572 6d69 6e65 6420 6279 2074 6861 7420  ermined by that 
-00001d20: 616e 6420 6073 335f 6461 7461 5f6e 616d  and `s3_data_nam
-00001d30: 696e 6760 0a33 2e20 4966 2060 7333 5f64  ing`.3. If `s3_d
-00001d40: 6174 615f 6469 7260 2069 7320 6e6f 7420  ata_dir` is not 
-00001d50: 6465 6669 6e65 6420 6461 7461 2069 7320  defined data is 
-00001d60: 7374 6f72 6564 2075 6e64 6572 2060 7333  stored under `s3
-00001d70: 5f73 7461 6769 6e67 5f64 6972 2f74 6162  _staging_dir/tab
-00001d80: 6c65 732f 600a 0a48 6572 6520 616c 6c20  les/`..Here all 
-00001d90: 7468 6520 6f70 7469 6f6e 7320 6176 6169  the options avai
-00001da0: 6c61 626c 6520 666f 7220 6073 335f 6461  lable for `s3_da
-00001db0: 7461 5f6e 616d 696e 6760 3a0a 2a20 6075  ta_naming`:.* `u
-00001dc0: 7569 6460 3a20 607b 7333 5f64 6174 615f  uid`: `{s3_data_
-00001dd0: 6469 727d 2f7b 7575 6964 3428 297d 2f60  dir}/{uuid4()}/`
-00001de0: 0a2a 2060 7461 626c 655f 7461 626c 6560  .* `table_table`
-00001df0: 3a20 607b 7333 5f64 6174 615f 6469 727d  : `{s3_data_dir}
-00001e00: 2f7b 7461 626c 657d 2f60 0a2a 2060 7461  /{table}/`.* `ta
-00001e10: 626c 655f 756e 6971 7565 603a 2060 7b73  ble_unique`: `{s
-00001e20: 335f 6461 7461 5f64 6972 7d2f 7b74 6162  3_data_dir}/{tab
-00001e30: 6c65 7d2f 7b75 7569 6434 2829 7d2f 600a  le}/{uuid4()}/`.
-00001e40: 2a20 6073 6368 656d 615f 7461 626c 6560  * `schema_table`
-00001e50: 3a20 607b 7333 5f64 6174 615f 6469 727d  : `{s3_data_dir}
-00001e60: 2f7b 7363 6865 6d61 7d2f 7b74 6162 6c65  /{schema}/{table
-00001e70: 7d2f 600a 2a20 6073 335f 6461 7461 5f6e  }/`.* `s3_data_n
-00001e80: 616d 696e 673d 7363 6865 6d61 5f74 6162  aming=schema_tab
-00001e90: 6c65 5f75 6e69 7175 6560 3a20 607b 7333  le_unique`: `{s3
-00001ea0: 5f64 6174 615f 6469 727d 2f7b 7363 6865  _data_dir}/{sche
-00001eb0: 6d61 7d2f 7b74 6162 6c65 7d2f 7b75 7569  ma}/{table}/{uui
-00001ec0: 6434 2829 7d2f 600a 0a49 7427 7320 706f  d4()}/`..It's po
-00001ed0: 7373 6962 6c65 2074 6f20 7365 7420 7468  ssible to set th
-00001ee0: 6520 6073 335f 6461 7461 5f6e 616d 696e  e `s3_data_namin
-00001ef0: 6760 2067 6c6f 6261 6c6c 7920 696e 2074  g` globally in t
-00001f00: 6865 2074 6172 6765 7420 7072 6f66 696c  he target profil
-00001f10: 652c 206f 7220 6f76 6572 7772 6974 6520  e, or overwrite 
-00001f20: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
-00001f30: 2074 6162 6c65 2063 6f6e 6669 672c 0a6f   table config,.o
-00001f40: 7220 7365 7474 696e 6720 7570 2074 6865  r setting up the
-00001f50: 2076 616c 7565 2066 6f72 2067 726f 7570   value for group
-00001f60: 7320 6f66 206d 6f64 656c 2069 6e20 6462  s of model in db
-00001f70: 745f 7072 6f6a 6563 742e 796d 6c2e 0a0a  t_project.yml...
-00001f80: 3e20 4e6f 7465 3a20 7768 656e 2075 7369  > Note: when usi
-00001f90: 6e67 2061 2077 6f72 6b20 6772 6f75 7020  ng a work group 
-00001fa0: 7769 7468 2061 2064 6566 6175 6c74 206f  with a default o
-00001fb0: 7574 7075 7420 6c6f 6361 7469 6f6e 2063  utput location c
-00001fc0: 6f6e 6669 6775 7265 642c 2060 7333 5f64  onfigured, `s3_d
-00001fd0: 6174 615f 6e61 6d69 6e67 6020 616e 6420  ata_naming` and 
-00001fe0: 616e 7920 636f 6e66 6967 7572 6564 2062  any configured b
-00001ff0: 7563 6b65 7473 2061 7265 2069 676e 6f72  uckets are ignor
-00002000: 6564 2061 6e64 2074 6865 206c 6f63 6174  ed and the locat
-00002010: 696f 6e20 636f 6e66 6967 7572 6564 2069  ion configured i
-00002020: 6e20 7468 6520 776f 726b 2067 726f 7570  n the work group
-00002030: 2069 7320 7573 6564 2e0a 0a0a 2323 2323   is used....####
-00002040: 2049 6e63 7265 6d65 6e74 616c 206d 6f64   Incremental mod
-00002050: 656c 730a 0a53 7570 706f 7274 2066 6f72  els..Support for
-00002060: 205b 696e 6372 656d 656e 7461 6c20 6d6f   [incremental mo
-00002070: 6465 6c73 5d28 6874 7470 733a 2f2f 646f  dels](https://do
-00002080: 6373 2e67 6574 6462 742e 636f 6d2f 646f  cs.getdbt.com/do
-00002090: 6373 2f62 7569 6c64 2f69 6e63 7265 6d65  cs/build/increme
-000020a0: 6e74 616c 2d6d 6f64 656c 7329 2e0a 0a54  ntal-models)...T
-000020b0: 6865 7365 2073 7472 6174 6567 6965 7320  hese strategies 
-000020c0: 6172 6520 7375 7070 6f72 7465 643a 0a0a  are supported:..
-000020d0: 2a20 6069 6e73 6572 745f 6f76 6572 7772  * `insert_overwr
-000020e0: 6974 6560 2028 6465 6661 756c 7429 3a20  ite` (default): 
-000020f0: 5468 6520 696e 7365 7274 206f 7665 7277  The insert overw
-00002100: 7269 7465 2073 7472 6174 6567 7920 6465  rite strategy de
-00002110: 6c65 7465 7320 7468 6520 6f76 6572 6c61  letes the overla
-00002120: 7070 696e 6720 7061 7274 6974 696f 6e73  pping partitions
-00002130: 2066 726f 6d20 7468 6520 6465 7374 696e   from the destin
-00002140: 6174 696f 6e0a 7461 626c 652c 2061 6e64  ation.table, and
-00002150: 2074 6865 6e20 696e 7365 7274 7320 7468   then inserts th
-00002160: 6520 6e65 7720 7265 636f 7264 7320 6672  e new records fr
-00002170: 6f6d 2074 6865 2073 6f75 7263 652e 2054  om the source. T
-00002180: 6869 7320 7374 7261 7465 6779 2064 6570  his strategy dep
-00002190: 656e 6473 206f 6e20 7468 6520 6070 6172  ends on the `par
-000021a0: 7469 7469 6f6e 6564 5f62 7960 206b 6579  titioned_by` key
-000021b0: 776f 7264 2120 4966 206e 6f0a 7061 7274  word! If no.part
-000021c0: 6974 696f 6e73 2061 7265 2064 6566 696e  itions are defin
-000021d0: 6564 2c20 6462 7420 7769 6c6c 2066 616c  ed, dbt will fal
-000021e0: 6c20 6261 636b 2074 6f20 7468 6520 6061  l back to the `a
-000021f0: 7070 656e 6460 2073 7472 6174 6567 792e  ppend` strategy.
-00002200: 0a2a 2060 6170 7065 6e64 603a 2049 6e73  .* `append`: Ins
-00002210: 6572 7420 6e65 7720 7265 636f 7264 7320  ert new records 
-00002220: 7769 7468 6f75 7420 7570 6461 7469 6e67  without updating
-00002230: 2c20 6465 6c65 7469 6e67 206f 7220 6f76  , deleting or ov
-00002240: 6572 7772 6974 696e 6720 616e 7920 6578  erwriting any ex
-00002250: 6973 7469 6e67 2064 6174 612e 2054 6865  isting data. The
-00002260: 7265 206d 6967 6874 2062 6520 6475 706c  re might be dupl
-00002270: 6963 6174 650a 6461 7461 2028 652e 672e  icate.data (e.g.
-00002280: 2067 7265 6174 2066 6f72 206c 6f67 206f   great for log o
-00002290: 7220 6869 7374 6f72 6963 616c 2064 6174  r historical dat
-000022a0: 6129 2e0a 2a20 606d 6572 6765 603a 2043  a)..* `merge`: C
-000022b0: 6f6e 6469 7469 6f6e 616c 6c79 2075 7064  onditionally upd
-000022c0: 6174 6573 2c20 6465 6c65 7465 732c 206f  ates, deletes, o
-000022d0: 7220 696e 7365 7274 7320 726f 7773 2069  r inserts rows i
-000022e0: 6e74 6f20 616e 2049 6365 6265 7267 2074  nto an Iceberg t
-000022f0: 6162 6c65 2e20 5573 6564 2069 6e20 636f  able. Used in co
-00002300: 6d62 696e 6174 696f 6e20 7769 7468 2060  mbination with `
-00002310: 756e 6971 7565 5f6b 6579 602e 0a4f 6e6c  unique_key`..Onl
-00002320: 7920 6176 6169 6c61 626c 6520 7768 656e  y available when
-00002330: 2075 7369 6e67 2049 6365 6265 7267 2e0a   using Iceberg..
-00002340: 0a23 2323 2320 4f6e 2073 6368 656d 6120  .#### On schema 
-00002350: 6368 616e 6765 0a0a 606f 6e5f 7363 6865  change..`on_sche
-00002360: 6d61 5f63 6861 6e67 6560 2069 7320 616e  ma_change` is an
-00002370: 206f 7074 696f 6e20 746f 2072 6566 6c65   option to refle
-00002380: 6374 2063 6861 6e67 6573 206f 6620 7363  ct changes of sc
-00002390: 6865 6d61 2069 6e20 696e 6372 656d 656e  hema in incremen
-000023a0: 7461 6c20 6d6f 6465 6c73 2e0a 5468 6520  tal models..The 
-000023b0: 666f 6c6c 6f77 696e 6720 6f70 7469 6f6e  following option
-000023c0: 7320 6172 6520 7375 7070 6f72 7465 643a  s are supported:
-000023d0: 0a2a 2060 6967 6e6f 7265 6020 2864 6566  .* `ignore` (def
-000023e0: 6175 6c74 290a 2a20 6066 6169 6c60 0a2a  ault).* `fail`.*
-000023f0: 2060 6170 7065 6e64 5f6e 6577 5f63 6f6c   `append_new_col
-00002400: 756d 6e73 600a 2a20 6073 796e 635f 616c  umns`.* `sync_al
-00002410: 6c5f 636f 6c75 6d6e 7360 0a0a 496e 2064  l_columns`..In d
-00002420: 6574 6169 6c2c 2070 6c65 6173 6520 7265  etail, please re
-00002430: 6665 7220 746f 205b 6462 7420 646f 6373  fer to [dbt docs
-00002440: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
-00002450: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
-00002460: 7569 6c64 2f69 6e63 7265 6d65 6e74 616c  uild/incremental
-00002470: 2d6d 6f64 656c 7323 7768 6174 2d69 662d  -models#what-if-
-00002480: 7468 652d 636f 6c75 6d6e 732d 6f66 2d6d  the-columns-of-m
-00002490: 792d 696e 6372 656d 656e 7461 6c2d 6d6f  y-incremental-mo
-000024a0: 6465 6c2d 6368 616e 6765 292e 0a0a 0a23  del-change)....#
-000024b0: 2323 2320 4963 6562 6572 670a 0a54 6865  ### Iceberg..The
-000024c0: 2061 6461 7074 6572 2073 7570 706f 7274   adapter support
-000024d0: 7320 7461 626c 6520 6d61 7465 7269 616c  s table material
-000024e0: 697a 6174 696f 6e20 666f 7220 4963 6562  ization for Iceb
-000024f0: 6572 672e 0a0a 546f 2067 6574 2073 7461  erg...To get sta
-00002500: 7274 6564 206a 7573 7420 6164 6420 7468  rted just add th
-00002510: 6973 2061 7320 796f 7572 206d 6f64 656c  is as your model
-00002520: 3a0a 6060 600a 7b7b 2063 6f6e 6669 6728  :.```.{{ config(
-00002530: 0a20 2020 206d 6174 6572 6961 6c69 7a65  .    materialize
-00002540: 643d 2774 6162 6c65 272c 0a20 2020 2074  d='table',.    t
-00002550: 6162 6c65 5f74 7970 653d 2769 6365 6265  able_type='icebe
-00002560: 7267 272c 0a20 2020 2066 6f72 6d61 743d  rg',.    format=
-00002570: 2770 6172 7175 6574 272c 0a20 2020 2070  'parquet',.    p
-00002580: 6172 7469 7469 6f6e 6564 5f62 793d 5b27  artitioned_by=['
-00002590: 6275 636b 6574 2875 7365 725f 6964 2c20  bucket(user_id, 
-000025a0: 3529 275d 2c0a 2020 2020 7461 626c 655f  5)'],.    table_
-000025b0: 7072 6f70 6572 7469 6573 3d7b 0a20 2020  properties={.   
-000025c0: 2009 276f 7074 696d 697a 655f 7265 7772   .'optimize_rewr
-000025d0: 6974 655f 6465 6c65 7465 5f66 696c 655f  ite_delete_file_
-000025e0: 7468 7265 7368 6f6c 6427 3a20 2732 270a  threshold': '2'.
-000025f0: 2020 2020 097d 0a29 207d 7d0a 0a53 454c      .}.) }}..SEL
-00002600: 4543 540a 0927 4127 2041 5320 7573 6572  ECT..'A' AS user
-00002610: 5f69 642c 0a09 2770 6927 2041 5320 6e61  _id,..'pi' AS na
-00002620: 6d65 2c0a 0927 6163 7469 7665 2720 4153  me,..'active' AS
-00002630: 2073 7461 7475 732c 0a09 3137 2e38 3920   status,..17.89 
-00002640: 4153 2063 6f73 742c 0a09 3120 4153 2071  AS cost,..1 AS q
-00002650: 7561 6e74 6974 792c 0a09 3130 3030 3030  uantity,..100000
-00002660: 3030 3020 4153 2071 7561 6e74 6974 795f  000 AS quantity_
-00002670: 6269 672c 0a09 6375 7272 656e 745f 6461  big,..current_da
-00002680: 7465 2041 5320 6d79 5f64 6174 650a 6060  te AS my_date.``
-00002690: 600a 0a49 6365 6265 7267 2073 7570 706f  `..Iceberg suppo
-000026a0: 7274 7320 6275 636b 6574 696e 6720 6173  rts bucketing as
-000026b0: 2068 6964 6465 6e20 7061 7274 6974 696f   hidden partitio
-000026c0: 6e73 2c20 7468 6572 6566 6f72 6520 7573  ns, therefore us
-000026d0: 6520 7468 6520 6070 6172 7469 7469 6f6e  e the `partition
-000026e0: 6564 5f62 7960 2063 6f6e 6669 6720 746f  ed_by` config to
-000026f0: 2061 6464 2073 7065 6369 6669 6320 6275   add specific bu
-00002700: 636b 6574 696e 6720 636f 6e64 6974 696f  cketing conditio
-00002710: 6e73 2e0a 0a49 6365 6265 7267 2073 7570  ns...Iceberg sup
-00002720: 706f 7274 7320 7365 7665 7261 6c20 7461  ports several ta
-00002730: 626c 6520 666f 726d 6174 7320 666f 7220  ble formats for 
-00002740: 6461 7461 203a 2060 5041 5251 5545 5460  data : `PARQUET`
-00002750: 2c20 6041 5652 4f60 2061 6e64 2060 4f52  , `AVRO` and `OR
-00002760: 4360 2e0a 0a49 7420 6973 2070 6f73 7369  C`...It is possi
-00002770: 626c 6520 746f 2075 7365 2069 6365 6265  ble to use icebe
-00002780: 7267 2069 6e20 616e 2069 6e63 7265 6d65  rg in an increme
-00002790: 6e74 616c 2066 6173 6869 6f6e 2c20 7370  ntal fashion, sp
-000027a0: 6563 6966 6963 616c 6c79 2032 2073 7472  ecifically 2 str
-000027b0: 6174 6567 6965 7320 6172 6520 7375 7070  ategies are supp
-000027c0: 6f72 7465 643a 0a2a 2060 6170 7065 6e64  orted:.* `append
-000027d0: 603a 206e 6577 2072 6563 6f72 6473 2061  `: new records a
-000027e0: 7265 2061 7070 656e 6465 6420 746f 2074  re appended to t
-000027f0: 6865 2074 6162 6c65 2c20 7468 6973 2063  he table, this c
-00002800: 616e 206c 6561 6420 746f 2064 7570 6c69  an lead to dupli
-00002810: 6361 7465 730a 2a20 606d 6572 6765 603a  cates.* `merge`:
-00002820: 206d 7573 7420 6265 2075 7365 6420 696e   must be used in
-00002830: 2063 6f6d 6269 6e61 7469 6f6e 2077 6974   combination wit
-00002840: 6820 6075 6e69 7175 655f 6b65 7960 2061  h `unique_key` a
-00002850: 6e64 2069 7427 7320 6f6e 6c79 2061 7661  nd it's only ava
-00002860: 696c 6162 6c65 2077 6974 6820 456e 6769  ilable with Engi
-00002870: 6e65 2076 6572 7369 6f6e 2033 2e0a 2020  ne version 3..  
-00002880: 2049 7420 7065 7266 6f72 6d73 2061 6e20   It performs an 
-00002890: 7570 7365 7274 2c20 6e65 7720 7265 636f  upsert, new reco
-000028a0: 7264 2061 7265 2061 6464 6564 2c20 616e  rd are added, an
-000028b0: 6420 7265 636f 7264 2061 6c72 6561 6479  d record already
-000028c0: 2065 7869 7374 696e 6720 6172 6520 7570   existing are up
-000028d0: 6461 7465 640a 0a23 2323 2320 4869 6768  dated..#### High
-000028e0: 2061 7661 696c 6162 6c65 2074 6162 6c65   available table
-000028f0: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-00002900: 0a54 6865 2063 7572 7265 6e74 2069 6d70  .The current imp
-00002910: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
-00002920: 6865 2074 6162 6c65 206d 6174 6572 6961  he table materia
-00002930: 6c69 7a61 7469 6f6e 2063 616e 206c 6561  lization can lea
-00002940: 6420 746f 2064 6f77 6e74 696d 652c 2061  d to downtime, a
-00002950: 7320 7461 7267 6574 2074 6162 6c65 2069  s target table i
-00002960: 7320 6472 6f70 7065 6420 616e 6420 7265  s dropped and re
-00002970: 2d63 7265 6174 6564 2e0a 546f 2068 6176  -created..To hav
-00002980: 6520 7468 6520 6c65 7373 2064 6573 7472  e the less destr
-00002990: 7563 7469 7665 2062 6568 6176 696f 7220  uctive behavior 
-000029a0: 6974 2773 2070 6f73 7369 626c 6520 746f  it's possible to
-000029b0: 2075 7365 2060 7461 626c 653d 2774 6162   use `table='tab
-000029c0: 6c65 5f68 6976 655f 6861 2760 206d 6174  le_hive_ha'` mat
-000029d0: 6572 6961 6c69 7a61 7469 6f6e 2e0a 2a2a  erialization..**
-000029e0: 7461 626c 655f 6869 7665 5f68 612a 2a20  table_hive_ha** 
-000029f0: 6c65 7665 7261 6765 2074 6865 2074 6162  leverage the tab
-00002a00: 6c65 2076 6572 7369 6f6e 7320 6665 6174  le versions feat
-00002a10: 7572 6520 6f66 2067 6c75 6520 6361 7461  ure of glue cata
-00002a20: 6c6f 672c 2063 7265 6174 696e 6720 6120  log, creating a 
-00002a30: 746d 7020 7461 626c 6520 616e 6420 7377  tmp table and sw
-00002a40: 6170 7069 6e67 0a74 6865 2074 6172 6765  apping.the targe
-00002a50: 7420 7461 626c 6520 746f 2074 6865 206c  t table to the l
-00002a60: 6f63 6174 696f 6e20 6f66 2074 6865 2074  ocation of the t
-00002a70: 6d70 2074 6162 6c65 2e0a 5468 6973 206d  mp table..This m
-00002a80: 6174 6572 6961 6c69 7a61 7469 6f6e 2069  aterialization i
-00002a90: 7320 6f6e 6c79 2061 7661 696c 6162 6c65  s only available
-00002aa0: 2066 6f72 2060 7461 626c 655f 7479 7065   for `table_type
-00002ab0: 3d68 6976 6560 2061 6e64 2072 6571 7569  =hive` and requi
-00002ac0: 7265 7320 7573 696e 6720 756e 6971 7565  res using unique
-00002ad0: 206c 6f63 6174 696f 6e73 2e0a 0a60 6060   locations...```
-00002ae0: 0a7b 7b20 636f 6e66 6967 280a 2020 2020  .{{ config(.    
-00002af0: 6d61 7465 7269 616c 697a 6564 3d27 7461  materialized='ta
-00002b00: 626c 655f 6869 7665 5f68 6127 2c0a 2020  ble_hive_ha',.  
-00002b10: 2020 666f 726d 6174 3d27 7061 7271 7565    format='parque
-00002b20: 7427 2c0a 2020 2020 7061 7274 6974 696f  t',.    partitio
-00002b30: 6e5f 6279 3d5b 2773 7461 7475 7327 5d2c  n_by=['status'],
-00002b40: 0a20 2020 2073 335f 6461 7461 5f6e 616d  .    s3_data_nam
-00002b50: 696e 673d 2774 6162 6c65 5f75 6e69 7175  ing='table_uniqu
-00002b60: 6527 0a29 207d 7d0a 0a0a 7365 6c65 6374  e'.) }}...select
-00002b70: 0a20 2027 6127 2061 7320 7573 6572 5f69  .  'a' as user_i
-00002b80: 642c 0a20 2027 7069 2720 6173 2075 7365  d,.  'pi' as use
-00002b90: 725f 6e61 6d65 2c0a 2020 2761 6374 6976  r_name,.  'activ
-00002ba0: 6527 2061 7320 7374 6174 7573 0a75 6e69  e' as status.uni
-00002bb0: 6f6e 2061 6c6c 0a73 656c 6563 740a 2020  on all.select.  
-00002bc0: 2762 2720 6173 2075 7365 725f 6964 2c0a  'b' as user_id,.
-00002bd0: 2020 2773 6827 2061 7320 7573 6572 5f6e    'sh' as user_n
-00002be0: 616d 652c 0a20 2027 6469 7361 626c 6564  ame,.  'disabled
-00002bf0: 2720 6173 2073 7461 7475 730a 6060 600a  ' as status.```.
-00002c00: 0a42 7920 6465 6661 756c 742c 2074 6865  .By default, the
-00002c10: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-00002c20: 206b 6565 7073 2074 6865 206c 6173 7420   keeps the last 
-00002c30: 3420 7461 626c 6520 7665 7273 696f 6e73  4 table versions
-00002c40: 2c20 796f 7520 6361 6e20 6368 616e 6765  , you can change
-00002c50: 2069 7420 7468 6174 2073 6574 7469 6e67   it that setting
-00002c60: 2060 7665 7273 696f 6e73 5f74 6f5f 6b65   `versions_to_ke
-00002c70: 6570 602e 0a0a 2323 2323 2320 4b6e 6f77  ep`...##### Know
-00002c80: 6e20 6973 7375 6573 0a2a 2057 6865 6e20  n issues.* When 
-00002c90: 7377 6170 7069 6e67 2066 726f 6d20 6120  swapping from a 
-00002ca0: 7461 626c 6520 7769 7468 2070 6172 7469  table with parti
-00002cb0: 7469 6f6e 7320 746f 2061 2074 6162 6c65  tions to a table
-00002cc0: 2077 6974 686f 7574 2028 616e 6420 7468   without (and th
-00002cd0: 6520 6f74 6865 7220 7761 7920 6172 6f75  e other way arou
-00002ce0: 6e64 292c 2074 6865 7265 2063 6f75 6c64  nd), there could
-00002cf0: 2062 6520 6120 6c69 7474 6c65 2064 6f77   be a little dow
-00002d00: 6e74 696d 652e 0a20 2049 6e20 6361 7365  ntime..  In case
-00002d10: 2068 6967 6820 7065 7266 6f72 6d61 6e63   high performanc
-00002d20: 6573 2061 7265 206e 6565 6465 6420 636f  es are needed co
-00002d30: 6e73 6964 6572 2062 7563 6b65 7469 6e67  nsider bucketing
-00002d40: 2069 6e73 7465 6164 206f 6620 7061 7274   instead of part
-00002d50: 6974 696f 6e73 0a2a 2042 7920 6465 6661  itions.* By defa
-00002d60: 756c 742c 2047 6c75 6520 2264 7570 6c69  ult, Glue "dupli
-00002d70: 6361 7465 2220 7468 6520 7665 7273 696f  cate" the versio
-00002d80: 6e73 2069 6e74 6572 6e61 6c6c 792c 2073  ns internally, s
-00002d90: 6f20 7468 6520 6c61 7374 2032 2076 6572  o the last 2 ver
-00002da0: 7369 6f6e 7320 6f66 2061 2074 6162 6c65  sions of a table
-00002db0: 2070 6f69 6e74 2074 6f20 7468 6520 7361   point to the sa
-00002dc0: 6d65 206c 6f63 6174 696f 6e0a 2a20 4974  me location.* It
-00002dd0: 2773 2072 6563 6f6d 6d65 6e64 6564 2074  's recommended t
-00002de0: 6f20 6861 7665 2076 6572 7369 6f6e 735f  o have versions_
-00002df0: 746f 5f6b 6565 703e 3d20 342c 2061 7320  to_keep>= 4, as 
-00002e00: 7468 6973 2077 696c 6c20 6176 6f69 6420  this will avoid 
-00002e10: 746f 2068 6176 6520 7468 6520 6f6c 6465  to have the olde
-00002e20: 7220 6c6f 6361 7469 6f6e 2072 656d 6f76  r location remov
-00002e30: 6564 0a2a 2054 6865 206d 6163 726f 2061  ed.* The macro a
-00002e40: 7468 656e 615f 5f65 6e64 5f6f 665f 7469  thena__end_of_ti
-00002e50: 6d65 206e 6565 6473 2074 6f20 6265 206f  me needs to be o
-00002e60: 7665 7277 7269 7474 656e 2062 7920 7468  verwritten by th
-00002e70: 6520 7573 6572 2069 6620 7573 696e 6720  e user if using 
-00002e80: 4174 6865 6e61 2076 3320 7369 6e63 6520  Athena v3 since 
-00002e90: 6974 2072 6571 7569 7265 7320 6120 7072  it requires a pr
-00002ea0: 6563 6973 696f 6e20 7061 7261 6d65 7465  ecision paramete
-00002eb0: 7220 666f 7220 7469 6d65 7374 616d 7073  r for timestamps
-00002ec0: 0a0a 0a23 2323 2053 6e61 7073 686f 7473  ...### Snapshots
-00002ed0: 0a0a 5468 6520 6164 6170 7465 7220 7375  ..The adapter su
-00002ee0: 7070 6f72 7473 2073 6e61 7073 686f 7420  pports snapshot 
-00002ef0: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
-00002f00: 2049 7420 7375 7070 6f72 7473 2062 6f74   It supports bot
-00002f10: 6820 7469 6d65 7374 616d 7020 616e 6420  h timestamp and 
-00002f20: 6368 6563 6b20 7374 7261 7465 6779 2e20  check strategy. 
-00002f30: 546f 2063 7265 6174 6520 6120 736e 6170  To create a snap
-00002f40: 7368 6f74 2063 7265 6174 6520 6120 736e  shot create a sn
-00002f50: 6170 7368 6f74 2066 696c 6520 696e 2074  apshot file in t
-00002f60: 6865 2073 6e61 7073 686f 7473 2064 6972  he snapshots dir
-00002f70: 6563 746f 7279 2e20 4966 2064 6972 6563  ectory. If direc
-00002f80: 746f 7279 2064 6f65 7320 6e6f 7420 6578  tory does not ex
-00002f90: 6973 7420 6372 6561 7465 206f 6e65 2e0a  ist create one..
-00002fa0: 0a23 2323 2320 5469 6d65 7374 616d 7020  .#### Timestamp 
-00002fb0: 7374 7261 7465 6779 0a0a 546f 2075 7365  strategy..To use
-00002fc0: 2074 6865 2074 696d 6573 7461 6d70 2073   the timestamp s
-00002fd0: 7472 6174 6567 7920 7265 6665 7220 746f  trategy refer to
-00002fe0: 2074 6865 205b 6462 7420 646f 6373 5d28   the [dbt docs](
-00002ff0: 6874 7470 733a 2f2f 646f 6373 2e67 6574  https://docs.get
-00003000: 6462 742e 636f 6d2f 646f 6373 2f62 7569  dbt.com/docs/bui
-00003010: 6c64 2f73 6e61 7073 686f 7473 2374 696d  ld/snapshots#tim
-00003020: 6573 7461 6d70 2d73 7472 6174 6567 792d  estamp-strategy-
-00003030: 7265 636f 6d6d 656e 6465 6429 0a0a 2323  recommended)..##
-00003040: 2323 2043 6865 636b 2073 7472 6174 6567  ## Check strateg
-00003050: 790a 0a54 6f20 7573 6520 7468 6520 6368  y..To use the ch
-00003060: 6563 6b20 7374 7261 7465 6779 2072 6566  eck strategy ref
-00003070: 6572 2074 6f20 7468 6520 5b64 6274 2064  er to the [dbt d
-00003080: 6f63 735d 2868 7474 7073 3a2f 2f64 6f63  ocs](https://doc
-00003090: 732e 6765 7464 6274 2e63 6f6d 2f64 6f63  s.getdbt.com/doc
-000030a0: 732f 6275 696c 642f 736e 6170 7368 6f74  s/build/snapshot
-000030b0: 7323 6368 6563 6b2d 7374 7261 7465 6779  s#check-strategy
-000030c0: 290a 0a23 2323 2320 4861 7264 2d64 656c  )..#### Hard-del
-000030d0: 6574 6573 0a0a 5468 6520 6d61 7465 7269  etes..The materi
-000030e0: 616c 697a 6174 696f 6e20 616c 736f 2073  alization also s
-000030f0: 7570 706f 7274 7320 696e 7661 6c69 6461  upports invalida
-00003100: 7469 6e67 2068 6172 6420 6465 6c65 7465  ting hard delete
-00003110: 732e 2043 6865 636b 2074 6865 205b 646f  s. Check the [do
-00003120: 6373 5d28 6874 7470 733a 2f2f 646f 6373  cs](https://docs
-00003130: 2e67 6574 6462 742e 636f 6d2f 646f 6373  .getdbt.com/docs
-00003140: 2f62 7569 6c64 2f73 6e61 7073 686f 7473  /build/snapshots
-00003150: 2368 6172 642d 6465 6c65 7465 732d 6f70  #hard-deletes-op
-00003160: 742d 696e 2920 746f 2075 6e64 6572 7374  t-in) to underst
-00003170: 616e 6420 7573 6167 652e 0a0a 2323 2320  and usage...### 
-00003180: 576f 726b 696e 6720 6578 616d 706c 650a  Working example.
-00003190: 0a73 6565 6420 6669 6c65 202d 2065 6d70  .seed file - emp
-000031a0: 6c6f 7965 6e74 5f69 6e64 6963 6174 6f72  loyent_indicator
-000031b0: 735f 6e6f 7665 6d62 6572 5f32 3032 325f  s_november_2022_
-000031c0: 6373 765f 7461 626c 6573 2e63 7376 0a60  csv_tables.csv.`
-000031d0: 6060 0a53 6572 6965 735f 7265 6665 7265  ``.Series_refere
-000031e0: 6e63 652c 5065 7269 6f64 2c44 6174 615f  nce,Period,Data_
-000031f0: 7661 6c75 652c 5375 7070 7265 7373 6564  value,Suppressed
-00003200: 0a4d 4549 4d2e 5331 5741 2c31 3939 392e  .MEIM.S1WA,1999.
-00003210: 3034 2c38 3032 3637 2c0a 4d45 494d 2e53  04,80267,.MEIM.S
-00003220: 3157 412c 3139 3939 2e30 352c 3730 3830  1WA,1999.05,7080
-00003230: 332c 0a4d 4549 4d2e 5331 5741 2c31 3939  3,.MEIM.S1WA,199
-00003240: 392e 3036 2c36 3537 3932 2c0a 4d45 494d  9.06,65792,.MEIM
-00003250: 2e53 3157 412c 3139 3939 2e30 372c 3636  .S1WA,1999.07,66
-00003260: 3139 342c 0a4d 4549 4d2e 5331 5741 2c31  194,.MEIM.S1WA,1
-00003270: 3939 392e 3038 2c36 3732 3539 2c0a 4d45  999.08,67259,.ME
-00003280: 494d 2e53 3157 412c 3139 3939 2e30 392c  IM.S1WA,1999.09,
-00003290: 3639 3639 312c 0a4d 4549 4d2e 5331 5741  69691,.MEIM.S1WA
-000032a0: 2c31 3939 392e 312c 3732 3437 352c 0a4d  ,1999.1,72475,.M
-000032b0: 4549 4d2e 5331 5741 2c31 3939 392e 3131  EIM.S1WA,1999.11
-000032c0: 2c37 3932 3633 2c0a 4d45 494d 2e53 3157  ,79263,.MEIM.S1W
-000032d0: 412c 3139 3939 2e31 322c 3836 3534 302c  A,1999.12,86540,
-000032e0: 0a4d 4549 4d2e 5331 5741 2c32 3030 302e  .MEIM.S1WA,2000.
-000032f0: 3031 2c38 3235 3532 2c0a 4d45 494d 2e53  01,82552,.MEIM.S
-00003300: 3157 412c 3230 3030 2e30 322c 3831 3730  1WA,2000.02,8170
-00003310: 392c 0a4d 4549 4d2e 5331 5741 2c32 3030  9,.MEIM.S1WA,200
-00003320: 302e 3033 2c38 3431 3236 2c0a 4d45 494d  0.03,84126,.MEIM
-00003330: 2e53 3157 412c 3230 3030 2e30 342c 3737  .S1WA,2000.04,77
-00003340: 3038 392c 0a4d 4549 4d2e 5331 5741 2c32  089,.MEIM.S1WA,2
-00003350: 3030 302e 3035 2c37 3338 3131 2c0a 4d45  000.05,73811,.ME
-00003360: 494d 2e53 3157 412c 3230 3030 2e30 362c  IM.S1WA,2000.06,
-00003370: 3730 3037 302c 0a4d 4549 4d2e 5331 5741  70070,.MEIM.S1WA
-00003380: 2c32 3030 302e 3037 2c36 3938 3733 2c0a  ,2000.07,69873,.
-00003390: 4d45 494d 2e53 3157 412c 3230 3030 2e30  MEIM.S1WA,2000.0
-000033a0: 382c 3731 3436 382c 0a4d 4549 4d2e 5331  8,71468,.MEIM.S1
-000033b0: 5741 2c32 3030 302e 3039 2c37 3234 3632  WA,2000.09,72462
-000033c0: 2c0a 4d45 494d 2e53 3157 412c 3230 3030  ,.MEIM.S1WA,2000
-000033d0: 2e31 2c37 3438 3937 2c0a 6060 600a 0a6d  .1,74897,.```..m
-000033e0: 6f64 656c 2e73 716c 0a60 6060 0a7b 7b20  odel.sql.```.{{ 
-000033f0: 636f 6e66 6967 280a 2020 2020 6d61 7465  config(.    mate
-00003400: 7269 616c 697a 6564 3d27 7461 626c 6527  rialized='table'
-00003410: 0a29 207d 7d0a 0a0a 5345 4c45 4354 0a20  .) }}...SELECT. 
-00003420: 2020 2052 4f57 5f4e 554d 4245 5228 2920     ROW_NUMBER() 
-00003430: 4f56 4552 2028 2920 4153 2069 640a 2020  OVER () AS id.  
-00003440: 2020 2c20 2a0a 2020 2020 2c20 6361 7374    , *.    , cast
-00003450: 2866 726f 6d5f 756e 6978 7469 6d65 2874  (from_unixtime(t
-00003460: 6f5f 756e 6978 7469 6d65 286e 6f77 2829  o_unixtime(now()
-00003470: 2929 2061 7320 7469 6d65 7374 616d 7028  )) as timestamp(
-00003480: 3629 2920 4153 2072 6566 7265 7368 5f74  6)) AS refresh_t
-00003490: 696d 6573 7461 6d70 0a46 524f 4d20 7b7b  imestamp.FROM {{
-000034a0: 2072 6566 2827 656d 706c 6f79 6d65 6e74   ref('employment
-000034b0: 5f69 6e64 6963 6174 6f72 735f 6e6f 7665  _indicators_nove
-000034c0: 6d62 6572 5f32 3032 325f 6373 765f 7461  mber_2022_csv_ta
-000034d0: 626c 6573 2729 207d 7d0a 6060 600a 0a74  bles') }}.```..t
-000034e0: 696d 6573 7461 6d70 2073 7472 6174 6567  imestamp strateg
-000034f0: 7920 2d20 6d6f 6465 6c5f 736e 6170 7368  y - model_snapsh
-00003500: 6f74 5f31 0a0a 6060 600a 7b25 2073 6e61  ot_1..```.{% sna
-00003510: 7073 686f 7420 6d6f 6465 6c5f 736e 6170  pshot model_snap
-00003520: 7368 6f74 5f31 2025 7d0a 0a7b 7b0a 2020  shot_1 %}..{{.  
-00003530: 2020 636f 6e66 6967 280a 2020 2020 2020    config(.      
-00003540: 7374 7261 7465 6779 3d27 7469 6d65 7374  strategy='timest
-00003550: 616d 7027 2c0a 2020 2020 2020 7570 6461  amp',.      upda
-00003560: 7465 645f 6174 3d27 7265 6672 6573 685f  ted_at='refresh_
-00003570: 7469 6d65 7374 616d 7027 2c0a 2020 2020  timestamp',.    
-00003580: 2020 756e 6971 7565 5f6b 6579 3d27 6964    unique_key='id
-00003590: 270a 2020 2020 290a 7d7d 0a0a 0a0a 5345  '.    ).}}....SE
-000035a0: 4c45 4354 202a 0a0a 6672 6f6d 207b 7b20  LECT *..from {{ 
-000035b0: 7265 6628 276d 6f64 656c 2729 207d 7d0a  ref('model') }}.
-000035c0: 0a7b 2520 656e 6473 6e61 7073 686f 7420  .{% endsnapshot 
-000035d0: 257d 0a60 6060 0a0a 696e 7661 6c69 6461  %}.```..invalida
-000035e0: 7465 2068 6172 6420 6465 6c65 7465 7320  te hard deletes 
-000035f0: 2d20 6d6f 6465 6c5f 736e 6170 7368 6f74  - model_snapshot
-00003600: 5f32 0a60 6060 0a7b 2520 736e 6170 7368  _2.```.{% snapsh
-00003610: 6f74 206d 6f64 656c 5f73 6e61 7073 686f  ot model_snapsho
-00003620: 745f 3220 257d 0a0a 7b7b 0a20 2020 2063  t_2 %}..{{.    c
-00003630: 6f6e 6669 670a 2020 2020 280a 2020 2020  onfig.    (.    
-00003640: 2020 2020 756e 6971 7565 5f6b 6579 3d27      unique_key='
-00003650: 6964 272c 0a20 2020 2020 2020 2073 7472  id',.        str
-00003660: 6174 6567 793d 2774 696d 6573 7461 6d70  ategy='timestamp
-00003670: 272c 0a20 2020 2020 2020 2075 7064 6174  ',.        updat
-00003680: 6564 5f61 743d 2772 6566 7265 7368 5f74  ed_at='refresh_t
-00003690: 696d 6573 7461 6d70 272c 0a20 2020 2020  imestamp',.     
-000036a0: 2020 2069 6e76 616c 6964 6174 655f 6861     invalidate_ha
-000036b0: 7264 5f64 656c 6574 6573 3d54 7275 652c  rd_deletes=True,
-000036c0: 0a20 2020 2029 0a7d 7d0a 5345 4c45 4354  .    ).}}.SELECT
-000036d0: 202a 2066 726f 6d20 7b7b 2072 6566 2827   * from {{ ref('
-000036e0: 6d6f 6465 6c27 2920 7d7d 0a0a 7b25 2065  model') }}..{% e
-000036f0: 6e64 736e 6170 7368 6f74 2025 7d0a 6060  ndsnapshot %}.``
-00003700: 600a 0a63 6865 636b 2073 7472 6174 6567  `..check strateg
-00003710: 7920 2d20 6d6f 6465 6c5f 736e 6170 7368  y - model_snapsh
-00003720: 6f74 5f33 0a60 6060 0a7b 2520 736e 6170  ot_3.```.{% snap
-00003730: 7368 6f74 206d 6f64 656c 5f73 6e61 7073  shot model_snaps
-00003740: 686f 745f 3320 257d 0a0a 7b7b 0a20 2020  hot_3 %}..{{.   
-00003750: 2063 6f6e 6669 670a 2020 2020 280a 2020   config.    (.  
-00003760: 2020 2020 2020 756e 6971 7565 5f6b 6579        unique_key
-00003770: 3d27 6964 272c 0a20 2020 2020 2020 2073  ='id',.        s
-00003780: 7472 6174 6567 793d 2763 6865 636b 272c  trategy='check',
-00003790: 0a20 2020 2020 2020 2063 6865 636b 5f63  .        check_c
-000037a0: 6f6c 733d 5b27 7365 7269 6573 5f72 6566  ols=['series_ref
-000037b0: 6572 656e 6365 272c 2764 6174 615f 7661  erence','data_va
-000037c0: 6c75 6527 5d0a 2020 2020 290a 7d7d 0a53  lue'].    ).}}.S
-000037d0: 454c 4543 5420 2a20 6672 6f6d 207b 7b20  ELECT * from {{ 
-000037e0: 7265 6628 276d 6f64 656c 2729 207d 7d0a  ref('model') }}.
-000037f0: 0a7b 2520 656e 6473 6e61 7073 686f 7420  .{% endsnapshot 
-00003800: 257d 0a60 6060 0a0a 2323 2320 4b6e 6f77  %}.```..### Know
-00003810: 6e20 6973 7375 6573 0a0a 2a20 496e 6372  n issues..* Incr
-00003820: 656d 656e 7461 6c20 4963 6562 6572 6720  emental Iceberg 
-00003830: 6d6f 6465 6c73 202d 2053 796e 6320 616c  models - Sync al
-00003840: 6c20 636f 6c75 6d6e 7320 6f6e 2073 6368  l columns on sch
-00003850: 656d 6120 6368 616e 6765 2063 616e 2774  ema change can't
-00003860: 2072 656d 6f76 6520 636f 6c75 6d6e 7320   remove columns 
-00003870: 7573 6564 2061 7320 7061 7274 6974 696f  used as partitio
-00003880: 6e69 6e67 2e0a 5468 6520 6f6e 6c79 2077  ning..The only w
-00003890: 6179 2c20 6672 6f6d 2061 2064 6274 2070  ay, from a dbt p
-000038a0: 6572 7370 6563 7469 7665 2c20 6973 2074  erspective, is t
-000038b0: 6f20 646f 2061 2066 756c 6c2d 7265 6672  o do a full-refr
-000038c0: 6573 6820 6f66 2074 6865 2069 6e63 7265  esh of the incre
-000038d0: 6d65 6e74 616c 206d 6f64 656c 2e0a 0a2a  mental model...*
-000038e0: 2054 6162 6c65 732c 2073 6368 656d 6173   Tables, schemas
-000038f0: 2061 6e64 2064 6174 6162 6173 6520 7368   and database sh
-00003900: 6f75 6c64 206f 6e6c 7920 6265 206c 6f77  ould only be low
-00003910: 6572 6361 7365 0a0a 2a20 496e 206f 7264  ercase..* In ord
-00003920: 6572 2074 6f20 6176 6f69 6420 706f 7465  er to avoid pote
-00003930: 6e74 6961 6c20 636f 6e66 6c69 6374 732c  ntial conflicts,
-00003940: 206d 616b 6520 7375 7265 205b 6064 6274   make sure [`dbt
-00003950: 2d61 7468 656e 612d 6164 6170 7465 7260  -athena-adapter`
-00003960: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003970: 2e63 6f6d 2f54 6f6d 6d65 2f64 6274 2d61  .com/Tomme/dbt-a
-00003980: 7468 656e 6129 2069 7320 6e6f 7420 696e  thena) is not in
-00003990: 7374 616c 6c65 6420 696e 2074 6865 2074  stalled in the t
-000039a0: 6172 6765 7420 656e 7669 726f 6e6d 656e  arget environmen
-000039b0: 742e 0a20 2053 6565 2068 7474 7073 3a2f  t..  See https:/
-000039c0: 2f67 6974 6875 622e 636f 6d2f 6462 742d  /github.com/dbt-
-000039d0: 6174 6865 6e61 2f64 6274 2d61 7468 656e  athena/dbt-athen
-000039e0: 612f 6973 7375 6573 2f31 3033 2066 6f72  a/issues/103 for
-000039f0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-00003a00: 2a20 536e 6170 7368 6f74 2064 6f65 7320  * Snapshot does 
-00003a10: 6e6f 7420 7375 7070 6f72 7420 6472 6f70  not support drop
-00003a20: 7069 6e67 2063 6f6c 756d 6e73 2066 726f  ping columns fro
-00003a30: 6d20 7468 6520 736f 7572 6365 2074 6162  m the source tab
-00003a40: 6c65 2e20 4966 2079 6f75 2064 726f 7020  le. If you drop 
-00003a50: 6120 636f 6c75 6d6e 206d 616b 6520 7375  a column make su
-00003a60: 7265 2074 6f20 6472 6f70 2074 6865 2063  re to drop the c
-00003a70: 6f6c 756d 6e20 6672 6f6d 2074 6865 2073  olumn from the s
-00003a80: 6e61 7073 686f 7420 6173 2077 656c 6c2e  napshot as well.
-00003a90: 2041 6e6f 7468 6572 2077 6f72 6b61 726f   Another workaro
-00003aa0: 756e 6420 6973 2074 6f20 4e55 4c4c 2074  und is to NULL t
-00003ab0: 6865 2063 6f6c 756d 6e20 696e 2074 6865  he column in the
-00003ac0: 2073 6e61 7073 686f 7420 6465 6669 6e69   snapshot defini
-00003ad0: 7469 6f6e 2074 6f20 7072 6573 6572 7665  tion to preserve
-00003ae0: 2068 6973 746f 7279 0a0a 2323 2320 436f   history..### Co
-00003af0: 6e74 7269 6275 7469 6e67 0a0a 5468 6973  ntributing..This
-00003b00: 2063 6f6e 6e65 6374 6f72 2077 6f72 6b73   connector works
-00003b10: 2077 6974 6820 5079 7468 6f6e 2066 726f   with Python fro
-00003b20: 6d20 332e 3720 746f 2033 2e31 312e 0a0a  m 3.7 to 3.11...
-00003b30: 2323 2323 2047 6574 7469 6e67 2073 7461  #### Getting sta
-00003b40: 7274 6564 0a0a 496e 206f 7264 6572 2074  rted..In order t
-00003b50: 6f20 7374 6172 7420 6465 7665 6c6f 7069  o start developi
-00003b60: 6e67 206f 6e20 7468 6973 2061 6461 7074  ng on this adapt
-00003b70: 6572 2063 6c6f 6e65 2074 6865 2072 6570  er clone the rep
-00003b80: 6f20 616e 6420 7275 6e20 7468 6973 206d  o and run this m
-00003b90: 616b 6520 636f 6d6d 616e 6420 2873 6565  ake command (see
-00003ba0: 205b 4d61 6b65 6669 6c65 5d28 4d61 6b65   [Makefile](Make
-00003bb0: 6669 6c65 2929 203a 0a0a 6060 6062 6173  file)) :..```bas
-00003bc0: 680a 6d61 6b65 2073 6574 7570 0a60 6060  h.make setup.```
-00003bd0: 0a0a 4974 2077 696c 6c20 3a0a 312e 2049  ..It will :.1. I
-00003be0: 6e73 7461 6c6c 2061 6c6c 2064 6570 656e  nstall all depen
-00003bf0: 6465 6e63 6965 732e 0a32 2e20 496e 7374  dencies..2. Inst
-00003c00: 616c 6c20 7072 652d 636f 6d6d 6974 2068  all pre-commit h
-00003c10: 6f6f 6b73 2e0a 332e 2047 656e 6572 6174  ooks..3. Generat
-00003c20: 6520 796f 7572 2060 2e65 6e76 6020 6669  e your `.env` fi
-00003c30: 6c65 0a0a 4e65 7874 2c20 6164 6a75 7374  le..Next, adjust
-00003c40: 2060 2e65 6e76 6020 6669 6c65 2062 7920   `.env` file by 
-00003c50: 636f 6e66 6967 7572 696e 6720 7468 6520  configuring the 
-00003c60: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00003c70: 6162 6c65 7320 746f 206d 6174 6368 2079  ables to match y
-00003c80: 6f75 7220 4174 6865 6e61 2064 6576 656c  our Athena devel
-00003c90: 6f70 6d65 6e74 2065 6e76 6972 6f6e 6d65  opment environme
-00003ca0: 6e74 2e0a 0a23 2323 2320 5275 6e6e 696e  nt...#### Runnin
-00003cb0: 6720 7465 7374 730a 0a57 6520 6861 7665  g tests..We have
-00003cc0: 2032 2064 6966 6665 7265 6e74 2074 7970   2 different typ
-00003cd0: 6573 206f 6620 7465 7374 696e 673a 0a2a  es of testing:.*
-00003ce0: 202a 2a75 6e69 7420 7465 7374 696e 672a   **unit testing*
-00003cf0: 2a3a 2079 6f75 2063 616e 2072 756e 2074  *: you can run t
-00003d00: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
-00003d10: 7320 7275 6e6e 696e 6720 606d 616b 6520  s running `make 
-00003d20: 756e 6974 5f74 6573 7460 0a2a 202a 2a66  unit_test`.* **f
-00003d30: 756e 6374 696f 6e61 6c20 7465 7374 696e  unctional testin
-00003d40: 672a 2a3a 2079 6f75 206d 7573 7420 6861  g**: you must ha
-00003d50: 7665 2061 6e20 4157 5320 6163 636f 756e  ve an AWS accoun
-00003d60: 7420 7769 7468 2041 7468 656e 6120 7365  t with Athena se
-00003d70: 7475 7020 696e 206f 7264 6572 2074 6f20  tup in order to 
-00003d80: 6c61 756e 6368 2074 6869 7320 7479 7065  launch this type
-00003d90: 206f 6620 7465 7374 7320 616e 6420 6861   of tests and ha
-00003da0: 7665 2061 2060 2e65 6e76 6020 6669 6c65  ve a `.env` file
-00003db0: 2069 6e20 706c 6163 6520 7769 7468 2074   in place with t
-00003dc0: 6865 2072 6967 6874 2076 616c 7565 732e  he right values.
-00003dd0: 0a20 2059 6f75 2063 616e 2072 756e 2074  .  You can run t
-00003de0: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
-00003df0: 7320 7275 6e6e 696e 6720 606d 616b 6520  s running `make 
-00003e00: 6675 6e63 7469 6f6e 616c 5f74 6573 7460  functional_test`
-00003e10: 0a0a 0a41 6c6c 2074 7970 6520 6f66 2074  ...All type of t
-00003e20: 6573 7473 2063 616e 2062 6520 7275 6e20  ests can be run 
-00003e30: 7573 696e 6720 606d 616b 6560 3a0a 6060  using `make`:.``
-00003e40: 6062 6173 680a 6d61 6b65 2074 6573 740a  `bash.make test.
-00003e50: 6060 600a 0a23 2323 2320 5075 6c6c 2052  ```..#### Pull R
-00003e60: 6571 7565 7374 0a0a 2a20 4372 6561 7465  equest..* Create
-00003e70: 2061 2063 6f6d 6d69 7420 7769 7468 2079   a commit with y
-00003e80: 6f75 7220 6368 616e 6765 7320 616e 6420  our changes and 
-00003e90: 7075 7368 2074 6865 6d20 746f 2061 0a20  push them to a. 
-00003ea0: 205b 666f 726b 5d28 6874 7470 733a 2f2f   [fork](https://
-00003eb0: 646f 6373 2e67 6974 6875 622e 636f 6d2f  docs.github.com/
-00003ec0: 656e 2f67 6574 2d73 7461 7274 6564 2f71  en/get-started/q
-00003ed0: 7569 636b 7374 6172 742f 666f 726b 2d61  uickstart/fork-a
-00003ee0: 2d72 6570 6f29 2e0a 2a20 4372 6561 7465  -repo)..* Create
-00003ef0: 2061 205b 7075 6c6c 2072 6571 7565 7374   a [pull request
-00003f00: 206f 6e0a 2020 4769 7468 7562 5d28 6874   on.  Github](ht
-00003f10: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
-00003f20: 622e 636f 6d2f 656e 2f67 6974 6875 622f  b.com/en/github/
-00003f30: 636f 6c6c 6162 6f72 6174 696e 672d 7769  collaborating-wi
-00003f40: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
-00003f50: 2f70 726f 706f 7369 6e67 2d63 6861 6e67  /proposing-chang
-00003f60: 6573 2d74 6f2d 796f 7572 2d77 6f72 6b2d  es-to-your-work-
-00003f70: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
-00003f80: 7473 2f63 7265 6174 696e 672d 612d 7075  ts/creating-a-pu
-00003f90: 6c6c 2d72 6571 7565 7374 2d66 726f 6d2d  ll-request-from-
-00003fa0: 612d 666f 726b 292e 0a2a 2050 756c 6c20  a-fork)..* Pull 
-00003fb0: 7265 7175 6573 7420 7469 746c 6520 616e  request title an
-00003fc0: 6420 6d65 7373 6167 6520 2861 6e64 2050  d message (and P
-00003fd0: 5220 7469 746c 6520 616e 6420 6465 7363  R title and desc
-00003fe0: 7269 7074 696f 6e29 206d 7573 7420 6164  ription) must ad
-00003ff0: 6865 7265 2074 6f0a 2020 5b63 6f6e 7665  here to.  [conve
-00004000: 6e74 696f 6e61 6c63 6f6d 6d69 7473 5d28  ntionalcommits](
-00004010: 6874 7470 733a 2f2f 7777 772e 636f 6e76  https://www.conv
-00004020: 656e 7469 6f6e 616c 636f 6d6d 6974 732e  entionalcommits.
-00004030: 6f72 6729 2e0a 2a20 5075 6c6c 2072 6571  org)..* Pull req
-00004040: 7565 7374 2062 6f64 7920 7368 6f75 6c64  uest body should
-00004050: 2064 6573 6372 6962 6520 5f6d 6f74 6976   describe _motiv
-00004060: 6174 696f 6e5f 2e0a 0a23 2323 2048 656c  ation_...### Hel
-00004070: 7066 756c 2052 6573 6f75 7263 6573 0a0a  pful Resources..
-00004080: 2a20 5b41 7468 656e 6120 4352 4541 5445  * [Athena CREATE
-00004090: 2054 4142 4c45 2041 535d 2868 7474 7073   TABLE AS](https
-000040a0: 3a2f 2f64 6f63 732e 6177 732e 616d 617a  ://docs.aws.amaz
-000040b0: 6f6e 2e63 6f6d 2f61 7468 656e 612f 6c61  on.com/athena/la
-000040c0: 7465 7374 2f75 672f 6372 6561 7465 2d74  test/ug/create-t
-000040d0: 6162 6c65 2d61 732e 6874 6d6c 290a 2a20  able-as.html).* 
-000040e0: 5b64 6274 2d6c 6162 732f 6462 742d 636f  [dbt-labs/dbt-co
-000040f0: 7265 5d28 6874 7470 733a 2f2f 6769 7468  re](https://gith
-00004100: 7562 2e63 6f6d 2f64 6274 2d6c 6162 732f  ub.com/dbt-labs/
-00004110: 6462 742d 636f 7265 290a 2a20 5b6c 6175  dbt-core).* [lau
-00004120: 6768 696e 676d 616e 3737 3433 2f50 7941  ghingman7743/PyA
-00004130: 7468 656e 615d 2868 7474 7073 3a2f 2f67  thena](https://g
-00004140: 6974 6875 622e 636f 6d2f 6c61 7567 6869  ithub.com/laughi
-00004150: 6e67 6d61 6e37 3734 332f 5079 4174 6865  ngman7743/PyAthe
-00004160: 6e61 290a                                na).
+000013f0: 2020 2020 2020 207c 204f 7074 696f 6e61         | Optiona
+00001400: 6c20 207c 2060 6d79 2d63 7573 746f 6d2d  l  | `my-custom-
+00001410: 776f 726b 6772 6f75 7060 2020 2020 2020  workgroup`      
+00001420: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001430: 7c20 6e75 6d5f 7265 7472 6965 7320 2020  | num_retries   
+00001440: 2020 207c 204e 756d 6265 7220 6f66 2074     | Number of t
+00001450: 696d 6573 2074 6f20 7265 7472 7920 6120  imes to retry a 
+00001460: 6661 696c 696e 6720 7175 6572 7920 2020  failing query   
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 2020 7c20 4f70 7469 6f6e 616c 2020      | Optional  
+000014a0: 7c20 6033 6020 2020 2020 2020 2020 2020  | `3`           
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 207c 0a7c 206c             |.| l
+000014d0: 665f 7461 6773 2020 2020 2020 2020 2020  f_tags          
+000014e0: 7c20 4465 6661 756c 7420 6c66 2074 6167  | Default lf tag
+000014f0: 7320 746f 2061 7070 6c79 2074 6f20 616e  s to apply to an
+00001500: 7920 6461 7461 6261 7365 2063 7265 6174  y database creat
+00001510: 6564 2062 7920 6462 7420 2020 2020 2020  ed by dbt       
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 207c 204f 7074 696f 6e61 6c20 207c 2060   | Optional  | `
+00001540: 7b22 6f72 6967 696e 223a 2022 6462 7422  {"origin": "dbt"
+00001550: 2c20 2274 6561 6d22 3a20 2261 6e61 6c79  , "team": "analy
+00001560: 7469 6373 227d 6020 7c0a 0a2a 2a45 7861  tics"}` |..**Exa
+00001570: 6d70 6c65 2070 726f 6669 6c65 732e 796d  mple profiles.ym
+00001580: 6c20 656e 7472 793a 2a2a 0a60 6060 7961  l entry:**.```ya
+00001590: 6d6c 0a61 7468 656e 613a 0a20 2074 6172  ml.athena:.  tar
+000015a0: 6765 743a 2064 6576 0a20 206f 7574 7075  get: dev.  outpu
+000015b0: 7473 3a0a 2020 2020 6465 763a 0a20 2020  ts:.    dev:.   
+000015c0: 2020 2074 7970 653a 2061 7468 656e 610a     type: athena.
+000015d0: 2020 2020 2020 7333 5f73 7461 6769 6e67        s3_staging
+000015e0: 5f64 6972 3a20 7333 3a2f 2f61 7468 656e  _dir: s3://athen
+000015f0: 612d 7175 6572 792d 7265 7375 6c74 732f  a-query-results/
+00001600: 6462 742f 0a20 2020 2020 2073 335f 6461  dbt/.      s3_da
+00001610: 7461 5f64 6972 3a20 7333 3a2f 2f79 6f75  ta_dir: s3://you
+00001620: 725f 7333 5f62 7563 6b65 742f 6462 742f  r_s3_bucket/dbt/
+00001630: 0a20 2020 2020 2073 335f 6461 7461 5f6e  .      s3_data_n
+00001640: 616d 696e 673a 2073 6368 656d 615f 7461  aming: schema_ta
+00001650: 626c 650a 2020 2020 2020 7265 6769 6f6e  ble.      region
+00001660: 5f6e 616d 653a 2065 752d 7765 7374 2d31  _name: eu-west-1
+00001670: 0a20 2020 2020 2073 6368 656d 613a 2064  .      schema: d
+00001680: 6274 0a20 2020 2020 2064 6174 6162 6173  bt.      databas
+00001690: 653a 2061 7773 6461 7461 6361 7461 6c6f  e: awsdatacatalo
+000016a0: 670a 2020 2020 2020 6177 735f 7072 6f66  g.      aws_prof
+000016b0: 696c 655f 6e61 6d65 3a20 6d79 2d70 726f  ile_name: my-pro
+000016c0: 6669 6c65 0a20 2020 2020 2077 6f72 6b5f  file.      work_
+000016d0: 6772 6f75 703a 206d 792d 776f 726b 6772  group: my-workgr
+000016e0: 6f75 700a 2020 2020 2020 6c66 5f74 6167  oup.      lf_tag
+000016f0: 733a 0a20 2020 2020 2020 206f 7269 6769  s:.        origi
+00001700: 6e3a 2064 6274 0a20 2020 2020 2020 2074  n: dbt.        t
+00001710: 6561 6d3a 2061 6e61 6c79 7469 6373 0a60  eam: analytics.`
+00001720: 6060 0a0a 5f41 6464 6974 696f 6e61 6c20  ``.._Additional 
+00001730: 696e 666f 726d 6174 696f 6e5f 0a2a 2060  information_.* `
+00001740: 7468 7265 6164 7360 2069 7320 7375 7070  threads` is supp
+00001750: 6f72 7465 640a 2a20 6064 6174 6162 6173  orted.* `databas
+00001760: 6560 2061 6e64 2060 6361 7461 6c6f 6760  e` and `catalog`
+00001770: 2063 616e 2062 6520 7573 6564 2069 6e74   can be used int
+00001780: 6572 6368 616e 6765 6162 6c79 0a0a 0a23  erchangeably...#
+00001790: 2320 4d6f 6465 6c73 0a0a 2323 2320 5461  # Models..### Ta
+000017a0: 626c 6520 436f 6e66 6967 7572 6174 696f  ble Configuratio
+000017b0: 6e0a 0a2a 2060 6578 7465 726e 616c 5f6c  n..* `external_l
+000017c0: 6f63 6174 696f 6e60 2028 6064 6566 6175  ocation` (`defau
+000017d0: 6c74 3d6e 6f6e 6560 290a 2020 2a20 4966  lt=none`).  * If
+000017e0: 2073 6574 2c20 7468 6520 6675 6c6c 2053   set, the full S
+000017f0: 3320 7061 7468 2069 6e20 7768 6963 6820  3 path in which 
+00001800: 7468 6520 7461 626c 6520 7769 6c6c 2062  the table will b
+00001810: 6520 7361 7665 642e 2028 446f 6573 206e  e saved. (Does n
+00001820: 6f74 2077 6f72 6b20 7769 7468 2049 6365  ot work with Ice
+00001830: 6265 7267 2074 6162 6c65 292e 0a2a 2060  berg table)..* `
+00001840: 7061 7274 6974 696f 6e65 645f 6279 6020  partitioned_by` 
+00001850: 2860 6465 6661 756c 743d 6e6f 6e65 6029  (`default=none`)
+00001860: 0a20 202a 2041 6e20 6172 7261 7920 6c69  .  * An array li
+00001870: 7374 206f 6620 636f 6c75 6d6e 7320 6279  st of columns by
+00001880: 2077 6869 6368 2074 6865 2074 6162 6c65   which the table
+00001890: 2077 696c 6c20 6265 2070 6172 7469 7469   will be partiti
+000018a0: 6f6e 6564 0a20 202a 204c 696d 6974 6564  oned.  * Limited
+000018b0: 2074 6f20 6372 6561 7469 6f6e 206f 6620   to creation of 
+000018c0: 3130 3020 7061 7274 6974 696f 6e73 2028  100 partitions (
+000018d0: 5f63 7572 7265 6e74 6c79 5f29 0a2a 2060  _currently_).* `
+000018e0: 6275 636b 6574 6564 5f62 7960 2028 6064  bucketed_by` (`d
+000018f0: 6566 6175 6c74 3d6e 6f6e 6560 290a 2020  efault=none`).  
+00001900: 2a20 416e 2061 7272 6179 206c 6973 7420  * An array list 
+00001910: 6f66 2063 6f6c 756d 6e73 2074 6f20 6275  of columns to bu
+00001920: 636b 6574 2064 6174 612c 2069 676e 6f72  cket data, ignor
+00001930: 6564 2069 6620 7573 696e 6720 4963 6562  ed if using Iceb
+00001940: 6572 670a 2a20 6062 7563 6b65 745f 636f  erg.* `bucket_co
+00001950: 756e 7460 2028 6064 6566 6175 6c74 3d6e  unt` (`default=n
+00001960: 6f6e 6560 290a 2020 2a20 5468 6520 6e75  one`).  * The nu
+00001970: 6d62 6572 206f 6620 6275 636b 6574 7320  mber of buckets 
+00001980: 666f 7220 6275 636b 6574 696e 6720 796f  for bucketing yo
+00001990: 7572 2064 6174 612c 2069 676e 6f72 6564  ur data, ignored
+000019a0: 2069 6620 7573 696e 6720 4963 6562 6572   if using Iceber
+000019b0: 670a 2a20 6074 6162 6c65 5f74 7970 6560  g.* `table_type`
+000019c0: 2028 6064 6566 6175 6c74 3d27 6869 7665   (`default='hive
+000019d0: 2760 290a 2020 2a20 5468 6520 7479 7065  '`).  * The type
+000019e0: 206f 6620 7461 626c 650a 2020 2a20 5375   of table.  * Su
+000019f0: 7070 6f72 7473 2060 6869 7665 6020 6f72  pports `hive` or
+00001a00: 2060 6963 6562 6572 6760 0a2a 2060 666f   `iceberg`.* `fo
+00001a10: 726d 6174 6020 2860 6465 6661 756c 743d  rmat` (`default=
+00001a20: 2770 6172 7175 6574 2760 290a 2020 2a20  'parquet'`).  * 
+00001a30: 5468 6520 6461 7461 2066 6f72 6d61 7420  The data format 
+00001a40: 666f 7220 7468 6520 7461 626c 650a 2020  for the table.  
+00001a50: 2a20 5375 7070 6f72 7473 2060 4f52 4360  * Supports `ORC`
+00001a60: 2c20 6050 4152 5155 4554 602c 2060 4156  , `PARQUET`, `AV
+00001a70: 524f 602c 2060 4a53 4f4e 602c 2060 5445  RO`, `JSON`, `TE
+00001a80: 5854 4649 4c45 600a 2a20 6077 7269 7465  XTFILE`.* `write
+00001a90: 5f63 6f6d 7072 6573 7369 6f6e 6020 2860  _compression` (`
+00001aa0: 6465 6661 756c 743d 6e6f 6e65 6029 0a20  default=none`). 
+00001ab0: 202a 2054 6865 2063 6f6d 7072 6573 7369   * The compressi
+00001ac0: 6f6e 2074 7970 6520 746f 2075 7365 2066  on type to use f
+00001ad0: 6f72 2061 6e79 2073 746f 7261 6765 2066  or any storage f
+00001ae0: 6f72 6d61 7420 7468 6174 2061 6c6c 6f77  ormat that allow
+00001af0: 7320 636f 6d70 7265 7373 696f 6e20 746f  s compression to
+00001b00: 2062 6520 7370 6563 6966 6965 642e 2054   be specified. T
+00001b10: 6f20 7365 6520 7768 6963 6820 6f70 7469  o see which opti
+00001b20: 6f6e 7320 6172 6520 6176 6169 6c61 626c  ons are availabl
+00001b30: 652c 2063 6865 636b 206f 7574 205b 4352  e, check out [CR
+00001b40: 4541 5445 2054 4142 4c45 2041 535d 5b63  EATE TABLE AS][c
+00001b50: 7265 6174 652d 7461 626c 652d 6173 5d0a  reate-table-as].
+00001b60: 2a20 6066 6965 6c64 5f64 656c 696d 6974  * `field_delimit
+00001b70: 6572 6020 2860 6465 6661 756c 743d 6e6f  er` (`default=no
+00001b80: 6e65 6029 0a20 202a 2043 7573 746f 6d20  ne`).  * Custom 
+00001b90: 6669 656c 6420 6465 6c69 6d69 7465 722c  field delimiter,
+00001ba0: 2066 6f72 2077 6865 6e20 666f 726d 6174   for when format
+00001bb0: 2069 7320 7365 7420 746f 2060 5445 5854   is set to `TEXT
+00001bc0: 4649 4c45 600a 2a20 6074 6162 6c65 5f70  FILE`.* `table_p
+00001bd0: 726f 7065 7274 6965 7360 3a20 7461 626c  roperties`: tabl
+00001be0: 6520 7072 6f70 6572 7469 6573 2074 6f20  e properties to 
+00001bf0: 6164 6420 746f 2074 6865 2074 6162 6c65  add to the table
+00001c00: 2c20 7661 6c69 6420 666f 7220 4963 6562  , valid for Iceb
+00001c10: 6572 6720 6f6e 6c79 0a2a 2060 6c66 5f74  erg only.* `lf_t
+00001c20: 6167 7360 2028 6064 6566 6175 6c74 3d6e  ags` (`default=n
+00001c30: 6f6e 6560 290a 2020 2a20 6c66 2074 6167  one`).  * lf tag
+00001c40: 7320 746f 2061 7373 6f63 6961 7465 2077  s to associate w
+00001c50: 6974 6820 7468 6520 7461 626c 650a 2020  ith the table.  
+00001c60: 2a20 666f 726d 6174 3a20 607b 2274 6167  * format: `{"tag
+00001c70: 3122 3a20 2276 616c 7565 3122 2c20 2274  1": "value1", "t
+00001c80: 6167 3222 3a20 2276 616c 7565 3222 7d60  ag2": "value2"}`
+00001c90: 0a2a 2060 6c66 5f74 6167 735f 636f 6c75  .* `lf_tags_colu
+00001ca0: 6d6e 7360 2028 6064 6566 6175 6c74 3d6e  mns` (`default=n
+00001cb0: 6f6e 6560 290a 2020 2a20 6c66 2074 6167  one`).  * lf tag
+00001cc0: 7320 746f 2061 7373 6f63 6961 7465 2077  s to associate w
+00001cd0: 6974 6820 7468 6520 7461 626c 6520 636f  ith the table co
+00001ce0: 6c75 6d6e 730a 2020 2a20 666f 726d 6174  lumns.  * format
+00001cf0: 3a20 607b 2274 6167 3122 3a20 7b22 7661  : `{"tag1": {"va
+00001d00: 6c75 6531 223a 205b 2263 6f6c 756d 6e31  lue1": ["column1
+00001d10: 223a 2022 636f 6c75 6d6e 3222 5d7d 7d60  ": "column2"]}}`
+00001d20: 0a0a 2323 2320 5461 626c 6520 6c6f 6361  ..### Table loca
+00001d30: 7469 6f6e 0a0a 5468 6520 6c6f 6361 7469  tion..The locati
+00001d40: 6f6e 2069 6e20 7768 6963 6820 6120 7461  on in which a ta
+00001d50: 626c 6520 6973 2073 6176 6564 2069 7320  ble is saved is 
+00001d60: 6465 7465 726d 696e 6564 2062 793a 0a0a  determined by:..
+00001d70: 312e 2049 6620 6065 7874 6572 6e61 6c5f  1. If `external_
+00001d80: 6c6f 6361 7469 6f6e 6020 6973 2064 6566  location` is def
+00001d90: 696e 6564 2c20 7468 6174 2076 616c 7565  ined, that value
+00001da0: 2069 7320 7573 6564 2e0a 322e 2049 6620   is used..2. If 
+00001db0: 6073 335f 6461 7461 5f64 6972 6020 6973  `s3_data_dir` is
+00001dc0: 2064 6566 696e 6564 2c20 7468 6520 7061   defined, the pa
+00001dd0: 7468 2069 7320 6465 7465 726d 696e 6564  th is determined
+00001de0: 2062 7920 7468 6174 2061 6e64 2060 7333   by that and `s3
+00001df0: 5f64 6174 615f 6e61 6d69 6e67 600a 332e  _data_naming`.3.
+00001e00: 2049 6620 6073 335f 6461 7461 5f64 6972   If `s3_data_dir
+00001e10: 6020 6973 206e 6f74 2064 6566 696e 6564  ` is not defined
+00001e20: 2064 6174 6120 6973 2073 746f 7265 6420   data is stored 
+00001e30: 756e 6465 7220 6073 335f 7374 6167 696e  under `s3_stagin
+00001e40: 675f 6469 722f 7461 626c 6573 2f60 0a0a  g_dir/tables/`..
+00001e50: 4865 7265 2061 6c6c 2074 6865 206f 7074  Here all the opt
+00001e60: 696f 6e73 2061 7661 696c 6162 6c65 2066  ions available f
+00001e70: 6f72 2060 7333 5f64 6174 615f 6e61 6d69  or `s3_data_nami
+00001e80: 6e67 603a 0a2a 2060 7575 6964 603a 2060  ng`:.* `uuid`: `
+00001e90: 7b73 335f 6461 7461 5f64 6972 7d2f 7b75  {s3_data_dir}/{u
+00001ea0: 7569 6434 2829 7d2f 600a 2a20 6074 6162  uid4()}/`.* `tab
+00001eb0: 6c65 5f74 6162 6c65 603a 2060 7b73 335f  le_table`: `{s3_
+00001ec0: 6461 7461 5f64 6972 7d2f 7b74 6162 6c65  data_dir}/{table
+00001ed0: 7d2f 600a 2a20 6074 6162 6c65 5f75 6e69  }/`.* `table_uni
+00001ee0: 7175 6560 3a20 607b 7333 5f64 6174 615f  que`: `{s3_data_
+00001ef0: 6469 727d 2f7b 7461 626c 657d 2f7b 7575  dir}/{table}/{uu
+00001f00: 6964 3428 297d 2f60 0a2a 2060 7363 6865  id4()}/`.* `sche
+00001f10: 6d61 5f74 6162 6c65 603a 2060 7b73 335f  ma_table`: `{s3_
+00001f20: 6461 7461 5f64 6972 7d2f 7b73 6368 656d  data_dir}/{schem
+00001f30: 617d 2f7b 7461 626c 657d 2f60 0a2a 2060  a}/{table}/`.* `
+00001f40: 7333 5f64 6174 615f 6e61 6d69 6e67 3d73  s3_data_naming=s
+00001f50: 6368 656d 615f 7461 626c 655f 756e 6971  chema_table_uniq
+00001f60: 7565 603a 2060 7b73 335f 6461 7461 5f64  ue`: `{s3_data_d
+00001f70: 6972 7d2f 7b73 6368 656d 617d 2f7b 7461  ir}/{schema}/{ta
+00001f80: 626c 657d 2f7b 7575 6964 3428 297d 2f60  ble}/{uuid4()}/`
+00001f90: 0a0a 4974 2773 2070 6f73 7369 626c 6520  ..It's possible 
+00001fa0: 746f 2073 6574 2074 6865 2060 7333 5f64  to set the `s3_d
+00001fb0: 6174 615f 6e61 6d69 6e67 6020 676c 6f62  ata_naming` glob
+00001fc0: 616c 6c79 2069 6e20 7468 6520 7461 7267  ally in the targ
+00001fd0: 6574 2070 726f 6669 6c65 2c20 6f72 206f  et profile, or o
+00001fe0: 7665 7277 7269 7465 2074 6865 2076 616c  verwrite the val
+00001ff0: 7565 2069 6e20 7468 6520 7461 626c 6520  ue in the table 
+00002000: 636f 6e66 6967 2c0a 6f72 2073 6574 7469  config,.or setti
+00002010: 6e67 2075 7020 7468 6520 7661 6c75 6520  ng up the value 
+00002020: 666f 7220 6772 6f75 7073 206f 6620 6d6f  for groups of mo
+00002030: 6465 6c20 696e 2064 6274 5f70 726f 6a65  del in dbt_proje
+00002040: 6374 2e79 6d6c 2e0a 0a3e 204e 6f74 653a  ct.yml...> Note:
+00002050: 2077 6865 6e20 7573 696e 6720 6120 776f   when using a wo
+00002060: 726b 2067 726f 7570 2077 6974 6820 6120  rk group with a 
+00002070: 6465 6661 756c 7420 6f75 7470 7574 206c  default output l
+00002080: 6f63 6174 696f 6e20 636f 6e66 6967 7572  ocation configur
+00002090: 6564 2c20 6073 335f 6461 7461 5f6e 616d  ed, `s3_data_nam
+000020a0: 696e 6760 2061 6e64 2061 6e79 2063 6f6e  ing` and any con
+000020b0: 6669 6775 7265 6420 6275 636b 6574 7320  figured buckets 
+000020c0: 6172 6520 6967 6e6f 7265 6420 616e 6420  are ignored and 
+000020d0: 7468 6520 6c6f 6361 7469 6f6e 2063 6f6e  the location con
+000020e0: 6669 6775 7265 6420 696e 2074 6865 2077  figured in the w
+000020f0: 6f72 6b20 6772 6f75 7020 6973 2075 7365  ork group is use
+00002100: 642e 0a0a 2323 2320 496e 6372 656d 656e  d...### Incremen
+00002110: 7461 6c20 6d6f 6465 6c73 0a0a 5375 7070  tal models..Supp
+00002120: 6f72 7420 666f 7220 5b69 6e63 7265 6d65  ort for [increme
+00002130: 6e74 616c 206d 6f64 656c 735d 2868 7474  ntal models](htt
+00002140: 7073 3a2f 2f64 6f63 732e 6765 7464 6274  ps://docs.getdbt
+00002150: 2e63 6f6d 2f64 6f63 732f 6275 696c 642f  .com/docs/build/
+00002160: 696e 6372 656d 656e 7461 6c2d 6d6f 6465  incremental-mode
+00002170: 6c73 292e 0a0a 5468 6573 6520 7374 7261  ls)...These stra
+00002180: 7465 6769 6573 2061 7265 2073 7570 706f  tegies are suppo
+00002190: 7274 6564 3a0a 0a2a 2060 696e 7365 7274  rted:..* `insert
+000021a0: 5f6f 7665 7277 7269 7465 6020 2864 6566  _overwrite` (def
+000021b0: 6175 6c74 293a 2054 6865 2069 6e73 6572  ault): The inser
+000021c0: 7420 6f76 6572 7772 6974 6520 7374 7261  t overwrite stra
+000021d0: 7465 6779 2064 656c 6574 6573 2074 6865  tegy deletes the
+000021e0: 206f 7665 726c 6170 7069 6e67 2070 6172   overlapping par
+000021f0: 7469 7469 6f6e 7320 6672 6f6d 2074 6865  titions from the
+00002200: 2064 6573 7469 6e61 7469 6f6e 0a74 6162   destination.tab
+00002210: 6c65 2c20 616e 6420 7468 656e 2069 6e73  le, and then ins
+00002220: 6572 7473 2074 6865 206e 6577 2072 6563  erts the new rec
+00002230: 6f72 6473 2066 726f 6d20 7468 6520 736f  ords from the so
+00002240: 7572 6365 2e20 5468 6973 2073 7472 6174  urce. This strat
+00002250: 6567 7920 6465 7065 6e64 7320 6f6e 2074  egy depends on t
+00002260: 6865 2060 7061 7274 6974 696f 6e65 645f  he `partitioned_
+00002270: 6279 6020 6b65 7977 6f72 6421 2049 6620  by` keyword! If 
+00002280: 6e6f 0a70 6172 7469 7469 6f6e 7320 6172  no.partitions ar
+00002290: 6520 6465 6669 6e65 642c 2064 6274 2077  e defined, dbt w
+000022a0: 696c 6c20 6661 6c6c 2062 6163 6b20 746f  ill fall back to
+000022b0: 2074 6865 2060 6170 7065 6e64 6020 7374   the `append` st
+000022c0: 7261 7465 6779 2e0a 2a20 6061 7070 656e  rategy..* `appen
+000022d0: 6460 3a20 496e 7365 7274 206e 6577 2072  d`: Insert new r
+000022e0: 6563 6f72 6473 2077 6974 686f 7574 2075  ecords without u
+000022f0: 7064 6174 696e 672c 2064 656c 6574 696e  pdating, deletin
+00002300: 6720 6f72 206f 7665 7277 7269 7469 6e67  g or overwriting
+00002310: 2061 6e79 2065 7869 7374 696e 6720 6461   any existing da
+00002320: 7461 2e20 5468 6572 6520 6d69 6768 7420  ta. There might 
+00002330: 6265 2064 7570 6c69 6361 7465 0a64 6174  be duplicate.dat
+00002340: 6120 2865 2e67 2e20 6772 6561 7420 666f  a (e.g. great fo
+00002350: 7220 6c6f 6720 6f72 2068 6973 746f 7269  r log or histori
+00002360: 6361 6c20 6461 7461 292e 0a2a 2060 6d65  cal data)..* `me
+00002370: 7267 6560 3a20 436f 6e64 6974 696f 6e61  rge`: Conditiona
+00002380: 6c6c 7920 7570 6461 7465 732c 2064 656c  lly updates, del
+00002390: 6574 6573 2c20 6f72 2069 6e73 6572 7473  etes, or inserts
+000023a0: 2072 6f77 7320 696e 746f 2061 6e20 4963   rows into an Ic
+000023b0: 6562 6572 6720 7461 626c 652e 2055 7365  eberg table. Use
+000023c0: 6420 696e 2063 6f6d 6269 6e61 7469 6f6e  d in combination
+000023d0: 2077 6974 6820 6075 6e69 7175 655f 6b65   with `unique_ke
+000023e0: 7960 2e0a 4f6e 6c79 2061 7661 696c 6162  y`..Only availab
+000023f0: 6c65 2077 6865 6e20 7573 696e 6720 4963  le when using Ic
+00002400: 6562 6572 672e 0a0a 2323 2320 4f6e 2073  eberg...### On s
+00002410: 6368 656d 6120 6368 616e 6765 0a0a 606f  chema change..`o
+00002420: 6e5f 7363 6865 6d61 5f63 6861 6e67 6560  n_schema_change`
+00002430: 2069 7320 616e 206f 7074 696f 6e20 746f   is an option to
+00002440: 2072 6566 6c65 6374 2063 6861 6e67 6573   reflect changes
+00002450: 206f 6620 7363 6865 6d61 2069 6e20 696e   of schema in in
+00002460: 6372 656d 656e 7461 6c20 6d6f 6465 6c73  cremental models
+00002470: 2e0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
+00002480: 6f70 7469 6f6e 7320 6172 6520 7375 7070  options are supp
+00002490: 6f72 7465 643a 0a2a 2060 6967 6e6f 7265  orted:.* `ignore
+000024a0: 6020 2864 6566 6175 6c74 290a 2a20 6066  ` (default).* `f
+000024b0: 6169 6c60 0a2a 2060 6170 7065 6e64 5f6e  ail`.* `append_n
+000024c0: 6577 5f63 6f6c 756d 6e73 600a 2a20 6073  ew_columns`.* `s
+000024d0: 796e 635f 616c 6c5f 636f 6c75 6d6e 7360  ync_all_columns`
+000024e0: 0a0a 496e 2064 6574 6169 6c2c 2070 6c65  ..In detail, ple
+000024f0: 6173 6520 7265 6665 7220 746f 205b 6462  ase refer to [db
+00002500: 7420 646f 6373 5d28 6874 7470 733a 2f2f  t docs](https://
+00002510: 646f 6373 2e67 6574 6462 742e 636f 6d2f  docs.getdbt.com/
+00002520: 646f 6373 2f62 7569 6c64 2f69 6e63 7265  docs/build/incre
+00002530: 6d65 6e74 616c 2d6d 6f64 656c 7323 7768  mental-models#wh
+00002540: 6174 2d69 662d 7468 652d 636f 6c75 6d6e  at-if-the-column
+00002550: 732d 6f66 2d6d 792d 696e 6372 656d 656e  s-of-my-incremen
+00002560: 7461 6c2d 6d6f 6465 6c2d 6368 616e 6765  tal-model-change
+00002570: 292e 0a0a 2323 2320 4963 6562 6572 670a  )...### Iceberg.
+00002580: 0a54 6865 2061 6461 7074 6572 2073 7570  .The adapter sup
+00002590: 706f 7274 7320 7461 626c 6520 6d61 7465  ports table mate
+000025a0: 7269 616c 697a 6174 696f 6e20 666f 7220  rialization for 
+000025b0: 4963 6562 6572 672e 0a0a 546f 2067 6574  Iceberg...To get
+000025c0: 2073 7461 7274 6564 206a 7573 7420 6164   started just ad
+000025d0: 6420 7468 6973 2061 7320 796f 7572 206d  d this as your m
+000025e0: 6f64 656c 3a0a 6060 600a 7b7b 2063 6f6e  odel:.```.{{ con
+000025f0: 6669 6728 0a20 2020 206d 6174 6572 6961  fig(.    materia
+00002600: 6c69 7a65 643d 2774 6162 6c65 272c 0a20  lized='table',. 
+00002610: 2020 2074 6162 6c65 5f74 7970 653d 2769     table_type='i
+00002620: 6365 6265 7267 272c 0a20 2020 2066 6f72  ceberg',.    for
+00002630: 6d61 743d 2770 6172 7175 6574 272c 0a20  mat='parquet',. 
+00002640: 2020 2070 6172 7469 7469 6f6e 6564 5f62     partitioned_b
+00002650: 793d 5b27 6275 636b 6574 2875 7365 725f  y=['bucket(user_
+00002660: 6964 2c20 3529 275d 2c0a 2020 2020 7461  id, 5)'],.    ta
+00002670: 626c 655f 7072 6f70 6572 7469 6573 3d7b  ble_properties={
+00002680: 0a20 2020 2009 276f 7074 696d 697a 655f  .    .'optimize_
+00002690: 7265 7772 6974 655f 6465 6c65 7465 5f66  rewrite_delete_f
+000026a0: 696c 655f 7468 7265 7368 6f6c 6427 3a20  ile_threshold': 
+000026b0: 2732 270a 2020 2020 097d 0a29 207d 7d0a  '2'.    .}.) }}.
+000026c0: 0a53 454c 4543 540a 0927 4127 2041 5320  .SELECT..'A' AS 
+000026d0: 7573 6572 5f69 642c 0a09 2770 6927 2041  user_id,..'pi' A
+000026e0: 5320 6e61 6d65 2c0a 0927 6163 7469 7665  S name,..'active
+000026f0: 2720 4153 2073 7461 7475 732c 0a09 3137  ' AS status,..17
+00002700: 2e38 3920 4153 2063 6f73 742c 0a09 3120  .89 AS cost,..1 
+00002710: 4153 2071 7561 6e74 6974 792c 0a09 3130  AS quantity,..10
+00002720: 3030 3030 3030 3020 4153 2071 7561 6e74  0000000 AS quant
+00002730: 6974 795f 6269 672c 0a09 6375 7272 656e  ity_big,..curren
+00002740: 745f 6461 7465 2041 5320 6d79 5f64 6174  t_date AS my_dat
+00002750: 650a 6060 600a 0a49 6365 6265 7267 2073  e.```..Iceberg s
+00002760: 7570 706f 7274 7320 6275 636b 6574 696e  upports bucketin
+00002770: 6720 6173 2068 6964 6465 6e20 7061 7274  g as hidden part
+00002780: 6974 696f 6e73 2c20 7468 6572 6566 6f72  itions, therefor
+00002790: 6520 7573 6520 7468 6520 6070 6172 7469  e use the `parti
+000027a0: 7469 6f6e 6564 5f62 7960 2063 6f6e 6669  tioned_by` confi
+000027b0: 6720 746f 2061 6464 2073 7065 6369 6669  g to add specifi
+000027c0: 6320 6275 636b 6574 696e 6720 636f 6e64  c bucketing cond
+000027d0: 6974 696f 6e73 2e0a 0a49 6365 6265 7267  itions...Iceberg
+000027e0: 2073 7570 706f 7274 7320 7365 7665 7261   supports severa
+000027f0: 6c20 7461 626c 6520 666f 726d 6174 7320  l table formats 
+00002800: 666f 7220 6461 7461 203a 2060 5041 5251  for data : `PARQ
+00002810: 5545 5460 2c20 6041 5652 4f60 2061 6e64  UET`, `AVRO` and
+00002820: 2060 4f52 4360 2e0a 0a49 7420 6973 2070   `ORC`...It is p
+00002830: 6f73 7369 626c 6520 746f 2075 7365 2069  ossible to use i
+00002840: 6365 6265 7267 2069 6e20 616e 2069 6e63  ceberg in an inc
+00002850: 7265 6d65 6e74 616c 2066 6173 6869 6f6e  remental fashion
+00002860: 2c20 7370 6563 6966 6963 616c 6c79 2032  , specifically 2
+00002870: 2073 7472 6174 6567 6965 7320 6172 6520   strategies are 
+00002880: 7375 7070 6f72 7465 643a 0a2a 2060 6170  supported:.* `ap
+00002890: 7065 6e64 603a 206e 6577 2072 6563 6f72  pend`: new recor
+000028a0: 6473 2061 7265 2061 7070 656e 6465 6420  ds are appended 
+000028b0: 746f 2074 6865 2074 6162 6c65 2c20 7468  to the table, th
+000028c0: 6973 2063 616e 206c 6561 6420 746f 2064  is can lead to d
+000028d0: 7570 6c69 6361 7465 730a 2a20 606d 6572  uplicates.* `mer
+000028e0: 6765 603a 206d 7573 7420 6265 2075 7365  ge`: must be use
+000028f0: 6420 696e 2063 6f6d 6269 6e61 7469 6f6e  d in combination
+00002900: 2077 6974 6820 6075 6e69 7175 655f 6b65   with `unique_ke
+00002910: 7960 2061 6e64 2069 7427 7320 6f6e 6c79  y` and it's only
+00002920: 2061 7661 696c 6162 6c65 2077 6974 6820   available with 
+00002930: 456e 6769 6e65 2076 6572 7369 6f6e 2033  Engine version 3
+00002940: 2e0a 2020 2049 7420 7065 7266 6f72 6d73  ..   It performs
+00002950: 2061 6e20 7570 7365 7274 2c20 6e65 7720   an upsert, new 
+00002960: 7265 636f 7264 2061 7265 2061 6464 6564  record are added
+00002970: 2c20 616e 6420 7265 636f 7264 2061 6c72  , and record alr
+00002980: 6561 6479 2065 7869 7374 696e 6720 6172  eady existing ar
+00002990: 6520 7570 6461 7465 640a 0a23 2323 2048  e updated..### H
+000029a0: 6967 6820 6176 6169 6c61 626c 6520 7461  igh available ta
+000029b0: 626c 6520 6d61 7465 7269 616c 697a 6174  ble materializat
+000029c0: 696f 6e0a 5468 6520 6375 7272 656e 7420  ion.The current 
+000029d0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+000029e0: 6620 7468 6520 7461 626c 6520 6d61 7465  f the table mate
+000029f0: 7269 616c 697a 6174 696f 6e20 6361 6e20  rialization can 
+00002a00: 6c65 6164 2074 6f20 646f 776e 7469 6d65  lead to downtime
+00002a10: 2c20 6173 2074 6172 6765 7420 7461 626c  , as target tabl
+00002a20: 6520 6973 2064 726f 7070 6564 2061 6e64  e is dropped and
+00002a30: 2072 652d 6372 6561 7465 642e 0a54 6f20   re-created..To 
+00002a40: 6861 7665 2074 6865 206c 6573 7320 6465  have the less de
+00002a50: 7374 7275 6374 6976 6520 6265 6861 7669  structive behavi
+00002a60: 6f72 2069 7427 7320 706f 7373 6962 6c65  or it's possible
+00002a70: 2074 6f20 7573 6520 6074 6162 6c65 3d27   to use `table='
+00002a80: 7461 626c 655f 6869 7665 5f68 6127 6020  table_hive_ha'` 
+00002a90: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
+00002aa0: 0a2a 2a74 6162 6c65 5f68 6976 655f 6861  .**table_hive_ha
+00002ab0: 2a2a 206c 6576 6572 6167 6520 7468 6520  ** leverage the 
+00002ac0: 7461 626c 6520 7665 7273 696f 6e73 2066  table versions f
+00002ad0: 6561 7475 7265 206f 6620 676c 7565 2063  eature of glue c
+00002ae0: 6174 616c 6f67 2c20 6372 6561 7469 6e67  atalog, creating
+00002af0: 2061 2074 6d70 2074 6162 6c65 2061 6e64   a tmp table and
+00002b00: 2073 7761 7070 696e 670a 7468 6520 7461   swapping.the ta
+00002b10: 7267 6574 2074 6162 6c65 2074 6f20 7468  rget table to th
+00002b20: 6520 6c6f 6361 7469 6f6e 206f 6620 7468  e location of th
+00002b30: 6520 746d 7020 7461 626c 652e 0a54 6869  e tmp table..Thi
+00002b40: 7320 6d61 7465 7269 616c 697a 6174 696f  s materializatio
+00002b50: 6e20 6973 206f 6e6c 7920 6176 6169 6c61  n is only availa
+00002b60: 626c 6520 666f 7220 6074 6162 6c65 5f74  ble for `table_t
+00002b70: 7970 653d 6869 7665 6020 616e 6420 7265  ype=hive` and re
+00002b80: 7175 6972 6573 2075 7369 6e67 2075 6e69  quires using uni
+00002b90: 7175 6520 6c6f 6361 7469 6f6e 732e 0a0a  que locations...
+00002ba0: 6060 600a 7b7b 2063 6f6e 6669 6728 0a20  ```.{{ config(. 
+00002bb0: 2020 206d 6174 6572 6961 6c69 7a65 643d     materialized=
+00002bc0: 2774 6162 6c65 5f68 6976 655f 6861 272c  'table_hive_ha',
+00002bd0: 0a20 2020 2066 6f72 6d61 743d 2770 6172  .    format='par
+00002be0: 7175 6574 272c 0a20 2020 2070 6172 7469  quet',.    parti
+00002bf0: 7469 6f6e 5f62 793d 5b27 7374 6174 7573  tion_by=['status
+00002c00: 275d 2c0a 2020 2020 7333 5f64 6174 615f  '],.    s3_data_
+00002c10: 6e61 6d69 6e67 3d27 7461 626c 655f 756e  naming='table_un
+00002c20: 6971 7565 270a 2920 7d7d 0a0a 7365 6c65  ique'.) }}..sele
+00002c30: 6374 0a20 2027 6127 2061 7320 7573 6572  ct.  'a' as user
+00002c40: 5f69 642c 0a20 2027 7069 2720 6173 2075  _id,.  'pi' as u
+00002c50: 7365 725f 6e61 6d65 2c0a 2020 2761 6374  ser_name,.  'act
+00002c60: 6976 6527 2061 7320 7374 6174 7573 0a75  ive' as status.u
+00002c70: 6e69 6f6e 2061 6c6c 0a73 656c 6563 740a  nion all.select.
+00002c80: 2020 2762 2720 6173 2075 7365 725f 6964    'b' as user_id
+00002c90: 2c0a 2020 2773 6827 2061 7320 7573 6572  ,.  'sh' as user
+00002ca0: 5f6e 616d 652c 0a20 2027 6469 7361 626c  _name,.  'disabl
+00002cb0: 6564 2720 6173 2073 7461 7475 730a 6060  ed' as status.``
+00002cc0: 600a 0a42 7920 6465 6661 756c 742c 2074  `..By default, t
+00002cd0: 6865 206d 6174 6572 6961 6c69 7a61 7469  he materializati
+00002ce0: 6f6e 206b 6565 7073 2074 6865 206c 6173  on keeps the las
+00002cf0: 7420 3420 7461 626c 6520 7665 7273 696f  t 4 table versio
+00002d00: 6e73 2c20 796f 7520 6361 6e20 6368 616e  ns, you can chan
+00002d10: 6765 2069 7420 7468 6174 2073 6574 7469  ge it that setti
+00002d20: 6e67 2060 7665 7273 696f 6e73 5f74 6f5f  ng `versions_to_
+00002d30: 6b65 6570 602e 0a0a 2323 2323 204b 6e6f  keep`...#### Kno
+00002d40: 776e 2069 7373 7565 730a 2a20 5768 656e  wn issues.* When
+00002d50: 2073 7761 7070 696e 6720 6672 6f6d 2061   swapping from a
+00002d60: 2074 6162 6c65 2077 6974 6820 7061 7274   table with part
+00002d70: 6974 696f 6e73 2074 6f20 6120 7461 626c  itions to a tabl
+00002d80: 6520 7769 7468 6f75 7420 2861 6e64 2074  e without (and t
+00002d90: 6865 206f 7468 6572 2077 6179 2061 726f  he other way aro
+00002da0: 756e 6429 2c20 7468 6572 6520 636f 756c  und), there coul
+00002db0: 6420 6265 2061 206c 6974 746c 6520 646f  d be a little do
+00002dc0: 776e 7469 6d65 2e0a 2020 496e 2063 6173  wntime..  In cas
+00002dd0: 6520 6869 6768 2070 6572 666f 726d 616e  e high performan
+00002de0: 6365 7320 6172 6520 6e65 6564 6564 2063  ces are needed c
+00002df0: 6f6e 7369 6465 7220 6275 636b 6574 696e  onsider bucketin
+00002e00: 6720 696e 7374 6561 6420 6f66 2070 6172  g instead of par
+00002e10: 7469 7469 6f6e 730a 2a20 4279 2064 6566  titions.* By def
+00002e20: 6175 6c74 2c20 476c 7565 2022 6475 706c  ault, Glue "dupl
+00002e30: 6963 6174 6522 2074 6865 2076 6572 7369  icate" the versi
+00002e40: 6f6e 7320 696e 7465 726e 616c 6c79 2c20  ons internally, 
+00002e50: 736f 2074 6865 206c 6173 7420 3220 7665  so the last 2 ve
+00002e60: 7273 696f 6e73 206f 6620 6120 7461 626c  rsions of a tabl
+00002e70: 6520 706f 696e 7420 746f 2074 6865 2073  e point to the s
+00002e80: 616d 6520 6c6f 6361 7469 6f6e 0a2a 2049  ame location.* I
+00002e90: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+00002ea0: 746f 2068 6176 6520 7665 7273 696f 6e73  to have versions
+00002eb0: 5f74 6f5f 6b65 6570 3e3d 2034 2c20 6173  _to_keep>= 4, as
+00002ec0: 2074 6869 7320 7769 6c6c 2061 766f 6964   this will avoid
+00002ed0: 2074 6f20 6861 7665 2074 6865 206f 6c64   to have the old
+00002ee0: 6572 206c 6f63 6174 696f 6e20 7265 6d6f  er location remo
+00002ef0: 7665 640a 2a20 5468 6520 6d61 6372 6f20  ved.* The macro 
+00002f00: 6174 6865 6e61 5f5f 656e 645f 6f66 5f74  athena__end_of_t
+00002f10: 696d 6520 6e65 6564 7320 746f 2062 6520  ime needs to be 
+00002f20: 6f76 6572 7772 6974 7465 6e20 6279 2074  overwritten by t
+00002f30: 6865 2075 7365 7220 6966 2075 7369 6e67  he user if using
+00002f40: 2041 7468 656e 6120 7633 2073 696e 6365   Athena v3 since
+00002f50: 2069 7420 7265 7175 6972 6573 2061 2070   it requires a p
+00002f60: 7265 6369 7369 6f6e 2070 6172 616d 6574  recision paramet
+00002f70: 6572 2066 6f72 2074 696d 6573 7461 6d70  er for timestamp
+00002f80: 730a 0a0a 2323 2053 6e61 7073 686f 7473  s...## Snapshots
+00002f90: 0a0a 5468 6520 6164 6170 7465 7220 7375  ..The adapter su
+00002fa0: 7070 6f72 7473 2073 6e61 7073 686f 7420  pports snapshot 
+00002fb0: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
+00002fc0: 2049 7420 7375 7070 6f72 7473 2062 6f74   It supports bot
+00002fd0: 6820 7469 6d65 7374 616d 7020 616e 6420  h timestamp and 
+00002fe0: 6368 6563 6b20 7374 7261 7465 6779 2e20  check strategy. 
+00002ff0: 546f 2063 7265 6174 6520 6120 736e 6170  To create a snap
+00003000: 7368 6f74 2063 7265 6174 6520 6120 736e  shot create a sn
+00003010: 6170 7368 6f74 2066 696c 6520 696e 2074  apshot file in t
+00003020: 6865 2073 6e61 7073 686f 7473 2064 6972  he snapshots dir
+00003030: 6563 746f 7279 2e20 4966 2064 6972 6563  ectory. If direc
+00003040: 746f 7279 2064 6f65 7320 6e6f 7420 6578  tory does not ex
+00003050: 6973 7420 6372 6561 7465 206f 6e65 2e0a  ist create one..
+00003060: 0a23 2323 2054 696d 6573 7461 6d70 2073  .### Timestamp s
+00003070: 7472 6174 6567 790a 0a54 6f20 7573 6520  trategy..To use 
+00003080: 7468 6520 7469 6d65 7374 616d 7020 7374  the timestamp st
+00003090: 7261 7465 6779 2072 6566 6572 2074 6f20  rategy refer to 
+000030a0: 7468 6520 5b64 6274 2064 6f63 735d 2868  the [dbt docs](h
+000030b0: 7474 7073 3a2f 2f64 6f63 732e 6765 7464  ttps://docs.getd
+000030c0: 6274 2e63 6f6d 2f64 6f63 732f 6275 696c  bt.com/docs/buil
+000030d0: 642f 736e 6170 7368 6f74 7323 7469 6d65  d/snapshots#time
+000030e0: 7374 616d 702d 7374 7261 7465 6779 2d72  stamp-strategy-r
+000030f0: 6563 6f6d 6d65 6e64 6564 290a 0a23 2323  ecommended)..###
+00003100: 2043 6865 636b 2073 7472 6174 6567 790a   Check strategy.
+00003110: 0a54 6f20 7573 6520 7468 6520 6368 6563  .To use the chec
+00003120: 6b20 7374 7261 7465 6779 2072 6566 6572  k strategy refer
+00003130: 2074 6f20 7468 6520 5b64 6274 2064 6f63   to the [dbt doc
+00003140: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
+00003150: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+00003160: 6275 696c 642f 736e 6170 7368 6f74 7323  build/snapshots#
+00003170: 6368 6563 6b2d 7374 7261 7465 6779 290a  check-strategy).
+00003180: 0a23 2323 2048 6172 642d 6465 6c65 7465  .### Hard-delete
+00003190: 730a 0a54 6865 206d 6174 6572 6961 6c69  s..The materiali
+000031a0: 7a61 7469 6f6e 2061 6c73 6f20 7375 7070  zation also supp
+000031b0: 6f72 7473 2069 6e76 616c 6964 6174 696e  orts invalidatin
+000031c0: 6720 6861 7264 2064 656c 6574 6573 2e20  g hard deletes. 
+000031d0: 4368 6563 6b20 7468 6520 5b64 6f63 735d  Check the [docs]
+000031e0: 2868 7474 7073 3a2f 2f64 6f63 732e 6765  (https://docs.ge
+000031f0: 7464 6274 2e63 6f6d 2f64 6f63 732f 6275  tdbt.com/docs/bu
+00003200: 696c 642f 736e 6170 7368 6f74 7323 6861  ild/snapshots#ha
+00003210: 7264 2d64 656c 6574 6573 2d6f 7074 2d69  rd-deletes-opt-i
+00003220: 6e29 2074 6f20 756e 6465 7273 7461 6e64  n) to understand
+00003230: 2075 7361 6765 2e0a 0a23 2323 2057 6f72   usage...### Wor
+00003240: 6b69 6e67 2065 7861 6d70 6c65 0a0a 7365  king example..se
+00003250: 6564 2066 696c 6520 2d20 656d 706c 6f79  ed file - employ
+00003260: 656e 745f 696e 6469 6361 746f 7273 5f6e  ent_indicators_n
+00003270: 6f76 656d 6265 725f 3230 3232 5f63 7376  ovember_2022_csv
+00003280: 5f74 6162 6c65 732e 6373 760a 6060 600a  _tables.csv.```.
+00003290: 5365 7269 6573 5f72 6566 6572 656e 6365  Series_reference
+000032a0: 2c50 6572 696f 642c 4461 7461 5f76 616c  ,Period,Data_val
+000032b0: 7565 2c53 7570 7072 6573 7365 640a 4d45  ue,Suppressed.ME
+000032c0: 494d 2e53 3157 412c 3139 3939 2e30 342c  IM.S1WA,1999.04,
+000032d0: 3830 3236 372c 0a4d 4549 4d2e 5331 5741  80267,.MEIM.S1WA
+000032e0: 2c31 3939 392e 3035 2c37 3038 3033 2c0a  ,1999.05,70803,.
+000032f0: 4d45 494d 2e53 3157 412c 3139 3939 2e30  MEIM.S1WA,1999.0
+00003300: 362c 3635 3739 322c 0a4d 4549 4d2e 5331  6,65792,.MEIM.S1
+00003310: 5741 2c31 3939 392e 3037 2c36 3631 3934  WA,1999.07,66194
+00003320: 2c0a 4d45 494d 2e53 3157 412c 3139 3939  ,.MEIM.S1WA,1999
+00003330: 2e30 382c 3637 3235 392c 0a4d 4549 4d2e  .08,67259,.MEIM.
+00003340: 5331 5741 2c31 3939 392e 3039 2c36 3936  S1WA,1999.09,696
+00003350: 3931 2c0a 4d45 494d 2e53 3157 412c 3139  91,.MEIM.S1WA,19
+00003360: 3939 2e31 2c37 3234 3735 2c0a 4d45 494d  99.1,72475,.MEIM
+00003370: 2e53 3157 412c 3139 3939 2e31 312c 3739  .S1WA,1999.11,79
+00003380: 3236 332c 0a4d 4549 4d2e 5331 5741 2c31  263,.MEIM.S1WA,1
+00003390: 3939 392e 3132 2c38 3635 3430 2c0a 4d45  999.12,86540,.ME
+000033a0: 494d 2e53 3157 412c 3230 3030 2e30 312c  IM.S1WA,2000.01,
+000033b0: 3832 3535 322c 0a4d 4549 4d2e 5331 5741  82552,.MEIM.S1WA
+000033c0: 2c32 3030 302e 3032 2c38 3137 3039 2c0a  ,2000.02,81709,.
+000033d0: 4d45 494d 2e53 3157 412c 3230 3030 2e30  MEIM.S1WA,2000.0
+000033e0: 332c 3834 3132 362c 0a4d 4549 4d2e 5331  3,84126,.MEIM.S1
+000033f0: 5741 2c32 3030 302e 3034 2c37 3730 3839  WA,2000.04,77089
+00003400: 2c0a 4d45 494d 2e53 3157 412c 3230 3030  ,.MEIM.S1WA,2000
+00003410: 2e30 352c 3733 3831 312c 0a4d 4549 4d2e  .05,73811,.MEIM.
+00003420: 5331 5741 2c32 3030 302e 3036 2c37 3030  S1WA,2000.06,700
+00003430: 3730 2c0a 4d45 494d 2e53 3157 412c 3230  70,.MEIM.S1WA,20
+00003440: 3030 2e30 372c 3639 3837 332c 0a4d 4549  00.07,69873,.MEI
+00003450: 4d2e 5331 5741 2c32 3030 302e 3038 2c37  M.S1WA,2000.08,7
+00003460: 3134 3638 2c0a 4d45 494d 2e53 3157 412c  1468,.MEIM.S1WA,
+00003470: 3230 3030 2e30 392c 3732 3436 322c 0a4d  2000.09,72462,.M
+00003480: 4549 4d2e 5331 5741 2c32 3030 302e 312c  EIM.S1WA,2000.1,
+00003490: 3734 3839 372c 0a60 6060 0a0a 6d6f 6465  74897,.```..mode
+000034a0: 6c2e 7371 6c0a 6060 600a 7b7b 2063 6f6e  l.sql.```.{{ con
+000034b0: 6669 6728 0a20 2020 206d 6174 6572 6961  fig(.    materia
+000034c0: 6c69 7a65 643d 2774 6162 6c65 270a 2920  lized='table'.) 
+000034d0: 7d7d 0a0a 5345 4c45 4354 0a20 2020 2052  }}..SELECT.    R
+000034e0: 4f57 5f4e 554d 4245 5228 2920 4f56 4552  OW_NUMBER() OVER
+000034f0: 2028 2920 4153 2069 640a 2020 2020 2c20   () AS id.    , 
+00003500: 2a0a 2020 2020 2c20 6361 7374 2866 726f  *.    , cast(fro
+00003510: 6d5f 756e 6978 7469 6d65 2874 6f5f 756e  m_unixtime(to_un
+00003520: 6978 7469 6d65 286e 6f77 2829 2929 2061  ixtime(now())) a
+00003530: 7320 7469 6d65 7374 616d 7028 3629 2920  s timestamp(6)) 
+00003540: 4153 2072 6566 7265 7368 5f74 696d 6573  AS refresh_times
+00003550: 7461 6d70 0a46 524f 4d20 7b7b 2072 6566  tamp.FROM {{ ref
+00003560: 2827 656d 706c 6f79 6d65 6e74 5f69 6e64  ('employment_ind
+00003570: 6963 6174 6f72 735f 6e6f 7665 6d62 6572  icators_november
+00003580: 5f32 3032 325f 6373 765f 7461 626c 6573  _2022_csv_tables
+00003590: 2729 207d 7d0a 6060 600a 0a74 696d 6573  ') }}.```..times
+000035a0: 7461 6d70 2073 7472 6174 6567 7920 2d20  tamp strategy - 
+000035b0: 6d6f 6465 6c5f 736e 6170 7368 6f74 5f31  model_snapshot_1
+000035c0: 0a0a 6060 600a 7b25 2073 6e61 7073 686f  ..```.{% snapsho
+000035d0: 7420 6d6f 6465 6c5f 736e 6170 7368 6f74  t model_snapshot
+000035e0: 5f31 2025 7d0a 0a7b 7b0a 2020 2020 636f  _1 %}..{{.    co
+000035f0: 6e66 6967 280a 2020 2020 2020 7374 7261  nfig(.      stra
+00003600: 7465 6779 3d27 7469 6d65 7374 616d 7027  tegy='timestamp'
+00003610: 2c0a 2020 2020 2020 7570 6461 7465 645f  ,.      updated_
+00003620: 6174 3d27 7265 6672 6573 685f 7469 6d65  at='refresh_time
+00003630: 7374 616d 7027 2c0a 2020 2020 2020 756e  stamp',.      un
+00003640: 6971 7565 5f6b 6579 3d27 6964 270a 2020  ique_key='id'.  
+00003650: 2020 290a 7d7d 0a0a 5345 4c45 4354 202a    ).}}..SELECT *
+00003660: 0a0a 6672 6f6d 207b 7b20 7265 6628 276d  ..from {{ ref('m
+00003670: 6f64 656c 2729 207d 7d0a 0a7b 2520 656e  odel') }}..{% en
+00003680: 6473 6e61 7073 686f 7420 257d 0a60 6060  dsnapshot %}.```
+00003690: 0a0a 696e 7661 6c69 6461 7465 2068 6172  ..invalidate har
+000036a0: 6420 6465 6c65 7465 7320 2d20 6d6f 6465  d deletes - mode
+000036b0: 6c5f 736e 6170 7368 6f74 5f32 0a60 6060  l_snapshot_2.```
+000036c0: 0a7b 2520 736e 6170 7368 6f74 206d 6f64  .{% snapshot mod
+000036d0: 656c 5f73 6e61 7073 686f 745f 3220 257d  el_snapshot_2 %}
+000036e0: 0a0a 7b7b 0a20 2020 2063 6f6e 6669 670a  ..{{.    config.
+000036f0: 2020 2020 280a 2020 2020 2020 2020 756e      (.        un
+00003700: 6971 7565 5f6b 6579 3d27 6964 272c 0a20  ique_key='id',. 
+00003710: 2020 2020 2020 2073 7472 6174 6567 793d         strategy=
+00003720: 2774 696d 6573 7461 6d70 272c 0a20 2020  'timestamp',.   
+00003730: 2020 2020 2075 7064 6174 6564 5f61 743d       updated_at=
+00003740: 2772 6566 7265 7368 5f74 696d 6573 7461  'refresh_timesta
+00003750: 6d70 272c 0a20 2020 2020 2020 2069 6e76  mp',.        inv
+00003760: 616c 6964 6174 655f 6861 7264 5f64 656c  alidate_hard_del
+00003770: 6574 6573 3d54 7275 652c 0a20 2020 2029  etes=True,.    )
+00003780: 0a7d 7d0a 5345 4c45 4354 202a 2066 726f  .}}.SELECT * fro
+00003790: 6d20 7b7b 2072 6566 2827 6d6f 6465 6c27  m {{ ref('model'
+000037a0: 2920 7d7d 0a0a 7b25 2065 6e64 736e 6170  ) }}..{% endsnap
+000037b0: 7368 6f74 2025 7d0a 6060 600a 0a63 6865  shot %}.```..che
+000037c0: 636b 2073 7472 6174 6567 7920 2d20 6d6f  ck strategy - mo
+000037d0: 6465 6c5f 736e 6170 7368 6f74 5f33 0a60  del_snapshot_3.`
+000037e0: 6060 0a7b 2520 736e 6170 7368 6f74 206d  ``.{% snapshot m
+000037f0: 6f64 656c 5f73 6e61 7073 686f 745f 3320  odel_snapshot_3 
+00003800: 257d 0a0a 7b7b 0a20 2020 2063 6f6e 6669  %}..{{.    confi
+00003810: 670a 2020 2020 280a 2020 2020 2020 2020  g.    (.        
+00003820: 756e 6971 7565 5f6b 6579 3d27 6964 272c  unique_key='id',
+00003830: 0a20 2020 2020 2020 2073 7472 6174 6567  .        strateg
+00003840: 793d 2763 6865 636b 272c 0a20 2020 2020  y='check',.     
+00003850: 2020 2063 6865 636b 5f63 6f6c 733d 5b27     check_cols=['
+00003860: 7365 7269 6573 5f72 6566 6572 656e 6365  series_reference
+00003870: 272c 2764 6174 615f 7661 6c75 6527 5d0a  ','data_value'].
+00003880: 2020 2020 290a 7d7d 0a53 454c 4543 5420      ).}}.SELECT 
+00003890: 2a20 6672 6f6d 207b 7b20 7265 6628 276d  * from {{ ref('m
+000038a0: 6f64 656c 2729 207d 7d0a 0a7b 2520 656e  odel') }}..{% en
+000038b0: 6473 6e61 7073 686f 7420 257d 0a60 6060  dsnapshot %}.```
+000038c0: 0a0a 2323 2320 4b6e 6f77 6e20 6973 7375  ..### Known issu
+000038d0: 6573 0a0a 2a20 496e 6372 656d 656e 7461  es..* Incrementa
+000038e0: 6c20 4963 6562 6572 6720 6d6f 6465 6c73  l Iceberg models
+000038f0: 202d 2053 796e 6320 616c 6c20 636f 6c75   - Sync all colu
+00003900: 6d6e 7320 6f6e 2073 6368 656d 6120 6368  mns on schema ch
+00003910: 616e 6765 2063 616e 2774 2072 656d 6f76  ange can't remov
+00003920: 6520 636f 6c75 6d6e 7320 7573 6564 2061  e columns used a
+00003930: 7320 7061 7274 6974 696f 6e69 6e67 2e0a  s partitioning..
+00003940: 5468 6520 6f6e 6c79 2077 6179 2c20 6672  The only way, fr
+00003950: 6f6d 2061 2064 6274 2070 6572 7370 6563  om a dbt perspec
+00003960: 7469 7665 2c20 6973 2074 6f20 646f 2061  tive, is to do a
+00003970: 2066 756c 6c2d 7265 6672 6573 6820 6f66   full-refresh of
+00003980: 2074 6865 2069 6e63 7265 6d65 6e74 616c   the incremental
+00003990: 206d 6f64 656c 2e0a 0a2a 2054 6162 6c65   model...* Table
+000039a0: 732c 2073 6368 656d 6173 2061 6e64 2064  s, schemas and d
+000039b0: 6174 6162 6173 6520 7368 6f75 6c64 206f  atabase should o
+000039c0: 6e6c 7920 6265 206c 6f77 6572 6361 7365  nly be lowercase
+000039d0: 0a0a 2a20 496e 206f 7264 6572 2074 6f20  ..* In order to 
+000039e0: 6176 6f69 6420 706f 7465 6e74 6961 6c20  avoid potential 
+000039f0: 636f 6e66 6c69 6374 732c 206d 616b 6520  conflicts, make 
+00003a00: 7375 7265 205b 6064 6274 2d61 7468 656e  sure [`dbt-athen
+00003a10: 612d 6164 6170 7465 7260 5d28 6874 7470  a-adapter`](http
+00003a20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00003a30: 6f6d 6d65 2f64 6274 2d61 7468 656e 6129  omme/dbt-athena)
+00003a40: 2069 7320 6e6f 7420 696e 7374 616c 6c65   is not installe
+00003a50: 6420 696e 2074 6865 2074 6172 6765 7420  d in the target 
+00003a60: 656e 7669 726f 6e6d 656e 742e 0a20 2053  environment..  S
+00003a70: 6565 2068 7474 7073 3a2f 2f67 6974 6875  ee https://githu
+00003a80: 622e 636f 6d2f 6462 742d 6174 6865 6e61  b.com/dbt-athena
+00003a90: 2f64 6274 2d61 7468 656e 612f 6973 7375  /dbt-athena/issu
+00003aa0: 6573 2f31 3033 2066 6f72 206d 6f72 6520  es/103 for more 
+00003ab0: 6465 7461 696c 732e 0a0a 2a20 536e 6170  details...* Snap
+00003ac0: 7368 6f74 2064 6f65 7320 6e6f 7420 7375  shot does not su
+00003ad0: 7070 6f72 7420 6472 6f70 7069 6e67 2063  pport dropping c
+00003ae0: 6f6c 756d 6e73 2066 726f 6d20 7468 6520  olumns from the 
+00003af0: 736f 7572 6365 2074 6162 6c65 2e20 4966  source table. If
+00003b00: 2079 6f75 2064 726f 7020 6120 636f 6c75   you drop a colu
+00003b10: 6d6e 206d 616b 6520 7375 7265 2074 6f20  mn make sure to 
+00003b20: 6472 6f70 2074 6865 2063 6f6c 756d 6e20  drop the column 
+00003b30: 6672 6f6d 2074 6865 2073 6e61 7073 686f  from the snapsho
+00003b40: 7420 6173 2077 656c 6c2e 2041 6e6f 7468  t as well. Anoth
+00003b50: 6572 2077 6f72 6b61 726f 756e 6420 6973  er workaround is
+00003b60: 2074 6f20 4e55 4c4c 2074 6865 2063 6f6c   to NULL the col
+00003b70: 756d 6e20 696e 2074 6865 2073 6e61 7073  umn in the snaps
+00003b80: 686f 7420 6465 6669 6e69 7469 6f6e 2074  hot definition t
+00003b90: 6f20 7072 6573 6572 7665 2068 6973 746f  o preserve histo
+00003ba0: 7279 0a0a 0a23 2320 436f 6e74 7269 6275  ry...## Contribu
+00003bb0: 7469 6e67 0a0a 5468 6973 2063 6f6e 6e65  ting..This conne
+00003bc0: 6374 6f72 2077 6f72 6b73 2077 6974 6820  ctor works with 
+00003bd0: 5079 7468 6f6e 2066 726f 6d20 332e 3720  Python from 3.7 
+00003be0: 746f 2033 2e31 312e 0a0a 2323 2320 4765  to 3.11...### Ge
+00003bf0: 7474 696e 6720 7374 6172 7465 640a 0a49  tting started..I
+00003c00: 6e20 6f72 6465 7220 746f 2073 7461 7274  n order to start
+00003c10: 2064 6576 656c 6f70 696e 6720 6f6e 2074   developing on t
+00003c20: 6869 7320 6164 6170 7465 7220 636c 6f6e  his adapter clon
+00003c30: 6520 7468 6520 7265 706f 2061 6e64 2072  e the repo and r
+00003c40: 756e 2074 6869 7320 6d61 6b65 2063 6f6d  un this make com
+00003c50: 6d61 6e64 2028 7365 6520 5b4d 616b 6566  mand (see [Makef
+00003c60: 696c 655d 284d 616b 6566 696c 6529 2920  ile](Makefile)) 
+00003c70: 3a0a 0a60 6060 6261 7368 0a6d 616b 6520  :..```bash.make 
+00003c80: 7365 7475 700a 6060 600a 0a49 7420 7769  setup.```..It wi
+00003c90: 6c6c 203a 0a31 2e20 496e 7374 616c 6c20  ll :.1. Install 
+00003ca0: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
+00003cb0: 2e0a 322e 2049 6e73 7461 6c6c 2070 7265  ..2. Install pre
+00003cc0: 2d63 6f6d 6d69 7420 686f 6f6b 732e 0a33  -commit hooks..3
+00003cd0: 2e20 4765 6e65 7261 7465 2079 6f75 7220  . Generate your 
+00003ce0: 602e 656e 7660 2066 696c 650a 0a4e 6578  `.env` file..Nex
+00003cf0: 742c 2061 646a 7573 7420 602e 656e 7660  t, adjust `.env`
+00003d00: 2066 696c 6520 6279 2063 6f6e 6669 6775   file by configu
+00003d10: 7269 6e67 2074 6865 2065 6e76 6972 6f6e  ring the environ
+00003d20: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
+00003d30: 6f20 6d61 7463 6820 796f 7572 2041 7468  o match your Ath
+00003d40: 656e 6120 6465 7665 6c6f 706d 656e 7420  ena development 
+00003d50: 656e 7669 726f 6e6d 656e 742e 0a0a 2323  environment...##
+00003d60: 2320 5275 6e6e 696e 6720 7465 7374 730a  # Running tests.
+00003d70: 0a57 6520 6861 7665 2032 2064 6966 6665  .We have 2 diffe
+00003d80: 7265 6e74 2074 7970 6573 206f 6620 7465  rent types of te
+00003d90: 7374 696e 673a 0a2a 202a 2a75 6e69 7420  sting:.* **unit 
+00003da0: 7465 7374 696e 672a 2a3a 2079 6f75 2063  testing**: you c
+00003db0: 616e 2072 756e 2074 6869 7320 7479 7065  an run this type
+00003dc0: 206f 6620 7465 7374 7320 7275 6e6e 696e   of tests runnin
+00003dd0: 6720 606d 616b 6520 756e 6974 5f74 6573  g `make unit_tes
+00003de0: 7460 0a2a 202a 2a66 756e 6374 696f 6e61  t`.* **functiona
+00003df0: 6c20 7465 7374 696e 672a 2a3a 2079 6f75  l testing**: you
+00003e00: 206d 7573 7420 6861 7665 2061 6e20 4157   must have an AW
+00003e10: 5320 6163 636f 756e 7420 7769 7468 2041  S account with A
+00003e20: 7468 656e 6120 7365 7475 7020 696e 206f  thena setup in o
+00003e30: 7264 6572 2074 6f20 6c61 756e 6368 2074  rder to launch t
+00003e40: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
+00003e50: 7320 616e 6420 6861 7665 2061 2060 2e65  s and have a `.e
+00003e60: 6e76 6020 6669 6c65 2069 6e20 706c 6163  nv` file in plac
+00003e70: 6520 7769 7468 2074 6865 2072 6967 6874  e with the right
+00003e80: 2076 616c 7565 732e 0a20 2059 6f75 2063   values..  You c
+00003e90: 616e 2072 756e 2074 6869 7320 7479 7065  an run this type
+00003ea0: 206f 6620 7465 7374 7320 7275 6e6e 696e   of tests runnin
+00003eb0: 6720 606d 616b 6520 6675 6e63 7469 6f6e  g `make function
+00003ec0: 616c 5f74 6573 7460 0a0a 416c 6c20 7479  al_test`..All ty
+00003ed0: 7065 206f 6620 7465 7374 7320 6361 6e20  pe of tests can 
+00003ee0: 6265 2072 756e 2075 7369 6e67 2060 6d61  be run using `ma
+00003ef0: 6b65 603a 0a60 6060 6261 7368 0a6d 616b  ke`:.```bash.mak
+00003f00: 6520 7465 7374 0a60 6060 0a0a 2323 2320  e test.```..### 
+00003f10: 5075 6c6c 2052 6571 7565 7374 0a0a 2a20  Pull Request..* 
+00003f20: 4372 6561 7465 2061 2063 6f6d 6d69 7420  Create a commit 
+00003f30: 7769 7468 2079 6f75 7220 6368 616e 6765  with your change
+00003f40: 7320 616e 6420 7075 7368 2074 6865 6d20  s and push them 
+00003f50: 746f 2061 0a20 205b 666f 726b 5d28 6874  to a.  [fork](ht
+00003f60: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
+00003f70: 622e 636f 6d2f 656e 2f67 6574 2d73 7461  b.com/en/get-sta
+00003f80: 7274 6564 2f71 7569 636b 7374 6172 742f  rted/quickstart/
+00003f90: 666f 726b 2d61 2d72 6570 6f29 2e0a 2a20  fork-a-repo)..* 
+00003fa0: 4372 6561 7465 2061 205b 7075 6c6c 2072  Create a [pull r
+00003fb0: 6571 7565 7374 206f 6e0a 2020 4769 7468  equest on.  Gith
+00003fc0: 7562 5d28 6874 7470 733a 2f2f 646f 6373  ub](https://docs
+00003fd0: 2e67 6974 6875 622e 636f 6d2f 656e 2f67  .github.com/en/g
+00003fe0: 6974 6875 622f 636f 6c6c 6162 6f72 6174  ithub/collaborat
+00003ff0: 696e 672d 7769 7468 2d70 756c 6c2d 7265  ing-with-pull-re
+00004000: 7175 6573 7473 2f70 726f 706f 7369 6e67  quests/proposing
+00004010: 2d63 6861 6e67 6573 2d74 6f2d 796f 7572  -changes-to-your
+00004020: 2d77 6f72 6b2d 7769 7468 2d70 756c 6c2d  -work-with-pull-
+00004030: 7265 7175 6573 7473 2f63 7265 6174 696e  requests/creatin
+00004040: 672d 612d 7075 6c6c 2d72 6571 7565 7374  g-a-pull-request
+00004050: 2d66 726f 6d2d 612d 666f 726b 292e 0a2a  -from-a-fork)..*
+00004060: 2050 756c 6c20 7265 7175 6573 7420 7469   Pull request ti
+00004070: 746c 6520 616e 6420 6d65 7373 6167 6520  tle and message 
+00004080: 2861 6e64 2050 5220 7469 746c 6520 616e  (and PR title an
+00004090: 6420 6465 7363 7269 7074 696f 6e29 206d  d description) m
+000040a0: 7573 7420 6164 6865 7265 2074 6f0a 2020  ust adhere to.  
+000040b0: 5b63 6f6e 7665 6e74 696f 6e61 6c63 6f6d  [conventionalcom
+000040c0: 6d69 7473 5d28 6874 7470 733a 2f2f 7777  mits](https://ww
+000040d0: 772e 636f 6e76 656e 7469 6f6e 616c 636f  w.conventionalco
+000040e0: 6d6d 6974 732e 6f72 6729 2e0a 2a20 5075  mmits.org)..* Pu
+000040f0: 6c6c 2072 6571 7565 7374 2062 6f64 7920  ll request body 
+00004100: 7368 6f75 6c64 2064 6573 6372 6962 6520  should describe 
+00004110: 5f6d 6f74 6976 6174 696f 6e5f 2e0a 0a0a  _motivation_....
+00004120: 2323 2052 6573 6f75 7263 6573 0a2a 205b  ## Resources.* [
+00004130: 4174 6865 6e61 2043 5245 4154 4520 5441  Athena CREATE TA
+00004140: 424c 4520 4153 5d28 6874 7470 733a 2f2f  BLE AS](https://
+00004150: 646f 6373 2e61 7773 2e61 6d61 7a6f 6e2e  docs.aws.amazon.
+00004160: 636f 6d2f 6174 6865 6e61 2f6c 6174 6573  com/athena/lates
+00004170: 742f 7567 2f63 7265 6174 652d 7461 626c  t/ug/create-tabl
+00004180: 652d 6173 2e68 746d 6c29 0a2a 205b 6462  e-as.html).* [db
+00004190: 742d 6c61 6273 2f64 6274 2d63 6f72 655d  t-labs/dbt-core]
+000041a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000041b0: 636f 6d2f 6462 742d 6c61 6273 2f64 6274  com/dbt-labs/dbt
+000041c0: 2d63 6f72 6529 0a2a 205b 6c61 7567 6869  -core).* [laughi
+000041d0: 6e67 6d61 6e37 3734 332f 5079 4174 6865  ngman7743/PyAthe
+000041e0: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
+000041f0: 7562 2e63 6f6d 2f6c 6175 6768 696e 676d  ub.com/laughingm
+00004200: 616e 3737 3433 2f50 7941 7468 656e 6129  an7743/PyAthena)
+00004210: 0a0a 0a23 2320 436f 6e74 7269 6275 746f  ...## Contributo
+00004220: 7273 20e2 9ca8 0a0a 5468 616e 6b73 2067  rs .....Thanks g
+00004230: 6f65 7320 746f 2074 6865 7365 2077 6f6e  oes to these won
+00004240: 6465 7266 756c 2070 656f 706c 6520 285b  derful people ([
+00004250: 656d 6f6a 6920 6b65 795d 2868 7474 7073  emoji key](https
+00004260: 3a2f 2f61 6c6c 636f 6e74 7269 6275 746f  ://allcontributo
+00004270: 7273 2e6f 7267 2f64 6f63 732f 656e 2f65  rs.org/docs/en/e
+00004280: 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c 212d  moji-key)):..<!-
+00004290: 2d20 414c 4c2d 434f 4e54 5249 4255 544f  - ALL-CONTRIBUTO
+000042a0: 5253 2d4c 4953 543a 5354 4152 5420 2d20  RS-LIST:START - 
+000042b0: 446f 206e 6f74 2072 656d 6f76 6520 6f72  Do not remove or
+000042c0: 206d 6f64 6966 7920 7468 6973 2073 6563   modify this sec
+000042d0: 7469 6f6e 202d 2d3e 0a3c 212d 2d20 7072  tion -->.<!-- pr
+000042e0: 6574 7469 6572 2d69 676e 6f72 652d 7374  ettier-ignore-st
+000042f0: 6172 7420 2d2d 3e0a 3c21 2d2d 206d 6172  art -->.<!-- mar
+00004300: 6b64 6f77 6e6c 696e 742d 6469 7361 626c  kdownlint-disabl
+00004310: 6520 2d2d 3e0a 3c74 6162 6c65 3e0a 2020  e -->.<table>.  
+00004320: 3c74 626f 6479 3e0a 2020 2020 3c74 723e  <tbody>.    <tr>
+00004330: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00004340: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00004350: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00004360: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00004370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004380: 6d2f 6e69 636f 7238 3822 3e3c 696d 6720  m/nicor88"><img 
+00004390: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
+000043a0: 7461 7273 2e67 6974 6875 6275 7365 7263  tars.githubuserc
+000043b0: 6f6e 7465 6e74 2e63 6f6d 2f75 2f36 3237  ontent.com/u/627
+000043c0: 3835 3437 3f76 3d34 3f73 3d31 3030 2220  8547?v=4?s=100" 
+000043d0: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
+000043e0: 6c74 3d22 6e69 636f 7238 3822 2f3e 3c62  lt="nicor88"/><b
+000043f0: 7220 2f3e 3c73 7562 3e3c 623e 6e69 636f  r /><sub><b>nico
+00004400: 7238 383c 2f62 3e3c 2f73 7562 3e3c 2f61  r88</b></sub></a
+00004410: 3e3c 6272 202f 3e3c 6120 6872 6566 3d22  ><br /><a href="
+00004420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004430: 6f6d 2f64 6274 2d61 7468 656e 612f 6462  om/dbt-athena/db
+00004440: 742d 6174 6865 6e61 2f63 6f6d 6d69 7473  t-athena/commits
+00004450: 3f61 7574 686f 723d 6e69 636f 7238 3822  ?author=nicor88"
+00004460: 2074 6974 6c65 3d22 436f 6465 223e f09f   title="Code">..
+00004470: 92bb 3c2f 613e 203c 6120 6872 6566 3d22  ..</a> <a href="
+00004480: 236d 6169 6e74 656e 616e 6365 2d6e 6963  #maintenance-nic
+00004490: 6f72 3838 2220 7469 746c 653d 224d 6169  or88" title="Mai
+000044a0: 6e74 656e 616e 6365 223e f09f 9aa7 3c2f  ntenance">....</
+000044b0: 613e 3c2f 7464 3e0a 2020 2020 2020 3c74  a></td>.      <t
+000044c0: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+000044d0: 2076 616c 6967 6e3d 2274 6f70 2220 7769   valign="top" wi
+000044e0: 6474 683d 2231 342e 3238 2522 3e3c 6120  dth="14.28%"><a 
+000044f0: 6872 6566 3d22 6874 7470 733a 2f2f 6a65  href="https://je
+00004500: 7373 6564 6f62 6265 6c61 652e 7265 223e  ssedobbelae.re">
+00004510: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00004520: 2f2f 6176 6174 6172 732e 6769 7468 7562  //avatars.github
+00004530: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00004540: 752f 3133 3532 3937 393f 763d 343f 733d  u/1352979?v=4?s=
+00004550: 3130 3022 2077 6964 7468 3d22 3130 3070  100" width="100p
+00004560: 783b 2220 616c 743d 224a 6573 7365 2044  x;" alt="Jesse D
+00004570: 6f62 6265 6c61 6572 6522 2f3e 3c62 7220  obbelaere"/><br 
+00004580: 2f3e 3c73 7562 3e3c 623e 4a65 7373 6520  /><sub><b>Jesse 
+00004590: 446f 6262 656c 6165 7265 3c2f 623e 3c2f  Dobbelaere</b></
+000045a0: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+000045b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000045c0: 6974 6875 622e 636f 6d2f 6462 742d 6174  ithub.com/dbt-at
+000045d0: 6865 6e61 2f64 6274 2d61 7468 656e 612f  hena/dbt-athena/
+000045e0: 6973 7375 6573 3f71 3d61 7574 686f 7225  issues?q=author%
+000045f0: 3341 6a65 7373 6564 6f62 6265 6c61 6572  3Ajessedobbelaer
+00004600: 6522 2074 6974 6c65 3d22 4275 6720 7265  e" title="Bug re
+00004610: 706f 7274 7322 3ef0 9f90 9b3c 2f61 3e20  ports">....</a> 
+00004620: 3c61 2068 7265 663d 2223 6d61 696e 7465  <a href="#mainte
+00004630: 6e61 6e63 652d 6a65 7373 6564 6f62 6265  nance-jessedobbe
+00004640: 6c61 6572 6522 2074 6974 6c65 3d22 4d61  laere" title="Ma
+00004650: 696e 7465 6e61 6e63 6522 3ef0 9f9a a73c  intenance">....<
+00004660: 2f61 3e3c 2f74 643e 0a20 2020 2020 203c  /a></td>.      <
+00004670: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00004680: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+00004690: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+000046a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000046b0: 6974 6875 622e 636f 6d2f 6c65 6d69 6666  ithub.com/lemiff
+000046c0: 6522 3e3c 696d 6720 7372 633d 2268 7474  e"><img src="htt
+000046d0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+000046e0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000046f0: 6f6d 2f75 2f37 3438 3737 3732 3f76 3d34  om/u/7487772?v=4
+00004700: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
+00004710: 3030 7078 3b22 2061 6c74 3d22 4c65 6d69  00px;" alt="Lemi
+00004720: 6666 6522 2f3e 3c62 7220 2f3e 3c73 7562  ffe"/><br /><sub
+00004730: 3e3c 623e 4c65 6d69 6666 653c 2f62 3e3c  ><b>Lemiffe</b><
+00004740: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
+00004750: 6120 6872 6566 3d22 2364 6573 6967 6e2d  a href="#design-
+00004760: 6c65 6d69 6666 6522 2074 6974 6c65 3d22  lemiffe" title="
+00004770: 4465 7369 676e 223e f09f 8ea8 3c2f 613e  Design">....</a>
+00004780: 3c2f 7464 3e0a 2020 2020 2020 3c74 6420  </td>.      <td 
+00004790: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
+000047a0: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
+000047b0: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
+000047c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000047d0: 7562 2e63 6f6d 2f4a 726d 7979 223e 3c69  ub.com/Jrmyy"><i
+000047e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000047f0: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
+00004800: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
+00004810: 3932 3531 3335 333f 763d 343f 733d 3130  9251353?v=4?s=10
+00004820: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
+00004830: 2220 616c 743d 224a c3a9 72c3 a96d 7920  " alt="J..r..my 
+00004840: 4775 6973 656c 696e 222f 3e3c 6272 202f  Guiselin"/><br /
+00004850: 3e3c 7375 623e 3c62 3e4a c3a9 72c3 a96d  ><sub><b>J..r..m
+00004860: 7920 4775 6973 656c 696e 3c2f 623e 3c2f  y Guiselin</b></
+00004870: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00004880: 2068 7265 663d 2223 6d61 696e 7465 6e61   href="#maintena
+00004890: 6e63 652d 4a72 6d79 7922 2074 6974 6c65  nce-Jrmyy" title
+000048a0: 3d22 4d61 696e 7465 6e61 6e63 6522 3ef0  ="Maintenance">.
+000048b0: 9f9a a73c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
+000048c0: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+000048d0: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
+000048e0: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
+000048f0: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004900: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00004910: 6d6d 6522 3e3c 696d 6720 7372 633d 2268  mme"><img src="h
+00004920: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
+00004930: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00004940: 2e63 6f6d 2f75 2f39 3332 3839 353f 763d  .com/u/932895?v=
+00004950: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00004960: 3130 3070 783b 2220 616c 743d 2254 6f6d  100px;" alt="Tom
+00004970: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
+00004980: 3e54 6f6d 3c2f 623e 3c2f 7375 623e 3c2f  >Tom</b></sub></
+00004990: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
+000049a0: 2223 6d61 696e 7465 6e61 6e63 652d 546f  "#maintenance-To
+000049b0: 6d6d 6522 2074 6974 6c65 3d22 4d61 696e  mme" title="Main
+000049c0: 7465 6e61 6e63 6522 3ef0 9f9a a73c 2f61  tenance">....</a
+000049d0: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+000049e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6462  ://github.com/db
+000049f0: 742d 6174 6865 6e61 2f64 6274 2d61 7468  t-athena/dbt-ath
+00004a00: 656e 612f 636f 6d6d 6974 733f 6175 7468  ena/commits?auth
+00004a10: 6f72 3d54 6f6d 6d65 2220 7469 746c 653d  or=Tomme" title=
+00004a20: 2243 6f64 6522 3ef0 9f92 bb3c 2f61 3e3c  "Code">....</a><
+00004a30: 2f74 643e 0a20 2020 2020 203c 7464 2061  /td>.      <td a
+00004a40: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
+00004a50: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
+00004a60: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
+00004a70: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00004a80: 622e 636f 6d2f 6d61 7474 6961 6d61 7472  b.com/mattiamatr
+00004a90: 6978 223e 3c69 6d67 2073 7263 3d22 6874  ix"><img src="ht
+00004aa0: 7470 733a 2f2f 6176 6174 6172 732e 6769  tps://avatars.gi
+00004ab0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00004ac0: 636f 6d2f 752f 3530 3133 3635 343f 763d  com/u/5013654?v=
+00004ad0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00004ae0: 3130 3070 783b 2220 616c 743d 224d 6174  100px;" alt="Mat
+00004af0: 7469 6122 2f3e 3c62 7220 2f3e 3c73 7562  tia"/><br /><sub
+00004b00: 3e3c 623e 4d61 7474 6961 3c2f 623e 3c2f  ><b>Mattia</b></
+00004b10: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00004b20: 2068 7265 663d 2223 6d61 696e 7465 6e61   href="#maintena
+00004b30: 6e63 652d 6d61 7474 6961 6d61 7472 6978  nce-mattiamatrix
+00004b40: 2220 7469 746c 653d 224d 6169 6e74 656e  " title="Mainten
+00004b50: 616e 6365 223e f09f 9aa7 3c2f 613e 3c2f  ance">....</a></
+00004b60: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00004b70: 3c2f 7462 6f64 793e 0a3c 2f74 6162 6c65  </tbody>.</table
+00004b80: 3e0a 0a3c 212d 2d20 6d61 726b 646f 776e  >..<!-- markdown
+00004b90: 6c69 6e74 2d72 6573 746f 7265 202d 2d3e  lint-restore -->
+00004ba0: 0a3c 212d 2d20 7072 6574 7469 6572 2d69  .<!-- prettier-i
+00004bb0: 676e 6f72 652d 656e 6420 2d2d 3e0a 0a3c  gnore-end -->..<
+00004bc0: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00004bd0: 544f 5253 2d4c 4953 543a 454e 4420 2d2d  TORS-LIST:END --
+00004be0: 3e0a 0a54 6869 7320 7072 6f6a 6563 7420  >..This project 
+00004bf0: 666f 6c6c 6f77 7320 7468 6520 5b61 6c6c  follows the [all
+00004c00: 2d63 6f6e 7472 6962 7574 6f72 735d 2868  -contributors](h
+00004c10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004c20: 6d2f 616c 6c2d 636f 6e74 7269 6275 746f  m/all-contributo
+00004c30: 7273 2f61 6c6c 2d63 6f6e 7472 6962 7574  rs/all-contribut
+00004c40: 6f72 7329 2073 7065 6369 6669 6361 7469  ors) specificati
+00004c50: 6f6e 2e20 436f 6e74 7269 6275 7469 6f6e  on. Contribution
+00004c60: 7320 6f66 2061 6e79 206b 696e 6420 7765  s of any kind we
+00004c70: 6c63 6f6d 6521 0a                        lcome!.
```

### Comparing `dbt-athena-community-1.4.2/README.md` & `dbt-athena-community-1.4.3/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,1031 +1,1224 @@
-00000000: 5b21 5b70 7970 695d 2868 7474 7073 3a2f  [![pypi](https:/
-00000010: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-00000020: 792f 6462 742d 6174 6865 6e61 2d63 6f6d  y/dbt-athena-com
-00000030: 6d75 6e69 7479 2e73 7667 295d 2868 7474  munity.svg)](htt
-00000040: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000050: 6f6a 6563 742f 6462 742d 6174 6865 6e61  oject/dbt-athena
-00000060: 2d63 6f6d 6d75 6e69 7479 2f29 0a5b 215b  -community/).[![
-00000070: 496d 706f 7274 733a 2069 736f 7274 5d28  Imports: isort](
-00000080: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000090: 6c64 732e 696f 2f62 6164 6765 2f25 3230  lds.io/badge/%20
-000000a0: 696d 706f 7274 732d 6973 6f72 742d 2532  imports-isort-%2
-000000b0: 3331 3637 3462 313f 7374 796c 653d 666c  31674b1?style=fl
-000000c0: 6174 266c 6162 656c 436f 6c6f 723d 6566  at&labelColor=ef
-000000d0: 3833 3336 295d 2868 7474 7073 3a2f 2f70  8336)](https://p
-000000e0: 7963 7161 2e67 6974 6875 622e 696f 2f69  ycqa.github.io/i
-000000f0: 736f 7274 2f29 0a5b 215b 436f 6465 2073  sort/).[![Code s
-00000100: 7479 6c65 3a20 626c 6163 6b5d 2868 7474  tyle: black](htt
-00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000120: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
-00000130: 3073 7479 6c65 2d62 6c61 636b 2d30 3030  0style-black-000
-00000140: 3030 302e 7376 6729 5d28 6874 7470 733a  000.svg)](https:
-00000150: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
-00000160: 2f62 6c61 636b 290a 5b21 5b53 7461 7473  /black).[![Stats
-00000170: 3a20 7065 7079 5d28 6874 7470 733a 2f2f  : pepy](https://
-00000180: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
-00000190: 6462 742d 6174 6865 6e61 2d63 6f6d 6d75  dbt-athena-commu
-000001a0: 6e69 7479 2f6d 6f6e 7468 295d 2868 7474  nity/month)](htt
-000001b0: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
-000001c0: 726f 6a65 6374 2f64 6274 2d61 7468 656e  roject/dbt-athen
-000001d0: 612d 636f 6d6d 756e 6974 7929 0a0a 2320  a-community)..# 
-000001e0: 6462 742d 6174 6865 6e61 0a0a 2a20 5375  dbt-athena..* Su
-000001f0: 7070 6f72 7473 2064 6274 2076 6572 7369  pports dbt versi
-00000200: 6f6e 2060 312e 342e 2a60 0a2a 2053 7570  on `1.4.*`.* Sup
-00000210: 706f 7274 7320 5b53 6565 6473 5d5b 7365  ports [Seeds][se
-00000220: 6564 735d 0a2a 2043 6f72 7265 6374 6c79  eds].* Correctly
-00000230: 2064 6574 6563 7473 2076 6965 7773 2061   detects views a
-00000240: 6e64 2074 6865 6972 2063 6f6c 756d 6e73  nd their columns
-00000250: 0a2a 2053 7570 706f 7274 7320 5b74 6162  .* Supports [tab
-00000260: 6c65 206d 6174 6572 6961 6c69 7a61 7469  le materializati
-00000270: 6f6e 5d5b 7461 626c 655d 0a20 202a 205b  on][table].  * [
-00000280: 4963 6562 6572 6720 7461 626c 6573 5d5b  Iceberg tables][
-00000290: 6174 6865 6e61 2d69 6365 6265 7267 5d20  athena-iceberg] 
-000002a0: 6973 2073 7570 706f 7274 6564 202a 2a6f  is supported **o
-000002b0: 6e6c 7920 7769 7468 2041 7468 656e 6120  nly with Athena 
-000002c0: 456e 6769 6e65 2076 332a 2a20 616e 6420  Engine v3** and 
-000002d0: 2a2a 6120 756e 6971 7565 2074 6162 6c65  **a unique table
-000002e0: 206c 6f63 6174 696f 6e2a 2a0a 2020 2873   location**.  (s
-000002f0: 6565 2074 6162 6c65 206c 6f63 6174 696f  ee table locatio
-00000300: 6e20 7365 6374 696f 6e20 6265 6c6f 7729  n section below)
-00000310: 0a20 202a 2048 6976 6520 7461 626c 6573  .  * Hive tables
-00000320: 2069 7320 7375 7070 6f72 7465 6420 6279   is supported by
-00000330: 2062 6f74 6820 4174 6865 6e61 2065 6e67   both Athena eng
-00000340: 696e 6573 2e0a 2a20 5375 7070 6f72 7473  ines..* Supports
-00000350: 205b 696e 6372 656d 656e 7461 6c20 6d6f   [incremental mo
-00000360: 6465 6c73 5d5b 696e 6372 656d 656e 7461  dels][incrementa
-00000370: 6c5d 0a20 202a 204f 6e20 6963 6562 6572  l].  * On iceber
-00000380: 6720 7461 626c 6573 203a 0a20 2020 202a  g tables :.    *
-00000390: 2053 7570 706f 7274 2074 6865 2075 7365   Support the use
-000003a0: 206f 6620 6075 6e69 7175 655f 6b65 7960   of `unique_key`
-000003b0: 206f 6e6c 7920 7769 7468 2074 6865 2060   only with the `
-000003c0: 6d65 7267 6560 2073 7472 6174 6567 790a  merge` strategy.
-000003d0: 2020 2020 2a20 5375 7070 6f72 7420 7468      * Support th
-000003e0: 6520 6061 7070 656e 6460 2073 7472 6174  e `append` strat
-000003f0: 6567 790a 2020 2a20 4f6e 2048 6976 6520  egy.  * On Hive 
-00000400: 7461 626c 6573 203a 0a20 2020 202a 2053  tables :.    * S
-00000410: 7570 706f 7274 2074 776f 2069 6e63 7265  upport two incre
-00000420: 6d65 6e74 616c 2075 7064 6174 6520 7374  mental update st
-00000430: 7261 7465 6769 6573 3a20 6069 6e73 6572  rategies: `inser
-00000440: 745f 6f76 6572 7772 6974 6560 2061 6e64  t_overwrite` and
-00000450: 2060 6170 7065 6e64 600a 2020 2020 2a20   `append`.    * 
-00000460: 446f 6573 202a 2a6e 6f74 2a2a 2073 7570  Does **not** sup
-00000470: 706f 7274 2074 6865 2075 7365 206f 6620  port the use of 
-00000480: 6075 6e69 7175 655f 6b65 7960 0a2a 2053  `unique_key`.* S
-00000490: 7570 706f 7274 7320 5b73 6e61 7073 686f  upports [snapsho
-000004a0: 7473 5d5b 736e 6170 7368 6f74 735d 0a2a  ts][snapshots].*
-000004b0: 2044 6f65 7320 6e6f 7420 7375 7070 6f72   Does not suppor
-000004c0: 7420 5b50 7974 686f 6e20 6d6f 6465 6c73  t [Python models
-000004d0: 5d5b 7079 7468 6f6e 2d6d 6f64 656c 735d  ][python-models]
-000004e0: 0a2a 2044 6f65 7320 6e6f 7420 7375 7070  .* Does not supp
-000004f0: 6f72 7420 5b70 6572 7369 7374 2064 6f63  ort [persist doc
-00000500: 735d 5b70 6572 7369 7374 2d64 6f63 735d  s][persist-docs]
-00000510: 2066 6f72 2076 6965 7773 0a0a 5b73 6565   for views..[see
-00000520: 6473 5d3a 2068 7474 7073 3a2f 2f64 6f63  ds]: https://doc
-00000530: 732e 6765 7464 6274 2e63 6f6d 2f64 6f63  s.getdbt.com/doc
-00000540: 732f 6275 696c 6469 6e67 2d61 2d64 6274  s/building-a-dbt
-00000550: 2d70 726f 6a65 6374 2f73 6565 6473 0a5b  -project/seeds.[
-00000560: 696e 6372 656d 656e 7461 6c5d 3a20 6874  incremental]: ht
-00000570: 7470 733a 2f2f 646f 6373 2e67 6574 6462  tps://docs.getdb
-00000580: 742e 636f 6d2f 646f 6373 2f62 7569 6c64  t.com/docs/build
-00000590: 2f69 6e63 7265 6d65 6e74 616c 2d6d 6f64  /incremental-mod
-000005a0: 656c 730a 5b74 6162 6c65 5d3a 2068 7474  els.[table]: htt
-000005b0: 7073 3a2f 2f64 6f63 732e 6765 7464 6274  ps://docs.getdbt
-000005c0: 2e63 6f6d 2f64 6f63 732f 6275 696c 642f  .com/docs/build/
-000005d0: 6d61 7465 7269 616c 697a 6174 696f 6e73  materializations
-000005e0: 2374 6162 6c65 0a5b 7079 7468 6f6e 2d6d  #table.[python-m
-000005f0: 6f64 656c 735d 3a20 6874 7470 733a 2f2f  odels]: https://
-00000600: 646f 6373 2e67 6574 6462 742e 636f 6d2f  docs.getdbt.com/
-00000610: 646f 6373 2f62 7569 6c64 2f70 7974 686f  docs/build/pytho
-00000620: 6e2d 6d6f 6465 6c73 2363 6f6e 6669 6775  n-models#configu
-00000630: 7269 6e67 2d70 7974 686f 6e2d 6d6f 6465  ring-python-mode
-00000640: 6c73 0a5b 6174 6865 6e61 2d69 6365 6265  ls.[athena-icebe
-00000650: 7267 5d3a 2068 7474 7073 3a2f 2f64 6f63  rg]: https://doc
-00000660: 732e 6177 732e 616d 617a 6f6e 2e63 6f6d  s.aws.amazon.com
-00000670: 2f61 7468 656e 612f 6c61 7465 7374 2f75  /athena/latest/u
-00000680: 672f 7175 6572 7969 6e67 2d69 6365 6265  g/querying-icebe
-00000690: 7267 2e68 746d 6c0a 5b73 6e61 7073 686f  rg.html.[snapsho
-000006a0: 7473 5d3a 2068 7474 7073 3a2f 2f64 6f63  ts]: https://doc
-000006b0: 732e 6765 7464 6274 2e63 6f6d 2f64 6f63  s.getdbt.com/doc
-000006c0: 732f 6275 696c 642f 736e 6170 7368 6f74  s/build/snapshot
-000006d0: 730a 5b70 6572 7369 7374 2d64 6f63 735d  s.[persist-docs]
-000006e0: 3a20 6874 7470 733a 2f2f 646f 6373 2e67  : https://docs.g
-000006f0: 6574 6462 742e 636f 6d2f 7265 6665 7265  etdbt.com/refere
-00000700: 6e63 652f 7265 736f 7572 6365 2d63 6f6e  nce/resource-con
-00000710: 6669 6773 2f70 6572 7369 7374 5f64 6f63  figs/persist_doc
-00000720: 730a 0a23 2323 2049 6e73 7461 6c6c 6174  s..### Installat
-00000730: 696f 6e0a 0a2a 2060 7069 7020 696e 7374  ion..* `pip inst
-00000740: 616c 6c20 6462 742d 6174 6865 6e61 2d63  all dbt-athena-c
-00000750: 6f6d 6d75 6e69 7479 600a 2a20 4f72 2060  ommunity`.* Or `
-00000760: 7069 7020 696e 7374 616c 6c20 6769 742b  pip install git+
-00000770: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000780: 6f6d 2f64 6274 2d61 7468 656e 612f 6462  om/dbt-athena/db
-00000790: 742d 6174 6865 6e61 2e67 6974 600a 0a23  t-athena.git`..#
-000007a0: 2323 2050 7265 7265 7175 6973 6974 6573  ## Prerequisites
-000007b0: 0a0a 546f 2073 7461 7274 2c20 796f 7520  ..To start, you 
-000007c0: 7769 6c6c 206e 6565 6420 616e 2053 3320  will need an S3 
-000007d0: 6275 636b 6574 2c20 666f 7220 696e 7374  bucket, for inst
-000007e0: 616e 6365 2060 6d79 2d62 7563 6b65 7460  ance `my-bucket`
-000007f0: 2061 6e64 2061 6e20 4174 6865 6e61 2064   and an Athena d
-00000800: 6174 6162 6173 653a 0a0a 6060 6073 716c  atabase:..```sql
-00000810: 0a43 5245 4154 4520 4441 5441 4241 5345  .CREATE DATABASE
-00000820: 2049 4620 4e4f 5420 4558 4953 5453 2061   IF NOT EXISTS a
-00000830: 6e61 6c79 7469 6373 5f64 6576 0a43 4f4d  nalytics_dev.COM
-00000840: 4d45 4e54 2027 416e 616c 7974 6963 7320  MENT 'Analytics 
-00000850: 6d6f 6465 6c73 2067 656e 6572 6174 6564  models generated
-00000860: 2062 7920 6462 7420 2864 6576 656c 6f70   by dbt (develop
-00000870: 6d65 6e74 2927 0a4c 4f43 4154 494f 4e20  ment)'.LOCATION 
-00000880: 2773 333a 2f2f 6d79 2d62 7563 6b65 742f  's3://my-bucket/
-00000890: 270a 5749 5448 2044 4250 524f 5045 5254  '.WITH DBPROPERT
-000008a0: 4945 5320 2827 6372 6561 746f 7227 3d27  IES ('creator'='
-000008b0: 466f 6f20 4261 7227 2c20 2765 6d61 696c  Foo Bar', 'email
-000008c0: 273d 2766 6f6f 4062 6172 2e63 6f6d 2729  '='foo@bar.com')
-000008d0: 3b0a 6060 600a 0a4e 6f74 6573 3a0a 2d20  ;.```..Notes:.- 
-000008e0: 5461 6b65 206e 6f74 6520 6f66 2079 6f75  Take note of you
-000008f0: 7220 4157 5320 7265 6769 6f6e 2063 6f64  r AWS region cod
-00000900: 6520 2865 2e67 2e20 6075 732d 7765 7374  e (e.g. `us-west
-00000910: 2d32 6020 6f72 2060 6575 2d77 6573 742d  -2` or `eu-west-
-00000920: 3260 2c20 6574 632e 292e 0a2d 2059 6f75  2`, etc.)..- You
-00000930: 2063 616e 2061 6c73 6f20 7573 6520 5b41   can also use [A
-00000940: 5753 2047 6c75 655d 2868 7474 7073 3a2f  WS Glue](https:/
-00000950: 2f64 6f63 732e 6177 732e 616d 617a 6f6e  /docs.aws.amazon
-00000960: 2e63 6f6d 2f61 7468 656e 612f 6c61 7465  .com/athena/late
-00000970: 7374 2f75 672f 676c 7565 2d61 7468 656e  st/ug/glue-athen
-00000980: 612e 6874 6d6c 2920 746f 2063 7265 6174  a.html) to creat
-00000990: 6520 616e 6420 6d61 6e61 6765 2041 7468  e and manage Ath
-000009a0: 656e 6120 6461 7461 6261 7365 732e 0a0a  ena databases...
-000009b0: 2323 2320 4372 6564 656e 7469 616c 730a  ### Credentials.
-000009c0: 0a54 6869 7320 706c 7567 696e 2064 6f65  .This plugin doe
-000009d0: 7320 6e6f 7420 6163 6365 7074 2061 6e79  s not accept any
-000009e0: 2063 7265 6465 6e74 6961 6c73 2064 6972   credentials dir
-000009f0: 6563 746c 792e 2049 6e73 7465 6164 2c20  ectly. Instead, 
-00000a00: 5b63 7265 6465 6e74 6961 6c73 2061 7265  [credentials are
-00000a10: 2064 6574 6572 6d69 6e65 6420 6175 746f   determined auto
-00000a20: 6d61 7469 6361 6c6c 795d 2868 7474 7073  matically](https
-00000a30: 3a2f 2f62 6f74 6f33 2e61 6d61 7a6f 6e61  ://boto3.amazona
-00000a40: 7773 2e63 6f6d 2f76 312f 646f 6375 6d65  ws.com/v1/docume
-00000a50: 6e74 6174 696f 6e2f 6170 692f 6c61 7465  ntation/api/late
-00000a60: 7374 2f67 7569 6465 2f63 7265 6465 6e74  st/guide/credent
-00000a70: 6961 6c73 2e68 746d 6c29 2062 6173 6564  ials.html) based
-00000a80: 206f 6e20 6061 7773 2063 6c69 602f 6062   on `aws cli`/`b
-00000a90: 6f74 6f33 6020 636f 6e76 656e 7469 6f6e  oto3` convention
-00000aa0: 7320 616e 640a 7374 6f72 6564 206c 6f67  s and.stored log
-00000ab0: 696e 2069 6e66 6f2e 2059 6f75 2063 616e  in info. You can
-00000ac0: 2063 6f6e 6669 6775 7265 2074 6865 2041   configure the A
-00000ad0: 5753 2070 726f 6669 6c65 206e 616d 6520  WS profile name 
-00000ae0: 746f 2075 7365 2076 6961 2060 6177 735f  to use via `aws_
-00000af0: 7072 6f66 696c 655f 6e61 6d65 602e 2043  profile_name`. C
-00000b00: 6865 636b 6f75 7420 4442 5420 7072 6f66  heckout DBT prof
-00000b10: 696c 6520 636f 6e66 6967 7572 6174 696f  ile configuratio
-00000b20: 6e20 6265 6c6f 7720 666f 7220 6465 7461  n below for deta
-00000b30: 696c 732e 0a0a 2323 2320 436f 6e66 6967  ils...### Config
-00000b40: 7572 696e 6720 796f 7572 2070 726f 6669  uring your profi
-00000b50: 6c65 0a0a 4120 6462 7420 7072 6f66 696c  le..A dbt profil
-00000b60: 6520 6361 6e20 6265 2063 6f6e 6669 6775  e can be configu
-00000b70: 7265 6420 746f 2072 756e 2061 6761 696e  red to run again
-00000b80: 7374 2041 5753 2041 7468 656e 6120 7573  st AWS Athena us
-00000b90: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-00000ba0: 6720 636f 6e66 6967 7572 6174 696f 6e3a  g configuration:
-00000bb0: 0a0a 7c20 4f70 7469 6f6e 2020 2020 2020  ..| Option      
-00000bc0: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
-00000bd0: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c10: 2020 2020 2020 7c20 5265 7175 6972 6564        | Required
-00000c20: 3f20 7c20 4578 616d 706c 6520 2020 2020  ? | Example     
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c40: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00000c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000c60: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
-00000c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000cb0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---|-----------|
-00000cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 7333  ----------|.| s3
-00000cf0: 5f73 7461 6769 6e67 5f64 6972 2020 207c  _staging_dir   |
-00000d00: 2053 3320 6c6f 6361 7469 6f6e 2074 6f20   S3 location to 
-00000d10: 7374 6f72 6520 4174 6865 6e61 2071 7565  store Athena que
-00000d20: 7279 2072 6573 756c 7473 2061 6e64 206d  ry results and m
-00000d30: 6574 6164 6174 6120 2020 2020 2020 2020  etadata         
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 7c20 5265 7175 6972 6564 2020 7c20 6073  | Required  | `s
-00000d60: 333a 2f2f 6275 636b 6574 2f64 6274 2f60  3://bucket/dbt/`
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 207c 0a7c 2073 335f 6461         |.| s3_da
-00000d90: 7461 5f64 6972 2020 2020 2020 7c20 5072  ta_dir      | Pr
-00000da0: 6566 6978 2066 6f72 2073 746f 7269 6e67  efix for storing
-00000db0: 2074 6162 6c65 732c 2069 6620 6469 6666   tables, if diff
-00000dc0: 6572 656e 7420 6672 6f6d 2074 6865 2063  erent from the c
-00000dd0: 6f6e 6e65 6374 696f 6e27 7320 6073 335f  onnection's `s3_
-00000de0: 7374 6167 696e 675f 6469 7260 207c 204f  staging_dir` | O
-00000df0: 7074 696f 6e61 6c20 207c 2060 7333 3a2f  ptional  | `s3:/
-00000e00: 2f62 7563 6b65 7432 2f64 6274 2f60 2020  /bucket2/dbt/`  
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 7c0a 7c20 7333 5f64 6174 615f      |.| s3_data_
-00000e30: 6e61 6d69 6e67 2020 207c 2048 6f77 2074  naming   | How t
-00000e40: 6f20 6765 6e65 7261 7465 2074 6162 6c65  o generate table
-00000e50: 2070 6174 6873 2069 6e20 6073 335f 6461   paths in `s3_da
-00000e60: 7461 5f64 6972 6020 2020 2020 2020 2020  ta_dir`         
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2020 2020 2020 2020 2020 7c20 4f70 7469            | Opti
-00000e90: 6f6e 616c 2020 7c20 6073 6368 656d 615f  onal  | `schema_
-00000ea0: 7461 626c 655f 756e 6971 7565 6020 2020  table_unique`   
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 207c 0a7c 2072 6567 696f 6e5f 6e61 6d65   |.| region_name
-00000ed0: 2020 2020 2020 7c20 4157 5320 7265 6769        | AWS regi
-00000ee0: 6f6e 206f 6620 796f 7572 2041 7468 656e  on of your Athen
-00000ef0: 6120 696e 7374 616e 6365 2020 2020 2020  a instance      
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 207c 2052 6571 7569 7265         | Require
-00000f30: 6420 207c 2060 6575 2d77 6573 742d 3160  d  | `eu-west-1`
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000f60: 7c20 7363 6865 6d61 2020 2020 2020 2020  | schema        
-00000f70: 2020 207c 2053 7065 6369 6679 2074 6865     | Specify the
-00000f80: 2073 6368 656d 6120 2841 7468 656e 6120   schema (Athena 
-00000f90: 6461 7461 6261 7365 2920 746f 2062 7569  database) to bui
-00000fa0: 6c64 206d 6f64 656c 7320 696e 746f 2028  ld models into (
-00000fb0: 6c6f 7765 7263 6173 6520 2a2a 6f6e 6c79  lowercase **only
-00000fc0: 2a2a 2920 7c20 5265 7175 6972 6564 2020  **) | Required  
-00000fd0: 7c20 6064 6274 6020 2020 2020 2020 2020  | `dbt`         
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2020 2020 2020 2020 207c 0a7c 2064             |.| d
-00001000: 6174 6162 6173 6520 2020 2020 2020 2020  atabase         
-00001010: 7c20 5370 6563 6966 7920 7468 6520 6461  | Specify the da
-00001020: 7461 6261 7365 2028 4461 7461 2063 6174  tabase (Data cat
-00001030: 616c 6f67 2920 746f 2062 7569 6c64 206d  alog) to build m
-00001040: 6f64 656c 7320 696e 746f 2028 6c6f 7765  odels into (lowe
-00001050: 7263 6173 6520 2a2a 6f6e 6c79 2a2a 2920  rcase **only**) 
-00001060: 207c 2052 6571 7569 7265 6420 207c 2060   | Required  | `
-00001070: 6177 7364 6174 6163 6174 616c 6f67 6020  awsdatacatalog` 
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 7c0a 7c20 706f 6c6c          |.| poll
-000010a0: 5f69 6e74 6572 7661 6c20 2020 207c 2049  _interval    | I
-000010b0: 6e74 6572 7661 6c20 696e 2073 6563 6f6e  nterval in secon
-000010c0: 6473 2074 6f20 7573 6520 666f 7220 706f  ds to use for po
-000010d0: 6c6c 696e 6720 7468 6520 7374 6174 7573  lling the status
-000010e0: 206f 6620 7175 6572 7920 7265 7375 6c74   of query result
-000010f0: 7320 696e 2041 7468 656e 6120 2020 7c20  s in Athena   | 
-00001100: 4f70 7469 6f6e 616c 2020 7c20 6035 6020  Optional  | `5` 
-00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2020 2020 207c 0a7c 2061 7773 5f70 726f       |.| aws_pro
-00001140: 6669 6c65 5f6e 616d 6520 7c20 5072 6f66  file_name | Prof
-00001150: 696c 6520 746f 2075 7365 2066 726f 6d20  ile to use from 
-00001160: 796f 7572 2041 5753 2073 6861 7265 6420  your AWS shared 
-00001170: 6372 6564 656e 7469 616c 7320 6669 6c65  credentials file
-00001180: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00001190: 2020 2020 2020 2020 2020 207c 204f 7074             | Opt
-000011a0: 696f 6e61 6c20 207c 2060 6d79 2d70 726f  ional  | `my-pro
-000011b0: 6669 6c65 6020 2020 2020 2020 2020 2020  file`           
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 7c0a 7c20 776f 726b 5f67 726f 7570    |.| work_group
-000011e0: 2020 2020 2020 207c 2049 6465 6e74 6966         | Identif
-000011f0: 6965 7220 6f66 2041 7468 656e 6120 776f  ier of Athena wo
-00001200: 726b 6772 6f75 7020 2020 2020 2020 2020  rkgroup         
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2020 2020 2020 7c20 4f70 7469 6f6e          | Option
-00001240: 616c 2020 7c20 606d 792d 6375 7374 6f6d  al  | `my-custom
-00001250: 2d77 6f72 6b67 726f 7570 6020 2020 2020  -workgroup`     
-00001260: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001270: 0a7c 206e 756d 5f72 6574 7269 6573 2020  .| num_retries  
-00001280: 2020 2020 7c20 4e75 6d62 6572 206f 6620      | Number of 
-00001290: 7469 6d65 7320 746f 2072 6574 7279 2061  times to retry a
-000012a0: 2066 6169 6c69 6e67 2071 7565 7279 2020   failing query  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 207c 204f 7074 696f 6e61 6c20       | Optional 
-000012e0: 207c 2060 3360 2020 2020 2020 2020 2020   | `3`          
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00001310: 6c66 5f74 6167 7320 2020 2020 2020 2020  lf_tags         
-00001320: 207c 2044 6566 6175 6c74 206c 6620 7461   | Default lf ta
-00001330: 6773 2074 6f20 6170 706c 7920 746f 2061  gs to apply to a
-00001340: 6e79 2064 6174 6162 6173 6520 6372 6561  ny database crea
-00001350: 7465 6420 6279 2064 6274 2020 2020 2020  ted by dbt      
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 7c20 4f70 7469 6f6e 616c 2020 7c20    | Optional  | 
-00001380: 607b 226f 7269 6769 6e22 3a20 2264 6274  `{"origin": "dbt
-00001390: 222c 2022 7465 616d 223a 2022 616e 616c  ", "team": "anal
-000013a0: 7974 6963 7322 7d60 207c 0a0a 2a2a 4578  ytics"}` |..**Ex
-000013b0: 616d 706c 6520 7072 6f66 696c 6573 2e79  ample profiles.y
-000013c0: 6d6c 2065 6e74 7279 3a2a 2a0a 6060 6079  ml entry:**.```y
-000013d0: 616d 6c0a 6174 6865 6e61 3a0a 2020 7461  aml.athena:.  ta
-000013e0: 7267 6574 3a20 6465 760a 2020 6f75 7470  rget: dev.  outp
-000013f0: 7574 733a 0a20 2020 2064 6576 3a0a 2020  uts:.    dev:.  
-00001400: 2020 2020 7479 7065 3a20 6174 6865 6e61      type: athena
-00001410: 0a20 2020 2020 2073 335f 7374 6167 696e  .      s3_stagin
-00001420: 675f 6469 723a 2073 333a 2f2f 6174 6865  g_dir: s3://athe
-00001430: 6e61 2d71 7565 7279 2d72 6573 756c 7473  na-query-results
-00001440: 2f64 6274 2f0a 2020 2020 2020 7333 5f64  /dbt/.      s3_d
-00001450: 6174 615f 6469 723a 2073 333a 2f2f 796f  ata_dir: s3://yo
-00001460: 7572 5f73 335f 6275 636b 6574 2f64 6274  ur_s3_bucket/dbt
-00001470: 2f0a 2020 2020 2020 7333 5f64 6174 615f  /.      s3_data_
-00001480: 6e61 6d69 6e67 3a20 7363 6865 6d61 5f74  naming: schema_t
-00001490: 6162 6c65 0a20 2020 2020 2072 6567 696f  able.      regio
-000014a0: 6e5f 6e61 6d65 3a20 6575 2d77 6573 742d  n_name: eu-west-
-000014b0: 310a 2020 2020 2020 7363 6865 6d61 3a20  1.      schema: 
-000014c0: 6462 740a 2020 2020 2020 6461 7461 6261  dbt.      databa
-000014d0: 7365 3a20 6177 7364 6174 6163 6174 616c  se: awsdatacatal
-000014e0: 6f67 0a20 2020 2020 2061 7773 5f70 726f  og.      aws_pro
-000014f0: 6669 6c65 5f6e 616d 653a 206d 792d 7072  file_name: my-pr
-00001500: 6f66 696c 650a 2020 2020 2020 776f 726b  ofile.      work
-00001510: 5f67 726f 7570 3a20 6d79 2d77 6f72 6b67  _group: my-workg
-00001520: 726f 7570 0a20 2020 2020 206c 665f 7461  roup.      lf_ta
-00001530: 6773 3a0a 2020 2020 2020 2020 6f72 6967  gs:.        orig
-00001540: 696e 3a20 6462 740a 2020 2020 2020 2020  in: dbt.        
-00001550: 7465 616d 3a20 616e 616c 7974 6963 730a  team: analytics.
-00001560: 6060 600a 0a5f 4164 6469 7469 6f6e 616c  ```.._Additional
-00001570: 2069 6e66 6f72 6d61 7469 6f6e 5f0a 2a20   information_.* 
-00001580: 6074 6872 6561 6473 6020 6973 2073 7570  `threads` is sup
-00001590: 706f 7274 6564 0a2a 2060 6461 7461 6261  ported.* `databa
-000015a0: 7365 6020 616e 6420 6063 6174 616c 6f67  se` and `catalog
-000015b0: 6020 6361 6e20 6265 2075 7365 6420 696e  ` can be used in
-000015c0: 7465 7263 6861 6e67 6561 626c 790a 0a23  terchangeably..#
-000015d0: 2323 204d 6f64 656c 730a 0a23 2323 2320  ## Models..#### 
-000015e0: 5461 626c 6520 436f 6e66 6967 7572 6174  Table Configurat
-000015f0: 696f 6e0a 0a2a 2060 6578 7465 726e 616c  ion..* `external
-00001600: 5f6c 6f63 6174 696f 6e60 2028 6064 6566  _location` (`def
-00001610: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-00001620: 4966 2073 6574 2c20 7468 6520 6675 6c6c  If set, the full
-00001630: 2053 3320 7061 7468 2069 6e20 7768 6963   S3 path in whic
-00001640: 6820 7468 6520 7461 626c 6520 7769 6c6c  h the table will
-00001650: 2062 6520 7361 7665 642e 2028 446f 6573   be saved. (Does
-00001660: 206e 6f74 2077 6f72 6b20 7769 7468 2049   not work with I
-00001670: 6365 6265 7267 2074 6162 6c65 292e 0a2a  ceberg table)..*
-00001680: 2060 7061 7274 6974 696f 6e65 645f 6279   `partitioned_by
-00001690: 6020 2860 6465 6661 756c 743d 6e6f 6e65  ` (`default=none
-000016a0: 6029 0a20 202a 2041 6e20 6172 7261 7920  `).  * An array 
-000016b0: 6c69 7374 206f 6620 636f 6c75 6d6e 7320  list of columns 
-000016c0: 6279 2077 6869 6368 2074 6865 2074 6162  by which the tab
-000016d0: 6c65 2077 696c 6c20 6265 2070 6172 7469  le will be parti
-000016e0: 7469 6f6e 6564 0a20 202a 204c 696d 6974  tioned.  * Limit
-000016f0: 6564 2074 6f20 6372 6561 7469 6f6e 206f  ed to creation o
-00001700: 6620 3130 3020 7061 7274 6974 696f 6e73  f 100 partitions
-00001710: 2028 5f63 7572 7265 6e74 6c79 5f29 0a2a   (_currently_).*
-00001720: 2060 6275 636b 6574 6564 5f62 7960 2028   `bucketed_by` (
-00001730: 6064 6566 6175 6c74 3d6e 6f6e 6560 290a  `default=none`).
-00001740: 2020 2a20 416e 2061 7272 6179 206c 6973    * An array lis
-00001750: 7420 6f66 2063 6f6c 756d 6e73 2074 6f20  t of columns to 
-00001760: 6275 636b 6574 2064 6174 612c 2069 676e  bucket data, ign
-00001770: 6f72 6564 2069 6620 7573 696e 6720 4963  ored if using Ic
-00001780: 6562 6572 670a 2a20 6062 7563 6b65 745f  eberg.* `bucket_
-00001790: 636f 756e 7460 2028 6064 6566 6175 6c74  count` (`default
-000017a0: 3d6e 6f6e 6560 290a 2020 2a20 5468 6520  =none`).  * The 
-000017b0: 6e75 6d62 6572 206f 6620 6275 636b 6574  number of bucket
-000017c0: 7320 666f 7220 6275 636b 6574 696e 6720  s for bucketing 
-000017d0: 796f 7572 2064 6174 612c 2069 676e 6f72  your data, ignor
-000017e0: 6564 2069 6620 7573 696e 6720 4963 6562  ed if using Iceb
-000017f0: 6572 670a 2a20 6074 6162 6c65 5f74 7970  erg.* `table_typ
-00001800: 6560 2028 6064 6566 6175 6c74 3d27 6869  e` (`default='hi
-00001810: 7665 2760 290a 2020 2a20 5468 6520 7479  ve'`).  * The ty
-00001820: 7065 206f 6620 7461 626c 650a 2020 2a20  pe of table.  * 
-00001830: 5375 7070 6f72 7473 2060 6869 7665 6020  Supports `hive` 
-00001840: 6f72 2060 6963 6562 6572 6760 0a2a 2060  or `iceberg`.* `
-00001850: 666f 726d 6174 6020 2860 6465 6661 756c  format` (`defaul
-00001860: 743d 2770 6172 7175 6574 2760 290a 2020  t='parquet'`).  
-00001870: 2a20 5468 6520 6461 7461 2066 6f72 6d61  * The data forma
-00001880: 7420 666f 7220 7468 6520 7461 626c 650a  t for the table.
-00001890: 2020 2a20 5375 7070 6f72 7473 2060 4f52    * Supports `OR
-000018a0: 4360 2c20 6050 4152 5155 4554 602c 2060  C`, `PARQUET`, `
-000018b0: 4156 524f 602c 2060 4a53 4f4e 602c 2060  AVRO`, `JSON`, `
-000018c0: 5445 5854 4649 4c45 600a 2a20 6077 7269  TEXTFILE`.* `wri
-000018d0: 7465 5f63 6f6d 7072 6573 7369 6f6e 6020  te_compression` 
-000018e0: 2860 6465 6661 756c 743d 6e6f 6e65 6029  (`default=none`)
-000018f0: 0a20 202a 2054 6865 2063 6f6d 7072 6573  .  * The compres
-00001900: 7369 6f6e 2074 7970 6520 746f 2075 7365  sion type to use
-00001910: 2066 6f72 2061 6e79 2073 746f 7261 6765   for any storage
-00001920: 2066 6f72 6d61 7420 7468 6174 2061 6c6c   format that all
-00001930: 6f77 7320 636f 6d70 7265 7373 696f 6e20  ows compression 
-00001940: 746f 2062 6520 7370 6563 6966 6965 642e  to be specified.
-00001950: 2054 6f20 7365 6520 7768 6963 6820 6f70   To see which op
-00001960: 7469 6f6e 7320 6172 6520 6176 6169 6c61  tions are availa
-00001970: 626c 652c 2063 6865 636b 206f 7574 205b  ble, check out [
-00001980: 4352 4541 5445 2054 4142 4c45 2041 535d  CREATE TABLE AS]
-00001990: 5b63 7265 6174 652d 7461 626c 652d 6173  [create-table-as
-000019a0: 5d0a 2a20 6066 6965 6c64 5f64 656c 696d  ].* `field_delim
-000019b0: 6974 6572 6020 2860 6465 6661 756c 743d  iter` (`default=
-000019c0: 6e6f 6e65 6029 0a20 202a 2043 7573 746f  none`).  * Custo
-000019d0: 6d20 6669 656c 6420 6465 6c69 6d69 7465  m field delimite
-000019e0: 722c 2066 6f72 2077 6865 6e20 666f 726d  r, for when form
-000019f0: 6174 2069 7320 7365 7420 746f 2060 5445  at is set to `TE
-00001a00: 5854 4649 4c45 600a 2a20 6074 6162 6c65  XTFILE`.* `table
-00001a10: 5f70 726f 7065 7274 6965 7360 3a20 7461  _properties`: ta
-00001a20: 626c 6520 7072 6f70 6572 7469 6573 2074  ble properties t
-00001a30: 6f20 6164 6420 746f 2074 6865 2074 6162  o add to the tab
-00001a40: 6c65 2c20 7661 6c69 6420 666f 7220 4963  le, valid for Ic
-00001a50: 6562 6572 6720 6f6e 6c79 0a2a 2060 6c66  eberg only.* `lf
-00001a60: 5f74 6167 7360 2028 6064 6566 6175 6c74  _tags` (`default
-00001a70: 3d6e 6f6e 6560 290a 2020 2a20 6c66 2074  =none`).  * lf t
-00001a80: 6167 7320 746f 2061 7373 6f63 6961 7465  ags to associate
-00001a90: 2077 6974 6820 7468 6520 7461 626c 650a   with the table.
-00001aa0: 2020 2a20 666f 726d 6174 3a20 607b 2274    * format: `{"t
-00001ab0: 6167 3122 3a20 2276 616c 7565 3122 2c20  ag1": "value1", 
-00001ac0: 2274 6167 3222 3a20 2276 616c 7565 3222  "tag2": "value2"
-00001ad0: 7d60 0a2a 2060 6c66 5f74 6167 735f 636f  }`.* `lf_tags_co
-00001ae0: 6c75 6d6e 7360 2028 6064 6566 6175 6c74  lumns` (`default
-00001af0: 3d6e 6f6e 6560 290a 2020 2a20 6c66 2074  =none`).  * lf t
-00001b00: 6167 7320 746f 2061 7373 6f63 6961 7465  ags to associate
-00001b10: 2077 6974 6820 7468 6520 7461 626c 6520   with the table 
-00001b20: 636f 6c75 6d6e 730a 2020 2a20 666f 726d  columns.  * form
-00001b30: 6174 3a20 607b 2274 6167 3122 3a20 7b22  at: `{"tag1": {"
-00001b40: 7661 6c75 6531 223a 205b 2263 6f6c 756d  value1": ["colum
-00001b50: 6e31 223a 2022 636f 6c75 6d6e 3222 5d7d  n1": "column2"]}
-00001b60: 7d60 0a0a 2323 2323 2054 6162 6c65 206c  }`..#### Table l
-00001b70: 6f63 6174 696f 6e0a 0a54 6865 206c 6f63  ocation..The loc
-00001b80: 6174 696f 6e20 696e 2077 6869 6368 2061  ation in which a
-00001b90: 2074 6162 6c65 2069 7320 7361 7665 6420   table is saved 
-00001ba0: 6973 2064 6574 6572 6d69 6e65 6420 6279  is determined by
-00001bb0: 3a0a 0a31 2e20 4966 2060 6578 7465 726e  :..1. If `extern
-00001bc0: 616c 5f6c 6f63 6174 696f 6e60 2069 7320  al_location` is 
-00001bd0: 6465 6669 6e65 642c 2074 6861 7420 7661  defined, that va
-00001be0: 6c75 6520 6973 2075 7365 642e 0a32 2e20  lue is used..2. 
-00001bf0: 4966 2060 7333 5f64 6174 615f 6469 7260  If `s3_data_dir`
-00001c00: 2069 7320 6465 6669 6e65 642c 2074 6865   is defined, the
-00001c10: 2070 6174 6820 6973 2064 6574 6572 6d69   path is determi
-00001c20: 6e65 6420 6279 2074 6861 7420 616e 6420  ned by that and 
-00001c30: 6073 335f 6461 7461 5f6e 616d 696e 6760  `s3_data_naming`
-00001c40: 0a33 2e20 4966 2060 7333 5f64 6174 615f  .3. If `s3_data_
-00001c50: 6469 7260 2069 7320 6e6f 7420 6465 6669  dir` is not defi
-00001c60: 6e65 6420 6461 7461 2069 7320 7374 6f72  ned data is stor
-00001c70: 6564 2075 6e64 6572 2060 7333 5f73 7461  ed under `s3_sta
-00001c80: 6769 6e67 5f64 6972 2f74 6162 6c65 732f  ging_dir/tables/
-00001c90: 600a 0a48 6572 6520 616c 6c20 7468 6520  `..Here all the 
-00001ca0: 6f70 7469 6f6e 7320 6176 6169 6c61 626c  options availabl
-00001cb0: 6520 666f 7220 6073 335f 6461 7461 5f6e  e for `s3_data_n
-00001cc0: 616d 696e 6760 3a0a 2a20 6075 7569 6460  aming`:.* `uuid`
-00001cd0: 3a20 607b 7333 5f64 6174 615f 6469 727d  : `{s3_data_dir}
-00001ce0: 2f7b 7575 6964 3428 297d 2f60 0a2a 2060  /{uuid4()}/`.* `
-00001cf0: 7461 626c 655f 7461 626c 6560 3a20 607b  table_table`: `{
-00001d00: 7333 5f64 6174 615f 6469 727d 2f7b 7461  s3_data_dir}/{ta
-00001d10: 626c 657d 2f60 0a2a 2060 7461 626c 655f  ble}/`.* `table_
-00001d20: 756e 6971 7565 603a 2060 7b73 335f 6461  unique`: `{s3_da
-00001d30: 7461 5f64 6972 7d2f 7b74 6162 6c65 7d2f  ta_dir}/{table}/
-00001d40: 7b75 7569 6434 2829 7d2f 600a 2a20 6073  {uuid4()}/`.* `s
-00001d50: 6368 656d 615f 7461 626c 6560 3a20 607b  chema_table`: `{
-00001d60: 7333 5f64 6174 615f 6469 727d 2f7b 7363  s3_data_dir}/{sc
-00001d70: 6865 6d61 7d2f 7b74 6162 6c65 7d2f 600a  hema}/{table}/`.
-00001d80: 2a20 6073 335f 6461 7461 5f6e 616d 696e  * `s3_data_namin
-00001d90: 673d 7363 6865 6d61 5f74 6162 6c65 5f75  g=schema_table_u
-00001da0: 6e69 7175 6560 3a20 607b 7333 5f64 6174  nique`: `{s3_dat
-00001db0: 615f 6469 727d 2f7b 7363 6865 6d61 7d2f  a_dir}/{schema}/
-00001dc0: 7b74 6162 6c65 7d2f 7b75 7569 6434 2829  {table}/{uuid4()
-00001dd0: 7d2f 600a 0a49 7427 7320 706f 7373 6962  }/`..It's possib
-00001de0: 6c65 2074 6f20 7365 7420 7468 6520 6073  le to set the `s
-00001df0: 335f 6461 7461 5f6e 616d 696e 6760 2067  3_data_naming` g
-00001e00: 6c6f 6261 6c6c 7920 696e 2074 6865 2074  lobally in the t
-00001e10: 6172 6765 7420 7072 6f66 696c 652c 206f  arget profile, o
-00001e20: 7220 6f76 6572 7772 6974 6520 7468 6520  r overwrite the 
-00001e30: 7661 6c75 6520 696e 2074 6865 2074 6162  value in the tab
-00001e40: 6c65 2063 6f6e 6669 672c 0a6f 7220 7365  le config,.or se
-00001e50: 7474 696e 6720 7570 2074 6865 2076 616c  tting up the val
-00001e60: 7565 2066 6f72 2067 726f 7570 7320 6f66  ue for groups of
-00001e70: 206d 6f64 656c 2069 6e20 6462 745f 7072   model in dbt_pr
-00001e80: 6f6a 6563 742e 796d 6c2e 0a0a 3e20 4e6f  oject.yml...> No
-00001e90: 7465 3a20 7768 656e 2075 7369 6e67 2061  te: when using a
-00001ea0: 2077 6f72 6b20 6772 6f75 7020 7769 7468   work group with
-00001eb0: 2061 2064 6566 6175 6c74 206f 7574 7075   a default outpu
-00001ec0: 7420 6c6f 6361 7469 6f6e 2063 6f6e 6669  t location confi
-00001ed0: 6775 7265 642c 2060 7333 5f64 6174 615f  gured, `s3_data_
-00001ee0: 6e61 6d69 6e67 6020 616e 6420 616e 7920  naming` and any 
-00001ef0: 636f 6e66 6967 7572 6564 2062 7563 6b65  configured bucke
-00001f00: 7473 2061 7265 2069 676e 6f72 6564 2061  ts are ignored a
-00001f10: 6e64 2074 6865 206c 6f63 6174 696f 6e20  nd the location 
-00001f20: 636f 6e66 6967 7572 6564 2069 6e20 7468  configured in th
-00001f30: 6520 776f 726b 2067 726f 7570 2069 7320  e work group is 
-00001f40: 7573 6564 2e0a 0a0a 2323 2323 2049 6e63  used....#### Inc
-00001f50: 7265 6d65 6e74 616c 206d 6f64 656c 730a  remental models.
-00001f60: 0a53 7570 706f 7274 2066 6f72 205b 696e  .Support for [in
-00001f70: 6372 656d 656e 7461 6c20 6d6f 6465 6c73  cremental models
-00001f80: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
-00001f90: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
-00001fa0: 7569 6c64 2f69 6e63 7265 6d65 6e74 616c  uild/incremental
-00001fb0: 2d6d 6f64 656c 7329 2e0a 0a54 6865 7365  -models)...These
-00001fc0: 2073 7472 6174 6567 6965 7320 6172 6520   strategies are 
-00001fd0: 7375 7070 6f72 7465 643a 0a0a 2a20 6069  supported:..* `i
-00001fe0: 6e73 6572 745f 6f76 6572 7772 6974 6560  nsert_overwrite`
-00001ff0: 2028 6465 6661 756c 7429 3a20 5468 6520   (default): The 
-00002000: 696e 7365 7274 206f 7665 7277 7269 7465  insert overwrite
-00002010: 2073 7472 6174 6567 7920 6465 6c65 7465   strategy delete
-00002020: 7320 7468 6520 6f76 6572 6c61 7070 696e  s the overlappin
-00002030: 6720 7061 7274 6974 696f 6e73 2066 726f  g partitions fro
-00002040: 6d20 7468 6520 6465 7374 696e 6174 696f  m the destinatio
-00002050: 6e0a 7461 626c 652c 2061 6e64 2074 6865  n.table, and the
-00002060: 6e20 696e 7365 7274 7320 7468 6520 6e65  n inserts the ne
-00002070: 7720 7265 636f 7264 7320 6672 6f6d 2074  w records from t
-00002080: 6865 2073 6f75 7263 652e 2054 6869 7320  he source. This 
-00002090: 7374 7261 7465 6779 2064 6570 656e 6473  strategy depends
-000020a0: 206f 6e20 7468 6520 6070 6172 7469 7469   on the `partiti
-000020b0: 6f6e 6564 5f62 7960 206b 6579 776f 7264  oned_by` keyword
-000020c0: 2120 4966 206e 6f0a 7061 7274 6974 696f  ! If no.partitio
-000020d0: 6e73 2061 7265 2064 6566 696e 6564 2c20  ns are defined, 
-000020e0: 6462 7420 7769 6c6c 2066 616c 6c20 6261  dbt will fall ba
-000020f0: 636b 2074 6f20 7468 6520 6061 7070 656e  ck to the `appen
-00002100: 6460 2073 7472 6174 6567 792e 0a2a 2060  d` strategy..* `
-00002110: 6170 7065 6e64 603a 2049 6e73 6572 7420  append`: Insert 
-00002120: 6e65 7720 7265 636f 7264 7320 7769 7468  new records with
-00002130: 6f75 7420 7570 6461 7469 6e67 2c20 6465  out updating, de
-00002140: 6c65 7469 6e67 206f 7220 6f76 6572 7772  leting or overwr
-00002150: 6974 696e 6720 616e 7920 6578 6973 7469  iting any existi
-00002160: 6e67 2064 6174 612e 2054 6865 7265 206d  ng data. There m
-00002170: 6967 6874 2062 6520 6475 706c 6963 6174  ight be duplicat
-00002180: 650a 6461 7461 2028 652e 672e 2067 7265  e.data (e.g. gre
-00002190: 6174 2066 6f72 206c 6f67 206f 7220 6869  at for log or hi
-000021a0: 7374 6f72 6963 616c 2064 6174 6129 2e0a  storical data)..
-000021b0: 2a20 606d 6572 6765 603a 2043 6f6e 6469  * `merge`: Condi
-000021c0: 7469 6f6e 616c 6c79 2075 7064 6174 6573  tionally updates
-000021d0: 2c20 6465 6c65 7465 732c 206f 7220 696e  , deletes, or in
-000021e0: 7365 7274 7320 726f 7773 2069 6e74 6f20  serts rows into 
-000021f0: 616e 2049 6365 6265 7267 2074 6162 6c65  an Iceberg table
-00002200: 2e20 5573 6564 2069 6e20 636f 6d62 696e  . Used in combin
-00002210: 6174 696f 6e20 7769 7468 2060 756e 6971  ation with `uniq
-00002220: 7565 5f6b 6579 602e 0a4f 6e6c 7920 6176  ue_key`..Only av
-00002230: 6169 6c61 626c 6520 7768 656e 2075 7369  ailable when usi
-00002240: 6e67 2049 6365 6265 7267 2e0a 0a23 2323  ng Iceberg...###
-00002250: 2320 4f6e 2073 6368 656d 6120 6368 616e  # On schema chan
-00002260: 6765 0a0a 606f 6e5f 7363 6865 6d61 5f63  ge..`on_schema_c
-00002270: 6861 6e67 6560 2069 7320 616e 206f 7074  hange` is an opt
-00002280: 696f 6e20 746f 2072 6566 6c65 6374 2063  ion to reflect c
-00002290: 6861 6e67 6573 206f 6620 7363 6865 6d61  hanges of schema
-000022a0: 2069 6e20 696e 6372 656d 656e 7461 6c20   in incremental 
-000022b0: 6d6f 6465 6c73 2e0a 5468 6520 666f 6c6c  models..The foll
-000022c0: 6f77 696e 6720 6f70 7469 6f6e 7320 6172  owing options ar
-000022d0: 6520 7375 7070 6f72 7465 643a 0a2a 2060  e supported:.* `
-000022e0: 6967 6e6f 7265 6020 2864 6566 6175 6c74  ignore` (default
-000022f0: 290a 2a20 6066 6169 6c60 0a2a 2060 6170  ).* `fail`.* `ap
-00002300: 7065 6e64 5f6e 6577 5f63 6f6c 756d 6e73  pend_new_columns
-00002310: 600a 2a20 6073 796e 635f 616c 6c5f 636f  `.* `sync_all_co
-00002320: 6c75 6d6e 7360 0a0a 496e 2064 6574 6169  lumns`..In detai
-00002330: 6c2c 2070 6c65 6173 6520 7265 6665 7220  l, please refer 
-00002340: 746f 205b 6462 7420 646f 6373 5d28 6874  to [dbt docs](ht
-00002350: 7470 733a 2f2f 646f 6373 2e67 6574 6462  tps://docs.getdb
-00002360: 742e 636f 6d2f 646f 6373 2f62 7569 6c64  t.com/docs/build
-00002370: 2f69 6e63 7265 6d65 6e74 616c 2d6d 6f64  /incremental-mod
-00002380: 656c 7323 7768 6174 2d69 662d 7468 652d  els#what-if-the-
-00002390: 636f 6c75 6d6e 732d 6f66 2d6d 792d 696e  columns-of-my-in
-000023a0: 6372 656d 656e 7461 6c2d 6d6f 6465 6c2d  cremental-model-
-000023b0: 6368 616e 6765 292e 0a0a 0a23 2323 2320  change)....#### 
-000023c0: 4963 6562 6572 670a 0a54 6865 2061 6461  Iceberg..The ada
-000023d0: 7074 6572 2073 7570 706f 7274 7320 7461  pter supports ta
-000023e0: 626c 6520 6d61 7465 7269 616c 697a 6174  ble materializat
-000023f0: 696f 6e20 666f 7220 4963 6562 6572 672e  ion for Iceberg.
-00002400: 0a0a 546f 2067 6574 2073 7461 7274 6564  ..To get started
-00002410: 206a 7573 7420 6164 6420 7468 6973 2061   just add this a
-00002420: 7320 796f 7572 206d 6f64 656c 3a0a 6060  s your model:.``
-00002430: 600a 7b7b 2063 6f6e 6669 6728 0a20 2020  `.{{ config(.   
-00002440: 206d 6174 6572 6961 6c69 7a65 643d 2774   materialized='t
-00002450: 6162 6c65 272c 0a20 2020 2074 6162 6c65  able',.    table
-00002460: 5f74 7970 653d 2769 6365 6265 7267 272c  _type='iceberg',
-00002470: 0a20 2020 2066 6f72 6d61 743d 2770 6172  .    format='par
-00002480: 7175 6574 272c 0a20 2020 2070 6172 7469  quet',.    parti
-00002490: 7469 6f6e 6564 5f62 793d 5b27 6275 636b  tioned_by=['buck
-000024a0: 6574 2875 7365 725f 6964 2c20 3529 275d  et(user_id, 5)']
-000024b0: 2c0a 2020 2020 7461 626c 655f 7072 6f70  ,.    table_prop
-000024c0: 6572 7469 6573 3d7b 0a20 2020 2009 276f  erties={.    .'o
-000024d0: 7074 696d 697a 655f 7265 7772 6974 655f  ptimize_rewrite_
-000024e0: 6465 6c65 7465 5f66 696c 655f 7468 7265  delete_file_thre
-000024f0: 7368 6f6c 6427 3a20 2732 270a 2020 2020  shold': '2'.    
-00002500: 097d 0a29 207d 7d0a 0a53 454c 4543 540a  .}.) }}..SELECT.
-00002510: 0927 4127 2041 5320 7573 6572 5f69 642c  .'A' AS user_id,
-00002520: 0a09 2770 6927 2041 5320 6e61 6d65 2c0a  ..'pi' AS name,.
-00002530: 0927 6163 7469 7665 2720 4153 2073 7461  .'active' AS sta
-00002540: 7475 732c 0a09 3137 2e38 3920 4153 2063  tus,..17.89 AS c
-00002550: 6f73 742c 0a09 3120 4153 2071 7561 6e74  ost,..1 AS quant
-00002560: 6974 792c 0a09 3130 3030 3030 3030 3020  ity,..100000000 
-00002570: 4153 2071 7561 6e74 6974 795f 6269 672c  AS quantity_big,
-00002580: 0a09 6375 7272 656e 745f 6461 7465 2041  ..current_date A
-00002590: 5320 6d79 5f64 6174 650a 6060 600a 0a49  S my_date.```..I
-000025a0: 6365 6265 7267 2073 7570 706f 7274 7320  ceberg supports 
-000025b0: 6275 636b 6574 696e 6720 6173 2068 6964  bucketing as hid
-000025c0: 6465 6e20 7061 7274 6974 696f 6e73 2c20  den partitions, 
-000025d0: 7468 6572 6566 6f72 6520 7573 6520 7468  therefore use th
-000025e0: 6520 6070 6172 7469 7469 6f6e 6564 5f62  e `partitioned_b
-000025f0: 7960 2063 6f6e 6669 6720 746f 2061 6464  y` config to add
-00002600: 2073 7065 6369 6669 6320 6275 636b 6574   specific bucket
-00002610: 696e 6720 636f 6e64 6974 696f 6e73 2e0a  ing conditions..
-00002620: 0a49 6365 6265 7267 2073 7570 706f 7274  .Iceberg support
-00002630: 7320 7365 7665 7261 6c20 7461 626c 6520  s several table 
-00002640: 666f 726d 6174 7320 666f 7220 6461 7461  formats for data
-00002650: 203a 2060 5041 5251 5545 5460 2c20 6041   : `PARQUET`, `A
-00002660: 5652 4f60 2061 6e64 2060 4f52 4360 2e0a  VRO` and `ORC`..
-00002670: 0a49 7420 6973 2070 6f73 7369 626c 6520  .It is possible 
-00002680: 746f 2075 7365 2069 6365 6265 7267 2069  to use iceberg i
-00002690: 6e20 616e 2069 6e63 7265 6d65 6e74 616c  n an incremental
-000026a0: 2066 6173 6869 6f6e 2c20 7370 6563 6966   fashion, specif
-000026b0: 6963 616c 6c79 2032 2073 7472 6174 6567  ically 2 strateg
-000026c0: 6965 7320 6172 6520 7375 7070 6f72 7465  ies are supporte
-000026d0: 643a 0a2a 2060 6170 7065 6e64 603a 206e  d:.* `append`: n
-000026e0: 6577 2072 6563 6f72 6473 2061 7265 2061  ew records are a
-000026f0: 7070 656e 6465 6420 746f 2074 6865 2074  ppended to the t
-00002700: 6162 6c65 2c20 7468 6973 2063 616e 206c  able, this can l
-00002710: 6561 6420 746f 2064 7570 6c69 6361 7465  ead to duplicate
-00002720: 730a 2a20 606d 6572 6765 603a 206d 7573  s.* `merge`: mus
-00002730: 7420 6265 2075 7365 6420 696e 2063 6f6d  t be used in com
-00002740: 6269 6e61 7469 6f6e 2077 6974 6820 6075  bination with `u
-00002750: 6e69 7175 655f 6b65 7960 2061 6e64 2069  nique_key` and i
-00002760: 7427 7320 6f6e 6c79 2061 7661 696c 6162  t's only availab
-00002770: 6c65 2077 6974 6820 456e 6769 6e65 2076  le with Engine v
-00002780: 6572 7369 6f6e 2033 2e0a 2020 2049 7420  ersion 3..   It 
-00002790: 7065 7266 6f72 6d73 2061 6e20 7570 7365  performs an upse
-000027a0: 7274 2c20 6e65 7720 7265 636f 7264 2061  rt, new record a
-000027b0: 7265 2061 6464 6564 2c20 616e 6420 7265  re added, and re
-000027c0: 636f 7264 2061 6c72 6561 6479 2065 7869  cord already exi
-000027d0: 7374 696e 6720 6172 6520 7570 6461 7465  sting are update
-000027e0: 640a 0a23 2323 2320 4869 6768 2061 7661  d..#### High ava
-000027f0: 696c 6162 6c65 2074 6162 6c65 206d 6174  ilable table mat
-00002800: 6572 6961 6c69 7a61 7469 6f6e 0a54 6865  erialization.The
-00002810: 2063 7572 7265 6e74 2069 6d70 6c65 6d65   current impleme
-00002820: 6e74 6174 696f 6e20 6f66 2074 6865 2074  ntation of the t
-00002830: 6162 6c65 206d 6174 6572 6961 6c69 7a61  able materializa
-00002840: 7469 6f6e 2063 616e 206c 6561 6420 746f  tion can lead to
-00002850: 2064 6f77 6e74 696d 652c 2061 7320 7461   downtime, as ta
-00002860: 7267 6574 2074 6162 6c65 2069 7320 6472  rget table is dr
-00002870: 6f70 7065 6420 616e 6420 7265 2d63 7265  opped and re-cre
-00002880: 6174 6564 2e0a 546f 2068 6176 6520 7468  ated..To have th
-00002890: 6520 6c65 7373 2064 6573 7472 7563 7469  e less destructi
-000028a0: 7665 2062 6568 6176 696f 7220 6974 2773  ve behavior it's
-000028b0: 2070 6f73 7369 626c 6520 746f 2075 7365   possible to use
-000028c0: 2060 7461 626c 653d 2774 6162 6c65 5f68   `table='table_h
-000028d0: 6976 655f 6861 2760 206d 6174 6572 6961  ive_ha'` materia
-000028e0: 6c69 7a61 7469 6f6e 2e0a 2a2a 7461 626c  lization..**tabl
-000028f0: 655f 6869 7665 5f68 612a 2a20 6c65 7665  e_hive_ha** leve
-00002900: 7261 6765 2074 6865 2074 6162 6c65 2076  rage the table v
-00002910: 6572 7369 6f6e 7320 6665 6174 7572 6520  ersions feature 
-00002920: 6f66 2067 6c75 6520 6361 7461 6c6f 672c  of glue catalog,
-00002930: 2063 7265 6174 696e 6720 6120 746d 7020   creating a tmp 
-00002940: 7461 626c 6520 616e 6420 7377 6170 7069  table and swappi
-00002950: 6e67 0a74 6865 2074 6172 6765 7420 7461  ng.the target ta
-00002960: 626c 6520 746f 2074 6865 206c 6f63 6174  ble to the locat
-00002970: 696f 6e20 6f66 2074 6865 2074 6d70 2074  ion of the tmp t
-00002980: 6162 6c65 2e0a 5468 6973 206d 6174 6572  able..This mater
-00002990: 6961 6c69 7a61 7469 6f6e 2069 7320 6f6e  ialization is on
-000029a0: 6c79 2061 7661 696c 6162 6c65 2066 6f72  ly available for
-000029b0: 2060 7461 626c 655f 7479 7065 3d68 6976   `table_type=hiv
-000029c0: 6560 2061 6e64 2072 6571 7569 7265 7320  e` and requires 
-000029d0: 7573 696e 6720 756e 6971 7565 206c 6f63  using unique loc
-000029e0: 6174 696f 6e73 2e0a 0a60 6060 0a7b 7b20  ations...```.{{ 
-000029f0: 636f 6e66 6967 280a 2020 2020 6d61 7465  config(.    mate
-00002a00: 7269 616c 697a 6564 3d27 7461 626c 655f  rialized='table_
-00002a10: 6869 7665 5f68 6127 2c0a 2020 2020 666f  hive_ha',.    fo
-00002a20: 726d 6174 3d27 7061 7271 7565 7427 2c0a  rmat='parquet',.
-00002a30: 2020 2020 7061 7274 6974 696f 6e5f 6279      partition_by
-00002a40: 3d5b 2773 7461 7475 7327 5d2c 0a20 2020  =['status'],.   
-00002a50: 2073 335f 6461 7461 5f6e 616d 696e 673d   s3_data_naming=
-00002a60: 2774 6162 6c65 5f75 6e69 7175 6527 0a29  'table_unique'.)
-00002a70: 207d 7d0a 0a0a 7365 6c65 6374 0a20 2027   }}...select.  '
-00002a80: 6127 2061 7320 7573 6572 5f69 642c 0a20  a' as user_id,. 
-00002a90: 2027 7069 2720 6173 2075 7365 725f 6e61   'pi' as user_na
-00002aa0: 6d65 2c0a 2020 2761 6374 6976 6527 2061  me,.  'active' a
-00002ab0: 7320 7374 6174 7573 0a75 6e69 6f6e 2061  s status.union a
-00002ac0: 6c6c 0a73 656c 6563 740a 2020 2762 2720  ll.select.  'b' 
-00002ad0: 6173 2075 7365 725f 6964 2c0a 2020 2773  as user_id,.  's
-00002ae0: 6827 2061 7320 7573 6572 5f6e 616d 652c  h' as user_name,
-00002af0: 0a20 2027 6469 7361 626c 6564 2720 6173  .  'disabled' as
-00002b00: 2073 7461 7475 730a 6060 600a 0a42 7920   status.```..By 
-00002b10: 6465 6661 756c 742c 2074 6865 206d 6174  default, the mat
-00002b20: 6572 6961 6c69 7a61 7469 6f6e 206b 6565  erialization kee
-00002b30: 7073 2074 6865 206c 6173 7420 3420 7461  ps the last 4 ta
-00002b40: 626c 6520 7665 7273 696f 6e73 2c20 796f  ble versions, yo
-00002b50: 7520 6361 6e20 6368 616e 6765 2069 7420  u can change it 
-00002b60: 7468 6174 2073 6574 7469 6e67 2060 7665  that setting `ve
-00002b70: 7273 696f 6e73 5f74 6f5f 6b65 6570 602e  rsions_to_keep`.
-00002b80: 0a0a 2323 2323 2320 4b6e 6f77 6e20 6973  ..##### Known is
-00002b90: 7375 6573 0a2a 2057 6865 6e20 7377 6170  sues.* When swap
-00002ba0: 7069 6e67 2066 726f 6d20 6120 7461 626c  ping from a tabl
-00002bb0: 6520 7769 7468 2070 6172 7469 7469 6f6e  e with partition
-00002bc0: 7320 746f 2061 2074 6162 6c65 2077 6974  s to a table wit
-00002bd0: 686f 7574 2028 616e 6420 7468 6520 6f74  hout (and the ot
-00002be0: 6865 7220 7761 7920 6172 6f75 6e64 292c  her way around),
-00002bf0: 2074 6865 7265 2063 6f75 6c64 2062 6520   there could be 
-00002c00: 6120 6c69 7474 6c65 2064 6f77 6e74 696d  a little downtim
-00002c10: 652e 0a20 2049 6e20 6361 7365 2068 6967  e..  In case hig
-00002c20: 6820 7065 7266 6f72 6d61 6e63 6573 2061  h performances a
-00002c30: 7265 206e 6565 6465 6420 636f 6e73 6964  re needed consid
-00002c40: 6572 2062 7563 6b65 7469 6e67 2069 6e73  er bucketing ins
-00002c50: 7465 6164 206f 6620 7061 7274 6974 696f  tead of partitio
-00002c60: 6e73 0a2a 2042 7920 6465 6661 756c 742c  ns.* By default,
-00002c70: 2047 6c75 6520 2264 7570 6c69 6361 7465   Glue "duplicate
-00002c80: 2220 7468 6520 7665 7273 696f 6e73 2069  " the versions i
-00002c90: 6e74 6572 6e61 6c6c 792c 2073 6f20 7468  nternally, so th
-00002ca0: 6520 6c61 7374 2032 2076 6572 7369 6f6e  e last 2 version
-00002cb0: 7320 6f66 2061 2074 6162 6c65 2070 6f69  s of a table poi
-00002cc0: 6e74 2074 6f20 7468 6520 7361 6d65 206c  nt to the same l
-00002cd0: 6f63 6174 696f 6e0a 2a20 4974 2773 2072  ocation.* It's r
-00002ce0: 6563 6f6d 6d65 6e64 6564 2074 6f20 6861  ecommended to ha
-00002cf0: 7665 2076 6572 7369 6f6e 735f 746f 5f6b  ve versions_to_k
-00002d00: 6565 703e 3d20 342c 2061 7320 7468 6973  eep>= 4, as this
-00002d10: 2077 696c 6c20 6176 6f69 6420 746f 2068   will avoid to h
-00002d20: 6176 6520 7468 6520 6f6c 6465 7220 6c6f  ave the older lo
-00002d30: 6361 7469 6f6e 2072 656d 6f76 6564 0a2a  cation removed.*
-00002d40: 2054 6865 206d 6163 726f 2061 7468 656e   The macro athen
-00002d50: 615f 5f65 6e64 5f6f 665f 7469 6d65 206e  a__end_of_time n
-00002d60: 6565 6473 2074 6f20 6265 206f 7665 7277  eeds to be overw
-00002d70: 7269 7474 656e 2062 7920 7468 6520 7573  ritten by the us
-00002d80: 6572 2069 6620 7573 696e 6720 4174 6865  er if using Athe
-00002d90: 6e61 2076 3320 7369 6e63 6520 6974 2072  na v3 since it r
-00002da0: 6571 7569 7265 7320 6120 7072 6563 6973  equires a precis
-00002db0: 696f 6e20 7061 7261 6d65 7465 7220 666f  ion parameter fo
-00002dc0: 7220 7469 6d65 7374 616d 7073 0a0a 0a23  r timestamps...#
-00002dd0: 2323 2053 6e61 7073 686f 7473 0a0a 5468  ## Snapshots..Th
-00002de0: 6520 6164 6170 7465 7220 7375 7070 6f72  e adapter suppor
-00002df0: 7473 2073 6e61 7073 686f 7420 6d61 7465  ts snapshot mate
-00002e00: 7269 616c 697a 6174 696f 6e2e 2049 7420  rialization. It 
-00002e10: 7375 7070 6f72 7473 2062 6f74 6820 7469  supports both ti
-00002e20: 6d65 7374 616d 7020 616e 6420 6368 6563  mestamp and chec
-00002e30: 6b20 7374 7261 7465 6779 2e20 546f 2063  k strategy. To c
-00002e40: 7265 6174 6520 6120 736e 6170 7368 6f74  reate a snapshot
-00002e50: 2063 7265 6174 6520 6120 736e 6170 7368   create a snapsh
-00002e60: 6f74 2066 696c 6520 696e 2074 6865 2073  ot file in the s
-00002e70: 6e61 7073 686f 7473 2064 6972 6563 746f  napshots directo
-00002e80: 7279 2e20 4966 2064 6972 6563 746f 7279  ry. If directory
-00002e90: 2064 6f65 7320 6e6f 7420 6578 6973 7420   does not exist 
-00002ea0: 6372 6561 7465 206f 6e65 2e0a 0a23 2323  create one...###
-00002eb0: 2320 5469 6d65 7374 616d 7020 7374 7261  # Timestamp stra
-00002ec0: 7465 6779 0a0a 546f 2075 7365 2074 6865  tegy..To use the
-00002ed0: 2074 696d 6573 7461 6d70 2073 7472 6174   timestamp strat
-00002ee0: 6567 7920 7265 6665 7220 746f 2074 6865  egy refer to the
-00002ef0: 205b 6462 7420 646f 6373 5d28 6874 7470   [dbt docs](http
-00002f00: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
-00002f10: 636f 6d2f 646f 6373 2f62 7569 6c64 2f73  com/docs/build/s
-00002f20: 6e61 7073 686f 7473 2374 696d 6573 7461  napshots#timesta
-00002f30: 6d70 2d73 7472 6174 6567 792d 7265 636f  mp-strategy-reco
-00002f40: 6d6d 656e 6465 6429 0a0a 2323 2323 2043  mmended)..#### C
-00002f50: 6865 636b 2073 7472 6174 6567 790a 0a54  heck strategy..T
-00002f60: 6f20 7573 6520 7468 6520 6368 6563 6b20  o use the check 
-00002f70: 7374 7261 7465 6779 2072 6566 6572 2074  strategy refer t
-00002f80: 6f20 7468 6520 5b64 6274 2064 6f63 735d  o the [dbt docs]
-00002f90: 2868 7474 7073 3a2f 2f64 6f63 732e 6765  (https://docs.ge
-00002fa0: 7464 6274 2e63 6f6d 2f64 6f63 732f 6275  tdbt.com/docs/bu
-00002fb0: 696c 642f 736e 6170 7368 6f74 7323 6368  ild/snapshots#ch
-00002fc0: 6563 6b2d 7374 7261 7465 6779 290a 0a23  eck-strategy)..#
-00002fd0: 2323 2320 4861 7264 2d64 656c 6574 6573  ### Hard-deletes
-00002fe0: 0a0a 5468 6520 6d61 7465 7269 616c 697a  ..The materializ
-00002ff0: 6174 696f 6e20 616c 736f 2073 7570 706f  ation also suppo
-00003000: 7274 7320 696e 7661 6c69 6461 7469 6e67  rts invalidating
-00003010: 2068 6172 6420 6465 6c65 7465 732e 2043   hard deletes. C
-00003020: 6865 636b 2074 6865 205b 646f 6373 5d28  heck the [docs](
-00003030: 6874 7470 733a 2f2f 646f 6373 2e67 6574  https://docs.get
-00003040: 6462 742e 636f 6d2f 646f 6373 2f62 7569  dbt.com/docs/bui
-00003050: 6c64 2f73 6e61 7073 686f 7473 2368 6172  ld/snapshots#har
-00003060: 642d 6465 6c65 7465 732d 6f70 742d 696e  d-deletes-opt-in
-00003070: 2920 746f 2075 6e64 6572 7374 616e 6420  ) to understand 
-00003080: 7573 6167 652e 0a0a 2323 2320 576f 726b  usage...### Work
-00003090: 696e 6720 6578 616d 706c 650a 0a73 6565  ing example..see
-000030a0: 6420 6669 6c65 202d 2065 6d70 6c6f 7965  d file - employe
-000030b0: 6e74 5f69 6e64 6963 6174 6f72 735f 6e6f  nt_indicators_no
-000030c0: 7665 6d62 6572 5f32 3032 325f 6373 765f  vember_2022_csv_
-000030d0: 7461 626c 6573 2e63 7376 0a60 6060 0a53  tables.csv.```.S
-000030e0: 6572 6965 735f 7265 6665 7265 6e63 652c  eries_reference,
-000030f0: 5065 7269 6f64 2c44 6174 615f 7661 6c75  Period,Data_valu
-00003100: 652c 5375 7070 7265 7373 6564 0a4d 4549  e,Suppressed.MEI
-00003110: 4d2e 5331 5741 2c31 3939 392e 3034 2c38  M.S1WA,1999.04,8
-00003120: 3032 3637 2c0a 4d45 494d 2e53 3157 412c  0267,.MEIM.S1WA,
-00003130: 3139 3939 2e30 352c 3730 3830 332c 0a4d  1999.05,70803,.M
-00003140: 4549 4d2e 5331 5741 2c31 3939 392e 3036  EIM.S1WA,1999.06
-00003150: 2c36 3537 3932 2c0a 4d45 494d 2e53 3157  ,65792,.MEIM.S1W
-00003160: 412c 3139 3939 2e30 372c 3636 3139 342c  A,1999.07,66194,
-00003170: 0a4d 4549 4d2e 5331 5741 2c31 3939 392e  .MEIM.S1WA,1999.
-00003180: 3038 2c36 3732 3539 2c0a 4d45 494d 2e53  08,67259,.MEIM.S
-00003190: 3157 412c 3139 3939 2e30 392c 3639 3639  1WA,1999.09,6969
-000031a0: 312c 0a4d 4549 4d2e 5331 5741 2c31 3939  1,.MEIM.S1WA,199
-000031b0: 392e 312c 3732 3437 352c 0a4d 4549 4d2e  9.1,72475,.MEIM.
-000031c0: 5331 5741 2c31 3939 392e 3131 2c37 3932  S1WA,1999.11,792
-000031d0: 3633 2c0a 4d45 494d 2e53 3157 412c 3139  63,.MEIM.S1WA,19
-000031e0: 3939 2e31 322c 3836 3534 302c 0a4d 4549  99.12,86540,.MEI
-000031f0: 4d2e 5331 5741 2c32 3030 302e 3031 2c38  M.S1WA,2000.01,8
-00003200: 3235 3532 2c0a 4d45 494d 2e53 3157 412c  2552,.MEIM.S1WA,
-00003210: 3230 3030 2e30 322c 3831 3730 392c 0a4d  2000.02,81709,.M
-00003220: 4549 4d2e 5331 5741 2c32 3030 302e 3033  EIM.S1WA,2000.03
-00003230: 2c38 3431 3236 2c0a 4d45 494d 2e53 3157  ,84126,.MEIM.S1W
-00003240: 412c 3230 3030 2e30 342c 3737 3038 392c  A,2000.04,77089,
-00003250: 0a4d 4549 4d2e 5331 5741 2c32 3030 302e  .MEIM.S1WA,2000.
-00003260: 3035 2c37 3338 3131 2c0a 4d45 494d 2e53  05,73811,.MEIM.S
-00003270: 3157 412c 3230 3030 2e30 362c 3730 3037  1WA,2000.06,7007
-00003280: 302c 0a4d 4549 4d2e 5331 5741 2c32 3030  0,.MEIM.S1WA,200
-00003290: 302e 3037 2c36 3938 3733 2c0a 4d45 494d  0.07,69873,.MEIM
-000032a0: 2e53 3157 412c 3230 3030 2e30 382c 3731  .S1WA,2000.08,71
-000032b0: 3436 382c 0a4d 4549 4d2e 5331 5741 2c32  468,.MEIM.S1WA,2
-000032c0: 3030 302e 3039 2c37 3234 3632 2c0a 4d45  000.09,72462,.ME
-000032d0: 494d 2e53 3157 412c 3230 3030 2e31 2c37  IM.S1WA,2000.1,7
-000032e0: 3438 3937 2c0a 6060 600a 0a6d 6f64 656c  4897,.```..model
-000032f0: 2e73 716c 0a60 6060 0a7b 7b20 636f 6e66  .sql.```.{{ conf
-00003300: 6967 280a 2020 2020 6d61 7465 7269 616c  ig(.    material
-00003310: 697a 6564 3d27 7461 626c 6527 0a29 207d  ized='table'.) }
-00003320: 7d0a 0a0a 5345 4c45 4354 0a20 2020 2052  }...SELECT.    R
-00003330: 4f57 5f4e 554d 4245 5228 2920 4f56 4552  OW_NUMBER() OVER
-00003340: 2028 2920 4153 2069 640a 2020 2020 2c20   () AS id.    , 
-00003350: 2a0a 2020 2020 2c20 6361 7374 2866 726f  *.    , cast(fro
-00003360: 6d5f 756e 6978 7469 6d65 2874 6f5f 756e  m_unixtime(to_un
-00003370: 6978 7469 6d65 286e 6f77 2829 2929 2061  ixtime(now())) a
-00003380: 7320 7469 6d65 7374 616d 7028 3629 2920  s timestamp(6)) 
-00003390: 4153 2072 6566 7265 7368 5f74 696d 6573  AS refresh_times
-000033a0: 7461 6d70 0a46 524f 4d20 7b7b 2072 6566  tamp.FROM {{ ref
-000033b0: 2827 656d 706c 6f79 6d65 6e74 5f69 6e64  ('employment_ind
-000033c0: 6963 6174 6f72 735f 6e6f 7665 6d62 6572  icators_november
-000033d0: 5f32 3032 325f 6373 765f 7461 626c 6573  _2022_csv_tables
-000033e0: 2729 207d 7d0a 6060 600a 0a74 696d 6573  ') }}.```..times
-000033f0: 7461 6d70 2073 7472 6174 6567 7920 2d20  tamp strategy - 
-00003400: 6d6f 6465 6c5f 736e 6170 7368 6f74 5f31  model_snapshot_1
-00003410: 0a0a 6060 600a 7b25 2073 6e61 7073 686f  ..```.{% snapsho
-00003420: 7420 6d6f 6465 6c5f 736e 6170 7368 6f74  t model_snapshot
-00003430: 5f31 2025 7d0a 0a7b 7b0a 2020 2020 636f  _1 %}..{{.    co
-00003440: 6e66 6967 280a 2020 2020 2020 7374 7261  nfig(.      stra
-00003450: 7465 6779 3d27 7469 6d65 7374 616d 7027  tegy='timestamp'
-00003460: 2c0a 2020 2020 2020 7570 6461 7465 645f  ,.      updated_
-00003470: 6174 3d27 7265 6672 6573 685f 7469 6d65  at='refresh_time
-00003480: 7374 616d 7027 2c0a 2020 2020 2020 756e  stamp',.      un
-00003490: 6971 7565 5f6b 6579 3d27 6964 270a 2020  ique_key='id'.  
-000034a0: 2020 290a 7d7d 0a0a 0a0a 5345 4c45 4354    ).}}....SELECT
-000034b0: 202a 0a0a 6672 6f6d 207b 7b20 7265 6628   *..from {{ ref(
-000034c0: 276d 6f64 656c 2729 207d 7d0a 0a7b 2520  'model') }}..{% 
-000034d0: 656e 6473 6e61 7073 686f 7420 257d 0a60  endsnapshot %}.`
-000034e0: 6060 0a0a 696e 7661 6c69 6461 7465 2068  ``..invalidate h
-000034f0: 6172 6420 6465 6c65 7465 7320 2d20 6d6f  ard deletes - mo
-00003500: 6465 6c5f 736e 6170 7368 6f74 5f32 0a60  del_snapshot_2.`
-00003510: 6060 0a7b 2520 736e 6170 7368 6f74 206d  ``.{% snapshot m
-00003520: 6f64 656c 5f73 6e61 7073 686f 745f 3220  odel_snapshot_2 
-00003530: 257d 0a0a 7b7b 0a20 2020 2063 6f6e 6669  %}..{{.    confi
-00003540: 670a 2020 2020 280a 2020 2020 2020 2020  g.    (.        
-00003550: 756e 6971 7565 5f6b 6579 3d27 6964 272c  unique_key='id',
-00003560: 0a20 2020 2020 2020 2073 7472 6174 6567  .        strateg
-00003570: 793d 2774 696d 6573 7461 6d70 272c 0a20  y='timestamp',. 
-00003580: 2020 2020 2020 2075 7064 6174 6564 5f61         updated_a
-00003590: 743d 2772 6566 7265 7368 5f74 696d 6573  t='refresh_times
-000035a0: 7461 6d70 272c 0a20 2020 2020 2020 2069  tamp',.        i
-000035b0: 6e76 616c 6964 6174 655f 6861 7264 5f64  nvalidate_hard_d
-000035c0: 656c 6574 6573 3d54 7275 652c 0a20 2020  eletes=True,.   
-000035d0: 2029 0a7d 7d0a 5345 4c45 4354 202a 2066   ).}}.SELECT * f
-000035e0: 726f 6d20 7b7b 2072 6566 2827 6d6f 6465  rom {{ ref('mode
-000035f0: 6c27 2920 7d7d 0a0a 7b25 2065 6e64 736e  l') }}..{% endsn
-00003600: 6170 7368 6f74 2025 7d0a 6060 600a 0a63  apshot %}.```..c
-00003610: 6865 636b 2073 7472 6174 6567 7920 2d20  heck strategy - 
-00003620: 6d6f 6465 6c5f 736e 6170 7368 6f74 5f33  model_snapshot_3
-00003630: 0a60 6060 0a7b 2520 736e 6170 7368 6f74  .```.{% snapshot
-00003640: 206d 6f64 656c 5f73 6e61 7073 686f 745f   model_snapshot_
-00003650: 3320 257d 0a0a 7b7b 0a20 2020 2063 6f6e  3 %}..{{.    con
-00003660: 6669 670a 2020 2020 280a 2020 2020 2020  fig.    (.      
-00003670: 2020 756e 6971 7565 5f6b 6579 3d27 6964    unique_key='id
-00003680: 272c 0a20 2020 2020 2020 2073 7472 6174  ',.        strat
-00003690: 6567 793d 2763 6865 636b 272c 0a20 2020  egy='check',.   
-000036a0: 2020 2020 2063 6865 636b 5f63 6f6c 733d       check_cols=
-000036b0: 5b27 7365 7269 6573 5f72 6566 6572 656e  ['series_referen
-000036c0: 6365 272c 2764 6174 615f 7661 6c75 6527  ce','data_value'
-000036d0: 5d0a 2020 2020 290a 7d7d 0a53 454c 4543  ].    ).}}.SELEC
-000036e0: 5420 2a20 6672 6f6d 207b 7b20 7265 6628  T * from {{ ref(
-000036f0: 276d 6f64 656c 2729 207d 7d0a 0a7b 2520  'model') }}..{% 
-00003700: 656e 6473 6e61 7073 686f 7420 257d 0a60  endsnapshot %}.`
-00003710: 6060 0a0a 2323 2320 4b6e 6f77 6e20 6973  ``..### Known is
-00003720: 7375 6573 0a0a 2a20 496e 6372 656d 656e  sues..* Incremen
-00003730: 7461 6c20 4963 6562 6572 6720 6d6f 6465  tal Iceberg mode
-00003740: 6c73 202d 2053 796e 6320 616c 6c20 636f  ls - Sync all co
-00003750: 6c75 6d6e 7320 6f6e 2073 6368 656d 6120  lumns on schema 
-00003760: 6368 616e 6765 2063 616e 2774 2072 656d  change can't rem
-00003770: 6f76 6520 636f 6c75 6d6e 7320 7573 6564  ove columns used
-00003780: 2061 7320 7061 7274 6974 696f 6e69 6e67   as partitioning
-00003790: 2e0a 5468 6520 6f6e 6c79 2077 6179 2c20  ..The only way, 
-000037a0: 6672 6f6d 2061 2064 6274 2070 6572 7370  from a dbt persp
-000037b0: 6563 7469 7665 2c20 6973 2074 6f20 646f  ective, is to do
-000037c0: 2061 2066 756c 6c2d 7265 6672 6573 6820   a full-refresh 
-000037d0: 6f66 2074 6865 2069 6e63 7265 6d65 6e74  of the increment
-000037e0: 616c 206d 6f64 656c 2e0a 0a2a 2054 6162  al model...* Tab
-000037f0: 6c65 732c 2073 6368 656d 6173 2061 6e64  les, schemas and
-00003800: 2064 6174 6162 6173 6520 7368 6f75 6c64   database should
-00003810: 206f 6e6c 7920 6265 206c 6f77 6572 6361   only be lowerca
-00003820: 7365 0a0a 2a20 496e 206f 7264 6572 2074  se..* In order t
-00003830: 6f20 6176 6f69 6420 706f 7465 6e74 6961  o avoid potentia
-00003840: 6c20 636f 6e66 6c69 6374 732c 206d 616b  l conflicts, mak
-00003850: 6520 7375 7265 205b 6064 6274 2d61 7468  e sure [`dbt-ath
-00003860: 656e 612d 6164 6170 7465 7260 5d28 6874  ena-adapter`](ht
-00003870: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003880: 2f54 6f6d 6d65 2f64 6274 2d61 7468 656e  /Tomme/dbt-athen
-00003890: 6129 2069 7320 6e6f 7420 696e 7374 616c  a) is not instal
-000038a0: 6c65 6420 696e 2074 6865 2074 6172 6765  led in the targe
-000038b0: 7420 656e 7669 726f 6e6d 656e 742e 0a20  t environment.. 
-000038c0: 2053 6565 2068 7474 7073 3a2f 2f67 6974   See https://git
-000038d0: 6875 622e 636f 6d2f 6462 742d 6174 6865  hub.com/dbt-athe
-000038e0: 6e61 2f64 6274 2d61 7468 656e 612f 6973  na/dbt-athena/is
-000038f0: 7375 6573 2f31 3033 2066 6f72 206d 6f72  sues/103 for mor
-00003900: 6520 6465 7461 696c 732e 0a0a 2a20 536e  e details...* Sn
-00003910: 6170 7368 6f74 2064 6f65 7320 6e6f 7420  apshot does not 
-00003920: 7375 7070 6f72 7420 6472 6f70 7069 6e67  support dropping
-00003930: 2063 6f6c 756d 6e73 2066 726f 6d20 7468   columns from th
-00003940: 6520 736f 7572 6365 2074 6162 6c65 2e20  e source table. 
-00003950: 4966 2079 6f75 2064 726f 7020 6120 636f  If you drop a co
-00003960: 6c75 6d6e 206d 616b 6520 7375 7265 2074  lumn make sure t
-00003970: 6f20 6472 6f70 2074 6865 2063 6f6c 756d  o drop the colum
-00003980: 6e20 6672 6f6d 2074 6865 2073 6e61 7073  n from the snaps
-00003990: 686f 7420 6173 2077 656c 6c2e 2041 6e6f  hot as well. Ano
-000039a0: 7468 6572 2077 6f72 6b61 726f 756e 6420  ther workaround 
-000039b0: 6973 2074 6f20 4e55 4c4c 2074 6865 2063  is to NULL the c
-000039c0: 6f6c 756d 6e20 696e 2074 6865 2073 6e61  olumn in the sna
-000039d0: 7073 686f 7420 6465 6669 6e69 7469 6f6e  pshot definition
-000039e0: 2074 6f20 7072 6573 6572 7665 2068 6973   to preserve his
-000039f0: 746f 7279 0a0a 2323 2320 436f 6e74 7269  tory..### Contri
-00003a00: 6275 7469 6e67 0a0a 5468 6973 2063 6f6e  buting..This con
-00003a10: 6e65 6374 6f72 2077 6f72 6b73 2077 6974  nector works wit
-00003a20: 6820 5079 7468 6f6e 2066 726f 6d20 332e  h Python from 3.
-00003a30: 3720 746f 2033 2e31 312e 0a0a 2323 2323  7 to 3.11...####
-00003a40: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
-00003a50: 0a0a 496e 206f 7264 6572 2074 6f20 7374  ..In order to st
-00003a60: 6172 7420 6465 7665 6c6f 7069 6e67 206f  art developing o
-00003a70: 6e20 7468 6973 2061 6461 7074 6572 2063  n this adapter c
-00003a80: 6c6f 6e65 2074 6865 2072 6570 6f20 616e  lone the repo an
-00003a90: 6420 7275 6e20 7468 6973 206d 616b 6520  d run this make 
-00003aa0: 636f 6d6d 616e 6420 2873 6565 205b 4d61  command (see [Ma
-00003ab0: 6b65 6669 6c65 5d28 4d61 6b65 6669 6c65  kefile](Makefile
-00003ac0: 2929 203a 0a0a 6060 6062 6173 680a 6d61  )) :..```bash.ma
-00003ad0: 6b65 2073 6574 7570 0a60 6060 0a0a 4974  ke setup.```..It
-00003ae0: 2077 696c 6c20 3a0a 312e 2049 6e73 7461   will :.1. Insta
-00003af0: 6c6c 2061 6c6c 2064 6570 656e 6465 6e63  ll all dependenc
-00003b00: 6965 732e 0a32 2e20 496e 7374 616c 6c20  ies..2. Install 
-00003b10: 7072 652d 636f 6d6d 6974 2068 6f6f 6b73  pre-commit hooks
-00003b20: 2e0a 332e 2047 656e 6572 6174 6520 796f  ..3. Generate yo
-00003b30: 7572 2060 2e65 6e76 6020 6669 6c65 0a0a  ur `.env` file..
-00003b40: 4e65 7874 2c20 6164 6a75 7374 2060 2e65  Next, adjust `.e
-00003b50: 6e76 6020 6669 6c65 2062 7920 636f 6e66  nv` file by conf
-00003b60: 6967 7572 696e 6720 7468 6520 656e 7669  iguring the envi
-00003b70: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00003b80: 7320 746f 206d 6174 6368 2079 6f75 7220  s to match your 
-00003b90: 4174 6865 6e61 2064 6576 656c 6f70 6d65  Athena developme
-00003ba0: 6e74 2065 6e76 6972 6f6e 6d65 6e74 2e0a  nt environment..
-00003bb0: 0a23 2323 2320 5275 6e6e 696e 6720 7465  .#### Running te
-00003bc0: 7374 730a 0a57 6520 6861 7665 2032 2064  sts..We have 2 d
-00003bd0: 6966 6665 7265 6e74 2074 7970 6573 206f  ifferent types o
-00003be0: 6620 7465 7374 696e 673a 0a2a 202a 2a75  f testing:.* **u
-00003bf0: 6e69 7420 7465 7374 696e 672a 2a3a 2079  nit testing**: y
-00003c00: 6f75 2063 616e 2072 756e 2074 6869 7320  ou can run this 
-00003c10: 7479 7065 206f 6620 7465 7374 7320 7275  type of tests ru
-00003c20: 6e6e 696e 6720 606d 616b 6520 756e 6974  nning `make unit
-00003c30: 5f74 6573 7460 0a2a 202a 2a66 756e 6374  _test`.* **funct
-00003c40: 696f 6e61 6c20 7465 7374 696e 672a 2a3a  ional testing**:
-00003c50: 2079 6f75 206d 7573 7420 6861 7665 2061   you must have a
-00003c60: 6e20 4157 5320 6163 636f 756e 7420 7769  n AWS account wi
-00003c70: 7468 2041 7468 656e 6120 7365 7475 7020  th Athena setup 
-00003c80: 696e 206f 7264 6572 2074 6f20 6c61 756e  in order to laun
-00003c90: 6368 2074 6869 7320 7479 7065 206f 6620  ch this type of 
-00003ca0: 7465 7374 7320 616e 6420 6861 7665 2061  tests and have a
-00003cb0: 2060 2e65 6e76 6020 6669 6c65 2069 6e20   `.env` file in 
-00003cc0: 706c 6163 6520 7769 7468 2074 6865 2072  place with the r
-00003cd0: 6967 6874 2076 616c 7565 732e 0a20 2059  ight values..  Y
-00003ce0: 6f75 2063 616e 2072 756e 2074 6869 7320  ou can run this 
-00003cf0: 7479 7065 206f 6620 7465 7374 7320 7275  type of tests ru
-00003d00: 6e6e 696e 6720 606d 616b 6520 6675 6e63  nning `make func
-00003d10: 7469 6f6e 616c 5f74 6573 7460 0a0a 0a41  tional_test`...A
-00003d20: 6c6c 2074 7970 6520 6f66 2074 6573 7473  ll type of tests
-00003d30: 2063 616e 2062 6520 7275 6e20 7573 696e   can be run usin
-00003d40: 6720 606d 616b 6560 3a0a 6060 6062 6173  g `make`:.```bas
-00003d50: 680a 6d61 6b65 2074 6573 740a 6060 600a  h.make test.```.
-00003d60: 0a23 2323 2320 5075 6c6c 2052 6571 7565  .#### Pull Reque
-00003d70: 7374 0a0a 2a20 4372 6561 7465 2061 2063  st..* Create a c
-00003d80: 6f6d 6d69 7420 7769 7468 2079 6f75 7220  ommit with your 
-00003d90: 6368 616e 6765 7320 616e 6420 7075 7368  changes and push
-00003da0: 2074 6865 6d20 746f 2061 0a20 205b 666f   them to a.  [fo
-00003db0: 726b 5d28 6874 7470 733a 2f2f 646f 6373  rk](https://docs
-00003dc0: 2e67 6974 6875 622e 636f 6d2f 656e 2f67  .github.com/en/g
-00003dd0: 6574 2d73 7461 7274 6564 2f71 7569 636b  et-started/quick
-00003de0: 7374 6172 742f 666f 726b 2d61 2d72 6570  start/fork-a-rep
-00003df0: 6f29 2e0a 2a20 4372 6561 7465 2061 205b  o)..* Create a [
-00003e00: 7075 6c6c 2072 6571 7565 7374 206f 6e0a  pull request on.
-00003e10: 2020 4769 7468 7562 5d28 6874 7470 733a    Github](https:
-00003e20: 2f2f 646f 6373 2e67 6974 6875 622e 636f  //docs.github.co
-00003e30: 6d2f 656e 2f67 6974 6875 622f 636f 6c6c  m/en/github/coll
-00003e40: 6162 6f72 6174 696e 672d 7769 7468 2d70  aborating-with-p
-00003e50: 756c 6c2d 7265 7175 6573 7473 2f70 726f  ull-requests/pro
-00003e60: 706f 7369 6e67 2d63 6861 6e67 6573 2d74  posing-changes-t
-00003e70: 6f2d 796f 7572 2d77 6f72 6b2d 7769 7468  o-your-work-with
-00003e80: 2d70 756c 6c2d 7265 7175 6573 7473 2f63  -pull-requests/c
-00003e90: 7265 6174 696e 672d 612d 7075 6c6c 2d72  reating-a-pull-r
-00003ea0: 6571 7565 7374 2d66 726f 6d2d 612d 666f  equest-from-a-fo
-00003eb0: 726b 292e 0a2a 2050 756c 6c20 7265 7175  rk)..* Pull requ
-00003ec0: 6573 7420 7469 746c 6520 616e 6420 6d65  est title and me
-00003ed0: 7373 6167 6520 2861 6e64 2050 5220 7469  ssage (and PR ti
-00003ee0: 746c 6520 616e 6420 6465 7363 7269 7074  tle and descript
-00003ef0: 696f 6e29 206d 7573 7420 6164 6865 7265  ion) must adhere
-00003f00: 2074 6f0a 2020 5b63 6f6e 7665 6e74 696f   to.  [conventio
-00003f10: 6e61 6c63 6f6d 6d69 7473 5d28 6874 7470  nalcommits](http
-00003f20: 733a 2f2f 7777 772e 636f 6e76 656e 7469  s://www.conventi
-00003f30: 6f6e 616c 636f 6d6d 6974 732e 6f72 6729  onalcommits.org)
-00003f40: 2e0a 2a20 5075 6c6c 2072 6571 7565 7374  ..* Pull request
-00003f50: 2062 6f64 7920 7368 6f75 6c64 2064 6573   body should des
-00003f60: 6372 6962 6520 5f6d 6f74 6976 6174 696f  cribe _motivatio
-00003f70: 6e5f 2e0a 0a23 2323 2048 656c 7066 756c  n_...### Helpful
-00003f80: 2052 6573 6f75 7263 6573 0a0a 2a20 5b41   Resources..* [A
-00003f90: 7468 656e 6120 4352 4541 5445 2054 4142  thena CREATE TAB
-00003fa0: 4c45 2041 535d 2868 7474 7073 3a2f 2f64  LE AS](https://d
-00003fb0: 6f63 732e 6177 732e 616d 617a 6f6e 2e63  ocs.aws.amazon.c
-00003fc0: 6f6d 2f61 7468 656e 612f 6c61 7465 7374  om/athena/latest
-00003fd0: 2f75 672f 6372 6561 7465 2d74 6162 6c65  /ug/create-table
-00003fe0: 2d61 732e 6874 6d6c 290a 2a20 5b64 6274  -as.html).* [dbt
-00003ff0: 2d6c 6162 732f 6462 742d 636f 7265 5d28  -labs/dbt-core](
-00004000: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004010: 6f6d 2f64 6274 2d6c 6162 732f 6462 742d  om/dbt-labs/dbt-
-00004020: 636f 7265 290a 2a20 5b6c 6175 6768 696e  core).* [laughin
-00004030: 676d 616e 3737 3433 2f50 7941 7468 656e  gman7743/PyAthen
-00004040: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00004050: 622e 636f 6d2f 6c61 7567 6869 6e67 6d61  b.com/laughingma
-00004060: 6e37 3734 332f 5079 4174 6865 6e61 290a  n7743/PyAthena).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6462 742d  : 2.1.Name: dbt-
+00000020: 6174 6865 6e61 2d63 6f6d 6d75 6e69 7479  athena-community
+00000030: 0a56 6572 7369 6f6e 3a20 312e 342e 330a  .Version: 1.4.3.
+00000040: 5375 6d6d 6172 793a 2054 6865 2061 7468  Summary: The ath
+00000050: 656e 6120 6164 6170 7465 7220 706c 7567  ena adapter plug
+00000060: 696e 2066 6f72 2064 6274 2028 6461 7461  in for dbt (data
+00000070: 2062 7569 6c64 2074 6f6f 6c29 0a48 6f6d   build tool).Hom
+00000080: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000090: 6769 7468 7562 2e63 6f6d 2f64 6274 2d61  github.com/dbt-a
+000000a0: 7468 656e 612f 6462 742d 6174 6865 6e61  thena/dbt-athena
+000000b0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000000c0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000000d0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+000000e0: 2d46 696c 653a 204c 4943 454e 5345 2e74  -File: LICENSE.t
+000000f0: 7874 0a0a 3c70 2061 6c69 676e 3d22 6365  xt..<p align="ce
+00000100: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
+00000110: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000120: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000130: 6e74 2e63 6f6d 2f64 6274 2d61 7468 656e  nt.com/dbt-athen
+00000140: 612f 6462 742d 6174 6865 6e61 2f6d 6169  a/dbt-athena/mai
+00000150: 6e2f 7374 6174 6963 2f69 6d61 6765 732f  n/static/images/
+00000160: 6462 742d 6174 6865 6e61 2d6c 6f6e 672e  dbt-athena-long.
+00000170: 706e 6722 202f 3e0a 2020 2020 3c61 2068  png" />.    <a h
+00000180: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000190: 692e 6f72 672f 7072 6f6a 6563 742f 6462  i.org/project/db
+000001a0: 742d 6174 6865 6e61 2d63 6f6d 6d75 6e69  t-athena-communi
+000001b0: 7479 2f22 3e3c 696d 6720 7372 633d 2268  ty/"><img src="h
+000001c0: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+000001d0: 792e 696f 2f70 792f 6462 742d 6174 6865  y.io/py/dbt-athe
+000001e0: 6e61 2d63 6f6d 6d75 6e69 7479 2e73 7667  na-community.svg
+000001f0: 2220 2f3e 3c2f 613e 0a20 2020 203c 6120  " /></a>.    <a 
+00000200: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000210: 6371 612e 6769 7468 7562 2e69 6f2f 6973  cqa.github.io/is
+00000220: 6f72 742f 223e 3c69 6d67 2073 7263 3d22  ort/"><img src="
+00000230: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000240: 6c64 732e 696f 2f62 6164 6765 2f25 3230  lds.io/badge/%20
+00000250: 696d 706f 7274 732d 6973 6f72 742d 2532  imports-isort-%2
+00000260: 3331 3637 3462 313f 7374 796c 653d 666c  31674b1?style=fl
+00000270: 6174 266c 6162 656c 436f 6c6f 723d 6566  at&labelColor=ef
+00000280: 3833 3336 2220 2f3e 3c2f 613e 0a20 2020  8336" /></a>.   
+00000290: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000002a0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+000002b0: 2f62 6c61 636b 223e 3c69 6d67 2073 7263  /black"><img src
+000002c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002d0: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
+000002e0: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
+000002f0: 6b2d 3030 3030 3030 2e73 7667 2220 2f3e  k-000000.svg" />
+00000300: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000310: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00000320: 6563 682f 7072 6f6a 6563 742f 6462 742d  ech/project/dbt-
+00000330: 6174 6865 6e61 2d63 6f6d 6d75 6e69 7479  athena-community
+00000340: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000350: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+00000360: 6467 652f 6462 742d 6174 6865 6e61 2d63  dge/dbt-athena-c
+00000370: 6f6d 6d75 6e69 7479 2f6d 6f6e 7468 2220  ommunity/month" 
+00000380: 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a23 2320  /></a>.</p>..## 
+00000390: 4665 6174 7572 6573 0a0a 2a20 5375 7070  Features..* Supp
+000003a0: 6f72 7473 2064 6274 2076 6572 7369 6f6e  orts dbt version
+000003b0: 2060 312e 342e 2a60 0a2a 2053 7570 706f   `1.4.*`.* Suppo
+000003c0: 7274 7320 5b53 6565 6473 5d5b 7365 6564  rts [Seeds][seed
+000003d0: 735d 0a2a 2043 6f72 7265 6374 6c79 2064  s].* Correctly d
+000003e0: 6574 6563 7473 2076 6965 7773 2061 6e64  etects views and
+000003f0: 2074 6865 6972 2063 6f6c 756d 6e73 0a2a   their columns.*
+00000400: 2053 7570 706f 7274 7320 5b74 6162 6c65   Supports [table
+00000410: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
+00000420: 5d5b 7461 626c 655d 0a20 202a 205b 4963  ][table].  * [Ic
+00000430: 6562 6572 6720 7461 626c 6573 5d5b 6174  eberg tables][at
+00000440: 6865 6e61 2d69 6365 6265 7267 5d20 6973  hena-iceberg] is
+00000450: 2073 7570 706f 7274 6564 202a 2a6f 6e6c   supported **onl
+00000460: 7920 7769 7468 2041 7468 656e 6120 456e  y with Athena En
+00000470: 6769 6e65 2076 332a 2a20 616e 6420 2a2a  gine v3** and **
+00000480: 6120 756e 6971 7565 2074 6162 6c65 206c  a unique table l
+00000490: 6f63 6174 696f 6e2a 2a0a 2020 2873 6565  ocation**.  (see
+000004a0: 2074 6162 6c65 206c 6f63 6174 696f 6e20   table location 
+000004b0: 7365 6374 696f 6e20 6265 6c6f 7729 0a20  section below). 
+000004c0: 202a 2048 6976 6520 7461 626c 6573 2069   * Hive tables i
+000004d0: 7320 7375 7070 6f72 7465 6420 6279 2062  s supported by b
+000004e0: 6f74 6820 4174 6865 6e61 2065 6e67 696e  oth Athena engin
+000004f0: 6573 2e0a 2a20 5375 7070 6f72 7473 205b  es..* Supports [
+00000500: 696e 6372 656d 656e 7461 6c20 6d6f 6465  incremental mode
+00000510: 6c73 5d5b 696e 6372 656d 656e 7461 6c5d  ls][incremental]
+00000520: 0a20 202a 204f 6e20 6963 6562 6572 6720  .  * On iceberg 
+00000530: 7461 626c 6573 203a 0a20 2020 202a 2053  tables :.    * S
+00000540: 7570 706f 7274 2074 6865 2075 7365 206f  upport the use o
+00000550: 6620 6075 6e69 7175 655f 6b65 7960 206f  f `unique_key` o
+00000560: 6e6c 7920 7769 7468 2074 6865 2060 6d65  nly with the `me
+00000570: 7267 6560 2073 7472 6174 6567 790a 2020  rge` strategy.  
+00000580: 2020 2a20 5375 7070 6f72 7420 7468 6520    * Support the 
+00000590: 6061 7070 656e 6460 2073 7472 6174 6567  `append` strateg
+000005a0: 790a 2020 2a20 4f6e 2048 6976 6520 7461  y.  * On Hive ta
+000005b0: 626c 6573 203a 0a20 2020 202a 2053 7570  bles :.    * Sup
+000005c0: 706f 7274 2074 776f 2069 6e63 7265 6d65  port two increme
+000005d0: 6e74 616c 2075 7064 6174 6520 7374 7261  ntal update stra
+000005e0: 7465 6769 6573 3a20 6069 6e73 6572 745f  tegies: `insert_
+000005f0: 6f76 6572 7772 6974 6560 2061 6e64 2060  overwrite` and `
+00000600: 6170 7065 6e64 600a 2020 2020 2a20 446f  append`.    * Do
+00000610: 6573 202a 2a6e 6f74 2a2a 2073 7570 706f  es **not** suppo
+00000620: 7274 2074 6865 2075 7365 206f 6620 6075  rt the use of `u
+00000630: 6e69 7175 655f 6b65 7960 0a2a 2053 7570  nique_key`.* Sup
+00000640: 706f 7274 7320 5b73 6e61 7073 686f 7473  ports [snapshots
+00000650: 5d5b 736e 6170 7368 6f74 735d 0a2a 2044  ][snapshots].* D
+00000660: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+00000670: 5b50 7974 686f 6e20 6d6f 6465 6c73 5d5b  [Python models][
+00000680: 7079 7468 6f6e 2d6d 6f64 656c 735d 0a2a  python-models].*
+00000690: 2044 6f65 7320 6e6f 7420 7375 7070 6f72   Does not suppor
+000006a0: 7420 5b70 6572 7369 7374 2064 6f63 735d  t [persist docs]
+000006b0: 5b70 6572 7369 7374 2d64 6f63 735d 2066  [persist-docs] f
+000006c0: 6f72 2076 6965 7773 0a0a 5b73 6565 6473  or views..[seeds
+000006d0: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+000006e0: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+000006f0: 6275 696c 6469 6e67 2d61 2d64 6274 2d70  building-a-dbt-p
+00000700: 726f 6a65 6374 2f73 6565 6473 0a5b 696e  roject/seeds.[in
+00000710: 6372 656d 656e 7461 6c5d 3a20 6874 7470  cremental]: http
+00000720: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
+00000730: 636f 6d2f 646f 6373 2f62 7569 6c64 2f69  com/docs/build/i
+00000740: 6e63 7265 6d65 6e74 616c 2d6d 6f64 656c  ncremental-model
+00000750: 730a 5b74 6162 6c65 5d3a 2068 7474 7073  s.[table]: https
+00000760: 3a2f 2f64 6f63 732e 6765 7464 6274 2e63  ://docs.getdbt.c
+00000770: 6f6d 2f64 6f63 732f 6275 696c 642f 6d61  om/docs/build/ma
+00000780: 7465 7269 616c 697a 6174 696f 6e73 2374  terializations#t
+00000790: 6162 6c65 0a5b 7079 7468 6f6e 2d6d 6f64  able.[python-mod
+000007a0: 656c 735d 3a20 6874 7470 733a 2f2f 646f  els]: https://do
+000007b0: 6373 2e67 6574 6462 742e 636f 6d2f 646f  cs.getdbt.com/do
+000007c0: 6373 2f62 7569 6c64 2f70 7974 686f 6e2d  cs/build/python-
+000007d0: 6d6f 6465 6c73 2363 6f6e 6669 6775 7269  models#configuri
+000007e0: 6e67 2d70 7974 686f 6e2d 6d6f 6465 6c73  ng-python-models
+000007f0: 0a5b 6174 6865 6e61 2d69 6365 6265 7267  .[athena-iceberg
+00000800: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+00000810: 6177 732e 616d 617a 6f6e 2e63 6f6d 2f61  aws.amazon.com/a
+00000820: 7468 656e 612f 6c61 7465 7374 2f75 672f  thena/latest/ug/
+00000830: 7175 6572 7969 6e67 2d69 6365 6265 7267  querying-iceberg
+00000840: 2e68 746d 6c0a 5b73 6e61 7073 686f 7473  .html.[snapshots
+00000850: 5d3a 2068 7474 7073 3a2f 2f64 6f63 732e  ]: https://docs.
+00000860: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+00000870: 6275 696c 642f 736e 6170 7368 6f74 730a  build/snapshots.
+00000880: 5b70 6572 7369 7374 2d64 6f63 735d 3a20  [persist-docs]: 
+00000890: 6874 7470 733a 2f2f 646f 6373 2e67 6574  https://docs.get
+000008a0: 6462 742e 636f 6d2f 7265 6665 7265 6e63  dbt.com/referenc
+000008b0: 652f 7265 736f 7572 6365 2d63 6f6e 6669  e/resource-confi
+000008c0: 6773 2f70 6572 7369 7374 5f64 6f63 730a  gs/persist_docs.
+000008d0: 0a0a 2323 2051 7569 636b 2053 7461 7274  ..## Quick Start
+000008e0: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+000008f0: 6f6e 0a0a 2a20 6070 6970 2069 6e73 7461  on..* `pip insta
+00000900: 6c6c 2064 6274 2d61 7468 656e 612d 636f  ll dbt-athena-co
+00000910: 6d6d 756e 6974 7960 0a2a 204f 7220 6070  mmunity`.* Or `p
+00000920: 6970 2069 6e73 7461 6c6c 2067 6974 2b68  ip install git+h
+00000930: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000940: 6d2f 6462 742d 6174 6865 6e61 2f64 6274  m/dbt-athena/dbt
+00000950: 2d61 7468 656e 612e 6769 7460 0a0a 2323  -athena.git`..##
+00000960: 2320 5072 6572 6571 7569 7369 7465 730a  # Prerequisites.
+00000970: 0a54 6f20 7374 6172 742c 2079 6f75 2077  .To start, you w
+00000980: 696c 6c20 6e65 6564 2061 6e20 5333 2062  ill need an S3 b
+00000990: 7563 6b65 742c 2066 6f72 2069 6e73 7461  ucket, for insta
+000009a0: 6e63 6520 606d 792d 6275 636b 6574 6020  nce `my-bucket` 
+000009b0: 616e 6420 616e 2041 7468 656e 6120 6461  and an Athena da
+000009c0: 7461 6261 7365 3a0a 0a60 6060 7371 6c0a  tabase:..```sql.
+000009d0: 4352 4541 5445 2044 4154 4142 4153 4520  CREATE DATABASE 
+000009e0: 4946 204e 4f54 2045 5849 5354 5320 616e  IF NOT EXISTS an
+000009f0: 616c 7974 6963 735f 6465 760a 434f 4d4d  alytics_dev.COMM
+00000a00: 454e 5420 2741 6e61 6c79 7469 6373 206d  ENT 'Analytics m
+00000a10: 6f64 656c 7320 6765 6e65 7261 7465 6420  odels generated 
+00000a20: 6279 2064 6274 2028 6465 7665 6c6f 706d  by dbt (developm
+00000a30: 656e 7429 270a 4c4f 4341 5449 4f4e 2027  ent)'.LOCATION '
+00000a40: 7333 3a2f 2f6d 792d 6275 636b 6574 2f27  s3://my-bucket/'
+00000a50: 0a57 4954 4820 4442 5052 4f50 4552 5449  .WITH DBPROPERTI
+00000a60: 4553 2028 2763 7265 6174 6f72 273d 2746  ES ('creator'='F
+00000a70: 6f6f 2042 6172 272c 2027 656d 6169 6c27  oo Bar', 'email'
+00000a80: 3d27 666f 6f40 6261 722e 636f 6d27 293b  ='foo@bar.com');
+00000a90: 0a60 6060 0a0a 4e6f 7465 733a 0a2d 2054  .```..Notes:.- T
+00000aa0: 616b 6520 6e6f 7465 206f 6620 796f 7572  ake note of your
+00000ab0: 2041 5753 2072 6567 696f 6e20 636f 6465   AWS region code
+00000ac0: 2028 652e 672e 2060 7573 2d77 6573 742d   (e.g. `us-west-
+00000ad0: 3260 206f 7220 6065 752d 7765 7374 2d32  2` or `eu-west-2
+00000ae0: 602c 2065 7463 2e29 2e0a 2d20 596f 7520  `, etc.)..- You 
+00000af0: 6361 6e20 616c 736f 2075 7365 205b 4157  can also use [AW
+00000b00: 5320 476c 7565 5d28 6874 7470 733a 2f2f  S Glue](https://
+00000b10: 646f 6373 2e61 7773 2e61 6d61 7a6f 6e2e  docs.aws.amazon.
+00000b20: 636f 6d2f 6174 6865 6e61 2f6c 6174 6573  com/athena/lates
+00000b30: 742f 7567 2f67 6c75 652d 6174 6865 6e61  t/ug/glue-athena
+00000b40: 2e68 746d 6c29 2074 6f20 6372 6561 7465  .html) to create
+00000b50: 2061 6e64 206d 616e 6167 6520 4174 6865   and manage Athe
+00000b60: 6e61 2064 6174 6162 6173 6573 2e0a 0a23  na databases...#
+00000b70: 2323 2043 7265 6465 6e74 6961 6c73 0a0a  ## Credentials..
+00000b80: 5468 6973 2070 6c75 6769 6e20 646f 6573  This plugin does
+00000b90: 206e 6f74 2061 6363 6570 7420 616e 7920   not accept any 
+00000ba0: 6372 6564 656e 7469 616c 7320 6469 7265  credentials dire
+00000bb0: 6374 6c79 2e20 496e 7374 6561 642c 205b  ctly. Instead, [
+00000bc0: 6372 6564 656e 7469 616c 7320 6172 6520  credentials are 
+00000bd0: 6465 7465 726d 696e 6564 2061 7574 6f6d  determined autom
+00000be0: 6174 6963 616c 6c79 5d28 6874 7470 733a  atically](https:
+00000bf0: 2f2f 626f 746f 332e 616d 617a 6f6e 6177  //boto3.amazonaw
+00000c00: 732e 636f 6d2f 7631 2f64 6f63 756d 656e  s.com/v1/documen
+00000c10: 7461 7469 6f6e 2f61 7069 2f6c 6174 6573  tation/api/lates
+00000c20: 742f 6775 6964 652f 6372 6564 656e 7469  t/guide/credenti
+00000c30: 616c 732e 6874 6d6c 2920 6261 7365 6420  als.html) based 
+00000c40: 6f6e 2060 6177 7320 636c 6960 2f60 626f  on `aws cli`/`bo
+00000c50: 746f 3360 2063 6f6e 7665 6e74 696f 6e73  to3` conventions
+00000c60: 2061 6e64 0a73 746f 7265 6420 6c6f 6769   and.stored logi
+00000c70: 6e20 696e 666f 2e20 596f 7520 6361 6e20  n info. You can 
+00000c80: 636f 6e66 6967 7572 6520 7468 6520 4157  configure the AW
+00000c90: 5320 7072 6f66 696c 6520 6e61 6d65 2074  S profile name t
+00000ca0: 6f20 7573 6520 7669 6120 6061 7773 5f70  o use via `aws_p
+00000cb0: 726f 6669 6c65 5f6e 616d 6560 2e20 4368  rofile_name`. Ch
+00000cc0: 6563 6b6f 7574 2044 4254 2070 726f 6669  eckout DBT profi
+00000cd0: 6c65 2063 6f6e 6669 6775 7261 7469 6f6e  le configuration
+00000ce0: 2062 656c 6f77 2066 6f72 2064 6574 6169   below for detai
+00000cf0: 6c73 2e0a 0a23 2323 2043 6f6e 6669 6775  ls...### Configu
+00000d00: 7269 6e67 2079 6f75 7220 7072 6f66 696c  ring your profil
+00000d10: 650a 0a41 2064 6274 2070 726f 6669 6c65  e..A dbt profile
+00000d20: 2063 616e 2062 6520 636f 6e66 6967 7572   can be configur
+00000d30: 6564 2074 6f20 7275 6e20 6167 6169 6e73  ed to run agains
+00000d40: 7420 4157 5320 4174 6865 6e61 2075 7369  t AWS Athena usi
+00000d50: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
+00000d60: 2063 6f6e 6669 6775 7261 7469 6f6e 3a0a   configuration:.
+00000d70: 0a7c 204f 7074 696f 6e20 2020 2020 2020  .| Option       
+00000d80: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
+00000d90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dd0: 2020 2020 207c 2052 6571 7569 7265 643f       | Required?
+00000de0: 207c 2045 7861 6d70 6c65 2020 2020 2020   | Example      
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
+00000e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e20: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e70: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --|-----------|-
+00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ea0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2073 335f  ---------|.| s3_
+00000eb0: 7374 6167 696e 675f 6469 7220 2020 7c20  staging_dir   | 
+00000ec0: 5333 206c 6f63 6174 696f 6e20 746f 2073  S3 location to s
+00000ed0: 746f 7265 2041 7468 656e 6120 7175 6572  tore Athena quer
+00000ee0: 7920 7265 7375 6c74 7320 616e 6420 6d65  y results and me
+00000ef0: 7461 6461 7461 2020 2020 2020 2020 2020  tadata          
+00000f00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000f10: 2052 6571 7569 7265 6420 207c 2060 7333   Required  | `s3
+00000f20: 3a2f 2f62 7563 6b65 742f 6462 742f 6020  ://bucket/dbt/` 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 7c0a 7c20 7333 5f64 6174        |.| s3_dat
+00000f50: 615f 6469 7220 2020 2020 207c 2050 7265  a_dir      | Pre
+00000f60: 6669 7820 666f 7220 7374 6f72 696e 6720  fix for storing 
+00000f70: 7461 626c 6573 2c20 6966 2064 6966 6665  tables, if diffe
+00000f80: 7265 6e74 2066 726f 6d20 7468 6520 636f  rent from the co
+00000f90: 6e6e 6563 7469 6f6e 2773 2060 7333 5f73  nnection's `s3_s
+00000fa0: 7461 6769 6e67 5f64 6972 6020 7c20 4f70  taging_dir` | Op
+00000fb0: 7469 6f6e 616c 2020 7c20 6073 333a 2f2f  tional  | `s3://
+00000fc0: 6275 636b 6574 322f 6462 742f 6020 2020  bucket2/dbt/`   
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 207c 0a7c 2073 335f 6461 7461 5f6e     |.| s3_data_n
+00000ff0: 616d 696e 6720 2020 7c20 486f 7720 746f  aming   | How to
+00001000: 2067 656e 6572 6174 6520 7461 626c 6520   generate table 
+00001010: 7061 7468 7320 696e 2060 7333 5f64 6174  paths in `s3_dat
+00001020: 615f 6469 7260 2020 2020 2020 2020 2020  a_dir`          
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 207c 204f 7074 696f           | Optio
+00001050: 6e61 6c20 207c 2060 7363 6865 6d61 5f74  nal  | `schema_t
+00001060: 6162 6c65 5f75 6e69 7175 6560 2020 2020  able_unique`    
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 7c0a 7c20 7265 6769 6f6e 5f6e 616d 6520  |.| region_name 
+00001090: 2020 2020 207c 2041 5753 2072 6567 696f       | AWS regio
+000010a0: 6e20 6f66 2079 6f75 7220 4174 6865 6e61  n of your Athena
+000010b0: 2069 6e73 7461 6e63 6520 2020 2020 2020   instance       
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2020 2020 7c20 5265 7175 6972 6564        | Required
+000010f0: 2020 7c20 6065 752d 7765 7374 2d31 6020    | `eu-west-1` 
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00001120: 2073 6368 656d 6120 2020 2020 2020 2020   schema         
+00001130: 2020 7c20 5370 6563 6966 7920 7468 6520    | Specify the 
+00001140: 7363 6865 6d61 2028 4174 6865 6e61 2064  schema (Athena d
+00001150: 6174 6162 6173 6529 2074 6f20 6275 696c  atabase) to buil
+00001160: 6420 6d6f 6465 6c73 2069 6e74 6f20 286c  d models into (l
+00001170: 6f77 6572 6361 7365 202a 2a6f 6e6c 792a  owercase **only*
+00001180: 2a29 207c 2052 6571 7569 7265 6420 207c  *) | Required  |
+00001190: 2060 6462 7460 2020 2020 2020 2020 2020   `dbt`          
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2020 2020 2020 2020 7c0a 7c20 6461            |.| da
+000011c0: 7461 6261 7365 2020 2020 2020 2020 207c  tabase         |
+000011d0: 2053 7065 6369 6679 2074 6865 2064 6174   Specify the dat
+000011e0: 6162 6173 6520 2844 6174 6120 6361 7461  abase (Data cata
+000011f0: 6c6f 6729 2074 6f20 6275 696c 6420 6d6f  log) to build mo
+00001200: 6465 6c73 2069 6e74 6f20 286c 6f77 6572  dels into (lower
+00001210: 6361 7365 202a 2a6f 6e6c 792a 2a29 2020  case **only**)  
+00001220: 7c20 5265 7175 6972 6564 2020 7c20 6061  | Required  | `a
+00001230: 7773 6461 7461 6361 7461 6c6f 6760 2020  wsdatacatalog`  
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 2020 2020 207c 0a7c 2070 6f6c 6c5f         |.| poll_
+00001260: 696e 7465 7276 616c 2020 2020 7c20 496e  interval    | In
+00001270: 7465 7276 616c 2069 6e20 7365 636f 6e64  terval in second
+00001280: 7320 746f 2075 7365 2066 6f72 2070 6f6c  s to use for pol
+00001290: 6c69 6e67 2074 6865 2073 7461 7475 7320  ling the status 
+000012a0: 6f66 2071 7565 7279 2072 6573 756c 7473  of query results
+000012b0: 2069 6e20 4174 6865 6e61 2020 207c 204f   in Athena   | O
+000012c0: 7074 696f 6e61 6c20 207c 2060 3560 2020  ptional  | `5`  
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 7c0a 7c20 6177 735f 7072 6f66      |.| aws_prof
+00001300: 696c 655f 6e61 6d65 207c 2050 726f 6669  ile_name | Profi
+00001310: 6c65 2074 6f20 7573 6520 6672 6f6d 2079  le to use from y
+00001320: 6f75 7220 4157 5320 7368 6172 6564 2063  our AWS shared c
+00001330: 7265 6465 6e74 6961 6c73 2066 696c 652e  redentials file.
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2020 2020 2020 7c20 4f70 7469            | Opti
+00001360: 6f6e 616c 2020 7c20 606d 792d 7072 6f66  onal  | `my-prof
+00001370: 696c 6560 2020 2020 2020 2020 2020 2020  ile`            
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 207c 0a7c 2077 6f72 6b5f 6772 6f75 7020   |.| work_group 
+000013a0: 2020 2020 2020 7c20 4964 656e 7469 6669        | Identifi
+000013b0: 6572 206f 6620 4174 6865 6e61 2077 6f72  er of Athena wor
+000013c0: 6b67 726f 7570 2020 2020 2020 2020 2020  kgroup          
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 2020 2020 207c 204f 7074 696f 6e61         | Optiona
+00001400: 6c20 207c 2060 6d79 2d63 7573 746f 6d2d  l  | `my-custom-
+00001410: 776f 726b 6772 6f75 7060 2020 2020 2020  workgroup`      
+00001420: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001430: 7c20 6e75 6d5f 7265 7472 6965 7320 2020  | num_retries   
+00001440: 2020 207c 204e 756d 6265 7220 6f66 2074     | Number of t
+00001450: 696d 6573 2074 6f20 7265 7472 7920 6120  imes to retry a 
+00001460: 6661 696c 696e 6720 7175 6572 7920 2020  failing query   
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 2020 7c20 4f70 7469 6f6e 616c 2020      | Optional  
+000014a0: 7c20 6033 6020 2020 2020 2020 2020 2020  | `3`           
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 207c 0a7c 206c             |.| l
+000014d0: 665f 7461 6773 2020 2020 2020 2020 2020  f_tags          
+000014e0: 7c20 4465 6661 756c 7420 6c66 2074 6167  | Default lf tag
+000014f0: 7320 746f 2061 7070 6c79 2074 6f20 616e  s to apply to an
+00001500: 7920 6461 7461 6261 7365 2063 7265 6174  y database creat
+00001510: 6564 2062 7920 6462 7420 2020 2020 2020  ed by dbt       
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 207c 204f 7074 696f 6e61 6c20 207c 2060   | Optional  | `
+00001540: 7b22 6f72 6967 696e 223a 2022 6462 7422  {"origin": "dbt"
+00001550: 2c20 2274 6561 6d22 3a20 2261 6e61 6c79  , "team": "analy
+00001560: 7469 6373 227d 6020 7c0a 0a2a 2a45 7861  tics"}` |..**Exa
+00001570: 6d70 6c65 2070 726f 6669 6c65 732e 796d  mple profiles.ym
+00001580: 6c20 656e 7472 793a 2a2a 0a60 6060 7961  l entry:**.```ya
+00001590: 6d6c 0a61 7468 656e 613a 0a20 2074 6172  ml.athena:.  tar
+000015a0: 6765 743a 2064 6576 0a20 206f 7574 7075  get: dev.  outpu
+000015b0: 7473 3a0a 2020 2020 6465 763a 0a20 2020  ts:.    dev:.   
+000015c0: 2020 2074 7970 653a 2061 7468 656e 610a     type: athena.
+000015d0: 2020 2020 2020 7333 5f73 7461 6769 6e67        s3_staging
+000015e0: 5f64 6972 3a20 7333 3a2f 2f61 7468 656e  _dir: s3://athen
+000015f0: 612d 7175 6572 792d 7265 7375 6c74 732f  a-query-results/
+00001600: 6462 742f 0a20 2020 2020 2073 335f 6461  dbt/.      s3_da
+00001610: 7461 5f64 6972 3a20 7333 3a2f 2f79 6f75  ta_dir: s3://you
+00001620: 725f 7333 5f62 7563 6b65 742f 6462 742f  r_s3_bucket/dbt/
+00001630: 0a20 2020 2020 2073 335f 6461 7461 5f6e  .      s3_data_n
+00001640: 616d 696e 673a 2073 6368 656d 615f 7461  aming: schema_ta
+00001650: 626c 650a 2020 2020 2020 7265 6769 6f6e  ble.      region
+00001660: 5f6e 616d 653a 2065 752d 7765 7374 2d31  _name: eu-west-1
+00001670: 0a20 2020 2020 2073 6368 656d 613a 2064  .      schema: d
+00001680: 6274 0a20 2020 2020 2064 6174 6162 6173  bt.      databas
+00001690: 653a 2061 7773 6461 7461 6361 7461 6c6f  e: awsdatacatalo
+000016a0: 670a 2020 2020 2020 6177 735f 7072 6f66  g.      aws_prof
+000016b0: 696c 655f 6e61 6d65 3a20 6d79 2d70 726f  ile_name: my-pro
+000016c0: 6669 6c65 0a20 2020 2020 2077 6f72 6b5f  file.      work_
+000016d0: 6772 6f75 703a 206d 792d 776f 726b 6772  group: my-workgr
+000016e0: 6f75 700a 2020 2020 2020 6c66 5f74 6167  oup.      lf_tag
+000016f0: 733a 0a20 2020 2020 2020 206f 7269 6769  s:.        origi
+00001700: 6e3a 2064 6274 0a20 2020 2020 2020 2074  n: dbt.        t
+00001710: 6561 6d3a 2061 6e61 6c79 7469 6373 0a60  eam: analytics.`
+00001720: 6060 0a0a 5f41 6464 6974 696f 6e61 6c20  ``.._Additional 
+00001730: 696e 666f 726d 6174 696f 6e5f 0a2a 2060  information_.* `
+00001740: 7468 7265 6164 7360 2069 7320 7375 7070  threads` is supp
+00001750: 6f72 7465 640a 2a20 6064 6174 6162 6173  orted.* `databas
+00001760: 6560 2061 6e64 2060 6361 7461 6c6f 6760  e` and `catalog`
+00001770: 2063 616e 2062 6520 7573 6564 2069 6e74   can be used int
+00001780: 6572 6368 616e 6765 6162 6c79 0a0a 0a23  erchangeably...#
+00001790: 2320 4d6f 6465 6c73 0a0a 2323 2320 5461  # Models..### Ta
+000017a0: 626c 6520 436f 6e66 6967 7572 6174 696f  ble Configuratio
+000017b0: 6e0a 0a2a 2060 6578 7465 726e 616c 5f6c  n..* `external_l
+000017c0: 6f63 6174 696f 6e60 2028 6064 6566 6175  ocation` (`defau
+000017d0: 6c74 3d6e 6f6e 6560 290a 2020 2a20 4966  lt=none`).  * If
+000017e0: 2073 6574 2c20 7468 6520 6675 6c6c 2053   set, the full S
+000017f0: 3320 7061 7468 2069 6e20 7768 6963 6820  3 path in which 
+00001800: 7468 6520 7461 626c 6520 7769 6c6c 2062  the table will b
+00001810: 6520 7361 7665 642e 2028 446f 6573 206e  e saved. (Does n
+00001820: 6f74 2077 6f72 6b20 7769 7468 2049 6365  ot work with Ice
+00001830: 6265 7267 2074 6162 6c65 292e 0a2a 2060  berg table)..* `
+00001840: 7061 7274 6974 696f 6e65 645f 6279 6020  partitioned_by` 
+00001850: 2860 6465 6661 756c 743d 6e6f 6e65 6029  (`default=none`)
+00001860: 0a20 202a 2041 6e20 6172 7261 7920 6c69  .  * An array li
+00001870: 7374 206f 6620 636f 6c75 6d6e 7320 6279  st of columns by
+00001880: 2077 6869 6368 2074 6865 2074 6162 6c65   which the table
+00001890: 2077 696c 6c20 6265 2070 6172 7469 7469   will be partiti
+000018a0: 6f6e 6564 0a20 202a 204c 696d 6974 6564  oned.  * Limited
+000018b0: 2074 6f20 6372 6561 7469 6f6e 206f 6620   to creation of 
+000018c0: 3130 3020 7061 7274 6974 696f 6e73 2028  100 partitions (
+000018d0: 5f63 7572 7265 6e74 6c79 5f29 0a2a 2060  _currently_).* `
+000018e0: 6275 636b 6574 6564 5f62 7960 2028 6064  bucketed_by` (`d
+000018f0: 6566 6175 6c74 3d6e 6f6e 6560 290a 2020  efault=none`).  
+00001900: 2a20 416e 2061 7272 6179 206c 6973 7420  * An array list 
+00001910: 6f66 2063 6f6c 756d 6e73 2074 6f20 6275  of columns to bu
+00001920: 636b 6574 2064 6174 612c 2069 676e 6f72  cket data, ignor
+00001930: 6564 2069 6620 7573 696e 6720 4963 6562  ed if using Iceb
+00001940: 6572 670a 2a20 6062 7563 6b65 745f 636f  erg.* `bucket_co
+00001950: 756e 7460 2028 6064 6566 6175 6c74 3d6e  unt` (`default=n
+00001960: 6f6e 6560 290a 2020 2a20 5468 6520 6e75  one`).  * The nu
+00001970: 6d62 6572 206f 6620 6275 636b 6574 7320  mber of buckets 
+00001980: 666f 7220 6275 636b 6574 696e 6720 796f  for bucketing yo
+00001990: 7572 2064 6174 612c 2069 676e 6f72 6564  ur data, ignored
+000019a0: 2069 6620 7573 696e 6720 4963 6562 6572   if using Iceber
+000019b0: 670a 2a20 6074 6162 6c65 5f74 7970 6560  g.* `table_type`
+000019c0: 2028 6064 6566 6175 6c74 3d27 6869 7665   (`default='hive
+000019d0: 2760 290a 2020 2a20 5468 6520 7479 7065  '`).  * The type
+000019e0: 206f 6620 7461 626c 650a 2020 2a20 5375   of table.  * Su
+000019f0: 7070 6f72 7473 2060 6869 7665 6020 6f72  pports `hive` or
+00001a00: 2060 6963 6562 6572 6760 0a2a 2060 666f   `iceberg`.* `fo
+00001a10: 726d 6174 6020 2860 6465 6661 756c 743d  rmat` (`default=
+00001a20: 2770 6172 7175 6574 2760 290a 2020 2a20  'parquet'`).  * 
+00001a30: 5468 6520 6461 7461 2066 6f72 6d61 7420  The data format 
+00001a40: 666f 7220 7468 6520 7461 626c 650a 2020  for the table.  
+00001a50: 2a20 5375 7070 6f72 7473 2060 4f52 4360  * Supports `ORC`
+00001a60: 2c20 6050 4152 5155 4554 602c 2060 4156  , `PARQUET`, `AV
+00001a70: 524f 602c 2060 4a53 4f4e 602c 2060 5445  RO`, `JSON`, `TE
+00001a80: 5854 4649 4c45 600a 2a20 6077 7269 7465  XTFILE`.* `write
+00001a90: 5f63 6f6d 7072 6573 7369 6f6e 6020 2860  _compression` (`
+00001aa0: 6465 6661 756c 743d 6e6f 6e65 6029 0a20  default=none`). 
+00001ab0: 202a 2054 6865 2063 6f6d 7072 6573 7369   * The compressi
+00001ac0: 6f6e 2074 7970 6520 746f 2075 7365 2066  on type to use f
+00001ad0: 6f72 2061 6e79 2073 746f 7261 6765 2066  or any storage f
+00001ae0: 6f72 6d61 7420 7468 6174 2061 6c6c 6f77  ormat that allow
+00001af0: 7320 636f 6d70 7265 7373 696f 6e20 746f  s compression to
+00001b00: 2062 6520 7370 6563 6966 6965 642e 2054   be specified. T
+00001b10: 6f20 7365 6520 7768 6963 6820 6f70 7469  o see which opti
+00001b20: 6f6e 7320 6172 6520 6176 6169 6c61 626c  ons are availabl
+00001b30: 652c 2063 6865 636b 206f 7574 205b 4352  e, check out [CR
+00001b40: 4541 5445 2054 4142 4c45 2041 535d 5b63  EATE TABLE AS][c
+00001b50: 7265 6174 652d 7461 626c 652d 6173 5d0a  reate-table-as].
+00001b60: 2a20 6066 6965 6c64 5f64 656c 696d 6974  * `field_delimit
+00001b70: 6572 6020 2860 6465 6661 756c 743d 6e6f  er` (`default=no
+00001b80: 6e65 6029 0a20 202a 2043 7573 746f 6d20  ne`).  * Custom 
+00001b90: 6669 656c 6420 6465 6c69 6d69 7465 722c  field delimiter,
+00001ba0: 2066 6f72 2077 6865 6e20 666f 726d 6174   for when format
+00001bb0: 2069 7320 7365 7420 746f 2060 5445 5854   is set to `TEXT
+00001bc0: 4649 4c45 600a 2a20 6074 6162 6c65 5f70  FILE`.* `table_p
+00001bd0: 726f 7065 7274 6965 7360 3a20 7461 626c  roperties`: tabl
+00001be0: 6520 7072 6f70 6572 7469 6573 2074 6f20  e properties to 
+00001bf0: 6164 6420 746f 2074 6865 2074 6162 6c65  add to the table
+00001c00: 2c20 7661 6c69 6420 666f 7220 4963 6562  , valid for Iceb
+00001c10: 6572 6720 6f6e 6c79 0a2a 2060 6c66 5f74  erg only.* `lf_t
+00001c20: 6167 7360 2028 6064 6566 6175 6c74 3d6e  ags` (`default=n
+00001c30: 6f6e 6560 290a 2020 2a20 6c66 2074 6167  one`).  * lf tag
+00001c40: 7320 746f 2061 7373 6f63 6961 7465 2077  s to associate w
+00001c50: 6974 6820 7468 6520 7461 626c 650a 2020  ith the table.  
+00001c60: 2a20 666f 726d 6174 3a20 607b 2274 6167  * format: `{"tag
+00001c70: 3122 3a20 2276 616c 7565 3122 2c20 2274  1": "value1", "t
+00001c80: 6167 3222 3a20 2276 616c 7565 3222 7d60  ag2": "value2"}`
+00001c90: 0a2a 2060 6c66 5f74 6167 735f 636f 6c75  .* `lf_tags_colu
+00001ca0: 6d6e 7360 2028 6064 6566 6175 6c74 3d6e  mns` (`default=n
+00001cb0: 6f6e 6560 290a 2020 2a20 6c66 2074 6167  one`).  * lf tag
+00001cc0: 7320 746f 2061 7373 6f63 6961 7465 2077  s to associate w
+00001cd0: 6974 6820 7468 6520 7461 626c 6520 636f  ith the table co
+00001ce0: 6c75 6d6e 730a 2020 2a20 666f 726d 6174  lumns.  * format
+00001cf0: 3a20 607b 2274 6167 3122 3a20 7b22 7661  : `{"tag1": {"va
+00001d00: 6c75 6531 223a 205b 2263 6f6c 756d 6e31  lue1": ["column1
+00001d10: 223a 2022 636f 6c75 6d6e 3222 5d7d 7d60  ": "column2"]}}`
+00001d20: 0a0a 2323 2320 5461 626c 6520 6c6f 6361  ..### Table loca
+00001d30: 7469 6f6e 0a0a 5468 6520 6c6f 6361 7469  tion..The locati
+00001d40: 6f6e 2069 6e20 7768 6963 6820 6120 7461  on in which a ta
+00001d50: 626c 6520 6973 2073 6176 6564 2069 7320  ble is saved is 
+00001d60: 6465 7465 726d 696e 6564 2062 793a 0a0a  determined by:..
+00001d70: 312e 2049 6620 6065 7874 6572 6e61 6c5f  1. If `external_
+00001d80: 6c6f 6361 7469 6f6e 6020 6973 2064 6566  location` is def
+00001d90: 696e 6564 2c20 7468 6174 2076 616c 7565  ined, that value
+00001da0: 2069 7320 7573 6564 2e0a 322e 2049 6620   is used..2. If 
+00001db0: 6073 335f 6461 7461 5f64 6972 6020 6973  `s3_data_dir` is
+00001dc0: 2064 6566 696e 6564 2c20 7468 6520 7061   defined, the pa
+00001dd0: 7468 2069 7320 6465 7465 726d 696e 6564  th is determined
+00001de0: 2062 7920 7468 6174 2061 6e64 2060 7333   by that and `s3
+00001df0: 5f64 6174 615f 6e61 6d69 6e67 600a 332e  _data_naming`.3.
+00001e00: 2049 6620 6073 335f 6461 7461 5f64 6972   If `s3_data_dir
+00001e10: 6020 6973 206e 6f74 2064 6566 696e 6564  ` is not defined
+00001e20: 2064 6174 6120 6973 2073 746f 7265 6420   data is stored 
+00001e30: 756e 6465 7220 6073 335f 7374 6167 696e  under `s3_stagin
+00001e40: 675f 6469 722f 7461 626c 6573 2f60 0a0a  g_dir/tables/`..
+00001e50: 4865 7265 2061 6c6c 2074 6865 206f 7074  Here all the opt
+00001e60: 696f 6e73 2061 7661 696c 6162 6c65 2066  ions available f
+00001e70: 6f72 2060 7333 5f64 6174 615f 6e61 6d69  or `s3_data_nami
+00001e80: 6e67 603a 0a2a 2060 7575 6964 603a 2060  ng`:.* `uuid`: `
+00001e90: 7b73 335f 6461 7461 5f64 6972 7d2f 7b75  {s3_data_dir}/{u
+00001ea0: 7569 6434 2829 7d2f 600a 2a20 6074 6162  uid4()}/`.* `tab
+00001eb0: 6c65 5f74 6162 6c65 603a 2060 7b73 335f  le_table`: `{s3_
+00001ec0: 6461 7461 5f64 6972 7d2f 7b74 6162 6c65  data_dir}/{table
+00001ed0: 7d2f 600a 2a20 6074 6162 6c65 5f75 6e69  }/`.* `table_uni
+00001ee0: 7175 6560 3a20 607b 7333 5f64 6174 615f  que`: `{s3_data_
+00001ef0: 6469 727d 2f7b 7461 626c 657d 2f7b 7575  dir}/{table}/{uu
+00001f00: 6964 3428 297d 2f60 0a2a 2060 7363 6865  id4()}/`.* `sche
+00001f10: 6d61 5f74 6162 6c65 603a 2060 7b73 335f  ma_table`: `{s3_
+00001f20: 6461 7461 5f64 6972 7d2f 7b73 6368 656d  data_dir}/{schem
+00001f30: 617d 2f7b 7461 626c 657d 2f60 0a2a 2060  a}/{table}/`.* `
+00001f40: 7333 5f64 6174 615f 6e61 6d69 6e67 3d73  s3_data_naming=s
+00001f50: 6368 656d 615f 7461 626c 655f 756e 6971  chema_table_uniq
+00001f60: 7565 603a 2060 7b73 335f 6461 7461 5f64  ue`: `{s3_data_d
+00001f70: 6972 7d2f 7b73 6368 656d 617d 2f7b 7461  ir}/{schema}/{ta
+00001f80: 626c 657d 2f7b 7575 6964 3428 297d 2f60  ble}/{uuid4()}/`
+00001f90: 0a0a 4974 2773 2070 6f73 7369 626c 6520  ..It's possible 
+00001fa0: 746f 2073 6574 2074 6865 2060 7333 5f64  to set the `s3_d
+00001fb0: 6174 615f 6e61 6d69 6e67 6020 676c 6f62  ata_naming` glob
+00001fc0: 616c 6c79 2069 6e20 7468 6520 7461 7267  ally in the targ
+00001fd0: 6574 2070 726f 6669 6c65 2c20 6f72 206f  et profile, or o
+00001fe0: 7665 7277 7269 7465 2074 6865 2076 616c  verwrite the val
+00001ff0: 7565 2069 6e20 7468 6520 7461 626c 6520  ue in the table 
+00002000: 636f 6e66 6967 2c0a 6f72 2073 6574 7469  config,.or setti
+00002010: 6e67 2075 7020 7468 6520 7661 6c75 6520  ng up the value 
+00002020: 666f 7220 6772 6f75 7073 206f 6620 6d6f  for groups of mo
+00002030: 6465 6c20 696e 2064 6274 5f70 726f 6a65  del in dbt_proje
+00002040: 6374 2e79 6d6c 2e0a 0a3e 204e 6f74 653a  ct.yml...> Note:
+00002050: 2077 6865 6e20 7573 696e 6720 6120 776f   when using a wo
+00002060: 726b 2067 726f 7570 2077 6974 6820 6120  rk group with a 
+00002070: 6465 6661 756c 7420 6f75 7470 7574 206c  default output l
+00002080: 6f63 6174 696f 6e20 636f 6e66 6967 7572  ocation configur
+00002090: 6564 2c20 6073 335f 6461 7461 5f6e 616d  ed, `s3_data_nam
+000020a0: 696e 6760 2061 6e64 2061 6e79 2063 6f6e  ing` and any con
+000020b0: 6669 6775 7265 6420 6275 636b 6574 7320  figured buckets 
+000020c0: 6172 6520 6967 6e6f 7265 6420 616e 6420  are ignored and 
+000020d0: 7468 6520 6c6f 6361 7469 6f6e 2063 6f6e  the location con
+000020e0: 6669 6775 7265 6420 696e 2074 6865 2077  figured in the w
+000020f0: 6f72 6b20 6772 6f75 7020 6973 2075 7365  ork group is use
+00002100: 642e 0a0a 2323 2320 496e 6372 656d 656e  d...### Incremen
+00002110: 7461 6c20 6d6f 6465 6c73 0a0a 5375 7070  tal models..Supp
+00002120: 6f72 7420 666f 7220 5b69 6e63 7265 6d65  ort for [increme
+00002130: 6e74 616c 206d 6f64 656c 735d 2868 7474  ntal models](htt
+00002140: 7073 3a2f 2f64 6f63 732e 6765 7464 6274  ps://docs.getdbt
+00002150: 2e63 6f6d 2f64 6f63 732f 6275 696c 642f  .com/docs/build/
+00002160: 696e 6372 656d 656e 7461 6c2d 6d6f 6465  incremental-mode
+00002170: 6c73 292e 0a0a 5468 6573 6520 7374 7261  ls)...These stra
+00002180: 7465 6769 6573 2061 7265 2073 7570 706f  tegies are suppo
+00002190: 7274 6564 3a0a 0a2a 2060 696e 7365 7274  rted:..* `insert
+000021a0: 5f6f 7665 7277 7269 7465 6020 2864 6566  _overwrite` (def
+000021b0: 6175 6c74 293a 2054 6865 2069 6e73 6572  ault): The inser
+000021c0: 7420 6f76 6572 7772 6974 6520 7374 7261  t overwrite stra
+000021d0: 7465 6779 2064 656c 6574 6573 2074 6865  tegy deletes the
+000021e0: 206f 7665 726c 6170 7069 6e67 2070 6172   overlapping par
+000021f0: 7469 7469 6f6e 7320 6672 6f6d 2074 6865  titions from the
+00002200: 2064 6573 7469 6e61 7469 6f6e 0a74 6162   destination.tab
+00002210: 6c65 2c20 616e 6420 7468 656e 2069 6e73  le, and then ins
+00002220: 6572 7473 2074 6865 206e 6577 2072 6563  erts the new rec
+00002230: 6f72 6473 2066 726f 6d20 7468 6520 736f  ords from the so
+00002240: 7572 6365 2e20 5468 6973 2073 7472 6174  urce. This strat
+00002250: 6567 7920 6465 7065 6e64 7320 6f6e 2074  egy depends on t
+00002260: 6865 2060 7061 7274 6974 696f 6e65 645f  he `partitioned_
+00002270: 6279 6020 6b65 7977 6f72 6421 2049 6620  by` keyword! If 
+00002280: 6e6f 0a70 6172 7469 7469 6f6e 7320 6172  no.partitions ar
+00002290: 6520 6465 6669 6e65 642c 2064 6274 2077  e defined, dbt w
+000022a0: 696c 6c20 6661 6c6c 2062 6163 6b20 746f  ill fall back to
+000022b0: 2074 6865 2060 6170 7065 6e64 6020 7374   the `append` st
+000022c0: 7261 7465 6779 2e0a 2a20 6061 7070 656e  rategy..* `appen
+000022d0: 6460 3a20 496e 7365 7274 206e 6577 2072  d`: Insert new r
+000022e0: 6563 6f72 6473 2077 6974 686f 7574 2075  ecords without u
+000022f0: 7064 6174 696e 672c 2064 656c 6574 696e  pdating, deletin
+00002300: 6720 6f72 206f 7665 7277 7269 7469 6e67  g or overwriting
+00002310: 2061 6e79 2065 7869 7374 696e 6720 6461   any existing da
+00002320: 7461 2e20 5468 6572 6520 6d69 6768 7420  ta. There might 
+00002330: 6265 2064 7570 6c69 6361 7465 0a64 6174  be duplicate.dat
+00002340: 6120 2865 2e67 2e20 6772 6561 7420 666f  a (e.g. great fo
+00002350: 7220 6c6f 6720 6f72 2068 6973 746f 7269  r log or histori
+00002360: 6361 6c20 6461 7461 292e 0a2a 2060 6d65  cal data)..* `me
+00002370: 7267 6560 3a20 436f 6e64 6974 696f 6e61  rge`: Conditiona
+00002380: 6c6c 7920 7570 6461 7465 732c 2064 656c  lly updates, del
+00002390: 6574 6573 2c20 6f72 2069 6e73 6572 7473  etes, or inserts
+000023a0: 2072 6f77 7320 696e 746f 2061 6e20 4963   rows into an Ic
+000023b0: 6562 6572 6720 7461 626c 652e 2055 7365  eberg table. Use
+000023c0: 6420 696e 2063 6f6d 6269 6e61 7469 6f6e  d in combination
+000023d0: 2077 6974 6820 6075 6e69 7175 655f 6b65   with `unique_ke
+000023e0: 7960 2e0a 4f6e 6c79 2061 7661 696c 6162  y`..Only availab
+000023f0: 6c65 2077 6865 6e20 7573 696e 6720 4963  le when using Ic
+00002400: 6562 6572 672e 0a0a 2323 2320 4f6e 2073  eberg...### On s
+00002410: 6368 656d 6120 6368 616e 6765 0a0a 606f  chema change..`o
+00002420: 6e5f 7363 6865 6d61 5f63 6861 6e67 6560  n_schema_change`
+00002430: 2069 7320 616e 206f 7074 696f 6e20 746f   is an option to
+00002440: 2072 6566 6c65 6374 2063 6861 6e67 6573   reflect changes
+00002450: 206f 6620 7363 6865 6d61 2069 6e20 696e   of schema in in
+00002460: 6372 656d 656e 7461 6c20 6d6f 6465 6c73  cremental models
+00002470: 2e0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
+00002480: 6f70 7469 6f6e 7320 6172 6520 7375 7070  options are supp
+00002490: 6f72 7465 643a 0a2a 2060 6967 6e6f 7265  orted:.* `ignore
+000024a0: 6020 2864 6566 6175 6c74 290a 2a20 6066  ` (default).* `f
+000024b0: 6169 6c60 0a2a 2060 6170 7065 6e64 5f6e  ail`.* `append_n
+000024c0: 6577 5f63 6f6c 756d 6e73 600a 2a20 6073  ew_columns`.* `s
+000024d0: 796e 635f 616c 6c5f 636f 6c75 6d6e 7360  ync_all_columns`
+000024e0: 0a0a 496e 2064 6574 6169 6c2c 2070 6c65  ..In detail, ple
+000024f0: 6173 6520 7265 6665 7220 746f 205b 6462  ase refer to [db
+00002500: 7420 646f 6373 5d28 6874 7470 733a 2f2f  t docs](https://
+00002510: 646f 6373 2e67 6574 6462 742e 636f 6d2f  docs.getdbt.com/
+00002520: 646f 6373 2f62 7569 6c64 2f69 6e63 7265  docs/build/incre
+00002530: 6d65 6e74 616c 2d6d 6f64 656c 7323 7768  mental-models#wh
+00002540: 6174 2d69 662d 7468 652d 636f 6c75 6d6e  at-if-the-column
+00002550: 732d 6f66 2d6d 792d 696e 6372 656d 656e  s-of-my-incremen
+00002560: 7461 6c2d 6d6f 6465 6c2d 6368 616e 6765  tal-model-change
+00002570: 292e 0a0a 2323 2320 4963 6562 6572 670a  )...### Iceberg.
+00002580: 0a54 6865 2061 6461 7074 6572 2073 7570  .The adapter sup
+00002590: 706f 7274 7320 7461 626c 6520 6d61 7465  ports table mate
+000025a0: 7269 616c 697a 6174 696f 6e20 666f 7220  rialization for 
+000025b0: 4963 6562 6572 672e 0a0a 546f 2067 6574  Iceberg...To get
+000025c0: 2073 7461 7274 6564 206a 7573 7420 6164   started just ad
+000025d0: 6420 7468 6973 2061 7320 796f 7572 206d  d this as your m
+000025e0: 6f64 656c 3a0a 6060 600a 7b7b 2063 6f6e  odel:.```.{{ con
+000025f0: 6669 6728 0a20 2020 206d 6174 6572 6961  fig(.    materia
+00002600: 6c69 7a65 643d 2774 6162 6c65 272c 0a20  lized='table',. 
+00002610: 2020 2074 6162 6c65 5f74 7970 653d 2769     table_type='i
+00002620: 6365 6265 7267 272c 0a20 2020 2066 6f72  ceberg',.    for
+00002630: 6d61 743d 2770 6172 7175 6574 272c 0a20  mat='parquet',. 
+00002640: 2020 2070 6172 7469 7469 6f6e 6564 5f62     partitioned_b
+00002650: 793d 5b27 6275 636b 6574 2875 7365 725f  y=['bucket(user_
+00002660: 6964 2c20 3529 275d 2c0a 2020 2020 7461  id, 5)'],.    ta
+00002670: 626c 655f 7072 6f70 6572 7469 6573 3d7b  ble_properties={
+00002680: 0a20 2020 2009 276f 7074 696d 697a 655f  .    .'optimize_
+00002690: 7265 7772 6974 655f 6465 6c65 7465 5f66  rewrite_delete_f
+000026a0: 696c 655f 7468 7265 7368 6f6c 6427 3a20  ile_threshold': 
+000026b0: 2732 270a 2020 2020 097d 0a29 207d 7d0a  '2'.    .}.) }}.
+000026c0: 0a53 454c 4543 540a 0927 4127 2041 5320  .SELECT..'A' AS 
+000026d0: 7573 6572 5f69 642c 0a09 2770 6927 2041  user_id,..'pi' A
+000026e0: 5320 6e61 6d65 2c0a 0927 6163 7469 7665  S name,..'active
+000026f0: 2720 4153 2073 7461 7475 732c 0a09 3137  ' AS status,..17
+00002700: 2e38 3920 4153 2063 6f73 742c 0a09 3120  .89 AS cost,..1 
+00002710: 4153 2071 7561 6e74 6974 792c 0a09 3130  AS quantity,..10
+00002720: 3030 3030 3030 3020 4153 2071 7561 6e74  0000000 AS quant
+00002730: 6974 795f 6269 672c 0a09 6375 7272 656e  ity_big,..curren
+00002740: 745f 6461 7465 2041 5320 6d79 5f64 6174  t_date AS my_dat
+00002750: 650a 6060 600a 0a49 6365 6265 7267 2073  e.```..Iceberg s
+00002760: 7570 706f 7274 7320 6275 636b 6574 696e  upports bucketin
+00002770: 6720 6173 2068 6964 6465 6e20 7061 7274  g as hidden part
+00002780: 6974 696f 6e73 2c20 7468 6572 6566 6f72  itions, therefor
+00002790: 6520 7573 6520 7468 6520 6070 6172 7469  e use the `parti
+000027a0: 7469 6f6e 6564 5f62 7960 2063 6f6e 6669  tioned_by` confi
+000027b0: 6720 746f 2061 6464 2073 7065 6369 6669  g to add specifi
+000027c0: 6320 6275 636b 6574 696e 6720 636f 6e64  c bucketing cond
+000027d0: 6974 696f 6e73 2e0a 0a49 6365 6265 7267  itions...Iceberg
+000027e0: 2073 7570 706f 7274 7320 7365 7665 7261   supports severa
+000027f0: 6c20 7461 626c 6520 666f 726d 6174 7320  l table formats 
+00002800: 666f 7220 6461 7461 203a 2060 5041 5251  for data : `PARQ
+00002810: 5545 5460 2c20 6041 5652 4f60 2061 6e64  UET`, `AVRO` and
+00002820: 2060 4f52 4360 2e0a 0a49 7420 6973 2070   `ORC`...It is p
+00002830: 6f73 7369 626c 6520 746f 2075 7365 2069  ossible to use i
+00002840: 6365 6265 7267 2069 6e20 616e 2069 6e63  ceberg in an inc
+00002850: 7265 6d65 6e74 616c 2066 6173 6869 6f6e  remental fashion
+00002860: 2c20 7370 6563 6966 6963 616c 6c79 2032  , specifically 2
+00002870: 2073 7472 6174 6567 6965 7320 6172 6520   strategies are 
+00002880: 7375 7070 6f72 7465 643a 0a2a 2060 6170  supported:.* `ap
+00002890: 7065 6e64 603a 206e 6577 2072 6563 6f72  pend`: new recor
+000028a0: 6473 2061 7265 2061 7070 656e 6465 6420  ds are appended 
+000028b0: 746f 2074 6865 2074 6162 6c65 2c20 7468  to the table, th
+000028c0: 6973 2063 616e 206c 6561 6420 746f 2064  is can lead to d
+000028d0: 7570 6c69 6361 7465 730a 2a20 606d 6572  uplicates.* `mer
+000028e0: 6765 603a 206d 7573 7420 6265 2075 7365  ge`: must be use
+000028f0: 6420 696e 2063 6f6d 6269 6e61 7469 6f6e  d in combination
+00002900: 2077 6974 6820 6075 6e69 7175 655f 6b65   with `unique_ke
+00002910: 7960 2061 6e64 2069 7427 7320 6f6e 6c79  y` and it's only
+00002920: 2061 7661 696c 6162 6c65 2077 6974 6820   available with 
+00002930: 456e 6769 6e65 2076 6572 7369 6f6e 2033  Engine version 3
+00002940: 2e0a 2020 2049 7420 7065 7266 6f72 6d73  ..   It performs
+00002950: 2061 6e20 7570 7365 7274 2c20 6e65 7720   an upsert, new 
+00002960: 7265 636f 7264 2061 7265 2061 6464 6564  record are added
+00002970: 2c20 616e 6420 7265 636f 7264 2061 6c72  , and record alr
+00002980: 6561 6479 2065 7869 7374 696e 6720 6172  eady existing ar
+00002990: 6520 7570 6461 7465 640a 0a23 2323 2048  e updated..### H
+000029a0: 6967 6820 6176 6169 6c61 626c 6520 7461  igh available ta
+000029b0: 626c 6520 6d61 7465 7269 616c 697a 6174  ble materializat
+000029c0: 696f 6e0a 5468 6520 6375 7272 656e 7420  ion.The current 
+000029d0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+000029e0: 6620 7468 6520 7461 626c 6520 6d61 7465  f the table mate
+000029f0: 7269 616c 697a 6174 696f 6e20 6361 6e20  rialization can 
+00002a00: 6c65 6164 2074 6f20 646f 776e 7469 6d65  lead to downtime
+00002a10: 2c20 6173 2074 6172 6765 7420 7461 626c  , as target tabl
+00002a20: 6520 6973 2064 726f 7070 6564 2061 6e64  e is dropped and
+00002a30: 2072 652d 6372 6561 7465 642e 0a54 6f20   re-created..To 
+00002a40: 6861 7665 2074 6865 206c 6573 7320 6465  have the less de
+00002a50: 7374 7275 6374 6976 6520 6265 6861 7669  structive behavi
+00002a60: 6f72 2069 7427 7320 706f 7373 6962 6c65  or it's possible
+00002a70: 2074 6f20 7573 6520 6074 6162 6c65 3d27   to use `table='
+00002a80: 7461 626c 655f 6869 7665 5f68 6127 6020  table_hive_ha'` 
+00002a90: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
+00002aa0: 0a2a 2a74 6162 6c65 5f68 6976 655f 6861  .**table_hive_ha
+00002ab0: 2a2a 206c 6576 6572 6167 6520 7468 6520  ** leverage the 
+00002ac0: 7461 626c 6520 7665 7273 696f 6e73 2066  table versions f
+00002ad0: 6561 7475 7265 206f 6620 676c 7565 2063  eature of glue c
+00002ae0: 6174 616c 6f67 2c20 6372 6561 7469 6e67  atalog, creating
+00002af0: 2061 2074 6d70 2074 6162 6c65 2061 6e64   a tmp table and
+00002b00: 2073 7761 7070 696e 670a 7468 6520 7461   swapping.the ta
+00002b10: 7267 6574 2074 6162 6c65 2074 6f20 7468  rget table to th
+00002b20: 6520 6c6f 6361 7469 6f6e 206f 6620 7468  e location of th
+00002b30: 6520 746d 7020 7461 626c 652e 0a54 6869  e tmp table..Thi
+00002b40: 7320 6d61 7465 7269 616c 697a 6174 696f  s materializatio
+00002b50: 6e20 6973 206f 6e6c 7920 6176 6169 6c61  n is only availa
+00002b60: 626c 6520 666f 7220 6074 6162 6c65 5f74  ble for `table_t
+00002b70: 7970 653d 6869 7665 6020 616e 6420 7265  ype=hive` and re
+00002b80: 7175 6972 6573 2075 7369 6e67 2075 6e69  quires using uni
+00002b90: 7175 6520 6c6f 6361 7469 6f6e 732e 0a0a  que locations...
+00002ba0: 6060 600a 7b7b 2063 6f6e 6669 6728 0a20  ```.{{ config(. 
+00002bb0: 2020 206d 6174 6572 6961 6c69 7a65 643d     materialized=
+00002bc0: 2774 6162 6c65 5f68 6976 655f 6861 272c  'table_hive_ha',
+00002bd0: 0a20 2020 2066 6f72 6d61 743d 2770 6172  .    format='par
+00002be0: 7175 6574 272c 0a20 2020 2070 6172 7469  quet',.    parti
+00002bf0: 7469 6f6e 5f62 793d 5b27 7374 6174 7573  tion_by=['status
+00002c00: 275d 2c0a 2020 2020 7333 5f64 6174 615f  '],.    s3_data_
+00002c10: 6e61 6d69 6e67 3d27 7461 626c 655f 756e  naming='table_un
+00002c20: 6971 7565 270a 2920 7d7d 0a0a 7365 6c65  ique'.) }}..sele
+00002c30: 6374 0a20 2027 6127 2061 7320 7573 6572  ct.  'a' as user
+00002c40: 5f69 642c 0a20 2027 7069 2720 6173 2075  _id,.  'pi' as u
+00002c50: 7365 725f 6e61 6d65 2c0a 2020 2761 6374  ser_name,.  'act
+00002c60: 6976 6527 2061 7320 7374 6174 7573 0a75  ive' as status.u
+00002c70: 6e69 6f6e 2061 6c6c 0a73 656c 6563 740a  nion all.select.
+00002c80: 2020 2762 2720 6173 2075 7365 725f 6964    'b' as user_id
+00002c90: 2c0a 2020 2773 6827 2061 7320 7573 6572  ,.  'sh' as user
+00002ca0: 5f6e 616d 652c 0a20 2027 6469 7361 626c  _name,.  'disabl
+00002cb0: 6564 2720 6173 2073 7461 7475 730a 6060  ed' as status.``
+00002cc0: 600a 0a42 7920 6465 6661 756c 742c 2074  `..By default, t
+00002cd0: 6865 206d 6174 6572 6961 6c69 7a61 7469  he materializati
+00002ce0: 6f6e 206b 6565 7073 2074 6865 206c 6173  on keeps the las
+00002cf0: 7420 3420 7461 626c 6520 7665 7273 696f  t 4 table versio
+00002d00: 6e73 2c20 796f 7520 6361 6e20 6368 616e  ns, you can chan
+00002d10: 6765 2069 7420 7468 6174 2073 6574 7469  ge it that setti
+00002d20: 6e67 2060 7665 7273 696f 6e73 5f74 6f5f  ng `versions_to_
+00002d30: 6b65 6570 602e 0a0a 2323 2323 204b 6e6f  keep`...#### Kno
+00002d40: 776e 2069 7373 7565 730a 2a20 5768 656e  wn issues.* When
+00002d50: 2073 7761 7070 696e 6720 6672 6f6d 2061   swapping from a
+00002d60: 2074 6162 6c65 2077 6974 6820 7061 7274   table with part
+00002d70: 6974 696f 6e73 2074 6f20 6120 7461 626c  itions to a tabl
+00002d80: 6520 7769 7468 6f75 7420 2861 6e64 2074  e without (and t
+00002d90: 6865 206f 7468 6572 2077 6179 2061 726f  he other way aro
+00002da0: 756e 6429 2c20 7468 6572 6520 636f 756c  und), there coul
+00002db0: 6420 6265 2061 206c 6974 746c 6520 646f  d be a little do
+00002dc0: 776e 7469 6d65 2e0a 2020 496e 2063 6173  wntime..  In cas
+00002dd0: 6520 6869 6768 2070 6572 666f 726d 616e  e high performan
+00002de0: 6365 7320 6172 6520 6e65 6564 6564 2063  ces are needed c
+00002df0: 6f6e 7369 6465 7220 6275 636b 6574 696e  onsider bucketin
+00002e00: 6720 696e 7374 6561 6420 6f66 2070 6172  g instead of par
+00002e10: 7469 7469 6f6e 730a 2a20 4279 2064 6566  titions.* By def
+00002e20: 6175 6c74 2c20 476c 7565 2022 6475 706c  ault, Glue "dupl
+00002e30: 6963 6174 6522 2074 6865 2076 6572 7369  icate" the versi
+00002e40: 6f6e 7320 696e 7465 726e 616c 6c79 2c20  ons internally, 
+00002e50: 736f 2074 6865 206c 6173 7420 3220 7665  so the last 2 ve
+00002e60: 7273 696f 6e73 206f 6620 6120 7461 626c  rsions of a tabl
+00002e70: 6520 706f 696e 7420 746f 2074 6865 2073  e point to the s
+00002e80: 616d 6520 6c6f 6361 7469 6f6e 0a2a 2049  ame location.* I
+00002e90: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+00002ea0: 746f 2068 6176 6520 7665 7273 696f 6e73  to have versions
+00002eb0: 5f74 6f5f 6b65 6570 3e3d 2034 2c20 6173  _to_keep>= 4, as
+00002ec0: 2074 6869 7320 7769 6c6c 2061 766f 6964   this will avoid
+00002ed0: 2074 6f20 6861 7665 2074 6865 206f 6c64   to have the old
+00002ee0: 6572 206c 6f63 6174 696f 6e20 7265 6d6f  er location remo
+00002ef0: 7665 640a 2a20 5468 6520 6d61 6372 6f20  ved.* The macro 
+00002f00: 6174 6865 6e61 5f5f 656e 645f 6f66 5f74  athena__end_of_t
+00002f10: 696d 6520 6e65 6564 7320 746f 2062 6520  ime needs to be 
+00002f20: 6f76 6572 7772 6974 7465 6e20 6279 2074  overwritten by t
+00002f30: 6865 2075 7365 7220 6966 2075 7369 6e67  he user if using
+00002f40: 2041 7468 656e 6120 7633 2073 696e 6365   Athena v3 since
+00002f50: 2069 7420 7265 7175 6972 6573 2061 2070   it requires a p
+00002f60: 7265 6369 7369 6f6e 2070 6172 616d 6574  recision paramet
+00002f70: 6572 2066 6f72 2074 696d 6573 7461 6d70  er for timestamp
+00002f80: 730a 0a0a 2323 2053 6e61 7073 686f 7473  s...## Snapshots
+00002f90: 0a0a 5468 6520 6164 6170 7465 7220 7375  ..The adapter su
+00002fa0: 7070 6f72 7473 2073 6e61 7073 686f 7420  pports snapshot 
+00002fb0: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
+00002fc0: 2049 7420 7375 7070 6f72 7473 2062 6f74   It supports bot
+00002fd0: 6820 7469 6d65 7374 616d 7020 616e 6420  h timestamp and 
+00002fe0: 6368 6563 6b20 7374 7261 7465 6779 2e20  check strategy. 
+00002ff0: 546f 2063 7265 6174 6520 6120 736e 6170  To create a snap
+00003000: 7368 6f74 2063 7265 6174 6520 6120 736e  shot create a sn
+00003010: 6170 7368 6f74 2066 696c 6520 696e 2074  apshot file in t
+00003020: 6865 2073 6e61 7073 686f 7473 2064 6972  he snapshots dir
+00003030: 6563 746f 7279 2e20 4966 2064 6972 6563  ectory. If direc
+00003040: 746f 7279 2064 6f65 7320 6e6f 7420 6578  tory does not ex
+00003050: 6973 7420 6372 6561 7465 206f 6e65 2e0a  ist create one..
+00003060: 0a23 2323 2054 696d 6573 7461 6d70 2073  .### Timestamp s
+00003070: 7472 6174 6567 790a 0a54 6f20 7573 6520  trategy..To use 
+00003080: 7468 6520 7469 6d65 7374 616d 7020 7374  the timestamp st
+00003090: 7261 7465 6779 2072 6566 6572 2074 6f20  rategy refer to 
+000030a0: 7468 6520 5b64 6274 2064 6f63 735d 2868  the [dbt docs](h
+000030b0: 7474 7073 3a2f 2f64 6f63 732e 6765 7464  ttps://docs.getd
+000030c0: 6274 2e63 6f6d 2f64 6f63 732f 6275 696c  bt.com/docs/buil
+000030d0: 642f 736e 6170 7368 6f74 7323 7469 6d65  d/snapshots#time
+000030e0: 7374 616d 702d 7374 7261 7465 6779 2d72  stamp-strategy-r
+000030f0: 6563 6f6d 6d65 6e64 6564 290a 0a23 2323  ecommended)..###
+00003100: 2043 6865 636b 2073 7472 6174 6567 790a   Check strategy.
+00003110: 0a54 6f20 7573 6520 7468 6520 6368 6563  .To use the chec
+00003120: 6b20 7374 7261 7465 6779 2072 6566 6572  k strategy refer
+00003130: 2074 6f20 7468 6520 5b64 6274 2064 6f63   to the [dbt doc
+00003140: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
+00003150: 6765 7464 6274 2e63 6f6d 2f64 6f63 732f  getdbt.com/docs/
+00003160: 6275 696c 642f 736e 6170 7368 6f74 7323  build/snapshots#
+00003170: 6368 6563 6b2d 7374 7261 7465 6779 290a  check-strategy).
+00003180: 0a23 2323 2048 6172 642d 6465 6c65 7465  .### Hard-delete
+00003190: 730a 0a54 6865 206d 6174 6572 6961 6c69  s..The materiali
+000031a0: 7a61 7469 6f6e 2061 6c73 6f20 7375 7070  zation also supp
+000031b0: 6f72 7473 2069 6e76 616c 6964 6174 696e  orts invalidatin
+000031c0: 6720 6861 7264 2064 656c 6574 6573 2e20  g hard deletes. 
+000031d0: 4368 6563 6b20 7468 6520 5b64 6f63 735d  Check the [docs]
+000031e0: 2868 7474 7073 3a2f 2f64 6f63 732e 6765  (https://docs.ge
+000031f0: 7464 6274 2e63 6f6d 2f64 6f63 732f 6275  tdbt.com/docs/bu
+00003200: 696c 642f 736e 6170 7368 6f74 7323 6861  ild/snapshots#ha
+00003210: 7264 2d64 656c 6574 6573 2d6f 7074 2d69  rd-deletes-opt-i
+00003220: 6e29 2074 6f20 756e 6465 7273 7461 6e64  n) to understand
+00003230: 2075 7361 6765 2e0a 0a23 2323 2057 6f72   usage...### Wor
+00003240: 6b69 6e67 2065 7861 6d70 6c65 0a0a 7365  king example..se
+00003250: 6564 2066 696c 6520 2d20 656d 706c 6f79  ed file - employ
+00003260: 656e 745f 696e 6469 6361 746f 7273 5f6e  ent_indicators_n
+00003270: 6f76 656d 6265 725f 3230 3232 5f63 7376  ovember_2022_csv
+00003280: 5f74 6162 6c65 732e 6373 760a 6060 600a  _tables.csv.```.
+00003290: 5365 7269 6573 5f72 6566 6572 656e 6365  Series_reference
+000032a0: 2c50 6572 696f 642c 4461 7461 5f76 616c  ,Period,Data_val
+000032b0: 7565 2c53 7570 7072 6573 7365 640a 4d45  ue,Suppressed.ME
+000032c0: 494d 2e53 3157 412c 3139 3939 2e30 342c  IM.S1WA,1999.04,
+000032d0: 3830 3236 372c 0a4d 4549 4d2e 5331 5741  80267,.MEIM.S1WA
+000032e0: 2c31 3939 392e 3035 2c37 3038 3033 2c0a  ,1999.05,70803,.
+000032f0: 4d45 494d 2e53 3157 412c 3139 3939 2e30  MEIM.S1WA,1999.0
+00003300: 362c 3635 3739 322c 0a4d 4549 4d2e 5331  6,65792,.MEIM.S1
+00003310: 5741 2c31 3939 392e 3037 2c36 3631 3934  WA,1999.07,66194
+00003320: 2c0a 4d45 494d 2e53 3157 412c 3139 3939  ,.MEIM.S1WA,1999
+00003330: 2e30 382c 3637 3235 392c 0a4d 4549 4d2e  .08,67259,.MEIM.
+00003340: 5331 5741 2c31 3939 392e 3039 2c36 3936  S1WA,1999.09,696
+00003350: 3931 2c0a 4d45 494d 2e53 3157 412c 3139  91,.MEIM.S1WA,19
+00003360: 3939 2e31 2c37 3234 3735 2c0a 4d45 494d  99.1,72475,.MEIM
+00003370: 2e53 3157 412c 3139 3939 2e31 312c 3739  .S1WA,1999.11,79
+00003380: 3236 332c 0a4d 4549 4d2e 5331 5741 2c31  263,.MEIM.S1WA,1
+00003390: 3939 392e 3132 2c38 3635 3430 2c0a 4d45  999.12,86540,.ME
+000033a0: 494d 2e53 3157 412c 3230 3030 2e30 312c  IM.S1WA,2000.01,
+000033b0: 3832 3535 322c 0a4d 4549 4d2e 5331 5741  82552,.MEIM.S1WA
+000033c0: 2c32 3030 302e 3032 2c38 3137 3039 2c0a  ,2000.02,81709,.
+000033d0: 4d45 494d 2e53 3157 412c 3230 3030 2e30  MEIM.S1WA,2000.0
+000033e0: 332c 3834 3132 362c 0a4d 4549 4d2e 5331  3,84126,.MEIM.S1
+000033f0: 5741 2c32 3030 302e 3034 2c37 3730 3839  WA,2000.04,77089
+00003400: 2c0a 4d45 494d 2e53 3157 412c 3230 3030  ,.MEIM.S1WA,2000
+00003410: 2e30 352c 3733 3831 312c 0a4d 4549 4d2e  .05,73811,.MEIM.
+00003420: 5331 5741 2c32 3030 302e 3036 2c37 3030  S1WA,2000.06,700
+00003430: 3730 2c0a 4d45 494d 2e53 3157 412c 3230  70,.MEIM.S1WA,20
+00003440: 3030 2e30 372c 3639 3837 332c 0a4d 4549  00.07,69873,.MEI
+00003450: 4d2e 5331 5741 2c32 3030 302e 3038 2c37  M.S1WA,2000.08,7
+00003460: 3134 3638 2c0a 4d45 494d 2e53 3157 412c  1468,.MEIM.S1WA,
+00003470: 3230 3030 2e30 392c 3732 3436 322c 0a4d  2000.09,72462,.M
+00003480: 4549 4d2e 5331 5741 2c32 3030 302e 312c  EIM.S1WA,2000.1,
+00003490: 3734 3839 372c 0a60 6060 0a0a 6d6f 6465  74897,.```..mode
+000034a0: 6c2e 7371 6c0a 6060 600a 7b7b 2063 6f6e  l.sql.```.{{ con
+000034b0: 6669 6728 0a20 2020 206d 6174 6572 6961  fig(.    materia
+000034c0: 6c69 7a65 643d 2774 6162 6c65 270a 2920  lized='table'.) 
+000034d0: 7d7d 0a0a 5345 4c45 4354 0a20 2020 2052  }}..SELECT.    R
+000034e0: 4f57 5f4e 554d 4245 5228 2920 4f56 4552  OW_NUMBER() OVER
+000034f0: 2028 2920 4153 2069 640a 2020 2020 2c20   () AS id.    , 
+00003500: 2a0a 2020 2020 2c20 6361 7374 2866 726f  *.    , cast(fro
+00003510: 6d5f 756e 6978 7469 6d65 2874 6f5f 756e  m_unixtime(to_un
+00003520: 6978 7469 6d65 286e 6f77 2829 2929 2061  ixtime(now())) a
+00003530: 7320 7469 6d65 7374 616d 7028 3629 2920  s timestamp(6)) 
+00003540: 4153 2072 6566 7265 7368 5f74 696d 6573  AS refresh_times
+00003550: 7461 6d70 0a46 524f 4d20 7b7b 2072 6566  tamp.FROM {{ ref
+00003560: 2827 656d 706c 6f79 6d65 6e74 5f69 6e64  ('employment_ind
+00003570: 6963 6174 6f72 735f 6e6f 7665 6d62 6572  icators_november
+00003580: 5f32 3032 325f 6373 765f 7461 626c 6573  _2022_csv_tables
+00003590: 2729 207d 7d0a 6060 600a 0a74 696d 6573  ') }}.```..times
+000035a0: 7461 6d70 2073 7472 6174 6567 7920 2d20  tamp strategy - 
+000035b0: 6d6f 6465 6c5f 736e 6170 7368 6f74 5f31  model_snapshot_1
+000035c0: 0a0a 6060 600a 7b25 2073 6e61 7073 686f  ..```.{% snapsho
+000035d0: 7420 6d6f 6465 6c5f 736e 6170 7368 6f74  t model_snapshot
+000035e0: 5f31 2025 7d0a 0a7b 7b0a 2020 2020 636f  _1 %}..{{.    co
+000035f0: 6e66 6967 280a 2020 2020 2020 7374 7261  nfig(.      stra
+00003600: 7465 6779 3d27 7469 6d65 7374 616d 7027  tegy='timestamp'
+00003610: 2c0a 2020 2020 2020 7570 6461 7465 645f  ,.      updated_
+00003620: 6174 3d27 7265 6672 6573 685f 7469 6d65  at='refresh_time
+00003630: 7374 616d 7027 2c0a 2020 2020 2020 756e  stamp',.      un
+00003640: 6971 7565 5f6b 6579 3d27 6964 270a 2020  ique_key='id'.  
+00003650: 2020 290a 7d7d 0a0a 5345 4c45 4354 202a    ).}}..SELECT *
+00003660: 0a0a 6672 6f6d 207b 7b20 7265 6628 276d  ..from {{ ref('m
+00003670: 6f64 656c 2729 207d 7d0a 0a7b 2520 656e  odel') }}..{% en
+00003680: 6473 6e61 7073 686f 7420 257d 0a60 6060  dsnapshot %}.```
+00003690: 0a0a 696e 7661 6c69 6461 7465 2068 6172  ..invalidate har
+000036a0: 6420 6465 6c65 7465 7320 2d20 6d6f 6465  d deletes - mode
+000036b0: 6c5f 736e 6170 7368 6f74 5f32 0a60 6060  l_snapshot_2.```
+000036c0: 0a7b 2520 736e 6170 7368 6f74 206d 6f64  .{% snapshot mod
+000036d0: 656c 5f73 6e61 7073 686f 745f 3220 257d  el_snapshot_2 %}
+000036e0: 0a0a 7b7b 0a20 2020 2063 6f6e 6669 670a  ..{{.    config.
+000036f0: 2020 2020 280a 2020 2020 2020 2020 756e      (.        un
+00003700: 6971 7565 5f6b 6579 3d27 6964 272c 0a20  ique_key='id',. 
+00003710: 2020 2020 2020 2073 7472 6174 6567 793d         strategy=
+00003720: 2774 696d 6573 7461 6d70 272c 0a20 2020  'timestamp',.   
+00003730: 2020 2020 2075 7064 6174 6564 5f61 743d       updated_at=
+00003740: 2772 6566 7265 7368 5f74 696d 6573 7461  'refresh_timesta
+00003750: 6d70 272c 0a20 2020 2020 2020 2069 6e76  mp',.        inv
+00003760: 616c 6964 6174 655f 6861 7264 5f64 656c  alidate_hard_del
+00003770: 6574 6573 3d54 7275 652c 0a20 2020 2029  etes=True,.    )
+00003780: 0a7d 7d0a 5345 4c45 4354 202a 2066 726f  .}}.SELECT * fro
+00003790: 6d20 7b7b 2072 6566 2827 6d6f 6465 6c27  m {{ ref('model'
+000037a0: 2920 7d7d 0a0a 7b25 2065 6e64 736e 6170  ) }}..{% endsnap
+000037b0: 7368 6f74 2025 7d0a 6060 600a 0a63 6865  shot %}.```..che
+000037c0: 636b 2073 7472 6174 6567 7920 2d20 6d6f  ck strategy - mo
+000037d0: 6465 6c5f 736e 6170 7368 6f74 5f33 0a60  del_snapshot_3.`
+000037e0: 6060 0a7b 2520 736e 6170 7368 6f74 206d  ``.{% snapshot m
+000037f0: 6f64 656c 5f73 6e61 7073 686f 745f 3320  odel_snapshot_3 
+00003800: 257d 0a0a 7b7b 0a20 2020 2063 6f6e 6669  %}..{{.    confi
+00003810: 670a 2020 2020 280a 2020 2020 2020 2020  g.    (.        
+00003820: 756e 6971 7565 5f6b 6579 3d27 6964 272c  unique_key='id',
+00003830: 0a20 2020 2020 2020 2073 7472 6174 6567  .        strateg
+00003840: 793d 2763 6865 636b 272c 0a20 2020 2020  y='check',.     
+00003850: 2020 2063 6865 636b 5f63 6f6c 733d 5b27     check_cols=['
+00003860: 7365 7269 6573 5f72 6566 6572 656e 6365  series_reference
+00003870: 272c 2764 6174 615f 7661 6c75 6527 5d0a  ','data_value'].
+00003880: 2020 2020 290a 7d7d 0a53 454c 4543 5420      ).}}.SELECT 
+00003890: 2a20 6672 6f6d 207b 7b20 7265 6628 276d  * from {{ ref('m
+000038a0: 6f64 656c 2729 207d 7d0a 0a7b 2520 656e  odel') }}..{% en
+000038b0: 6473 6e61 7073 686f 7420 257d 0a60 6060  dsnapshot %}.```
+000038c0: 0a0a 2323 2320 4b6e 6f77 6e20 6973 7375  ..### Known issu
+000038d0: 6573 0a0a 2a20 496e 6372 656d 656e 7461  es..* Incrementa
+000038e0: 6c20 4963 6562 6572 6720 6d6f 6465 6c73  l Iceberg models
+000038f0: 202d 2053 796e 6320 616c 6c20 636f 6c75   - Sync all colu
+00003900: 6d6e 7320 6f6e 2073 6368 656d 6120 6368  mns on schema ch
+00003910: 616e 6765 2063 616e 2774 2072 656d 6f76  ange can't remov
+00003920: 6520 636f 6c75 6d6e 7320 7573 6564 2061  e columns used a
+00003930: 7320 7061 7274 6974 696f 6e69 6e67 2e0a  s partitioning..
+00003940: 5468 6520 6f6e 6c79 2077 6179 2c20 6672  The only way, fr
+00003950: 6f6d 2061 2064 6274 2070 6572 7370 6563  om a dbt perspec
+00003960: 7469 7665 2c20 6973 2074 6f20 646f 2061  tive, is to do a
+00003970: 2066 756c 6c2d 7265 6672 6573 6820 6f66   full-refresh of
+00003980: 2074 6865 2069 6e63 7265 6d65 6e74 616c   the incremental
+00003990: 206d 6f64 656c 2e0a 0a2a 2054 6162 6c65   model...* Table
+000039a0: 732c 2073 6368 656d 6173 2061 6e64 2064  s, schemas and d
+000039b0: 6174 6162 6173 6520 7368 6f75 6c64 206f  atabase should o
+000039c0: 6e6c 7920 6265 206c 6f77 6572 6361 7365  nly be lowercase
+000039d0: 0a0a 2a20 496e 206f 7264 6572 2074 6f20  ..* In order to 
+000039e0: 6176 6f69 6420 706f 7465 6e74 6961 6c20  avoid potential 
+000039f0: 636f 6e66 6c69 6374 732c 206d 616b 6520  conflicts, make 
+00003a00: 7375 7265 205b 6064 6274 2d61 7468 656e  sure [`dbt-athen
+00003a10: 612d 6164 6170 7465 7260 5d28 6874 7470  a-adapter`](http
+00003a20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00003a30: 6f6d 6d65 2f64 6274 2d61 7468 656e 6129  omme/dbt-athena)
+00003a40: 2069 7320 6e6f 7420 696e 7374 616c 6c65   is not installe
+00003a50: 6420 696e 2074 6865 2074 6172 6765 7420  d in the target 
+00003a60: 656e 7669 726f 6e6d 656e 742e 0a20 2053  environment..  S
+00003a70: 6565 2068 7474 7073 3a2f 2f67 6974 6875  ee https://githu
+00003a80: 622e 636f 6d2f 6462 742d 6174 6865 6e61  b.com/dbt-athena
+00003a90: 2f64 6274 2d61 7468 656e 612f 6973 7375  /dbt-athena/issu
+00003aa0: 6573 2f31 3033 2066 6f72 206d 6f72 6520  es/103 for more 
+00003ab0: 6465 7461 696c 732e 0a0a 2a20 536e 6170  details...* Snap
+00003ac0: 7368 6f74 2064 6f65 7320 6e6f 7420 7375  shot does not su
+00003ad0: 7070 6f72 7420 6472 6f70 7069 6e67 2063  pport dropping c
+00003ae0: 6f6c 756d 6e73 2066 726f 6d20 7468 6520  olumns from the 
+00003af0: 736f 7572 6365 2074 6162 6c65 2e20 4966  source table. If
+00003b00: 2079 6f75 2064 726f 7020 6120 636f 6c75   you drop a colu
+00003b10: 6d6e 206d 616b 6520 7375 7265 2074 6f20  mn make sure to 
+00003b20: 6472 6f70 2074 6865 2063 6f6c 756d 6e20  drop the column 
+00003b30: 6672 6f6d 2074 6865 2073 6e61 7073 686f  from the snapsho
+00003b40: 7420 6173 2077 656c 6c2e 2041 6e6f 7468  t as well. Anoth
+00003b50: 6572 2077 6f72 6b61 726f 756e 6420 6973  er workaround is
+00003b60: 2074 6f20 4e55 4c4c 2074 6865 2063 6f6c   to NULL the col
+00003b70: 756d 6e20 696e 2074 6865 2073 6e61 7073  umn in the snaps
+00003b80: 686f 7420 6465 6669 6e69 7469 6f6e 2074  hot definition t
+00003b90: 6f20 7072 6573 6572 7665 2068 6973 746f  o preserve histo
+00003ba0: 7279 0a0a 0a23 2320 436f 6e74 7269 6275  ry...## Contribu
+00003bb0: 7469 6e67 0a0a 5468 6973 2063 6f6e 6e65  ting..This conne
+00003bc0: 6374 6f72 2077 6f72 6b73 2077 6974 6820  ctor works with 
+00003bd0: 5079 7468 6f6e 2066 726f 6d20 332e 3720  Python from 3.7 
+00003be0: 746f 2033 2e31 312e 0a0a 2323 2320 4765  to 3.11...### Ge
+00003bf0: 7474 696e 6720 7374 6172 7465 640a 0a49  tting started..I
+00003c00: 6e20 6f72 6465 7220 746f 2073 7461 7274  n order to start
+00003c10: 2064 6576 656c 6f70 696e 6720 6f6e 2074   developing on t
+00003c20: 6869 7320 6164 6170 7465 7220 636c 6f6e  his adapter clon
+00003c30: 6520 7468 6520 7265 706f 2061 6e64 2072  e the repo and r
+00003c40: 756e 2074 6869 7320 6d61 6b65 2063 6f6d  un this make com
+00003c50: 6d61 6e64 2028 7365 6520 5b4d 616b 6566  mand (see [Makef
+00003c60: 696c 655d 284d 616b 6566 696c 6529 2920  ile](Makefile)) 
+00003c70: 3a0a 0a60 6060 6261 7368 0a6d 616b 6520  :..```bash.make 
+00003c80: 7365 7475 700a 6060 600a 0a49 7420 7769  setup.```..It wi
+00003c90: 6c6c 203a 0a31 2e20 496e 7374 616c 6c20  ll :.1. Install 
+00003ca0: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
+00003cb0: 2e0a 322e 2049 6e73 7461 6c6c 2070 7265  ..2. Install pre
+00003cc0: 2d63 6f6d 6d69 7420 686f 6f6b 732e 0a33  -commit hooks..3
+00003cd0: 2e20 4765 6e65 7261 7465 2079 6f75 7220  . Generate your 
+00003ce0: 602e 656e 7660 2066 696c 650a 0a4e 6578  `.env` file..Nex
+00003cf0: 742c 2061 646a 7573 7420 602e 656e 7660  t, adjust `.env`
+00003d00: 2066 696c 6520 6279 2063 6f6e 6669 6775   file by configu
+00003d10: 7269 6e67 2074 6865 2065 6e76 6972 6f6e  ring the environ
+00003d20: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
+00003d30: 6f20 6d61 7463 6820 796f 7572 2041 7468  o match your Ath
+00003d40: 656e 6120 6465 7665 6c6f 706d 656e 7420  ena development 
+00003d50: 656e 7669 726f 6e6d 656e 742e 0a0a 2323  environment...##
+00003d60: 2320 5275 6e6e 696e 6720 7465 7374 730a  # Running tests.
+00003d70: 0a57 6520 6861 7665 2032 2064 6966 6665  .We have 2 diffe
+00003d80: 7265 6e74 2074 7970 6573 206f 6620 7465  rent types of te
+00003d90: 7374 696e 673a 0a2a 202a 2a75 6e69 7420  sting:.* **unit 
+00003da0: 7465 7374 696e 672a 2a3a 2079 6f75 2063  testing**: you c
+00003db0: 616e 2072 756e 2074 6869 7320 7479 7065  an run this type
+00003dc0: 206f 6620 7465 7374 7320 7275 6e6e 696e   of tests runnin
+00003dd0: 6720 606d 616b 6520 756e 6974 5f74 6573  g `make unit_tes
+00003de0: 7460 0a2a 202a 2a66 756e 6374 696f 6e61  t`.* **functiona
+00003df0: 6c20 7465 7374 696e 672a 2a3a 2079 6f75  l testing**: you
+00003e00: 206d 7573 7420 6861 7665 2061 6e20 4157   must have an AW
+00003e10: 5320 6163 636f 756e 7420 7769 7468 2041  S account with A
+00003e20: 7468 656e 6120 7365 7475 7020 696e 206f  thena setup in o
+00003e30: 7264 6572 2074 6f20 6c61 756e 6368 2074  rder to launch t
+00003e40: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
+00003e50: 7320 616e 6420 6861 7665 2061 2060 2e65  s and have a `.e
+00003e60: 6e76 6020 6669 6c65 2069 6e20 706c 6163  nv` file in plac
+00003e70: 6520 7769 7468 2074 6865 2072 6967 6874  e with the right
+00003e80: 2076 616c 7565 732e 0a20 2059 6f75 2063   values..  You c
+00003e90: 616e 2072 756e 2074 6869 7320 7479 7065  an run this type
+00003ea0: 206f 6620 7465 7374 7320 7275 6e6e 696e   of tests runnin
+00003eb0: 6720 606d 616b 6520 6675 6e63 7469 6f6e  g `make function
+00003ec0: 616c 5f74 6573 7460 0a0a 416c 6c20 7479  al_test`..All ty
+00003ed0: 7065 206f 6620 7465 7374 7320 6361 6e20  pe of tests can 
+00003ee0: 6265 2072 756e 2075 7369 6e67 2060 6d61  be run using `ma
+00003ef0: 6b65 603a 0a60 6060 6261 7368 0a6d 616b  ke`:.```bash.mak
+00003f00: 6520 7465 7374 0a60 6060 0a0a 2323 2320  e test.```..### 
+00003f10: 5075 6c6c 2052 6571 7565 7374 0a0a 2a20  Pull Request..* 
+00003f20: 4372 6561 7465 2061 2063 6f6d 6d69 7420  Create a commit 
+00003f30: 7769 7468 2079 6f75 7220 6368 616e 6765  with your change
+00003f40: 7320 616e 6420 7075 7368 2074 6865 6d20  s and push them 
+00003f50: 746f 2061 0a20 205b 666f 726b 5d28 6874  to a.  [fork](ht
+00003f60: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
+00003f70: 622e 636f 6d2f 656e 2f67 6574 2d73 7461  b.com/en/get-sta
+00003f80: 7274 6564 2f71 7569 636b 7374 6172 742f  rted/quickstart/
+00003f90: 666f 726b 2d61 2d72 6570 6f29 2e0a 2a20  fork-a-repo)..* 
+00003fa0: 4372 6561 7465 2061 205b 7075 6c6c 2072  Create a [pull r
+00003fb0: 6571 7565 7374 206f 6e0a 2020 4769 7468  equest on.  Gith
+00003fc0: 7562 5d28 6874 7470 733a 2f2f 646f 6373  ub](https://docs
+00003fd0: 2e67 6974 6875 622e 636f 6d2f 656e 2f67  .github.com/en/g
+00003fe0: 6974 6875 622f 636f 6c6c 6162 6f72 6174  ithub/collaborat
+00003ff0: 696e 672d 7769 7468 2d70 756c 6c2d 7265  ing-with-pull-re
+00004000: 7175 6573 7473 2f70 726f 706f 7369 6e67  quests/proposing
+00004010: 2d63 6861 6e67 6573 2d74 6f2d 796f 7572  -changes-to-your
+00004020: 2d77 6f72 6b2d 7769 7468 2d70 756c 6c2d  -work-with-pull-
+00004030: 7265 7175 6573 7473 2f63 7265 6174 696e  requests/creatin
+00004040: 672d 612d 7075 6c6c 2d72 6571 7565 7374  g-a-pull-request
+00004050: 2d66 726f 6d2d 612d 666f 726b 292e 0a2a  -from-a-fork)..*
+00004060: 2050 756c 6c20 7265 7175 6573 7420 7469   Pull request ti
+00004070: 746c 6520 616e 6420 6d65 7373 6167 6520  tle and message 
+00004080: 2861 6e64 2050 5220 7469 746c 6520 616e  (and PR title an
+00004090: 6420 6465 7363 7269 7074 696f 6e29 206d  d description) m
+000040a0: 7573 7420 6164 6865 7265 2074 6f0a 2020  ust adhere to.  
+000040b0: 5b63 6f6e 7665 6e74 696f 6e61 6c63 6f6d  [conventionalcom
+000040c0: 6d69 7473 5d28 6874 7470 733a 2f2f 7777  mits](https://ww
+000040d0: 772e 636f 6e76 656e 7469 6f6e 616c 636f  w.conventionalco
+000040e0: 6d6d 6974 732e 6f72 6729 2e0a 2a20 5075  mmits.org)..* Pu
+000040f0: 6c6c 2072 6571 7565 7374 2062 6f64 7920  ll request body 
+00004100: 7368 6f75 6c64 2064 6573 6372 6962 6520  should describe 
+00004110: 5f6d 6f74 6976 6174 696f 6e5f 2e0a 0a0a  _motivation_....
+00004120: 2323 2052 6573 6f75 7263 6573 0a2a 205b  ## Resources.* [
+00004130: 4174 6865 6e61 2043 5245 4154 4520 5441  Athena CREATE TA
+00004140: 424c 4520 4153 5d28 6874 7470 733a 2f2f  BLE AS](https://
+00004150: 646f 6373 2e61 7773 2e61 6d61 7a6f 6e2e  docs.aws.amazon.
+00004160: 636f 6d2f 6174 6865 6e61 2f6c 6174 6573  com/athena/lates
+00004170: 742f 7567 2f63 7265 6174 652d 7461 626c  t/ug/create-tabl
+00004180: 652d 6173 2e68 746d 6c29 0a2a 205b 6462  e-as.html).* [db
+00004190: 742d 6c61 6273 2f64 6274 2d63 6f72 655d  t-labs/dbt-core]
+000041a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000041b0: 636f 6d2f 6462 742d 6c61 6273 2f64 6274  com/dbt-labs/dbt
+000041c0: 2d63 6f72 6529 0a2a 205b 6c61 7567 6869  -core).* [laughi
+000041d0: 6e67 6d61 6e37 3734 332f 5079 4174 6865  ngman7743/PyAthe
+000041e0: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
+000041f0: 7562 2e63 6f6d 2f6c 6175 6768 696e 676d  ub.com/laughingm
+00004200: 616e 3737 3433 2f50 7941 7468 656e 6129  an7743/PyAthena)
+00004210: 0a0a 0a23 2320 436f 6e74 7269 6275 746f  ...## Contributo
+00004220: 7273 20e2 9ca8 0a0a 5468 616e 6b73 2067  rs .....Thanks g
+00004230: 6f65 7320 746f 2074 6865 7365 2077 6f6e  oes to these won
+00004240: 6465 7266 756c 2070 656f 706c 6520 285b  derful people ([
+00004250: 656d 6f6a 6920 6b65 795d 2868 7474 7073  emoji key](https
+00004260: 3a2f 2f61 6c6c 636f 6e74 7269 6275 746f  ://allcontributo
+00004270: 7273 2e6f 7267 2f64 6f63 732f 656e 2f65  rs.org/docs/en/e
+00004280: 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c 212d  moji-key)):..<!-
+00004290: 2d20 414c 4c2d 434f 4e54 5249 4255 544f  - ALL-CONTRIBUTO
+000042a0: 5253 2d4c 4953 543a 5354 4152 5420 2d20  RS-LIST:START - 
+000042b0: 446f 206e 6f74 2072 656d 6f76 6520 6f72  Do not remove or
+000042c0: 206d 6f64 6966 7920 7468 6973 2073 6563   modify this sec
+000042d0: 7469 6f6e 202d 2d3e 0a3c 212d 2d20 7072  tion -->.<!-- pr
+000042e0: 6574 7469 6572 2d69 676e 6f72 652d 7374  ettier-ignore-st
+000042f0: 6172 7420 2d2d 3e0a 3c21 2d2d 206d 6172  art -->.<!-- mar
+00004300: 6b64 6f77 6e6c 696e 742d 6469 7361 626c  kdownlint-disabl
+00004310: 6520 2d2d 3e0a 3c74 6162 6c65 3e0a 2020  e -->.<table>.  
+00004320: 3c74 626f 6479 3e0a 2020 2020 3c74 723e  <tbody>.    <tr>
+00004330: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00004340: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00004350: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00004360: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00004370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004380: 6d2f 6e69 636f 7238 3822 3e3c 696d 6720  m/nicor88"><img 
+00004390: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
+000043a0: 7461 7273 2e67 6974 6875 6275 7365 7263  tars.githubuserc
+000043b0: 6f6e 7465 6e74 2e63 6f6d 2f75 2f36 3237  ontent.com/u/627
+000043c0: 3835 3437 3f76 3d34 3f73 3d31 3030 2220  8547?v=4?s=100" 
+000043d0: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
+000043e0: 6c74 3d22 6e69 636f 7238 3822 2f3e 3c62  lt="nicor88"/><b
+000043f0: 7220 2f3e 3c73 7562 3e3c 623e 6e69 636f  r /><sub><b>nico
+00004400: 7238 383c 2f62 3e3c 2f73 7562 3e3c 2f61  r88</b></sub></a
+00004410: 3e3c 6272 202f 3e3c 6120 6872 6566 3d22  ><br /><a href="
+00004420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004430: 6f6d 2f64 6274 2d61 7468 656e 612f 6462  om/dbt-athena/db
+00004440: 742d 6174 6865 6e61 2f63 6f6d 6d69 7473  t-athena/commits
+00004450: 3f61 7574 686f 723d 6e69 636f 7238 3822  ?author=nicor88"
+00004460: 2074 6974 6c65 3d22 436f 6465 223e f09f   title="Code">..
+00004470: 92bb 3c2f 613e 203c 6120 6872 6566 3d22  ..</a> <a href="
+00004480: 236d 6169 6e74 656e 616e 6365 2d6e 6963  #maintenance-nic
+00004490: 6f72 3838 2220 7469 746c 653d 224d 6169  or88" title="Mai
+000044a0: 6e74 656e 616e 6365 223e f09f 9aa7 3c2f  ntenance">....</
+000044b0: 613e 3c2f 7464 3e0a 2020 2020 2020 3c74  a></td>.      <t
+000044c0: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+000044d0: 2076 616c 6967 6e3d 2274 6f70 2220 7769   valign="top" wi
+000044e0: 6474 683d 2231 342e 3238 2522 3e3c 6120  dth="14.28%"><a 
+000044f0: 6872 6566 3d22 6874 7470 733a 2f2f 6a65  href="https://je
+00004500: 7373 6564 6f62 6265 6c61 652e 7265 223e  ssedobbelae.re">
+00004510: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00004520: 2f2f 6176 6174 6172 732e 6769 7468 7562  //avatars.github
+00004530: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00004540: 752f 3133 3532 3937 393f 763d 343f 733d  u/1352979?v=4?s=
+00004550: 3130 3022 2077 6964 7468 3d22 3130 3070  100" width="100p
+00004560: 783b 2220 616c 743d 224a 6573 7365 2044  x;" alt="Jesse D
+00004570: 6f62 6265 6c61 6572 6522 2f3e 3c62 7220  obbelaere"/><br 
+00004580: 2f3e 3c73 7562 3e3c 623e 4a65 7373 6520  /><sub><b>Jesse 
+00004590: 446f 6262 656c 6165 7265 3c2f 623e 3c2f  Dobbelaere</b></
+000045a0: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+000045b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000045c0: 6974 6875 622e 636f 6d2f 6462 742d 6174  ithub.com/dbt-at
+000045d0: 6865 6e61 2f64 6274 2d61 7468 656e 612f  hena/dbt-athena/
+000045e0: 6973 7375 6573 3f71 3d61 7574 686f 7225  issues?q=author%
+000045f0: 3341 6a65 7373 6564 6f62 6265 6c61 6572  3Ajessedobbelaer
+00004600: 6522 2074 6974 6c65 3d22 4275 6720 7265  e" title="Bug re
+00004610: 706f 7274 7322 3ef0 9f90 9b3c 2f61 3e20  ports">....</a> 
+00004620: 3c61 2068 7265 663d 2223 6d61 696e 7465  <a href="#mainte
+00004630: 6e61 6e63 652d 6a65 7373 6564 6f62 6265  nance-jessedobbe
+00004640: 6c61 6572 6522 2074 6974 6c65 3d22 4d61  laere" title="Ma
+00004650: 696e 7465 6e61 6e63 6522 3ef0 9f9a a73c  intenance">....<
+00004660: 2f61 3e3c 2f74 643e 0a20 2020 2020 203c  /a></td>.      <
+00004670: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00004680: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+00004690: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+000046a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000046b0: 6974 6875 622e 636f 6d2f 6c65 6d69 6666  ithub.com/lemiff
+000046c0: 6522 3e3c 696d 6720 7372 633d 2268 7474  e"><img src="htt
+000046d0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+000046e0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000046f0: 6f6d 2f75 2f37 3438 3737 3732 3f76 3d34  om/u/7487772?v=4
+00004700: 3f73 3d31 3030 2220 7769 6474 683d 2231  ?s=100" width="1
+00004710: 3030 7078 3b22 2061 6c74 3d22 4c65 6d69  00px;" alt="Lemi
+00004720: 6666 6522 2f3e 3c62 7220 2f3e 3c73 7562  ffe"/><br /><sub
+00004730: 3e3c 623e 4c65 6d69 6666 653c 2f62 3e3c  ><b>Lemiffe</b><
+00004740: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
+00004750: 6120 6872 6566 3d22 2364 6573 6967 6e2d  a href="#design-
+00004760: 6c65 6d69 6666 6522 2074 6974 6c65 3d22  lemiffe" title="
+00004770: 4465 7369 676e 223e f09f 8ea8 3c2f 613e  Design">....</a>
+00004780: 3c2f 7464 3e0a 2020 2020 2020 3c74 6420  </td>.      <td 
+00004790: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
+000047a0: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
+000047b0: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
+000047c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000047d0: 7562 2e63 6f6d 2f4a 726d 7979 223e 3c69  ub.com/Jrmyy"><i
+000047e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000047f0: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
+00004800: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
+00004810: 3932 3531 3335 333f 763d 343f 733d 3130  9251353?v=4?s=10
+00004820: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
+00004830: 2220 616c 743d 224a c3a9 72c3 a96d 7920  " alt="J..r..my 
+00004840: 4775 6973 656c 696e 222f 3e3c 6272 202f  Guiselin"/><br /
+00004850: 3e3c 7375 623e 3c62 3e4a c3a9 72c3 a96d  ><sub><b>J..r..m
+00004860: 7920 4775 6973 656c 696e 3c2f 623e 3c2f  y Guiselin</b></
+00004870: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00004880: 2068 7265 663d 2223 6d61 696e 7465 6e61   href="#maintena
+00004890: 6e63 652d 4a72 6d79 7922 2074 6974 6c65  nce-Jrmyy" title
+000048a0: 3d22 4d61 696e 7465 6e61 6e63 6522 3ef0  ="Maintenance">.
+000048b0: 9f9a a73c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
+000048c0: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+000048d0: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
+000048e0: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
+000048f0: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004900: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00004910: 6d6d 6522 3e3c 696d 6720 7372 633d 2268  mme"><img src="h
+00004920: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
+00004930: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00004940: 2e63 6f6d 2f75 2f39 3332 3839 353f 763d  .com/u/932895?v=
+00004950: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00004960: 3130 3070 783b 2220 616c 743d 2254 6f6d  100px;" alt="Tom
+00004970: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
+00004980: 3e54 6f6d 3c2f 623e 3c2f 7375 623e 3c2f  >Tom</b></sub></
+00004990: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
+000049a0: 2223 6d61 696e 7465 6e61 6e63 652d 546f  "#maintenance-To
+000049b0: 6d6d 6522 2074 6974 6c65 3d22 4d61 696e  mme" title="Main
+000049c0: 7465 6e61 6e63 6522 3ef0 9f9a a73c 2f61  tenance">....</a
+000049d0: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+000049e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6462  ://github.com/db
+000049f0: 742d 6174 6865 6e61 2f64 6274 2d61 7468  t-athena/dbt-ath
+00004a00: 656e 612f 636f 6d6d 6974 733f 6175 7468  ena/commits?auth
+00004a10: 6f72 3d54 6f6d 6d65 2220 7469 746c 653d  or=Tomme" title=
+00004a20: 2243 6f64 6522 3ef0 9f92 bb3c 2f61 3e3c  "Code">....</a><
+00004a30: 2f74 643e 0a20 2020 2020 203c 7464 2061  /td>.      <td a
+00004a40: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
+00004a50: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
+00004a60: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
+00004a70: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00004a80: 622e 636f 6d2f 6d61 7474 6961 6d61 7472  b.com/mattiamatr
+00004a90: 6978 223e 3c69 6d67 2073 7263 3d22 6874  ix"><img src="ht
+00004aa0: 7470 733a 2f2f 6176 6174 6172 732e 6769  tps://avatars.gi
+00004ab0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00004ac0: 636f 6d2f 752f 3530 3133 3635 343f 763d  com/u/5013654?v=
+00004ad0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00004ae0: 3130 3070 783b 2220 616c 743d 224d 6174  100px;" alt="Mat
+00004af0: 7469 6122 2f3e 3c62 7220 2f3e 3c73 7562  tia"/><br /><sub
+00004b00: 3e3c 623e 4d61 7474 6961 3c2f 623e 3c2f  ><b>Mattia</b></
+00004b10: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00004b20: 2068 7265 663d 2223 6d61 696e 7465 6e61   href="#maintena
+00004b30: 6e63 652d 6d61 7474 6961 6d61 7472 6978  nce-mattiamatrix
+00004b40: 2220 7469 746c 653d 224d 6169 6e74 656e  " title="Mainten
+00004b50: 616e 6365 223e f09f 9aa7 3c2f 613e 3c2f  ance">....</a></
+00004b60: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00004b70: 3c2f 7462 6f64 793e 0a3c 2f74 6162 6c65  </tbody>.</table
+00004b80: 3e0a 0a3c 212d 2d20 6d61 726b 646f 776e  >..<!-- markdown
+00004b90: 6c69 6e74 2d72 6573 746f 7265 202d 2d3e  lint-restore -->
+00004ba0: 0a3c 212d 2d20 7072 6574 7469 6572 2d69  .<!-- prettier-i
+00004bb0: 676e 6f72 652d 656e 6420 2d2d 3e0a 0a3c  gnore-end -->..<
+00004bc0: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00004bd0: 544f 5253 2d4c 4953 543a 454e 4420 2d2d  TORS-LIST:END --
+00004be0: 3e0a 0a54 6869 7320 7072 6f6a 6563 7420  >..This project 
+00004bf0: 666f 6c6c 6f77 7320 7468 6520 5b61 6c6c  follows the [all
+00004c00: 2d63 6f6e 7472 6962 7574 6f72 735d 2868  -contributors](h
+00004c10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004c20: 6d2f 616c 6c2d 636f 6e74 7269 6275 746f  m/all-contributo
+00004c30: 7273 2f61 6c6c 2d63 6f6e 7472 6962 7574  rs/all-contribut
+00004c40: 6f72 7329 2073 7065 6369 6669 6361 7469  ors) specificati
+00004c50: 6f6e 2e20 436f 6e74 7269 6275 7469 6f6e  on. Contribution
+00004c60: 7320 6f66 2061 6e79 206b 696e 6420 7765  s of any kind we
+00004c70: 6c63 6f6d 6521 0a                        lcome!.
```

### Comparing `dbt-athena-community-1.4.2/dbt/adapters/athena/__init__.py` & `dbt-athena-community-1.4.3/dbt/adapters/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/adapters/athena/connections.py` & `dbt-athena-community-1.4.3/dbt/adapters/athena/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/adapters/athena/impl.py` & `dbt-athena-community-1.4.3/dbt/adapters/athena/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import agate
 from botocore.exceptions import ClientError
 
 from dbt.adapters.athena import AthenaConnectionManager
+from dbt.adapters.athena.column import AthenaColumn
 from dbt.adapters.athena.config import get_boto3_config
-from dbt.adapters.athena.relation import AthenaRelation, AthenaSchemaSearchMap
+from dbt.adapters.athena.relation import (
+    AthenaRelation,
+    AthenaSchemaSearchMap,
+    TableType,
+)
 from dbt.adapters.athena.utils import clean_sql_comment
-from dbt.adapters.base import Column, available
+from dbt.adapters.base import available
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import CompiledNode
 from dbt.events import AdapterLogger
 from dbt.exceptions import DbtRuntimeError
 
@@ -29,21 +34,21 @@
 
 
 class AthenaAdapter(SQLAdapter):
     ConnectionManager = AthenaConnectionManager
     Relation = AthenaRelation
 
     relation_type_map = {
-        "EXTERNAL_TABLE": "table",
-        "MANAGED_TABLE": "table",
-        "VIRTUAL_VIEW": "view",
-        "table": "table",
-        "view": "view",
-        "cte": "cte",
-        "materializedview": "materializedview",
+        "EXTERNAL_TABLE": TableType.TABLE,
+        "MANAGED_TABLE": TableType.TABLE,
+        "VIRTUAL_VIEW": TableType.VIEW,
+        "table": TableType.TABLE,
+        "view": TableType.VIEW,
+        "cte": TableType.CTE,
+        "materializedview": TableType.MATERIALIZED_VIEW,
     }
 
     @classmethod
     def date_function(cls) -> str:
         return "now()"
 
     @classmethod
@@ -135,29 +140,38 @@
                                 "TableWithColumns": {"DatabaseName": database, "Name": table, "ColumnNames": columns}
                             },
                             LFTags=[{"TagKey": tag_key, "TagValues": [tag_value]}],
                         )
                         logger.debug(self.parse_lf_response(response, database, table, columns, {tag_key: tag_value}))
 
     @available
-    def get_work_group_output_location(self) -> Optional[str]:
+    def is_work_group_output_location_enforced(self) -> bool:
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
 
         with boto3_client_lock:
             athena_client = client.session.client("athena", region_name=client.region_name, config=get_boto3_config())
 
-        work_group = athena_client.get_work_group(WorkGroup=creds.work_group)
-        return (
-            work_group.get("WorkGroup", {})
-            .get("Configuration", {})
-            .get("ResultConfiguration", {})
-            .get("OutputLocation")
-        )
+        if creds.work_group:
+            work_group = athena_client.get_work_group(WorkGroup=creds.work_group)
+            output_location = (
+                work_group.get("WorkGroup", {})
+                .get("Configuration", {})
+                .get("ResultConfiguration", {})
+                .get("OutputLocation", None)
+            )
+
+            output_location_enforced = (
+                work_group.get("WorkGroup", {}).get("Configuration", {}).get("EnforceWorkGroupConfiguration", False)
+            )
+
+            return output_location is not None and output_location_enforced
+        else:
+            return False
 
     @available
     def s3_table_prefix(self, s3_data_dir: Optional[str]) -> str:
         """
         Returns the root location for storing tables in S3.
         This is `s3_data_dir`, if set, and `s3_staging_dir/tables/` if not.
         We generate a value here even if `s3_data_dir` is not set,
@@ -359,15 +373,15 @@
         )
 
     def _get_one_table_for_catalog(self, table: dict, database: str) -> list:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
-            "table_type": self.relation_type_map[table["TableType"]],
+            "table_type": self.relation_type_map[table["TableType"]].value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
         }
         return [
             {
                 **table_catalog,
                 **{
                     "column_name": col["Name"],
@@ -479,34 +493,34 @@
             # don't error out when schema doesn't exist
             # this allows dbt to create and manage schemas/databases
             logger.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
 
         return relations
 
     @available
-    def get_table_type(self, db_name, table_name):
+    def get_table_type(self, db_name, table_name) -> TableType:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         try:
             response = glue_client.get_table(DatabaseName=db_name, Name=table_name)
-            _type = self.relation_type_map.get(response.get("Table", {}).get("TableType", "Table"))
+            _type = self.relation_type_map.get(response.get("Table", {}).get("TableType"))
             _specific_type = response.get("Table", {}).get("Parameters", {}).get("table_type", "")
 
             if _specific_type.lower() == "iceberg":
-                _type = "iceberg_table"
+                _type = TableType.ICEBERG
 
             if _type is None:
                 raise ValueError("Table type cannot be None")
 
-            logger.debug("table_name : " + table_name)
-            logger.debug("table type : " + _type)
+            logger.debug(f"table_name : {table_name}")
+            logger.debug(f"table type : {_type}")
 
             return _type
 
         except glue_client.exceptions.EntityNotFoundException as e:
             logger.debug(f"Error calling Glue get_table: {e}")
 
     @available
@@ -670,22 +684,33 @@
         Check if a column is explicit set as not current. If not, it is considered as current.
         """
         if col.get("Parameters", {}).get("iceberg.field.current") == "false":
             return False
         return True
 
     @available
-    def get_columns_in_relation(self, relation: AthenaRelation) -> List[Column]:
+    def get_columns_in_relation(self, relation: AthenaRelation) -> List[AthenaColumn]:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
-        table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.identifier)["Table"]
+        try:
+            table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.identifier)["Table"]
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "EntityNotFoundException":
+                logger.debug("table not exist, catching the error")
+                return []
+            else:
+                logger.error(e)
+                raise e
+        table_type = self.get_table_type(relation.schema, relation.identifier)
 
         columns = [c for c in table["StorageDescriptor"]["Columns"] if self._is_current_column(c)]
         partition_keys = table.get("PartitionKeys", [])
 
         logger.debug(f"Columns in relation {relation.identifier}: {columns + partition_keys}")
 
-        return [Column(c["Name"], c["Type"]) for c in columns + partition_keys]
+        return [
+            AthenaColumn(column=c["Name"], dtype=c["Type"], table_type=table_type) for c in columns + partition_keys
+        ]
```

### Comparing `dbt-athena-community-1.4.2/dbt/adapters/athena/query_headers.py` & `dbt-athena-community-1.4.3/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/adapters/athena/relation.py` & `dbt-athena-community-1.4.3/dbt/adapters/athena/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from dataclasses import dataclass, field
+from enum import Enum
 from typing import Dict, Optional, Set
 
 from dbt.adapters.base.relation import BaseRelation, InformationSchema, Policy
 
 
+class TableType(Enum):
+    TABLE = "table"
+    VIEW = "view"
+    CTE = "cte"
+    MATERIALIZED_VIEW = "materializedview"
+    ICEBERG = "iceberg_table"
+
+
 @dataclass
 class AthenaIncludePolicy(Policy):
-    database: bool = False
+    database: bool = True
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class AthenaRelation(BaseRelation):
     quote_character: str = '"'  # Presto quote character
```

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/adapters/relation.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 {% macro athena__drop_relation(relation) -%}
   {% set rel_type = adapter.get_table_type(relation.schema, relation.table) %}
   {%- if rel_type is not none %}
     {%- if rel_type == 'table' %}
       {%- do adapter.clean_up_table(relation.schema, relation.table) -%}
     {%- endif %}
     {% call statement('drop_relation', auto_begin=False) -%}
-      drop {{ relation.type }} if exists {{ relation.render_hive() }}
+      {%- if relation.type == 'view' -%}
+        drop {{ relation.type }} if exists {{ relation.render() }}
+      {%- else -%}
+        drop {{ relation.type }} if exists {{ relation.render_hive() }}
+      {% endif %}
     {%- endcall %}
   {%- endif %}
 {% endmacro %}
 
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
```

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   {%- set write_compression = config.get('write_compression', default=none) -%}
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', default=target.s3_data_naming) -%}
   {%- set extra_table_properties = config.get('table_properties', default=none) -%}
 
   {%- set location_property = 'external_location' -%}
   {%- set partition_property = 'partitioned_by' -%}
-  {%- set work_group_output_location = adapter.get_work_group_output_location() -%}
+  {%- set work_group_output_location_enforced = adapter.is_work_group_output_location_enforced() -%}
   {%- set location = adapter.s3_table_location(s3_data_dir, s3_data_naming, relation.schema, relation.identifier, external_location, temporary) -%}
 
   {%- if materialized == 'table_hive_ha' -%}
     {%- set location = location.replace('__ha', '') -%}
   {%- endif %}
 
   {%- if table_type == 'iceberg' -%}
@@ -44,15 +44,15 @@
 
   {% do adapter.delete_from_s3(location) %}
 
   create table {{ relation }}
   with (
     table_type='{{ table_type }}',
     is_external={%- if table_type == 'iceberg' -%}false{%- else -%}true{%- endif %},
-  {%- if work_group_output_location is none -%}
+  {%- if not work_group_output_location_enforced -%}
     {{ location_property }}='{{ location }}',
   {%- endif %}
   {%- if partitioned_by is not none %}
     {{ partition_property }}=ARRAY{{ partitioned_by | tojson | replace('\"', '\'') }},
   {%- endif %}
   {%- if bucketed_by is not none %}
     bucketed_by=ARRAY{{ bucketed_by | tojson | replace('\"', '\'') }},
```

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/datediff.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/macros/utils/ddl_data_type.sql` & `dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/ddl_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt/include/athena/profile_template.yml` & `dbt-athena-community-1.4.3/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/dbt_athena_community.egg-info/PKG-INFO` & `dbt-athena-community-1.4.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,1047 +1,1209 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6462 742d  : 2.1.Name: dbt-
-00000020: 6174 6865 6e61 2d63 6f6d 6d75 6e69 7479  athena-community
-00000030: 0a56 6572 7369 6f6e 3a20 312e 342e 320a  .Version: 1.4.2.
-00000040: 5375 6d6d 6172 793a 2054 6865 2061 7468  Summary: The ath
-00000050: 656e 6120 6164 6170 7465 7220 706c 7567  ena adapter plug
-00000060: 696e 2066 6f72 2064 6274 2028 6461 7461  in for dbt (data
-00000070: 2062 7569 6c64 2074 6f6f 6c29 0a48 6f6d   build tool).Hom
-00000080: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-00000090: 6769 7468 7562 2e63 6f6d 2f64 6274 2d61  github.com/dbt-a
-000000a0: 7468 656e 612f 6462 742d 6174 6865 6e61  thena/dbt-athena
-000000b0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000000c0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000000d0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-000000e0: 2d46 696c 653a 204c 4943 454e 5345 2e74  -File: LICENSE.t
-000000f0: 7874 0a0a 5b21 5b70 7970 695d 2868 7474  xt..[![pypi](htt
-00000100: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000110: 696f 2f70 792f 6462 742d 6174 6865 6e61  io/py/dbt-athena
-00000120: 2d63 6f6d 6d75 6e69 7479 2e73 7667 295d  -community.svg)]
-00000130: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000140: 672f 7072 6f6a 6563 742f 6462 742d 6174  g/project/dbt-at
-00000150: 6865 6e61 2d63 6f6d 6d75 6e69 7479 2f29  hena-community/)
-00000160: 0a5b 215b 496d 706f 7274 733a 2069 736f  .[![Imports: iso
-00000170: 7274 5d28 6874 7470 733a 2f2f 696d 672e  rt](https://img.
-00000180: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000190: 2f25 3230 696d 706f 7274 732d 6973 6f72  /%20imports-isor
-000001a0: 742d 2532 3331 3637 3462 313f 7374 796c  t-%231674b1?styl
-000001b0: 653d 666c 6174 266c 6162 656c 436f 6c6f  e=flat&labelColo
-000001c0: 723d 6566 3833 3336 295d 2868 7474 7073  r=ef8336)](https
-000001d0: 3a2f 2f70 7963 7161 2e67 6974 6875 622e  ://pycqa.github.
-000001e0: 696f 2f69 736f 7274 2f29 0a5b 215b 436f  io/isort/).[![Co
-000001f0: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
-00000200: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000210: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00000220: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-00000230: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
-00000240: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000250: 2f70 7366 2f62 6c61 636b 290a 5b21 5b53  /psf/black).[![S
-00000260: 7461 7473 3a20 7065 7079 5d28 6874 7470  tats: pepy](http
-00000270: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
-00000280: 6467 652f 6462 742d 6174 6865 6e61 2d63  dge/dbt-athena-c
-00000290: 6f6d 6d75 6e69 7479 2f6d 6f6e 7468 295d  ommunity/month)]
-000002a0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-000002b0: 6368 2f70 726f 6a65 6374 2f64 6274 2d61  ch/project/dbt-a
-000002c0: 7468 656e 612d 636f 6d6d 756e 6974 7929  thena-community)
-000002d0: 0a0a 2320 6462 742d 6174 6865 6e61 0a0a  ..# dbt-athena..
-000002e0: 2a20 5375 7070 6f72 7473 2064 6274 2076  * Supports dbt v
-000002f0: 6572 7369 6f6e 2060 312e 342e 2a60 0a2a  ersion `1.4.*`.*
-00000300: 2053 7570 706f 7274 7320 5b53 6565 6473   Supports [Seeds
-00000310: 5d5b 7365 6564 735d 0a2a 2043 6f72 7265  ][seeds].* Corre
-00000320: 6374 6c79 2064 6574 6563 7473 2076 6965  ctly detects vie
-00000330: 7773 2061 6e64 2074 6865 6972 2063 6f6c  ws and their col
-00000340: 756d 6e73 0a2a 2053 7570 706f 7274 7320  umns.* Supports 
-00000350: 5b74 6162 6c65 206d 6174 6572 6961 6c69  [table materiali
-00000360: 7a61 7469 6f6e 5d5b 7461 626c 655d 0a20  zation][table]. 
-00000370: 202a 205b 4963 6562 6572 6720 7461 626c   * [Iceberg tabl
-00000380: 6573 5d5b 6174 6865 6e61 2d69 6365 6265  es][athena-icebe
-00000390: 7267 5d20 6973 2073 7570 706f 7274 6564  rg] is supported
-000003a0: 202a 2a6f 6e6c 7920 7769 7468 2041 7468   **only with Ath
-000003b0: 656e 6120 456e 6769 6e65 2076 332a 2a20  ena Engine v3** 
-000003c0: 616e 6420 2a2a 6120 756e 6971 7565 2074  and **a unique t
-000003d0: 6162 6c65 206c 6f63 6174 696f 6e2a 2a0a  able location**.
-000003e0: 2020 2873 6565 2074 6162 6c65 206c 6f63    (see table loc
-000003f0: 6174 696f 6e20 7365 6374 696f 6e20 6265  ation section be
-00000400: 6c6f 7729 0a20 202a 2048 6976 6520 7461  low).  * Hive ta
-00000410: 626c 6573 2069 7320 7375 7070 6f72 7465  bles is supporte
-00000420: 6420 6279 2062 6f74 6820 4174 6865 6e61  d by both Athena
-00000430: 2065 6e67 696e 6573 2e0a 2a20 5375 7070   engines..* Supp
-00000440: 6f72 7473 205b 696e 6372 656d 656e 7461  orts [incrementa
-00000450: 6c20 6d6f 6465 6c73 5d5b 696e 6372 656d  l models][increm
-00000460: 656e 7461 6c5d 0a20 202a 204f 6e20 6963  ental].  * On ic
-00000470: 6562 6572 6720 7461 626c 6573 203a 0a20  eberg tables :. 
-00000480: 2020 202a 2053 7570 706f 7274 2074 6865     * Support the
-00000490: 2075 7365 206f 6620 6075 6e69 7175 655f   use of `unique_
-000004a0: 6b65 7960 206f 6e6c 7920 7769 7468 2074  key` only with t
-000004b0: 6865 2060 6d65 7267 6560 2073 7472 6174  he `merge` strat
-000004c0: 6567 790a 2020 2020 2a20 5375 7070 6f72  egy.    * Suppor
-000004d0: 7420 7468 6520 6061 7070 656e 6460 2073  t the `append` s
-000004e0: 7472 6174 6567 790a 2020 2a20 4f6e 2048  trategy.  * On H
-000004f0: 6976 6520 7461 626c 6573 203a 0a20 2020  ive tables :.   
-00000500: 202a 2053 7570 706f 7274 2074 776f 2069   * Support two i
-00000510: 6e63 7265 6d65 6e74 616c 2075 7064 6174  ncremental updat
-00000520: 6520 7374 7261 7465 6769 6573 3a20 6069  e strategies: `i
-00000530: 6e73 6572 745f 6f76 6572 7772 6974 6560  nsert_overwrite`
-00000540: 2061 6e64 2060 6170 7065 6e64 600a 2020   and `append`.  
-00000550: 2020 2a20 446f 6573 202a 2a6e 6f74 2a2a    * Does **not**
-00000560: 2073 7570 706f 7274 2074 6865 2075 7365   support the use
-00000570: 206f 6620 6075 6e69 7175 655f 6b65 7960   of `unique_key`
-00000580: 0a2a 2053 7570 706f 7274 7320 5b73 6e61  .* Supports [sna
-00000590: 7073 686f 7473 5d5b 736e 6170 7368 6f74  pshots][snapshot
-000005a0: 735d 0a2a 2044 6f65 7320 6e6f 7420 7375  s].* Does not su
-000005b0: 7070 6f72 7420 5b50 7974 686f 6e20 6d6f  pport [Python mo
-000005c0: 6465 6c73 5d5b 7079 7468 6f6e 2d6d 6f64  dels][python-mod
-000005d0: 656c 735d 0a2a 2044 6f65 7320 6e6f 7420  els].* Does not 
-000005e0: 7375 7070 6f72 7420 5b70 6572 7369 7374  support [persist
-000005f0: 2064 6f63 735d 5b70 6572 7369 7374 2d64   docs][persist-d
-00000600: 6f63 735d 2066 6f72 2076 6965 7773 0a0a  ocs] for views..
-00000610: 5b73 6565 6473 5d3a 2068 7474 7073 3a2f  [seeds]: https:/
-00000620: 2f64 6f63 732e 6765 7464 6274 2e63 6f6d  /docs.getdbt.com
-00000630: 2f64 6f63 732f 6275 696c 6469 6e67 2d61  /docs/building-a
-00000640: 2d64 6274 2d70 726f 6a65 6374 2f73 6565  -dbt-project/see
-00000650: 6473 0a5b 696e 6372 656d 656e 7461 6c5d  ds.[incremental]
-00000660: 3a20 6874 7470 733a 2f2f 646f 6373 2e67  : https://docs.g
-00000670: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
-00000680: 7569 6c64 2f69 6e63 7265 6d65 6e74 616c  uild/incremental
-00000690: 2d6d 6f64 656c 730a 5b74 6162 6c65 5d3a  -models.[table]:
-000006a0: 2068 7474 7073 3a2f 2f64 6f63 732e 6765   https://docs.ge
-000006b0: 7464 6274 2e63 6f6d 2f64 6f63 732f 6275  tdbt.com/docs/bu
-000006c0: 696c 642f 6d61 7465 7269 616c 697a 6174  ild/materializat
-000006d0: 696f 6e73 2374 6162 6c65 0a5b 7079 7468  ions#table.[pyth
-000006e0: 6f6e 2d6d 6f64 656c 735d 3a20 6874 7470  on-models]: http
-000006f0: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
-00000700: 636f 6d2f 646f 6373 2f62 7569 6c64 2f70  com/docs/build/p
-00000710: 7974 686f 6e2d 6d6f 6465 6c73 2363 6f6e  ython-models#con
-00000720: 6669 6775 7269 6e67 2d70 7974 686f 6e2d  figuring-python-
-00000730: 6d6f 6465 6c73 0a5b 6174 6865 6e61 2d69  models.[athena-i
-00000740: 6365 6265 7267 5d3a 2068 7474 7073 3a2f  ceberg]: https:/
-00000750: 2f64 6f63 732e 6177 732e 616d 617a 6f6e  /docs.aws.amazon
-00000760: 2e63 6f6d 2f61 7468 656e 612f 6c61 7465  .com/athena/late
-00000770: 7374 2f75 672f 7175 6572 7969 6e67 2d69  st/ug/querying-i
-00000780: 6365 6265 7267 2e68 746d 6c0a 5b73 6e61  ceberg.html.[sna
-00000790: 7073 686f 7473 5d3a 2068 7474 7073 3a2f  pshots]: https:/
-000007a0: 2f64 6f63 732e 6765 7464 6274 2e63 6f6d  /docs.getdbt.com
-000007b0: 2f64 6f63 732f 6275 696c 642f 736e 6170  /docs/build/snap
-000007c0: 7368 6f74 730a 5b70 6572 7369 7374 2d64  shots.[persist-d
-000007d0: 6f63 735d 3a20 6874 7470 733a 2f2f 646f  ocs]: https://do
-000007e0: 6373 2e67 6574 6462 742e 636f 6d2f 7265  cs.getdbt.com/re
-000007f0: 6665 7265 6e63 652f 7265 736f 7572 6365  ference/resource
-00000800: 2d63 6f6e 6669 6773 2f70 6572 7369 7374  -configs/persist
-00000810: 5f64 6f63 730a 0a23 2323 2049 6e73 7461  _docs..### Insta
-00000820: 6c6c 6174 696f 6e0a 0a2a 2060 7069 7020  llation..* `pip 
-00000830: 696e 7374 616c 6c20 6462 742d 6174 6865  install dbt-athe
-00000840: 6e61 2d63 6f6d 6d75 6e69 7479 600a 2a20  na-community`.* 
-00000850: 4f72 2060 7069 7020 696e 7374 616c 6c20  Or `pip install 
-00000860: 6769 742b 6874 7470 733a 2f2f 6769 7468  git+https://gith
-00000870: 7562 2e63 6f6d 2f64 6274 2d61 7468 656e  ub.com/dbt-athen
-00000880: 612f 6462 742d 6174 6865 6e61 2e67 6974  a/dbt-athena.git
-00000890: 600a 0a23 2323 2050 7265 7265 7175 6973  `..### Prerequis
-000008a0: 6974 6573 0a0a 546f 2073 7461 7274 2c20  ites..To start, 
-000008b0: 796f 7520 7769 6c6c 206e 6565 6420 616e  you will need an
-000008c0: 2053 3320 6275 636b 6574 2c20 666f 7220   S3 bucket, for 
-000008d0: 696e 7374 616e 6365 2060 6d79 2d62 7563  instance `my-buc
-000008e0: 6b65 7460 2061 6e64 2061 6e20 4174 6865  ket` and an Athe
-000008f0: 6e61 2064 6174 6162 6173 653a 0a0a 6060  na database:..``
-00000900: 6073 716c 0a43 5245 4154 4520 4441 5441  `sql.CREATE DATA
-00000910: 4241 5345 2049 4620 4e4f 5420 4558 4953  BASE IF NOT EXIS
-00000920: 5453 2061 6e61 6c79 7469 6373 5f64 6576  TS analytics_dev
-00000930: 0a43 4f4d 4d45 4e54 2027 416e 616c 7974  .COMMENT 'Analyt
-00000940: 6963 7320 6d6f 6465 6c73 2067 656e 6572  ics models gener
-00000950: 6174 6564 2062 7920 6462 7420 2864 6576  ated by dbt (dev
-00000960: 656c 6f70 6d65 6e74 2927 0a4c 4f43 4154  elopment)'.LOCAT
-00000970: 494f 4e20 2773 333a 2f2f 6d79 2d62 7563  ION 's3://my-buc
-00000980: 6b65 742f 270a 5749 5448 2044 4250 524f  ket/'.WITH DBPRO
-00000990: 5045 5254 4945 5320 2827 6372 6561 746f  PERTIES ('creato
-000009a0: 7227 3d27 466f 6f20 4261 7227 2c20 2765  r'='Foo Bar', 'e
-000009b0: 6d61 696c 273d 2766 6f6f 4062 6172 2e63  mail'='foo@bar.c
-000009c0: 6f6d 2729 3b0a 6060 600a 0a4e 6f74 6573  om');.```..Notes
-000009d0: 3a0a 2d20 5461 6b65 206e 6f74 6520 6f66  :.- Take note of
-000009e0: 2079 6f75 7220 4157 5320 7265 6769 6f6e   your AWS region
-000009f0: 2063 6f64 6520 2865 2e67 2e20 6075 732d   code (e.g. `us-
-00000a00: 7765 7374 2d32 6020 6f72 2060 6575 2d77  west-2` or `eu-w
-00000a10: 6573 742d 3260 2c20 6574 632e 292e 0a2d  est-2`, etc.)..-
-00000a20: 2059 6f75 2063 616e 2061 6c73 6f20 7573   You can also us
-00000a30: 6520 5b41 5753 2047 6c75 655d 2868 7474  e [AWS Glue](htt
-00000a40: 7073 3a2f 2f64 6f63 732e 6177 732e 616d  ps://docs.aws.am
-00000a50: 617a 6f6e 2e63 6f6d 2f61 7468 656e 612f  azon.com/athena/
-00000a60: 6c61 7465 7374 2f75 672f 676c 7565 2d61  latest/ug/glue-a
-00000a70: 7468 656e 612e 6874 6d6c 2920 746f 2063  thena.html) to c
-00000a80: 7265 6174 6520 616e 6420 6d61 6e61 6765  reate and manage
-00000a90: 2041 7468 656e 6120 6461 7461 6261 7365   Athena database
-00000aa0: 732e 0a0a 2323 2320 4372 6564 656e 7469  s...### Credenti
-00000ab0: 616c 730a 0a54 6869 7320 706c 7567 696e  als..This plugin
-00000ac0: 2064 6f65 7320 6e6f 7420 6163 6365 7074   does not accept
-00000ad0: 2061 6e79 2063 7265 6465 6e74 6961 6c73   any credentials
-00000ae0: 2064 6972 6563 746c 792e 2049 6e73 7465   directly. Inste
-00000af0: 6164 2c20 5b63 7265 6465 6e74 6961 6c73  ad, [credentials
-00000b00: 2061 7265 2064 6574 6572 6d69 6e65 6420   are determined 
-00000b10: 6175 746f 6d61 7469 6361 6c6c 795d 2868  automatically](h
-00000b20: 7474 7073 3a2f 2f62 6f74 6f33 2e61 6d61  ttps://boto3.ama
-00000b30: 7a6f 6e61 7773 2e63 6f6d 2f76 312f 646f  zonaws.com/v1/do
-00000b40: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
-00000b50: 6c61 7465 7374 2f67 7569 6465 2f63 7265  latest/guide/cre
-00000b60: 6465 6e74 6961 6c73 2e68 746d 6c29 2062  dentials.html) b
-00000b70: 6173 6564 206f 6e20 6061 7773 2063 6c69  ased on `aws cli
-00000b80: 602f 6062 6f74 6f33 6020 636f 6e76 656e  `/`boto3` conven
-00000b90: 7469 6f6e 7320 616e 640a 7374 6f72 6564  tions and.stored
-00000ba0: 206c 6f67 696e 2069 6e66 6f2e 2059 6f75   login info. You
-00000bb0: 2063 616e 2063 6f6e 6669 6775 7265 2074   can configure t
-00000bc0: 6865 2041 5753 2070 726f 6669 6c65 206e  he AWS profile n
-00000bd0: 616d 6520 746f 2075 7365 2076 6961 2060  ame to use via `
-00000be0: 6177 735f 7072 6f66 696c 655f 6e61 6d65  aws_profile_name
-00000bf0: 602e 2043 6865 636b 6f75 7420 4442 5420  `. Checkout DBT 
-00000c00: 7072 6f66 696c 6520 636f 6e66 6967 7572  profile configur
-00000c10: 6174 696f 6e20 6265 6c6f 7720 666f 7220  ation below for 
-00000c20: 6465 7461 696c 732e 0a0a 2323 2320 436f  details...### Co
-00000c30: 6e66 6967 7572 696e 6720 796f 7572 2070  nfiguring your p
-00000c40: 726f 6669 6c65 0a0a 4120 6462 7420 7072  rofile..A dbt pr
-00000c50: 6f66 696c 6520 6361 6e20 6265 2063 6f6e  ofile can be con
-00000c60: 6669 6775 7265 6420 746f 2072 756e 2061  figured to run a
-00000c70: 6761 696e 7374 2041 5753 2041 7468 656e  gainst AWS Athen
-00000c80: 6120 7573 696e 6720 7468 6520 666f 6c6c  a using the foll
-00000c90: 6f77 696e 6720 636f 6e66 6967 7572 6174  owing configurat
-00000ca0: 696f 6e3a 0a0a 7c20 4f70 7469 6f6e 2020  ion:..| Option  
-00000cb0: 2020 2020 2020 2020 207c 2044 6573 6372           | Descr
-00000cc0: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000020: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000030: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000040: 6f6d 2f64 6274 2d61 7468 656e 612f 6462  om/dbt-athena/db
+00000050: 742d 6174 6865 6e61 2f6d 6169 6e2f 7374  t-athena/main/st
+00000060: 6174 6963 2f69 6d61 6765 732f 6462 742d  atic/images/dbt-
+00000070: 6174 6865 6e61 2d6c 6f6e 672e 706e 6722  athena-long.png"
+00000080: 202f 3e0a 2020 2020 3c61 2068 7265 663d   />.    <a href=
+00000090: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000000a0: 672f 7072 6f6a 6563 742f 6462 742d 6174  g/project/dbt-at
+000000b0: 6865 6e61 2d63 6f6d 6d75 6e69 7479 2f22  hena-community/"
+000000c0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000000d0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+000000e0: 2f70 792f 6462 742d 6174 6865 6e61 2d63  /py/dbt-athena-c
+000000f0: 6f6d 6d75 6e69 7479 2e73 7667 2220 2f3e  ommunity.svg" />
+00000100: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000110: 3d22 6874 7470 733a 2f2f 7079 6371 612e  ="https://pycqa.
+00000120: 6769 7468 7562 2e69 6f2f 6973 6f72 742f  github.io/isort/
+00000130: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000140: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000150: 696f 2f62 6164 6765 2f25 3230 696d 706f  io/badge/%20impo
+00000160: 7274 732d 6973 6f72 742d 2532 3331 3637  rts-isort-%23167
+00000170: 3462 313f 7374 796c 653d 666c 6174 266c  4b1?style=flat&l
+00000180: 6162 656c 436f 6c6f 723d 6566 3833 3336  abelColor=ef8336
+00000190: 2220 2f3e 3c2f 613e 0a20 2020 203c 6120  " /></a>.    <a 
+000001a0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000001b0: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
+000001c0: 636b 223e 3c69 6d67 2073 7263 3d22 6874  ck"><img src="ht
+000001d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000001e0: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+000001f0: 3230 7374 796c 652d 626c 6163 6b2d 3030  20style-black-00
+00000200: 3030 3030 2e73 7667 2220 2f3e 3c2f 613e  0000.svg" /></a>
+00000210: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000220: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00000230: 7072 6f6a 6563 742f 6462 742d 6174 6865  project/dbt-athe
+00000240: 6e61 2d63 6f6d 6d75 6e69 7479 223e 3c69  na-community"><i
+00000250: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000260: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+00000270: 6462 742d 6174 6865 6e61 2d63 6f6d 6d75  dbt-athena-commu
+00000280: 6e69 7479 2f6d 6f6e 7468 2220 2f3e 3c2f  nity/month" /></
+00000290: 613e 0a3c 2f70 3e0a 0a23 2320 4665 6174  a>.</p>..## Feat
+000002a0: 7572 6573 0a0a 2a20 5375 7070 6f72 7473  ures..* Supports
+000002b0: 2064 6274 2076 6572 7369 6f6e 2060 312e   dbt version `1.
+000002c0: 342e 2a60 0a2a 2053 7570 706f 7274 7320  4.*`.* Supports 
+000002d0: 5b53 6565 6473 5d5b 7365 6564 735d 0a2a  [Seeds][seeds].*
+000002e0: 2043 6f72 7265 6374 6c79 2064 6574 6563   Correctly detec
+000002f0: 7473 2076 6965 7773 2061 6e64 2074 6865  ts views and the
+00000300: 6972 2063 6f6c 756d 6e73 0a2a 2053 7570  ir columns.* Sup
+00000310: 706f 7274 7320 5b74 6162 6c65 206d 6174  ports [table mat
+00000320: 6572 6961 6c69 7a61 7469 6f6e 5d5b 7461  erialization][ta
+00000330: 626c 655d 0a20 202a 205b 4963 6562 6572  ble].  * [Iceber
+00000340: 6720 7461 626c 6573 5d5b 6174 6865 6e61  g tables][athena
+00000350: 2d69 6365 6265 7267 5d20 6973 2073 7570  -iceberg] is sup
+00000360: 706f 7274 6564 202a 2a6f 6e6c 7920 7769  ported **only wi
+00000370: 7468 2041 7468 656e 6120 456e 6769 6e65  th Athena Engine
+00000380: 2076 332a 2a20 616e 6420 2a2a 6120 756e   v3** and **a un
+00000390: 6971 7565 2074 6162 6c65 206c 6f63 6174  ique table locat
+000003a0: 696f 6e2a 2a0a 2020 2873 6565 2074 6162  ion**.  (see tab
+000003b0: 6c65 206c 6f63 6174 696f 6e20 7365 6374  le location sect
+000003c0: 696f 6e20 6265 6c6f 7729 0a20 202a 2048  ion below).  * H
+000003d0: 6976 6520 7461 626c 6573 2069 7320 7375  ive tables is su
+000003e0: 7070 6f72 7465 6420 6279 2062 6f74 6820  pported by both 
+000003f0: 4174 6865 6e61 2065 6e67 696e 6573 2e0a  Athena engines..
+00000400: 2a20 5375 7070 6f72 7473 205b 696e 6372  * Supports [incr
+00000410: 656d 656e 7461 6c20 6d6f 6465 6c73 5d5b  emental models][
+00000420: 696e 6372 656d 656e 7461 6c5d 0a20 202a  incremental].  *
+00000430: 204f 6e20 6963 6562 6572 6720 7461 626c   On iceberg tabl
+00000440: 6573 203a 0a20 2020 202a 2053 7570 706f  es :.    * Suppo
+00000450: 7274 2074 6865 2075 7365 206f 6620 6075  rt the use of `u
+00000460: 6e69 7175 655f 6b65 7960 206f 6e6c 7920  nique_key` only 
+00000470: 7769 7468 2074 6865 2060 6d65 7267 6560  with the `merge`
+00000480: 2073 7472 6174 6567 790a 2020 2020 2a20   strategy.    * 
+00000490: 5375 7070 6f72 7420 7468 6520 6061 7070  Support the `app
+000004a0: 656e 6460 2073 7472 6174 6567 790a 2020  end` strategy.  
+000004b0: 2a20 4f6e 2048 6976 6520 7461 626c 6573  * On Hive tables
+000004c0: 203a 0a20 2020 202a 2053 7570 706f 7274   :.    * Support
+000004d0: 2074 776f 2069 6e63 7265 6d65 6e74 616c   two incremental
+000004e0: 2075 7064 6174 6520 7374 7261 7465 6769   update strategi
+000004f0: 6573 3a20 6069 6e73 6572 745f 6f76 6572  es: `insert_over
+00000500: 7772 6974 6560 2061 6e64 2060 6170 7065  write` and `appe
+00000510: 6e64 600a 2020 2020 2a20 446f 6573 202a  nd`.    * Does *
+00000520: 2a6e 6f74 2a2a 2073 7570 706f 7274 2074  *not** support t
+00000530: 6865 2075 7365 206f 6620 6075 6e69 7175  he use of `uniqu
+00000540: 655f 6b65 7960 0a2a 2053 7570 706f 7274  e_key`.* Support
+00000550: 7320 5b73 6e61 7073 686f 7473 5d5b 736e  s [snapshots][sn
+00000560: 6170 7368 6f74 735d 0a2a 2044 6f65 7320  apshots].* Does 
+00000570: 6e6f 7420 7375 7070 6f72 7420 5b50 7974  not support [Pyt
+00000580: 686f 6e20 6d6f 6465 6c73 5d5b 7079 7468  hon models][pyth
+00000590: 6f6e 2d6d 6f64 656c 735d 0a2a 2044 6f65  on-models].* Doe
+000005a0: 7320 6e6f 7420 7375 7070 6f72 7420 5b70  s not support [p
+000005b0: 6572 7369 7374 2064 6f63 735d 5b70 6572  ersist docs][per
+000005c0: 7369 7374 2d64 6f63 735d 2066 6f72 2076  sist-docs] for v
+000005d0: 6965 7773 0a0a 5b73 6565 6473 5d3a 2068  iews..[seeds]: h
+000005e0: 7474 7073 3a2f 2f64 6f63 732e 6765 7464  ttps://docs.getd
+000005f0: 6274 2e63 6f6d 2f64 6f63 732f 6275 696c  bt.com/docs/buil
+00000600: 6469 6e67 2d61 2d64 6274 2d70 726f 6a65  ding-a-dbt-proje
+00000610: 6374 2f73 6565 6473 0a5b 696e 6372 656d  ct/seeds.[increm
+00000620: 656e 7461 6c5d 3a20 6874 7470 733a 2f2f  ental]: https://
+00000630: 646f 6373 2e67 6574 6462 742e 636f 6d2f  docs.getdbt.com/
+00000640: 646f 6373 2f62 7569 6c64 2f69 6e63 7265  docs/build/incre
+00000650: 6d65 6e74 616c 2d6d 6f64 656c 730a 5b74  mental-models.[t
+00000660: 6162 6c65 5d3a 2068 7474 7073 3a2f 2f64  able]: https://d
+00000670: 6f63 732e 6765 7464 6274 2e63 6f6d 2f64  ocs.getdbt.com/d
+00000680: 6f63 732f 6275 696c 642f 6d61 7465 7269  ocs/build/materi
+00000690: 616c 697a 6174 696f 6e73 2374 6162 6c65  alizations#table
+000006a0: 0a5b 7079 7468 6f6e 2d6d 6f64 656c 735d  .[python-models]
+000006b0: 3a20 6874 7470 733a 2f2f 646f 6373 2e67  : https://docs.g
+000006c0: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
+000006d0: 7569 6c64 2f70 7974 686f 6e2d 6d6f 6465  uild/python-mode
+000006e0: 6c73 2363 6f6e 6669 6775 7269 6e67 2d70  ls#configuring-p
+000006f0: 7974 686f 6e2d 6d6f 6465 6c73 0a5b 6174  ython-models.[at
+00000700: 6865 6e61 2d69 6365 6265 7267 5d3a 2068  hena-iceberg]: h
+00000710: 7474 7073 3a2f 2f64 6f63 732e 6177 732e  ttps://docs.aws.
+00000720: 616d 617a 6f6e 2e63 6f6d 2f61 7468 656e  amazon.com/athen
+00000730: 612f 6c61 7465 7374 2f75 672f 7175 6572  a/latest/ug/quer
+00000740: 7969 6e67 2d69 6365 6265 7267 2e68 746d  ying-iceberg.htm
+00000750: 6c0a 5b73 6e61 7073 686f 7473 5d3a 2068  l.[snapshots]: h
+00000760: 7474 7073 3a2f 2f64 6f63 732e 6765 7464  ttps://docs.getd
+00000770: 6274 2e63 6f6d 2f64 6f63 732f 6275 696c  bt.com/docs/buil
+00000780: 642f 736e 6170 7368 6f74 730a 5b70 6572  d/snapshots.[per
+00000790: 7369 7374 2d64 6f63 735d 3a20 6874 7470  sist-docs]: http
+000007a0: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
+000007b0: 636f 6d2f 7265 6665 7265 6e63 652f 7265  com/reference/re
+000007c0: 736f 7572 6365 2d63 6f6e 6669 6773 2f70  source-configs/p
+000007d0: 6572 7369 7374 5f64 6f63 730a 0a0a 2323  ersist_docs...##
+000007e0: 2051 7569 636b 2053 7461 7274 0a0a 2323   Quick Start..##
+000007f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
+00000800: 2a20 6070 6970 2069 6e73 7461 6c6c 2064  * `pip install d
+00000810: 6274 2d61 7468 656e 612d 636f 6d6d 756e  bt-athena-commun
+00000820: 6974 7960 0a2a 204f 7220 6070 6970 2069  ity`.* Or `pip i
+00000830: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
+00000840: 3a2f 2f67 6974 6875 622e 636f 6d2f 6462  ://github.com/db
+00000850: 742d 6174 6865 6e61 2f64 6274 2d61 7468  t-athena/dbt-ath
+00000860: 656e 612e 6769 7460 0a0a 2323 2320 5072  ena.git`..### Pr
+00000870: 6572 6571 7569 7369 7465 730a 0a54 6f20  erequisites..To 
+00000880: 7374 6172 742c 2079 6f75 2077 696c 6c20  start, you will 
+00000890: 6e65 6564 2061 6e20 5333 2062 7563 6b65  need an S3 bucke
+000008a0: 742c 2066 6f72 2069 6e73 7461 6e63 6520  t, for instance 
+000008b0: 606d 792d 6275 636b 6574 6020 616e 6420  `my-bucket` and 
+000008c0: 616e 2041 7468 656e 6120 6461 7461 6261  an Athena databa
+000008d0: 7365 3a0a 0a60 6060 7371 6c0a 4352 4541  se:..```sql.CREA
+000008e0: 5445 2044 4154 4142 4153 4520 4946 204e  TE DATABASE IF N
+000008f0: 4f54 2045 5849 5354 5320 616e 616c 7974  OT EXISTS analyt
+00000900: 6963 735f 6465 760a 434f 4d4d 454e 5420  ics_dev.COMMENT 
+00000910: 2741 6e61 6c79 7469 6373 206d 6f64 656c  'Analytics model
+00000920: 7320 6765 6e65 7261 7465 6420 6279 2064  s generated by d
+00000930: 6274 2028 6465 7665 6c6f 706d 656e 7429  bt (development)
+00000940: 270a 4c4f 4341 5449 4f4e 2027 7333 3a2f  '.LOCATION 's3:/
+00000950: 2f6d 792d 6275 636b 6574 2f27 0a57 4954  /my-bucket/'.WIT
+00000960: 4820 4442 5052 4f50 4552 5449 4553 2028  H DBPROPERTIES (
+00000970: 2763 7265 6174 6f72 273d 2746 6f6f 2042  'creator'='Foo B
+00000980: 6172 272c 2027 656d 6169 6c27 3d27 666f  ar', 'email'='fo
+00000990: 6f40 6261 722e 636f 6d27 293b 0a60 6060  o@bar.com');.```
+000009a0: 0a0a 4e6f 7465 733a 0a2d 2054 616b 6520  ..Notes:.- Take 
+000009b0: 6e6f 7465 206f 6620 796f 7572 2041 5753  note of your AWS
+000009c0: 2072 6567 696f 6e20 636f 6465 2028 652e   region code (e.
+000009d0: 672e 2060 7573 2d77 6573 742d 3260 206f  g. `us-west-2` o
+000009e0: 7220 6065 752d 7765 7374 2d32 602c 2065  r `eu-west-2`, e
+000009f0: 7463 2e29 2e0a 2d20 596f 7520 6361 6e20  tc.)..- You can 
+00000a00: 616c 736f 2075 7365 205b 4157 5320 476c  also use [AWS Gl
+00000a10: 7565 5d28 6874 7470 733a 2f2f 646f 6373  ue](https://docs
+00000a20: 2e61 7773 2e61 6d61 7a6f 6e2e 636f 6d2f  .aws.amazon.com/
+00000a30: 6174 6865 6e61 2f6c 6174 6573 742f 7567  athena/latest/ug
+00000a40: 2f67 6c75 652d 6174 6865 6e61 2e68 746d  /glue-athena.htm
+00000a50: 6c29 2074 6f20 6372 6561 7465 2061 6e64  l) to create and
+00000a60: 206d 616e 6167 6520 4174 6865 6e61 2064   manage Athena d
+00000a70: 6174 6162 6173 6573 2e0a 0a23 2323 2043  atabases...### C
+00000a80: 7265 6465 6e74 6961 6c73 0a0a 5468 6973  redentials..This
+00000a90: 2070 6c75 6769 6e20 646f 6573 206e 6f74   plugin does not
+00000aa0: 2061 6363 6570 7420 616e 7920 6372 6564   accept any cred
+00000ab0: 656e 7469 616c 7320 6469 7265 6374 6c79  entials directly
+00000ac0: 2e20 496e 7374 6561 642c 205b 6372 6564  . Instead, [cred
+00000ad0: 656e 7469 616c 7320 6172 6520 6465 7465  entials are dete
+00000ae0: 726d 696e 6564 2061 7574 6f6d 6174 6963  rmined automatic
+00000af0: 616c 6c79 5d28 6874 7470 733a 2f2f 626f  ally](https://bo
+00000b00: 746f 332e 616d 617a 6f6e 6177 732e 636f  to3.amazonaws.co
+00000b10: 6d2f 7631 2f64 6f63 756d 656e 7461 7469  m/v1/documentati
+00000b20: 6f6e 2f61 7069 2f6c 6174 6573 742f 6775  on/api/latest/gu
+00000b30: 6964 652f 6372 6564 656e 7469 616c 732e  ide/credentials.
+00000b40: 6874 6d6c 2920 6261 7365 6420 6f6e 2060  html) based on `
+00000b50: 6177 7320 636c 6960 2f60 626f 746f 3360  aws cli`/`boto3`
+00000b60: 2063 6f6e 7665 6e74 696f 6e73 2061 6e64   conventions and
+00000b70: 0a73 746f 7265 6420 6c6f 6769 6e20 696e  .stored login in
+00000b80: 666f 2e20 596f 7520 6361 6e20 636f 6e66  fo. You can conf
+00000b90: 6967 7572 6520 7468 6520 4157 5320 7072  igure the AWS pr
+00000ba0: 6f66 696c 6520 6e61 6d65 2074 6f20 7573  ofile name to us
+00000bb0: 6520 7669 6120 6061 7773 5f70 726f 6669  e via `aws_profi
+00000bc0: 6c65 5f6e 616d 6560 2e20 4368 6563 6b6f  le_name`. Checko
+00000bd0: 7574 2044 4254 2070 726f 6669 6c65 2063  ut DBT profile c
+00000be0: 6f6e 6669 6775 7261 7469 6f6e 2062 656c  onfiguration bel
+00000bf0: 6f77 2066 6f72 2064 6574 6169 6c73 2e0a  ow for details..
+00000c00: 0a23 2323 2043 6f6e 6669 6775 7269 6e67  .### Configuring
+00000c10: 2079 6f75 7220 7072 6f66 696c 650a 0a41   your profile..A
+00000c20: 2064 6274 2070 726f 6669 6c65 2063 616e   dbt profile can
+00000c30: 2062 6520 636f 6e66 6967 7572 6564 2074   be configured t
+00000c40: 6f20 7275 6e20 6167 6169 6e73 7420 4157  o run against AW
+00000c50: 5320 4174 6865 6e61 2075 7369 6e67 2074  S Athena using t
+00000c60: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+00000c70: 6669 6775 7261 7469 6f6e 3a0a 0a7c 204f  figuration:..| O
+00000c80: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
+00000c90: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2020 2020 2020 7c20 5265 7175            | Requ
-00000d10: 6972 6564 3f20 7c20 4578 616d 706c 6520  ired? | Example 
-00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
-00000d50: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00000ce0: 207c 2052 6571 7569 7265 643f 207c 2045   | Required? | E
+00000cf0: 7861 6d70 6c65 2020 2020 2020 2020 2020  xample          
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 2020 2020 7c0a 7c2d 2d2d 2d2d          |.|-----
+00000d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00000d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
+00000d80: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
 00000d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000da0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000db0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-00000de0: 7c20 7333 5f73 7461 6769 6e67 5f64 6972  | s3_staging_dir
-00000df0: 2020 207c 2053 3320 6c6f 6361 7469 6f6e     | S3 location
-00000e00: 2074 6f20 7374 6f72 6520 4174 6865 6e61   to store Athena
-00000e10: 2071 7565 7279 2072 6573 756c 7473 2061   query results a
-00000e20: 6e64 206d 6574 6164 6174 6120 2020 2020  nd metadata     
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 2020 2020 7c20 5265 7175 6972 6564 2020      | Required  
-00000e50: 7c20 6073 333a 2f2f 6275 636b 6574 2f64  | `s3://bucket/d
-00000e60: 6274 2f60 2020 2020 2020 2020 2020 2020  bt/`            
-00000e70: 2020 2020 2020 2020 2020 207c 0a7c 2073             |.| s
-00000e80: 335f 6461 7461 5f64 6972 2020 2020 2020  3_data_dir      
-00000e90: 7c20 5072 6566 6978 2066 6f72 2073 746f  | Prefix for sto
-00000ea0: 7269 6e67 2074 6162 6c65 732c 2069 6620  ring tables, if 
-00000eb0: 6469 6666 6572 656e 7420 6672 6f6d 2074  different from t
-00000ec0: 6865 2063 6f6e 6e65 6374 696f 6e27 7320  he connection's 
-00000ed0: 6073 335f 7374 6167 696e 675f 6469 7260  `s3_staging_dir`
-00000ee0: 207c 204f 7074 696f 6e61 6c20 207c 2060   | Optional  | `
-00000ef0: 7333 3a2f 2f62 7563 6b65 7432 2f64 6274  s3://bucket2/dbt
-00000f00: 2f60 2020 2020 2020 2020 2020 2020 2020  /`              
-00000f10: 2020 2020 2020 2020 7c0a 7c20 7333 5f64          |.| s3_d
-00000f20: 6174 615f 6e61 6d69 6e67 2020 207c 2048  ata_naming   | H
-00000f30: 6f77 2074 6f20 6765 6e65 7261 7465 2074  ow to generate t
-00000f40: 6162 6c65 2070 6174 6873 2069 6e20 6073  able paths in `s
-00000f50: 335f 6461 7461 5f64 6972 6020 2020 2020  3_data_dir`     
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000f80: 4f70 7469 6f6e 616c 2020 7c20 6073 6368  Optional  | `sch
-00000f90: 656d 615f 7461 626c 655f 756e 6971 7565  ema_table_unique
-00000fa0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00000fb0: 2020 2020 207c 0a7c 2072 6567 696f 6e5f       |.| region_
-00000fc0: 6e61 6d65 2020 2020 2020 7c20 4157 5320  name      | AWS 
-00000fd0: 7265 6769 6f6e 206f 6620 796f 7572 2041  region of your A
-00000fe0: 7468 656e 6120 696e 7374 616e 6365 2020  thena instance  
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 2020 2020 207c 2052 6571             | Req
-00001020: 7569 7265 6420 207c 2060 6575 2d77 6573  uired  | `eu-wes
-00001030: 742d 3160 2020 2020 2020 2020 2020 2020  t-1`            
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 7c0a 7c20 7363 6865 6d61 2020 2020    |.| schema    
-00001060: 2020 2020 2020 207c 2053 7065 6369 6679         | Specify
-00001070: 2074 6865 2073 6368 656d 6120 2841 7468   the schema (Ath
-00001080: 656e 6120 6461 7461 6261 7365 2920 746f  ena database) to
-00001090: 2062 7569 6c64 206d 6f64 656c 7320 696e   build models in
-000010a0: 746f 2028 6c6f 7765 7263 6173 6520 2a2a  to (lowercase **
-000010b0: 6f6e 6c79 2a2a 2920 7c20 5265 7175 6972  only**) | Requir
-000010c0: 6564 2020 7c20 6064 6274 6020 2020 2020  ed  | `dbt`     
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000010f0: 0a7c 2064 6174 6162 6173 6520 2020 2020  .| database     
-00001100: 2020 2020 7c20 5370 6563 6966 7920 7468      | Specify th
-00001110: 6520 6461 7461 6261 7365 2028 4461 7461  e database (Data
-00001120: 2063 6174 616c 6f67 2920 746f 2062 7569   catalog) to bui
-00001130: 6c64 206d 6f64 656c 7320 696e 746f 2028  ld models into (
-00001140: 6c6f 7765 7263 6173 6520 2a2a 6f6e 6c79  lowercase **only
-00001150: 2a2a 2920 207c 2052 6571 7569 7265 6420  **)  | Required 
-00001160: 207c 2060 6177 7364 6174 6163 6174 616c   | `awsdatacatal
-00001170: 6f67 6020 2020 2020 2020 2020 2020 2020  og`             
-00001180: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00001190: 706f 6c6c 5f69 6e74 6572 7661 6c20 2020  poll_interval   
-000011a0: 207c 2049 6e74 6572 7661 6c20 696e 2073   | Interval in s
-000011b0: 6563 6f6e 6473 2074 6f20 7573 6520 666f  econds to use fo
-000011c0: 7220 706f 6c6c 696e 6720 7468 6520 7374  r polling the st
-000011d0: 6174 7573 206f 6620 7175 6572 7920 7265  atus of query re
-000011e0: 7375 6c74 7320 696e 2041 7468 656e 6120  sults in Athena 
-000011f0: 2020 7c20 4f70 7469 6f6e 616c 2020 7c20    | Optional  | 
-00001200: 6035 6020 2020 2020 2020 2020 2020 2020  `5`             
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 207c 0a7c 2061 7773           |.| aws
-00001230: 5f70 726f 6669 6c65 5f6e 616d 6520 7c20  _profile_name | 
-00001240: 5072 6f66 696c 6520 746f 2075 7365 2066  Profile to use f
-00001250: 726f 6d20 796f 7572 2041 5753 2073 6861  rom your AWS sha
-00001260: 7265 6420 6372 6564 656e 7469 616c 7320  red credentials 
-00001270: 6669 6c65 2e20 2020 2020 2020 2020 2020  file.           
-00001280: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001290: 204f 7074 696f 6e61 6c20 207c 2060 6d79   Optional  | `my
-000012a0: 2d70 726f 6669 6c65 6020 2020 2020 2020  -profile`       
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 7c0a 7c20 776f 726b 5f67        |.| work_g
-000012d0: 726f 7570 2020 2020 2020 207c 2049 6465  roup       | Ide
-000012e0: 6e74 6966 6965 7220 6f66 2041 7468 656e  ntifier of Athen
-000012f0: 6120 776f 726b 6772 6f75 7020 2020 2020  a workgroup     
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 2020 2020 2020 2020 7c20 4f70              | Op
-00001330: 7469 6f6e 616c 2020 7c20 606d 792d 6375  tional  | `my-cu
-00001340: 7374 6f6d 2d77 6f72 6b67 726f 7570 6020  stom-workgroup` 
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 207c 0a7c 206e 756d 5f72 6574 7269     |.| num_retri
-00001370: 6573 2020 2020 2020 7c20 4e75 6d62 6572  es      | Number
-00001380: 206f 6620 7469 6d65 7320 746f 2072 6574   of times to ret
-00001390: 7279 2061 2066 6169 6c69 6e67 2071 7565  ry a failing que
-000013a0: 7279 2020 2020 2020 2020 2020 2020 2020  ry              
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 2020 2020 207c 204f 7074 696f           | Optio
-000013d0: 6e61 6c20 207c 2060 3360 2020 2020 2020  nal  | `3`      
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 7c0a 7c20 6c66 5f74 6167 7320 2020 2020  |.| lf_tags     
-00001410: 2020 2020 207c 2044 6566 6175 6c74 206c       | Default l
-00001420: 6620 7461 6773 2074 6f20 6170 706c 7920  f tags to apply 
-00001430: 746f 2061 6e79 2064 6174 6162 6173 6520  to any database 
-00001440: 6372 6561 7465 6420 6279 2064 6274 2020  created by dbt  
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 2020 2020 2020 7c20 4f70 7469 6f6e 616c        | Optional
-00001470: 2020 7c20 607b 226f 7269 6769 6e22 3a20    | `{"origin": 
-00001480: 2264 6274 222c 2022 7465 616d 223a 2022  "dbt", "team": "
-00001490: 616e 616c 7974 6963 7322 7d60 207c 0a0a  analytics"}` |..
-000014a0: 2a2a 4578 616d 706c 6520 7072 6f66 696c  **Example profil
-000014b0: 6573 2e79 6d6c 2065 6e74 7279 3a2a 2a0a  es.yml entry:**.
-000014c0: 6060 6079 616d 6c0a 6174 6865 6e61 3a0a  ```yaml.athena:.
-000014d0: 2020 7461 7267 6574 3a20 6465 760a 2020    target: dev.  
-000014e0: 6f75 7470 7574 733a 0a20 2020 2064 6576  outputs:.    dev
-000014f0: 3a0a 2020 2020 2020 7479 7065 3a20 6174  :.      type: at
-00001500: 6865 6e61 0a20 2020 2020 2073 335f 7374  hena.      s3_st
-00001510: 6167 696e 675f 6469 723a 2073 333a 2f2f  aging_dir: s3://
-00001520: 6174 6865 6e61 2d71 7565 7279 2d72 6573  athena-query-res
-00001530: 756c 7473 2f64 6274 2f0a 2020 2020 2020  ults/dbt/.      
-00001540: 7333 5f64 6174 615f 6469 723a 2073 333a  s3_data_dir: s3:
-00001550: 2f2f 796f 7572 5f73 335f 6275 636b 6574  //your_s3_bucket
-00001560: 2f64 6274 2f0a 2020 2020 2020 7333 5f64  /dbt/.      s3_d
-00001570: 6174 615f 6e61 6d69 6e67 3a20 7363 6865  ata_naming: sche
-00001580: 6d61 5f74 6162 6c65 0a20 2020 2020 2072  ma_table.      r
-00001590: 6567 696f 6e5f 6e61 6d65 3a20 6575 2d77  egion_name: eu-w
-000015a0: 6573 742d 310a 2020 2020 2020 7363 6865  est-1.      sche
-000015b0: 6d61 3a20 6462 740a 2020 2020 2020 6461  ma: dbt.      da
-000015c0: 7461 6261 7365 3a20 6177 7364 6174 6163  tabase: awsdatac
-000015d0: 6174 616c 6f67 0a20 2020 2020 2061 7773  atalog.      aws
-000015e0: 5f70 726f 6669 6c65 5f6e 616d 653a 206d  _profile_name: m
-000015f0: 792d 7072 6f66 696c 650a 2020 2020 2020  y-profile.      
-00001600: 776f 726b 5f67 726f 7570 3a20 6d79 2d77  work_group: my-w
-00001610: 6f72 6b67 726f 7570 0a20 2020 2020 206c  orkgroup.      l
-00001620: 665f 7461 6773 3a0a 2020 2020 2020 2020  f_tags:.        
-00001630: 6f72 6967 696e 3a20 6462 740a 2020 2020  origin: dbt.    
-00001640: 2020 2020 7465 616d 3a20 616e 616c 7974      team: analyt
-00001650: 6963 730a 6060 600a 0a5f 4164 6469 7469  ics.```.._Additi
-00001660: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
-00001670: 5f0a 2a20 6074 6872 6561 6473 6020 6973  _.* `threads` is
-00001680: 2073 7570 706f 7274 6564 0a2a 2060 6461   supported.* `da
-00001690: 7461 6261 7365 6020 616e 6420 6063 6174  tabase` and `cat
-000016a0: 616c 6f67 6020 6361 6e20 6265 2075 7365  alog` can be use
-000016b0: 6420 696e 7465 7263 6861 6e67 6561 626c  d interchangeabl
-000016c0: 790a 0a23 2323 204d 6f64 656c 730a 0a23  y..### Models..#
-000016d0: 2323 2320 5461 626c 6520 436f 6e66 6967  ### Table Config
-000016e0: 7572 6174 696f 6e0a 0a2a 2060 6578 7465  uration..* `exte
-000016f0: 726e 616c 5f6c 6f63 6174 696f 6e60 2028  rnal_location` (
-00001700: 6064 6566 6175 6c74 3d6e 6f6e 6560 290a  `default=none`).
-00001710: 2020 2a20 4966 2073 6574 2c20 7468 6520    * If set, the 
-00001720: 6675 6c6c 2053 3320 7061 7468 2069 6e20  full S3 path in 
-00001730: 7768 6963 6820 7468 6520 7461 626c 6520  which the table 
-00001740: 7769 6c6c 2062 6520 7361 7665 642e 2028  will be saved. (
-00001750: 446f 6573 206e 6f74 2077 6f72 6b20 7769  Does not work wi
-00001760: 7468 2049 6365 6265 7267 2074 6162 6c65  th Iceberg table
-00001770: 292e 0a2a 2060 7061 7274 6974 696f 6e65  )..* `partitione
-00001780: 645f 6279 6020 2860 6465 6661 756c 743d  d_by` (`default=
-00001790: 6e6f 6e65 6029 0a20 202a 2041 6e20 6172  none`).  * An ar
-000017a0: 7261 7920 6c69 7374 206f 6620 636f 6c75  ray list of colu
-000017b0: 6d6e 7320 6279 2077 6869 6368 2074 6865  mns by which the
-000017c0: 2074 6162 6c65 2077 696c 6c20 6265 2070   table will be p
-000017d0: 6172 7469 7469 6f6e 6564 0a20 202a 204c  artitioned.  * L
-000017e0: 696d 6974 6564 2074 6f20 6372 6561 7469  imited to creati
-000017f0: 6f6e 206f 6620 3130 3020 7061 7274 6974  on of 100 partit
-00001800: 696f 6e73 2028 5f63 7572 7265 6e74 6c79  ions (_currently
-00001810: 5f29 0a2a 2060 6275 636b 6574 6564 5f62  _).* `bucketed_b
-00001820: 7960 2028 6064 6566 6175 6c74 3d6e 6f6e  y` (`default=non
-00001830: 6560 290a 2020 2a20 416e 2061 7272 6179  e`).  * An array
-00001840: 206c 6973 7420 6f66 2063 6f6c 756d 6e73   list of columns
-00001850: 2074 6f20 6275 636b 6574 2064 6174 612c   to bucket data,
-00001860: 2069 676e 6f72 6564 2069 6620 7573 696e   ignored if usin
-00001870: 6720 4963 6562 6572 670a 2a20 6062 7563  g Iceberg.* `buc
-00001880: 6b65 745f 636f 756e 7460 2028 6064 6566  ket_count` (`def
-00001890: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-000018a0: 5468 6520 6e75 6d62 6572 206f 6620 6275  The number of bu
-000018b0: 636b 6574 7320 666f 7220 6275 636b 6574  ckets for bucket
-000018c0: 696e 6720 796f 7572 2064 6174 612c 2069  ing your data, i
-000018d0: 676e 6f72 6564 2069 6620 7573 696e 6720  gnored if using 
-000018e0: 4963 6562 6572 670a 2a20 6074 6162 6c65  Iceberg.* `table
-000018f0: 5f74 7970 6560 2028 6064 6566 6175 6c74  _type` (`default
-00001900: 3d27 6869 7665 2760 290a 2020 2a20 5468  ='hive'`).  * Th
-00001910: 6520 7479 7065 206f 6620 7461 626c 650a  e type of table.
-00001920: 2020 2a20 5375 7070 6f72 7473 2060 6869    * Supports `hi
-00001930: 7665 6020 6f72 2060 6963 6562 6572 6760  ve` or `iceberg`
-00001940: 0a2a 2060 666f 726d 6174 6020 2860 6465  .* `format` (`de
-00001950: 6661 756c 743d 2770 6172 7175 6574 2760  fault='parquet'`
-00001960: 290a 2020 2a20 5468 6520 6461 7461 2066  ).  * The data f
-00001970: 6f72 6d61 7420 666f 7220 7468 6520 7461  ormat for the ta
-00001980: 626c 650a 2020 2a20 5375 7070 6f72 7473  ble.  * Supports
-00001990: 2060 4f52 4360 2c20 6050 4152 5155 4554   `ORC`, `PARQUET
-000019a0: 602c 2060 4156 524f 602c 2060 4a53 4f4e  `, `AVRO`, `JSON
-000019b0: 602c 2060 5445 5854 4649 4c45 600a 2a20  `, `TEXTFILE`.* 
-000019c0: 6077 7269 7465 5f63 6f6d 7072 6573 7369  `write_compressi
-000019d0: 6f6e 6020 2860 6465 6661 756c 743d 6e6f  on` (`default=no
-000019e0: 6e65 6029 0a20 202a 2054 6865 2063 6f6d  ne`).  * The com
-000019f0: 7072 6573 7369 6f6e 2074 7970 6520 746f  pression type to
-00001a00: 2075 7365 2066 6f72 2061 6e79 2073 746f   use for any sto
-00001a10: 7261 6765 2066 6f72 6d61 7420 7468 6174  rage format that
-00001a20: 2061 6c6c 6f77 7320 636f 6d70 7265 7373   allows compress
-00001a30: 696f 6e20 746f 2062 6520 7370 6563 6966  ion to be specif
-00001a40: 6965 642e 2054 6f20 7365 6520 7768 6963  ied. To see whic
-00001a50: 6820 6f70 7469 6f6e 7320 6172 6520 6176  h options are av
-00001a60: 6169 6c61 626c 652c 2063 6865 636b 206f  ailable, check o
-00001a70: 7574 205b 4352 4541 5445 2054 4142 4c45  ut [CREATE TABLE
-00001a80: 2041 535d 5b63 7265 6174 652d 7461 626c   AS][create-tabl
-00001a90: 652d 6173 5d0a 2a20 6066 6965 6c64 5f64  e-as].* `field_d
-00001aa0: 656c 696d 6974 6572 6020 2860 6465 6661  elimiter` (`defa
-00001ab0: 756c 743d 6e6f 6e65 6029 0a20 202a 2043  ult=none`).  * C
-00001ac0: 7573 746f 6d20 6669 656c 6420 6465 6c69  ustom field deli
-00001ad0: 6d69 7465 722c 2066 6f72 2077 6865 6e20  miter, for when 
-00001ae0: 666f 726d 6174 2069 7320 7365 7420 746f  format is set to
-00001af0: 2060 5445 5854 4649 4c45 600a 2a20 6074   `TEXTFILE`.* `t
-00001b00: 6162 6c65 5f70 726f 7065 7274 6965 7360  able_properties`
-00001b10: 3a20 7461 626c 6520 7072 6f70 6572 7469  : table properti
-00001b20: 6573 2074 6f20 6164 6420 746f 2074 6865  es to add to the
-00001b30: 2074 6162 6c65 2c20 7661 6c69 6420 666f   table, valid fo
-00001b40: 7220 4963 6562 6572 6720 6f6e 6c79 0a2a  r Iceberg only.*
-00001b50: 2060 6c66 5f74 6167 7360 2028 6064 6566   `lf_tags` (`def
-00001b60: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-00001b70: 6c66 2074 6167 7320 746f 2061 7373 6f63  lf tags to assoc
-00001b80: 6961 7465 2077 6974 6820 7468 6520 7461  iate with the ta
-00001b90: 626c 650a 2020 2a20 666f 726d 6174 3a20  ble.  * format: 
-00001ba0: 607b 2274 6167 3122 3a20 2276 616c 7565  `{"tag1": "value
-00001bb0: 3122 2c20 2274 6167 3222 3a20 2276 616c  1", "tag2": "val
-00001bc0: 7565 3222 7d60 0a2a 2060 6c66 5f74 6167  ue2"}`.* `lf_tag
-00001bd0: 735f 636f 6c75 6d6e 7360 2028 6064 6566  s_columns` (`def
-00001be0: 6175 6c74 3d6e 6f6e 6560 290a 2020 2a20  ault=none`).  * 
-00001bf0: 6c66 2074 6167 7320 746f 2061 7373 6f63  lf tags to assoc
-00001c00: 6961 7465 2077 6974 6820 7468 6520 7461  iate with the ta
-00001c10: 626c 6520 636f 6c75 6d6e 730a 2020 2a20  ble columns.  * 
-00001c20: 666f 726d 6174 3a20 607b 2274 6167 3122  format: `{"tag1"
-00001c30: 3a20 7b22 7661 6c75 6531 223a 205b 2263  : {"value1": ["c
-00001c40: 6f6c 756d 6e31 223a 2022 636f 6c75 6d6e  olumn1": "column
-00001c50: 3222 5d7d 7d60 0a0a 2323 2323 2054 6162  2"]}}`..#### Tab
-00001c60: 6c65 206c 6f63 6174 696f 6e0a 0a54 6865  le location..The
-00001c70: 206c 6f63 6174 696f 6e20 696e 2077 6869   location in whi
-00001c80: 6368 2061 2074 6162 6c65 2069 7320 7361  ch a table is sa
-00001c90: 7665 6420 6973 2064 6574 6572 6d69 6e65  ved is determine
-00001ca0: 6420 6279 3a0a 0a31 2e20 4966 2060 6578  d by:..1. If `ex
-00001cb0: 7465 726e 616c 5f6c 6f63 6174 696f 6e60  ternal_location`
-00001cc0: 2069 7320 6465 6669 6e65 642c 2074 6861   is defined, tha
-00001cd0: 7420 7661 6c75 6520 6973 2075 7365 642e  t value is used.
-00001ce0: 0a32 2e20 4966 2060 7333 5f64 6174 615f  .2. If `s3_data_
-00001cf0: 6469 7260 2069 7320 6465 6669 6e65 642c  dir` is defined,
-00001d00: 2074 6865 2070 6174 6820 6973 2064 6574   the path is det
-00001d10: 6572 6d69 6e65 6420 6279 2074 6861 7420  ermined by that 
-00001d20: 616e 6420 6073 335f 6461 7461 5f6e 616d  and `s3_data_nam
-00001d30: 696e 6760 0a33 2e20 4966 2060 7333 5f64  ing`.3. If `s3_d
-00001d40: 6174 615f 6469 7260 2069 7320 6e6f 7420  ata_dir` is not 
-00001d50: 6465 6669 6e65 6420 6461 7461 2069 7320  defined data is 
-00001d60: 7374 6f72 6564 2075 6e64 6572 2060 7333  stored under `s3
-00001d70: 5f73 7461 6769 6e67 5f64 6972 2f74 6162  _staging_dir/tab
-00001d80: 6c65 732f 600a 0a48 6572 6520 616c 6c20  les/`..Here all 
-00001d90: 7468 6520 6f70 7469 6f6e 7320 6176 6169  the options avai
-00001da0: 6c61 626c 6520 666f 7220 6073 335f 6461  lable for `s3_da
-00001db0: 7461 5f6e 616d 696e 6760 3a0a 2a20 6075  ta_naming`:.* `u
-00001dc0: 7569 6460 3a20 607b 7333 5f64 6174 615f  uid`: `{s3_data_
-00001dd0: 6469 727d 2f7b 7575 6964 3428 297d 2f60  dir}/{uuid4()}/`
-00001de0: 0a2a 2060 7461 626c 655f 7461 626c 6560  .* `table_table`
+00000da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000db0: 2d2d 2d2d 2d7c 0a7c 2073 335f 7374 6167  -----|.| s3_stag
+00000dc0: 696e 675f 6469 7220 2020 7c20 5333 206c  ing_dir   | S3 l
+00000dd0: 6f63 6174 696f 6e20 746f 2073 746f 7265  ocation to store
+00000de0: 2041 7468 656e 6120 7175 6572 7920 7265   Athena query re
+00000df0: 7375 6c74 7320 616e 6420 6d65 7461 6461  sults and metada
+00000e00: 7461 2020 2020 2020 2020 2020 2020 2020  ta              
+00000e10: 2020 2020 2020 2020 2020 207c 2052 6571             | Req
+00000e20: 7569 7265 6420 207c 2060 7333 3a2f 2f62  uired  | `s3://b
+00000e30: 7563 6b65 742f 6462 742f 6020 2020 2020  ucket/dbt/`     
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 7c0a 7c20 7333 5f64 6174 615f 6469    |.| s3_data_di
+00000e60: 7220 2020 2020 207c 2050 7265 6669 7820  r      | Prefix 
+00000e70: 666f 7220 7374 6f72 696e 6720 7461 626c  for storing tabl
+00000e80: 6573 2c20 6966 2064 6966 6665 7265 6e74  es, if different
+00000e90: 2066 726f 6d20 7468 6520 636f 6e6e 6563   from the connec
+00000ea0: 7469 6f6e 2773 2060 7333 5f73 7461 6769  tion's `s3_stagi
+00000eb0: 6e67 5f64 6972 6020 7c20 4f70 7469 6f6e  ng_dir` | Option
+00000ec0: 616c 2020 7c20 6073 333a 2f2f 6275 636b  al  | `s3://buck
+00000ed0: 6574 322f 6462 742f 6020 2020 2020 2020  et2/dbt/`       
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000ef0: 0a7c 2073 335f 6461 7461 5f6e 616d 696e  .| s3_data_namin
+00000f00: 6720 2020 7c20 486f 7720 746f 2067 656e  g   | How to gen
+00000f10: 6572 6174 6520 7461 626c 6520 7061 7468  erate table path
+00000f20: 7320 696e 2060 7333 5f64 6174 615f 6469  s in `s3_data_di
+00000f30: 7260 2020 2020 2020 2020 2020 2020 2020  r`              
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2020 207c 204f 7074 696f 6e61 6c20       | Optional 
+00000f60: 207c 2060 7363 6865 6d61 5f74 6162 6c65   | `schema_table
+00000f70: 5f75 6e69 7175 6560 2020 2020 2020 2020  _unique`        
+00000f80: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00000f90: 7265 6769 6f6e 5f6e 616d 6520 2020 2020  region_name     
+00000fa0: 207c 2041 5753 2072 6567 696f 6e20 6f66   | AWS region of
+00000fb0: 2079 6f75 7220 4174 6865 6e61 2069 6e73   your Athena ins
+00000fc0: 7461 6e63 6520 2020 2020 2020 2020 2020  tance           
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 2020 7c20 5265 7175 6972 6564 2020 7c20    | Required  | 
+00001000: 6065 752d 7765 7374 2d31 6020 2020 2020  `eu-west-1`     
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 2020 2020 2020 207c 0a7c 2073 6368           |.| sch
+00001030: 656d 6120 2020 2020 2020 2020 2020 7c20  ema           | 
+00001040: 5370 6563 6966 7920 7468 6520 7363 6865  Specify the sche
+00001050: 6d61 2028 4174 6865 6e61 2064 6174 6162  ma (Athena datab
+00001060: 6173 6529 2074 6f20 6275 696c 6420 6d6f  ase) to build mo
+00001070: 6465 6c73 2069 6e74 6f20 286c 6f77 6572  dels into (lower
+00001080: 6361 7365 202a 2a6f 6e6c 792a 2a29 207c  case **only**) |
+00001090: 2052 6571 7569 7265 6420 207c 2060 6462   Required  | `db
+000010a0: 7460 2020 2020 2020 2020 2020 2020 2020  t`              
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 2020 2020 2020 7c0a 7c20 6461 7461 6261        |.| databa
+000010d0: 7365 2020 2020 2020 2020 207c 2053 7065  se         | Spe
+000010e0: 6369 6679 2074 6865 2064 6174 6162 6173  cify the databas
+000010f0: 6520 2844 6174 6120 6361 7461 6c6f 6729  e (Data catalog)
+00001100: 2074 6f20 6275 696c 6420 6d6f 6465 6c73   to build models
+00001110: 2069 6e74 6f20 286c 6f77 6572 6361 7365   into (lowercase
+00001120: 202a 2a6f 6e6c 792a 2a29 2020 7c20 5265   **only**)  | Re
+00001130: 7175 6972 6564 2020 7c20 6061 7773 6461  quired  | `awsda
+00001140: 7461 6361 7461 6c6f 6760 2020 2020 2020  tacatalog`      
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 207c 0a7c 2070 6f6c 6c5f 696e 7465     |.| poll_inte
+00001170: 7276 616c 2020 2020 7c20 496e 7465 7276  rval    | Interv
+00001180: 616c 2069 6e20 7365 636f 6e64 7320 746f  al in seconds to
+00001190: 2075 7365 2066 6f72 2070 6f6c 6c69 6e67   use for polling
+000011a0: 2074 6865 2073 7461 7475 7320 6f66 2071   the status of q
+000011b0: 7565 7279 2072 6573 756c 7473 2069 6e20  uery results in 
+000011c0: 4174 6865 6e61 2020 207c 204f 7074 696f  Athena   | Optio
+000011d0: 6e61 6c20 207c 2060 3560 2020 2020 2020  nal  | `5`      
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 7c0a 7c20 6177 735f 7072 6f66 696c 655f  |.| aws_profile_
+00001210: 6e61 6d65 207c 2050 726f 6669 6c65 2074  name | Profile t
+00001220: 6f20 7573 6520 6672 6f6d 2079 6f75 7220  o use from your 
+00001230: 4157 5320 7368 6172 6564 2063 7265 6465  AWS shared crede
+00001240: 6e74 6961 6c73 2066 696c 652e 2020 2020  ntials file.    
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 7c20 4f70 7469 6f6e 616c        | Optional
+00001270: 2020 7c20 606d 792d 7072 6f66 696c 6560    | `my-profile`
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000012a0: 2077 6f72 6b5f 6772 6f75 7020 2020 2020   work_group     
+000012b0: 2020 7c20 4964 656e 7469 6669 6572 206f    | Identifier o
+000012c0: 6620 4174 6865 6e61 2077 6f72 6b67 726f  f Athena workgro
+000012d0: 7570 2020 2020 2020 2020 2020 2020 2020  up              
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 207c 204f 7074 696f 6e61 6c20 207c     | Optional  |
+00001310: 2060 6d79 2d63 7573 746f 6d2d 776f 726b   `my-custom-work
+00001320: 6772 6f75 7060 2020 2020 2020 2020 2020  group`          
+00001330: 2020 2020 2020 2020 2020 7c0a 7c20 6e75            |.| nu
+00001340: 6d5f 7265 7472 6965 7320 2020 2020 207c  m_retries      |
+00001350: 204e 756d 6265 7220 6f66 2074 696d 6573   Number of times
+00001360: 2074 6f20 7265 7472 7920 6120 6661 696c   to retry a fail
+00001370: 696e 6720 7175 6572 7920 2020 2020 2020  ing query       
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 7c20 4f70 7469 6f6e 616c 2020 7c20 6033  | Optional  | `3
+000013b0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 2020 2020 207c 0a7c 206c 665f 7461         |.| lf_ta
+000013e0: 6773 2020 2020 2020 2020 2020 7c20 4465  gs          | De
+000013f0: 6661 756c 7420 6c66 2074 6167 7320 746f  fault lf tags to
+00001400: 2061 7070 6c79 2074 6f20 616e 7920 6461   apply to any da
+00001410: 7461 6261 7365 2063 7265 6174 6564 2062  tabase created b
+00001420: 7920 6462 7420 2020 2020 2020 2020 2020  y dbt           
+00001430: 2020 2020 2020 2020 2020 2020 207c 204f               | O
+00001440: 7074 696f 6e61 6c20 207c 2060 7b22 6f72  ptional  | `{"or
+00001450: 6967 696e 223a 2022 6462 7422 2c20 2274  igin": "dbt", "t
+00001460: 6561 6d22 3a20 2261 6e61 6c79 7469 6373  eam": "analytics
+00001470: 227d 6020 7c0a 0a2a 2a45 7861 6d70 6c65  "}` |..**Example
+00001480: 2070 726f 6669 6c65 732e 796d 6c20 656e   profiles.yml en
+00001490: 7472 793a 2a2a 0a60 6060 7961 6d6c 0a61  try:**.```yaml.a
+000014a0: 7468 656e 613a 0a20 2074 6172 6765 743a  thena:.  target:
+000014b0: 2064 6576 0a20 206f 7574 7075 7473 3a0a   dev.  outputs:.
+000014c0: 2020 2020 6465 763a 0a20 2020 2020 2074      dev:.      t
+000014d0: 7970 653a 2061 7468 656e 610a 2020 2020  ype: athena.    
+000014e0: 2020 7333 5f73 7461 6769 6e67 5f64 6972    s3_staging_dir
+000014f0: 3a20 7333 3a2f 2f61 7468 656e 612d 7175  : s3://athena-qu
+00001500: 6572 792d 7265 7375 6c74 732f 6462 742f  ery-results/dbt/
+00001510: 0a20 2020 2020 2073 335f 6461 7461 5f64  .      s3_data_d
+00001520: 6972 3a20 7333 3a2f 2f79 6f75 725f 7333  ir: s3://your_s3
+00001530: 5f62 7563 6b65 742f 6462 742f 0a20 2020  _bucket/dbt/.   
+00001540: 2020 2073 335f 6461 7461 5f6e 616d 696e     s3_data_namin
+00001550: 673a 2073 6368 656d 615f 7461 626c 650a  g: schema_table.
+00001560: 2020 2020 2020 7265 6769 6f6e 5f6e 616d        region_nam
+00001570: 653a 2065 752d 7765 7374 2d31 0a20 2020  e: eu-west-1.   
+00001580: 2020 2073 6368 656d 613a 2064 6274 0a20     schema: dbt. 
+00001590: 2020 2020 2064 6174 6162 6173 653a 2061       database: a
+000015a0: 7773 6461 7461 6361 7461 6c6f 670a 2020  wsdatacatalog.  
+000015b0: 2020 2020 6177 735f 7072 6f66 696c 655f      aws_profile_
+000015c0: 6e61 6d65 3a20 6d79 2d70 726f 6669 6c65  name: my-profile
+000015d0: 0a20 2020 2020 2077 6f72 6b5f 6772 6f75  .      work_grou
+000015e0: 703a 206d 792d 776f 726b 6772 6f75 700a  p: my-workgroup.
+000015f0: 2020 2020 2020 6c66 5f74 6167 733a 0a20        lf_tags:. 
+00001600: 2020 2020 2020 206f 7269 6769 6e3a 2064         origin: d
+00001610: 6274 0a20 2020 2020 2020 2074 6561 6d3a  bt.        team:
+00001620: 2061 6e61 6c79 7469 6373 0a60 6060 0a0a   analytics.```..
+00001630: 5f41 6464 6974 696f 6e61 6c20 696e 666f  _Additional info
+00001640: 726d 6174 696f 6e5f 0a2a 2060 7468 7265  rmation_.* `thre
+00001650: 6164 7360 2069 7320 7375 7070 6f72 7465  ads` is supporte
+00001660: 640a 2a20 6064 6174 6162 6173 6560 2061  d.* `database` a
+00001670: 6e64 2060 6361 7461 6c6f 6760 2063 616e  nd `catalog` can
+00001680: 2062 6520 7573 6564 2069 6e74 6572 6368   be used interch
+00001690: 616e 6765 6162 6c79 0a0a 0a23 2320 4d6f  angeably...## Mo
+000016a0: 6465 6c73 0a0a 2323 2320 5461 626c 6520  dels..### Table 
+000016b0: 436f 6e66 6967 7572 6174 696f 6e0a 0a2a  Configuration..*
+000016c0: 2060 6578 7465 726e 616c 5f6c 6f63 6174   `external_locat
+000016d0: 696f 6e60 2028 6064 6566 6175 6c74 3d6e  ion` (`default=n
+000016e0: 6f6e 6560 290a 2020 2a20 4966 2073 6574  one`).  * If set
+000016f0: 2c20 7468 6520 6675 6c6c 2053 3320 7061  , the full S3 pa
+00001700: 7468 2069 6e20 7768 6963 6820 7468 6520  th in which the 
+00001710: 7461 626c 6520 7769 6c6c 2062 6520 7361  table will be sa
+00001720: 7665 642e 2028 446f 6573 206e 6f74 2077  ved. (Does not w
+00001730: 6f72 6b20 7769 7468 2049 6365 6265 7267  ork with Iceberg
+00001740: 2074 6162 6c65 292e 0a2a 2060 7061 7274   table)..* `part
+00001750: 6974 696f 6e65 645f 6279 6020 2860 6465  itioned_by` (`de
+00001760: 6661 756c 743d 6e6f 6e65 6029 0a20 202a  fault=none`).  *
+00001770: 2041 6e20 6172 7261 7920 6c69 7374 206f   An array list o
+00001780: 6620 636f 6c75 6d6e 7320 6279 2077 6869  f columns by whi
+00001790: 6368 2074 6865 2074 6162 6c65 2077 696c  ch the table wil
+000017a0: 6c20 6265 2070 6172 7469 7469 6f6e 6564  l be partitioned
+000017b0: 0a20 202a 204c 696d 6974 6564 2074 6f20  .  * Limited to 
+000017c0: 6372 6561 7469 6f6e 206f 6620 3130 3020  creation of 100 
+000017d0: 7061 7274 6974 696f 6e73 2028 5f63 7572  partitions (_cur
+000017e0: 7265 6e74 6c79 5f29 0a2a 2060 6275 636b  rently_).* `buck
+000017f0: 6574 6564 5f62 7960 2028 6064 6566 6175  eted_by` (`defau
+00001800: 6c74 3d6e 6f6e 6560 290a 2020 2a20 416e  lt=none`).  * An
+00001810: 2061 7272 6179 206c 6973 7420 6f66 2063   array list of c
+00001820: 6f6c 756d 6e73 2074 6f20 6275 636b 6574  olumns to bucket
+00001830: 2064 6174 612c 2069 676e 6f72 6564 2069   data, ignored i
+00001840: 6620 7573 696e 6720 4963 6562 6572 670a  f using Iceberg.
+00001850: 2a20 6062 7563 6b65 745f 636f 756e 7460  * `bucket_count`
+00001860: 2028 6064 6566 6175 6c74 3d6e 6f6e 6560   (`default=none`
+00001870: 290a 2020 2a20 5468 6520 6e75 6d62 6572  ).  * The number
+00001880: 206f 6620 6275 636b 6574 7320 666f 7220   of buckets for 
+00001890: 6275 636b 6574 696e 6720 796f 7572 2064  bucketing your d
+000018a0: 6174 612c 2069 676e 6f72 6564 2069 6620  ata, ignored if 
+000018b0: 7573 696e 6720 4963 6562 6572 670a 2a20  using Iceberg.* 
+000018c0: 6074 6162 6c65 5f74 7970 6560 2028 6064  `table_type` (`d
+000018d0: 6566 6175 6c74 3d27 6869 7665 2760 290a  efault='hive'`).
+000018e0: 2020 2a20 5468 6520 7479 7065 206f 6620    * The type of 
+000018f0: 7461 626c 650a 2020 2a20 5375 7070 6f72  table.  * Suppor
+00001900: 7473 2060 6869 7665 6020 6f72 2060 6963  ts `hive` or `ic
+00001910: 6562 6572 6760 0a2a 2060 666f 726d 6174  eberg`.* `format
+00001920: 6020 2860 6465 6661 756c 743d 2770 6172  ` (`default='par
+00001930: 7175 6574 2760 290a 2020 2a20 5468 6520  quet'`).  * The 
+00001940: 6461 7461 2066 6f72 6d61 7420 666f 7220  data format for 
+00001950: 7468 6520 7461 626c 650a 2020 2a20 5375  the table.  * Su
+00001960: 7070 6f72 7473 2060 4f52 4360 2c20 6050  pports `ORC`, `P
+00001970: 4152 5155 4554 602c 2060 4156 524f 602c  ARQUET`, `AVRO`,
+00001980: 2060 4a53 4f4e 602c 2060 5445 5854 4649   `JSON`, `TEXTFI
+00001990: 4c45 600a 2a20 6077 7269 7465 5f63 6f6d  LE`.* `write_com
+000019a0: 7072 6573 7369 6f6e 6020 2860 6465 6661  pression` (`defa
+000019b0: 756c 743d 6e6f 6e65 6029 0a20 202a 2054  ult=none`).  * T
+000019c0: 6865 2063 6f6d 7072 6573 7369 6f6e 2074  he compression t
+000019d0: 7970 6520 746f 2075 7365 2066 6f72 2061  ype to use for a
+000019e0: 6e79 2073 746f 7261 6765 2066 6f72 6d61  ny storage forma
+000019f0: 7420 7468 6174 2061 6c6c 6f77 7320 636f  t that allows co
+00001a00: 6d70 7265 7373 696f 6e20 746f 2062 6520  mpression to be 
+00001a10: 7370 6563 6966 6965 642e 2054 6f20 7365  specified. To se
+00001a20: 6520 7768 6963 6820 6f70 7469 6f6e 7320  e which options 
+00001a30: 6172 6520 6176 6169 6c61 626c 652c 2063  are available, c
+00001a40: 6865 636b 206f 7574 205b 4352 4541 5445  heck out [CREATE
+00001a50: 2054 4142 4c45 2041 535d 5b63 7265 6174   TABLE AS][creat
+00001a60: 652d 7461 626c 652d 6173 5d0a 2a20 6066  e-table-as].* `f
+00001a70: 6965 6c64 5f64 656c 696d 6974 6572 6020  ield_delimiter` 
+00001a80: 2860 6465 6661 756c 743d 6e6f 6e65 6029  (`default=none`)
+00001a90: 0a20 202a 2043 7573 746f 6d20 6669 656c  .  * Custom fiel
+00001aa0: 6420 6465 6c69 6d69 7465 722c 2066 6f72  d delimiter, for
+00001ab0: 2077 6865 6e20 666f 726d 6174 2069 7320   when format is 
+00001ac0: 7365 7420 746f 2060 5445 5854 4649 4c45  set to `TEXTFILE
+00001ad0: 600a 2a20 6074 6162 6c65 5f70 726f 7065  `.* `table_prope
+00001ae0: 7274 6965 7360 3a20 7461 626c 6520 7072  rties`: table pr
+00001af0: 6f70 6572 7469 6573 2074 6f20 6164 6420  operties to add 
+00001b00: 746f 2074 6865 2074 6162 6c65 2c20 7661  to the table, va
+00001b10: 6c69 6420 666f 7220 4963 6562 6572 6720  lid for Iceberg 
+00001b20: 6f6e 6c79 0a2a 2060 6c66 5f74 6167 7360  only.* `lf_tags`
+00001b30: 2028 6064 6566 6175 6c74 3d6e 6f6e 6560   (`default=none`
+00001b40: 290a 2020 2a20 6c66 2074 6167 7320 746f  ).  * lf tags to
+00001b50: 2061 7373 6f63 6961 7465 2077 6974 6820   associate with 
+00001b60: 7468 6520 7461 626c 650a 2020 2a20 666f  the table.  * fo
+00001b70: 726d 6174 3a20 607b 2274 6167 3122 3a20  rmat: `{"tag1": 
+00001b80: 2276 616c 7565 3122 2c20 2274 6167 3222  "value1", "tag2"
+00001b90: 3a20 2276 616c 7565 3222 7d60 0a2a 2060  : "value2"}`.* `
+00001ba0: 6c66 5f74 6167 735f 636f 6c75 6d6e 7360  lf_tags_columns`
+00001bb0: 2028 6064 6566 6175 6c74 3d6e 6f6e 6560   (`default=none`
+00001bc0: 290a 2020 2a20 6c66 2074 6167 7320 746f  ).  * lf tags to
+00001bd0: 2061 7373 6f63 6961 7465 2077 6974 6820   associate with 
+00001be0: 7468 6520 7461 626c 6520 636f 6c75 6d6e  the table column
+00001bf0: 730a 2020 2a20 666f 726d 6174 3a20 607b  s.  * format: `{
+00001c00: 2274 6167 3122 3a20 7b22 7661 6c75 6531  "tag1": {"value1
+00001c10: 223a 205b 2263 6f6c 756d 6e31 223a 2022  ": ["column1": "
+00001c20: 636f 6c75 6d6e 3222 5d7d 7d60 0a0a 2323  column2"]}}`..##
+00001c30: 2320 5461 626c 6520 6c6f 6361 7469 6f6e  # Table location
+00001c40: 0a0a 5468 6520 6c6f 6361 7469 6f6e 2069  ..The location i
+00001c50: 6e20 7768 6963 6820 6120 7461 626c 6520  n which a table 
+00001c60: 6973 2073 6176 6564 2069 7320 6465 7465  is saved is dete
+00001c70: 726d 696e 6564 2062 793a 0a0a 312e 2049  rmined by:..1. I
+00001c80: 6620 6065 7874 6572 6e61 6c5f 6c6f 6361  f `external_loca
+00001c90: 7469 6f6e 6020 6973 2064 6566 696e 6564  tion` is defined
+00001ca0: 2c20 7468 6174 2076 616c 7565 2069 7320  , that value is 
+00001cb0: 7573 6564 2e0a 322e 2049 6620 6073 335f  used..2. If `s3_
+00001cc0: 6461 7461 5f64 6972 6020 6973 2064 6566  data_dir` is def
+00001cd0: 696e 6564 2c20 7468 6520 7061 7468 2069  ined, the path i
+00001ce0: 7320 6465 7465 726d 696e 6564 2062 7920  s determined by 
+00001cf0: 7468 6174 2061 6e64 2060 7333 5f64 6174  that and `s3_dat
+00001d00: 615f 6e61 6d69 6e67 600a 332e 2049 6620  a_naming`.3. If 
+00001d10: 6073 335f 6461 7461 5f64 6972 6020 6973  `s3_data_dir` is
+00001d20: 206e 6f74 2064 6566 696e 6564 2064 6174   not defined dat
+00001d30: 6120 6973 2073 746f 7265 6420 756e 6465  a is stored unde
+00001d40: 7220 6073 335f 7374 6167 696e 675f 6469  r `s3_staging_di
+00001d50: 722f 7461 626c 6573 2f60 0a0a 4865 7265  r/tables/`..Here
+00001d60: 2061 6c6c 2074 6865 206f 7074 696f 6e73   all the options
+00001d70: 2061 7661 696c 6162 6c65 2066 6f72 2060   available for `
+00001d80: 7333 5f64 6174 615f 6e61 6d69 6e67 603a  s3_data_naming`:
+00001d90: 0a2a 2060 7575 6964 603a 2060 7b73 335f  .* `uuid`: `{s3_
+00001da0: 6461 7461 5f64 6972 7d2f 7b75 7569 6434  data_dir}/{uuid4
+00001db0: 2829 7d2f 600a 2a20 6074 6162 6c65 5f74  ()}/`.* `table_t
+00001dc0: 6162 6c65 603a 2060 7b73 335f 6461 7461  able`: `{s3_data
+00001dd0: 5f64 6972 7d2f 7b74 6162 6c65 7d2f 600a  _dir}/{table}/`.
+00001de0: 2a20 6074 6162 6c65 5f75 6e69 7175 6560  * `table_unique`
 00001df0: 3a20 607b 7333 5f64 6174 615f 6469 727d  : `{s3_data_dir}
-00001e00: 2f7b 7461 626c 657d 2f60 0a2a 2060 7461  /{table}/`.* `ta
-00001e10: 626c 655f 756e 6971 7565 603a 2060 7b73  ble_unique`: `{s
-00001e20: 335f 6461 7461 5f64 6972 7d2f 7b74 6162  3_data_dir}/{tab
-00001e30: 6c65 7d2f 7b75 7569 6434 2829 7d2f 600a  le}/{uuid4()}/`.
-00001e40: 2a20 6073 6368 656d 615f 7461 626c 6560  * `schema_table`
-00001e50: 3a20 607b 7333 5f64 6174 615f 6469 727d  : `{s3_data_dir}
-00001e60: 2f7b 7363 6865 6d61 7d2f 7b74 6162 6c65  /{schema}/{table
-00001e70: 7d2f 600a 2a20 6073 335f 6461 7461 5f6e  }/`.* `s3_data_n
-00001e80: 616d 696e 673d 7363 6865 6d61 5f74 6162  aming=schema_tab
-00001e90: 6c65 5f75 6e69 7175 6560 3a20 607b 7333  le_unique`: `{s3
-00001ea0: 5f64 6174 615f 6469 727d 2f7b 7363 6865  _data_dir}/{sche
-00001eb0: 6d61 7d2f 7b74 6162 6c65 7d2f 7b75 7569  ma}/{table}/{uui
-00001ec0: 6434 2829 7d2f 600a 0a49 7427 7320 706f  d4()}/`..It's po
-00001ed0: 7373 6962 6c65 2074 6f20 7365 7420 7468  ssible to set th
-00001ee0: 6520 6073 335f 6461 7461 5f6e 616d 696e  e `s3_data_namin
-00001ef0: 6760 2067 6c6f 6261 6c6c 7920 696e 2074  g` globally in t
-00001f00: 6865 2074 6172 6765 7420 7072 6f66 696c  he target profil
-00001f10: 652c 206f 7220 6f76 6572 7772 6974 6520  e, or overwrite 
-00001f20: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
-00001f30: 2074 6162 6c65 2063 6f6e 6669 672c 0a6f   table config,.o
-00001f40: 7220 7365 7474 696e 6720 7570 2074 6865  r setting up the
-00001f50: 2076 616c 7565 2066 6f72 2067 726f 7570   value for group
-00001f60: 7320 6f66 206d 6f64 656c 2069 6e20 6462  s of model in db
-00001f70: 745f 7072 6f6a 6563 742e 796d 6c2e 0a0a  t_project.yml...
-00001f80: 3e20 4e6f 7465 3a20 7768 656e 2075 7369  > Note: when usi
-00001f90: 6e67 2061 2077 6f72 6b20 6772 6f75 7020  ng a work group 
-00001fa0: 7769 7468 2061 2064 6566 6175 6c74 206f  with a default o
-00001fb0: 7574 7075 7420 6c6f 6361 7469 6f6e 2063  utput location c
-00001fc0: 6f6e 6669 6775 7265 642c 2060 7333 5f64  onfigured, `s3_d
-00001fd0: 6174 615f 6e61 6d69 6e67 6020 616e 6420  ata_naming` and 
-00001fe0: 616e 7920 636f 6e66 6967 7572 6564 2062  any configured b
-00001ff0: 7563 6b65 7473 2061 7265 2069 676e 6f72  uckets are ignor
-00002000: 6564 2061 6e64 2074 6865 206c 6f63 6174  ed and the locat
-00002010: 696f 6e20 636f 6e66 6967 7572 6564 2069  ion configured i
-00002020: 6e20 7468 6520 776f 726b 2067 726f 7570  n the work group
-00002030: 2069 7320 7573 6564 2e0a 0a0a 2323 2323   is used....####
-00002040: 2049 6e63 7265 6d65 6e74 616c 206d 6f64   Incremental mod
-00002050: 656c 730a 0a53 7570 706f 7274 2066 6f72  els..Support for
-00002060: 205b 696e 6372 656d 656e 7461 6c20 6d6f   [incremental mo
-00002070: 6465 6c73 5d28 6874 7470 733a 2f2f 646f  dels](https://do
-00002080: 6373 2e67 6574 6462 742e 636f 6d2f 646f  cs.getdbt.com/do
-00002090: 6373 2f62 7569 6c64 2f69 6e63 7265 6d65  cs/build/increme
-000020a0: 6e74 616c 2d6d 6f64 656c 7329 2e0a 0a54  ntal-models)...T
-000020b0: 6865 7365 2073 7472 6174 6567 6965 7320  hese strategies 
-000020c0: 6172 6520 7375 7070 6f72 7465 643a 0a0a  are supported:..
-000020d0: 2a20 6069 6e73 6572 745f 6f76 6572 7772  * `insert_overwr
-000020e0: 6974 6560 2028 6465 6661 756c 7429 3a20  ite` (default): 
-000020f0: 5468 6520 696e 7365 7274 206f 7665 7277  The insert overw
-00002100: 7269 7465 2073 7472 6174 6567 7920 6465  rite strategy de
-00002110: 6c65 7465 7320 7468 6520 6f76 6572 6c61  letes the overla
-00002120: 7070 696e 6720 7061 7274 6974 696f 6e73  pping partitions
-00002130: 2066 726f 6d20 7468 6520 6465 7374 696e   from the destin
-00002140: 6174 696f 6e0a 7461 626c 652c 2061 6e64  ation.table, and
-00002150: 2074 6865 6e20 696e 7365 7274 7320 7468   then inserts th
-00002160: 6520 6e65 7720 7265 636f 7264 7320 6672  e new records fr
-00002170: 6f6d 2074 6865 2073 6f75 7263 652e 2054  om the source. T
-00002180: 6869 7320 7374 7261 7465 6779 2064 6570  his strategy dep
-00002190: 656e 6473 206f 6e20 7468 6520 6070 6172  ends on the `par
-000021a0: 7469 7469 6f6e 6564 5f62 7960 206b 6579  titioned_by` key
-000021b0: 776f 7264 2120 4966 206e 6f0a 7061 7274  word! If no.part
-000021c0: 6974 696f 6e73 2061 7265 2064 6566 696e  itions are defin
-000021d0: 6564 2c20 6462 7420 7769 6c6c 2066 616c  ed, dbt will fal
-000021e0: 6c20 6261 636b 2074 6f20 7468 6520 6061  l back to the `a
-000021f0: 7070 656e 6460 2073 7472 6174 6567 792e  ppend` strategy.
-00002200: 0a2a 2060 6170 7065 6e64 603a 2049 6e73  .* `append`: Ins
-00002210: 6572 7420 6e65 7720 7265 636f 7264 7320  ert new records 
-00002220: 7769 7468 6f75 7420 7570 6461 7469 6e67  without updating
-00002230: 2c20 6465 6c65 7469 6e67 206f 7220 6f76  , deleting or ov
-00002240: 6572 7772 6974 696e 6720 616e 7920 6578  erwriting any ex
-00002250: 6973 7469 6e67 2064 6174 612e 2054 6865  isting data. The
-00002260: 7265 206d 6967 6874 2062 6520 6475 706c  re might be dupl
-00002270: 6963 6174 650a 6461 7461 2028 652e 672e  icate.data (e.g.
-00002280: 2067 7265 6174 2066 6f72 206c 6f67 206f   great for log o
-00002290: 7220 6869 7374 6f72 6963 616c 2064 6174  r historical dat
-000022a0: 6129 2e0a 2a20 606d 6572 6765 603a 2043  a)..* `merge`: C
-000022b0: 6f6e 6469 7469 6f6e 616c 6c79 2075 7064  onditionally upd
-000022c0: 6174 6573 2c20 6465 6c65 7465 732c 206f  ates, deletes, o
-000022d0: 7220 696e 7365 7274 7320 726f 7773 2069  r inserts rows i
-000022e0: 6e74 6f20 616e 2049 6365 6265 7267 2074  nto an Iceberg t
-000022f0: 6162 6c65 2e20 5573 6564 2069 6e20 636f  able. Used in co
-00002300: 6d62 696e 6174 696f 6e20 7769 7468 2060  mbination with `
-00002310: 756e 6971 7565 5f6b 6579 602e 0a4f 6e6c  unique_key`..Onl
-00002320: 7920 6176 6169 6c61 626c 6520 7768 656e  y available when
-00002330: 2075 7369 6e67 2049 6365 6265 7267 2e0a   using Iceberg..
-00002340: 0a23 2323 2320 4f6e 2073 6368 656d 6120  .#### On schema 
-00002350: 6368 616e 6765 0a0a 606f 6e5f 7363 6865  change..`on_sche
-00002360: 6d61 5f63 6861 6e67 6560 2069 7320 616e  ma_change` is an
-00002370: 206f 7074 696f 6e20 746f 2072 6566 6c65   option to refle
-00002380: 6374 2063 6861 6e67 6573 206f 6620 7363  ct changes of sc
-00002390: 6865 6d61 2069 6e20 696e 6372 656d 656e  hema in incremen
-000023a0: 7461 6c20 6d6f 6465 6c73 2e0a 5468 6520  tal models..The 
-000023b0: 666f 6c6c 6f77 696e 6720 6f70 7469 6f6e  following option
-000023c0: 7320 6172 6520 7375 7070 6f72 7465 643a  s are supported:
-000023d0: 0a2a 2060 6967 6e6f 7265 6020 2864 6566  .* `ignore` (def
-000023e0: 6175 6c74 290a 2a20 6066 6169 6c60 0a2a  ault).* `fail`.*
-000023f0: 2060 6170 7065 6e64 5f6e 6577 5f63 6f6c   `append_new_col
-00002400: 756d 6e73 600a 2a20 6073 796e 635f 616c  umns`.* `sync_al
-00002410: 6c5f 636f 6c75 6d6e 7360 0a0a 496e 2064  l_columns`..In d
-00002420: 6574 6169 6c2c 2070 6c65 6173 6520 7265  etail, please re
-00002430: 6665 7220 746f 205b 6462 7420 646f 6373  fer to [dbt docs
-00002440: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
-00002450: 6574 6462 742e 636f 6d2f 646f 6373 2f62  etdbt.com/docs/b
-00002460: 7569 6c64 2f69 6e63 7265 6d65 6e74 616c  uild/incremental
-00002470: 2d6d 6f64 656c 7323 7768 6174 2d69 662d  -models#what-if-
-00002480: 7468 652d 636f 6c75 6d6e 732d 6f66 2d6d  the-columns-of-m
-00002490: 792d 696e 6372 656d 656e 7461 6c2d 6d6f  y-incremental-mo
-000024a0: 6465 6c2d 6368 616e 6765 292e 0a0a 0a23  del-change)....#
-000024b0: 2323 2320 4963 6562 6572 670a 0a54 6865  ### Iceberg..The
-000024c0: 2061 6461 7074 6572 2073 7570 706f 7274   adapter support
-000024d0: 7320 7461 626c 6520 6d61 7465 7269 616c  s table material
-000024e0: 697a 6174 696f 6e20 666f 7220 4963 6562  ization for Iceb
-000024f0: 6572 672e 0a0a 546f 2067 6574 2073 7461  erg...To get sta
-00002500: 7274 6564 206a 7573 7420 6164 6420 7468  rted just add th
-00002510: 6973 2061 7320 796f 7572 206d 6f64 656c  is as your model
-00002520: 3a0a 6060 600a 7b7b 2063 6f6e 6669 6728  :.```.{{ config(
-00002530: 0a20 2020 206d 6174 6572 6961 6c69 7a65  .    materialize
-00002540: 643d 2774 6162 6c65 272c 0a20 2020 2074  d='table',.    t
-00002550: 6162 6c65 5f74 7970 653d 2769 6365 6265  able_type='icebe
-00002560: 7267 272c 0a20 2020 2066 6f72 6d61 743d  rg',.    format=
-00002570: 2770 6172 7175 6574 272c 0a20 2020 2070  'parquet',.    p
-00002580: 6172 7469 7469 6f6e 6564 5f62 793d 5b27  artitioned_by=['
-00002590: 6275 636b 6574 2875 7365 725f 6964 2c20  bucket(user_id, 
-000025a0: 3529 275d 2c0a 2020 2020 7461 626c 655f  5)'],.    table_
-000025b0: 7072 6f70 6572 7469 6573 3d7b 0a20 2020  properties={.   
-000025c0: 2009 276f 7074 696d 697a 655f 7265 7772   .'optimize_rewr
-000025d0: 6974 655f 6465 6c65 7465 5f66 696c 655f  ite_delete_file_
-000025e0: 7468 7265 7368 6f6c 6427 3a20 2732 270a  threshold': '2'.
-000025f0: 2020 2020 097d 0a29 207d 7d0a 0a53 454c      .}.) }}..SEL
-00002600: 4543 540a 0927 4127 2041 5320 7573 6572  ECT..'A' AS user
-00002610: 5f69 642c 0a09 2770 6927 2041 5320 6e61  _id,..'pi' AS na
-00002620: 6d65 2c0a 0927 6163 7469 7665 2720 4153  me,..'active' AS
-00002630: 2073 7461 7475 732c 0a09 3137 2e38 3920   status,..17.89 
-00002640: 4153 2063 6f73 742c 0a09 3120 4153 2071  AS cost,..1 AS q
-00002650: 7561 6e74 6974 792c 0a09 3130 3030 3030  uantity,..100000
-00002660: 3030 3020 4153 2071 7561 6e74 6974 795f  000 AS quantity_
-00002670: 6269 672c 0a09 6375 7272 656e 745f 6461  big,..current_da
-00002680: 7465 2041 5320 6d79 5f64 6174 650a 6060  te AS my_date.``
-00002690: 600a 0a49 6365 6265 7267 2073 7570 706f  `..Iceberg suppo
-000026a0: 7274 7320 6275 636b 6574 696e 6720 6173  rts bucketing as
-000026b0: 2068 6964 6465 6e20 7061 7274 6974 696f   hidden partitio
-000026c0: 6e73 2c20 7468 6572 6566 6f72 6520 7573  ns, therefore us
-000026d0: 6520 7468 6520 6070 6172 7469 7469 6f6e  e the `partition
-000026e0: 6564 5f62 7960 2063 6f6e 6669 6720 746f  ed_by` config to
-000026f0: 2061 6464 2073 7065 6369 6669 6320 6275   add specific bu
-00002700: 636b 6574 696e 6720 636f 6e64 6974 696f  cketing conditio
-00002710: 6e73 2e0a 0a49 6365 6265 7267 2073 7570  ns...Iceberg sup
-00002720: 706f 7274 7320 7365 7665 7261 6c20 7461  ports several ta
-00002730: 626c 6520 666f 726d 6174 7320 666f 7220  ble formats for 
-00002740: 6461 7461 203a 2060 5041 5251 5545 5460  data : `PARQUET`
-00002750: 2c20 6041 5652 4f60 2061 6e64 2060 4f52  , `AVRO` and `OR
-00002760: 4360 2e0a 0a49 7420 6973 2070 6f73 7369  C`...It is possi
-00002770: 626c 6520 746f 2075 7365 2069 6365 6265  ble to use icebe
-00002780: 7267 2069 6e20 616e 2069 6e63 7265 6d65  rg in an increme
-00002790: 6e74 616c 2066 6173 6869 6f6e 2c20 7370  ntal fashion, sp
-000027a0: 6563 6966 6963 616c 6c79 2032 2073 7472  ecifically 2 str
-000027b0: 6174 6567 6965 7320 6172 6520 7375 7070  ategies are supp
-000027c0: 6f72 7465 643a 0a2a 2060 6170 7065 6e64  orted:.* `append
-000027d0: 603a 206e 6577 2072 6563 6f72 6473 2061  `: new records a
-000027e0: 7265 2061 7070 656e 6465 6420 746f 2074  re appended to t
-000027f0: 6865 2074 6162 6c65 2c20 7468 6973 2063  he table, this c
-00002800: 616e 206c 6561 6420 746f 2064 7570 6c69  an lead to dupli
-00002810: 6361 7465 730a 2a20 606d 6572 6765 603a  cates.* `merge`:
-00002820: 206d 7573 7420 6265 2075 7365 6420 696e   must be used in
-00002830: 2063 6f6d 6269 6e61 7469 6f6e 2077 6974   combination wit
-00002840: 6820 6075 6e69 7175 655f 6b65 7960 2061  h `unique_key` a
-00002850: 6e64 2069 7427 7320 6f6e 6c79 2061 7661  nd it's only ava
-00002860: 696c 6162 6c65 2077 6974 6820 456e 6769  ilable with Engi
-00002870: 6e65 2076 6572 7369 6f6e 2033 2e0a 2020  ne version 3..  
-00002880: 2049 7420 7065 7266 6f72 6d73 2061 6e20   It performs an 
-00002890: 7570 7365 7274 2c20 6e65 7720 7265 636f  upsert, new reco
-000028a0: 7264 2061 7265 2061 6464 6564 2c20 616e  rd are added, an
-000028b0: 6420 7265 636f 7264 2061 6c72 6561 6479  d record already
-000028c0: 2065 7869 7374 696e 6720 6172 6520 7570   existing are up
-000028d0: 6461 7465 640a 0a23 2323 2320 4869 6768  dated..#### High
-000028e0: 2061 7661 696c 6162 6c65 2074 6162 6c65   available table
-000028f0: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-00002900: 0a54 6865 2063 7572 7265 6e74 2069 6d70  .The current imp
-00002910: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
-00002920: 6865 2074 6162 6c65 206d 6174 6572 6961  he table materia
-00002930: 6c69 7a61 7469 6f6e 2063 616e 206c 6561  lization can lea
-00002940: 6420 746f 2064 6f77 6e74 696d 652c 2061  d to downtime, a
-00002950: 7320 7461 7267 6574 2074 6162 6c65 2069  s target table i
-00002960: 7320 6472 6f70 7065 6420 616e 6420 7265  s dropped and re
-00002970: 2d63 7265 6174 6564 2e0a 546f 2068 6176  -created..To hav
-00002980: 6520 7468 6520 6c65 7373 2064 6573 7472  e the less destr
-00002990: 7563 7469 7665 2062 6568 6176 696f 7220  uctive behavior 
-000029a0: 6974 2773 2070 6f73 7369 626c 6520 746f  it's possible to
-000029b0: 2075 7365 2060 7461 626c 653d 2774 6162   use `table='tab
-000029c0: 6c65 5f68 6976 655f 6861 2760 206d 6174  le_hive_ha'` mat
-000029d0: 6572 6961 6c69 7a61 7469 6f6e 2e0a 2a2a  erialization..**
-000029e0: 7461 626c 655f 6869 7665 5f68 612a 2a20  table_hive_ha** 
-000029f0: 6c65 7665 7261 6765 2074 6865 2074 6162  leverage the tab
-00002a00: 6c65 2076 6572 7369 6f6e 7320 6665 6174  le versions feat
-00002a10: 7572 6520 6f66 2067 6c75 6520 6361 7461  ure of glue cata
-00002a20: 6c6f 672c 2063 7265 6174 696e 6720 6120  log, creating a 
-00002a30: 746d 7020 7461 626c 6520 616e 6420 7377  tmp table and sw
-00002a40: 6170 7069 6e67 0a74 6865 2074 6172 6765  apping.the targe
-00002a50: 7420 7461 626c 6520 746f 2074 6865 206c  t table to the l
-00002a60: 6f63 6174 696f 6e20 6f66 2074 6865 2074  ocation of the t
-00002a70: 6d70 2074 6162 6c65 2e0a 5468 6973 206d  mp table..This m
-00002a80: 6174 6572 6961 6c69 7a61 7469 6f6e 2069  aterialization i
-00002a90: 7320 6f6e 6c79 2061 7661 696c 6162 6c65  s only available
-00002aa0: 2066 6f72 2060 7461 626c 655f 7479 7065   for `table_type
-00002ab0: 3d68 6976 6560 2061 6e64 2072 6571 7569  =hive` and requi
-00002ac0: 7265 7320 7573 696e 6720 756e 6971 7565  res using unique
-00002ad0: 206c 6f63 6174 696f 6e73 2e0a 0a60 6060   locations...```
-00002ae0: 0a7b 7b20 636f 6e66 6967 280a 2020 2020  .{{ config(.    
-00002af0: 6d61 7465 7269 616c 697a 6564 3d27 7461  materialized='ta
-00002b00: 626c 655f 6869 7665 5f68 6127 2c0a 2020  ble_hive_ha',.  
-00002b10: 2020 666f 726d 6174 3d27 7061 7271 7565    format='parque
-00002b20: 7427 2c0a 2020 2020 7061 7274 6974 696f  t',.    partitio
-00002b30: 6e5f 6279 3d5b 2773 7461 7475 7327 5d2c  n_by=['status'],
-00002b40: 0a20 2020 2073 335f 6461 7461 5f6e 616d  .    s3_data_nam
-00002b50: 696e 673d 2774 6162 6c65 5f75 6e69 7175  ing='table_uniqu
-00002b60: 6527 0a29 207d 7d0a 0a0a 7365 6c65 6374  e'.) }}...select
-00002b70: 0a20 2027 6127 2061 7320 7573 6572 5f69  .  'a' as user_i
-00002b80: 642c 0a20 2027 7069 2720 6173 2075 7365  d,.  'pi' as use
-00002b90: 725f 6e61 6d65 2c0a 2020 2761 6374 6976  r_name,.  'activ
-00002ba0: 6527 2061 7320 7374 6174 7573 0a75 6e69  e' as status.uni
-00002bb0: 6f6e 2061 6c6c 0a73 656c 6563 740a 2020  on all.select.  
-00002bc0: 2762 2720 6173 2075 7365 725f 6964 2c0a  'b' as user_id,.
-00002bd0: 2020 2773 6827 2061 7320 7573 6572 5f6e    'sh' as user_n
-00002be0: 616d 652c 0a20 2027 6469 7361 626c 6564  ame,.  'disabled
-00002bf0: 2720 6173 2073 7461 7475 730a 6060 600a  ' as status.```.
-00002c00: 0a42 7920 6465 6661 756c 742c 2074 6865  .By default, the
-00002c10: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-00002c20: 206b 6565 7073 2074 6865 206c 6173 7420   keeps the last 
-00002c30: 3420 7461 626c 6520 7665 7273 696f 6e73  4 table versions
-00002c40: 2c20 796f 7520 6361 6e20 6368 616e 6765  , you can change
-00002c50: 2069 7420 7468 6174 2073 6574 7469 6e67   it that setting
-00002c60: 2060 7665 7273 696f 6e73 5f74 6f5f 6b65   `versions_to_ke
-00002c70: 6570 602e 0a0a 2323 2323 2320 4b6e 6f77  ep`...##### Know
-00002c80: 6e20 6973 7375 6573 0a2a 2057 6865 6e20  n issues.* When 
-00002c90: 7377 6170 7069 6e67 2066 726f 6d20 6120  swapping from a 
-00002ca0: 7461 626c 6520 7769 7468 2070 6172 7469  table with parti
-00002cb0: 7469 6f6e 7320 746f 2061 2074 6162 6c65  tions to a table
-00002cc0: 2077 6974 686f 7574 2028 616e 6420 7468   without (and th
-00002cd0: 6520 6f74 6865 7220 7761 7920 6172 6f75  e other way arou
-00002ce0: 6e64 292c 2074 6865 7265 2063 6f75 6c64  nd), there could
-00002cf0: 2062 6520 6120 6c69 7474 6c65 2064 6f77   be a little dow
-00002d00: 6e74 696d 652e 0a20 2049 6e20 6361 7365  ntime..  In case
-00002d10: 2068 6967 6820 7065 7266 6f72 6d61 6e63   high performanc
-00002d20: 6573 2061 7265 206e 6565 6465 6420 636f  es are needed co
-00002d30: 6e73 6964 6572 2062 7563 6b65 7469 6e67  nsider bucketing
-00002d40: 2069 6e73 7465 6164 206f 6620 7061 7274   instead of part
-00002d50: 6974 696f 6e73 0a2a 2042 7920 6465 6661  itions.* By defa
-00002d60: 756c 742c 2047 6c75 6520 2264 7570 6c69  ult, Glue "dupli
-00002d70: 6361 7465 2220 7468 6520 7665 7273 696f  cate" the versio
-00002d80: 6e73 2069 6e74 6572 6e61 6c6c 792c 2073  ns internally, s
-00002d90: 6f20 7468 6520 6c61 7374 2032 2076 6572  o the last 2 ver
-00002da0: 7369 6f6e 7320 6f66 2061 2074 6162 6c65  sions of a table
-00002db0: 2070 6f69 6e74 2074 6f20 7468 6520 7361   point to the sa
-00002dc0: 6d65 206c 6f63 6174 696f 6e0a 2a20 4974  me location.* It
-00002dd0: 2773 2072 6563 6f6d 6d65 6e64 6564 2074  's recommended t
-00002de0: 6f20 6861 7665 2076 6572 7369 6f6e 735f  o have versions_
-00002df0: 746f 5f6b 6565 703e 3d20 342c 2061 7320  to_keep>= 4, as 
-00002e00: 7468 6973 2077 696c 6c20 6176 6f69 6420  this will avoid 
-00002e10: 746f 2068 6176 6520 7468 6520 6f6c 6465  to have the olde
-00002e20: 7220 6c6f 6361 7469 6f6e 2072 656d 6f76  r location remov
-00002e30: 6564 0a2a 2054 6865 206d 6163 726f 2061  ed.* The macro a
-00002e40: 7468 656e 615f 5f65 6e64 5f6f 665f 7469  thena__end_of_ti
-00002e50: 6d65 206e 6565 6473 2074 6f20 6265 206f  me needs to be o
-00002e60: 7665 7277 7269 7474 656e 2062 7920 7468  verwritten by th
-00002e70: 6520 7573 6572 2069 6620 7573 696e 6720  e user if using 
-00002e80: 4174 6865 6e61 2076 3320 7369 6e63 6520  Athena v3 since 
-00002e90: 6974 2072 6571 7569 7265 7320 6120 7072  it requires a pr
-00002ea0: 6563 6973 696f 6e20 7061 7261 6d65 7465  ecision paramete
-00002eb0: 7220 666f 7220 7469 6d65 7374 616d 7073  r for timestamps
-00002ec0: 0a0a 0a23 2323 2053 6e61 7073 686f 7473  ...### Snapshots
-00002ed0: 0a0a 5468 6520 6164 6170 7465 7220 7375  ..The adapter su
-00002ee0: 7070 6f72 7473 2073 6e61 7073 686f 7420  pports snapshot 
-00002ef0: 6d61 7465 7269 616c 697a 6174 696f 6e2e  materialization.
-00002f00: 2049 7420 7375 7070 6f72 7473 2062 6f74   It supports bot
-00002f10: 6820 7469 6d65 7374 616d 7020 616e 6420  h timestamp and 
-00002f20: 6368 6563 6b20 7374 7261 7465 6779 2e20  check strategy. 
-00002f30: 546f 2063 7265 6174 6520 6120 736e 6170  To create a snap
-00002f40: 7368 6f74 2063 7265 6174 6520 6120 736e  shot create a sn
-00002f50: 6170 7368 6f74 2066 696c 6520 696e 2074  apshot file in t
-00002f60: 6865 2073 6e61 7073 686f 7473 2064 6972  he snapshots dir
-00002f70: 6563 746f 7279 2e20 4966 2064 6972 6563  ectory. If direc
-00002f80: 746f 7279 2064 6f65 7320 6e6f 7420 6578  tory does not ex
-00002f90: 6973 7420 6372 6561 7465 206f 6e65 2e0a  ist create one..
-00002fa0: 0a23 2323 2320 5469 6d65 7374 616d 7020  .#### Timestamp 
-00002fb0: 7374 7261 7465 6779 0a0a 546f 2075 7365  strategy..To use
-00002fc0: 2074 6865 2074 696d 6573 7461 6d70 2073   the timestamp s
-00002fd0: 7472 6174 6567 7920 7265 6665 7220 746f  trategy refer to
-00002fe0: 2074 6865 205b 6462 7420 646f 6373 5d28   the [dbt docs](
-00002ff0: 6874 7470 733a 2f2f 646f 6373 2e67 6574  https://docs.get
-00003000: 6462 742e 636f 6d2f 646f 6373 2f62 7569  dbt.com/docs/bui
-00003010: 6c64 2f73 6e61 7073 686f 7473 2374 696d  ld/snapshots#tim
-00003020: 6573 7461 6d70 2d73 7472 6174 6567 792d  estamp-strategy-
-00003030: 7265 636f 6d6d 656e 6465 6429 0a0a 2323  recommended)..##
-00003040: 2323 2043 6865 636b 2073 7472 6174 6567  ## Check strateg
-00003050: 790a 0a54 6f20 7573 6520 7468 6520 6368  y..To use the ch
-00003060: 6563 6b20 7374 7261 7465 6779 2072 6566  eck strategy ref
-00003070: 6572 2074 6f20 7468 6520 5b64 6274 2064  er to the [dbt d
-00003080: 6f63 735d 2868 7474 7073 3a2f 2f64 6f63  ocs](https://doc
-00003090: 732e 6765 7464 6274 2e63 6f6d 2f64 6f63  s.getdbt.com/doc
-000030a0: 732f 6275 696c 642f 736e 6170 7368 6f74  s/build/snapshot
-000030b0: 7323 6368 6563 6b2d 7374 7261 7465 6779  s#check-strategy
-000030c0: 290a 0a23 2323 2320 4861 7264 2d64 656c  )..#### Hard-del
-000030d0: 6574 6573 0a0a 5468 6520 6d61 7465 7269  etes..The materi
-000030e0: 616c 697a 6174 696f 6e20 616c 736f 2073  alization also s
-000030f0: 7570 706f 7274 7320 696e 7661 6c69 6461  upports invalida
-00003100: 7469 6e67 2068 6172 6420 6465 6c65 7465  ting hard delete
-00003110: 732e 2043 6865 636b 2074 6865 205b 646f  s. Check the [do
-00003120: 6373 5d28 6874 7470 733a 2f2f 646f 6373  cs](https://docs
-00003130: 2e67 6574 6462 742e 636f 6d2f 646f 6373  .getdbt.com/docs
-00003140: 2f62 7569 6c64 2f73 6e61 7073 686f 7473  /build/snapshots
-00003150: 2368 6172 642d 6465 6c65 7465 732d 6f70  #hard-deletes-op
-00003160: 742d 696e 2920 746f 2075 6e64 6572 7374  t-in) to underst
-00003170: 616e 6420 7573 6167 652e 0a0a 2323 2320  and usage...### 
-00003180: 576f 726b 696e 6720 6578 616d 706c 650a  Working example.
-00003190: 0a73 6565 6420 6669 6c65 202d 2065 6d70  .seed file - emp
-000031a0: 6c6f 7965 6e74 5f69 6e64 6963 6174 6f72  loyent_indicator
-000031b0: 735f 6e6f 7665 6d62 6572 5f32 3032 325f  s_november_2022_
-000031c0: 6373 765f 7461 626c 6573 2e63 7376 0a60  csv_tables.csv.`
-000031d0: 6060 0a53 6572 6965 735f 7265 6665 7265  ``.Series_refere
-000031e0: 6e63 652c 5065 7269 6f64 2c44 6174 615f  nce,Period,Data_
-000031f0: 7661 6c75 652c 5375 7070 7265 7373 6564  value,Suppressed
-00003200: 0a4d 4549 4d2e 5331 5741 2c31 3939 392e  .MEIM.S1WA,1999.
-00003210: 3034 2c38 3032 3637 2c0a 4d45 494d 2e53  04,80267,.MEIM.S
-00003220: 3157 412c 3139 3939 2e30 352c 3730 3830  1WA,1999.05,7080
-00003230: 332c 0a4d 4549 4d2e 5331 5741 2c31 3939  3,.MEIM.S1WA,199
-00003240: 392e 3036 2c36 3537 3932 2c0a 4d45 494d  9.06,65792,.MEIM
-00003250: 2e53 3157 412c 3139 3939 2e30 372c 3636  .S1WA,1999.07,66
-00003260: 3139 342c 0a4d 4549 4d2e 5331 5741 2c31  194,.MEIM.S1WA,1
-00003270: 3939 392e 3038 2c36 3732 3539 2c0a 4d45  999.08,67259,.ME
-00003280: 494d 2e53 3157 412c 3139 3939 2e30 392c  IM.S1WA,1999.09,
-00003290: 3639 3639 312c 0a4d 4549 4d2e 5331 5741  69691,.MEIM.S1WA
-000032a0: 2c31 3939 392e 312c 3732 3437 352c 0a4d  ,1999.1,72475,.M
-000032b0: 4549 4d2e 5331 5741 2c31 3939 392e 3131  EIM.S1WA,1999.11
-000032c0: 2c37 3932 3633 2c0a 4d45 494d 2e53 3157  ,79263,.MEIM.S1W
-000032d0: 412c 3139 3939 2e31 322c 3836 3534 302c  A,1999.12,86540,
-000032e0: 0a4d 4549 4d2e 5331 5741 2c32 3030 302e  .MEIM.S1WA,2000.
-000032f0: 3031 2c38 3235 3532 2c0a 4d45 494d 2e53  01,82552,.MEIM.S
-00003300: 3157 412c 3230 3030 2e30 322c 3831 3730  1WA,2000.02,8170
-00003310: 392c 0a4d 4549 4d2e 5331 5741 2c32 3030  9,.MEIM.S1WA,200
-00003320: 302e 3033 2c38 3431 3236 2c0a 4d45 494d  0.03,84126,.MEIM
-00003330: 2e53 3157 412c 3230 3030 2e30 342c 3737  .S1WA,2000.04,77
-00003340: 3038 392c 0a4d 4549 4d2e 5331 5741 2c32  089,.MEIM.S1WA,2
-00003350: 3030 302e 3035 2c37 3338 3131 2c0a 4d45  000.05,73811,.ME
-00003360: 494d 2e53 3157 412c 3230 3030 2e30 362c  IM.S1WA,2000.06,
-00003370: 3730 3037 302c 0a4d 4549 4d2e 5331 5741  70070,.MEIM.S1WA
-00003380: 2c32 3030 302e 3037 2c36 3938 3733 2c0a  ,2000.07,69873,.
-00003390: 4d45 494d 2e53 3157 412c 3230 3030 2e30  MEIM.S1WA,2000.0
-000033a0: 382c 3731 3436 382c 0a4d 4549 4d2e 5331  8,71468,.MEIM.S1
-000033b0: 5741 2c32 3030 302e 3039 2c37 3234 3632  WA,2000.09,72462
-000033c0: 2c0a 4d45 494d 2e53 3157 412c 3230 3030  ,.MEIM.S1WA,2000
-000033d0: 2e31 2c37 3438 3937 2c0a 6060 600a 0a6d  .1,74897,.```..m
-000033e0: 6f64 656c 2e73 716c 0a60 6060 0a7b 7b20  odel.sql.```.{{ 
-000033f0: 636f 6e66 6967 280a 2020 2020 6d61 7465  config(.    mate
-00003400: 7269 616c 697a 6564 3d27 7461 626c 6527  rialized='table'
-00003410: 0a29 207d 7d0a 0a0a 5345 4c45 4354 0a20  .) }}...SELECT. 
-00003420: 2020 2052 4f57 5f4e 554d 4245 5228 2920     ROW_NUMBER() 
-00003430: 4f56 4552 2028 2920 4153 2069 640a 2020  OVER () AS id.  
-00003440: 2020 2c20 2a0a 2020 2020 2c20 6361 7374    , *.    , cast
-00003450: 2866 726f 6d5f 756e 6978 7469 6d65 2874  (from_unixtime(t
-00003460: 6f5f 756e 6978 7469 6d65 286e 6f77 2829  o_unixtime(now()
-00003470: 2929 2061 7320 7469 6d65 7374 616d 7028  )) as timestamp(
-00003480: 3629 2920 4153 2072 6566 7265 7368 5f74  6)) AS refresh_t
-00003490: 696d 6573 7461 6d70 0a46 524f 4d20 7b7b  imestamp.FROM {{
-000034a0: 2072 6566 2827 656d 706c 6f79 6d65 6e74   ref('employment
-000034b0: 5f69 6e64 6963 6174 6f72 735f 6e6f 7665  _indicators_nove
-000034c0: 6d62 6572 5f32 3032 325f 6373 765f 7461  mber_2022_csv_ta
-000034d0: 626c 6573 2729 207d 7d0a 6060 600a 0a74  bles') }}.```..t
-000034e0: 696d 6573 7461 6d70 2073 7472 6174 6567  imestamp strateg
-000034f0: 7920 2d20 6d6f 6465 6c5f 736e 6170 7368  y - model_snapsh
-00003500: 6f74 5f31 0a0a 6060 600a 7b25 2073 6e61  ot_1..```.{% sna
-00003510: 7073 686f 7420 6d6f 6465 6c5f 736e 6170  pshot model_snap
-00003520: 7368 6f74 5f31 2025 7d0a 0a7b 7b0a 2020  shot_1 %}..{{.  
-00003530: 2020 636f 6e66 6967 280a 2020 2020 2020    config(.      
-00003540: 7374 7261 7465 6779 3d27 7469 6d65 7374  strategy='timest
-00003550: 616d 7027 2c0a 2020 2020 2020 7570 6461  amp',.      upda
-00003560: 7465 645f 6174 3d27 7265 6672 6573 685f  ted_at='refresh_
-00003570: 7469 6d65 7374 616d 7027 2c0a 2020 2020  timestamp',.    
-00003580: 2020 756e 6971 7565 5f6b 6579 3d27 6964    unique_key='id
-00003590: 270a 2020 2020 290a 7d7d 0a0a 0a0a 5345  '.    ).}}....SE
-000035a0: 4c45 4354 202a 0a0a 6672 6f6d 207b 7b20  LECT *..from {{ 
-000035b0: 7265 6628 276d 6f64 656c 2729 207d 7d0a  ref('model') }}.
-000035c0: 0a7b 2520 656e 6473 6e61 7073 686f 7420  .{% endsnapshot 
-000035d0: 257d 0a60 6060 0a0a 696e 7661 6c69 6461  %}.```..invalida
-000035e0: 7465 2068 6172 6420 6465 6c65 7465 7320  te hard deletes 
-000035f0: 2d20 6d6f 6465 6c5f 736e 6170 7368 6f74  - model_snapshot
-00003600: 5f32 0a60 6060 0a7b 2520 736e 6170 7368  _2.```.{% snapsh
-00003610: 6f74 206d 6f64 656c 5f73 6e61 7073 686f  ot model_snapsho
-00003620: 745f 3220 257d 0a0a 7b7b 0a20 2020 2063  t_2 %}..{{.    c
-00003630: 6f6e 6669 670a 2020 2020 280a 2020 2020  onfig.    (.    
-00003640: 2020 2020 756e 6971 7565 5f6b 6579 3d27      unique_key='
-00003650: 6964 272c 0a20 2020 2020 2020 2073 7472  id',.        str
-00003660: 6174 6567 793d 2774 696d 6573 7461 6d70  ategy='timestamp
-00003670: 272c 0a20 2020 2020 2020 2075 7064 6174  ',.        updat
-00003680: 6564 5f61 743d 2772 6566 7265 7368 5f74  ed_at='refresh_t
-00003690: 696d 6573 7461 6d70 272c 0a20 2020 2020  imestamp',.     
-000036a0: 2020 2069 6e76 616c 6964 6174 655f 6861     invalidate_ha
-000036b0: 7264 5f64 656c 6574 6573 3d54 7275 652c  rd_deletes=True,
-000036c0: 0a20 2020 2029 0a7d 7d0a 5345 4c45 4354  .    ).}}.SELECT
-000036d0: 202a 2066 726f 6d20 7b7b 2072 6566 2827   * from {{ ref('
-000036e0: 6d6f 6465 6c27 2920 7d7d 0a0a 7b25 2065  model') }}..{% e
-000036f0: 6e64 736e 6170 7368 6f74 2025 7d0a 6060  ndsnapshot %}.``
-00003700: 600a 0a63 6865 636b 2073 7472 6174 6567  `..check strateg
-00003710: 7920 2d20 6d6f 6465 6c5f 736e 6170 7368  y - model_snapsh
-00003720: 6f74 5f33 0a60 6060 0a7b 2520 736e 6170  ot_3.```.{% snap
-00003730: 7368 6f74 206d 6f64 656c 5f73 6e61 7073  shot model_snaps
-00003740: 686f 745f 3320 257d 0a0a 7b7b 0a20 2020  hot_3 %}..{{.   
-00003750: 2063 6f6e 6669 670a 2020 2020 280a 2020   config.    (.  
-00003760: 2020 2020 2020 756e 6971 7565 5f6b 6579        unique_key
-00003770: 3d27 6964 272c 0a20 2020 2020 2020 2073  ='id',.        s
-00003780: 7472 6174 6567 793d 2763 6865 636b 272c  trategy='check',
-00003790: 0a20 2020 2020 2020 2063 6865 636b 5f63  .        check_c
-000037a0: 6f6c 733d 5b27 7365 7269 6573 5f72 6566  ols=['series_ref
-000037b0: 6572 656e 6365 272c 2764 6174 615f 7661  erence','data_va
-000037c0: 6c75 6527 5d0a 2020 2020 290a 7d7d 0a53  lue'].    ).}}.S
-000037d0: 454c 4543 5420 2a20 6672 6f6d 207b 7b20  ELECT * from {{ 
-000037e0: 7265 6628 276d 6f64 656c 2729 207d 7d0a  ref('model') }}.
-000037f0: 0a7b 2520 656e 6473 6e61 7073 686f 7420  .{% endsnapshot 
-00003800: 257d 0a60 6060 0a0a 2323 2320 4b6e 6f77  %}.```..### Know
-00003810: 6e20 6973 7375 6573 0a0a 2a20 496e 6372  n issues..* Incr
-00003820: 656d 656e 7461 6c20 4963 6562 6572 6720  emental Iceberg 
-00003830: 6d6f 6465 6c73 202d 2053 796e 6320 616c  models - Sync al
-00003840: 6c20 636f 6c75 6d6e 7320 6f6e 2073 6368  l columns on sch
-00003850: 656d 6120 6368 616e 6765 2063 616e 2774  ema change can't
-00003860: 2072 656d 6f76 6520 636f 6c75 6d6e 7320   remove columns 
-00003870: 7573 6564 2061 7320 7061 7274 6974 696f  used as partitio
-00003880: 6e69 6e67 2e0a 5468 6520 6f6e 6c79 2077  ning..The only w
-00003890: 6179 2c20 6672 6f6d 2061 2064 6274 2070  ay, from a dbt p
-000038a0: 6572 7370 6563 7469 7665 2c20 6973 2074  erspective, is t
-000038b0: 6f20 646f 2061 2066 756c 6c2d 7265 6672  o do a full-refr
-000038c0: 6573 6820 6f66 2074 6865 2069 6e63 7265  esh of the incre
-000038d0: 6d65 6e74 616c 206d 6f64 656c 2e0a 0a2a  mental model...*
-000038e0: 2054 6162 6c65 732c 2073 6368 656d 6173   Tables, schemas
-000038f0: 2061 6e64 2064 6174 6162 6173 6520 7368   and database sh
-00003900: 6f75 6c64 206f 6e6c 7920 6265 206c 6f77  ould only be low
-00003910: 6572 6361 7365 0a0a 2a20 496e 206f 7264  ercase..* In ord
-00003920: 6572 2074 6f20 6176 6f69 6420 706f 7465  er to avoid pote
-00003930: 6e74 6961 6c20 636f 6e66 6c69 6374 732c  ntial conflicts,
-00003940: 206d 616b 6520 7375 7265 205b 6064 6274   make sure [`dbt
-00003950: 2d61 7468 656e 612d 6164 6170 7465 7260  -athena-adapter`
-00003960: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003970: 2e63 6f6d 2f54 6f6d 6d65 2f64 6274 2d61  .com/Tomme/dbt-a
-00003980: 7468 656e 6129 2069 7320 6e6f 7420 696e  thena) is not in
-00003990: 7374 616c 6c65 6420 696e 2074 6865 2074  stalled in the t
-000039a0: 6172 6765 7420 656e 7669 726f 6e6d 656e  arget environmen
-000039b0: 742e 0a20 2053 6565 2068 7474 7073 3a2f  t..  See https:/
-000039c0: 2f67 6974 6875 622e 636f 6d2f 6462 742d  /github.com/dbt-
-000039d0: 6174 6865 6e61 2f64 6274 2d61 7468 656e  athena/dbt-athen
-000039e0: 612f 6973 7375 6573 2f31 3033 2066 6f72  a/issues/103 for
-000039f0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-00003a00: 2a20 536e 6170 7368 6f74 2064 6f65 7320  * Snapshot does 
-00003a10: 6e6f 7420 7375 7070 6f72 7420 6472 6f70  not support drop
-00003a20: 7069 6e67 2063 6f6c 756d 6e73 2066 726f  ping columns fro
-00003a30: 6d20 7468 6520 736f 7572 6365 2074 6162  m the source tab
-00003a40: 6c65 2e20 4966 2079 6f75 2064 726f 7020  le. If you drop 
-00003a50: 6120 636f 6c75 6d6e 206d 616b 6520 7375  a column make su
-00003a60: 7265 2074 6f20 6472 6f70 2074 6865 2063  re to drop the c
-00003a70: 6f6c 756d 6e20 6672 6f6d 2074 6865 2073  olumn from the s
-00003a80: 6e61 7073 686f 7420 6173 2077 656c 6c2e  napshot as well.
-00003a90: 2041 6e6f 7468 6572 2077 6f72 6b61 726f   Another workaro
-00003aa0: 756e 6420 6973 2074 6f20 4e55 4c4c 2074  und is to NULL t
-00003ab0: 6865 2063 6f6c 756d 6e20 696e 2074 6865  he column in the
-00003ac0: 2073 6e61 7073 686f 7420 6465 6669 6e69   snapshot defini
-00003ad0: 7469 6f6e 2074 6f20 7072 6573 6572 7665  tion to preserve
-00003ae0: 2068 6973 746f 7279 0a0a 2323 2320 436f   history..### Co
-00003af0: 6e74 7269 6275 7469 6e67 0a0a 5468 6973  ntributing..This
-00003b00: 2063 6f6e 6e65 6374 6f72 2077 6f72 6b73   connector works
-00003b10: 2077 6974 6820 5079 7468 6f6e 2066 726f   with Python fro
-00003b20: 6d20 332e 3720 746f 2033 2e31 312e 0a0a  m 3.7 to 3.11...
-00003b30: 2323 2323 2047 6574 7469 6e67 2073 7461  #### Getting sta
-00003b40: 7274 6564 0a0a 496e 206f 7264 6572 2074  rted..In order t
-00003b50: 6f20 7374 6172 7420 6465 7665 6c6f 7069  o start developi
-00003b60: 6e67 206f 6e20 7468 6973 2061 6461 7074  ng on this adapt
-00003b70: 6572 2063 6c6f 6e65 2074 6865 2072 6570  er clone the rep
-00003b80: 6f20 616e 6420 7275 6e20 7468 6973 206d  o and run this m
-00003b90: 616b 6520 636f 6d6d 616e 6420 2873 6565  ake command (see
-00003ba0: 205b 4d61 6b65 6669 6c65 5d28 4d61 6b65   [Makefile](Make
-00003bb0: 6669 6c65 2929 203a 0a0a 6060 6062 6173  file)) :..```bas
-00003bc0: 680a 6d61 6b65 2073 6574 7570 0a60 6060  h.make setup.```
-00003bd0: 0a0a 4974 2077 696c 6c20 3a0a 312e 2049  ..It will :.1. I
-00003be0: 6e73 7461 6c6c 2061 6c6c 2064 6570 656e  nstall all depen
-00003bf0: 6465 6e63 6965 732e 0a32 2e20 496e 7374  dencies..2. Inst
-00003c00: 616c 6c20 7072 652d 636f 6d6d 6974 2068  all pre-commit h
-00003c10: 6f6f 6b73 2e0a 332e 2047 656e 6572 6174  ooks..3. Generat
-00003c20: 6520 796f 7572 2060 2e65 6e76 6020 6669  e your `.env` fi
-00003c30: 6c65 0a0a 4e65 7874 2c20 6164 6a75 7374  le..Next, adjust
-00003c40: 2060 2e65 6e76 6020 6669 6c65 2062 7920   `.env` file by 
-00003c50: 636f 6e66 6967 7572 696e 6720 7468 6520  configuring the 
-00003c60: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00003c70: 6162 6c65 7320 746f 206d 6174 6368 2079  ables to match y
-00003c80: 6f75 7220 4174 6865 6e61 2064 6576 656c  our Athena devel
-00003c90: 6f70 6d65 6e74 2065 6e76 6972 6f6e 6d65  opment environme
-00003ca0: 6e74 2e0a 0a23 2323 2320 5275 6e6e 696e  nt...#### Runnin
-00003cb0: 6720 7465 7374 730a 0a57 6520 6861 7665  g tests..We have
-00003cc0: 2032 2064 6966 6665 7265 6e74 2074 7970   2 different typ
-00003cd0: 6573 206f 6620 7465 7374 696e 673a 0a2a  es of testing:.*
-00003ce0: 202a 2a75 6e69 7420 7465 7374 696e 672a   **unit testing*
-00003cf0: 2a3a 2079 6f75 2063 616e 2072 756e 2074  *: you can run t
-00003d00: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
-00003d10: 7320 7275 6e6e 696e 6720 606d 616b 6520  s running `make 
-00003d20: 756e 6974 5f74 6573 7460 0a2a 202a 2a66  unit_test`.* **f
-00003d30: 756e 6374 696f 6e61 6c20 7465 7374 696e  unctional testin
-00003d40: 672a 2a3a 2079 6f75 206d 7573 7420 6861  g**: you must ha
-00003d50: 7665 2061 6e20 4157 5320 6163 636f 756e  ve an AWS accoun
-00003d60: 7420 7769 7468 2041 7468 656e 6120 7365  t with Athena se
-00003d70: 7475 7020 696e 206f 7264 6572 2074 6f20  tup in order to 
-00003d80: 6c61 756e 6368 2074 6869 7320 7479 7065  launch this type
-00003d90: 206f 6620 7465 7374 7320 616e 6420 6861   of tests and ha
-00003da0: 7665 2061 2060 2e65 6e76 6020 6669 6c65  ve a `.env` file
-00003db0: 2069 6e20 706c 6163 6520 7769 7468 2074   in place with t
-00003dc0: 6865 2072 6967 6874 2076 616c 7565 732e  he right values.
-00003dd0: 0a20 2059 6f75 2063 616e 2072 756e 2074  .  You can run t
-00003de0: 6869 7320 7479 7065 206f 6620 7465 7374  his type of test
-00003df0: 7320 7275 6e6e 696e 6720 606d 616b 6520  s running `make 
-00003e00: 6675 6e63 7469 6f6e 616c 5f74 6573 7460  functional_test`
-00003e10: 0a0a 0a41 6c6c 2074 7970 6520 6f66 2074  ...All type of t
-00003e20: 6573 7473 2063 616e 2062 6520 7275 6e20  ests can be run 
-00003e30: 7573 696e 6720 606d 616b 6560 3a0a 6060  using `make`:.``
-00003e40: 6062 6173 680a 6d61 6b65 2074 6573 740a  `bash.make test.
-00003e50: 6060 600a 0a23 2323 2320 5075 6c6c 2052  ```..#### Pull R
-00003e60: 6571 7565 7374 0a0a 2a20 4372 6561 7465  equest..* Create
-00003e70: 2061 2063 6f6d 6d69 7420 7769 7468 2079   a commit with y
-00003e80: 6f75 7220 6368 616e 6765 7320 616e 6420  our changes and 
-00003e90: 7075 7368 2074 6865 6d20 746f 2061 0a20  push them to a. 
-00003ea0: 205b 666f 726b 5d28 6874 7470 733a 2f2f   [fork](https://
-00003eb0: 646f 6373 2e67 6974 6875 622e 636f 6d2f  docs.github.com/
-00003ec0: 656e 2f67 6574 2d73 7461 7274 6564 2f71  en/get-started/q
-00003ed0: 7569 636b 7374 6172 742f 666f 726b 2d61  uickstart/fork-a
-00003ee0: 2d72 6570 6f29 2e0a 2a20 4372 6561 7465  -repo)..* Create
-00003ef0: 2061 205b 7075 6c6c 2072 6571 7565 7374   a [pull request
-00003f00: 206f 6e0a 2020 4769 7468 7562 5d28 6874   on.  Github](ht
-00003f10: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
-00003f20: 622e 636f 6d2f 656e 2f67 6974 6875 622f  b.com/en/github/
-00003f30: 636f 6c6c 6162 6f72 6174 696e 672d 7769  collaborating-wi
-00003f40: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
-00003f50: 2f70 726f 706f 7369 6e67 2d63 6861 6e67  /proposing-chang
-00003f60: 6573 2d74 6f2d 796f 7572 2d77 6f72 6b2d  es-to-your-work-
-00003f70: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
-00003f80: 7473 2f63 7265 6174 696e 672d 612d 7075  ts/creating-a-pu
-00003f90: 6c6c 2d72 6571 7565 7374 2d66 726f 6d2d  ll-request-from-
-00003fa0: 612d 666f 726b 292e 0a2a 2050 756c 6c20  a-fork)..* Pull 
-00003fb0: 7265 7175 6573 7420 7469 746c 6520 616e  request title an
-00003fc0: 6420 6d65 7373 6167 6520 2861 6e64 2050  d message (and P
-00003fd0: 5220 7469 746c 6520 616e 6420 6465 7363  R title and desc
-00003fe0: 7269 7074 696f 6e29 206d 7573 7420 6164  ription) must ad
-00003ff0: 6865 7265 2074 6f0a 2020 5b63 6f6e 7665  here to.  [conve
-00004000: 6e74 696f 6e61 6c63 6f6d 6d69 7473 5d28  ntionalcommits](
-00004010: 6874 7470 733a 2f2f 7777 772e 636f 6e76  https://www.conv
-00004020: 656e 7469 6f6e 616c 636f 6d6d 6974 732e  entionalcommits.
-00004030: 6f72 6729 2e0a 2a20 5075 6c6c 2072 6571  org)..* Pull req
-00004040: 7565 7374 2062 6f64 7920 7368 6f75 6c64  uest body should
-00004050: 2064 6573 6372 6962 6520 5f6d 6f74 6976   describe _motiv
-00004060: 6174 696f 6e5f 2e0a 0a23 2323 2048 656c  ation_...### Hel
-00004070: 7066 756c 2052 6573 6f75 7263 6573 0a0a  pful Resources..
-00004080: 2a20 5b41 7468 656e 6120 4352 4541 5445  * [Athena CREATE
-00004090: 2054 4142 4c45 2041 535d 2868 7474 7073   TABLE AS](https
-000040a0: 3a2f 2f64 6f63 732e 6177 732e 616d 617a  ://docs.aws.amaz
-000040b0: 6f6e 2e63 6f6d 2f61 7468 656e 612f 6c61  on.com/athena/la
-000040c0: 7465 7374 2f75 672f 6372 6561 7465 2d74  test/ug/create-t
-000040d0: 6162 6c65 2d61 732e 6874 6d6c 290a 2a20  able-as.html).* 
-000040e0: 5b64 6274 2d6c 6162 732f 6462 742d 636f  [dbt-labs/dbt-co
-000040f0: 7265 5d28 6874 7470 733a 2f2f 6769 7468  re](https://gith
-00004100: 7562 2e63 6f6d 2f64 6274 2d6c 6162 732f  ub.com/dbt-labs/
-00004110: 6462 742d 636f 7265 290a 2a20 5b6c 6175  dbt-core).* [lau
-00004120: 6768 696e 676d 616e 3737 3433 2f50 7941  ghingman7743/PyA
-00004130: 7468 656e 615d 2868 7474 7073 3a2f 2f67  thena](https://g
-00004140: 6974 6875 622e 636f 6d2f 6c61 7567 6869  ithub.com/laughi
-00004150: 6e67 6d61 6e37 3734 332f 5079 4174 6865  ngman7743/PyAthe
-00004160: 6e61 290a                                na).
+00001e00: 2f7b 7461 626c 657d 2f7b 7575 6964 3428  /{table}/{uuid4(
+00001e10: 297d 2f60 0a2a 2060 7363 6865 6d61 5f74  )}/`.* `schema_t
+00001e20: 6162 6c65 603a 2060 7b73 335f 6461 7461  able`: `{s3_data
+00001e30: 5f64 6972 7d2f 7b73 6368 656d 617d 2f7b  _dir}/{schema}/{
+00001e40: 7461 626c 657d 2f60 0a2a 2060 7333 5f64  table}/`.* `s3_d
+00001e50: 6174 615f 6e61 6d69 6e67 3d73 6368 656d  ata_naming=schem
+00001e60: 615f 7461 626c 655f 756e 6971 7565 603a  a_table_unique`:
+00001e70: 2060 7b73 335f 6461 7461 5f64 6972 7d2f   `{s3_data_dir}/
+00001e80: 7b73 6368 656d 617d 2f7b 7461 626c 657d  {schema}/{table}
+00001e90: 2f7b 7575 6964 3428 297d 2f60 0a0a 4974  /{uuid4()}/`..It
+00001ea0: 2773 2070 6f73 7369 626c 6520 746f 2073  's possible to s
+00001eb0: 6574 2074 6865 2060 7333 5f64 6174 615f  et the `s3_data_
+00001ec0: 6e61 6d69 6e67 6020 676c 6f62 616c 6c79  naming` globally
+00001ed0: 2069 6e20 7468 6520 7461 7267 6574 2070   in the target p
+00001ee0: 726f 6669 6c65 2c20 6f72 206f 7665 7277  rofile, or overw
+00001ef0: 7269 7465 2074 6865 2076 616c 7565 2069  rite the value i
+00001f00: 6e20 7468 6520 7461 626c 6520 636f 6e66  n the table conf
+00001f10: 6967 2c0a 6f72 2073 6574 7469 6e67 2075  ig,.or setting u
+00001f20: 7020 7468 6520 7661 6c75 6520 666f 7220  p the value for 
+00001f30: 6772 6f75 7073 206f 6620 6d6f 6465 6c20  groups of model 
+00001f40: 696e 2064 6274 5f70 726f 6a65 6374 2e79  in dbt_project.y
+00001f50: 6d6c 2e0a 0a3e 204e 6f74 653a 2077 6865  ml...> Note: whe
+00001f60: 6e20 7573 696e 6720 6120 776f 726b 2067  n using a work g
+00001f70: 726f 7570 2077 6974 6820 6120 6465 6661  roup with a defa
+00001f80: 756c 7420 6f75 7470 7574 206c 6f63 6174  ult output locat
+00001f90: 696f 6e20 636f 6e66 6967 7572 6564 2c20  ion configured, 
+00001fa0: 6073 335f 6461 7461 5f6e 616d 696e 6760  `s3_data_naming`
+00001fb0: 2061 6e64 2061 6e79 2063 6f6e 6669 6775   and any configu
+00001fc0: 7265 6420 6275 636b 6574 7320 6172 6520  red buckets are 
+00001fd0: 6967 6e6f 7265 6420 616e 6420 7468 6520  ignored and the 
+00001fe0: 6c6f 6361 7469 6f6e 2063 6f6e 6669 6775  location configu
+00001ff0: 7265 6420 696e 2074 6865 2077 6f72 6b20  red in the work 
+00002000: 6772 6f75 7020 6973 2075 7365 642e 0a0a  group is used...
+00002010: 2323 2320 496e 6372 656d 656e 7461 6c20  ### Incremental 
+00002020: 6d6f 6465 6c73 0a0a 5375 7070 6f72 7420  models..Support 
+00002030: 666f 7220 5b69 6e63 7265 6d65 6e74 616c  for [incremental
+00002040: 206d 6f64 656c 735d 2868 7474 7073 3a2f   models](https:/
+00002050: 2f64 6f63 732e 6765 7464 6274 2e63 6f6d  /docs.getdbt.com
+00002060: 2f64 6f63 732f 6275 696c 642f 696e 6372  /docs/build/incr
+00002070: 656d 656e 7461 6c2d 6d6f 6465 6c73 292e  emental-models).
+00002080: 0a0a 5468 6573 6520 7374 7261 7465 6769  ..These strategi
+00002090: 6573 2061 7265 2073 7570 706f 7274 6564  es are supported
+000020a0: 3a0a 0a2a 2060 696e 7365 7274 5f6f 7665  :..* `insert_ove
+000020b0: 7277 7269 7465 6020 2864 6566 6175 6c74  rwrite` (default
+000020c0: 293a 2054 6865 2069 6e73 6572 7420 6f76  ): The insert ov
+000020d0: 6572 7772 6974 6520 7374 7261 7465 6779  erwrite strategy
+000020e0: 2064 656c 6574 6573 2074 6865 206f 7665   deletes the ove
+000020f0: 726c 6170 7069 6e67 2070 6172 7469 7469  rlapping partiti
+00002100: 6f6e 7320 6672 6f6d 2074 6865 2064 6573  ons from the des
+00002110: 7469 6e61 7469 6f6e 0a74 6162 6c65 2c20  tination.table, 
+00002120: 616e 6420 7468 656e 2069 6e73 6572 7473  and then inserts
+00002130: 2074 6865 206e 6577 2072 6563 6f72 6473   the new records
+00002140: 2066 726f 6d20 7468 6520 736f 7572 6365   from the source
+00002150: 2e20 5468 6973 2073 7472 6174 6567 7920  . This strategy 
+00002160: 6465 7065 6e64 7320 6f6e 2074 6865 2060  depends on the `
+00002170: 7061 7274 6974 696f 6e65 645f 6279 6020  partitioned_by` 
+00002180: 6b65 7977 6f72 6421 2049 6620 6e6f 0a70  keyword! If no.p
+00002190: 6172 7469 7469 6f6e 7320 6172 6520 6465  artitions are de
+000021a0: 6669 6e65 642c 2064 6274 2077 696c 6c20  fined, dbt will 
+000021b0: 6661 6c6c 2062 6163 6b20 746f 2074 6865  fall back to the
+000021c0: 2060 6170 7065 6e64 6020 7374 7261 7465   `append` strate
+000021d0: 6779 2e0a 2a20 6061 7070 656e 6460 3a20  gy..* `append`: 
+000021e0: 496e 7365 7274 206e 6577 2072 6563 6f72  Insert new recor
+000021f0: 6473 2077 6974 686f 7574 2075 7064 6174  ds without updat
+00002200: 696e 672c 2064 656c 6574 696e 6720 6f72  ing, deleting or
+00002210: 206f 7665 7277 7269 7469 6e67 2061 6e79   overwriting any
+00002220: 2065 7869 7374 696e 6720 6461 7461 2e20   existing data. 
+00002230: 5468 6572 6520 6d69 6768 7420 6265 2064  There might be d
+00002240: 7570 6c69 6361 7465 0a64 6174 6120 2865  uplicate.data (e
+00002250: 2e67 2e20 6772 6561 7420 666f 7220 6c6f  .g. great for lo
+00002260: 6720 6f72 2068 6973 746f 7269 6361 6c20  g or historical 
+00002270: 6461 7461 292e 0a2a 2060 6d65 7267 6560  data)..* `merge`
+00002280: 3a20 436f 6e64 6974 696f 6e61 6c6c 7920  : Conditionally 
+00002290: 7570 6461 7465 732c 2064 656c 6574 6573  updates, deletes
+000022a0: 2c20 6f72 2069 6e73 6572 7473 2072 6f77  , or inserts row
+000022b0: 7320 696e 746f 2061 6e20 4963 6562 6572  s into an Iceber
+000022c0: 6720 7461 626c 652e 2055 7365 6420 696e  g table. Used in
+000022d0: 2063 6f6d 6269 6e61 7469 6f6e 2077 6974   combination wit
+000022e0: 6820 6075 6e69 7175 655f 6b65 7960 2e0a  h `unique_key`..
+000022f0: 4f6e 6c79 2061 7661 696c 6162 6c65 2077  Only available w
+00002300: 6865 6e20 7573 696e 6720 4963 6562 6572  hen using Iceber
+00002310: 672e 0a0a 2323 2320 4f6e 2073 6368 656d  g...### On schem
+00002320: 6120 6368 616e 6765 0a0a 606f 6e5f 7363  a change..`on_sc
+00002330: 6865 6d61 5f63 6861 6e67 6560 2069 7320  hema_change` is 
+00002340: 616e 206f 7074 696f 6e20 746f 2072 6566  an option to ref
+00002350: 6c65 6374 2063 6861 6e67 6573 206f 6620  lect changes of 
+00002360: 7363 6865 6d61 2069 6e20 696e 6372 656d  schema in increm
+00002370: 656e 7461 6c20 6d6f 6465 6c73 2e0a 5468  ental models..Th
+00002380: 6520 666f 6c6c 6f77 696e 6720 6f70 7469  e following opti
+00002390: 6f6e 7320 6172 6520 7375 7070 6f72 7465  ons are supporte
+000023a0: 643a 0a2a 2060 6967 6e6f 7265 6020 2864  d:.* `ignore` (d
+000023b0: 6566 6175 6c74 290a 2a20 6066 6169 6c60  efault).* `fail`
+000023c0: 0a2a 2060 6170 7065 6e64 5f6e 6577 5f63  .* `append_new_c
+000023d0: 6f6c 756d 6e73 600a 2a20 6073 796e 635f  olumns`.* `sync_
+000023e0: 616c 6c5f 636f 6c75 6d6e 7360 0a0a 496e  all_columns`..In
+000023f0: 2064 6574 6169 6c2c 2070 6c65 6173 6520   detail, please 
+00002400: 7265 6665 7220 746f 205b 6462 7420 646f  refer to [dbt do
+00002410: 6373 5d28 6874 7470 733a 2f2f 646f 6373  cs](https://docs
+00002420: 2e67 6574 6462 742e 636f 6d2f 646f 6373  .getdbt.com/docs
+00002430: 2f62 7569 6c64 2f69 6e63 7265 6d65 6e74  /build/increment
+00002440: 616c 2d6d 6f64 656c 7323 7768 6174 2d69  al-models#what-i
+00002450: 662d 7468 652d 636f 6c75 6d6e 732d 6f66  f-the-columns-of
+00002460: 2d6d 792d 696e 6372 656d 656e 7461 6c2d  -my-incremental-
+00002470: 6d6f 6465 6c2d 6368 616e 6765 292e 0a0a  model-change)...
+00002480: 2323 2320 4963 6562 6572 670a 0a54 6865  ### Iceberg..The
+00002490: 2061 6461 7074 6572 2073 7570 706f 7274   adapter support
+000024a0: 7320 7461 626c 6520 6d61 7465 7269 616c  s table material
+000024b0: 697a 6174 696f 6e20 666f 7220 4963 6562  ization for Iceb
+000024c0: 6572 672e 0a0a 546f 2067 6574 2073 7461  erg...To get sta
+000024d0: 7274 6564 206a 7573 7420 6164 6420 7468  rted just add th
+000024e0: 6973 2061 7320 796f 7572 206d 6f64 656c  is as your model
+000024f0: 3a0a 6060 600a 7b7b 2063 6f6e 6669 6728  :.```.{{ config(
+00002500: 0a20 2020 206d 6174 6572 6961 6c69 7a65  .    materialize
+00002510: 643d 2774 6162 6c65 272c 0a20 2020 2074  d='table',.    t
+00002520: 6162 6c65 5f74 7970 653d 2769 6365 6265  able_type='icebe
+00002530: 7267 272c 0a20 2020 2066 6f72 6d61 743d  rg',.    format=
+00002540: 2770 6172 7175 6574 272c 0a20 2020 2070  'parquet',.    p
+00002550: 6172 7469 7469 6f6e 6564 5f62 793d 5b27  artitioned_by=['
+00002560: 6275 636b 6574 2875 7365 725f 6964 2c20  bucket(user_id, 
+00002570: 3529 275d 2c0a 2020 2020 7461 626c 655f  5)'],.    table_
+00002580: 7072 6f70 6572 7469 6573 3d7b 0a20 2020  properties={.   
+00002590: 2009 276f 7074 696d 697a 655f 7265 7772   .'optimize_rewr
+000025a0: 6974 655f 6465 6c65 7465 5f66 696c 655f  ite_delete_file_
+000025b0: 7468 7265 7368 6f6c 6427 3a20 2732 270a  threshold': '2'.
+000025c0: 2020 2020 097d 0a29 207d 7d0a 0a53 454c      .}.) }}..SEL
+000025d0: 4543 540a 0927 4127 2041 5320 7573 6572  ECT..'A' AS user
+000025e0: 5f69 642c 0a09 2770 6927 2041 5320 6e61  _id,..'pi' AS na
+000025f0: 6d65 2c0a 0927 6163 7469 7665 2720 4153  me,..'active' AS
+00002600: 2073 7461 7475 732c 0a09 3137 2e38 3920   status,..17.89 
+00002610: 4153 2063 6f73 742c 0a09 3120 4153 2071  AS cost,..1 AS q
+00002620: 7561 6e74 6974 792c 0a09 3130 3030 3030  uantity,..100000
+00002630: 3030 3020 4153 2071 7561 6e74 6974 795f  000 AS quantity_
+00002640: 6269 672c 0a09 6375 7272 656e 745f 6461  big,..current_da
+00002650: 7465 2041 5320 6d79 5f64 6174 650a 6060  te AS my_date.``
+00002660: 600a 0a49 6365 6265 7267 2073 7570 706f  `..Iceberg suppo
+00002670: 7274 7320 6275 636b 6574 696e 6720 6173  rts bucketing as
+00002680: 2068 6964 6465 6e20 7061 7274 6974 696f   hidden partitio
+00002690: 6e73 2c20 7468 6572 6566 6f72 6520 7573  ns, therefore us
+000026a0: 6520 7468 6520 6070 6172 7469 7469 6f6e  e the `partition
+000026b0: 6564 5f62 7960 2063 6f6e 6669 6720 746f  ed_by` config to
+000026c0: 2061 6464 2073 7065 6369 6669 6320 6275   add specific bu
+000026d0: 636b 6574 696e 6720 636f 6e64 6974 696f  cketing conditio
+000026e0: 6e73 2e0a 0a49 6365 6265 7267 2073 7570  ns...Iceberg sup
+000026f0: 706f 7274 7320 7365 7665 7261 6c20 7461  ports several ta
+00002700: 626c 6520 666f 726d 6174 7320 666f 7220  ble formats for 
+00002710: 6461 7461 203a 2060 5041 5251 5545 5460  data : `PARQUET`
+00002720: 2c20 6041 5652 4f60 2061 6e64 2060 4f52  , `AVRO` and `OR
+00002730: 4360 2e0a 0a49 7420 6973 2070 6f73 7369  C`...It is possi
+00002740: 626c 6520 746f 2075 7365 2069 6365 6265  ble to use icebe
+00002750: 7267 2069 6e20 616e 2069 6e63 7265 6d65  rg in an increme
+00002760: 6e74 616c 2066 6173 6869 6f6e 2c20 7370  ntal fashion, sp
+00002770: 6563 6966 6963 616c 6c79 2032 2073 7472  ecifically 2 str
+00002780: 6174 6567 6965 7320 6172 6520 7375 7070  ategies are supp
+00002790: 6f72 7465 643a 0a2a 2060 6170 7065 6e64  orted:.* `append
+000027a0: 603a 206e 6577 2072 6563 6f72 6473 2061  `: new records a
+000027b0: 7265 2061 7070 656e 6465 6420 746f 2074  re appended to t
+000027c0: 6865 2074 6162 6c65 2c20 7468 6973 2063  he table, this c
+000027d0: 616e 206c 6561 6420 746f 2064 7570 6c69  an lead to dupli
+000027e0: 6361 7465 730a 2a20 606d 6572 6765 603a  cates.* `merge`:
+000027f0: 206d 7573 7420 6265 2075 7365 6420 696e   must be used in
+00002800: 2063 6f6d 6269 6e61 7469 6f6e 2077 6974   combination wit
+00002810: 6820 6075 6e69 7175 655f 6b65 7960 2061  h `unique_key` a
+00002820: 6e64 2069 7427 7320 6f6e 6c79 2061 7661  nd it's only ava
+00002830: 696c 6162 6c65 2077 6974 6820 456e 6769  ilable with Engi
+00002840: 6e65 2076 6572 7369 6f6e 2033 2e0a 2020  ne version 3..  
+00002850: 2049 7420 7065 7266 6f72 6d73 2061 6e20   It performs an 
+00002860: 7570 7365 7274 2c20 6e65 7720 7265 636f  upsert, new reco
+00002870: 7264 2061 7265 2061 6464 6564 2c20 616e  rd are added, an
+00002880: 6420 7265 636f 7264 2061 6c72 6561 6479  d record already
+00002890: 2065 7869 7374 696e 6720 6172 6520 7570   existing are up
+000028a0: 6461 7465 640a 0a23 2323 2048 6967 6820  dated..### High 
+000028b0: 6176 6169 6c61 626c 6520 7461 626c 6520  available table 
+000028c0: 6d61 7465 7269 616c 697a 6174 696f 6e0a  materialization.
+000028d0: 5468 6520 6375 7272 656e 7420 696d 706c  The current impl
+000028e0: 656d 656e 7461 7469 6f6e 206f 6620 7468  ementation of th
+000028f0: 6520 7461 626c 6520 6d61 7465 7269 616c  e table material
+00002900: 697a 6174 696f 6e20 6361 6e20 6c65 6164  ization can lead
+00002910: 2074 6f20 646f 776e 7469 6d65 2c20 6173   to downtime, as
+00002920: 2074 6172 6765 7420 7461 626c 6520 6973   target table is
+00002930: 2064 726f 7070 6564 2061 6e64 2072 652d   dropped and re-
+00002940: 6372 6561 7465 642e 0a54 6f20 6861 7665  created..To have
+00002950: 2074 6865 206c 6573 7320 6465 7374 7275   the less destru
+00002960: 6374 6976 6520 6265 6861 7669 6f72 2069  ctive behavior i
+00002970: 7427 7320 706f 7373 6962 6c65 2074 6f20  t's possible to 
+00002980: 7573 6520 6074 6162 6c65 3d27 7461 626c  use `table='tabl
+00002990: 655f 6869 7665 5f68 6127 6020 6d61 7465  e_hive_ha'` mate
+000029a0: 7269 616c 697a 6174 696f 6e2e 0a2a 2a74  rialization..**t
+000029b0: 6162 6c65 5f68 6976 655f 6861 2a2a 206c  able_hive_ha** l
+000029c0: 6576 6572 6167 6520 7468 6520 7461 626c  everage the tabl
+000029d0: 6520 7665 7273 696f 6e73 2066 6561 7475  e versions featu
+000029e0: 7265 206f 6620 676c 7565 2063 6174 616c  re of glue catal
+000029f0: 6f67 2c20 6372 6561 7469 6e67 2061 2074  og, creating a t
+00002a00: 6d70 2074 6162 6c65 2061 6e64 2073 7761  mp table and swa
+00002a10: 7070 696e 670a 7468 6520 7461 7267 6574  pping.the target
+00002a20: 2074 6162 6c65 2074 6f20 7468 6520 6c6f   table to the lo
+00002a30: 6361 7469 6f6e 206f 6620 7468 6520 746d  cation of the tm
+00002a40: 7020 7461 626c 652e 0a54 6869 7320 6d61  p table..This ma
+00002a50: 7465 7269 616c 697a 6174 696f 6e20 6973  terialization is
+00002a60: 206f 6e6c 7920 6176 6169 6c61 626c 6520   only available 
+00002a70: 666f 7220 6074 6162 6c65 5f74 7970 653d  for `table_type=
+00002a80: 6869 7665 6020 616e 6420 7265 7175 6972  hive` and requir
+00002a90: 6573 2075 7369 6e67 2075 6e69 7175 6520  es using unique 
+00002aa0: 6c6f 6361 7469 6f6e 732e 0a0a 6060 600a  locations...```.
+00002ab0: 7b7b 2063 6f6e 6669 6728 0a20 2020 206d  {{ config(.    m
+00002ac0: 6174 6572 6961 6c69 7a65 643d 2774 6162  aterialized='tab
+00002ad0: 6c65 5f68 6976 655f 6861 272c 0a20 2020  le_hive_ha',.   
+00002ae0: 2066 6f72 6d61 743d 2770 6172 7175 6574   format='parquet
+00002af0: 272c 0a20 2020 2070 6172 7469 7469 6f6e  ',.    partition
+00002b00: 5f62 793d 5b27 7374 6174 7573 275d 2c0a  _by=['status'],.
+00002b10: 2020 2020 7333 5f64 6174 615f 6e61 6d69      s3_data_nami
+00002b20: 6e67 3d27 7461 626c 655f 756e 6971 7565  ng='table_unique
+00002b30: 270a 2920 7d7d 0a0a 7365 6c65 6374 0a20  '.) }}..select. 
+00002b40: 2027 6127 2061 7320 7573 6572 5f69 642c   'a' as user_id,
+00002b50: 0a20 2027 7069 2720 6173 2075 7365 725f  .  'pi' as user_
+00002b60: 6e61 6d65 2c0a 2020 2761 6374 6976 6527  name,.  'active'
+00002b70: 2061 7320 7374 6174 7573 0a75 6e69 6f6e   as status.union
+00002b80: 2061 6c6c 0a73 656c 6563 740a 2020 2762   all.select.  'b
+00002b90: 2720 6173 2075 7365 725f 6964 2c0a 2020  ' as user_id,.  
+00002ba0: 2773 6827 2061 7320 7573 6572 5f6e 616d  'sh' as user_nam
+00002bb0: 652c 0a20 2027 6469 7361 626c 6564 2720  e,.  'disabled' 
+00002bc0: 6173 2073 7461 7475 730a 6060 600a 0a42  as status.```..B
+00002bd0: 7920 6465 6661 756c 742c 2074 6865 206d  y default, the m
+00002be0: 6174 6572 6961 6c69 7a61 7469 6f6e 206b  aterialization k
+00002bf0: 6565 7073 2074 6865 206c 6173 7420 3420  eeps the last 4 
+00002c00: 7461 626c 6520 7665 7273 696f 6e73 2c20  table versions, 
+00002c10: 796f 7520 6361 6e20 6368 616e 6765 2069  you can change i
+00002c20: 7420 7468 6174 2073 6574 7469 6e67 2060  t that setting `
+00002c30: 7665 7273 696f 6e73 5f74 6f5f 6b65 6570  versions_to_keep
+00002c40: 602e 0a0a 2323 2323 204b 6e6f 776e 2069  `...#### Known i
+00002c50: 7373 7565 730a 2a20 5768 656e 2073 7761  ssues.* When swa
+00002c60: 7070 696e 6720 6672 6f6d 2061 2074 6162  pping from a tab
+00002c70: 6c65 2077 6974 6820 7061 7274 6974 696f  le with partitio
+00002c80: 6e73 2074 6f20 6120 7461 626c 6520 7769  ns to a table wi
+00002c90: 7468 6f75 7420 2861 6e64 2074 6865 206f  thout (and the o
+00002ca0: 7468 6572 2077 6179 2061 726f 756e 6429  ther way around)
+00002cb0: 2c20 7468 6572 6520 636f 756c 6420 6265  , there could be
+00002cc0: 2061 206c 6974 746c 6520 646f 776e 7469   a little downti
+00002cd0: 6d65 2e0a 2020 496e 2063 6173 6520 6869  me..  In case hi
+00002ce0: 6768 2070 6572 666f 726d 616e 6365 7320  gh performances 
+00002cf0: 6172 6520 6e65 6564 6564 2063 6f6e 7369  are needed consi
+00002d00: 6465 7220 6275 636b 6574 696e 6720 696e  der bucketing in
+00002d10: 7374 6561 6420 6f66 2070 6172 7469 7469  stead of partiti
+00002d20: 6f6e 730a 2a20 4279 2064 6566 6175 6c74  ons.* By default
+00002d30: 2c20 476c 7565 2022 6475 706c 6963 6174  , Glue "duplicat
+00002d40: 6522 2074 6865 2076 6572 7369 6f6e 7320  e" the versions 
+00002d50: 696e 7465 726e 616c 6c79 2c20 736f 2074  internally, so t
+00002d60: 6865 206c 6173 7420 3220 7665 7273 696f  he last 2 versio
+00002d70: 6e73 206f 6620 6120 7461 626c 6520 706f  ns of a table po
+00002d80: 696e 7420 746f 2074 6865 2073 616d 6520  int to the same 
+00002d90: 6c6f 6361 7469 6f6e 0a2a 2049 7427 7320  location.* It's 
+00002da0: 7265 636f 6d6d 656e 6465 6420 746f 2068  recommended to h
+00002db0: 6176 6520 7665 7273 696f 6e73 5f74 6f5f  ave versions_to_
+00002dc0: 6b65 6570 3e3d 2034 2c20 6173 2074 6869  keep>= 4, as thi
+00002dd0: 7320 7769 6c6c 2061 766f 6964 2074 6f20  s will avoid to 
+00002de0: 6861 7665 2074 6865 206f 6c64 6572 206c  have the older l
+00002df0: 6f63 6174 696f 6e20 7265 6d6f 7665 640a  ocation removed.
+00002e00: 2a20 5468 6520 6d61 6372 6f20 6174 6865  * The macro athe
+00002e10: 6e61 5f5f 656e 645f 6f66 5f74 696d 6520  na__end_of_time 
+00002e20: 6e65 6564 7320 746f 2062 6520 6f76 6572  needs to be over
+00002e30: 7772 6974 7465 6e20 6279 2074 6865 2075  written by the u
+00002e40: 7365 7220 6966 2075 7369 6e67 2041 7468  ser if using Ath
+00002e50: 656e 6120 7633 2073 696e 6365 2069 7420  ena v3 since it 
+00002e60: 7265 7175 6972 6573 2061 2070 7265 6369  requires a preci
+00002e70: 7369 6f6e 2070 6172 616d 6574 6572 2066  sion parameter f
+00002e80: 6f72 2074 696d 6573 7461 6d70 730a 0a0a  or timestamps...
+00002e90: 2323 2053 6e61 7073 686f 7473 0a0a 5468  ## Snapshots..Th
+00002ea0: 6520 6164 6170 7465 7220 7375 7070 6f72  e adapter suppor
+00002eb0: 7473 2073 6e61 7073 686f 7420 6d61 7465  ts snapshot mate
+00002ec0: 7269 616c 697a 6174 696f 6e2e 2049 7420  rialization. It 
+00002ed0: 7375 7070 6f72 7473 2062 6f74 6820 7469  supports both ti
+00002ee0: 6d65 7374 616d 7020 616e 6420 6368 6563  mestamp and chec
+00002ef0: 6b20 7374 7261 7465 6779 2e20 546f 2063  k strategy. To c
+00002f00: 7265 6174 6520 6120 736e 6170 7368 6f74  reate a snapshot
+00002f10: 2063 7265 6174 6520 6120 736e 6170 7368   create a snapsh
+00002f20: 6f74 2066 696c 6520 696e 2074 6865 2073  ot file in the s
+00002f30: 6e61 7073 686f 7473 2064 6972 6563 746f  napshots directo
+00002f40: 7279 2e20 4966 2064 6972 6563 746f 7279  ry. If directory
+00002f50: 2064 6f65 7320 6e6f 7420 6578 6973 7420   does not exist 
+00002f60: 6372 6561 7465 206f 6e65 2e0a 0a23 2323  create one...###
+00002f70: 2054 696d 6573 7461 6d70 2073 7472 6174   Timestamp strat
+00002f80: 6567 790a 0a54 6f20 7573 6520 7468 6520  egy..To use the 
+00002f90: 7469 6d65 7374 616d 7020 7374 7261 7465  timestamp strate
+00002fa0: 6779 2072 6566 6572 2074 6f20 7468 6520  gy refer to the 
+00002fb0: 5b64 6274 2064 6f63 735d 2868 7474 7073  [dbt docs](https
+00002fc0: 3a2f 2f64 6f63 732e 6765 7464 6274 2e63  ://docs.getdbt.c
+00002fd0: 6f6d 2f64 6f63 732f 6275 696c 642f 736e  om/docs/build/sn
+00002fe0: 6170 7368 6f74 7323 7469 6d65 7374 616d  apshots#timestam
+00002ff0: 702d 7374 7261 7465 6779 2d72 6563 6f6d  p-strategy-recom
+00003000: 6d65 6e64 6564 290a 0a23 2323 2043 6865  mended)..### Che
+00003010: 636b 2073 7472 6174 6567 790a 0a54 6f20  ck strategy..To 
+00003020: 7573 6520 7468 6520 6368 6563 6b20 7374  use the check st
+00003030: 7261 7465 6779 2072 6566 6572 2074 6f20  rategy refer to 
+00003040: 7468 6520 5b64 6274 2064 6f63 735d 2868  the [dbt docs](h
+00003050: 7474 7073 3a2f 2f64 6f63 732e 6765 7464  ttps://docs.getd
+00003060: 6274 2e63 6f6d 2f64 6f63 732f 6275 696c  bt.com/docs/buil
+00003070: 642f 736e 6170 7368 6f74 7323 6368 6563  d/snapshots#chec
+00003080: 6b2d 7374 7261 7465 6779 290a 0a23 2323  k-strategy)..###
+00003090: 2048 6172 642d 6465 6c65 7465 730a 0a54   Hard-deletes..T
+000030a0: 6865 206d 6174 6572 6961 6c69 7a61 7469  he materializati
+000030b0: 6f6e 2061 6c73 6f20 7375 7070 6f72 7473  on also supports
+000030c0: 2069 6e76 616c 6964 6174 696e 6720 6861   invalidating ha
+000030d0: 7264 2064 656c 6574 6573 2e20 4368 6563  rd deletes. Chec
+000030e0: 6b20 7468 6520 5b64 6f63 735d 2868 7474  k the [docs](htt
+000030f0: 7073 3a2f 2f64 6f63 732e 6765 7464 6274  ps://docs.getdbt
+00003100: 2e63 6f6d 2f64 6f63 732f 6275 696c 642f  .com/docs/build/
+00003110: 736e 6170 7368 6f74 7323 6861 7264 2d64  snapshots#hard-d
+00003120: 656c 6574 6573 2d6f 7074 2d69 6e29 2074  eletes-opt-in) t
+00003130: 6f20 756e 6465 7273 7461 6e64 2075 7361  o understand usa
+00003140: 6765 2e0a 0a23 2323 2057 6f72 6b69 6e67  ge...### Working
+00003150: 2065 7861 6d70 6c65 0a0a 7365 6564 2066   example..seed f
+00003160: 696c 6520 2d20 656d 706c 6f79 656e 745f  ile - employent_
+00003170: 696e 6469 6361 746f 7273 5f6e 6f76 656d  indicators_novem
+00003180: 6265 725f 3230 3232 5f63 7376 5f74 6162  ber_2022_csv_tab
+00003190: 6c65 732e 6373 760a 6060 600a 5365 7269  les.csv.```.Seri
+000031a0: 6573 5f72 6566 6572 656e 6365 2c50 6572  es_reference,Per
+000031b0: 696f 642c 4461 7461 5f76 616c 7565 2c53  iod,Data_value,S
+000031c0: 7570 7072 6573 7365 640a 4d45 494d 2e53  uppressed.MEIM.S
+000031d0: 3157 412c 3139 3939 2e30 342c 3830 3236  1WA,1999.04,8026
+000031e0: 372c 0a4d 4549 4d2e 5331 5741 2c31 3939  7,.MEIM.S1WA,199
+000031f0: 392e 3035 2c37 3038 3033 2c0a 4d45 494d  9.05,70803,.MEIM
+00003200: 2e53 3157 412c 3139 3939 2e30 362c 3635  .S1WA,1999.06,65
+00003210: 3739 322c 0a4d 4549 4d2e 5331 5741 2c31  792,.MEIM.S1WA,1
+00003220: 3939 392e 3037 2c36 3631 3934 2c0a 4d45  999.07,66194,.ME
+00003230: 494d 2e53 3157 412c 3139 3939 2e30 382c  IM.S1WA,1999.08,
+00003240: 3637 3235 392c 0a4d 4549 4d2e 5331 5741  67259,.MEIM.S1WA
+00003250: 2c31 3939 392e 3039 2c36 3936 3931 2c0a  ,1999.09,69691,.
+00003260: 4d45 494d 2e53 3157 412c 3139 3939 2e31  MEIM.S1WA,1999.1
+00003270: 2c37 3234 3735 2c0a 4d45 494d 2e53 3157  ,72475,.MEIM.S1W
+00003280: 412c 3139 3939 2e31 312c 3739 3236 332c  A,1999.11,79263,
+00003290: 0a4d 4549 4d2e 5331 5741 2c31 3939 392e  .MEIM.S1WA,1999.
+000032a0: 3132 2c38 3635 3430 2c0a 4d45 494d 2e53  12,86540,.MEIM.S
+000032b0: 3157 412c 3230 3030 2e30 312c 3832 3535  1WA,2000.01,8255
+000032c0: 322c 0a4d 4549 4d2e 5331 5741 2c32 3030  2,.MEIM.S1WA,200
+000032d0: 302e 3032 2c38 3137 3039 2c0a 4d45 494d  0.02,81709,.MEIM
+000032e0: 2e53 3157 412c 3230 3030 2e30 332c 3834  .S1WA,2000.03,84
+000032f0: 3132 362c 0a4d 4549 4d2e 5331 5741 2c32  126,.MEIM.S1WA,2
+00003300: 3030 302e 3034 2c37 3730 3839 2c0a 4d45  000.04,77089,.ME
+00003310: 494d 2e53 3157 412c 3230 3030 2e30 352c  IM.S1WA,2000.05,
+00003320: 3733 3831 312c 0a4d 4549 4d2e 5331 5741  73811,.MEIM.S1WA
+00003330: 2c32 3030 302e 3036 2c37 3030 3730 2c0a  ,2000.06,70070,.
+00003340: 4d45 494d 2e53 3157 412c 3230 3030 2e30  MEIM.S1WA,2000.0
+00003350: 372c 3639 3837 332c 0a4d 4549 4d2e 5331  7,69873,.MEIM.S1
+00003360: 5741 2c32 3030 302e 3038 2c37 3134 3638  WA,2000.08,71468
+00003370: 2c0a 4d45 494d 2e53 3157 412c 3230 3030  ,.MEIM.S1WA,2000
+00003380: 2e30 392c 3732 3436 322c 0a4d 4549 4d2e  .09,72462,.MEIM.
+00003390: 5331 5741 2c32 3030 302e 312c 3734 3839  S1WA,2000.1,7489
+000033a0: 372c 0a60 6060 0a0a 6d6f 6465 6c2e 7371  7,.```..model.sq
+000033b0: 6c0a 6060 600a 7b7b 2063 6f6e 6669 6728  l.```.{{ config(
+000033c0: 0a20 2020 206d 6174 6572 6961 6c69 7a65  .    materialize
+000033d0: 643d 2774 6162 6c65 270a 2920 7d7d 0a0a  d='table'.) }}..
+000033e0: 5345 4c45 4354 0a20 2020 2052 4f57 5f4e  SELECT.    ROW_N
+000033f0: 554d 4245 5228 2920 4f56 4552 2028 2920  UMBER() OVER () 
+00003400: 4153 2069 640a 2020 2020 2c20 2a0a 2020  AS id.    , *.  
+00003410: 2020 2c20 6361 7374 2866 726f 6d5f 756e    , cast(from_un
+00003420: 6978 7469 6d65 2874 6f5f 756e 6978 7469  ixtime(to_unixti
+00003430: 6d65 286e 6f77 2829 2929 2061 7320 7469  me(now())) as ti
+00003440: 6d65 7374 616d 7028 3629 2920 4153 2072  mestamp(6)) AS r
+00003450: 6566 7265 7368 5f74 696d 6573 7461 6d70  efresh_timestamp
+00003460: 0a46 524f 4d20 7b7b 2072 6566 2827 656d  .FROM {{ ref('em
+00003470: 706c 6f79 6d65 6e74 5f69 6e64 6963 6174  ployment_indicat
+00003480: 6f72 735f 6e6f 7665 6d62 6572 5f32 3032  ors_november_202
+00003490: 325f 6373 765f 7461 626c 6573 2729 207d  2_csv_tables') }
+000034a0: 7d0a 6060 600a 0a74 696d 6573 7461 6d70  }.```..timestamp
+000034b0: 2073 7472 6174 6567 7920 2d20 6d6f 6465   strategy - mode
+000034c0: 6c5f 736e 6170 7368 6f74 5f31 0a0a 6060  l_snapshot_1..``
+000034d0: 600a 7b25 2073 6e61 7073 686f 7420 6d6f  `.{% snapshot mo
+000034e0: 6465 6c5f 736e 6170 7368 6f74 5f31 2025  del_snapshot_1 %
+000034f0: 7d0a 0a7b 7b0a 2020 2020 636f 6e66 6967  }..{{.    config
+00003500: 280a 2020 2020 2020 7374 7261 7465 6779  (.      strategy
+00003510: 3d27 7469 6d65 7374 616d 7027 2c0a 2020  ='timestamp',.  
+00003520: 2020 2020 7570 6461 7465 645f 6174 3d27      updated_at='
+00003530: 7265 6672 6573 685f 7469 6d65 7374 616d  refresh_timestam
+00003540: 7027 2c0a 2020 2020 2020 756e 6971 7565  p',.      unique
+00003550: 5f6b 6579 3d27 6964 270a 2020 2020 290a  _key='id'.    ).
+00003560: 7d7d 0a0a 5345 4c45 4354 202a 0a0a 6672  }}..SELECT *..fr
+00003570: 6f6d 207b 7b20 7265 6628 276d 6f64 656c  om {{ ref('model
+00003580: 2729 207d 7d0a 0a7b 2520 656e 6473 6e61  ') }}..{% endsna
+00003590: 7073 686f 7420 257d 0a60 6060 0a0a 696e  pshot %}.```..in
+000035a0: 7661 6c69 6461 7465 2068 6172 6420 6465  validate hard de
+000035b0: 6c65 7465 7320 2d20 6d6f 6465 6c5f 736e  letes - model_sn
+000035c0: 6170 7368 6f74 5f32 0a60 6060 0a7b 2520  apshot_2.```.{% 
+000035d0: 736e 6170 7368 6f74 206d 6f64 656c 5f73  snapshot model_s
+000035e0: 6e61 7073 686f 745f 3220 257d 0a0a 7b7b  napshot_2 %}..{{
+000035f0: 0a20 2020 2063 6f6e 6669 670a 2020 2020  .    config.    
+00003600: 280a 2020 2020 2020 2020 756e 6971 7565  (.        unique
+00003610: 5f6b 6579 3d27 6964 272c 0a20 2020 2020  _key='id',.     
+00003620: 2020 2073 7472 6174 6567 793d 2774 696d     strategy='tim
+00003630: 6573 7461 6d70 272c 0a20 2020 2020 2020  estamp',.       
+00003640: 2075 7064 6174 6564 5f61 743d 2772 6566   updated_at='ref
+00003650: 7265 7368 5f74 696d 6573 7461 6d70 272c  resh_timestamp',
+00003660: 0a20 2020 2020 2020 2069 6e76 616c 6964  .        invalid
+00003670: 6174 655f 6861 7264 5f64 656c 6574 6573  ate_hard_deletes
+00003680: 3d54 7275 652c 0a20 2020 2029 0a7d 7d0a  =True,.    ).}}.
+00003690: 5345 4c45 4354 202a 2066 726f 6d20 7b7b  SELECT * from {{
+000036a0: 2072 6566 2827 6d6f 6465 6c27 2920 7d7d   ref('model') }}
+000036b0: 0a0a 7b25 2065 6e64 736e 6170 7368 6f74  ..{% endsnapshot
+000036c0: 2025 7d0a 6060 600a 0a63 6865 636b 2073   %}.```..check s
+000036d0: 7472 6174 6567 7920 2d20 6d6f 6465 6c5f  trategy - model_
+000036e0: 736e 6170 7368 6f74 5f33 0a60 6060 0a7b  snapshot_3.```.{
+000036f0: 2520 736e 6170 7368 6f74 206d 6f64 656c  % snapshot model
+00003700: 5f73 6e61 7073 686f 745f 3320 257d 0a0a  _snapshot_3 %}..
+00003710: 7b7b 0a20 2020 2063 6f6e 6669 670a 2020  {{.    config.  
+00003720: 2020 280a 2020 2020 2020 2020 756e 6971    (.        uniq
+00003730: 7565 5f6b 6579 3d27 6964 272c 0a20 2020  ue_key='id',.   
+00003740: 2020 2020 2073 7472 6174 6567 793d 2763       strategy='c
+00003750: 6865 636b 272c 0a20 2020 2020 2020 2063  heck',.        c
+00003760: 6865 636b 5f63 6f6c 733d 5b27 7365 7269  heck_cols=['seri
+00003770: 6573 5f72 6566 6572 656e 6365 272c 2764  es_reference','d
+00003780: 6174 615f 7661 6c75 6527 5d0a 2020 2020  ata_value'].    
+00003790: 290a 7d7d 0a53 454c 4543 5420 2a20 6672  ).}}.SELECT * fr
+000037a0: 6f6d 207b 7b20 7265 6628 276d 6f64 656c  om {{ ref('model
+000037b0: 2729 207d 7d0a 0a7b 2520 656e 6473 6e61  ') }}..{% endsna
+000037c0: 7073 686f 7420 257d 0a60 6060 0a0a 2323  pshot %}.```..##
+000037d0: 2320 4b6e 6f77 6e20 6973 7375 6573 0a0a  # Known issues..
+000037e0: 2a20 496e 6372 656d 656e 7461 6c20 4963  * Incremental Ic
+000037f0: 6562 6572 6720 6d6f 6465 6c73 202d 2053  eberg models - S
+00003800: 796e 6320 616c 6c20 636f 6c75 6d6e 7320  ync all columns 
+00003810: 6f6e 2073 6368 656d 6120 6368 616e 6765  on schema change
+00003820: 2063 616e 2774 2072 656d 6f76 6520 636f   can't remove co
+00003830: 6c75 6d6e 7320 7573 6564 2061 7320 7061  lumns used as pa
+00003840: 7274 6974 696f 6e69 6e67 2e0a 5468 6520  rtitioning..The 
+00003850: 6f6e 6c79 2077 6179 2c20 6672 6f6d 2061  only way, from a
+00003860: 2064 6274 2070 6572 7370 6563 7469 7665   dbt perspective
+00003870: 2c20 6973 2074 6f20 646f 2061 2066 756c  , is to do a ful
+00003880: 6c2d 7265 6672 6573 6820 6f66 2074 6865  l-refresh of the
+00003890: 2069 6e63 7265 6d65 6e74 616c 206d 6f64   incremental mod
+000038a0: 656c 2e0a 0a2a 2054 6162 6c65 732c 2073  el...* Tables, s
+000038b0: 6368 656d 6173 2061 6e64 2064 6174 6162  chemas and datab
+000038c0: 6173 6520 7368 6f75 6c64 206f 6e6c 7920  ase should only 
+000038d0: 6265 206c 6f77 6572 6361 7365 0a0a 2a20  be lowercase..* 
+000038e0: 496e 206f 7264 6572 2074 6f20 6176 6f69  In order to avoi
+000038f0: 6420 706f 7465 6e74 6961 6c20 636f 6e66  d potential conf
+00003900: 6c69 6374 732c 206d 616b 6520 7375 7265  licts, make sure
+00003910: 205b 6064 6274 2d61 7468 656e 612d 6164   [`dbt-athena-ad
+00003920: 6170 7465 7260 5d28 6874 7470 733a 2f2f  apter`](https://
+00003930: 6769 7468 7562 2e63 6f6d 2f54 6f6d 6d65  github.com/Tomme
+00003940: 2f64 6274 2d61 7468 656e 6129 2069 7320  /dbt-athena) is 
+00003950: 6e6f 7420 696e 7374 616c 6c65 6420 696e  not installed in
+00003960: 2074 6865 2074 6172 6765 7420 656e 7669   the target envi
+00003970: 726f 6e6d 656e 742e 0a20 2053 6565 2068  ronment..  See h
+00003980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003990: 6d2f 6462 742d 6174 6865 6e61 2f64 6274  m/dbt-athena/dbt
+000039a0: 2d61 7468 656e 612f 6973 7375 6573 2f31  -athena/issues/1
+000039b0: 3033 2066 6f72 206d 6f72 6520 6465 7461  03 for more deta
+000039c0: 696c 732e 0a0a 2a20 536e 6170 7368 6f74  ils...* Snapshot
+000039d0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+000039e0: 7420 6472 6f70 7069 6e67 2063 6f6c 756d  t dropping colum
+000039f0: 6e73 2066 726f 6d20 7468 6520 736f 7572  ns from the sour
+00003a00: 6365 2074 6162 6c65 2e20 4966 2079 6f75  ce table. If you
+00003a10: 2064 726f 7020 6120 636f 6c75 6d6e 206d   drop a column m
+00003a20: 616b 6520 7375 7265 2074 6f20 6472 6f70  ake sure to drop
+00003a30: 2074 6865 2063 6f6c 756d 6e20 6672 6f6d   the column from
+00003a40: 2074 6865 2073 6e61 7073 686f 7420 6173   the snapshot as
+00003a50: 2077 656c 6c2e 2041 6e6f 7468 6572 2077   well. Another w
+00003a60: 6f72 6b61 726f 756e 6420 6973 2074 6f20  orkaround is to 
+00003a70: 4e55 4c4c 2074 6865 2063 6f6c 756d 6e20  NULL the column 
+00003a80: 696e 2074 6865 2073 6e61 7073 686f 7420  in the snapshot 
+00003a90: 6465 6669 6e69 7469 6f6e 2074 6f20 7072  definition to pr
+00003aa0: 6573 6572 7665 2068 6973 746f 7279 0a0a  eserve history..
+00003ab0: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00003ac0: 0a0a 5468 6973 2063 6f6e 6e65 6374 6f72  ..This connector
+00003ad0: 2077 6f72 6b73 2077 6974 6820 5079 7468   works with Pyth
+00003ae0: 6f6e 2066 726f 6d20 332e 3720 746f 2033  on from 3.7 to 3
+00003af0: 2e31 312e 0a0a 2323 2320 4765 7474 696e  .11...### Gettin
+00003b00: 6720 7374 6172 7465 640a 0a49 6e20 6f72  g started..In or
+00003b10: 6465 7220 746f 2073 7461 7274 2064 6576  der to start dev
+00003b20: 656c 6f70 696e 6720 6f6e 2074 6869 7320  eloping on this 
+00003b30: 6164 6170 7465 7220 636c 6f6e 6520 7468  adapter clone th
+00003b40: 6520 7265 706f 2061 6e64 2072 756e 2074  e repo and run t
+00003b50: 6869 7320 6d61 6b65 2063 6f6d 6d61 6e64  his make command
+00003b60: 2028 7365 6520 5b4d 616b 6566 696c 655d   (see [Makefile]
+00003b70: 284d 616b 6566 696c 6529 2920 3a0a 0a60  (Makefile)) :..`
+00003b80: 6060 6261 7368 0a6d 616b 6520 7365 7475  ``bash.make setu
+00003b90: 700a 6060 600a 0a49 7420 7769 6c6c 203a  p.```..It will :
+00003ba0: 0a31 2e20 496e 7374 616c 6c20 616c 6c20  .1. Install all 
+00003bb0: 6465 7065 6e64 656e 6369 6573 2e0a 322e  dependencies..2.
+00003bc0: 2049 6e73 7461 6c6c 2070 7265 2d63 6f6d   Install pre-com
+00003bd0: 6d69 7420 686f 6f6b 732e 0a33 2e20 4765  mit hooks..3. Ge
+00003be0: 6e65 7261 7465 2079 6f75 7220 602e 656e  nerate your `.en
+00003bf0: 7660 2066 696c 650a 0a4e 6578 742c 2061  v` file..Next, a
+00003c00: 646a 7573 7420 602e 656e 7660 2066 696c  djust `.env` fil
+00003c10: 6520 6279 2063 6f6e 6669 6775 7269 6e67  e by configuring
+00003c20: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
+00003c30: 2076 6172 6961 626c 6573 2074 6f20 6d61   variables to ma
+00003c40: 7463 6820 796f 7572 2041 7468 656e 6120  tch your Athena 
+00003c50: 6465 7665 6c6f 706d 656e 7420 656e 7669  development envi
+00003c60: 726f 6e6d 656e 742e 0a0a 2323 2320 5275  ronment...### Ru
+00003c70: 6e6e 696e 6720 7465 7374 730a 0a57 6520  nning tests..We 
+00003c80: 6861 7665 2032 2064 6966 6665 7265 6e74  have 2 different
+00003c90: 2074 7970 6573 206f 6620 7465 7374 696e   types of testin
+00003ca0: 673a 0a2a 202a 2a75 6e69 7420 7465 7374  g:.* **unit test
+00003cb0: 696e 672a 2a3a 2079 6f75 2063 616e 2072  ing**: you can r
+00003cc0: 756e 2074 6869 7320 7479 7065 206f 6620  un this type of 
+00003cd0: 7465 7374 7320 7275 6e6e 696e 6720 606d  tests running `m
+00003ce0: 616b 6520 756e 6974 5f74 6573 7460 0a2a  ake unit_test`.*
+00003cf0: 202a 2a66 756e 6374 696f 6e61 6c20 7465   **functional te
+00003d00: 7374 696e 672a 2a3a 2079 6f75 206d 7573  sting**: you mus
+00003d10: 7420 6861 7665 2061 6e20 4157 5320 6163  t have an AWS ac
+00003d20: 636f 756e 7420 7769 7468 2041 7468 656e  count with Athen
+00003d30: 6120 7365 7475 7020 696e 206f 7264 6572  a setup in order
+00003d40: 2074 6f20 6c61 756e 6368 2074 6869 7320   to launch this 
+00003d50: 7479 7065 206f 6620 7465 7374 7320 616e  type of tests an
+00003d60: 6420 6861 7665 2061 2060 2e65 6e76 6020  d have a `.env` 
+00003d70: 6669 6c65 2069 6e20 706c 6163 6520 7769  file in place wi
+00003d80: 7468 2074 6865 2072 6967 6874 2076 616c  th the right val
+00003d90: 7565 732e 0a20 2059 6f75 2063 616e 2072  ues..  You can r
+00003da0: 756e 2074 6869 7320 7479 7065 206f 6620  un this type of 
+00003db0: 7465 7374 7320 7275 6e6e 696e 6720 606d  tests running `m
+00003dc0: 616b 6520 6675 6e63 7469 6f6e 616c 5f74  ake functional_t
+00003dd0: 6573 7460 0a0a 416c 6c20 7479 7065 206f  est`..All type o
+00003de0: 6620 7465 7374 7320 6361 6e20 6265 2072  f tests can be r
+00003df0: 756e 2075 7369 6e67 2060 6d61 6b65 603a  un using `make`:
+00003e00: 0a60 6060 6261 7368 0a6d 616b 6520 7465  .```bash.make te
+00003e10: 7374 0a60 6060 0a0a 2323 2320 5075 6c6c  st.```..### Pull
+00003e20: 2052 6571 7565 7374 0a0a 2a20 4372 6561   Request..* Crea
+00003e30: 7465 2061 2063 6f6d 6d69 7420 7769 7468  te a commit with
+00003e40: 2079 6f75 7220 6368 616e 6765 7320 616e   your changes an
+00003e50: 6420 7075 7368 2074 6865 6d20 746f 2061  d push them to a
+00003e60: 0a20 205b 666f 726b 5d28 6874 7470 733a  .  [fork](https:
+00003e70: 2f2f 646f 6373 2e67 6974 6875 622e 636f  //docs.github.co
+00003e80: 6d2f 656e 2f67 6574 2d73 7461 7274 6564  m/en/get-started
+00003e90: 2f71 7569 636b 7374 6172 742f 666f 726b  /quickstart/fork
+00003ea0: 2d61 2d72 6570 6f29 2e0a 2a20 4372 6561  -a-repo)..* Crea
+00003eb0: 7465 2061 205b 7075 6c6c 2072 6571 7565  te a [pull reque
+00003ec0: 7374 206f 6e0a 2020 4769 7468 7562 5d28  st on.  Github](
+00003ed0: 6874 7470 733a 2f2f 646f 6373 2e67 6974  https://docs.git
+00003ee0: 6875 622e 636f 6d2f 656e 2f67 6974 6875  hub.com/en/githu
+00003ef0: 622f 636f 6c6c 6162 6f72 6174 696e 672d  b/collaborating-
+00003f00: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
+00003f10: 7473 2f70 726f 706f 7369 6e67 2d63 6861  ts/proposing-cha
+00003f20: 6e67 6573 2d74 6f2d 796f 7572 2d77 6f72  nges-to-your-wor
+00003f30: 6b2d 7769 7468 2d70 756c 6c2d 7265 7175  k-with-pull-requ
+00003f40: 6573 7473 2f63 7265 6174 696e 672d 612d  ests/creating-a-
+00003f50: 7075 6c6c 2d72 6571 7565 7374 2d66 726f  pull-request-fro
+00003f60: 6d2d 612d 666f 726b 292e 0a2a 2050 756c  m-a-fork)..* Pul
+00003f70: 6c20 7265 7175 6573 7420 7469 746c 6520  l request title 
+00003f80: 616e 6420 6d65 7373 6167 6520 2861 6e64  and message (and
+00003f90: 2050 5220 7469 746c 6520 616e 6420 6465   PR title and de
+00003fa0: 7363 7269 7074 696f 6e29 206d 7573 7420  scription) must 
+00003fb0: 6164 6865 7265 2074 6f0a 2020 5b63 6f6e  adhere to.  [con
+00003fc0: 7665 6e74 696f 6e61 6c63 6f6d 6d69 7473  ventionalcommits
+00003fd0: 5d28 6874 7470 733a 2f2f 7777 772e 636f  ](https://www.co
+00003fe0: 6e76 656e 7469 6f6e 616c 636f 6d6d 6974  nventionalcommit
+00003ff0: 732e 6f72 6729 2e0a 2a20 5075 6c6c 2072  s.org)..* Pull r
+00004000: 6571 7565 7374 2062 6f64 7920 7368 6f75  equest body shou
+00004010: 6c64 2064 6573 6372 6962 6520 5f6d 6f74  ld describe _mot
+00004020: 6976 6174 696f 6e5f 2e0a 0a0a 2323 2052  ivation_....## R
+00004030: 6573 6f75 7263 6573 0a2a 205b 4174 6865  esources.* [Athe
+00004040: 6e61 2043 5245 4154 4520 5441 424c 4520  na CREATE TABLE 
+00004050: 4153 5d28 6874 7470 733a 2f2f 646f 6373  AS](https://docs
+00004060: 2e61 7773 2e61 6d61 7a6f 6e2e 636f 6d2f  .aws.amazon.com/
+00004070: 6174 6865 6e61 2f6c 6174 6573 742f 7567  athena/latest/ug
+00004080: 2f63 7265 6174 652d 7461 626c 652d 6173  /create-table-as
+00004090: 2e68 746d 6c29 0a2a 205b 6462 742d 6c61  .html).* [dbt-la
+000040a0: 6273 2f64 6274 2d63 6f72 655d 2868 7474  bs/dbt-core](htt
+000040b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000040c0: 6462 742d 6c61 6273 2f64 6274 2d63 6f72  dbt-labs/dbt-cor
+000040d0: 6529 0a2a 205b 6c61 7567 6869 6e67 6d61  e).* [laughingma
+000040e0: 6e37 3734 332f 5079 4174 6865 6e61 5d28  n7743/PyAthena](
+000040f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004100: 6f6d 2f6c 6175 6768 696e 676d 616e 3737  om/laughingman77
+00004110: 3433 2f50 7941 7468 656e 6129 0a0a 0a23  43/PyAthena)...#
+00004120: 2320 436f 6e74 7269 6275 746f 7273 20e2  # Contributors .
+00004130: 9ca8 0a0a 5468 616e 6b73 2067 6f65 7320  ....Thanks goes 
+00004140: 746f 2074 6865 7365 2077 6f6e 6465 7266  to these wonderf
+00004150: 756c 2070 656f 706c 6520 285b 656d 6f6a  ul people ([emoj
+00004160: 6920 6b65 795d 2868 7474 7073 3a2f 2f61  i key](https://a
+00004170: 6c6c 636f 6e74 7269 6275 746f 7273 2e6f  llcontributors.o
+00004180: 7267 2f64 6f63 732f 656e 2f65 6d6f 6a69  rg/docs/en/emoji
+00004190: 2d6b 6579 2929 3a0a 0a3c 212d 2d20 414c  -key)):..<!-- AL
+000041a0: 4c2d 434f 4e54 5249 4255 544f 5253 2d4c  L-CONTRIBUTORS-L
+000041b0: 4953 543a 5354 4152 5420 2d20 446f 206e  IST:START - Do n
+000041c0: 6f74 2072 656d 6f76 6520 6f72 206d 6f64  ot remove or mod
+000041d0: 6966 7920 7468 6973 2073 6563 7469 6f6e  ify this section
+000041e0: 202d 2d3e 0a3c 212d 2d20 7072 6574 7469   -->.<!-- pretti
+000041f0: 6572 2d69 676e 6f72 652d 7374 6172 7420  er-ignore-start 
+00004200: 2d2d 3e0a 3c21 2d2d 206d 6172 6b64 6f77  -->.<!-- markdow
+00004210: 6e6c 696e 742d 6469 7361 626c 6520 2d2d  nlint-disable --
+00004220: 3e0a 3c74 6162 6c65 3e0a 2020 3c74 626f  >.<table>.  <tbo
+00004230: 6479 3e0a 2020 2020 3c74 723e 0a20 2020  dy>.    <tr>.   
+00004240: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+00004250: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
+00004260: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
+00004270: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004280: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e69  ://github.com/ni
+00004290: 636f 7238 3822 3e3c 696d 6720 7372 633d  cor88"><img src=
+000042a0: 2268 7474 7073 3a2f 2f61 7661 7461 7273  "https://avatars
+000042b0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000042c0: 6e74 2e63 6f6d 2f75 2f36 3237 3835 3437  nt.com/u/6278547
+000042d0: 3f76 3d34 3f73 3d31 3030 2220 7769 6474  ?v=4?s=100" widt
+000042e0: 683d 2231 3030 7078 3b22 2061 6c74 3d22  h="100px;" alt="
+000042f0: 6e69 636f 7238 3822 2f3e 3c62 7220 2f3e  nicor88"/><br />
+00004300: 3c73 7562 3e3c 623e 6e69 636f 7238 383c  <sub><b>nicor88<
+00004310: 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c 6272  /b></sub></a><br
+00004320: 202f 3e3c 6120 6872 6566 3d22 6874 7470   /><a href="http
+00004330: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00004340: 6274 2d61 7468 656e 612f 6462 742d 6174  bt-athena/dbt-at
+00004350: 6865 6e61 2f63 6f6d 6d69 7473 3f61 7574  hena/commits?aut
+00004360: 686f 723d 6e69 636f 7238 3822 2074 6974  hor=nicor88" tit
+00004370: 6c65 3d22 436f 6465 223e f09f 92bb 3c2f  le="Code">....</
+00004380: 613e 203c 6120 6872 6566 3d22 236d 6169  a> <a href="#mai
+00004390: 6e74 656e 616e 6365 2d6e 6963 6f72 3838  ntenance-nicor88
+000043a0: 2220 7469 746c 653d 224d 6169 6e74 656e  " title="Mainten
+000043b0: 616e 6365 223e f09f 9aa7 3c2f 613e 3c2f  ance">....</a></
+000043c0: 7464 3e0a 2020 2020 2020 3c74 6420 616c  td>.      <td al
+000043d0: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
+000043e0: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
+000043f0: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
+00004400: 3d22 6874 7470 733a 2f2f 6a65 7373 6564  ="https://jessed
+00004410: 6f62 6265 6c61 652e 7265 223e 3c69 6d67  obbelae.re"><img
+00004420: 2073 7263 3d22 6874 7470 733a 2f2f 6176   src="https://av
+00004430: 6174 6172 732e 6769 7468 7562 7573 6572  atars.githubuser
+00004440: 636f 6e74 656e 742e 636f 6d2f 752f 3133  content.com/u/13
+00004450: 3532 3937 393f 763d 343f 733d 3130 3022  52979?v=4?s=100"
+00004460: 2077 6964 7468 3d22 3130 3070 783b 2220   width="100px;" 
+00004470: 616c 743d 224a 6573 7365 2044 6f62 6265  alt="Jesse Dobbe
+00004480: 6c61 6572 6522 2f3e 3c62 7220 2f3e 3c73  laere"/><br /><s
+00004490: 7562 3e3c 623e 4a65 7373 6520 446f 6262  ub><b>Jesse Dobb
+000044a0: 656c 6165 7265 3c2f 623e 3c2f 7375 623e  elaere</b></sub>
+000044b0: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
+000044c0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000044d0: 622e 636f 6d2f 6462 742d 6174 6865 6e61  b.com/dbt-athena
+000044e0: 2f64 6274 2d61 7468 656e 612f 6973 7375  /dbt-athena/issu
+000044f0: 6573 3f71 3d61 7574 686f 7225 3341 6a65  es?q=author%3Aje
+00004500: 7373 6564 6f62 6265 6c61 6572 6522 2074  ssedobbelaere" t
+00004510: 6974 6c65 3d22 4275 6720 7265 706f 7274  itle="Bug report
+00004520: 7322 3ef0 9f90 9b3c 2f61 3e20 3c61 2068  s">....</a> <a h
+00004530: 7265 663d 2223 6d61 696e 7465 6e61 6e63  ref="#maintenanc
+00004540: 652d 6a65 7373 6564 6f62 6265 6c61 6572  e-jessedobbelaer
+00004550: 6522 2074 6974 6c65 3d22 4d61 696e 7465  e" title="Mainte
+00004560: 6e61 6e63 6522 3ef0 9f9a a73c 2f61 3e3c  nance">....</a><
+00004570: 2f74 643e 0a20 2020 2020 203c 7464 2061  /td>.      <td a
+00004580: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
+00004590: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
+000045a0: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
+000045b0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000045c0: 622e 636f 6d2f 6c65 6d69 6666 6522 3e3c  b.com/lemiffe"><
+000045d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000045e0: 2f61 7661 7461 7273 2e67 6974 6875 6275  /avatars.githubu
+000045f0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f75  sercontent.com/u
+00004600: 2f37 3438 3737 3732 3f76 3d34 3f73 3d31  /7487772?v=4?s=1
+00004610: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
+00004620: 3b22 2061 6c74 3d22 4c65 6d69 6666 6522  ;" alt="Lemiffe"
+00004630: 2f3e 3c62 7220 2f3e 3c73 7562 3e3c 623e  /><br /><sub><b>
+00004640: 4c65 6d69 6666 653c 2f62 3e3c 2f73 7562  Lemiffe</b></sub
+00004650: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
+00004660: 6566 3d22 2364 6573 6967 6e2d 6c65 6d69  ef="#design-lemi
+00004670: 6666 6522 2074 6974 6c65 3d22 4465 7369  ffe" title="Desi
+00004680: 676e 223e f09f 8ea8 3c2f 613e 3c2f 7464  gn">....</a></td
+00004690: 3e0a 2020 2020 2020 3c74 6420 616c 6967  >.      <td alig
+000046a0: 6e3d 2263 656e 7465 7222 2076 616c 6967  n="center" valig
+000046b0: 6e3d 2274 6f70 2220 7769 6474 683d 2231  n="top" width="1
+000046c0: 342e 3238 2522 3e3c 6120 6872 6566 3d22  4.28%"><a href="
+000046d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000046e0: 6f6d 2f4a 726d 7979 223e 3c69 6d67 2073  om/Jrmyy"><img s
+000046f0: 7263 3d22 6874 7470 733a 2f2f 6176 6174  rc="https://avat
+00004700: 6172 732e 6769 7468 7562 7573 6572 636f  ars.githubuserco
+00004710: 6e74 656e 742e 636f 6d2f 752f 3932 3531  ntent.com/u/9251
+00004720: 3335 333f 763d 343f 733d 3130 3022 2077  353?v=4?s=100" w
+00004730: 6964 7468 3d22 3130 3070 783b 2220 616c  idth="100px;" al
+00004740: 743d 224a c3a9 72c3 a96d 7920 4775 6973  t="J..r..my Guis
+00004750: 656c 696e 222f 3e3c 6272 202f 3e3c 7375  elin"/><br /><su
+00004760: 623e 3c62 3e4a c3a9 72c3 a96d 7920 4775  b><b>J..r..my Gu
+00004770: 6973 656c 696e 3c2f 623e 3c2f 7375 623e  iselin</b></sub>
+00004780: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
+00004790: 663d 2223 6d61 696e 7465 6e61 6e63 652d  f="#maintenance-
+000047a0: 4a72 6d79 7922 2074 6974 6c65 3d22 4d61  Jrmyy" title="Ma
+000047b0: 696e 7465 6e61 6e63 6522 3ef0 9f9a a73c  intenance">....<
+000047c0: 2f61 3e3c 2f74 643e 0a20 2020 2020 203c  /a></td>.      <
+000047d0: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+000047e0: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+000047f0: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+00004800: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00004810: 6974 6875 622e 636f 6d2f 546f 6d6d 6522  ithub.com/Tomme"
+00004820: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00004830: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
+00004840: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00004850: 2f75 2f39 3332 3839 353f 763d 343f 733d  /u/932895?v=4?s=
+00004860: 3130 3022 2077 6964 7468 3d22 3130 3070  100" width="100p
+00004870: 783b 2220 616c 743d 2254 6f6d 222f 3e3c  x;" alt="Tom"/><
+00004880: 6272 202f 3e3c 7375 623e 3c62 3e54 6f6d  br /><sub><b>Tom
+00004890: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
+000048a0: 7220 2f3e 3c61 2068 7265 663d 2223 6d61  r /><a href="#ma
+000048b0: 696e 7465 6e61 6e63 652d 546f 6d6d 6522  intenance-Tomme"
+000048c0: 2074 6974 6c65 3d22 4d61 696e 7465 6e61   title="Maintena
+000048d0: 6e63 6522 3ef0 9f9a a73c 2f61 3e20 3c61  nce">....</a> <a
+000048e0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000048f0: 6974 6875 622e 636f 6d2f 6462 742d 6174  ithub.com/dbt-at
+00004900: 6865 6e61 2f64 6274 2d61 7468 656e 612f  hena/dbt-athena/
+00004910: 636f 6d6d 6974 733f 6175 7468 6f72 3d54  commits?author=T
+00004920: 6f6d 6d65 2220 7469 746c 653d 2243 6f64  omme" title="Cod
+00004930: 6522 3ef0 9f92 bb3c 2f61 3e3c 2f74 643e  e">....</a></td>
+00004940: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00004950: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00004960: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00004970: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00004980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004990: 6d2f 6d61 7474 6961 6d61 7472 6978 223e  m/mattiamatrix">
+000049a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000049b0: 2f2f 6176 6174 6172 732e 6769 7468 7562  //avatars.github
+000049c0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000049d0: 752f 3530 3133 3635 343f 763d 343f 733d  u/5013654?v=4?s=
+000049e0: 3130 3022 2077 6964 7468 3d22 3130 3070  100" width="100p
+000049f0: 783b 2220 616c 743d 224d 6174 7469 6122  x;" alt="Mattia"
+00004a00: 2f3e 3c62 7220 2f3e 3c73 7562 3e3c 623e  /><br /><sub><b>
+00004a10: 4d61 7474 6961 3c2f 623e 3c2f 7375 623e  Mattia</b></sub>
+00004a20: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
+00004a30: 663d 2223 6d61 696e 7465 6e61 6e63 652d  f="#maintenance-
+00004a40: 6d61 7474 6961 6d61 7472 6978 2220 7469  mattiamatrix" ti
+00004a50: 746c 653d 224d 6169 6e74 656e 616e 6365  tle="Maintenance
+00004a60: 223e f09f 9aa7 3c2f 613e 3c2f 7464 3e0a  ">....</a></td>.
+00004a70: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7462      </tr>.  </tb
+00004a80: 6f64 793e 0a3c 2f74 6162 6c65 3e0a 0a3c  ody>.</table>..<
+00004a90: 212d 2d20 6d61 726b 646f 776e 6c69 6e74  !-- markdownlint
+00004aa0: 2d72 6573 746f 7265 202d 2d3e 0a3c 212d  -restore -->.<!-
+00004ab0: 2d20 7072 6574 7469 6572 2d69 676e 6f72  - prettier-ignor
+00004ac0: 652d 656e 6420 2d2d 3e0a 0a3c 212d 2d20  e-end -->..<!-- 
+00004ad0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
+00004ae0: 2d4c 4953 543a 454e 4420 2d2d 3e0a 0a54  -LIST:END -->..T
+00004af0: 6869 7320 7072 6f6a 6563 7420 666f 6c6c  his project foll
+00004b00: 6f77 7320 7468 6520 5b61 6c6c 2d63 6f6e  ows the [all-con
+00004b10: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+00004b20: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+00004b30: 6c2d 636f 6e74 7269 6275 746f 7273 2f61  l-contributors/a
+00004b40: 6c6c 2d63 6f6e 7472 6962 7574 6f72 7329  ll-contributors)
+00004b50: 2073 7065 6369 6669 6361 7469 6f6e 2e20   specification. 
+00004b60: 436f 6e74 7269 6275 7469 6f6e 7320 6f66  Contributions of
+00004b70: 2061 6e79 206b 696e 6420 7765 6c63 6f6d   any kind welcom
+00004b80: 6521 0a                                  e!.
```

### Comparing `dbt-athena-community-1.4.2/dbt_athena_community.egg-info/SOURCES.txt` & `dbt-athena-community-1.4.3/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 dbt/__init__.py
 dbt/adapters/__init__.py
 dbt/adapters/athena/__init__.py
 dbt/adapters/athena/__version__.py
+dbt/adapters/athena/column.py
 dbt/adapters/athena/config.py
 dbt/adapters/athena/connections.py
 dbt/adapters/athena/impl.py
 dbt/adapters/athena/query_headers.py
 dbt/adapters/athena/relation.py
 dbt/adapters/athena/session.py
 dbt/adapters/athena/utils.py
```

### Comparing `dbt-athena-community-1.4.2/pyproject.toml` & `dbt-athena-community-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.2/setup.py` & `dbt-athena-community-1.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 
 from setuptools import find_namespace_packages, setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(this_directory, "README.md")) as f:
+with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 package_name = "dbt-athena-community"
 
 
 # get version from a separate file
 def _get_plugin_version_dict():
@@ -47,11 +47,11 @@
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         # In order to control dbt-core version and package version
         "boto3~=1.26",
         "dbt-core~=1.4.5",
-        "pyathena~=2.23",
+        "pyathena~=2.24",
         "tenacity~=8.2",
     ],
 )
```

