# Comparing `tmp/diengine-connect-0.0.3.tar.gz` & `tmp/diengine-connect-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diengine-connect-0.0.3.tar", last modified: Mon Apr 17 06:27:28 2023, max compression
+gzip compressed data, was "diengine-connect-0.1.7.tar", last modified: Thu Apr 13 02:38:50 2023, max compression
```

## Comparing `diengine-connect-0.0.3.tar` & `diengine-connect-0.1.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.888955 diengine-connect-0.0.3/
--rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-04-17 04:12:26.000000 diengine-connect-0.0.3/LICENSE
--rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-04-17 06:27:28.888814 diengine-connect-0.0.3/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)      313 2023-04-17 02:48:32.000000 diengine-connect-0.0.3/README.md
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.876792 diengine-connect-0.0.3/diengine_connect/
--rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-04-17 06:27:27.000000 diengine-connect-0.0.3/diengine_connect/VERSION
--rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.878260 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/
--rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.878892 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4768 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)    13573 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.879468 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1593 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7509 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3512 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.879990 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/sql/preparer.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.880438 diengine-connect-0.0.3/diengine_connect/cc_superset/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/cc_superset/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1226 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/cc_superset/datatypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-04-17 02:48:32.000000 diengine-connect-0.0.3/diengine_connect/cc_superset/engine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1987 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/common.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.882535 diengine-connect-0.0.3/diengine_connect/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)    14598 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)     9226 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/container.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2548 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/datatypes/format.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4643 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/network.py
--rw-r--r--   0 xushihao   (501) staff       (20)    11138 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/numeric.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2326 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/datatypes/registry.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3717 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/special.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5926 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/string.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/datatypes/temporal.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.883221 diengine-connect-0.0.3/diengine_connect/dbapi/
--rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/dbapi/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/dbapi/connection.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/dbapi/cursor.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.888411 diengine-connect-0.0.3/diengine_connect/driver/
--rw-r--r--   0 xushihao   (501) staff       (20)     6640 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/buffer.py
--rw-r--r--   0 xushihao   (501) staff       (20)    34594 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/driver/client.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6051 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/common.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/compression.py
--rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/constants.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/context.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/ctypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/dataconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)      817 2023-04-17 02:48:32.000000 diengine-connect-0.0.3/diengine_connect/driver/ddl.py
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/diengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2832 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/exceptions.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7170 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/extras.py
--rw-r--r--   0 xushihao   (501) staff       (20)    18856 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/httpclient.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6474 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/httputil.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6974 2023-04-17 02:33:27.000000 diengine-connect-0.0.3/diengine_connect/driver/insert.py
--rw-r--r--   0 xushihao   (501) staff       (20)      726 2023-04-17 03:21:05.000000 diengine-connect-0.0.3/diengine_connect/driver/models.py
--rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/npconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/npquery.py
--rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/options.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5706 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/parser.py
--rw-r--r--   0 xushihao   (501) staff       (20)    19939 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/query.py
--rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/tools.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5383 2023-04-17 03:27:42.000000 diengine-connect-0.0.3/diengine_connect/driver/transform.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driver/types.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.888639 diengine-connect-0.0.3/diengine_connect/driverc/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/driverc/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/entry_points.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/diengine_connect/json_impl.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-17 06:27:28.877619 diengine-connect-0.0.3/diengine_connect.egg-info/
--rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)     2554 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/SOURCES.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/dependency_links.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/entry_points.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/not-zip-safe
--rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/requires.txt
--rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-04-17 06:27:28.000000 diengine-connect-0.0.3/diengine_connect.egg-info/top_level.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/pyproject.toml
--rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-04-17 06:27:28.889001 diengine-connect-0.0.3/setup.cfg
--rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-04-14 12:56:07.000000 diengine-connect-0.0.3/setup.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212683 diengine-connect-0.1.7/
+-rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/LICENSE
+-rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-13 02:38:50.212551 diengine-connect-0.1.7/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)      315 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/README.md
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.204287 diengine-connect-0.1.7/diengine_connect/
+-rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-04-13 02:38:28.000000 diengine-connect-0.1.7/diengine_connect/VERSION
+-rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.205608 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/
+-rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206116 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4792 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    13591 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206484 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1599 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7513 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3512 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206860 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/preparer.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.207197 diengine-connect-0.1.7/diengine_connect/cc_superset/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1228 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/datatypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8404 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/engine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1989 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/common.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.208631 diengine-connect-0.1.7/diengine_connect/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    14636 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     9238 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/container.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2558 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/format.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4649 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/network.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    11148 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/numeric.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2352 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/registry.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3725 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/special.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5932 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/string.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8402 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/temporal.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.209002 diengine-connect-0.1.7/diengine_connect/dbapi/
+-rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/connection.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/cursor.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212275 diengine-connect-0.1.7/diengine_connect/driver/
+-rw-r--r--   0 xushihao   (501) staff       (20)     6674 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/buffer.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    34700 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/client.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6057 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/common.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/compression.py
+-rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/constants.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/context.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1316 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/ctypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/dataconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      823 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/ddl.py
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/diengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2842 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/exceptions.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7194 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/extras.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    18878 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/httpclient.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6476 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/httputil.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6980 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/insert.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      732 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/models.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/npconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/npquery.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/options.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5718 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/parser.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    19957 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/query.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/tools.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5385 2023-04-13 02:27:50.000000 diengine-connect-0.1.7/diengine_connect/driver/transform.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/types.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212399 diengine-connect-0.1.7/diengine_connect/driverc/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driverc/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/entry_points.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/json_impl.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.205120 diengine-connect-0.1.7/diengine_connect.egg-info/
+-rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)     2554 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/entry_points.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/not-zip-safe
+-rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/requires.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/top_level.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/pyproject.toml
+-rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-04-13 02:38:50.212731 diengine-connect-0.1.7/setup.cfg
+-rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/setup.py
```

### Comparing `diengine-connect-0.0.3/LICENSE` & `diengine-connect-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/PKG-INFO` & `diengine-connect-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.0.3
+Version: 0.1.7
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
-        A suite of Python packages for connecting Python to Diengine:
+        A suite of Python packages for connecting Python to ClickHouse:
         * Pandas DataFrames
         * Numpy Arrays
         * PyArrow Tables
         * SQLAlchemy 1.3 and 1.4 (limited feature set)
         * Apache Superset 1.4+
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/base.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import logging
 from typing import Dict, Type
 
 from sqlalchemy.exc import CompileError
 
-from diengine_connect.datatypes.base import DiengineType, TypeDef, EMPTY_TYPE_DEF
+from diengine_connect.datatypes.base import ClickHouseType, TypeDef, EMPTY_TYPE_DEF
 from diengine_connect.datatypes.registry import parse_name, type_map
 from diengine_connect.driver.query import format_query_value
 
 logger = logging.getLogger(__name__)
 
 
 class ChSqlaType:
     """
-    A SQLAlchemy TypeEngine that wraps a DiengineType.  We don't extend TypeEngine directly, instead all concrete
+    A SQLAlchemy TypeEngine that wraps a ClickHouseType.  We don't extend TypeEngine directly, instead all concrete
     subclasses will inherit from TypeEngine.
     """
-    ch_type: DiengineType = None
+    ch_type: ClickHouseType = None
     generic_type: None
     _ch_type_cls = None
     _instance = None
     _instance_cache: Dict[TypeDef, 'ChSqlaType'] = None
 
     def __init_subclass__(cls):
         """
-        Registers ChSqla type in the type map and sets the underlying DiengineType class to use to initialize
+        Registers ChSqla type in the type map and sets the underlying ClickHouseType class to use to initialize
         ChSqlaType instances
         """
         base = cls.__name__
         if not cls._ch_type_cls:
             try:
                 cls._ch_type_cls = type_map[base]
             except KeyError:
-                logger.warning('Attempted to register SQLAlchemy type without corresponding Diengine Type')
+                logger.warning('Attempted to register SQLAlchemy type without corresponding ClickHouse Type')
                 return
         schema_types.append(base)
         sqla_type_map[base] = cls
         cls._instance_cache = {}
 
     @classmethod
     def build(cls, type_def: TypeDef):
@@ -44,29 +44,29 @@
         :param type_def: -- TypeDef tuple that defines arguments for this instance
         :return: Shared instance of a configured ChSqlaType
         """
         return cls._instance_cache.setdefault(type_def, cls(type_def=type_def))
 
     def __init__(self, type_def: TypeDef = EMPTY_TYPE_DEF):
         """
-        Basic constructor that does nothing but set the wrapped DiengineType.  It is overridden in some cases
+        Basic constructor that does nothing but set the wrapped ClickHouseType.  It is overridden in some cases
         to add specific SqlAlchemy behavior when constructing subclasses "by hand", in which case the type_def
         parameter is normally set to None and other keyword parameters used for construction
-        :param type_def: TypeDef tuple used to build the underlying DiengineType.  This is normally populated by the
+        :param type_def: TypeDef tuple used to build the underlying ClickHouseType.  This is normally populated by the
         parse_name function
         """
         self.type_def = type_def
         self.ch_type = self._ch_type_cls.build(type_def)
 
     @property
     def name(self):
         return self.ch_type.name
 
     @name.setter
-    def name(self, name):  # Keep SQLAlchemy from overriding our Diengine name
+    def name(self, name):  # Keep SQLAlchemy from overriding our ClickHouse name
         pass
 
     @property
     def nullable(self):
         return self.ch_type.nullable
 
     @property
@@ -97,15 +97,15 @@
         confusing.
         """
         return format_query_value
 
     def _compiler_dispatch(self, _visitor, **_):
         """
         Override for the SqlAlchemy TypeEngine _compiler_dispatch method to sidestep unnecessary layers and complexity
-        when generating the type name.  The underlying DiengineType generates the correct name
+        when generating the type name.  The underlying ClickHouseType generates the correct name
         :return: Name generated by the underlying driver.
         """
         return self.name
 
 
 class CaseInsensitiveDict(dict):
     def __setitem__(self, key, value):
@@ -117,19 +117,19 @@
 
 sqla_type_map: Dict[str, Type[ChSqlaType]] = CaseInsensitiveDict()
 schema_types = []
 
 
 def sqla_type_from_name(name: str) -> ChSqlaType:
     """
-    Factory function to convert a Diengine type name to the appropriate ChSqlaType
-    :param name: Name returned from Diengine using Native protocol or WithNames format
+    Factory function to convert a ClickHouse type name to the appropriate ChSqlaType
+    :param name: Name returned from ClickHouse using Native protocol or WithNames format
     :return: ChSqlaType
     """
     base, name, type_def = parse_name(name)
     try:
         type_cls = sqla_type_map[base]
     except KeyError:
-        err_str = f'Unrecognized Diengine type base: {base} name: {name}'
+        err_str = f'Unrecognized ClickHouse type base: {base} name: {name}'
         logger.error(err_str)
         raise CompileError(err_str) from KeyError
     return type_cls.build(type_def)
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,26 +86,26 @@
     dec_size = 0
 
     def __init__(self, precision: int = 0, scale: int = 0, type_def: TypeDef = None):
         """
         Construct either with precision and scale (for DDL), or a TypeDef with those values (by name)
         :param precision:  Number of digits the Decimal
         :param scale: Digits after the decimal point
-        :param type_def: Parsed type def from Diengine arguments
+        :param type_def: Parsed type def from ClickHouse arguments
         """
         if type_def:
             if self.dec_size:
                 precision = decimal_prec[self.dec_size]
                 scale = type_def.values[0]
             else:
                 precision = 0;
                 scale = 0;
                 # precision, scale = type_def.values
         elif not precision or scale < 0 or scale > precision:
-            raise ArgumentError('Invalid precision or scale for Diengine Decimal type')
+            raise ArgumentError('Invalid precision or scale for ClickHouse Decimal type')
         else:
             type_def = TypeDef(values=(precision, scale))
         ChSqlaType.__init__(self, type_def)
         Numeric.__init__(self, precision, scale)
 
 
 # pylint: disable=duplicate-code
