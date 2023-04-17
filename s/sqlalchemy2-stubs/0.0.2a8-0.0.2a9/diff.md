# Comparing `tmp/sqlalchemy2-stubs-0.0.2a8.tar.gz` & `tmp/sqlalchemy2-stubs-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy2-stubs-0.0.2a8.tar", last modified: Fri Jul 30 15:33:29 2021, max compression
+gzip compressed data, was "sqlalchemy2-stubs-0.0.2a9.tar", last modified: Thu Aug 19 21:49:17 2021, max compression
```

## Comparing `sqlalchemy2-stubs-0.0.2a8.tar` & `sqlalchemy2-stubs-0.0.2a9.tar`

### file list

```diff
@@ -1,232 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.223312 sqlalchemy2-stubs-0.0.2a8/
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-07-30 15:33:29.223312 sqlalchemy2-stubs-0.0.2a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-07-30 15:33:29.223312 sqlalchemy2-stubs-0.0.2a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/_typing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      944 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/pyodbc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/databases/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/databases/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5508 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/fdb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14261 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/information_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/pymssql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.203311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12838 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/cymysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/enumerated.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mariadb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/oursql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      718 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/pymysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.207311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10474 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/provision.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.207311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/array.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15054 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/ext.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/psycopg2cffi.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/ranges.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.207311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      573 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/pysqlcipher.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.207311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6229 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/pysybase.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.211311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8721 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/characteristics.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4645 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/create.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10325 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/default.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/interfaces.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/result.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/row.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/strategies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/url.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.211311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/attr.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/legacy.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/registry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/exc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.211311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7843 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/associationproxy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.211311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/engine.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/result.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/session.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/automap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/baked.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/compiler.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.211311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/declarative/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/declarative/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/declarative/extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/horizontal_shard.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/hybrid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/indexable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/instrumentation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mutable.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.215311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/mock_orm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      953 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_b.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_c.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_t.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/orderinglist.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/serializer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.215311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3453 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/engine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.215311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/orm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/orm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/log.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.215311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12238 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/attributes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/clsregistry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/collections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/context.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3288 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/decl_api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/decl_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/dependency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/descriptor_props.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/dynamic.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/evaluator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6198 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/instrumentation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5349 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/interfaces.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/loading.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6012 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/mapper.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/path_registry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/persistence.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7946 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/query.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8465 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/relationships.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/scoping.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22227 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/session.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/state.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8238 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/strategies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5708 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/strategy_options.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      830 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/sync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/unitofwork.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6830 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.219311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/dbapi_proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/impl.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      987 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/processors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.219311 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      819 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/annotation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7242 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/coercions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    28452 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/crud.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7307 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/ddl.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/default_comparator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22598 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/elements.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3867 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/expression.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15448 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/lambdas.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/naming.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10770 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/operators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22148 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22264 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/selectable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    16754 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/sqltypes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    18270 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/traversals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6965 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/type_api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4747 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4271 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/visitors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.223312 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15066 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/_collections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/_concurrency_py3k.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/_preloaded.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6452 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/concurrency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/deprecations.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7962 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/langhelpers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/queue.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      545 2021-07-30 15:33:19.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/topological.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 15:33:29.223312 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-07-30 15:33:29.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7806 2021-07-30 15:33:29.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-30 15:33:29.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-30 15:33:29.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-07-30 15:33:29.000000 sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.094162 sqlalchemy2-stubs-0.0.2a9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-08-19 21:49:17.094162 sqlalchemy2-stubs-0.0.2a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-08-19 21:49:17.094162 sqlalchemy2-stubs-0.0.2a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4882 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/_typing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/pyodbc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/databases/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/databases/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5508 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/fdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.070162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    14261 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/information_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/pymssql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.074163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2541 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12838 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/cymysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/enumerated.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mariadb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/oursql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/pymysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.074163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10474 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/provision.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.074163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1760 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7264 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    15054 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4638 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/psycopg2cffi.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/ranges.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.074163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/pysqlcipher.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.074163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6229 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/pysybase.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.078163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8833 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/characteristics.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4645 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/create.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6960 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10325 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/default.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/interfaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3234 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/row.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/strategies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.078163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/legacy.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4400 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/exc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.078163 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7843 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/associationproxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.082162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5191 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/engine.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/scoping.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8411 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1386 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/automap.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1741 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/baked.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/compiler.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.082162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/declarative/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/declarative/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/declarative/extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/horizontal_shard.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/hybrid.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/indexable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/instrumentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2718 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mutable.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.082162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/mock_orm.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_b.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_t.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/orderinglist.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.082162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3453 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/engine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.082162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/orm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/log.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.086162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12238 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/attributes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/clsregistry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7404 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3288 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/decl_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2271 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/decl_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4614 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/dependency.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/descriptor_props.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/dynamic.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/evaluator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6198 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3259 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/instrumentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5349 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/interfaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/loading.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6012 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/mapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3310 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/path_registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/persistence.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1633 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7946 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8412 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/relationships.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/scoping.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    18829 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8238 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/strategies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5708 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/strategy_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/sync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/unitofwork.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6830 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.086162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/dbapi_proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.090162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/annotation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7242 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/coercions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    28452 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/crud.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7307 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/ddl.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/default_comparator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4359 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    22598 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/elements.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3867 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    15448 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/lambdas.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/naming.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10770 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/operators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    22148 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    22264 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/selectable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    16754 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/sqltypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    18270 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/traversals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6965 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/type_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4747 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4271 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/visitors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2511 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.090162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     8644 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    15066 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/_collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/_concurrency_py3k.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/_preloaded.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6452 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/concurrency.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/deprecations.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7962 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/langhelpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2021-08-19 21:49:05.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/topological.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 21:49:17.094162 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-08-19 21:49:17.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7847 2021-08-19 21:49:17.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-19 21:49:17.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-08-19 21:49:17.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-19 21:49:17.000000 sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/top_level.txt
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/LICENSE` & `sqlalchemy2-stubs-0.0.2a9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/PKG-INFO` & `sqlalchemy2-stubs-0.0.2a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy2-stubs
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: Typing Stubs for SQLAlchemy 1.4
 Home-page: http://www.sqlalchemy.org
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/sqlalchemy2-stubs/
 Platform: UNKNOWN
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/README.rst` & `sqlalchemy2-stubs-0.0.2a9/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/setup.cfg` & `sqlalchemy2-stubs-0.0.2a9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy2-stubs
-version = 0.0.2a8
+version = 0.0.2a9
 description = Typing Stubs for SQLAlchemy 1.4
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = http://www.sqlalchemy.org
 author = Mike Bayer
 author_email = mike_mp@zzzcomputing.com
 license = MIT
