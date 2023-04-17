# Comparing `tmp/aegis-tools-2.1.0.tar.gz` & `tmp/aegis-tools-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.0.tar", last modified: Tue Apr  4 23:23:21 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.2.tar", last modified: Mon Apr 17 16:13:28 2023, max compression
```

## Comparing `aegis-tools-2.1.0.tar` & `aegis-tools-2.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-04 23:23:21.594454 aegis-tools-2.1.0/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-04 23:23:21.590454 aegis-tools-2.1.0/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-04 23:23:21.578454 aegis-tools-2.1.0/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.0/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.0/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.0/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.0/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.0/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     6919 2023-04-04 23:19:50.000000 aegis-tools-2.1.0/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    41877 2023-04-04 03:38:47.000000 aegis-tools-2.1.0/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-04 23:23:21.582454 aegis-tools-2.1.0/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.0/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.0/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.0/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.0/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.0/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-02 17:41:52.000000 aegis-tools-2.1.0/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-04 23:23:21.590454 aegis-tools-2.1.0/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.0/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.0/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.0/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.0/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-03-26 04:29:07.000000 aegis-tools-2.1.0/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.0/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.0/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.0/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.0/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.0/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.0/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.0/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.0/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.0/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73082 2023-04-04 23:20:35.000000 aegis-tools-2.1.0/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-04 23:23:21.590454 aegis-tools-2.1.0/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-04-04 23:23:21.000000 aegis-tools-2.1.0/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-04-04 23:23:21.594454 aegis-tools-2.1.0/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-04-04 23:22:24.000000 aegis-tools-2.1.0/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.593039 aegis-tools-2.1.2/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.2/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.2/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.2/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.2/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.2/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     6919 2023-04-04 23:19:50.000000 aegis-tools-2.1.2/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42189 2023-04-17 16:11:36.000000 aegis-tools-2.1.2/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.601039 aegis-tools-2.1.2/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.2/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.2/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.2/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.2/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.2/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-02 17:41:52.000000 aegis-tools-2.1.2/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.609039 aegis-tools-2.1.2/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.2/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.2/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.2/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.2/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-03-26 04:29:07.000000 aegis-tools-2.1.2/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.2/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.2/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.2/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.2/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.2/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.2/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.2/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.2/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73096 2023-04-14 17:14:23.000000 aegis-tools-2.1.2/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.609039 aegis-tools-2.1.2/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-04-17 16:13:05.000000 aegis-tools-2.1.2/setup.py
```

### Comparing `aegis-tools-2.1.0/LICENSE` & `aegis-tools-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/PKG-INFO` & `aegis-tools-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.0
+Version: 2.1.2
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.0/README.md` & `aegis-tools-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/aegis_.py` & `aegis-tools-2.1.2/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/build.py` & `aegis-tools-2.1.2/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/config.py` & `aegis-tools-2.1.2/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/database.py` & `aegis-tools-2.1.2/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/hydra.py` & `aegis-tools-2.1.2/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/mailer.py` & `aegis-tools-2.1.2/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/model.py` & `aegis-tools-2.1.2/aegis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,20 @@
             sql += ' RETURNING email_id'
         return db().execute(sql, email)
 
     @classmethod
     def set_email(cls, email):
         email_row = cls.get_email(email)
         if not email_row:
-            email_id = cls.insert(email)
-            email_row = cls.get_id(email_id)
+            try:
+                email_id = cls.insert(email)
+                email_row = cls.get_id(email_id)
+            except (aegis.database.PgsqlUniqueViolation, aegis.database.MysqlIntegrityError) as ex:
+                logging.error("Duplicate Key Error   aegis.model.Email.set_email(%s). Very unlikely. Read from DB and carry one.", email)
+                email_row = cls.get_email(email)
         return email_row
 
     @classmethod
     def get_email(cls, email):
         sql = "SELECT * FROM email WHERE email=%s"
         return db().get(sql, email, cls=cls)
```

### Comparing `aegis-tools-2.1.0/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.2/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.2/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.2/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.2/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.2/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/google_signin.sql` & `aegis-tools-2.1.2/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.2/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.2/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/member_auth.sql` & `aegis-tools-2.1.2/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.2/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/sql/reports.sql` & `aegis-tools-2.1.2/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/stdlib.py` & `aegis-tools-2.1.2/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/build.html` & `aegis-tools-2.1.2/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/build_confirm.html` & `aegis-tools-2.1.2/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/build_form.html` & `aegis-tools-2.1.2/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/build_view.html` & `aegis-tools-2.1.2/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/frame.html` & `aegis-tools-2.1.2/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/hydra.html` & `aegis-tools-2.1.2/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/hydra_form.html` & `aegis-tools-2.1.2/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.2/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/report.html` & `aegis-tools-2.1.2/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/report_form.html` & `aegis-tools-2.1.2/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/reports.html` & `aegis-tools-2.1.2/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/templates/w3.css` & `aegis-tools-2.1.2/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/threadpool.py` & `aegis-tools-2.1.2/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/aegis/webapp.py` & `aegis-tools-2.1.2/aegis/webapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
             logging.warning("Pyreferrer type is social -> social")
             return self.finish_marketing('social')
         aegis.stdlib.logw(pr, "Pyreferrer")
         # Custom organic "netlocs" not (yet) in pyreferrer
         organic_netlocs = ['aol.com', 'baidu.com', 'www.daum.net', 'daum.net', 'search.brave.com', 'www.ecosia.org', 'www.msn.com',
                            'com.google.android.googlequicksearchbox']   # android-app://com.google.android.googlequicksearchbox
         for organic_netloc in organic_netlocs:
-            if url_parts.netloc.endswith(organic_netloc):
+            if url_parts and url_parts.netloc.endswith(organic_netloc):
                 logging.warning("Netloc endswith organic domain -> organic")
                 return self.finish_marketing('organic')
         # Mark it as an unknown referral
         logging.warning("Url unknown: %s" % referer)
         return self.finish_marketing('referral')
 
     def finish_marketing(self, marketing_name):
```

### Comparing `aegis-tools-2.1.0/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.2/aegis_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.0
+Version: 2.1.2
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.0/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.2/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.0/setup.py` & `aegis-tools-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.0',
+    version = '2.1.2',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