@@ -128,15 +128,15 @@
 class Enum(ChSqlaType, UserDefinedType):
     _size = 16
     python_type = str
 
     def __init__(self, enum: Type[PyEnum] = None, keys: Sequence[str] = None, values: Sequence[int] = None,
                  type_def: TypeDef = None):
         """
-        Construct a Diengine enum either from a Python Enum or parallel lists of keys and value.  Note that
+        Construct a ClickHouse enum either from a Python Enum or parallel lists of keys and value.  Note that
         Python enums do not support empty strings as keys, so the alternate keys/values must be used in that case
         :param enum: Python enum to convert
         :param keys: List of string keys
         :param values: List of integer values
         :param type_def: TypeDef from parse_name function
         """
         if not type_def:
@@ -152,23 +152,23 @@
             type_def = TypeDef(keys=tuple(keys), values=tuple(values))
         super().__init__(type_def)
 
     @classmethod
     def _validate(cls, keys: Sequence, values: Sequence):
         bad_key = next((x for x in keys if not isinstance(x, str)), None)
         if bad_key:
-            raise ArgumentError(f'Diengine enum key {bad_key} is not a string')
+            raise ArgumentError(f'ClickHouse enum key {bad_key} is not a string')
         bad_value = next((x for x in values if not isinstance(x, int)), None)
         if bad_value:
-            raise ArgumentError(f'Diengine enum value {bad_value} is not an integer')
+            raise ArgumentError(f'ClickHouse enum value {bad_value} is not an integer')
         value_min = -(2 ** (cls._size - 1))
         value_max = 2 ** (cls._size - 1) - 1
         bad_value = next((x for x in values if x < value_min or x > value_max), None)
         if bad_value:
-            raise ArgumentError(f'Diengine enum value {bad_value} is out of range')
+            raise ArgumentError(f'Clickhouse enum value {bad_value} is out of range')
 
 
 class Enum8(Enum):
     _size = 8
     _ch_type_cls = ChEnum8
 
 
@@ -207,15 +207,15 @@
 class Date32(ChSqlaType, SqlaDate):
     pass
 
 
 class DateTime(ChSqlaType, SqlaDateTime):
     def __init__(self, tz: str = None, type_def: TypeDef = None):
         """
-        Date time constructor with optional diengine timezone parameter if not constructed with TypeDef
+        Date time constructor with optional ClickHouse timezone parameter if not constructed with TypeDef
         :param tz: Timezone string as defined in pytz
         :param type_def: TypeDef from parse_name function
         """
         if not type_def:
             if tz:
                 pytz.timezone(tz)
                 type_def = TypeDef(values=(f"'{tz}'",))
@@ -225,27 +225,27 @@
         SqlaDateTime.__init__(self)
 
 
 class DateTime64(ChSqlaType, SqlaDateTime):
     def __init__(self, precision: int = None, tz: str = None, type_def: TypeDef = None):
         """
         Date time constructor with precision and timezone parameters if not constructed with TypeDef
-        :param precision:   Usually 3/6/9 for mill/micro/nansecond precision on diengine side
+        :param precision:   Usually 3/6/9 for mill/micro/nansecond precision on ClickHouse side
         :param tz: Timezone string as defined in pytz
         :param type_def: TypeDef from parse_name function
         """
         if not type_def:
             if tz:
                 pytz.timezone(tz)
                 type_def = TypeDef(values=(precision, f"'{tz}'"))
             else:
                 type_def = TypeDef(values=(precision,))
         prec = type_def.values[0] if len(type_def.values) else None
         if not isinstance(prec, int) or prec < 0 or prec > 9:
-            raise ArgumentError(f'Invalid precision value {prec} for diengine DateTime64')
+            raise ArgumentError(f'Invalid precision value {prec} for ClickHouse DateTime64')
         ChSqlaType.__init__(self, type_def)
         SqlaDateTime.__init__(self)
 
 
 class Nullable:
     """
     Class "wrapper" to use in DDL construction.  It is never actually initialized but instead creates the "wrapped"
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/custom.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     SqlAlchemy DDL statement that is essentially an alternative to the built in CreateSchema DDL class
     """
     # pylint: disable-msg=too-many-arguments
     def __init__(self, name: str, engine: str = None, zoo_path: str = None, shard_name: str = '{shard}',
                  replica_name: str = '{replica}'):
         """
         :param name: Database name
-        :param engine: Database Diengine engine type
-        :param zoo_path: Diengine zookeeper path for Replicated database engine
-        :param shard_name: Diengine shard name for Replicated database engine
+        :param engine: Database ClickHouse engine type
+        :param zoo_path: ClickHouse zookeeper path for Replicated database engine
+        :param shard_name: Clickhouse shard name for Replicated database engine
         :param replica_name: Replica name for Replicated database engine
         """
         if engine and engine not in ('Ordinary', 'Atomic', 'Lazy', 'Replicated'):
             raise ArgumentError(f'Unrecognized engine type {engine}')
         stmt = f'CREATE DATABASE {quote_identifier(name)}'
         if engine:
             stmt += f' Engine {engine}'
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/ddl/tableengine.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if isinstance(value, (tuple, list)):
         return f" {v} ({','.join(value)})"
     return f'{v} {value}'
 
 
 class TableEngine(SchemaEventTarget, Visitable):
     """
-    SqlAlchemy Schema element to support Diengine table engines.  At the moment provides no real
+    SqlAlchemy Schema element to support ClickHouse table engines.  At the moment provides no real
     functionality other than the CREATE TABLE argument string
     """
     arg_names = ()
     quoted_args = set()
     optional_args = set()
     eng_params = ()
 
@@ -216,15 +216,15 @@
         if not order_by and not primary_key:
             raise ArgumentError(None, 'Either PRIMARY KEY or ORDER BY must be specified')
         super().__init__(locals())
 
 
 def build_engine(full_engine: str) -> Optional[TableEngine]:
     """
-    Factory function to create TableEngine class from Diengine full_engine expression
+    Factory function to create TableEngine class from ClickHouse full_engine expression
     :param full_engine
     :return: TableEngine DDL element
     """
     if not full_engine:
         return None
     name = full_engine.split(' ')[0].split('(')[0]
     try:
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/dialect.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/inspector.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_superset/datatypes.py` & `diengine-connect-0.1.7/diengine_connect/cc_superset/datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     (r'^DATE', GenericDataType.TEMPORAL),
     (r'^BOOL', GenericDataType.BOOLEAN)
 )
 
 
 def configure_types():
     """
-    Monkey patch the Superset generic_type onto the diengine type, also set defaults for certain type formatting to be
+    Monkey patch the Superset generic_type onto the clickhouse type, also set defaults for certain type formatting to be
     better compatible with superset
     """
     set_default_formats('FixedString', 'string',
                         'IPv*', 'string',
                         'UInt64', 'signed',
                         'UUID', 'string',
                         '*Int256', 'string',
```

### Comparing `diengine-connect-0.0.3/diengine_connect/cc_superset/engine.py` & `diengine-connect-0.1.7/diengine_connect/cc_superset/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 from superset.models.core import Database
 
 from diengine_connect import driver_name
 from diengine_connect.common import set_setting
 from diengine_connect.driver import default_port
 from diengine_connect.cc_sqlalchemy.datatypes.base import sqla_type_from_name
 from diengine_connect.cc_superset.datatypes import configure_types
-from diengine_connect.driver.exceptions import DiengineError
+from diengine_connect.driver.exceptions import ClickHouseError
 
 logger = logging.getLogger(__name__)
 
 configure_types()
 set_setting('product_name', f"superset/{current_app.config.get('VERSION_STRING', 'dev')}")
 
 
-class DiengineParametersSchema(Schema):
+class ClickHouseParametersSchema(Schema):
     username = fields.String(allow_none=True, description=__('Username'))
     password = fields.String(allow_none=True, description=__('Password'))
     host = fields.String(required=True, description=__('Hostname or IP address'))
     port = fields.Integer(allow_none=True, description=__('Database port'), validate=Range(min=0, max=65535), )
     database = fields.String(allow_none=True, description=__('Database name'))
     encryption = fields.Boolean(default=True, description=__('Use an encrypted connection to the database'))
     query = fields.Dict(keys=fields.Str(), values=fields.Raw(), description=__('Additional parameters'))
@@ -64,15 +64,15 @@
         'P1W': 'toMonday(toDateTime({col}))',
         'P1M': 'toStartOfMonth(toDateTime({col}))',
         'P3M': 'toStartOfQuarter(toDateTime({col}))',
         'P1Y': 'toStartOfYear(toDateTime({col}))',
     }
 
     sqlalchemy_uri_placeholder = 'dienginedb://user:password@host[:port][/dbname][?secure=value&=value...]'
-    parameters_schema = DiengineParametersSchema()
+    parameters_schema = ClickHouseParametersSchema()
     encryption_parameters = {'secure': 'true'}
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
         return '{col}'
 
     @classmethod
@@ -102,15 +102,15 @@
             return cls._function_names
         try:
             names = database.get_df(
                 'SELECT name FROM system.functions UNION ALL ' +
                 'SELECT name FROM system.table_functions LIMIT 10000')['name'].tolist()
             cls._function_names = names
             return names
-        except DiengineError:
+        except ClickHouseError:
             logger.exception('Error retrieving system.functions')
             return []
 
     @classmethod
     def get_datatype(cls, type_code: str) -> str:
         return type_code
```

### Comparing `diengine-connect-0.0.3/diengine_connect/common.py` & `diengine-connect-0.1.7/diengine_connect/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def build_client_name(client_name: str):
     product_name = get_setting('product_name')
     product_name = product_name.strip() + ' ' if product_name else ''
     client_name = client_name.strip() + ' ' if client_name else ''
     py_version = sys.version.split(' ', maxsplit=1)[0]
-    return f'{client_name}{product_name}diengine-connect/{version()} (lv:py/{py_version}; os:{sys.platform})'
+    return f'{client_name}{product_name}clickhouse-connect/{version()} (lv:py/{py_version}; os:{sys.platform})'
 
 
 def get_setting(name: str):
     setting = _common_settings.get(name)
     if setting is None:
         raise ProgrammingError(f'Unrecognized common setting {name}')
     return setting.value if setting.value is not None else setting.default
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/base.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 logger = logging.getLogger(__name__)
 ch_read_formats = {}
 ch_write_formats = {}
 
 
 class TypeDef(NamedTuple):
     """
-    Immutable tuple that contains all additional information needed to construct a particular DiengineType
+    Immutable tuple that contains all additional information needed to construct a particular ClickHouseType
     """
     wrappers: tuple = ()
     keys: tuple = ()
     values: tuple = ()
 
     @property
     def arg_str(self):
         return f"({', '.join(str(v) for v in self.values)})" if self.values else ''
 
 
-class DiengineType(ABC):
+class ClickHouseType(ABC):
     """
-    Base class for all DiengineType objects.
+    Base class for all ClickHouseType objects.
     """
     __slots__ = 'nullable', 'low_card', 'wrappers', 'type_def', '__dict__'
     _name_suffix = ''
     encoding = 'utf8'
     np_type = 'O'  # Default to Numpy Object type
     nano_divisor = 0  # Only relevant for date like objects
     byte_size = 0
@@ -49,19 +49,19 @@
 
     def __init_subclass__(cls, registered: bool = True):
         if registered:
             cls.base_type = cls.__name__
             type_map[cls.base_type] = cls
 
     @classmethod
-    def build(cls: Type['DiengineType'], type_def: TypeDef):
+    def build(cls: Type['ClickHouseType'], type_def: TypeDef):
         return cls(type_def)
 
     @classmethod
-    def _active_format(cls, fmt_map: Dict[Type['DiengineType'], str], ctx: BaseQueryContext):
+    def _active_format(cls, fmt_map: Dict[Type['ClickHouseType'], str], ctx: BaseQueryContext):
         ctx_fmt = ctx.active_fmt(cls.base_type)
         if ctx_fmt:
             return ctx_fmt
         return fmt_map.get(cls, 'native')
 
     @classmethod
     def read_format(cls, ctx: BaseQueryContext):