@@ -23,23 +23,23 @@
 	Programming Language :: Python :: Implementation :: PyPy
 project_urls = 
 	Issue Tracker=https://github.com/sqlalchemy/sqlalchemy2-stubs/
 
 [options]
 python_requires = >=3.6
 install_requires = 
-	mypy>=0.800
 	typing-extensions>=3.7.4
 
 [options.data_files]
 
 [mypy]
 incremental = True
 strict = True
 warn_unused_ignores = False
+plugins = sqlalchemy.ext.mypy.plugin
 
 [flake8]
 show-source = false
 enable-extensions = G
 ignore = 
 	E203,E305,E711,E712,E721,E722,E741,
 	N801,N802,N806,
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/setup.py` & `sqlalchemy2-stubs-0.0.2a9/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/mxodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/mxodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/connectors/pyodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/connectors/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/information_schema.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/information_schema.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/provision.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/provision.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/pymssql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/pymssql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/cymysql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/cymysql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/dml.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/dml.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/enumerated.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/enumerated.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/oursql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/oursql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/pymysql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/pymysql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/reflection.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/reflection.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/mysql/types.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/mysql/types.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/oracle/provision.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/oracle/provision.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/array.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/array.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/dml.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/dml.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/ext.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/ext.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/hstore.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/hstore.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/json.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/json.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/provision.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/provision.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/postgresql/ranges.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/postgresql/ranges.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/dml.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/dml.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/provision.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/provision.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/dialects/sybase/pysybase.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/dialects/sybase/pysybase.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,25 @@
 _ExecutionOptions: util.immutabledict[Any, Any]
 
 class _ConnectionCallable(Protocol[_T_contra, _T_co]):
     def __call__(
         self, __connection: _T_contra, *args: Any, **kwargs: Any
     ) -> _T_co: ...
 
-class Connection(Connectable):
-    engine: Engine = ...
+class _ConnectionTypingCommon:
+    @property
+    def closed(self) -> bool: ...
+    @property
+    def invalidated(self) -> bool: ...
     dialect: Dialect = ...
+    @property
+    def default_isolation_level(self) -> Any: ...
+
+class Connection(_ConnectionTypingCommon, Connectable):
+    engine: Engine = ...
     should_close_with_result: bool = ...
     dispatch: Any = ...
     def __init__(
         self,
         engine: Engine,
         connection: Optional[_DBAPIConnection] = ...,
         close_with_result: bool = ...,
@@ -53,23 +61,17 @@
     ) -> None: ...
     def schema_for_object(self, obj: Any) -> str: ...
     def __enter__(self: _TConnection) -> _TConnection: ...
     def __exit__(self, type_: Any, value: Any, traceback: Any) -> None: ...
     def execution_options(self: _TConnection, **opt: Any) -> _TConnection: ...
     def get_execution_options(self) -> Dict[str, Any]: ...
     @property
-    def closed(self) -> bool: ...
-    @property
-    def invalidated(self) -> bool: ...
-    @property
     def connection(self) -> _DBAPIConnection: ...
     def get_isolation_level(self) -> Any: ...
     @property
