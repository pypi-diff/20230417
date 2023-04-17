# Comparing `tmp/tentaclio-1.1.0.tar.gz` & `tmp/tentaclio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentaclio-1.1.0.tar", last modified: Wed Apr  5 14:02:29 2023, max compression
+gzip compressed data, was "tentaclio-1.2.0.tar", last modified: Mon Apr 17 08:08:08 2023, max compression
```

## Comparing `tentaclio-1.1.0.tar` & `tentaclio-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.097017 tentaclio-1.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-05 14:02:06.000000 tentaclio-1.1.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-05 14:02:29.097017 tentaclio-1.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10286 2023-04-05 14:02:06.000000 tentaclio-1.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-04-05 14:02:29.105017 tentaclio-1.1.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2445 2023-04-05 14:02:06.000000 tentaclio-1.1.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.089017 tentaclio-1.1.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/__main__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/clients/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/base_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      703 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7290 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/ftp_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5512 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/http_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/importer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/local_fs_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5320 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/clients/sqla_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/credentials/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      143 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/credentials/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/credentials/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/credentials/env.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4774 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/credentials/injection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3214 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/credentials/reader.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/databases/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/databases/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/databases/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1366 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/databases/db_registry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/fs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/copier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/copiers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/remover.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/scanner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/fs/scanners.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1260 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/hooks/slack_hook.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/protocols.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/registry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio/streams/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2383 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7856 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/base_stream.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/csv_db_stream.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/stream_client_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2657 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/streams/stream_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4923 2023-04-05 14:02:06.000000 tentaclio-1.1.0/src/tentaclio/urls.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-05 14:02:29.093017 tentaclio-1.1.0/src/tentaclio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-05 14:02:28.000000 tentaclio-1.1.0/src/tentaclio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2023-04-05 14:02:29.000000 tentaclio-1.1.0/src/tentaclio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-05 14:02:28.000000 tentaclio-1.1.0/src/tentaclio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2023-04-05 14:02:28.000000 tentaclio-1.1.0/src/tentaclio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-05 14:02:28.000000 tentaclio-1.1.0/src/tentaclio.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-17 08:07:46.000000 tentaclio-1.2.0/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-17 08:08:08.558878 tentaclio-1.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10286 2023-04-17 08:07:46.000000 tentaclio-1.2.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-04-17 08:08:08.558878 tentaclio-1.2.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2445 2023-04-17 08:07:46.000000 tentaclio-1.2.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/__main__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio/clients/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/base_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      703 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7320 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/ftp_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/http_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/importer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/local_fs_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5487 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/sqla_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/credentials/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      143 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/env.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4774 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/injection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3214 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/reader.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/databases/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1366 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/db_registry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/fs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/copier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/copiers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/remover.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/scanner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/scanners.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1406 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/hooks/slack_hook.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/protocols.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/registry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/streams/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2403 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7856 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/base_stream.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/csv_db_stream.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/stream_client_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2657 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/stream_registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5212 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/urls.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/top_level.txt
```

### Comparing `tentaclio-1.1.0/LICENSE.txt` & `tentaclio-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/PKG-INFO` & `tentaclio-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentaclio
-Version: 1.1.0
+Version: 1.2.0
 Summary: Unification of data connectors for distributed data tasks
 Home-page: https://github.com/octoenergy/tentaclio
 Author: Octopus Energy
 Author-email: nerds@octoenergy.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tentaclio-1.1.0/README.md` & `tentaclio-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/setup.cfg` & `tentaclio-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/setup.py` & `tentaclio-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 import sys
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 
 REPO_ROOT = pathlib.Path(__file__).parent
 
 with open(REPO_ROOT / "README.md", encoding="utf-8") as f:
     README = f.read()
```

### Comparing `tentaclio-1.1.0/src/tentaclio/__init__.py` & `tentaclio-1.2.0/src/tentaclio/__init__.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/__main__.py` & `tentaclio-1.2.0/src/tentaclio/__main__.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/base_client.py` & `tentaclio-1.2.0/src/tentaclio/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/decorators.py` & `tentaclio-1.2.0/src/tentaclio/clients/decorators.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/ftp_client.py` & `tentaclio-1.2.0/src/tentaclio/clients/ftp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         conn.connect(self.url.hostname or "", port=self.port)
         conn.login(user=self.url.username or "", passwd=self.url.password or "")
         return conn
 
     # Stream methods:
 
     @decorators.check_conn