@@ -70,15 +70,15 @@
     @classmethod
     def write_format(cls, ctx: BaseQueryContext):
         return cls._active_format(ch_write_formats, ctx)
 
     def __init__(self, type_def: TypeDef):
         """
         Base class constructor that sets Nullable and LowCardinality wrappers
-        :param type_def:  DiengineType base configuration parameters
+        :param type_def:  ClickHouseType base configuration parameters
         """
         self.type_def = type_def
         self.wrappers = type_def.wrappers
         self.low_card = 'LowCardinality' in self.wrappers
         self.nullable = 'Nullable' in self.wrappers
 
     def __eq__(self, other):
@@ -93,15 +93,15 @@
         for wrapper in reversed(self.wrappers):
             name = f'{wrapper}({name})'
         return name
 
     def write_column_prefix(self, dest: MutableSequence):
         """
         Prefix is primarily used is for the LowCardinality version (but see the JSON data type).  Because of the
-        way the Diengine C++ code is written, this must be done before any data is written even if the
+        way the ClickHouse C++ code is written, this must be done before any data is written even if the
         LowCardinality column is within a container.  The only recognized low cardinality version is 1
         :param dest: The native protocol binary write buffer
         """
         if self.low_card:
             write_uint64(low_card_version, dest)
 
     def read_column_prefix(self, source: ByteSource):
@@ -113,27 +113,27 @@
         if self.low_card:
             v = source.read_uint64()
             if v != low_card_version:
                 logger.warning('Unexpected low cardinality version %d reading type %s', v, self.name)
 
     def read_column(self, source: ByteSource, num_rows: int, ctx: QueryContext) -> Sequence:
         """
-        Wrapping read method for all DiengineType data types.  Only overridden for container classes so that
+        Wrapping read method for all ClickHouseType data types.  Only overridden for container classes so that
          the LowCardinality version is read for the contained types
         :param source: Native protocol binary read buffer
         :param num_rows: Number of rows expected in the column
         :param ctx: QueryContext for query specific settings
         :return: The decoded column data as a sequence and the updated location pointer
         """
         self.read_column_prefix(source)
         return self.read_column_data(source, num_rows, ctx)
 
     def read_column_data(self, source: ByteSource, num_rows: int, ctx: QueryContext) -> Sequence:
         """
-        Public read method for all DiengineType data type columns
+        Public read method for all ClickHouseType data type columns
         :param source: Native protocol binary read buffer
         :param num_rows: Number of rows expected in the column
         :param ctx: QueryContext for query specific settings
         :return: The decoded column plus the updated location pointer
         """
         if self.low_card:
             column = self._read_low_card_column(source, num_rows, ctx)
@@ -153,46 +153,46 @@
     # delegate binary operations to their elements
 
     # pylint: disable=no-self-use
     def _read_column_binary(self,
                             _source: ByteSource,
                             _num_rows: int, _ctx: QueryContext) -> Union[Sequence, MutableSequence]:
         """
-        Lowest level read method for DiengineType native data columns
+        Lowest level read method for ClickHouseType native data columns
         :param _source: Native protocol binary read buffer
         :param _num_rows: Expected number of rows in the column
         :return: Decoded column plus updated read buffer
         """
         return [], 0
 
     def _finalize_column(self, column: Sequence, _ctx: QueryContext) -> Sequence:
         return column
 
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: MutableSequence, ctx: InsertContext):
         """
-        Lowest level write method for DiengineType data columns
+        Lowest level write method for ClickHouseType data columns
         :param column: Python data column
         :param dest: Native protocol write buffer
         :param ctx: Insert Context with insert specific settings
         """
 
     def write_column(self, column: Sequence, dest: MutableSequence, ctx: InsertContext):
         """
-        Wrapping write method for DiengineTypes.  Only overridden for container types that so that
+        Wrapping write method for ClickHouseTypes.  Only overridden for container types that so that
         the write_native_prefix is done at the right time for contained types
         :param column: Column/sequence of Python values to write
         :param dest: Native binary write buffer
         :param ctx: Insert Context with insert specific settings
         """
         self.write_column_prefix(dest)
         self.write_column_data(column, dest, ctx)
 
     def write_column_data(self, column: Sequence, dest: MutableSequence, ctx: InsertContext):
         """
-        Public native write method for DiengineTypes.  Delegates the actual write to either the LowCardinality
+        Public native write method for ClickHouseTypes.  Delegates the actual write to either the LowCardinality
         write method or the _write_native_binary method of the type
         :param column: Sequence of Python data
         :param dest: Native binary write buffer
         :param ctx: Insert Context with insert specific settings
         """
         if self.low_card:
             self._write_column_low_card(column, dest, ctx)
@@ -271,21 +271,21 @@
             return column[0]
         return None
 
 
 EMPTY_TYPE_DEF = TypeDef()
 NULLABLE_TYPE_DEF = TypeDef(wrappers=('Nullable',))
 LC_TYPE_DEF = TypeDef(wrappers=('LowCardinality',))
-type_map: Dict[str, Type[DiengineType]] = {}
+type_map: Dict[str, Type[ClickHouseType]] = {}
 
 
-class ArrayType(DiengineType, ABC, registered=False):
+class ArrayType(ClickHouseType, ABC, registered=False):
     """
-    Diengine type that utilizes Python or Numpy arrays for fast reads and writes of binary data.
-    arrays can only be used for Diengine types that can be translated into UInt64 (and smaller) integers
+    ClickHouse type that utilizes Python or Numpy arrays for fast reads and writes of binary data.
+    arrays can only be used for ClickHouse types that can be translated into UInt64 (and smaller) integers
     or Float32/64
     """
     _signed = True
     _array_type = None
     _struct_type = None
     valid_formats = 'string', 'native'
     python_type = int
@@ -337,17 +337,17 @@
         if ctx.as_pandas and ctx.use_na_values:
             return pd.NA
         if ctx.use_none:
             return None
         return 0
 
 
-class UnsupportedType(DiengineType, ABC, registered=False):
+class UnsupportedType(ClickHouseType, ABC, registered=False):
     """
-    Base class for Diengine types that can't be serialized/deserialized into Python types.
+    Base class for ClickHouse types that can't be serialized/deserialized into Python types.
     Mostly useful just for DDL statements
     """
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self._name_suffix = type_def.arg_str
 
     def _read_column_binary(self, source: Sequence, num_rows: int, ctx: QueryContext):
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/container.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import array
 from typing import Sequence, MutableSequence
 
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 from diengine_connect.json_impl import any_to_json
-from diengine_connect.datatypes.base import DiengineType, TypeDef
+from diengine_connect.datatypes.base import ClickHouseType, TypeDef
 from diengine_connect.driver.common import must_swap
 from diengine_connect.datatypes.registry import get_from_name
 
 
-class Array(DiengineType):
+class Array(ClickHouseType):
     __slots__ = ('element_type',)
     python_type = list
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self.element_type = get_from_name(type_def.values[0])
         self._name_suffix = f'({self.element_type.name})'
@@ -69,15 +69,15 @@
             if must_swap:
                 offsets.byteswap()
             dest += offsets.tobytes()
             column = data
         final_type.write_column_data(column, dest, ctx)
 
 
-class Tuple(DiengineType):
+class Tuple(ClickHouseType):
     _slots = 'element_names', 'element_types'
     python_type = tuple
     valid_formats = 'tuple', 'json', 'native'  # native is 'tuple' for unnamed tuples, and dict for named tuples
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self.element_names = type_def.keys
@@ -114,15 +114,15 @@
 
     def write_column_data(self, column: Sequence, dest: MutableSequence, ctx: InsertContext):
         columns = list(zip(*column))
         for e_type, elem_column in zip(self.element_types, columns):
             e_type.write_column_data(elem_column, dest, ctx)
 
 
-class Map(DiengineType):
+class Map(ClickHouseType):
     _slots = 'key_type', 'value_type'
     python_type = dict
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self.key_type = get_from_name(type_def.values[0])
         self.value_type = get_from_name(type_def.values[1])
@@ -164,15 +164,15 @@
         if must_swap:
             offsets.byteswap()
         dest += offsets.tobytes()
         self.key_type.write_column_data(keys, dest, ctx)
         self.value_type.write_column_data(values, dest, ctx)
 
 
-class Nested(DiengineType):
+class Nested(ClickHouseType):
     __slots__ = 'tuple_array', 'element_names', 'element_types'
     python_type = Sequence[dict]
 
     def __init__(self, type_def):
         super().__init__(type_def)
         self.element_names = type_def.keys
         self.tuple_array = get_from_name(f"Array(Tuple({','.join(type_def.values)}))")
@@ -193,15 +193,15 @@
 
     def write_column_data(self, column: Sequence, dest: MutableSequence, ctx: InsertContext):
         keys = self.element_names
         data = [[tuple(sub_row[key] for key in keys) for sub_row in row] for row in column]
         self.tuple_array.write_column_data(data, dest, ctx)
 
 
-class JSON(DiengineType):
+class JSON(ClickHouseType):
     python_type = dict
     # Native is a Python type (primitive, dict, array), string is an actual JSON string
     valid_formats = 'string', 'native'
 
     def write_column_prefix(self, dest: MutableSequence):
         dest.append(0x01)
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/format.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
 from typing import Dict, Type, Sequence, Optional
 
-from diengine_connect.datatypes.base import DiengineType, type_map, ch_read_formats, ch_write_formats
+from diengine_connect.datatypes.base import ClickHouseType, type_map, ch_read_formats, ch_write_formats
 from diengine_connect.driver.exceptions import ProgrammingError
 
 json_re = re.compile('json', re.IGNORECASE)
 
 
 def set_default_formats(*args, **kwargs):
     fmt_map = format_map(_convert_arguments(*args, **kwargs))
@@ -42,15 +42,15 @@
 
 
 def clear_read_format(pattern: str):
     for ch_type in _matching_types(pattern):
         ch_read_formats.pop(ch_type, None)
 
 
-def format_map(fmt_map: Optional[Dict[str, str]]) -> Dict[Type[DiengineType], str]:
+def format_map(fmt_map: Optional[Dict[str, str]]) -> Dict[Type[ClickHouseType], str]:
     if not fmt_map:
         return {}
     final_map = {}
     for pattern, fmt in fmt_map.items():
         for ch_type in _matching_types(pattern, fmt):
             final_map[ch_type] = fmt
     return final_map
@@ -63,17 +63,17 @@
             fmt_map[args[x]] = args[x + 1]
     except (IndexError, TypeError, ValueError) as ex:
         raise ProgrammingError('Invalid type/format arguments for format method') from ex
     fmt_map.update(kwargs)
     return fmt_map
 
 
-def _matching_types(pattern: str, fmt: str = None) -> Sequence[Type[DiengineType]]:
+def _matching_types(pattern: str, fmt: str = None) -> Sequence[Type[ClickHouseType]]:
     re_pattern = re.compile(pattern.replace('*', '.*'), re.IGNORECASE)
     matches = [ch_type for type_name, ch_type in type_map.items() if re_pattern.match(type_name)]
     if not matches:
-        ProgrammingError(f'Unrecognized Diengine type {pattern} when setting formats')
+        ProgrammingError(f'Unrecognized ClickHouse type {pattern} when setting formats')
     if fmt:
         invalid = [ch_type.__name__ for ch_type in matches if fmt not in ch_type.valid_formats]
         if invalid:
-            raise ProgrammingError(f"{fmt} is not a valid format for Diengine types {','.join(invalid)}.")
+            raise ProgrammingError(f"{fmt} is not a valid format for ClickHouse types {','.join(invalid)}.")
     return matches
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/network.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import socket
 from ipaddress import IPv4Address, IPv6Address
 from typing import Union, MutableSequence, Sequence
 
-from diengine_connect.datatypes.base import DiengineType
+from diengine_connect.datatypes.base import ClickHouseType
 from diengine_connect.driver.common import write_array, int_size
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 from diengine_connect.driver.ctypes import data_conv
 
 IPV4_V6_MASK = b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xff\xff'
 V6_NULL = bytes(b'\x00' * 16)
 
 
 # pylint: disable=protected-access