-    def default_isolation_level(self) -> Any: ...
-    @property
     def info(self) -> MutableMapping[Any, Any]: ...
     def connect(self: _TConnection, close_with_result: bool = ...) -> _TConnection: ...  # type: ignore[override]
     def invalidate(self, exception: Optional[Any] = ...) -> None: ...
     def detach(self) -> None: ...
     def begin(self) -> Transaction: ...
     def begin_nested(self) -> NestedTransaction: ...
     def begin_twophase(
@@ -157,42 +159,45 @@
     def __init__(self, connection: Connection) -> None: ...
 
 class TwoPhaseTransaction(RootTransaction):
     xid: str = ...
     def __init__(self, connection: Connection, xid: str) -> None: ...
     def prepare(self) -> None: ...
 
-class Engine(Connectable, log.Identified):
+class _EngineTypingCommon:
     pool: Pool = ...
     url: URL = ...
     dialect: Dialect = ...
     logging_name: Optional[str] = ...
     echo: Optional[Union[bool, Literal["debug"]]] = ...
     hide_parameters: bool = ...
+    @property
+    def name(self) -> str: ...
+    @property
+    def driver(self) -> str: ...
+    def clear_compiled_cache(self) -> None: ...
+    def update_execution_options(self, **opt: Any) -> None: ...
+    def get_execution_options(self) -> Dict[str, Any]: ...
+
+class Engine(_EngineTypingCommon, Connectable, log.Identified):
+    @property
+    def engine(self: _TEngine) -> _TEngine: ...
+    hide_parameters: bool = ...
     def __init__(
         self,
         pool: Pool,
         dialect: Dialect,
         url: URL,
         logging_name: Optional[str] = ...,
         echo: Optional[Union[bool, Literal["debug"]]] = ...,
         query_cache_size: int = ...,
         execution_options: Optional[Dict[str, Any]] = ...,
         hide_parameters: bool = ...,
     ) -> None: ...
-    @property
-    def engine(self: _TEngine) -> _TEngine: ...  # type: ignore[override]
-    def clear_compiled_cache(self) -> None: ...
-    def update_execution_options(self, **opt: Any) -> None: ...
     def execution_options(self, **opt: Any) -> OptionEngine: ...
-    def get_execution_options(self) -> Dict[str, Any]: ...
-    @property
-    def name(self) -> str: ...
-    @property
-    def driver(self) -> str: ...
     def dispose(self) -> None: ...
     class _trans_ctx:
         conn: Connection = ...
         transaction: Transaction = ...
         close_with_result: bool = ...
         def __init__(
             self,
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/characteristics.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/characteristics.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/create.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/create.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/cursor.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/cursor.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/default.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/default.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/events.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/events.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/interfaces.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/mock.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/mock.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/reflection.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/reflection.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/result.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/result.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/row.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/row.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/engine/url.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/engine/url.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/attr.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/attr.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/event/registry.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/event/registry.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/exc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/exc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/associationproxy.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/associationproxy.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -3,9 +3,12 @@
 from .engine import AsyncTransaction as AsyncTransaction
 from .engine import create_async_engine as create_async_engine
 from .events import AsyncConnectionEvents as AsyncConnectionEvents
 from .events import AsyncSessionEvents as AsyncSessionEvents
 from .result import AsyncMappingResult as AsyncMappingResult
 from .result import AsyncResult as AsyncResult
 from .result import AsyncScalarResult as AsyncScalarResult
+from .scoping import async_scoped_session as async_scoped_session
+from .session import async_object_session as async_object_session
+from .session import async_session as async_session
 from .session import AsyncSession as AsyncSession
 from .session import AsyncSessionTransaction as AsyncSessionTransaction
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/engine.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/engine.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -6,36 +6,43 @@
 from typing import NoReturn
 from typing import Optional
 from typing import TypeVar
 
 from .base import ProxyComparable
 from .base import StartableContext
 from .result import AsyncResult
+from ...engine import Dialect
 from ...engine import Result
 from ...engine import Transaction
+from ...engine.base import _ConnectionTypingCommon
+from ...engine.base import _EngineTypingCommon
 from ...future import Connection
 from ...future import Engine
 from ...sql import Executable
 
 _TAsyncConnection = TypeVar("_TAsyncConnection", bound=AsyncConnection)
 _TAsyncTransaction = TypeVar("_TAsyncTransaction", bound=AsyncTransaction)
+_TEngine = TypeVar("_TEngine", bound=AsyncEngine)
 
 def create_async_engine(*arg: Any, **kw: Any) -> AsyncEngine: ...
 
 class AsyncConnectable: ...
 
 class AsyncConnection(
-    ProxyComparable, StartableContext["AsyncConnection"], AsyncConnectable
+    _ConnectionTypingCommon,
+    ProxyComparable,
+    StartableContext["AsyncConnection"],
+    AsyncConnectable,
 ):
     # copied from future.Connection via create_proxy_methods
     @property
     def closed(self) -> bool: ...
     @property
     def invalidated(self) -> bool: ...
-    dialect: Any
+    dialect: Dialect
     @property
     def default_isolation_level(self) -> Any: ...
     # end copied
 
     engine: AsyncEngine = ...
     sync_engine: Engine = ...
     sync_connection: Optional[Connection] = ...
@@ -95,20 +102,17 @@
     def __await__(
         self: _TAsyncConnection,
     ) -> Generator[Any, None, _TAsyncConnection]: ...
     async def __aexit__(
         self, type_: Any, value: Any, traceback: Any
     ) -> None: ...
 
-class AsyncEngine(ProxyComparable, AsyncConnectable):
-    # copied from future.Engine by create_proxy_methods
-    def clear_compiled_cache(self) -> None: ...
-    def update_execution_options(self, **opt: Any) -> None: ...
-    def get_execution_options(self) -> Mapping[Any, Any]: ...
-    # end copied
+class AsyncEngine(_EngineTypingCommon, ProxyComparable, AsyncConnectable):
+    @property
+    def engine(self: _TEngine) -> _TEngine: ...
     class _trans_ctx(StartableContext[AsyncConnection]):
         conn: AsyncConnection = ...
         def __init__(self, conn: AsyncConnection) -> None: ...
         transaction: Any = ...
         async def start(self) -> AsyncConnection: ...
         def __await__(self) -> Generator[Any, None, AsyncConnection]: ...
         async def __aexit__(
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/asyncio/result.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/asyncio/result.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/automap.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/automap.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/baked.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/baked.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/declarative/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/declarative/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/declarative/extensions.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/declarative/extensions.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/horizontal_shard.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/horizontal_shard.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/hybrid.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/hybrid.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/indexable.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/indexable.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/instrumentation.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/instrumentation.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mutable.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mutable.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/mock_orm.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/mock_orm.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_b.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_b.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_c.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_c.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/mypy/plugin_t.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/mypy/plugin_t.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/ext/orderinglist.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/ext/orderinglist.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/future/engine.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/future/engine.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/inspection.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/inspection.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/log.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/log.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/attributes.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/attributes.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/clsregistry.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/clsregistry.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/collections.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/collections.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/context.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/context.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/decl_api.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/decl_api.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/decl_base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/decl_base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/dependency.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/dependency.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/descriptor_props.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/descriptor_props.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/dynamic.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/dynamic.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/evaluator.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/evaluator.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/events.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/events.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/exc.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/exc.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/identity.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/identity.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/instrumentation.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/instrumentation.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/interfaces.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/loading.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/loading.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/mapper.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/mapper.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/path_registry.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/path_registry.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/persistence.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/persistence.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/properties.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/properties.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/query.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/query.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/relationships.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/relationships.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     join_depth: Optional[int]
     omit_join: Optional[Literal[False]]
     local_remote_pairs: Any  # NOTE: not documented
     bake_queries: bool
     load_on_pending: bool
     comparator_factory: Any
     comparator: Any
-    info: MutableMapping[Any, Any]  # NOTE: not set if constructor argument is ``None``
+    info: MutableMapping[Any, Any]
     strategy_key: Tuple[Tuple[str, str]]  # NOTE: not documented
     order_by: Any
     back_populates: Union[None, str]
     backref: Union[None, str, _BackrefResult]
     def __init__(
         self,
         argument: Any,
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/session.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/session.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 from ..engine.base import _ExecutionOptions
 from ..sql import ClauseElement
 from ..sql import Executable
 from ..sql.base import Options
 
 _T = TypeVar("_T")
 _TSession = TypeVar("_TSession", bound=Session)
+_TSessionNoIoTypingCommon = TypeVar(
+    "_TSession", bound=_SessionNoIoTypingCommon
+)
 _TSessionTransaction = TypeVar(
     "_TSessionTransaction", bound=SessionTransaction
 )
 
 _TSharedSessionProtocol = TypeVar(
     "_TSharedSessionProtocol", bound=_SharedSessionProtocol[Any]
 )
@@ -137,23 +140,23 @@
         with_for_update: Optional[
             Union[Literal[True], Mapping[str, Any]]
         ] = ...,
     ) -> None: ...
     def delete(self, instance: Any) -> None: ...
     def get(
         self,
-        entity: Any,
+        entity: Type[_T],
         ident: Any,
         options: Optional[Sequence[Any]] = ...,
         populate_existing: bool = ...,
         with_for_update: Optional[
             Union[Literal[True], Mapping[str, Any]]
         ] = ...,
         identity_token: Optional[Any] = ...,
-    ) -> Any: ...
+    ) -> Optional[_T]: ...
     def merge(self, instance: _T, load: bool = ...) -> _T: ...
     def flush(self, objects: Optional[Collection[Any]] = ...) -> None: ...
     @classmethod
     def close_all(cls) -> None: ...  # NOTE: Deprecated.
 
 class _SessionTransactionProtocol(Protocol):
     nested: bool
@@ -175,132 +178,33 @@
     def close(self, invalidate: bool = ...) -> None: ...
     def __enter__(
         self: _TSessionTransactionProtocol,
     ) -> _TSessionTransactionProtocol: ...
     def __exit__(self, type_: Any, value: Any, traceback: Any) -> None: ...
 
 if sys.version_info >= (3, 0):
-    from typing import Generator
-    from ..ext.asyncio import AsyncEngine, AsyncConnection
+    from ..ext.asyncio.session import _AsyncSessionProtocol
 
     _TSessionMakerType = TypeVar(
         "_TSessionMakerType",
         bound=Union[_SessionProtocol, _AsyncSessionProtocol],
     )
-    _TAsyncSessionTransactionProtocol = TypeVar(
-        "_TAsyncSessionTransactionProtocol",
-        bound=_AsyncSessionTransactionProtocol,
-    )
-    _TAsyncSessionProtocol = TypeVar(
-        "_TAsyncSessionProtocol", bound=_AsyncSessionProtocol
-    )
-    class _AsyncSessionTransactionProtocol(Protocol):
-        @property
-        def is_active(self) -> bool: ...
-        async def commit(
-            self,
-        ) -> Optional[_AsyncSessionTransactionProtocol]: ...
-        async def rollback(
-            self,
-        ) -> Optional[_AsyncSessionTransactionProtocol]: ...
-        async def start(
-            self: _TAsyncSessionTransactionProtocol,
-        ) -> _TAsyncSessionTransactionProtocol: ...
-        def __await__(
-            self: _TAsyncSessionTransactionProtocol,
-        ) -> Generator[Any, None, _TAsyncSessionTransactionProtocol]: ...
-        async def __aenter__(
-            self: _TAsyncSessionTransactionProtocol,
-        ) -> _TAsyncSessionTransactionProtocol: ...
-        async def __aexit__(
-            self, type_: Any, value: Any, traceback: Any
-        ) -> None: ...
-    class _AsyncSessionProtocol(
-        _SharedSessionProtocol[Union[AsyncConnection, AsyncEngine]], Protocol
-    ):
-        async def __aenter__(
-            self: _TAsyncSessionProtocol,
-        ) -> _TAsyncSessionProtocol: ...
-        async def __aexit__(
-            self, type_: Any, value: Any, traceback: Any
-        ) -> None: ...
-        def begin(self) -> _AsyncSessionTransactionProtocol: ...
-        def begin_nested(self) -> _AsyncSessionTransactionProtocol: ...
-        async def rollback(self) -> None: ...
-        async def commit(self) -> None: ...
-        async def connection(self) -> Any: ...
-        async def execute(
-            self,
-            statement: Executable,
-            params: Optional[
-                Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
-            ] = ...,
-            execution_options: _ExecutionOptions = ...,
-            bind_arguments: Optional[_BindArguments] = ...,
-            **kw: Any,
-        ) -> Result: ...
-        async def scalar(
-            self,
-            statement: Executable,
-            params: Optional[
-                Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
-            ] = ...,
-            execution_options: _ExecutionOptions = ...,
-            bind_arguments: Optional[_BindArguments] = ...,
-            **kw: Any,
-        ) -> Any: ...
-        async def close(self) -> None: ...
-        async def refresh(
-            self,
-            instance: Any,
-            attribute_names: Optional[Iterable[str]] = ...,
-            with_for_update: Optional[
-                Union[Literal[True], Mapping[str, Any]]
-            ] = ...,
-        ) -> None: ...
-        async def get(
-            self,
-            entity: Any,
-            ident: Any,
-            options: Optional[Sequence[Any]] = ...,
-            populate_existing: bool = ...,
-            with_for_update: Optional[
-                Union[Literal[True], Mapping[str, Any]]
-            ] = ...,
-            identity_token: Optional[Any] = ...,
-        ) -> Any: ...
-        async def stream(
-            self,
-            statement: Any,
-            params: Optional[
-                Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
-            ] = ...,
-            execution_options: _ExecutionOptions = ...,
-            bind_arguments: Optional[_BindArguments] = ...,
-            **kw: Any,
-        ) -> Any: ...
-        async def delete(self, instance: Any) -> None: ...
-        async def merge(self, instance: _T, load: bool = ...) -> _T: ...
-        async def flush(
-            self, objects: Optional[Collection[Any]] = ...
-        ) -> None: ...
-        @classmethod
-        async def close_all(cls) -> None: ...  # NOTE: Deprecated.
-
 else:
     _TSessionMakerType = TypeVar("_TSessionMakerType", bound=_SessionProtocol)
 
-class _SessionClassMethods:
-    @classmethod
-    def close_all(cls) -> None: ...  # NOTE: Deprecated.
+class _SessionClassMethodNoIoTypingCommon:
     @classmethod
     def identity_key(cls, *args: Any, **kwargs: Any) -> Any: ...
     @classmethod
     def object_session(cls, instance: Any) -> Session: ...
 
+class _SessionClassMethods(_SessionClassMethodNoIoTypingCommon):
+    @classmethod
+    def close_all(cls) -> None: ...  # NOTE: Deprecated.
+
 ACTIVE: util.langhelpers._symbol
 PREPARED: util.langhelpers._symbol
 COMMITTED: util.langhelpers._symbol
 DEACTIVE: util.langhelpers._symbol
 CLOSED: util.langhelpers._symbol
 
 class ORMExecuteState(util.MemoizedSlots):
@@ -382,139 +286,97 @@
     def rollback(
         self, _capture_exception: bool = ..., _to_root: bool = ...
     ) -> Optional[SessionTransaction]: ...
     def close(self, invalidate: bool = ...) -> None: ...
     def __enter__(self: _TSessionTransaction) -> _TSessionTransaction: ...
     def __exit__(self, type_: Any, value: Any, traceback: Any) -> None: ...
 
-class Session(_SessionClassMethods):
+class _SessionNoIoTypingCommon:
+    @property
+    def dirty(self) -> util.IdentitySet[Any]: ...
+    @property
+    def deleted(self) -> util.IdentitySet[Any]: ...
+    @property
+    def new(self) -> util.IdentitySet[Any]: ...
     identity_map: _IdentityMap
-    bind: Optional[Union[Connection, Engine]]
-    future: bool
-    hash_key: int
+    @property
+    def is_active(self) -> bool: ...
     autoflush: bool
-    expire_on_commit: bool
-    enable_baked_queries: bool
-    autocommit: bool
-    twophase: bool
-    def __init__(
-        self,
-        bind: Optional[Union[Connection, Engine]] = ...,
-        autoflush: bool = ...,
-        future: bool = ...,
-        expire_on_commit: bool = ...,
-        autocommit: bool = ...,  # NOTE: Deprecated.
-        twophase: bool = ...,
-        binds: Optional[Mapping[Any, Union[Connection, Engine]]] = ...,
-        enable_baked_queries: bool = ...,
-        info: Optional[MutableMapping[Any, Any]] = ...,
-        query_cls: Optional[
-            Union[Type[Query[Any]], Callable[..., Query[Any]]]
-        ] = ...,
-    ) -> None: ...
-    connection_callable: Any = ...
-    def __enter__(self: _TSession) -> _TSession: ...
-    def __exit__(self, type_: Any, value: Any, traceback: Any) -> None: ...
     @property
-    def transaction(
-        self,
-    ) -> Optional[SessionTransaction]: ...  # NOTE: Deprecated.
-    def in_transaction(self) -> bool: ...
-    def in_nested_transaction(self) -> bool: ...
-    def get_transaction(self) -> Optional[SessionTransaction]: ...
-    def get_nested_transaction(self) -> Optional[SessionTransaction]: ...
+    def no_autoflush(
+        self: _TSessionNoIoTypingCommon,
+    ) -> ContextManager[_TSessionNoIoTypingCommon]: ...
     @util.memoized_property
     def info(self) -> MutableMapping[Any, Any]: ...
+    def __contains__(self, instance: Any) -> bool: ...
+    def __iter__(self) -> Iterator[Any]: ...
+    def add(self, instance: Any, _warn: bool = ...) -> None: ...
+    def add_all(self, instances: Any) -> None: ...
+    def expire(
+        self, instance: Any, attribute_names: Optional[Iterable[str]] = ...
+    ) -> None: ...
+    def expire_all(self) -> None: ...
+    def expunge(self, instance: Any) -> None: ...
+    def expunge_all(self) -> None: ...
+    def get_bind(
+        self,
+        mapper: Optional[Any] = ...,
+        clause: Optional[ClauseElement] = ...,
+        bind: Optional[Union[Connection, Engine]] = ...,
+        _sa_skip_events: Optional[Any] = ...,
+        _sa_skip_for_implicit_returning: bool = ...,
+    ) -> Union[Connection, Engine]: ...
+    def is_modified(
+        self, instance: Any, include_collections: bool = ...
+    ) -> bool: ...
+
+class _SessionTypingCommon(_SessionNoIoTypingCommon):
+    bind: Optional[Union[Connection, Engine]]
+    autocommit: bool
     def begin(
         self,
         subtransactions: bool = ...,  # NOTE: Deprecated.
         nested: bool = ...,
         _subtrans: bool = ...,
     ) -> SessionTransaction: ...
     def begin_nested(self) -> SessionTransaction: ...
-    def rollback(self) -> None: ...
+    def close(self) -> None: ...
     def commit(self) -> None: ...
-    def prepare(self) -> None: ...
     def connection(
         self,
         bind_arguments: Optional[_BindArguments] = ...,
         close_with_result: bool = ...,
         execution_options: _ExecutionOptions = ...,
         **kw: Any,
     ) -> Connection: ...
+    def delete(self, instance: Any) -> None: ...
     def execute(
         self,
         statement: Executable,
         params: Optional[
             Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
         ] = ...,
         execution_options: _ExecutionOptions = ...,
         bind_arguments: Optional[_BindArguments] = ...,
         _parent_execute_state: Optional[Any] = ...,
         _add_event: Optional[Any] = ...,
         **kw: Any,
     ) -> Result: ...
-    def scalar(
-        self,
-        statement: Executable,
-        params: Optional[
-            Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
-        ] = ...,
-        execution_options: _ExecutionOptions = ...,
-        bind_arguments: Optional[_BindArguments] = ...,
-        **kw: Any,
-    ) -> Any: ...
-    def close(self) -> None: ...
-    def invalidate(self) -> None: ...
-    def expunge_all(self) -> None: ...
-    def bind_mapper(self, mapper: Any, bind: Any) -> None: ...
-    def bind_table(self, table: Any, bind: Any) -> None: ...
-    def get_bind(
-        self,
-        mapper: Optional[Any] = ...,
-        clause: Optional[ClauseElement] = ...,
-        bind: Optional[Union[Connection, Engine]] = ...,
-        _sa_skip_events: Optional[Any] = ...,
-        _sa_skip_for_implicit_returning: bool = ...,
-    ) -> Union[Connection, Engine]: ...
-    def query(self, *entities: Any, **kwargs: Any) -> Query[Any]: ...
-    @property
-    def no_autoflush(self: _TSession) -> ContextManager[_TSession]: ...
-    def refresh(
-        self,
-        instance: Any,
-        attribute_names: Optional[Iterable[str]] = ...,
-        with_for_update: Optional[
-            Union[Literal[True], Mapping[str, Any]]
-        ] = ...,
-    ) -> None: ...
-    def expire_all(self) -> None: ...
-    def expire(
-        self, instance: Any, attribute_names: Optional[Iterable[str]] = ...
-    ) -> None: ...
-    def expunge(self, instance: Any) -> None: ...
-    def add(self, instance: Any, _warn: bool = ...) -> None: ...
-    def add_all(self, instances: Any) -> None: ...
-    def delete(self, instance: Any) -> None: ...
+    def flush(self, objects: Optional[Collection[Any]] = ...) -> None: ...
     def get(
         self,
-        entity: Any,
+        entity: Type[_T],
         ident: Any,
         options: Optional[Sequence[Any]] = ...,
         populate_existing: bool = ...,
         with_for_update: Optional[
             Union[Literal[True], Mapping[str, Any]]
         ] = ...,
         identity_token: Optional[Any] = ...,
-    ) -> Any: ...
-    def merge(self, instance: _T, load: bool = ...) -> _T: ...
-    def enable_relationship_loading(self, obj: Any) -> None: ...
-    def __contains__(self, instance: Any) -> bool: ...
-    def __iter__(self) -> Iterator[Any]: ...
-    def flush(self, objects: Optional[Collection[Any]] = ...) -> None: ...
+    ) -> Optional[_T]: ...
     def bulk_save_objects(
         self,
         objects: Sequence[Any],
         return_defaults: bool = ...,
         update_changed_only: bool = ...,
         preserve_order: bool = ...,
     ) -> None: ...
@@ -524,25 +386,79 @@
         mappings: Sequence[Mapping[str, Any]],
         return_defaults: bool = ...,
         render_nulls: bool = ...,
     ) -> None: ...
     def bulk_update_mappings(
         self, mapper: Any, mappings: Sequence[Mapping[str, Any]]
     ) -> None: ...