-    def get(self, writer: protocols.ByteWriter, file_path: str = None) -> None:
+    def get(self, writer: protocols.ByteWriter, file_path: Optional[str] = None) -> None:
         """Write the contents of a remote file into the passed writer.
 
         Arguments:
             :file_path: The path of the remote file if not passed
                 in the costructor as part of the url.
         """
         remote_path = file_path or self.url.path
@@ -158,15 +158,15 @@
             cnopts=cnopts,
             port=self.port,
         )
 
     # Stream methods:
 
     @decorators.check_conn
-    def get(self, writer: protocols.ByteWriter, file_path: str = None) -> None:
+    def get(self, writer: protocols.ByteWriter, file_path: Optional[str] = None) -> None:
         """Write the contents of a remote file into the passed writer.
 
         Arguments:
             :file_path: The path of the remote file if not passed
                 in the costructor as part of the url.
         """
         remote_path = file_path or self.url.path
@@ -176,15 +176,15 @@
         if not self.conn.isfile(remote_path):
             raise exceptions.FTPError("Unable to fetch the remote file")
 
         logger.info(f"sftp reading from {remote_path}")
         self.conn.getfo(remote_path, writer)
 
     @decorators.check_conn
-    def put(self, reader: protocols.ByteReader, file_path: str = None) -> None:
+    def put(self, reader: protocols.ByteReader, file_path: Optional[str] = None) -> None:
         """Write the contents of the reader into the remote file.
 
         Arguments:
             :file_path: The path of the remote file if not passed
                 in the costructor as part of the url.
         """
         remote_path = file_path or self.url.path