-class IPv4(DiengineType):
+class IPv4(ClickHouseType):
     _array_type = 'L' if int_size == 2 else 'I'
     valid_formats = 'string', 'native', 'int'
     python_type = IPv4Address
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         if self.read_format(ctx) == 'int':
             return source.read_array(self._array_type, num_rows)
@@ -48,15 +48,15 @@
             return '0.0.0.0'
         if fmt == 'int':
             return 0
         return None
 
 
 # pylint: disable=protected-access
-class IPv6(DiengineType):
+class IPv6(ClickHouseType):
     valid_formats = 'string', 'native'
     python_type = IPv6Address
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         if self.read_format(ctx) == 'string':
             return self._read_binary_str(source, num_rows)
         return self._read_binary_ip(source, num_rows)
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/numeric.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import decimal
 from typing import Union, Type, Sequence, MutableSequence
 
 from math import nan
 
-from diengine_connect.datatypes.base import TypeDef, ArrayType, DiengineType
+from diengine_connect.datatypes.base import TypeDef, ArrayType, ClickHouseType
 from diengine_connect.driver.common import array_type, write_array, decimal_size, decimal_prec
 from diengine_connect.driver.ctypes import numpy_conv, data_conv
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.options import pd, np
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 
@@ -72,15 +72,15 @@
         if ctx.use_pandas_na and self.nullable:
             return pd.array(column, dtype='Int64' if fmt == 'signed' else 'UInt64')
         if ctx.use_numpy and self.nullable and (not ctx.use_none):
             return np.array(column, dtype='<q' if fmt == 'signed' else '<u8')
         return column
 
 
-class BigInt(DiengineType, registered=False):
+class BigInt(ClickHouseType, registered=False):
     _signed = True
     valid_formats = 'string', 'native'
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         signed = self._signed
         sz = self.byte_size
         column = []
@@ -171,15 +171,15 @@
 
 
 class Float64(Float):
     _array_type = 'd'
     np_type = '<f8'
 
 
-class Bool(DiengineType):
+class Bool(ClickHouseType):
     np_type = '?'
     python_type = bool
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, _ctx: QueryContext):
         column = source.read_bytes(num_rows)
         return [b != 0 for b in column]
 
@@ -192,15 +192,15 @@
         write_array('B', [1 if x else 0 for x in column], dest)
 
 
 class Boolean(Bool):
     pass
 
 
-class Enum(DiengineType):
+class Enum(ClickHouseType):
     __slots__ = '_name_map', '_int_map'
     _array_type = 'b'
     valid_formats = 'native', 'int'
     python_type = str
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
@@ -232,15 +232,15 @@
     _array_type = 'b'
 
 
 class Enum16(Enum):
     _array_type = 'h'
 
 
-class Decimal(DiengineType):
+class Decimal(ClickHouseType):
     __slots__ = 'prec', 'scale', '_mult', '_zeros', 'byte_size', '_array_type'
     python_type = decimal.Decimal
     dec_size = 0
 
     @classmethod
     def build(cls: Type['Decimal'], type_def: TypeDef):
         size = cls.dec_size
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/registry.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 
 from typing import Tuple, Dict
-from diengine_connect.datatypes.base import TypeDef, DiengineType, type_map
+from diengine_connect.datatypes.base import TypeDef, ClickHouseType, type_map
 from diengine_connect.driver.exceptions import InternalError
 from diengine_connect.driver.parser import parse_enum, parse_callable, parse_columns
 
 logger = logging.getLogger(__name__)
-type_cache: Dict[str, DiengineType] = {}
+type_cache: Dict[str, ClickHouseType] = {}
 
 
 def parse_name(name: str) -> Tuple[str, str, TypeDef]:
     """
-    Converts a Diengine type name into the base class and the definition (TypeDef) needed for any
+    Converts a ClickHouse type name into the base class and the definition (TypeDef) needed for any
     additional instantiation
-    :param name: Diengine type name as returned by diengine
+    :param name: ClickHouse type name as returned by clickhouse
     :return: The original base name (before arguments), the full name as passed in and the TypeDef object that
      captures any additional arguments
     """
     base = name
     wrappers = []
     keys = tuple()
     if base.startswith('LowCardinality'):
@@ -35,28 +35,28 @@
     elif base.startswith('Tuple'):
         keys, values = parse_columns(base[5:])
         base = 'Tuple'
     else:
         try:
             base, values, _ = parse_callable(base)
         except IndexError:
-            raise InternalError(f'Can not parse Diengine data type: {name}') from None
+            raise InternalError(f'Can not parse ClickHouse data type: {name}') from None
     return base, name, TypeDef(tuple(wrappers), keys, values)
 
 
-def get_from_name(name: str) -> DiengineType:
+def get_from_name(name: str) -> ClickHouseType:
     """
-    Returns the DiengineType instance parsed from the Diengine type name.  Instances are cached
-    :param name: Diengine type name as returned by Diengine in WithNamesAndTypes FORMAT or the Native protocol
-    :return: The instance of the Diengine Type
+    Returns the ClickHouseType instance parsed from the ClickHouse type name.  Instances are cached
+    :param name: ClickHouse type name as returned by ClickHouse in WithNamesAndTypes FORMAT or the Native protocol
+    :return: The instance of the ClickHouse Type
     """
     ch_type = type_cache.get(name, None)
     if not ch_type:
         base, name, type_def = parse_name(name)
         try:
             ch_type = type_map[base].build(type_def)
         except KeyError:
-            err_str = f'Unrecognized Diengine type base: {base} name: {name}'
+            err_str = f'Unrecognized ClickHouse type base: {base} name: {name}'
             logger.error(err_str)
             raise InternalError(err_str) from None
         type_cache[name] = ch_type
     return ch_type
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/special.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/special.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Union, Sequence, MutableSequence
 from uuid import UUID as PYUUID
 
-from diengine_connect.datatypes.base import TypeDef, DiengineType, ArrayType, UnsupportedType
+from diengine_connect.datatypes.base import TypeDef, ClickHouseType, ArrayType, UnsupportedType
 from diengine_connect.datatypes.registry import get_from_name
 from diengine_connect.driver.ctypes import data_conv
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 
 empty_uuid_b = bytes(b'\x00' * 16)
 
 
-class UUID(DiengineType):
+class UUID(ClickHouseType):
     valid_formats = 'string', 'native'
     np_type = 'U36'
 
     def python_null(self, ctx):
         return '' if self.read_format(ctx) == 'string' else PYUUID(int=0)
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
@@ -75,20 +75,20 @@
         super().__init__(type_def)
         self.nullable = True
 
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: MutableSequence, _ctx):
         dest += bytes(0x30 for _ in range(len(column)))
 
 
-class SimpleAggregateFunction(DiengineType):
+class SimpleAggregateFunction(ClickHouseType):
     _slots = ('element_type',)
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
-        self.element_type: DiengineType = get_from_name(type_def.values[1])
+        self.element_type: ClickHouseType = get_from_name(type_def.values[1])
         self._name_suffix = type_def.arg_str
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         return self.element_type.read_column_data(source, num_rows, ctx)
 
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: MutableSequence, ctx: InsertContext):
         self.element_type.write_column_data(column, dest, ctx)
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/string.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Sequence, MutableSequence, Union
 
-from diengine_connect.datatypes.base import DiengineType, TypeDef
+from diengine_connect.datatypes.base import ClickHouseType, TypeDef
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 from diengine_connect.driver.options import np, pd
 
 
-class String(DiengineType):
+class String(ClickHouseType):
     valid_formats = 'bytes', 'native'
 
     def _active_encoding(self, ctx):
         if self.read_format(ctx) == 'bytes':
             return None
         if ctx.encoding:
             return ctx.encoding
@@ -94,15 +94,15 @@
         if ctx.use_none:
             return None
         if self.read_format(ctx) == 'bytes':
             return bytes()
         return ''
 
 
-class FixedString(DiengineType):
+class FixedString(ClickHouseType):
     valid_formats = 'string', 'native'
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self.byte_size = type_def.values[0]
         self._name_suffix = type_def.arg_str
         self._empty_bytes = bytes(b'\x00' * self.byte_size)
```

### Comparing `diengine-connect-0.0.3/diengine_connect/datatypes/temporal.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytz
 
 from datetime import date, datetime, tzinfo
 from typing import Union, Sequence, MutableSequence
 
-from diengine_connect.datatypes.base import TypeDef, DiengineType
+from diengine_connect.datatypes.base import TypeDef, ClickHouseType
 from diengine_connect.driver.common import write_array, np_date_types, int_size
 from diengine_connect.driver.exceptions import ProgrammingError
 from diengine_connect.driver.ctypes import data_conv, numpy_conv
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.query import QueryContext
 from diengine_connect.driver.types import ByteSource
 from diengine_connect.driver.options import np, pd
 
 epoch_start_date = date(1970, 1, 1)
 epoch_start_datetime = datetime(1970, 1, 1)
 
 
-class Date(DiengineType):
+class Date(ClickHouseType):
     _array_type = 'H'
     np_type = 'datetime64[D]'
     nano_divisor = 86400 * 1000000000
     valid_formats = 'native', 'int'
     python_type = date
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
@@ -77,15 +77,15 @@
         return data_conv.read_date32_col(source, num_rows)
 
 
 from_ts_naive = datetime.utcfromtimestamp
 from_ts_tz = datetime.fromtimestamp
 
 
-class DateTimeBase(DiengineType, registered=False):
+class DateTimeBase(ClickHouseType, registered=False):
     __slots__ = ('tzinfo',)
     valid_formats = 'native', 'int'
     python_type = datetime
 
     def _active_null(self, ctx: QueryContext):
         fmt = self.read_format(ctx)
         if ctx.use_pandas_na:
```

### Comparing `diengine-connect-0.0.3/diengine_connect/dbapi/__init__.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/dbapi/connection.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/dbapi/cursor.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/__init__.py` & `diengine-connect-0.1.7/diengine_connect/driver/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,60 +18,60 @@
                   port: int = 0,
                   secure: Union[bool, str] = False,
                   dsn: Optional[str] = None,
                   settings: Optional[Dict[str, Any]] = None,
                   generic_args: Optional[Dict[str, Any]] = None,
                   **kwargs) -> Client:
     """
-    The preferred method to get a Diengine Connect Client instance
+    The preferred method to get a ClickHouse Connect Client instance
 
-    :param host: The hostname or IP address of the Diengine server. If not set, localhost will be used.
-    :param username: The Diengine username. If not set, the default Diengine user will be used.
+    :param host: The hostname or IP address of the ClickHouse server. If not set, localhost will be used.
+    :param username: The ClickHouse username. If not set, the default ClickHouse user will be used.
     :param password: The password for username.
-    :param database:  The default database for the connection. If not set, Diengine Connect will use the
+    :param database:  The default database for the connection. If not set, ClickHouse Connect will use the
      default database for username.
     :param interface: Must be http or https.  Defaults to http, or to https if port is set to 8443 or 443
-    :param port: The Diengine HTTP or HTTPS port. If not set will default to 8123, or to 8443 if secure=True
+    :param port: The ClickHouse HTTP or HTTPS port. If not set will default to 8123, or to 8443 if secure=True
       or interface=https.
     :param secure: Use https/TLS. This overrides inferred values from the interface or port arguments.
     :param dsn: A string in standard DSN (Data Source Name) format. Other connection values (such as host or user)
       will be extracted from this string if not set otherwise.
-    :param settings: Diengine server settings to be used with the session/every request
-    :param generic_args: Used internally to parse DBAPI connection strings into keyword arguments and Diengine settings.
+    :param settings: ClickHouse server settings to be used with the session/every request
+    :param generic_args: Used internally to parse DBAPI connection strings into keyword arguments and ClickHouse settings.
       It is not recommended to use this parameter externally.
 
     :param kwargs -- Recognized keyword arguments (used by the HTTP client), see below
 
-    :param compress: Enable compression for Diengine HTTP inserts and query results.  True will select the preferred
+    :param compress: Enable compression for ClickHouse HTTP inserts and query results.  True will select the preferred
       compression method (lz4).  A str of 'lz4', 'zstd', 'brotli', or 'gzip' can be used to use a specific compression type
     :param query_limit: Default LIMIT on returned rows.  0 means no limit
     :param connect_timeout:  Timeout in seconds for the http connection
     :param send_receive_timeout: Read timeout in seconds for http connection
     :param client_name: client_name prepended to the HTTP User Agent header. Set this to track client queries
-      in the Diengine system.query_log.
+      in the ClickHouse system.query_log.
     :param send_progress: Deprecated, has no effect.  Previous functionality is now automatically determined
     :param verify: Verify the server certificate in secure/https mode
-    :param ca_cert: If verify is True, the file path to Certificate Authority root to validate Diengine server
-     certificate, in .pem format.  Ignored if verify is False.  This is not necessary if the Diengine server
+    :param ca_cert: If verify is True, the file path to Certificate Authority root to validate ClickHouse server
+     certificate, in .pem format.  Ignored if verify is False.  This is not necessary if the ClickHouse server
      certificate is trusted by the operating system.  To trust the maintained list of "global" public root
      certificates maintained by the Python 'certifi' package, set ca_cert to 'certifi'
     :param client_cert: File path to a TLS Client certificate in .pem format.  This file should contain any
       applicable intermediate certificates
     :param client_cert_key: File path to the private key for the Client Certificate.  Required if the private key
       is not included the Client Certificate key file
-    :param session_id Diengine session id.  If not specified and the common setting 'autogenerate_session_id'
+    :param session_id ClickHouse session id.  If not specified and the common setting 'autogenerate_session_id'
       is True, the client will generate a UUID1 session id
     :param pool_mgr Optional urllib3 PoolManager for this client.  Useful for creating separate connection
       pools for multiple client endpoints for applications with many clients
     :param http_proxy  http proxy address.  Equivalent to setting the HTTP_PROXY environment variable
     :param https_proxy https proxy address.  Equivalent to setting the HTTPS_PROXY environment variable
     :param server_host_name  This is the server host name that will be checked against a TLS certificate for
-      validity.  This option can be used if using an ssh_tunnel or other indirect means to an Diengine server
-      where the `host` argument refers to the tunnel or proxy and not the actual Diengine server
-    :return: Diengine Connect Client instance
+      validity.  This option can be used if using an ssh_tunnel or other indirect means to an ClickHouse server
+      where the `host` argument refers to the tunnel or proxy and not the actual ClickHouse server
+    :return: ClickHouse Connect Client instance
     """
     if dsn:
         parsed = urlparse(dsn)
         username = username or parsed.username
         password = password or parsed.password
         host = host or parsed.hostname
         port = port or parsed.port
@@ -107,8 +107,8 @@
         return HttpClient(interface, host, port, username, password, database, settings=settings, **kwargs)
     raise ProgrammingError(f'Unrecognized client type {interface}')
 
 
 def default_port(interface: str, secure: bool):
     if interface.startswith('http'):
         return 8443 if secure else 8123
-    raise ValueError('Unrecognized Diengine interface')
+    raise ValueError('Unrecognized ClickHouse interface')
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/buffer.py` & `diengine-connect-0.1.7/diengine_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/client.py` & `diengine-connect-0.1.7/diengine_connect/driver/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from abc import ABC, abstractmethod
 from typing import Iterable, Optional, Any, Union, Sequence, Dict, Generator, BinaryIO
 from pytz.exceptions import UnknownTimeZoneError
 
 from diengine_connect import common
 from diengine_connect.common import version
 from diengine_connect.datatypes.registry import get_from_name
-from diengine_connect.datatypes.base import DiengineType
+from diengine_connect.datatypes.base import ClickHouseType
 from diengine_connect.driver.common import dict_copy, StreamContext
 from diengine_connect.driver.constants import CH_VERSION_WITH_PROTOCOL, PROTOCOL_VERSION_WITH_LOW_CARD
 from diengine_connect.driver.exceptions import ProgrammingError
 from diengine_connect.driver.insert import InsertContext
 from diengine_connect.driver.models import ColumnDef, SettingDef, SettingStatus
 from diengine_connect.driver.query import QueryResult, to_arrow, QueryContext, arrow_buffer
 
@@ -23,25 +23,25 @@
 logger = logging.getLogger(__name__)
 arrow_str_setting = 'output_format_arrow_string_as_string'
 
 
 # pylint: disable=too-many-public-methods
 class Client(ABC):
     """
-    Base Diengine Connect client
+    Base ClickHouse Connect client
     """
     compression: str = None
     write_compression: str = None
     protocol_version = 0
     valid_transport_settings = set()
     optional_transport_settings = set()
 
     def __init__(self, database: str, query_limit: int, uri: str):
         """
-        Shared initialization of Diengine Connect client
+        Shared initialization of ClickHouse Connect client
         :param database: database name
         :param query_limit: default LIMIT for queries
         :param uri: uri for error messages
         """
         self.query_limit = query_limit
         self.server_tz = pytz.UTC
         # self.server_version, server_tz, self.database = \
@@ -61,15 +61,15 @@
             self.database = database
         if self.min_version(CH_VERSION_WITH_PROTOCOL):
             self.protocol_version = PROTOCOL_VERSION_WITH_LOW_CARD
         self.uri = uri
 
     def _validate_settings(self, settings: Optional[Dict[str, Any]]) -> Dict[str, str]:
         """
-        This strips any Diengine settings that are not recognized or are read only.
+        This strips any ClickHouse settings that are not recognized or are read only.
         :param settings:  Dictionary of setting name and values
         :return: A filtered dictionary of settings with values rendered as strings
         """
         validated = {}
         invalid_action = common.get_setting('invalid_setting_action')
         for key, value in settings.items():
             str_value = self._validate_setting(key, value, invalid_action)
@@ -110,19 +110,19 @@
     @abstractmethod
     def _query_with_context(self, context: QueryContext):
         pass
 
     @abstractmethod
     def set_client_setting(self, key, value):
         """
-        Set a Diengine setting for the client after initialization.  If a setting is not recognized by Diengine,
+        Set a clickhouse setting for the client after initialization.  If a setting is not recognized by ClickHouse,
         or the setting is identified as "read_only", this call will either throw a Programming exception or attempt
         to send the setting anyway based on the common setting 'invalid_setting_action'
-        :param key: Diengine setting name
-        :param value: Diengine setting value
+        :param key: ClickHouse setting name
+        :param value: ClickHouse setting value
         """
 
     @abstractmethod
     def get_client_setting(self, key) -> Optional[str]:
         """
         :param key: The setting key
         :return: The string value of the setting, if it exists, or None
@@ -145,15 +145,15 @@
               column_tzs: Optional[Dict[str, Union[str, tzinfo]]] = None) -> QueryResult:
         """
         Main query method for SELECT, DESCRIBE and other SQL statements that return a result matrix.  For
         parameters, see the create_query_context method
         :return: QueryResult -- data and metadata from response
         """
         if query and query.lower().strip().startswith('select __connect_version__'):
-            return QueryResult([[f'Diengine Connect v.{version()}  ⓒ Diengine Inc.']], None,
+            return QueryResult([[f'ClickHouse Connect v.{version()}  ⓒ ClickHouse Inc.']], None,
                                ('connect_version',), (get_from_name('String'),))
         kwargs = locals().copy()
         del kwargs['self']
         query_context = self.create_query_context(**kwargs)
         if query_context.is_command:
             response = self.command(query, parameters=query_context.parameters, settings=query_context.settings)
             return QueryResult([response] if isinstance(response, list) else [[response]])
@@ -216,22 +216,22 @@
     @abstractmethod
     def raw_query(self, query: str,
                   parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                   settings: Optional[Dict[str, Any]] = None,
                   fmt: str = None,
                   use_database: bool = True) -> bytes:
         """
-        Query method that simply returns the raw Diengine format bytes
+        Query method that simply returns the raw ClickHouse format bytes
         :param query: Query statement/format string
         :param parameters: Optional dictionary used to format the query
-        :param settings: Optional dictionary of Diengine settings (key/string values)
-        :param fmt: Diengine output format
-        :param use_database  Send the database parameter to Diengine so the command will be executed in the client
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
+        :param fmt: ClickHouse output format
+        :param use_database  Send the database parameter to ClickHouse so the command will be executed in the client
          database context.
-        :return: bytes representing raw Diengine return value based on format
+        :return: bytes representing raw ClickHouse return value based on format
         """
 
     # pylint: disable=duplicate-code,too-many-arguments,unused-argument
     def query_np(self,
                  query: str = None,
                  parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                  settings: Optional[Dict[str, Any]] = None,
@@ -323,34 +323,34 @@
                              use_na_values: Optional[bool] = None,
                              streaming: bool = False,
                              as_pandas: bool = False) -> QueryContext:
         """
         Creates or updates a reusable QueryContext object
         :param query: Query statement/format string
         :param parameters: Optional dictionary used to format the query
-        :param settings: Optional dictionary of Diengine settings (key/string values)
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param query_formats: See QueryContext __init__ docstring
         :param column_formats: See QueryContext __init__ docstring
         :param encoding: See QueryContext __init__ docstring
-        :param use_none: Use None for Diengine NULL instead of default values.  Note that using None in Numpy
+        :param use_none: Use None for ClickHouse NULL instead of default values.  Note that using None in Numpy
           arrays will force the numpy array dtype to 'object', which is often inefficient.  This effect also
           will impact the performance of Pandas dataframes.
         :param column_oriented: Deprecated. Controls orientation of the QueryResult result_set property
         :param use_numpy: Return QueryResult columns as one-dimensional numpy arrays
-        :param max_str_len: Limit returned Diengine String values to this length, which allows a Numpy
-          structured array even with Diengine variable length String columns.  If 0, Numpy arrays for
+        :param max_str_len: Limit returned ClickHouse String values to this length, which allows a Numpy
+          structured array even with ClickHouse variable length String columns.  If 0, Numpy arrays for
           String columns will always be object arrays
         :param context: An existing QueryContext to be updated with any provided parameter values
         :param query_tz  Either a string or a pytz tzinfo object.  (Strings will be converted to tzinfo objects).
           Values for any DateTime or DateTime64 column in the query will be converted to Python datetime.datetime
           objects with the selected timezone.
         :param column_tzs A dictionary of column names to tzinfo objects (or strings that will be converted to
           tzinfo objects).  The timezone will be applied to datetime objects returned in the query
         :param use_na_values:  Only relevant to Pandas Dataframe queries.  Use Pandas "missing types", such as
-          pandas.NA and pandas.NaT for Diengine NULL values.  Defaulted to True for query_df methods
+          pandas.NA and pandas.NaT for ClickHouse NULL values.  Defaulted to True for query_df methods
         :param as_pandas Return the result columns as pandas.Series objects
         :param streaming Marker used to correctly configure streaming queries
         :return: Reusable QueryContext
         """
         if context:
             return context.updated_copy(query=query,
                                         parameters=parameters,
@@ -391,19 +391,19 @@
 
     def query_arrow(self,
                     query: str,
                     parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                     settings: Optional[Dict[str, Any]] = None,
                     use_strings: bool = True):
         """
-        Query method using the Diengine Arrow format to return a PyArrow table
+        Query method using the ClickHouse Arrow format to return a PyArrow table
         :param query: Query statement/format string
         :param parameters: Optional dictionary used to format the query
-        :param settings: Optional dictionary of Diengine settings (key/string values)
-        :param use_strings:  Convert Diengine String type to Arrow string type (instead of binary)
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
+        :param use_strings:  Convert ClickHouse String type to Arrow string type (instead of binary)
         :return: PyArrow.Table
         """
         settings = dict_copy(settings)
         if self.database:
             settings['database'] = self.database
         if arrow_str_setting in self.server_settings and arrow_str_setting not in settings:
             settings[arrow_str_setting] = '1' if use_strings else '0'
@@ -414,56 +414,56 @@
                 cmd: str,
                 parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                 data: Union[str, bytes] = None,
                 settings: Dict[str, Any] = None,
                 use_database: bool = True) -> Union[str, int, Sequence[str]]:
         """
         Client method that returns a single value instead of a result set