-    def is_modified(
-        self, instance: Any, include_collections: bool = ...
-    ) -> bool: ...
-    @property
-    def is_active(self) -> bool: ...
-    @property
-    def dirty(self) -> util.IdentitySet[Any]: ...
-    @property
-    def deleted(self) -> util.IdentitySet[Any]: ...
+    def merge(self, instance: _T, load: bool = ...) -> _T: ...
+    def query(self, *entities: Any, **kwargs: Any) -> Query[Any]: ...
+    def refresh(
+        self,
+        instance: Any,
+        attribute_names: Optional[Iterable[str]] = ...,
+        with_for_update: Optional[
+            Union[Literal[True], Mapping[str, Any]]
+        ] = ...,
+    ) -> None: ...
+    def rollback(self) -> None: ...
+    def scalar(
+        self,
+        statement: Executable,
+        params: Optional[
+            Union[Mapping[str, Any], Sequence[Mapping[str, Any]]]
+        ] = ...,
+        execution_options: _ExecutionOptions = ...,
+        bind_arguments: Optional[_BindArguments] = ...,
+        **kw: Any,
+    ) -> Any: ...
+
+class _SessionInTransactionTypingCommon:
+    def in_transaction(self) -> bool: ...
+    def in_nested_transaction(self) -> bool: ...
+
+class Session(
+    _SessionTypingCommon,
+    _SessionInTransactionTypingCommon,
+    _SessionClassMethods,
+):
+    future: bool
+    hash_key: int
+    expire_on_commit: bool
+    enable_baked_queries: bool
+    twophase: bool
+    def __init__(
+        self,
+        bind: Optional[Union[Connection, Engine]] = ...,
+        autoflush: bool = ...,
+        future: bool = ...,
+        expire_on_commit: bool = ...,
+        autocommit: bool = ...,  # NOTE: Deprecated.
+        twophase: bool = ...,
+        binds: Optional[Mapping[Any, Union[Connection, Engine]]] = ...,
+        enable_baked_queries: bool = ...,
+        info: Optional[MutableMapping[Any, Any]] = ...,
+        query_cls: Optional[
+            Union[Type[Query[Any]], Callable[..., Query[Any]]]
+        ] = ...,
+    ) -> None: ...
+    connection_callable: Any = ...
+    def __enter__(self: _TSession) -> _TSession: ...
+    def __exit__(self, type_: Any, value: Any, traceback: Any) -> None: ...
     @property