```

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/http_client.py` & `tentaclio-1.2.0/src/tentaclio/clients/http_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,15 +34,18 @@
     username: Optional[str]
     password: Optional[str]
     hostname: str
     port: Optional[int]
     endpoint: str
 
     def __init__(
-        self, url: str, default_timeout: float = None, default_headers: dict = None
+        self,
+        url: str,
+        default_timeout: Optional[float] = None,
+        default_headers: Optional[dict] = None,
     ) -> None:
         """Create a new http/https client based on the passed url and extra params."""
         # Default connection timeout at 10''
         self.timeout = default_timeout or DEFAULT_TIMEOUT
         # Default JSON response back
         self.headers = default_headers or DEFAULT_HEADERS
         super().__init__(url)
@@ -77,17 +80,17 @@
 
     # Stream methods:
 
     @decorators.check_conn
     def get(
         self,
         writer: protocols.ByteWriter,
-        endpoint: str = None,
-        params: dict = None,
-        options: dict = None,
+        endpoint: Optional[str] = None,
+        params: Optional[dict] = None,
+        options: Optional[dict] = None,
     ) -> None:
         """Read the contents from the url and write them into the provided writer.
 
         Arguments:
             :end_point: Path to append to the url passed in the constructor.
             :params: Url params to add
             :options: More options for the request library.
@@ -99,17 +102,17 @@
 
         writer.write(response.content)
 
     @decorators.check_conn
     def put(
         self,
         reader: protocols.ByteReader,
-        endpoint: str = None,
-        params: dict = None,
-        options: dict = None,
+        endpoint: Optional[str] = None,
+        params: Optional[dict] = None,
+        options: Optional[dict] = None,
     ) -> None:
         """Write the contents of the provided reader into the url using POST.
 
         Arguments:
             :end_point: Path to append to the url passed in the constructor.
             :params: Url params to add
             :options: More options for the request library.
@@ -128,16 +131,16 @@
         base_url = parse.urlunparse((self.protocol, self.hostname, self.endpoint, "", "", ""))
         return parse.urljoin(base_url, endpoint)
 
     def _build_request(
         self,
         method: str,
         url: str,
-        default_data: protocols.Reader = None,
-        default_params: dict = None,
+        default_data: Optional[protocols.Reader] = None,
+        default_params: Optional[dict] = None,
     ):
         data: Union[protocols.Reader, list] = default_data or []
         params = default_params or {}
 
         if method == "GET":
             # GET uses params
             request = requests.Request(method, url, params=params, headers=self.headers)
@@ -145,15 +148,17 @@
             # POST uses data & params
             request = requests.Request(method, url, data=data, params=params, headers=self.headers)
         else:
             raise NotImplementedError
 
         return self.conn.prepare_request(request)
 
-    def _send_request(self, request: requests.PreparedRequest, default_options: dict = None):
+    def _send_request(
+        self, request: requests.PreparedRequest, default_options: Optional[dict] = None
+    ):
         options = default_options or {}
 
         response = self.conn.send(
             request,
             stream=options.get("stream", False),
             verify=options.get("verify", False),
             proxies=options.get("proxies", {}),
```

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/importer.py` & `tentaclio-1.2.0/src/tentaclio/clients/importer.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/local_fs_client.py` & `tentaclio-1.2.0/src/tentaclio/clients/local_fs_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/clients/sqla_client.py` & `tentaclio-1.2.0/src/tentaclio/clients/sqla_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 This client is used for convinience when using different sql
 providers and unifying the client creation. We do not intent to rewriter sqlalchemy.
 """
 import contextlib
 from typing import Container, Generator, Optional, Union
 
 import pandas as pd
+from sqlalchemy import text
 from sqlalchemy.engine import Connection, CursorResult, Engine, create_engine
-from sqlalchemy.engine import url as sqla_url
+from sqlalchemy.engine.url import URL as sqla_url
 from sqlalchemy.orm import session, sessionmaker
 from sqlalchemy.sql.schema import MetaData
 
 from tentaclio import urls
 
 from . import base_client, decorators
 
 
 __all__ = ["SQLAlchemyClient", "bound_session", "atomic_session"]
 
 
-SessionGenerator = Generator[None, session.Session, None]
+SessionGenerator = Generator[session.Session, None, None]
 
 
 class _TrueContainer(Container[str]):
     """String container that always returns true.
 
     As we don't have control over the protocols that sqlalchemy is able to
     accept. We shouldn't try to limit which urls can be used here or not.
@@ -53,15 +54,18 @@
     drivername: str
     username: Optional[str]
     password: Optional[str]
     host: Optional[str]
     port: Optional[int]
 
     def __init__(
-        self, url: Union[str, urls.URL], execution_options: dict = None, connect_args: dict = None
+        self,
+        url: Union[str, urls.URL],
+        execution_options: Optional[dict] = None,
+        connect_args: Optional[dict] = None,
     ) -> None:
         """Create sqlalchemy client based on the passed url.
 
         This is a wrapper for sqlalchemy engine/connection creation.
         """
         self.execution_options = execution_options or {}
         self.connect_args = connect_args or self.connect_args_default
@@ -80,24 +84,24 @@
         self.host = self.url.hostname
         self.port = self.url.port
         self.url_query = self.url.query
 
     # Connection methods:
 
     def _connect(self) -> Connection:
-
-        parsed_url = sqla_url.URL(
+        parsed_url = sqla_url.create(
             drivername=self.drivername,
             username=self.username,
             password=self.password,
             host=self.host,
             port=self.port,
             database=self.database,
-            query=self.url_query,
         )
+        if self.url.query_string:
+            parsed_url.update_query_string(self.url.query_string)
         if self.engine is None:
             self.engine = create_engine(
                 parsed_url,
                 execution_options=self.execution_options,
                 connect_args=self.connect_args,
             )
         return self.engine.connect()
@@ -120,32 +124,32 @@
 
     @decorators.check_conn
     def query(self, sql_query: str, **kwargs) -> CursorResult:
         """Execute a read-only SQL query, and return results.
 
         This will not commit any changes to the database.
         """
-        return self.conn.execute(sql_query, **kwargs)
+        return self.conn.execute(text(sql_query), **kwargs)
 
     @decorators.check_conn
     def execute(self, sql_query: str, **kwargs) -> None:
         """Execute a raw SQL query command."""
         trans = self.conn.begin()
         try:
-            self.conn.execute(sql_query, **kwargs)
+            self.conn.execute(text(sql_query), **kwargs)
         except Exception:
             trans.rollback()
             raise
         else:
             trans.commit()
 
     # Dataframe methods:
 
     @decorators.check_conn
-    def get_df(self, sql_query: str, params: dict = None, **kwargs) -> pd.DataFrame:
+    def get_df(self, sql_query: str, params: Optional[dict] = None, **kwargs) -> pd.DataFrame:
         """Run a raw SQL query and return a data frame."""
         return pd.read_sql(sql_query, self.conn, params=params, **kwargs)
 
 
 # Session context managers:
```

### Comparing `tentaclio-1.1.0/src/tentaclio/credentials/api.py` & `tentaclio-1.2.0/src/tentaclio/credentials/api.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/credentials/env.py` & `tentaclio-1.2.0/src/tentaclio/credentials/env.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/credentials/injection.py` & `tentaclio-1.2.0/src/tentaclio/credentials/injection.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/credentials/reader.py` & `tentaclio-1.2.0/src/tentaclio/credentials/reader.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/databases/db_registry.py` & `tentaclio-1.2.0/src/tentaclio/databases/db_registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/api.py` & `tentaclio-1.2.0/src/tentaclio/fs/api.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/copier.py` & `tentaclio-1.2.0/src/tentaclio/fs/copier.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/copiers.py` & `tentaclio-1.2.0/src/tentaclio/fs/copiers.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/remover.py` & `tentaclio-1.2.0/src/tentaclio/fs/remover.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/scanner.py` & `tentaclio-1.2.0/src/tentaclio/fs/scanner.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/fs/scanners.py` & `tentaclio-1.2.0/src/tentaclio/fs/scanners.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/hooks/slack_hook.py` & `tentaclio-1.2.0/src/tentaclio/hooks/slack_hook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Slack http hook."""
 import io
 import json
+from typing import Optional
 
 from tentaclio.clients import http_client
 
 
 __all__ = ["SlackHook"]
 
 
@@ -12,30 +13,37 @@
     """Slack incoming web hook (POST messages)."""
 
     def __init__(self, url: str) -> None:
         """Create a slack hook that connects to the given url."""
         self.url = url
 
     def notify(
-        self, message: str, channel: str = None, username: str = None, icon_emoji: str = None
+        self,
+        message: str,
+        channel: Optional[str] = None,
+        username: Optional[str] = None,
+        icon_emoji: Optional[str] = None,
     ) -> None:
         """Send a notification to slack."""
         body = self._build_request_body(
             message, channel=channel, username=username, icon_emoji=icon_emoji
         )
         stream = io.BytesIO(bytes(body, encoding="utf-8"))
         # Post streamed request
         with http_client.HTTPClient(self.url) as client:
             client.put(stream)
 
     # Helpers:
 
     @staticmethod
     def _build_request_body(
-        message: str, channel: str = None, username: str = None, icon_emoji: str = None
+        message: str,
+        channel: Optional[str] = None,
+        username: Optional[str] = None,
+        icon_emoji: Optional[str] = None,
     ) -> str:
         # Fetch message payload
         payload = dict(text=message)
         if channel:
             payload["channel"] = channel
         if username:
             payload["username"] = username
```

### Comparing `tentaclio-1.1.0/src/tentaclio/protocols.py` & `tentaclio-1.2.0/src/tentaclio/protocols.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/registry.py` & `tentaclio-1.2.0/src/tentaclio/registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/streams/api.py` & `tentaclio-1.2.0/src/tentaclio/streams/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Main entry points to tentaclio-io."""
-from typing import ContextManager, Union
+from typing import ContextManager, Optional, Union
 
 from tentaclio import protocols
 from tentaclio.credentials import authenticate
 
 from .base_stream import DirtyStreamerWriter, StreamerReader, StreamerWriter
 from .stream_registry import STREAM_HANDLER_REGISTRY, _WriterContextManager
 
@@ -13,15 +13,15 @@
 VALID_MODES = ("", "rb", "wb", "rt", "wt", "r", "w", "b", "t")
 
 AnyContextStreamerReaderWriter = Union[
     ContextManager[StreamerReader], ContextManager[StreamerWriter]
 ]
 
 
-def open(url: str, mode: str = None, **kwargs) -> AnyContextStreamerReaderWriter:
+def open(url: str, mode: Optional[str] = None, **kwargs) -> AnyContextStreamerReaderWriter:
     """Open a url and return a reader or writer depending on mode.
 
     Arguments:
         :mode: similar to built-in open, allowed modes are combinations of "w" for writing
         "r" for reading. "t" for text resources, and "b" for binary. The default is "rt".
     Examples:
         >>> open(path, 'b')  # opens binary reader
```

### Comparing `tentaclio-1.1.0/src/tentaclio/streams/base_stream.py` & `tentaclio-1.2.0/src/tentaclio/streams/base_stream.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/streams/csv_db_stream.py` & `tentaclio-1.2.0/src/tentaclio/streams/csv_db_stream.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/streams/stream_client_handler.py` & `tentaclio-1.2.0/src/tentaclio/streams/stream_client_handler.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/streams/stream_registry.py` & `tentaclio-1.2.0/src/tentaclio/streams/stream_registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.1.0/src/tentaclio/urls.py` & `tentaclio-1.2.0/src/tentaclio/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     _scheme: str
     _username: Optional[str] = None
     _password: Optional[str] = None
     _hostname: Optional[str] = None
     _port: Optional[int] = None
     _path: str
     _query: Optional[Dict[str, str]] = None
+    _query_string: Optional[str] = None
 
     def __init__(self, url: str) -> None:
         """Create a url by parsing the parametre."""
         self._url = url
         self._parse_url()
 
     # Helpers:
@@ -53,14 +54,15 @@
 
         self._scheme = parsed_url.scheme
         self._username = parsed_url.username
         self._password = parsed_url.password
         self._hostname = parsed_url.hostname
         self._port = parsed_url.port
         self._path = parsed_url.path
+        self._query_string = parsed_url.query
 
         # Replace %xx escapes - ONLY for username & password
         if parsed_url.username and self._username:
             self._username = parse.unquote(self._username)
         if parsed_url.password and self._password:
             self._password = parse.unquote(self._password)
 
@@ -70,21 +72,21 @@
                 key: value for key, value in parse.parse_qsl(parsed_url.query, strict_parsing=True)
             }
         else:
             self._query = None
 
     def copy(
         self,
-        scheme: str = None,
-        username: str = None,
-        password: str = None,
-        hostname: str = None,
-        port: int = None,
-        path: str = None,
-        query: str = None,
+        scheme: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        hostname: Optional[str] = None,
+        port: Optional[int] = None,
+        path: Optional[str] = None,
+        query: Optional[str] = None,
     ) -> "URL":
         """Copy this url optionally overwriting the provided components."""
         return URL.from_components(
             scheme=scheme or self.scheme,
             username=username or self.username,
             password=password or self.password,
             hostname=hostname or self.hostname,
@@ -165,10 +167,15 @@
 
     @property
     def query(self) -> Optional[Dict[str, str]]:
         """Access the query."""
         return self._query
 
     @property
+    def query_string(self) -> Optional[str]:
+        """Access the query string."""
+        return self._query_string
+
+    @property
     def url(self) -> str:
         """Return the original url."""
         return self._url
```

### Comparing `tentaclio-1.1.0/src/tentaclio.egg-info/PKG-INFO` & `tentaclio-1.2.0/src/tentaclio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentaclio
-Version: 1.1.0
+Version: 1.2.0
 Summary: Unification of data connectors for distributed data tasks
 Home-page: https://github.com/octoenergy/tentaclio
 Author: Octopus Energy
 Author-email: nerds@octoenergy.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tentaclio-1.1.0/src/tentaclio.egg-info/SOURCES.txt` & `tentaclio-1.2.0/src/tentaclio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