-        :param cmd: Diengine query/command as a python format string
+        :param cmd: ClickHouse query/command as a python format string
         :param parameters: Optional dictionary of key/values pairs to be formatted
         :param data: Optional 'data' for the command (for INSERT INTO in particular)
-        :param settings: Optional dictionary of Diengine settings (key/string values)
-        :param use_database: Send the database parameter to Diengine so the command will be executed in the client
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
+        :param use_database: Send the database parameter to ClickHouse so the command will be executed in the client
          database context.  Otherwise, no database will be specified with the command.  This is useful for determining
          the default user database
-        :return: Decoded response from Diengine as either a string, int, or sequence of strings
+        :return: Decoded response from ClickHouse as either a string, int, or sequence of strings
         """
 
     @abstractmethod
     def ping(self) -> bool:
         """
         Validate the connection, does not throw an Exception (see debug logs)
-        :return: Diengine server is up and reachable
+        :return: ClickHouse server is up and reachable
         """
 
     # pylint: disable=too-many-arguments
     def insert(self,
                table: Optional[str] = None,
                data: Sequence[Sequence[Any]] = None,
                column_names: Union[str, Iterable[str]] = '*',
                database: Optional[str] = None,
-               column_types: Sequence[DiengineType] = None,
+               column_types: Sequence[ClickHouseType] = None,
                column_type_names: Sequence[str] = None,
                column_oriented: bool = False,
                settings: Optional[Dict[str, Any]] = None,
                context: InsertContext = None) -> None:
         """
         Method to insert multiple rows/data matrix of native Python objects.  If context is specified arguments
         other than data are ignored
         :param table: Target table
         :param data: Sequence of sequences of Python data
         :param column_names: Ordered list of column names or '*' if column types should be retrieved from the
-            Diengine table definition
+            ClickHouse table definition
         :param database: Target database -- will use client default database if not specified.
-        :param column_types: Diengine column types.  If set then column data does not need to be retrieved from
+        :param column_types: ClickHouse column types.  If set then column data does not need to be retrieved from
             the server
-        :param column_type_names: Diengine column type names.  If set then column data does not need to be
+        :param column_type_names: ClickHouse column type names.  If set then column data does not need to be
             retrieved from the server
         :param column_oriented: If true the data is already "pivoted" in column form
-        :param settings: Optional dictionary of Diengine settings (key/string values)
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param context: Optional reusable insert context to allow repeated inserts into the same table with
             different data batches
         :return: No return, throws an exception if the insert fails
         """
         if (context is None or context.empty) and data is None:
             raise ProgrammingError('No data specified for insert') from None
         if context is None:
@@ -481,28 +481,28 @@
         self.data_insert(context)
 
     def insert_df(self, table: str = None,
                   df=None,
                   database: Optional[str] = None,
                   settings: Optional[Dict] = None,
                   column_names: Optional[Sequence[str]] = None,
-                  column_types: Sequence[DiengineType] = None,
+                  column_types: Sequence[ClickHouseType] = None,
                   column_type_names: Sequence[str] = None,
                   context: InsertContext = None) -> None:
         """
-        Insert a pandas DataFrame into Diengine.  If context is specified arguments other than df are ignored
-        :param table: Diengine table
+        Insert a pandas DataFrame into ClickHouse.  If context is specified arguments other than df are ignored
+        :param table: ClickHouse table
         :param df: two-dimensional pandas dataframe
-        :param database: Optional Diengine database
-        :param settings: Optional dictionary of Diengine settings (key/string values)
-        :param column_names: An optional list of Diengine column names.  If not set, the DataFrame column names
+        :param database: Optional ClickHouse database
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
+        :param column_names: An optional list of ClickHouse column names.  If not set, the DataFrame column names
            will be used
-        :param column_types: Diengine column types.  If set then column data does not need to be retrieved from
+        :param column_types: ClickHouse column types.  If set then column data does not need to be retrieved from
             the server
-        :param column_type_names: Diengine column type names.  If set then column data does not need to be
+        :param column_type_names: ClickHouse column type names.  If set then column data does not need to be
             retrieved from the server
         :param context: Optional reusable insert context to allow repeated inserts into the same table with
             different data batches
         :return: No return, throws an exception if the insert fails
         """
         if context is None:
             if column_names is None:
@@ -510,46 +510,46 @@
             elif len(column_names) != len(df.columns):
                 raise ProgrammingError('DataFrame column count does not match insert_columns') from None
         self.insert(table, df, column_names, database, column_types=column_types, column_type_names=column_type_names,
                     settings=settings, context=context)
 
     def insert_arrow(self, table: str, arrow_table, database: str = None, settings: Optional[Dict] = None):
         """
-        Insert a PyArrow table DataFrame into Diengine using raw Arrow format
-        :param table: Diengine table
+        Insert a PyArrow table DataFrame into ClickHouse using raw Arrow format
+        :param table: ClickHouse table
         :param arrow_table: PyArrow Table object
-        :param database: Optional Diengine database
-        :param settings: Optional dictionary of Diengine settings (key/string values)
+        :param database: Optional ClickHouse database
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :return: No return, throws an exception if the insert fails
         """
         full_table = table if '.' in table or not database else f'{database}.{table}'
         column_names, insert_block = arrow_buffer(arrow_table)
         self.raw_insert(full_table, column_names, insert_block, settings, 'Arrow')
 
     def create_insert_context(self,
                               table: str,
                               column_names: Optional[Union[str, Sequence[str]]] = None,
                               database: Optional[str] = None,
-                              column_types: Sequence[DiengineType] = None,
+                              column_types: Sequence[ClickHouseType] = None,
                               column_type_names: Sequence[str] = None,
                               column_oriented: bool = False,
                               settings: Optional[Dict[str, Any]] = None,
                               data: Optional[Sequence[Sequence[Any]]] = None) -> InsertContext:
         """
         Builds a reusable insert context to hold state for a duration of an insert
         :param table: Target table
         :param database: Target database.  If not set, uses the client default database
         :param column_names: Optional ordered list of column names.  If not set, all columns ('*') will be assumed
           in the order specified by the table definition
         :param database: Target database -- will use client default database if not specified
-        :param column_types: Diengine column types.  Optional  Sequence of DiengineType objects.  If neither column
+        :param column_types: ClickHouse column types.  Optional  Sequence of ClickHouseType objects.  If neither column
            types nor column type names are set, actual column types will be retrieved from the server.
-        :param column_type_names: Diengine column type names.  Specified column types by name string
+        :param column_type_names: ClickHouse column type names.  Specified column types by name string
         :param column_oriented: If true the data is already "pivoted" in column form
-        :param settings: Optional dictionary of Diengine settings (key/string values)
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param data: Initial dataset for insert
         :return Reusable insert context
         """
         full_table = table if '.' in table or not database else f'{database}.{table}'
         column_defs = []
         if column_types is None and column_type_names is None:
             describe_result = self.query(f'DESCRIBE TABLE {full_table}')
@@ -616,17 +616,17 @@
                    insert_block: Union[str, bytes, Generator[bytes, None, None], BinaryIO] = None,
                    settings: Optional[Dict] = None,
                    fmt: Optional[str] = None):
         """
         Insert data already formatted in a bytes object
         :param table: Table name (whether qualified with the database name or not)
         :param column_names: Sequence of column names
-        :param insert_block: Binary or string data already in a recognized Diengine format
-        :param settings:  Optional dictionary of Diengine settings (key/string values)
-        :param fmt: Valid Diengine format
+        :param insert_block: Binary or string data already in a recognized ClickHouse format
+        :param settings:  Optional dictionary of ClickHouse settings (key/string values)
+        :param fmt: Valid clickhouse format
         """
 
     def close(self):
         """
         Subclass implementation to close the connection to the server/deallocate the client
         """
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/common.py` & `diengine-connect-0.1.7/diengine_connect/driver/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             column = [float(x) for x in column]
         else:
             column = [int(x) for x in column]
     try:
         buff = array.array(code, column)
     except (TypeError, OverflowError) as ex:
         raise ProgrammingError('Unable to create Python array.  This is usually caused by trying to insert None ' +
-                               'values into a Diengine column that is not Nullable') from ex
+                               'values into a ClickHouse column that is not Nullable') from ex
     if must_swap:
         buff.byteswap()
     dest += buff.tobytes()
 
 
 def write_uint64(value: int, dest: MutableSequence):
     """
@@ -81,20 +81,20 @@
             dest.append(b)
             return
         dest.append(0x80 | b)
 
 
 def decimal_size(prec: int):
     """
-    Determine the bit size of a Diengine or Python Decimal needed to store a value of the requested precision
+    Determine the bit size of a ClickHouse or Python Decimal needed to store a value of the requested precision
     :param prec: Precision of the Decimal in total number of base 10 digits
     :return: Required bit size
     """
     if prec < 1 or prec > 79:
-        raise ArithmeticError(f'Invalid precision {prec} for Diengine Decimal type')
+        raise ArithmeticError(f'Invalid precision {prec} for ClickHouse Decimal type')
     if prec < 10:
         return 32
     if prec < 19:
         return 64
     if prec < 39:
         return 128
     return 256
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/compression.py` & `diengine-connect-0.1.7/diengine_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/context.py` & `diengine-connect-0.1.7/diengine_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/ctypes.py` & `diengine-connect-0.1.7/diengine_connect/driver/ctypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 logger = logging.getLogger(__name__)
 
 RespBuffCls = ResponseBuffer
 data_conv = pydc
 numpy_conv = pync
 
-if coerce_bool(os.environ.get('DIENGINE_CONNECT_USE_C', True)):
+if coerce_bool(os.environ.get('CLICKHOUSE_CONNECT_USE_C', True)):
     try:
         from diengine_connect.driverc.buffer import ResponseBuffer as CResponseBuffer
         import diengine_connect.driverc.dataconv as cdc
 
         data_conv = cdc
         RespBuffCls = CResponseBuffer
-        logger.info('Successfully imported Diengine Connect C data optimizations')
+        logger.info('Successfully imported ClickHouse Connect C data optimizations')
     except ImportError as ex:
         CResponseBuffer = None
         logger.warning('Unable to connect optimized C data functions [%s], falling back to pure Python',
                        str(ex))
     try:
         import diengine_connect.driverc.npconv as cnc
 
         numpy_conv = cnc
-        logger.info('Successfully import Diengine Connect C/Numpy optimizations')
+        logger.info('Successfully import ClickHouse Connect C/Numpy optimizations')
     except ImportError as ex:
-        logger.warning('Unable to connect Diengine Connect C to Numpy API [%s], falling back to pure Python',
+        logger.warning('Unable to connect ClickHouse Connect C to Numpy API [%s], falling back to pure Python',
                        str(ex))
 else:
-    logger.info('Diengine Connect C optimizations disabled')
+    logger.info('ClickHouse Connect C optimizations disabled')
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/dataconv.py` & `diengine-connect-0.1.7/diengine_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/ddl.py` & `diengine-connect-0.1.7/diengine_connect/driver/ddl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import NamedTuple, Sequence
 
-from diengine_connect.datatypes.base import DiengineType
+from diengine_connect.datatypes.base import ClickHouseType
 
 
 class TableColumnDef(NamedTuple):
     """
-    Simplified Diengine Table Column definition for DDL
+    Simplified ClickHouse Table Column definition for DDL
     """
     name: str
-    ch_type: DiengineType
+    ch_type: ClickHouseType
     expr_type: str = None
     expr: str = None
 
     @property
     def col_expr(self):
         expr = f'{self.name} {self.ch_type.name}'
         if self.expr_type:
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/exceptions.py` & `diengine-connect-0.1.7/diengine_connect/driver/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 The driver exception classes here include all named exceptions required by th DB API 2.0 specification. It's not clear
 how useful that naming convention is, but the convention is used for potential improved compatibility with other
 libraries.  In most cases docstring are taken from the DBIApi 2.0 documentation
 """
 
 
-class DiengineError(Exception):
-    """Exception related to operation with Diengine."""
+class ClickHouseError(Exception):
+    """Exception related to operation with ClickHouse."""
 
 
 # pylint: disable=redefined-builtin
-class Warning(Warning, DiengineError):
+class Warning(Warning, ClickHouseError):
     """Exception raised for important warnings like data truncations
     while inserting, etc."""
 
 
-class Error(DiengineError):
+class Error(ClickHouseError):
     """Exception that is the base class of all other error exceptions
     (not Warning)."""
 
 
 class InterfaceError(Error):
     """Exception raised for errors that are related to the database
     interface rather than the database itself."""
@@ -73,12 +73,12 @@
     """Exception raised when a stream operation is executed on a closed stream."""
 
     def __init__(self):
         super().__init__('Executing a streaming operation on a closed stream')
 
 
 class StreamCompleteException(Exception):
-    """ Internal exception used to indicate the end of a Diengine query result stream."""
+    """ Internal exception used to indicate the end of a ClickHouse query result stream."""
 
 
 class StreamFailureError(Exception):
     """ Stream failed unexpectedly """
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/extras.py` & `diengine-connect-0.1.7/diengine_connect/driver/extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 from decimal import Decimal as PyDecimal
 from ipaddress import IPv4Address, IPv6Address
 from random import random, choice
 from typing import Sequence, Union, NamedTuple, Callable, Type, Dict
 from datetime import date, datetime, timedelta
 
-from diengine_connect.datatypes.base import DiengineType
+from diengine_connect.datatypes.base import ClickHouseType
 from diengine_connect.datatypes.container import Array, Tuple, Map, Nested
 from diengine_connect.datatypes.network import IPv4, IPv6
 from diengine_connect.datatypes.numeric import BigInt, Float32, Float64, Enum, Bool, Boolean, Decimal
 from diengine_connect.datatypes.registry import get_from_name
 from diengine_connect.datatypes.special import UUID
 from diengine_connect.datatypes.string import String, FixedString
 from diengine_connect.datatypes.temporal import Date, Date32, DateTime, DateTime64
@@ -27,36 +27,36 @@
     """
     null_pct: float = 0.15
     str_len: int = 200
     arr_len: int = 12
     ascii_only: bool = False
 
 
-def random_col_data(ch_type: Union[str, DiengineType], cnt: int, col_def: RandomValueDef = RandomValueDef()):
+def random_col_data(ch_type: Union[str, ClickHouseType], cnt: int, col_def: RandomValueDef = RandomValueDef()):
     """
     Generate a column of random data for insert tests
-    :param ch_type: DiengineType or Diengine type name
+    :param ch_type: ClickHouseType or ClickHouse type name
     :param cnt: Number of values to generate
     :param col_def: Parameters to use for random data generation
-    :return: A tuple of length cnt of random Python data values of the requested DiengineType
+    :return: A tuple of length cnt of random Python data values of the requested ClickHouseType
     """
     if isinstance(ch_type, str):
         ch_type = get_from_name(ch_type)
     gen = random_value_gen(ch_type, col_def)
     if ch_type.nullable:
         x = col_def.null_pct
         return tuple(gen() if random() > x else None for _ in range(cnt))
     return tuple(gen() for _ in range(cnt))
 
 
 # pylint: disable=too-many-return-statements,too-many-branches,protected-access
-def random_value_gen(ch_type: DiengineType, col_def: RandomValueDef):
+def random_value_gen(ch_type: ClickHouseType, col_def: RandomValueDef):
     """
-    Returns a generator function of random values of the requested DiengineType
-    :param ch_type: DiengineType to generate
+    Returns a generator function of random values of the requested ClickHouseType
+    :param ch_type: ClickHouseType to generate
     :param col_def: Parameters for the generated values
     :return: Function or lambda that will return a random value of the requested type
     """
     if ch_type.__class__ in gen_map:
         return gen_map[ch_type.__class__]
     if isinstance(ch_type, BigInt) or ch_type.python_type == int:
         if isinstance(ch_type, BigInt):
@@ -87,15 +87,15 @@
             return lambda: random_ascii_str(col_def.str_len)
         return lambda: random_utf8_str(col_def.str_len)
     if isinstance(ch_type, FixedString):
         return lambda: bytes((int(random() * 256) for _ in range(ch_type.byte_size)))
     if isinstance(ch_type, DateTime64):
         prec = ch_type.prec
         return lambda: random_datetime64(prec)
-    raise ValueError(f'Invalid Diengine type {ch_type.name} for random column data')
+    raise ValueError(f'Invalid ClickHouse type {ch_type.name} for random column data')
 
 
 def random_float():
     return (random() * random() * 65536) / (random() * (random() * 256 - 128))
 
 
 def random_float32():
@@ -107,15 +107,15 @@
     digits = ''.join(str(int(random() * 12000000000)) for _ in range(prec // 10 + 1)).rjust(prec, '0')[:prec]
     sign = '' if ord(digits[0]) & 0x01 else '-'
     if scale == 0:
         return PyDecimal(f'{sign}{digits}')
     return PyDecimal(f'{sign}{digits[:-scale]}.{digits[-scale:]}')
 
 
-def random_tuple(element_types: Sequence[DiengineType], col_def):
+def random_tuple(element_types: Sequence[ClickHouseType], col_def):
     return tuple(random_value_gen(x, col_def)() for x in element_types)
 
 
 def random_map(key_type, value_type, sz: int, col_def):
     keys = random_col_data(key_type, sz, col_def)
     values = random_col_data(value_type, sz, col_def)
     return dict(zip(keys, values))
@@ -150,26 +150,26 @@
         # multiple randoms because of random float multiply limitations
         ip_int = (int(random() * 4294967296) << 96) | (int(random() * 4294967296)) | (
                     int(random() * 4294967296) << 32) | ( int(random() * 4294967296) << 64)
         return IPv6Address(ip_int)
     return IPv4Address(int(random() * 2 ** 32))
 
 
-def random_nested(keys: Sequence[str], types: Sequence[DiengineType], col_def: RandomValueDef):
+def random_nested(keys: Sequence[str], types: Sequence[ClickHouseType], col_def: RandomValueDef):
     sz = int(random() * col_def.arr_len) // 2
     row = []
     for _ in range(sz):
         nested_element = {}
         for name, col_type in zip(keys, types):
             nested_element[name] = random_value_gen(col_type, col_def)()
         row.append(nested_element)
     return row
 
 
-gen_map: Dict[Type[DiengineType], Callable] = {
+gen_map: Dict[Type[ClickHouseType], Callable] = {
     Float64: random_float,
     Float32: random_float32,
     Date: lambda: epoch_date + timedelta(days=int(random() * 65536)),
     Date32: lambda: date32_start_date + timedelta(days=random() * 130000),
     DateTime: random_datetime,
     UUID: uuid.uuid4,
     IPv4: lambda: IPv4Address(int(random() * 4294967296)),
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/httpclient.py` & `diengine-connect-0.1.7/diengine_connect/driver/httpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from urllib3 import Timeout
 from urllib3.exceptions import HTTPError
 from urllib3.poolmanager import PoolManager
 from urllib3.response import HTTPResponse
 
 from diengine_connect import common
 from diengine_connect.datatypes import registry
-from diengine_connect.datatypes.base import DiengineType
+from diengine_connect.datatypes.base import ClickHouseType
 from diengine_connect.driver.client import Client
 from diengine_connect.driver.common import dict_copy, coerce_bool, coerce_int
 from diengine_connect.driver.compression import available_compression
 from diengine_connect.driver.exceptions import DatabaseError, OperationalError, ProgrammingError
 from diengine_connect.driver.httputil import ResponseSource, get_pool_manager, get_response_data, \
     default_pool_manager, get_proxy_manager, all_managers
 from diengine_connect.driver.insert import InsertContext
@@ -62,29 +62,29 @@
                  session_id: Optional[str] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  pool_mgr: Optional[PoolManager] = None,
                  http_proxy: Optional[str] = None,
                  https_proxy: Optional[str] = None,
                  server_host_name: Optional[str] = None):
         """
-        Create an HTTP Diengine Connect client
+        Create an HTTP ClickHouse Connect client
         See diengine_connect.get_client for parameters
         """
         self.url = f'{interface}://{host}:{port}/api/engine/v1/sql/superset'
         self.headers = {}
         ch_settings = settings or {}
         self.http = pool_mgr
         if interface == 'https':
             if not https_proxy and 'HTTPS_PROXY' in os.environ:
                 https_proxy = os.environ['HTTPS_PROXY']
             if client_cert:
                 if not username:
                     raise ProgrammingError('username parameter is required for Mutual TLS authentication')
-                self.headers['X-Diengine-User'] = username
-                self.headers['X-Diengine-SSL-Certificate-Auth'] = 'on'
+                self.headers['X-ClickHouse-User'] = username
+                self.headers['X-ClickHouse-SSL-Certificate-Auth'] = 'on'
             verify = coerce_bool(verify)
             # pylint: disable=too-many-boolean-expressions
             if not self.http and (server_host_name or ca_cert or client_cert or not verify or https_proxy):
                 options = {
                     'ca_cert': ca_cert,
                     'client_cert': client_cert,
                     'verify': verify,
@@ -173,18 +173,18 @@
             context.block_info = True
         params.update(context.bind_params)
         params.update(self._validate_settings(context.settings))
         if columns_only_re.search(context.uncommented_query):
             response = self._raw_request(f'{context.final_query}\n FORMAT JSON',
                                          params, headers, retries=self.query_retries)
             json_result = json.loads(response.data)
-            # Diengine will respond with a JSON object of meta, data, and some other objects
+            # ClickHouse will respond with a JSON object of meta, data, and some other objects
             # We just grab the column names and column types from the metadata sub object
             names: List[str] = []
-            types: List[DiengineType] = []
+            types: List[ClickHouseType] = []
             for col in json_result['meta']:
                 names.append(col['name'])
                 types.append(registry.get_from_name(col['type']))
             return QueryResult([], None, tuple(names), tuple(types))
 
         if self.compression:
             headers['Accept-Encoding'] = self.compression
@@ -198,21 +198,21 @@
                                      server_wait=not context.streaming)
         
         data = json.loads(response.data)
         query_result = self._transform.diengine_pares_response(data)
         
         # byte_source = RespBuffCls(ResponseSource(response))  # pylint: disable=not-callable
         # query_result = self._transform.parse_response(byte_source, context)
-        if 'X-Diengine-Summary' in response.headers:
+        if 'X-ClickHouse-Summary' in response.headers:
             try:
-                summary = json.loads(response.headers['X-Diengine-Summary'])
+                summary = json.loads(response.headers['X-ClickHouse-Summary'])
                 query_result.summary = summary
             except json.JSONDecodeError:
                 pass
-        query_result.query_id = response.headers.get('X-Diengine-Query-Id')
+        query_result.query_id = response.headers.get('X-ClickHouse-Query-Id')
         return query_result
 
     def data_insert(self, context: InsertContext):
         """
         See BaseClient doc_string for this method
         """
         if context.empty:
@@ -320,15 +320,15 @@
                      error_handler: Callable = None) -> HTTPResponse:
         if isinstance(data, str):
             data = data.encode()
         # headers = dict_copy(self.headers, headers)
         attempts = 0
         if server_wait:
             params['wait_end_of_query'] = '1'
-        # We can't actually read the progress headers, but we enable them so Diengine sends something
+        # We can't actually read the progress headers, but we enable them so ClickHouse sends something
         # to keep the connection alive when waiting for long-running queries and (2) to get summary information
         # if not streaming
         if self._send_progress:
             params['send_progress_in_http_headers'] = '1'
         if self._progress_interval:
             params['http_headers_progress_interval_ms'] = self._progress_interval
         url = f'{self.url}'
@@ -347,15 +347,15 @@
         while True:
             attempts += 1
             try:
                 response: HTTPResponse = self.http.request(method, url, **kwargs)
             except HTTPError as ex:
                 if isinstance(ex.__context__, ConnectionResetError):
                     # The server closed the connection, probably because the Keep Alive has expired
-                    # We should be safe to retry, as Diengine should not have processed anything on a connection
+                    # We should be safe to retry, as ClickHouse should not have processed anything on a connection
                     # that it killed.  We also only retry this once, as multiple disconnects are unlikely to be
                     # related to the Keep Alive settings
                     if attempts == 1:
                         logger.debug('Retrying remotely closed connection')
                         continue
                 logger.exception('Unexpected Http Driver Exception')
                 raise OperationalError(f'Error {ex} executing HTTP request {self.url}') from ex
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/httputil.py` & `diengine-connect-0.1.7/diengine_connect/driver/httputil.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from diengine_connect.driver.exceptions import ProgrammingError
 
 logger = logging.getLogger(__name__)
 
 # We disable this warning.  Verify must explicitly set to false, so we assume the user knows what they're doing
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-# Increase this number just to be safe when Diengine is returning progress headers
+# Increase this number just to be safe when ClickHouse is returning progress headers
 http._MAXHEADERS = 10000  # pylint: disable=protected-access
 
 DEFAULT_KEEP_INTERVAL = 30
 DEFAULT_KEEP_COUNT = 3
 DEFAULT_KEEP_IDLE = 30
 
 SOCKET_TCP = socket.IPPROTO_TCP
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/insert.py` & `diengine-connect-0.1.7/diengine_connect/driver/insert.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 from diengine_connect.driver.common import SliceView
 from diengine_connect.driver.context import BaseQueryContext
 from diengine_connect.driver.options import np, pd
 from diengine_connect.driver.exceptions import ProgrammingError
 
 if TYPE_CHECKING:
-    from diengine_connect.datatypes.base import DiengineType
+    from diengine_connect.datatypes.base import ClickHouseType
 
 
 DEFAULT_BLOCK_SIZE = 16834
 
 
 class InsertBlock(NamedTuple):
     column_count: int
     row_count: int
     column_names: Iterable[str]
-    column_types: Iterable['DiengineType']
+    column_types: Iterable['ClickHouseType']
     column_data: Iterable[Sequence[Any]]
 
 
 # pylint: disable=too-many-instance-attributes
 class InsertContext(BaseQueryContext):
     """
     Reusable Argument/parameter object for inserts.
     """
     # pylint: disable=too-many-arguments
     def __init__(self,
                  table: str,
                  column_names: Sequence[str],
-                 column_types: Sequence['DiengineType'],
+                 column_types: Sequence['ClickHouseType'],
                  data: Any = None,
                  column_oriented: Optional[bool] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  compression: Optional[Union[str, bool]] = None,
                  query_formats: Optional[Dict[str, str]] = None,
                  column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                  block_size: Optional[int] = None):
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/models.py` & `diengine-connect-0.1.7/diengine_connect/driver/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import NamedTuple
 
 from diengine_connect.datatypes.registry import get_from_name
 
 
 class ColumnDef(NamedTuple):
     """
-    Diengine column definition from DESCRIBE TABLE command
+    ClickHouse column definition from DESCRIBE TABLE command
     """
     name: str
     type: str
     default_type: str
     default_expression: str
     comment: str
     codec_expression: str
@@ -18,20 +18,20 @@
     @property
     def ch_type(self):
         return get_from_name(self.type)
 
 
 class SettingDef(NamedTuple):
     """
-    Diengine setting definition from system.settings table
+    ClickHouse setting definition from system.settings table
     """
     name: str
     value: str
     readonly: int
 
 
 class SettingStatus(NamedTuple):
     """
-    Get the setting "status" from a Diengine server setting
+    Get the setting "status" from a ClickHouse server setting
     """
     is_set: bool
     is_writable: bool
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/npquery.py` & `diengine-connect-0.1.7/diengine_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/options.py` & `diengine-connect-0.1.7/diengine_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/parser.py` & `diengine-connect-0.1.7/diengine_connect/driver/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from diengine_connect.driver.common import unescape_identifier
 
 
 # pylint: disable=too-many-branches
 def parse_callable(expr) -> Tuple[str, Tuple[Union[str, int], ...], str]:
     """
-    Parses a single level Diengine optionally 'callable' function/identifier.  The identifier is returned as the
+    Parses a single level ClickHouse optionally 'callable' function/identifier.  The identifier is returned as the
     first value in the response tuple.  If the expression is callable -- i.e. an identifier followed by 0 or more
     arguments in parentheses, the second returned value is a tuple of the comma separated arguments.  The third and
     final tuple value is any text remaining after the initial expression for further parsing/processing.
 
     Examples:
       "Tuple(String, Enum('one' = 1, 'two' = 2))" will return "Tuple", ("String", "Enum('one' = 1,'two' = 2)"), ""
       "MergeTree() PARTITION BY key" will return "MergeTree", (), "PARTITION BY key"
 
-    :param expr:  Diengine DDL or Column Name expression
+    :param expr:  ClickHouse DDL or Column Name expression
     :return: Tuple of the identifier, a tuple of arguments, and remaining text
     """
     expr = expr.strip()
     pos = expr.find('(')
     space = expr.find(' ')
     if pos == -1 and space == -1:
         return expr, (), ''
@@ -75,16 +75,16 @@
     if value != '':
         add_value()
     return name, tuple(values), expr[pos:].strip()
 
 
 def parse_enum(expr) -> Tuple[Tuple[str], Tuple[int]]:
     """
-    Parse a Diengine enum definition expression of the form ('key1' = 1, 'key2' = 2)
-    :param expr: Diengine enum expression/arguments
+    Parse a ClickHouse enum definition expression of the form ('key1' = 1, 'key2' = 2)
+    :param expr: ClickHouse enum expression/arguments
     :return: Parallel tuples of string enum keys and integer enum values
     """
     keys = []
     values = []
     pos = expr.find('(') + 1
     in_key = False
     key = []
@@ -115,17 +115,17 @@
                 value.append(char)
     values, keys = zip(*sorted(zip(values, keys)))
     return tuple(keys), tuple(values)
 
 
 def parse_columns(expr: str):
     """
-    Parse a Diengine column list of the form (col1 String, col2 Array(Tuple(String, Int32))).  This also handles
+    Parse a ClickHouse column list of the form (col1 String, col2 Array(Tuple(String, Int32))).  This also handles
     unnamed columns (such as Tuple definitions).  Mixed named and unnamed columns are not currently supported.
-    :param expr: Diengine enum expression/arguments
+    :param expr: ClickHouse enum expression/arguments
     :return: Parallel tuples of column types and column types (strings)
     """
     names = []
     columns = []
     pos = 1
     named = False
     level = 0
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/query.py` & `diengine-connect-0.1.7/diengine_connect/driver/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,29 @@
                  as_pandas: bool = False,
                  streaming: bool = False):
         """
         Initializes various configuration settings for the query context
 
         :param query:  Query string with Python style format value replacements
         :param parameters: Optional dictionary of substitution values
-        :param settings: Optional Diengine settings for the query
-        :param query_formats: Optional dictionary of query formats with the key of a Diengine type name
+        :param settings: Optional ClickHouse settings for the query
+        :param query_formats: Optional dictionary of query formats with the key of a ClickHouse type name
           (with * wildcards) and a value of valid query formats for those types.
           The value 'encoding' can be sent to change the expected encoding for this query, with a value of
           the desired encoding such as `latin-1`
         :param column_formats: Optional dictionary of column specific formats.  The key is the column name,
           The value is either the format for the data column (such as 'string' for a UUID column) or a
-          second level "format" dictionary of a Diengine type name and a value of query formats.  This
+          second level "format" dictionary of a ClickHouse type name and a value of query formats.  This
           secondary dictionary can be used for nested column types such as Tuples or Maps
         :param encoding: Optional string encoding for this query, such as 'latin-1'
         :param column_formats: Optional dictionary
-        :param use_none: Use a Python None for Diengine NULL values in nullable columns.  Otherwise the default
+        :param use_none: Use a Python None for ClickHouse NULL values in nullable columns.  Otherwise the default
           value of the column (such as 0 for numbers) will be returned in the result_set
-        :param max_str_len Limit returned Diengine String values to this length, which allows a Numpy
-          structured array even with Diengine variable length String columns.  If 0, Numpy arrays for
+        :param max_str_len Limit returned ClickHouse String values to this length, which allows a Numpy
+          structured array even with ClickHouse variable length String columns.  If 0, Numpy arrays for
           String columns will always be object arrays
         :param query_tz  Either a string or a pytz tzinfo object.  (Strings will be converted to tzinfo objects).
           Values for any DateTime or DateTime64 column in the query will be converted to Python datetime.datetime
           objects with the selected timezone
         :param column_tzs A dictionary of column names to tzinfo objects (or strings that will be converted to
           tzinfo objects).  The timezone will be applied to datetime objects returned in the query
         """
@@ -371,15 +371,15 @@
 def format_str(value: str):
     return f"'{''.join(f'{BS}{c}' if c in must_escape else c for c in value)}'"
 
 
 # pylint: disable=too-many-return-statements
 def format_query_value(value: Any, server_tz: tzinfo = pytz.UTC):
     """
-    Format Python values in a Diengine query
+    Format Python values in a ClickHouse query
     :param value: Python object
     :param server_tz: Server timezone for adjusting datetime values
     :return: Literal string for python value
     """
     if value is None:
         return 'NULL'
     if isinstance(value, str):
@@ -405,15 +405,15 @@
     if isinstance(value, (uuid.UUID, ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return f"'{value}'"
     return str(value)
 
 
 def format_bind_value(value: Any, server_tz: tzinfo = pytz.UTC):
     """
-    Format Python values in a Diengine query
+    Format Python values in a ClickHouse query
     :param value: Python object
     :param server_tz: Server timezone for adjusting datetime values
     :return: Literal string for python value
     """
     if value is None:
         return 'NULL'
     if isinstance(value, datetime):
@@ -440,15 +440,15 @@
 comment_re = re.compile(r"(\".*?\"|\'.*?\')|(/\*.*?\*/|(--\s)[^\n]*$)", re.MULTILINE | re.DOTALL)
 
 
 def remove_sql_comments(sql: str) -> str:
     """
     Remove SQL comments.  This is useful to determine the type of SQL query, such as SELECT or INSERT, but we
     don't fully trust it to correctly ignore weird quoted strings, and other edge cases, so we always pass the
-    original SQL to Diengine (which uses a full-fledged AST/ token parser)
+    original SQL to ClickHouse (which uses a full-fledged AST/ token parser)
     :param sql:  SQL query
     :return: SQL Query without SQL comments
     """
 
     def replacer(match):
         # if the 2nd group (capturing comments) is not None, it means we have captured a
         # non-quoted, actual comment string, so return nothing to remove the comment
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/tools.py` & `diengine-connect-0.1.7/diengine_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/transform.py` & `diengine-connect-0.1.7/diengine_connect/driver/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                         col_type = col_types[col_num]
                     context.start_column(name)
                     column = col_type.read_column(source, num_rows, context)
                     result_block.append(column)
             except Exception as ex:
                 source.close()
                 if isinstance(ex, StreamCompleteException):
-                    # We ran out of data before it was expected, this could be Diengine reporting an error
+                    # We ran out of data before it was expected, this could be ClickHouse reporting an error
                     # in the response
                     message = source.last_message
                     if len(message) > 1024:
                         message = message[-1024:]
                     error_start = message.find('Code: ')
                     if error_start != -1:
                         message = message[error_start:]
```

### Comparing `diengine-connect-0.0.3/diengine_connect/driver/types.py` & `diengine-connect-0.1.7/diengine_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/entry_points.py` & `diengine-connect-0.1.7/diengine_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect/json_impl.py` & `diengine-connect-0.1.7/diengine_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/diengine_connect.egg-info/PKG-INFO` & `diengine-connect-0.1.7/diengine_connect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.0.3
+Version: 0.1.7
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
-        A suite of Python packages for connecting Python to Diengine:
+        A suite of Python packages for connecting Python to ClickHouse:
         * Pandas DataFrames
         * Numpy Arrays
         * PyArrow Tables
         * SQLAlchemy 1.3 and 1.4 (limited feature set)
         * Apache Superset 1.4+
```

### Comparing `diengine-connect-0.0.3/diengine_connect.egg-info/SOURCES.txt` & `diengine-connect-0.1.7/diengine_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.3/setup.py` & `diengine-connect-0.1.7/setup.py`

 * *Files identical despite different names*