-    def new(self) -> util.IdentitySet[Any]: ...
+    def transaction(
+        self,
+    ) -> Optional[SessionTransaction]: ...  # NOTE: Deprecated.
+    def get_transaction(self) -> Optional[SessionTransaction]: ...
+    def get_nested_transaction(self) -> Optional[SessionTransaction]: ...
+    def prepare(self) -> None: ...
+    def invalidate(self) -> None: ...
+    def bind_mapper(self, mapper: Any, bind: Any) -> None: ...
+    def bind_table(self, table: Any, bind: Any) -> None: ...
+    def enable_relationship_loading(self, obj: Any) -> None: ...
 
 class sessionmaker(_SessionClassMethods, Generic[_TSessionMakerType]):
     kw: Mapping[str, Any]
     class_: Type[_TSessionMakerType]
     if sys.version_info >= (3, 0):
         @overload
         def __init__(
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/state.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/state.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/strategies.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/strategies.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/strategy_options.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/sync.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/sync.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/unitofwork.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/unitofwork.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/orm/util.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/orm/util.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         logging_name: Optional[Any] = ...,
         reset_on_return: bool = ...,
         events: Optional[Any] = ...,
         dialect: Optional[Any] = ...,
         pre_ping: bool = ...,
         _dispatch: Optional[Any] = ...,
     ) -> None: ...
-    def recreate(self) -> None: ...
+    def recreate(self) -> Pool: ...
     def dispose(self) -> None: ...
     def connect(self): ...
-    def status(self) -> None: ...
+    def status(self) -> str: ...
 
 class _ConnectionRecord:
     finalize_callback: Any = ...
     def __init__(self, pool: Any, connect: bool = ...) -> None: ...
     fresh: bool = ...
     fairy_ref: Any = ...
     starttime: Any = ...
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/dbapi_proxy.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/dbapi_proxy.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/events.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/events.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/pool/impl.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/pool/impl.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/processors.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/processors.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/schema.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/schema.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/annotation.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/annotation.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/base.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/base.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/coercions.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/coercions.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/compiler.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/crud.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/crud.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/ddl.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/ddl.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/dml.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/dml.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/elements.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/elements.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/events.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/events.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/expression.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/expression.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/functions.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/functions.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/lambdas.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/lambdas.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/operators.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/operators.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/roles.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/roles.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/schema.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/selectable.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/selectable.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/sqltypes.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/sqltypes.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/traversals.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/traversals.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/type_api.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/type_api.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/util.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/util.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/sql/visitors.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/sql/visitors.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/types.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/__init__.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/_collections.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/_collections.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/_concurrency_py3k.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/_concurrency_py3k.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/compat.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/compat.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/concurrency.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/deprecations.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/deprecations.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/langhelpers.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/langhelpers.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/queue.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/queue.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy-stubs/util/topological.pyi` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy-stubs/util/topological.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/PKG-INFO` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy2-stubs
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: Typing Stubs for SQLAlchemy 1.4
 Home-page: http://www.sqlalchemy.org
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/sqlalchemy2-stubs/
 Platform: UNKNOWN
```

### Comparing `sqlalchemy2-stubs-0.0.2a8/sqlalchemy2_stubs.egg-info/SOURCES.txt` & `sqlalchemy2-stubs-0.0.2a9/sqlalchemy2_stubs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 sqlalchemy-stubs/ext/serializer.pyi
 sqlalchemy-stubs/ext/asyncio/__init__.pyi
 sqlalchemy-stubs/ext/asyncio/base.pyi
 sqlalchemy-stubs/ext/asyncio/engine.pyi
 sqlalchemy-stubs/ext/asyncio/events.pyi
 sqlalchemy-stubs/ext/asyncio/exc.pyi
 sqlalchemy-stubs/ext/asyncio/result.pyi
+sqlalchemy-stubs/ext/asyncio/scoping.pyi
 sqlalchemy-stubs/ext/asyncio/session.pyi
 sqlalchemy-stubs/ext/declarative/__init__.pyi
 sqlalchemy-stubs/ext/declarative/extensions.pyi
 sqlalchemy-stubs/ext/mypy/__init__.pyi
 sqlalchemy-stubs/ext/mypy/mock_orm.pyi
 sqlalchemy-stubs/ext/mypy/plugin.pyi
 sqlalchemy-stubs/ext/mypy/plugin_b.pyi
```

